# Comparing `tmp/databased-1.4.5.tar.gz` & `tmp/databased-1.5.0.tar.gz`

## Comparing `databased-1.4.5.tar` & `databased-1.5.0.tar`

### file list

```diff
@@ -1,14 +1,18 @@
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 databased-1.4.5/CHANGELOG.md
--rw-r--r--   0        0        0    34261 2020-02-02 00:00:00.000000 databased-1.4.5/docs/databased.html
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 databased-1.4.5/docs/index.html
--rw-r--r--   0        0        0    46828 2020-02-02 00:00:00.000000 databased-1.4.5/docs/search.js
--rw-r--r--   0        0        0   415769 2020-02-02 00:00:00.000000 databased-1.4.5/docs/databased/databased.html
--rw-r--r--   0        0        0   157452 2020-02-02 00:00:00.000000 databased-1.4.5/docs/databased/dbmanager.html
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 databased-1.4.5/src/databased/__init__.py
--rw-r--r--   0        0        0    21395 2020-02-02 00:00:00.000000 databased-1.4.5/src/databased/databased.py
--rw-r--r--   0        0        0     9680 2020-02-02 00:00:00.000000 databased-1.4.5/src/databased/dbmanager.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 databased-1.4.5/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 databased-1.4.5/LICENSE.txt
--rw-r--r--   0        0        0     7471 2020-02-02 00:00:00.000000 databased-1.4.5/README.md
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 databased-1.4.5/pyproject.toml
--rw-r--r--   0        0        0     8125 2020-02-02 00:00:00.000000 databased-1.4.5/PKG-INFO
+-rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 databased-1.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0    34888 2020-02-02 00:00:00.000000 databased-1.5.0/docs/databased.html
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 databased-1.5.0/docs/index.html
+-rw-r--r--   0        0        0    60821 2020-02-02 00:00:00.000000 databased-1.5.0/docs/search.js
+-rw-r--r--   0        0        0    44509 2020-02-02 00:00:00.000000 databased-1.5.0/docs/databased/custom_manager.html
+-rw-r--r--   0        0        0   406809 2020-02-02 00:00:00.000000 databased-1.5.0/docs/databased/databased.html
+-rw-r--r--   0        0        0   280216 2020-02-02 00:00:00.000000 databased-1.5.0/docs/databased/dbmanager.html
+-rw-r--r--   0        0        0   101086 2020-02-02 00:00:00.000000 databased-1.5.0/docs/databased/dbparsers.html
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 databased-1.5.0/src/databased/__init__.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 databased-1.5.0/src/databased/custom_manager.py
+-rw-r--r--   0        0        0    20869 2020-02-02 00:00:00.000000 databased-1.5.0/src/databased/databased.py
+-rw-r--r--   0        0        0    12433 2020-02-02 00:00:00.000000 databased-1.5.0/src/databased/dbmanager.py
+-rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 databased-1.5.0/src/databased/dbparsers.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 databased-1.5.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 databased-1.5.0/LICENSE.txt
+-rw-r--r--   0        0        0     7323 2020-02-02 00:00:00.000000 databased-1.5.0/README.md
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 databased-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     8010 2020-02-02 00:00:00.000000 databased-1.5.0/PKG-INFO
```

### Comparing `databased-1.4.5/CHANGELOG.md` & `databased-1.5.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,68 @@
 # Changelog
 
-## 1.4.4 (2023-04-02)
+## 1.5.0 (2023-04-27)
+
+#### New Features
+
+##### dbmanager
+* add do_add_row()
+* add functionality to add a row to database
+* add do_drop_table()
+* add do_create_table()
+* add parser to add a table
+* add do_search()
+* add get_search_parser()
+* add do_flush_log()
+* add do_customize()
+* add do_size()
+* add do_delete()
+* add get_update_parser()
+* add do_update()
+* add do_query()
+* add partial_matching flag to parser
+* add do_count()
+* add limit arg to parser
+* add order_by arg to parser
+* add do_backup
+
+#### Refactorings
+
+* delete create_manager()
+* replace dbmanager content with argshell version
+* implement usage of argshell package
+#### Docs
+
+* improve type annotations
+* update readme
+* fix doc string
+## v1.4.5 (2023-04-03)
+
+#### Fixes
+
+* fix condition causing infinite loop in data_to_string
+#### Refactorings
+
+* add print statements to data_to_string
+* remove uneeded lambda in data_to_string
+#### Others
+
+* build v1.4.5
+* update changelog
+
+
+## v1.4.4 (2023-04-02)
 
 #### Fixes
 
 * return statement was indented one level too many
+#### Others
+
+* build v1.4.4
+* update changelog
 
 
 ## v1.4.3 (2023-04-02)
 
 #### Performance improvements
 
 * rewrite data_to_string() with a different resizing algo
```

### Comparing `databased-1.4.5/docs/databased.html` & `databased-1.5.0/docs/databased.html`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,18 @@
 
             <input type="search" placeholder="Search..." role="searchbox" aria-label="search"
                    pattern=".+" required>
 
 
         <h2>Submodules</h2>
         <ul>
+                <li><a href="databased/custom_manager.html">custom_manager</a></li>
                 <li><a href="databased/databased.html">databased</a></li>
                 <li><a href="databased/dbmanager.html">dbmanager</a></li>
+                <li><a href="databased/dbparsers.html">dbparsers</a></li>
         </ul>
 
 
 
         <a class="attribution" title="pdoc: Python API documentation generator" href="https://pdoc.dev" target="_blank">
             built with <span class="visually-hidden">pdoc</span><img
                 alt="pdoc logo"
@@ -43,15 +45,18 @@
 databased    </h1>
 
                 
                         <input id="mod-databased-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 
                         <label class="view-source-button" for="mod-databased-view-source"><span>View Source</span></label>
 
-                        <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos">1</span></a><span class="kn">from</span> <span class="nn">.databased</span> <span class="kn">import</span> <span class="n">DataBased</span><span class="p">,</span> <span class="n">_connect</span><span class="p">,</span> <span class="n">data_to_string</span>
+                        <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos">1</span></a><span class="kn">from</span> <span class="nn">databased</span> <span class="kn">import</span> <span class="n">dbparsers</span>
+</span><span id="L-2"><a href="#L-2"><span class="linenos">2</span></a>
+</span><span id="L-3"><a href="#L-3"><span class="linenos">3</span></a><span class="kn">from</span> <span class="nn">.databased</span> <span class="kn">import</span> <span class="n">DataBased</span><span class="p">,</span> <span class="n">_connect</span><span class="p">,</span> <span class="n">data_to_string</span>
+</span><span id="L-4"><a href="#L-4"><span class="linenos">4</span></a><span class="kn">from</span> <span class="nn">.dbmanager</span> <span class="kn">import</span> <span class="n">DBManager</span>
 </span></pre></div>
 
 
             </section>
     </main>
 <script>
     function escapeHTML(html) {
```

#### html2text {}

```diff
@@ -1,13 +1,18 @@
 
 
   ⁰
 [Unknown INPUT type]
 ***** Submodules *****
+    * custom_manager
     * databased
     * dbmanager
+    * dbparsers
 built_with_pdoc[pdoc_logo]
 
 ****** databased ******
 ⁰ View Source
-1from .databased import DataBased, _connect, data_to_string
+1from databased import dbparsers
+2
+3from .databased import DataBased, _connect, data_to_string
+4from .dbmanager import DBManager
```

### Comparing `databased-1.4.5/docs/databased/databased.html` & `databased-1.5.0/docs/databased/databased.html`

 * *Files 2% similar despite different names*

```diff
@@ -33,17 +33,14 @@
             <li>
                     <a class="class" href="#DataBased">DataBased</a>
                             <ul class="memberlist">
                         <li>
                                 <a class="function" href="#DataBased.__init__">DataBased</a>
                         </li>
                         <li>
-                                <a class="function" href="#DataBased.create_manager">create_manager</a>
-                        </li>
-                        <li>
                                 <a class="function" href="#DataBased.open">open</a>
                         </li>
                         <li>
                                 <a class="function" href="#DataBased.close">close</a>
                         </li>
                         <li>
                                 <a class="function" href="#DataBased.query">query</a>
@@ -115,18 +112,18 @@
                         <label class="view-source-button" for="mod-databased-view-source"><span>View Source</span></label>
 
                         <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos">  1</span></a><span class="kn">import</span> <span class="nn">logging</span>
 </span><span id="L-2"><a href="#L-2"><span class="linenos">  2</span></a><span class="kn">import</span> <span class="nn">os</span>
 </span><span id="L-3"><a href="#L-3"><span class="linenos">  3</span></a><span class="kn">import</span> <span class="nn">sqlite3</span>
 </span><span id="L-4"><a href="#L-4"><span class="linenos">  4</span></a><span class="kn">from</span> <span class="nn">datetime</span> <span class="kn">import</span> <span class="n">datetime</span>
 </span><span id="L-5"><a href="#L-5"><span class="linenos">  5</span></a><span class="kn">from</span> <span class="nn">functools</span> <span class="kn">import</span> <span class="n">wraps</span>
-</span><span id="L-6"><a href="#L-6"><span class="linenos">  6</span></a><span class="kn">from</span> <span class="nn">pathlib</span> <span class="kn">import</span> <span class="n">Path</span>
-</span><span id="L-7"><a href="#L-7"><span class="linenos">  7</span></a><span class="kn">from</span> <span class="nn">typing</span> <span class="kn">import</span> <span class="n">Any</span>
-</span><span id="L-8"><a href="#L-8"><span class="linenos">  8</span></a>
-</span><span id="L-9"><a href="#L-9"><span class="linenos">  9</span></a><span class="kn">import</span> <span class="nn">pandas</span>
+</span><span id="L-6"><a href="#L-6"><span class="linenos">  6</span></a><span class="kn">from</span> <span class="nn">typing</span> <span class="kn">import</span> <span class="n">Any</span>
+</span><span id="L-7"><a href="#L-7"><span class="linenos">  7</span></a>
+</span><span id="L-8"><a href="#L-8"><span class="linenos">  8</span></a><span class="kn">import</span> <span class="nn">pandas</span>
+</span><span id="L-9"><a href="#L-9"><span class="linenos">  9</span></a><span class="kn">from</span> <span class="nn">pathier</span> <span class="kn">import</span> <span class="n">Pathier</span>
 </span><span id="L-10"><a href="#L-10"><span class="linenos"> 10</span></a><span class="kn">from</span> <span class="nn">tabulate</span> <span class="kn">import</span> <span class="n">tabulate</span>
 </span><span id="L-11"><a href="#L-11"><span class="linenos"> 11</span></a>
 </span><span id="L-12"><a href="#L-12"><span class="linenos"> 12</span></a>
 </span><span id="L-13"><a href="#L-13"><span class="linenos"> 13</span></a><span class="k">def</span> <span class="nf">_connect</span><span class="p">(</span><span class="n">func</span><span class="p">):</span>
 </span><span id="L-14"><a href="#L-14"><span class="linenos"> 14</span></a>    <span class="sd">&quot;&quot;&quot;Decorator to open db connection if it isn&#39;t already open.&quot;&quot;&quot;</span>
 </span><span id="L-15"><a href="#L-15"><span class="linenos"> 15</span></a>
 </span><span id="L-16"><a href="#L-16"><span class="linenos"> 16</span></a>    <span class="nd">@wraps</span><span class="p">(</span><span class="n">func</span><span class="p">)</span>
@@ -144,546 +141,535 @@
 </span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a>
 </span><span id="L-29"><a href="#L-29"><span class="linenos"> 29</span></a><span class="sd">    Supports saving and reading dates as datetime objects.</span>
 </span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a>
 </span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a><span class="sd">    Supports using a context manager.&quot;&quot;&quot;</span>
 </span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a>
 </span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
 </span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a>        <span class="n">dbpath</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="n">Path</span><span class="p">,</span>
+</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a>        <span class="n">dbpath</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="n">Pathier</span><span class="p">,</span>
 </span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a>        <span class="n">logger_encoding</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;utf-8&quot;</span><span class="p">,</span>
 </span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a>        <span class="n">logger_message_format</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="si">{levelname}</span><span class="s2">|-|</span><span class="si">{asctime}</span><span class="s2">|-|</span><span class="si">{message}</span><span class="s2">&quot;</span><span class="p">,</span>
 </span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a>    <span class="p">):</span>
 </span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a>        <span class="sd">&quot;&quot;&quot;</span>
 </span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a><span class="sd">        :param dbpath: String or Path object to database file.</span>
 </span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a><span class="sd">        If a relative path is given, it will be relative to the</span>
 </span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a><span class="sd">        current working directory. The log file will be saved to the</span>
 </span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a><span class="sd">        same directory.</span>
 </span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a>
 </span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a><span class="sd">        :param logger_message_format: &#39;{&#39; style format string</span>
 </span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a><span class="sd">        for the logger object.&quot;&quot;&quot;</span>
-</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Path</span><span class="p">(</span><span class="n">dbpath</span><span class="p">)</span>
-</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">dbname</span> <span class="o">=</span> <span class="n">Path</span><span class="p">(</span><span class="n">dbpath</span><span class="p">)</span><span class="o">.</span><span class="n">name</span>
+</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">dbpath</span><span class="p">)</span>
+</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">dbname</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">dbpath</span><span class="p">)</span><span class="o">.</span><span class="n">name</span>
 </span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
 </span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_logger_init</span><span class="p">(</span>
 </span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a>            <span class="n">encoding</span><span class="o">=</span><span class="n">logger_encoding</span><span class="p">,</span> <span class="n">message_format</span><span class="o">=</span><span class="n">logger_message_format</span>
 </span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a>        <span class="p">)</span>
 </span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">connection_open</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">create_manager</span><span class="p">()</span>
-</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>
-</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>    <span class="k">def</span> <span class="fm">__enter__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">open</span><span class="p">()</span>
-</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a>        <span class="k">return</span> <span class="bp">self</span>
-</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a>
-</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a>    <span class="k">def</span> <span class="fm">__exit__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">exception_type</span><span class="p">,</span> <span class="n">exception_value</span><span class="p">,</span> <span class="n">exception_traceback</span><span class="p">):</span>
-</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">close</span><span class="p">()</span>
-</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a>
-</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a>    <span class="k">def</span> <span class="nf">create_manager</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a>        <span class="sd">&quot;&quot;&quot;Create dbmanager.py in the same directory</span>
-</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a><span class="sd">        as the database file if it doesn&#39;t exist.&quot;&quot;&quot;</span>
-</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a>        <span class="n">manager_path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">parent</span> <span class="o">/</span> <span class="s2">&quot;dbmanager.py&quot;</span>
-</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">manager_path</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a>            <span class="n">manager_template</span> <span class="o">=</span> <span class="p">(</span><span class="n">Path</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span><span class="o">.</span><span class="n">parent</span> <span class="o">/</span> <span class="s2">&quot;dbmanager.py&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
-</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>            <span class="n">manager_path</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">manager_template</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;$dbname&quot;</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbname</span><span class="p">))</span>
-</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>
-</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>    <span class="k">def</span> <span class="nf">open</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>        <span class="sd">&quot;&quot;&quot;Open connection to db.&quot;&quot;&quot;</span>
-</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">connection</span> <span class="o">=</span> <span class="n">sqlite3</span><span class="o">.</span><span class="n">connect</span><span class="p">(</span>
-</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">,</span>
-</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>            <span class="n">detect_types</span><span class="o">=</span><span class="n">sqlite3</span><span class="o">.</span><span class="n">PARSE_DECLTYPES</span> <span class="o">|</span> <span class="n">sqlite3</span><span class="o">.</span><span class="n">PARSE_COLNAMES</span><span class="p">,</span>
-</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>            <span class="n">timeout</span><span class="o">=</span><span class="mi">10</span><span class="p">,</span>
-</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>        <span class="p">)</span>
-</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">connection</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="s2">&quot;pragma foreign_keys = 1&quot;</span><span class="p">)</span>
-</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">connection</span><span class="o">.</span><span class="n">cursor</span><span class="p">()</span>
-</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">connection_open</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>
-</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>    <span class="k">def</span> <span class="nf">close</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>        <span class="sd">&quot;&quot;&quot;Save and close connection to db.</span>
-</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>
-</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a><span class="sd">        Call this as soon as you are done using the database if you have</span>
-</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a><span class="sd">        multiple threads or processes using the same database.&quot;&quot;&quot;</span>
-</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">connection_open</span><span class="p">:</span>
-</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">connection</span><span class="o">.</span><span class="n">commit</span><span class="p">()</span>
-</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">connection</span><span class="o">.</span><span class="n">close</span><span class="p">()</span>
-</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">connection_open</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>
-</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>    <span class="k">def</span> <span class="nf">_logger_init</span><span class="p">(</span>
-</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>        <span class="n">message_format</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="si">{levelname}</span><span class="s2">|-|</span><span class="si">{asctime}</span><span class="s2">|-|</span><span class="si">{message}</span><span class="s2">&quot;</span><span class="p">,</span>
-</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;utf-8&quot;</span><span class="p">,</span>
-</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>    <span class="p">):</span>
-</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>        <span class="sd">&quot;&quot;&quot;:param message_format: &#39;{&#39; style format string&quot;&quot;&quot;</span>
-</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">logger</span> <span class="o">=</span> <span class="n">logging</span><span class="o">.</span><span class="n">getLogger</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbname</span><span class="p">)</span>
-</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">hasHandlers</span><span class="p">():</span>
-</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>            <span class="n">handler</span> <span class="o">=</span> <span class="n">logging</span><span class="o">.</span><span class="n">FileHandler</span><span class="p">(</span>
-</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>                <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">,</span> <span class="s2">&quot;&quot;</span><span class="p">)</span> <span class="o">+</span> <span class="s2">&quot;.log&quot;</span><span class="p">,</span> <span class="n">encoding</span><span class="o">=</span><span class="n">encoding</span>
-</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>            <span class="p">)</span>
-</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>            <span class="n">handler</span><span class="o">.</span><span class="n">setFormatter</span><span class="p">(</span>
-</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>                <span class="n">logging</span><span class="o">.</span><span class="n">Formatter</span><span class="p">(</span>
-</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>                    <span class="n">message_format</span><span class="p">,</span> <span class="n">style</span><span class="o">=</span><span class="s2">&quot;{&quot;</span><span class="p">,</span> <span class="n">datefmt</span><span class="o">=</span><span class="s2">&quot;%m/</span><span class="si">%d</span><span class="s2">/%Y %I:%M:%S %p&quot;</span>
-</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>                <span class="p">)</span>
-</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>            <span class="p">)</span>
-</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">addHandler</span><span class="p">(</span><span class="n">handler</span><span class="p">)</span>
-</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">setLevel</span><span class="p">(</span><span class="n">logging</span><span class="o">.</span><span class="n">INFO</span><span class="p">)</span>
-</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>
-</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>    <span class="k">def</span> <span class="nf">_get_dict</span><span class="p">(</span>
-</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="nb">list</span><span class="p">,</span> <span class="n">columns_to_return</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">dict</span><span class="p">:</span>
-</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>        <span class="sd">&quot;&quot;&quot;Converts the values of a row into a dictionary with column names as keys.</span>
-</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>
-</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a><span class="sd">        :param table: The table that values were pulled from.</span>
-</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>
-</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a><span class="sd">        :param values: List of values expected to be the same quantity</span>
-</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a><span class="sd">        and in the same order as the column names of table.</span>
+</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a>
+</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>    <span class="k">def</span> <span class="fm">__enter__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">open</span><span class="p">()</span>
+</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a>        <span class="k">return</span> <span class="bp">self</span>
+</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a>
+</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a>    <span class="k">def</span> <span class="fm">__exit__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">exception_type</span><span class="p">,</span> <span class="n">exception_value</span><span class="p">,</span> <span class="n">exception_traceback</span><span class="p">):</span>
+</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">close</span><span class="p">()</span>
+</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a>
+</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a>    <span class="k">def</span> <span class="nf">open</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a>        <span class="sd">&quot;&quot;&quot;Open connection to db.&quot;&quot;&quot;</span>
+</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">connection</span> <span class="o">=</span> <span class="n">sqlite3</span><span class="o">.</span><span class="n">connect</span><span class="p">(</span>
+</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">,</span>
+</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a>            <span class="n">detect_types</span><span class="o">=</span><span class="n">sqlite3</span><span class="o">.</span><span class="n">PARSE_DECLTYPES</span> <span class="o">|</span> <span class="n">sqlite3</span><span class="o">.</span><span class="n">PARSE_COLNAMES</span><span class="p">,</span>
+</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a>            <span class="n">timeout</span><span class="o">=</span><span class="mi">10</span><span class="p">,</span>
+</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a>        <span class="p">)</span>
+</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">connection</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="s2">&quot;pragma foreign_keys = 1&quot;</span><span class="p">)</span>
+</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">connection</span><span class="o">.</span><span class="n">cursor</span><span class="p">()</span>
+</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">connection_open</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>
+</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>    <span class="k">def</span> <span class="nf">close</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a>        <span class="sd">&quot;&quot;&quot;Save and close connection to db.</span>
+</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>
+</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a><span class="sd">        Call this as soon as you are done using the database if you have</span>
+</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a><span class="sd">        multiple threads or processes using the same database.&quot;&quot;&quot;</span>
+</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">connection_open</span><span class="p">:</span>
+</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">connection</span><span class="o">.</span><span class="n">commit</span><span class="p">()</span>
+</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">connection</span><span class="o">.</span><span class="n">close</span><span class="p">()</span>
+</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">connection_open</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>
+</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>    <span class="k">def</span> <span class="nf">_logger_init</span><span class="p">(</span>
+</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>        <span class="n">message_format</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="si">{levelname}</span><span class="s2">|-|</span><span class="si">{asctime}</span><span class="s2">|-|</span><span class="si">{message}</span><span class="s2">&quot;</span><span class="p">,</span>
+</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;utf-8&quot;</span><span class="p">,</span>
+</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>    <span class="p">):</span>
+</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>        <span class="sd">&quot;&quot;&quot;:param message_format: &#39;{&#39; style format string&quot;&quot;&quot;</span>
+</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">logger</span> <span class="o">=</span> <span class="n">logging</span><span class="o">.</span><span class="n">getLogger</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbname</span><span class="p">)</span>
+</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">hasHandlers</span><span class="p">():</span>
+</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>            <span class="n">handler</span> <span class="o">=</span> <span class="n">logging</span><span class="o">.</span><span class="n">FileHandler</span><span class="p">(</span>
+</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>                <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">,</span> <span class="s2">&quot;&quot;</span><span class="p">)</span> <span class="o">+</span> <span class="s2">&quot;.log&quot;</span><span class="p">,</span> <span class="n">encoding</span><span class="o">=</span><span class="n">encoding</span>
+</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>            <span class="p">)</span>
+</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>            <span class="n">handler</span><span class="o">.</span><span class="n">setFormatter</span><span class="p">(</span>
+</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>                <span class="n">logging</span><span class="o">.</span><span class="n">Formatter</span><span class="p">(</span>
+</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>                    <span class="n">message_format</span><span class="p">,</span> <span class="n">style</span><span class="o">=</span><span class="s2">&quot;{&quot;</span><span class="p">,</span> <span class="n">datefmt</span><span class="o">=</span><span class="s2">&quot;%m/</span><span class="si">%d</span><span class="s2">/%Y %I:%M:%S %p&quot;</span>
+</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>                <span class="p">)</span>
+</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>            <span class="p">)</span>
+</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">addHandler</span><span class="p">(</span><span class="n">handler</span><span class="p">)</span>
+</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">setLevel</span><span class="p">(</span><span class="n">logging</span><span class="o">.</span><span class="n">INFO</span><span class="p">)</span>
+</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>
+</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>    <span class="k">def</span> <span class="nf">_get_dict</span><span class="p">(</span>
+</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="nb">list</span><span class="p">,</span> <span class="n">columns_to_return</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">dict</span><span class="p">:</span>
+</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>        <span class="sd">&quot;&quot;&quot;Converts the values of a row into a dictionary with column names as keys.</span>
+</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>
+</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a><span class="sd">        :param table: The table that values were pulled from.</span>
+</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>
+</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a><span class="sd">        :param values: List of values expected to be the same quantity</span>
+</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a><span class="sd">        and in the same order as the column names of table.</span>
+</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>
+</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a><span class="sd">        :param columns_to_return: An optional list of column names.</span>
+</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a><span class="sd">        If given, only these columns will be included in the returned dictionary.</span>
+</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a><span class="sd">        Otherwise all columns and values are returned.&quot;&quot;&quot;</span>
+</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>        <span class="k">return</span> <span class="p">{</span>
+</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>            <span class="n">column</span><span class="p">:</span> <span class="n">value</span>
+</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>            <span class="k">for</span> <span class="n">column</span><span class="p">,</span> <span class="n">value</span> <span class="ow">in</span> <span class="nb">zip</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">get_column_names</span><span class="p">(</span><span class="n">table</span><span class="p">),</span> <span class="n">values</span><span class="p">)</span>
+</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>            <span class="k">if</span> <span class="ow">not</span> <span class="n">columns_to_return</span> <span class="ow">or</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns_to_return</span>
+</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>        <span class="p">}</span>
 </span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>
-</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a><span class="sd">        :param columns_to_return: An optional list of column names.</span>
-</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a><span class="sd">        If given, only these columns will be included in the returned dictionary.</span>
-</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a><span class="sd">        Otherwise all columns and values are returned.&quot;&quot;&quot;</span>
-</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>        <span class="k">return</span> <span class="p">{</span>
-</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>            <span class="n">column</span><span class="p">:</span> <span class="n">value</span>
-</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>            <span class="k">for</span> <span class="n">column</span><span class="p">,</span> <span class="n">value</span> <span class="ow">in</span> <span class="nb">zip</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">get_column_names</span><span class="p">(</span><span class="n">table</span><span class="p">),</span> <span class="n">values</span><span class="p">)</span>
-</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>            <span class="k">if</span> <span class="ow">not</span> <span class="n">columns_to_return</span> <span class="ow">or</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns_to_return</span>
-</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>        <span class="p">}</span>
+</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>    <span class="k">def</span> <span class="nf">_get_conditions</span><span class="p">(</span>
+</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>        <span class="sd">&quot;&quot;&quot;Builds and returns the conditional portion of a query.</span>
+</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>
+</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a><span class="sd">        :param match_criteria: Can be a list of 2-tuples where each</span>
+</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a><span class="sd">        tuple is (columnName, rowValue) or a dictionary where</span>
+</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a><span class="sd">        keys are column names and values are row values.</span>
 </span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>
-</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>    <span class="k">def</span> <span class="nf">_get_conditions</span><span class="p">(</span>
-</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>        <span class="sd">&quot;&quot;&quot;Builds and returns the conditional portion of a query.</span>
+</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a><span class="sd">        :param exact_match: If False, the rowValue for a give column</span>
+</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a><span class="sd">        will be matched as a substring.</span>
+</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>
+</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a><span class="sd">        Usage e.g.:</span>
 </span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>
-</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a><span class="sd">        :param match_criteria: Can be a list of 2-tuples where each</span>
-</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a><span class="sd">        tuple is (columnName, rowValue) or a dictionary where</span>
-</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a><span class="sd">        keys are column names and values are row values.</span>
-</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>
-</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a><span class="sd">        :param exact_match: If False, the rowValue for a give column</span>
-</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a><span class="sd">        will be matched as a substring.</span>
-</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>
-</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a><span class="sd">        Usage e.g.:</span>
-</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>
-</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a><span class="sd">        self.cursor.execute(f&#39;select * from {table} where {conditions}&#39;)&quot;&quot;&quot;</span>
-</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>        <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">)</span> <span class="o">==</span> <span class="nb">dict</span><span class="p">:</span>
-</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>            <span class="n">match_criteria</span> <span class="o">=</span> <span class="p">[(</span><span class="n">k</span><span class="p">,</span> <span class="n">v</span><span class="p">)</span> <span class="k">for</span> <span class="n">k</span><span class="p">,</span> <span class="n">v</span> <span class="ow">in</span> <span class="n">match_criteria</span><span class="o">.</span><span class="n">items</span><span class="p">()]</span>
-</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>        <span class="k">if</span> <span class="n">exact_match</span><span class="p">:</span>
-</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="s2">&quot; and &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
-</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>                <span class="sa">f</span><span class="s1">&#39;&quot;</span><span class="si">{</span><span class="n">column_row</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s1">&quot; = &quot;</span><span class="si">{</span><span class="n">column_row</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s1">&quot;&#39;</span>
-</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>                <span class="k">for</span> <span class="n">column_row</span> <span class="ow">in</span> <span class="n">match_criteria</span>
-</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>            <span class="p">)</span>
-</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="s2">&quot; and &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
-</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>                <span class="sa">f</span><span class="s1">&#39;&quot;</span><span class="si">{</span><span class="n">column_row</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s1">&quot; like &quot;%</span><span class="si">{</span><span class="n">column_row</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s1">%&quot;&#39;</span>
-</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>                <span class="k">for</span> <span class="n">column_row</span> <span class="ow">in</span> <span class="n">match_criteria</span>
-</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>            <span class="p">)</span>
-</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;(</span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">)&quot;</span>
-</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>
-</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>    <span class="nd">@_connect</span>
-</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a>    <span class="k">def</span> <span class="nf">query</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">query_</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]:</span>
-</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a>        <span class="sd">&quot;&quot;&quot;Execute an arbitrary query and</span>
-</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a><span class="sd">        return the results.&quot;&quot;&quot;</span>
-</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query_</span><span class="p">)</span>
-</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()</span>
-</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a>
-</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>    <span class="nd">@_connect</span>
-</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a>    <span class="k">def</span> <span class="nf">create_tables</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table_querys</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="p">[]):</span>
-</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>        <span class="sd">&quot;&quot;&quot;Create tables if they don&#39;t exist.</span>
+</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a><span class="sd">        self.cursor.execute(f&#39;select * from {table} where {conditions}&#39;)&quot;&quot;&quot;</span>
+</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>        <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">)</span> <span class="o">==</span> <span class="nb">dict</span><span class="p">:</span>
+</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>            <span class="n">match_criteria</span> <span class="o">=</span> <span class="p">[(</span><span class="n">k</span><span class="p">,</span> <span class="n">v</span><span class="p">)</span> <span class="k">for</span> <span class="n">k</span><span class="p">,</span> <span class="n">v</span> <span class="ow">in</span> <span class="n">match_criteria</span><span class="o">.</span><span class="n">items</span><span class="p">()]</span>
+</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>        <span class="k">if</span> <span class="n">exact_match</span><span class="p">:</span>
+</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="s2">&quot; and &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
+</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>                <span class="sa">f</span><span class="s1">&#39;&quot;</span><span class="si">{</span><span class="n">column_row</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s1">&quot; = &quot;</span><span class="si">{</span><span class="n">column_row</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s1">&quot;&#39;</span>
+</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>                <span class="k">for</span> <span class="n">column_row</span> <span class="ow">in</span> <span class="n">match_criteria</span>
+</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>            <span class="p">)</span>
+</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="s2">&quot; and &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
+</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>                <span class="sa">f</span><span class="s1">&#39;&quot;</span><span class="si">{</span><span class="n">column_row</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s1">&quot; like &quot;%</span><span class="si">{</span><span class="n">column_row</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s1">%&quot;&#39;</span>
+</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>                <span class="k">for</span> <span class="n">column_row</span> <span class="ow">in</span> <span class="n">match_criteria</span>
+</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>            <span class="p">)</span>
+</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;(</span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">)&quot;</span>
+</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>
+</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>    <span class="nd">@_connect</span>
+</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>    <span class="k">def</span> <span class="nf">query</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">query_</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]:</span>
+</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>        <span class="sd">&quot;&quot;&quot;Execute an arbitrary query and</span>
+</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a><span class="sd">        return the results.&quot;&quot;&quot;</span>
+</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query_</span><span class="p">)</span>
+</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()</span>
+</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>
+</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>    <span class="nd">@_connect</span>
+</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>    <span class="k">def</span> <span class="nf">create_tables</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table_querys</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="p">[]):</span>
+</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>        <span class="sd">&quot;&quot;&quot;Create tables if they don&#39;t exist.</span>
+</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a>
+</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a><span class="sd">        :param table_querys: Each query should be</span>
+</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a><span class="sd">        in the form &#39;tableName(columnDefinitions)&#39;&quot;&quot;&quot;</span>
+</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">table_querys</span><span class="p">)</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a>            <span class="n">table_names</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
+</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">table_querys</span><span class="p">:</span>
+</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>                <span class="k">if</span> <span class="n">table</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;(&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">table_names</span><span class="p">:</span>
+</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;create table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;</span><span class="si">{</span><span class="n">table</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;(&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s1"> table created.&#39;</span><span class="p">)</span>
 </span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a>
-</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a><span class="sd">        :param table_querys: Each query should be</span>
-</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a><span class="sd">        in the form &#39;tableName(columnDefinitions)&#39;&quot;&quot;&quot;</span>
-</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">table_querys</span><span class="p">)</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>            <span class="n">table_names</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
-</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">table_querys</span><span class="p">:</span>
-</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>                <span class="k">if</span> <span class="n">table</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;(&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">table_names</span><span class="p">:</span>
-</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;create table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;</span><span class="si">{</span><span class="n">table</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;(&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s1"> table created.&#39;</span><span class="p">)</span>
-</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a>
-</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>    <span class="nd">@_connect</span>
-</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a>    <span class="k">def</span> <span class="nf">create_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">column_defs</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]):</span>
-</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>        <span class="sd">&quot;&quot;&quot;Create a table if it doesn&#39;t exist.</span>
-</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>
-</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a><span class="sd">        :param table: Name of the table to create.</span>
-</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>
-</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a><span class="sd">        :param column_defs: List of column definitions in</span>
-</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a><span class="sd">        proper Sqlite3 sytax.</span>
-</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a><span class="sd">        i.e. &quot;columnName text unique&quot; or &quot;columnName int primary key&quot; etc.&quot;&quot;&quot;</span>
-</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>        <span class="k">if</span> <span class="n">table</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">():</span>
-</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>            <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;create table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">(</span><span class="si">{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">column_defs</span><span class="p">)</span><span class="si">}</span><span class="s2">)&quot;</span>
-</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
-</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;&#39;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&#39; table created.&quot;</span><span class="p">)</span>
-</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a>
-</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>    <span class="nd">@_connect</span>
-</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>    <span class="k">def</span> <span class="nf">get_table_names</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
-</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>        <span class="sd">&quot;&quot;&quot;Returns a list of table names from database.&quot;&quot;&quot;</span>
-</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>            <span class="s1">&#39;select name from sqlite_Schema where type = &quot;table&quot; and name not like &quot;sqlite_%&quot;&#39;</span>
-</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>        <span class="p">)</span>
-</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">result</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()]</span>
-</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>
-</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a>    <span class="nd">@_connect</span>
-</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>    <span class="k">def</span> <span class="nf">get_column_names</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
-</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a>        <span class="sd">&quot;&quot;&quot;Return a list of column names from a table.&quot;&quot;&quot;</span>
-</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;select * from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> where 1=0&quot;</span><span class="p">)</span>
-</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">description</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="k">for</span> <span class="n">description</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">description</span><span class="p">]</span>
+</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>    <span class="nd">@_connect</span>
+</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>    <span class="k">def</span> <span class="nf">create_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">column_defs</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]):</span>
+</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>        <span class="sd">&quot;&quot;&quot;Create a table if it doesn&#39;t exist.</span>
+</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>
+</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a><span class="sd">        :param table: Name of the table to create.</span>
+</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>
+</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a><span class="sd">        :param column_defs: List of column definitions in</span>
+</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a><span class="sd">        proper Sqlite3 sytax.</span>
+</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a><span class="sd">        i.e. &quot;columnName text unique&quot; or &quot;columnName int primary key&quot; etc.&quot;&quot;&quot;</span>
+</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>        <span class="k">if</span> <span class="n">table</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">():</span>
+</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a>            <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;create table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">(</span><span class="si">{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">column_defs</span><span class="p">)</span><span class="si">}</span><span class="s2">)&quot;</span>
+</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
+</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;&#39;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&#39; table created.&quot;</span><span class="p">)</span>
+</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>
+</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>    <span class="nd">@_connect</span>
+</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a>    <span class="k">def</span> <span class="nf">get_table_names</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
+</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>        <span class="sd">&quot;&quot;&quot;Returns a list of table names from database.&quot;&quot;&quot;</span>
+</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>            <span class="s1">&#39;select name from sqlite_Schema where type = &quot;table&quot; and name not like &quot;sqlite_%&quot;&#39;</span>
+</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>        <span class="p">)</span>
+</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">result</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()]</span>
+</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>
+</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a>    <span class="nd">@_connect</span>
+</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>    <span class="k">def</span> <span class="nf">get_column_names</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
+</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>        <span class="sd">&quot;&quot;&quot;Return a list of column names from a table.&quot;&quot;&quot;</span>
+</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;select * from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> where 1=0&quot;</span><span class="p">)</span>
+</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">description</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="k">for</span> <span class="n">description</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">description</span><span class="p">]</span>
+</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>
+</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>    <span class="nd">@_connect</span>
+</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>    <span class="k">def</span> <span class="nf">count</span><span class="p">(</span>
+</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
+</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a>        <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>        <span class="sd">&quot;&quot;&quot;Return number of items in table.</span>
 </span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>
-</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a>    <span class="nd">@_connect</span>
-</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a>    <span class="k">def</span> <span class="nf">count</span><span class="p">(</span>
-</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
-</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a>        <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a>        <span class="sd">&quot;&quot;&quot;Return number of items in table.</span>
-</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a>
-</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a><span class="sd">        :param match_criteria: Can be a list of 2-tuples where each</span>
-</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a><span class="sd">        tuple is (columnName, rowValue) or a dictionary where</span>
-</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a><span class="sd">        keys are column names and values are row values.</span>
-</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a><span class="sd">        If None, all rows from the table will be counted.</span>
-</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a>
-</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a><span class="sd">        :param exact_match: If False, the row value for a give column</span>
-</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a><span class="sd">        in match_criteria will be matched as a substring. Has no effect if</span>
-</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a><span class="sd">        match_criteria is None.</span>
-</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;select count(_rowid_) from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a>            <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
-</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a>                    <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">query</span><span class="si">}</span><span class="s2"> where </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a>                <span class="p">)</span>
-</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">query</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a>            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchone</span><span class="p">()[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a>        <span class="k">except</span><span class="p">:</span>
-</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a>            <span class="k">return</span> <span class="mi">0</span>
-</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a>
-</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a>    <span class="nd">@_connect</span>
-</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a>    <span class="k">def</span> <span class="nf">add_row</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="nb">any</span><span class="p">],</span> <span class="n">columns</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a>        <span class="sd">&quot;&quot;&quot;Add row of values to table.</span>
-</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a>
-</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a><span class="sd">        :param table: The table to insert into.</span>
-</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a>
-</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a><span class="sd">        :param values: A tuple of values to be inserted into the table.</span>
-</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a>
-</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a><span class="sd">        :param columns: If None, values param is expected to supply</span>
-</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a><span class="sd">        a value for every column in the table. If columns is</span>
-</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a><span class="sd">        provided, it should contain the same number of elements as values.&quot;&quot;&quot;</span>
-</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a>        <span class="n">parameterizer</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="s2">&quot;?&quot;</span> <span class="k">for</span> <span class="n">_</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
-</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a>        <span class="n">logger_values</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
-</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>            <span class="k">if</span> <span class="n">columns</span><span class="p">:</span>
-</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a>                <span class="n">columns</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">column</span> <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span><span class="p">)</span>
-</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a>                    <span class="sa">f</span><span class="s2">&quot;insert into </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> (</span><span class="si">{</span><span class="n">columns</span><span class="si">}</span><span class="s2">) values(</span><span class="si">{</span><span class="n">parameterizer</span><span class="si">}</span><span class="s2">)&quot;</span><span class="p">,</span> <span class="n">values</span>
-</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>                <span class="p">)</span>
-</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a>                    <span class="sa">f</span><span class="s2">&quot;insert into </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> values(</span><span class="si">{</span><span class="n">parameterizer</span><span class="si">}</span><span class="s2">)&quot;</span><span class="p">,</span> <span class="n">values</span>
+</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a><span class="sd">        :param match_criteria: Can be a list of 2-tuples where each</span>
+</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a><span class="sd">        tuple is (columnName, rowValue) or a dictionary where</span>
+</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a><span class="sd">        keys are column names and values are row values.</span>
+</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a><span class="sd">        If None, all rows from the table will be counted.</span>
+</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a>
+</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a><span class="sd">        :param exact_match: If False, the row value for a give column</span>
+</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a><span class="sd">        in match_criteria will be matched as a substring. Has no effect if</span>
+</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a><span class="sd">        match_criteria is None.</span>
+</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;select count(_rowid_) from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a>            <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
+</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a>                    <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">query</span><span class="si">}</span><span class="s2"> where </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a>                <span class="p">)</span>
+</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">query</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a>            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchone</span><span class="p">()[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a>        <span class="k">except</span><span class="p">:</span>
+</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a>            <span class="k">return</span> <span class="mi">0</span>
+</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a>
+</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a>    <span class="nd">@_connect</span>
+</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a>    <span class="k">def</span> <span class="nf">add_row</span><span class="p">(</span>
+</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="n">Any</span><span class="p">],</span> <span class="n">columns</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a>    <span class="p">):</span>
+</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a>        <span class="sd">&quot;&quot;&quot;Add row of values to table.</span>
+</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a>
+</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a><span class="sd">        :param table: The table to insert into.</span>
+</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a>
+</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a><span class="sd">        :param values: A tuple of values to be inserted into the table.</span>
+</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a>
+</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a><span class="sd">        :param columns: If None, values param is expected to supply</span>
+</span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a><span class="sd">        a value for every column in the table. If columns is</span>
+</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a><span class="sd">        provided, it should contain the same number of elements as values.&quot;&quot;&quot;</span>
+</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a>        <span class="n">parameterizer</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="s2">&quot;?&quot;</span> <span class="k">for</span> <span class="n">_</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
+</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a>        <span class="n">logger_values</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
+</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a>            <span class="k">if</span> <span class="n">columns</span><span class="p">:</span>
+</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a>                <span class="n">columns_query</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">column</span> <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span><span class="p">)</span>
+</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a>                    <span class="sa">f</span><span class="s2">&quot;insert into </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> (</span><span class="si">{</span><span class="n">columns_query</span><span class="si">}</span><span class="s2">) values(</span><span class="si">{</span><span class="n">parameterizer</span><span class="si">}</span><span class="s2">)&quot;</span><span class="p">,</span>
+</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a>                    <span class="n">values</span><span class="p">,</span>
+</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a>                <span class="p">)</span>
+</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a>                    <span class="sa">f</span><span class="s2">&quot;insert into </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> values(</span><span class="si">{</span><span class="n">parameterizer</span><span class="si">}</span><span class="s2">)&quot;</span><span class="p">,</span> <span class="n">values</span>
+</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a>                <span class="p">)</span>
+</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Added &quot;</span><span class="si">{</span><span class="n">logger_values</span><span class="si">}</span><span class="s1">&quot; to </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1"> table.&#39;</span><span class="p">)</span>
+</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a>            <span class="k">if</span> <span class="s2">&quot;constraint&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">)</span><span class="o">.</span><span class="n">lower</span><span class="p">():</span>
+</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">exception</span><span class="p">(</span>
+</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a>                    <span class="sa">f</span><span class="s1">&#39;Error adding &quot;</span><span class="si">{</span><span class="n">logger_values</span><span class="si">}</span><span class="s1">&quot; to </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1"> table.&#39;</span>
 </span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a>                <span class="p">)</span>
-</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Added &quot;</span><span class="si">{</span><span class="n">logger_values</span><span class="si">}</span><span class="s1">&quot; to </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1"> table.&#39;</span><span class="p">)</span>
-</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a>            <span class="k">if</span> <span class="s2">&quot;constraint&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">)</span><span class="o">.</span><span class="n">lower</span><span class="p">():</span>
-</span><span id="L-263"><a href="#L-263"><span class="linenos">263</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">exception</span><span class="p">(</span>
-</span><span id="L-264"><a href="#L-264"><span class="linenos">264</span></a>                    <span class="sa">f</span><span class="s1">&#39;Error adding &quot;</span><span class="si">{</span><span class="n">logger_values</span><span class="si">}</span><span class="s1">&quot; to </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1"> table.&#39;</span>
-</span><span id="L-265"><a href="#L-265"><span class="linenos">265</span></a>                <span class="p">)</span>
-</span><span id="L-266"><a href="#L-266"><span class="linenos">266</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="L-267"><a href="#L-267"><span class="linenos">267</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">debug</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">))</span>
-</span><span id="L-268"><a href="#L-268"><span class="linenos">268</span></a>
-</span><span id="L-269"><a href="#L-269"><span class="linenos">269</span></a>    <span class="nd">@_connect</span>
-</span><span id="L-270"><a href="#L-270"><span class="linenos">270</span></a>    <span class="k">def</span> <span class="nf">get_rows</span><span class="p">(</span>
-</span><span id="L-271"><a href="#L-271"><span class="linenos">271</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="L-272"><a href="#L-272"><span class="linenos">272</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
-</span><span id="L-273"><a href="#L-273"><span class="linenos">273</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="L-274"><a href="#L-274"><span class="linenos">274</span></a>        <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="L-275"><a href="#L-275"><span class="linenos">275</span></a>        <span class="n">sort_by_column</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="L-276"><a href="#L-276"><span class="linenos">276</span></a>        <span class="n">columns_to_return</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="L-277"><a href="#L-277"><span class="linenos">277</span></a>        <span class="n">return_as_dataframe</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
-</span><span id="L-278"><a href="#L-278"><span class="linenos">278</span></a>        <span class="n">values_only</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
-</span><span id="L-279"><a href="#L-279"><span class="linenos">279</span></a>        <span class="n">order_by</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="L-280"><a href="#L-280"><span class="linenos">280</span></a>        <span class="n">limit</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="L-281"><a href="#L-281"><span class="linenos">281</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]</span> <span class="o">|</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="n">pandas</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">:</span>
-</span><span id="L-282"><a href="#L-282"><span class="linenos">282</span></a>        <span class="sd">&quot;&quot;&quot;Returns rows from table as a list of dictionaries</span>
-</span><span id="L-283"><a href="#L-283"><span class="linenos">283</span></a><span class="sd">        where the key-value pairs of the dictionaries are</span>
-</span><span id="L-284"><a href="#L-284"><span class="linenos">284</span></a><span class="sd">        column name: row value.</span>
-</span><span id="L-285"><a href="#L-285"><span class="linenos">285</span></a>
-</span><span id="L-286"><a href="#L-286"><span class="linenos">286</span></a><span class="sd">        :param match_criteria: Can be a list of 2-tuples where each</span>
-</span><span id="L-287"><a href="#L-287"><span class="linenos">287</span></a><span class="sd">        tuple is (columnName, rowValue) or a dictionary where</span>
-</span><span id="L-288"><a href="#L-288"><span class="linenos">288</span></a><span class="sd">        keys are column names and values are row values.</span>
-</span><span id="L-289"><a href="#L-289"><span class="linenos">289</span></a>
-</span><span id="L-290"><a href="#L-290"><span class="linenos">290</span></a><span class="sd">        :param exact_match: If False, the rowValue for a give column</span>
-</span><span id="L-291"><a href="#L-291"><span class="linenos">291</span></a><span class="sd">        will be matched as a substring.</span>
-</span><span id="L-292"><a href="#L-292"><span class="linenos">292</span></a>
-</span><span id="L-293"><a href="#L-293"><span class="linenos">293</span></a><span class="sd">        :param sort_by_column: A column name to sort the results by.</span>
-</span><span id="L-294"><a href="#L-294"><span class="linenos">294</span></a><span class="sd">        This will sort results in Python after retrieving them from the db.</span>
-</span><span id="L-295"><a href="#L-295"><span class="linenos">295</span></a><span class="sd">        Use the &#39;order_by&#39; param to use SQLite engine for ordering.</span>
-</span><span id="L-296"><a href="#L-296"><span class="linenos">296</span></a>
-</span><span id="L-297"><a href="#L-297"><span class="linenos">297</span></a><span class="sd">        :param columns_to_return: Optional list of column names.</span>
-</span><span id="L-298"><a href="#L-298"><span class="linenos">298</span></a><span class="sd">        If provided, the elements returned by get_rows() will</span>
-</span><span id="L-299"><a href="#L-299"><span class="linenos">299</span></a><span class="sd">        only contain the provided columns. Otherwise every column</span>
-</span><span id="L-300"><a href="#L-300"><span class="linenos">300</span></a><span class="sd">        in the row is returned.</span>
-</span><span id="L-301"><a href="#L-301"><span class="linenos">301</span></a>
-</span><span id="L-302"><a href="#L-302"><span class="linenos">302</span></a><span class="sd">        :param return_as_dataframe: If True,</span>
-</span><span id="L-303"><a href="#L-303"><span class="linenos">303</span></a><span class="sd">        the results will be returned as a pandas.DataFrame object.</span>
-</span><span id="L-304"><a href="#L-304"><span class="linenos">304</span></a>
-</span><span id="L-305"><a href="#L-305"><span class="linenos">305</span></a><span class="sd">        :param values_only: Return the results as a list of tuples</span>
-</span><span id="L-306"><a href="#L-306"><span class="linenos">306</span></a><span class="sd">        instead of a list of dictionaries that have column names as keys.</span>
-</span><span id="L-307"><a href="#L-307"><span class="linenos">307</span></a><span class="sd">        The results will still be sorted according to sort_by_column if</span>
-</span><span id="L-308"><a href="#L-308"><span class="linenos">308</span></a><span class="sd">        one is provided.</span>
-</span><span id="L-309"><a href="#L-309"><span class="linenos">309</span></a>
-</span><span id="L-310"><a href="#L-310"><span class="linenos">310</span></a><span class="sd">        :param order_by: If given, a &#39;order by {order_by}&#39; clause</span>
-</span><span id="L-311"><a href="#L-311"><span class="linenos">311</span></a><span class="sd">        will be added to the select query.</span>
-</span><span id="L-312"><a href="#L-312"><span class="linenos">312</span></a>
-</span><span id="L-313"><a href="#L-313"><span class="linenos">313</span></a><span class="sd">        :param limit: If given, a &#39;limit {limit}&#39; clause will be</span>
-</span><span id="L-314"><a href="#L-314"><span class="linenos">314</span></a><span class="sd">        added to the select query.</span>
-</span><span id="L-315"><a href="#L-315"><span class="linenos">315</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="L-316"><a href="#L-316"><span class="linenos">316</span></a>
-</span><span id="L-317"><a href="#L-317"><span class="linenos">317</span></a>        <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">columns_to_return</span><span class="p">)</span> <span class="ow">is</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="L-318"><a href="#L-318"><span class="linenos">318</span></a>            <span class="n">columns_to_return</span> <span class="o">=</span> <span class="p">[</span><span class="n">columns_to_return</span><span class="p">]</span>
-</span><span id="L-319"><a href="#L-319"><span class="linenos">319</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;select * from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-320"><a href="#L-320"><span class="linenos">320</span></a>        <span class="n">matches</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="L-321"><a href="#L-321"><span class="linenos">321</span></a>        <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
-</span><span id="L-322"><a href="#L-322"><span class="linenos">322</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; where </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-323"><a href="#L-323"><span class="linenos">323</span></a>        <span class="k">if</span> <span class="n">order_by</span><span class="p">:</span>
-</span><span id="L-324"><a href="#L-324"><span class="linenos">324</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; order by </span><span class="si">{</span><span class="n">order_by</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-325"><a href="#L-325"><span class="linenos">325</span></a>        <span class="k">if</span> <span class="n">limit</span><span class="p">:</span>
-</span><span id="L-326"><a href="#L-326"><span class="linenos">326</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; limit </span><span class="si">{</span><span class="n">limit</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-327"><a href="#L-327"><span class="linenos">327</span></a>        <span class="n">query</span> <span class="o">+=</span> <span class="s2">&quot;;&quot;</span>
-</span><span id="L-328"><a href="#L-328"><span class="linenos">328</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
-</span><span id="L-329"><a href="#L-329"><span class="linenos">329</span></a>        <span class="n">matches</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()</span>
-</span><span id="L-330"><a href="#L-330"><span class="linenos">330</span></a>        <span class="n">results</span> <span class="o">=</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_dict</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">match</span><span class="p">,</span> <span class="n">columns_to_return</span><span class="p">)</span> <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">]</span>
-</span><span id="L-331"><a href="#L-331"><span class="linenos">331</span></a>        <span class="k">if</span> <span class="n">sort_by_column</span><span class="p">:</span>
-</span><span id="L-332"><a href="#L-332"><span class="linenos">332</span></a>            <span class="n">results</span> <span class="o">=</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">results</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="k">lambda</span> <span class="n">x</span><span class="p">:</span> <span class="n">x</span><span class="p">[</span><span class="n">sort_by_column</span><span class="p">])</span>
-</span><span id="L-333"><a href="#L-333"><span class="linenos">333</span></a>        <span class="k">if</span> <span class="n">return_as_dataframe</span><span class="p">:</span>
-</span><span id="L-334"><a href="#L-334"><span class="linenos">334</span></a>            <span class="k">return</span> <span class="n">pandas</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">(</span><span class="n">results</span><span class="p">)</span>
-</span><span id="L-335"><a href="#L-335"><span class="linenos">335</span></a>        <span class="k">if</span> <span class="n">values_only</span><span class="p">:</span>
-</span><span id="L-336"><a href="#L-336"><span class="linenos">336</span></a>            <span class="k">return</span> <span class="p">[</span><span class="nb">tuple</span><span class="p">(</span><span class="n">row</span><span class="o">.</span><span class="n">values</span><span class="p">())</span> <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">results</span><span class="p">]</span>
-</span><span id="L-337"><a href="#L-337"><span class="linenos">337</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="L-338"><a href="#L-338"><span class="linenos">338</span></a>            <span class="k">return</span> <span class="n">results</span>
-</span><span id="L-339"><a href="#L-339"><span class="linenos">339</span></a>
-</span><span id="L-340"><a href="#L-340"><span class="linenos">340</span></a>    <span class="nd">@_connect</span>
-</span><span id="L-341"><a href="#L-341"><span class="linenos">341</span></a>    <span class="k">def</span> <span class="nf">find</span><span class="p">(</span>
-</span><span id="L-342"><a href="#L-342"><span class="linenos">342</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">query_string</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">columns</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="L-343"><a href="#L-343"><span class="linenos">343</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">tuple</span><span class="p">[</span><span class="nb">dict</span><span class="p">]:</span>
-</span><span id="L-344"><a href="#L-344"><span class="linenos">344</span></a>        <span class="sd">&quot;&quot;&quot;Search for rows that contain query_string as a substring</span>
-</span><span id="L-345"><a href="#L-345"><span class="linenos">345</span></a><span class="sd">        of any column.</span>
-</span><span id="L-346"><a href="#L-346"><span class="linenos">346</span></a>
-</span><span id="L-347"><a href="#L-347"><span class="linenos">347</span></a><span class="sd">        :param table: The table to search.</span>
-</span><span id="L-348"><a href="#L-348"><span class="linenos">348</span></a>
-</span><span id="L-349"><a href="#L-349"><span class="linenos">349</span></a><span class="sd">        :param query_string: The substring to search for in all columns.</span>
-</span><span id="L-350"><a href="#L-350"><span class="linenos">350</span></a>
-</span><span id="L-351"><a href="#L-351"><span class="linenos">351</span></a><span class="sd">        :param columns: A list of columns to search for query_string.</span>
-</span><span id="L-352"><a href="#L-352"><span class="linenos">352</span></a><span class="sd">        If None, all columns in the table will be searched.</span>
-</span><span id="L-353"><a href="#L-353"><span class="linenos">353</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="L-354"><a href="#L-354"><span class="linenos">354</span></a>        <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">columns</span><span class="p">)</span> <span class="ow">is</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="L-355"><a href="#L-355"><span class="linenos">355</span></a>            <span class="n">columns</span> <span class="o">=</span> <span class="p">[</span><span class="n">columns</span><span class="p">]</span>
-</span><span id="L-356"><a href="#L-356"><span class="linenos">356</span></a>        <span class="n">results</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="L-357"><a href="#L-357"><span class="linenos">357</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">columns</span><span class="p">:</span>
-</span><span id="L-358"><a href="#L-358"><span class="linenos">358</span></a>            <span class="n">columns</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_column_names</span><span class="p">(</span><span class="n">table</span><span class="p">)</span>
-</span><span id="L-359"><a href="#L-359"><span class="linenos">359</span></a>        <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span><span class="p">:</span>
-</span><span id="L-360"><a href="#L-360"><span class="linenos">360</span></a>            <span class="n">results</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span>
-</span><span id="L-361"><a href="#L-361"><span class="linenos">361</span></a>                <span class="p">[</span>
-</span><span id="L-362"><a href="#L-362"><span class="linenos">362</span></a>                    <span class="n">row</span>
-</span><span id="L-363"><a href="#L-363"><span class="linenos">363</span></a>                    <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_rows</span><span class="p">(</span>
-</span><span id="L-364"><a href="#L-364"><span class="linenos">364</span></a>                        <span class="n">table</span><span class="p">,</span> <span class="p">[(</span><span class="n">column</span><span class="p">,</span> <span class="n">query_string</span><span class="p">)],</span> <span class="n">exact_match</span><span class="o">=</span><span class="kc">False</span>
-</span><span id="L-365"><a href="#L-365"><span class="linenos">365</span></a>                    <span class="p">)</span>
-</span><span id="L-366"><a href="#L-366"><span class="linenos">366</span></a>                    <span class="k">if</span> <span class="n">row</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">results</span>
-</span><span id="L-367"><a href="#L-367"><span class="linenos">367</span></a>                <span class="p">]</span>
-</span><span id="L-368"><a href="#L-368"><span class="linenos">368</span></a>            <span class="p">)</span>
-</span><span id="L-369"><a href="#L-369"><span class="linenos">369</span></a>        <span class="k">return</span> <span class="n">results</span>
+</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">debug</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">))</span>
+</span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a>
+</span><span id="L-263"><a href="#L-263"><span class="linenos">263</span></a>    <span class="nd">@_connect</span>
+</span><span id="L-264"><a href="#L-264"><span class="linenos">264</span></a>    <span class="k">def</span> <span class="nf">get_rows</span><span class="p">(</span>
+</span><span id="L-265"><a href="#L-265"><span class="linenos">265</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="L-266"><a href="#L-266"><span class="linenos">266</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
+</span><span id="L-267"><a href="#L-267"><span class="linenos">267</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="L-268"><a href="#L-268"><span class="linenos">268</span></a>        <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="L-269"><a href="#L-269"><span class="linenos">269</span></a>        <span class="n">sort_by_column</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="L-270"><a href="#L-270"><span class="linenos">270</span></a>        <span class="n">columns_to_return</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="L-271"><a href="#L-271"><span class="linenos">271</span></a>        <span class="n">return_as_dataframe</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
+</span><span id="L-272"><a href="#L-272"><span class="linenos">272</span></a>        <span class="n">values_only</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
+</span><span id="L-273"><a href="#L-273"><span class="linenos">273</span></a>        <span class="n">order_by</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="L-274"><a href="#L-274"><span class="linenos">274</span></a>        <span class="n">limit</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="L-275"><a href="#L-275"><span class="linenos">275</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]</span> <span class="o">|</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="n">pandas</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">:</span>
+</span><span id="L-276"><a href="#L-276"><span class="linenos">276</span></a>        <span class="sd">&quot;&quot;&quot;Returns rows from table as a list of dictionaries</span>
+</span><span id="L-277"><a href="#L-277"><span class="linenos">277</span></a><span class="sd">        where the key-value pairs of the dictionaries are</span>
+</span><span id="L-278"><a href="#L-278"><span class="linenos">278</span></a><span class="sd">        column name: row value.</span>
+</span><span id="L-279"><a href="#L-279"><span class="linenos">279</span></a>
+</span><span id="L-280"><a href="#L-280"><span class="linenos">280</span></a><span class="sd">        :param match_criteria: Can be a list of 2-tuples where each</span>
+</span><span id="L-281"><a href="#L-281"><span class="linenos">281</span></a><span class="sd">        tuple is (columnName, rowValue) or a dictionary where</span>
+</span><span id="L-282"><a href="#L-282"><span class="linenos">282</span></a><span class="sd">        keys are column names and values are row values.</span>
+</span><span id="L-283"><a href="#L-283"><span class="linenos">283</span></a>
+</span><span id="L-284"><a href="#L-284"><span class="linenos">284</span></a><span class="sd">        :param exact_match: If False, the rowValue for a give column</span>
+</span><span id="L-285"><a href="#L-285"><span class="linenos">285</span></a><span class="sd">        will be matched as a substring.</span>
+</span><span id="L-286"><a href="#L-286"><span class="linenos">286</span></a>
+</span><span id="L-287"><a href="#L-287"><span class="linenos">287</span></a><span class="sd">        :param sort_by_column: A column name to sort the results by.</span>
+</span><span id="L-288"><a href="#L-288"><span class="linenos">288</span></a><span class="sd">        This will sort results in Python after retrieving them from the db.</span>
+</span><span id="L-289"><a href="#L-289"><span class="linenos">289</span></a><span class="sd">        Use the &#39;order_by&#39; param to use SQLite engine for ordering.</span>
+</span><span id="L-290"><a href="#L-290"><span class="linenos">290</span></a>
+</span><span id="L-291"><a href="#L-291"><span class="linenos">291</span></a><span class="sd">        :param columns_to_return: Optional list of column names.</span>
+</span><span id="L-292"><a href="#L-292"><span class="linenos">292</span></a><span class="sd">        If provided, the elements returned by get_rows() will</span>
+</span><span id="L-293"><a href="#L-293"><span class="linenos">293</span></a><span class="sd">        only contain the provided columns. Otherwise every column</span>
+</span><span id="L-294"><a href="#L-294"><span class="linenos">294</span></a><span class="sd">        in the row is returned.</span>
+</span><span id="L-295"><a href="#L-295"><span class="linenos">295</span></a>
+</span><span id="L-296"><a href="#L-296"><span class="linenos">296</span></a><span class="sd">        :param return_as_dataframe: If True,</span>
+</span><span id="L-297"><a href="#L-297"><span class="linenos">297</span></a><span class="sd">        the results will be returned as a pandas.DataFrame object.</span>
+</span><span id="L-298"><a href="#L-298"><span class="linenos">298</span></a>
+</span><span id="L-299"><a href="#L-299"><span class="linenos">299</span></a><span class="sd">        :param values_only: Return the results as a list of tuples</span>
+</span><span id="L-300"><a href="#L-300"><span class="linenos">300</span></a><span class="sd">        instead of a list of dictionaries that have column names as keys.</span>
+</span><span id="L-301"><a href="#L-301"><span class="linenos">301</span></a><span class="sd">        The results will still be sorted according to sort_by_column if</span>
+</span><span id="L-302"><a href="#L-302"><span class="linenos">302</span></a><span class="sd">        one is provided.</span>
+</span><span id="L-303"><a href="#L-303"><span class="linenos">303</span></a>
+</span><span id="L-304"><a href="#L-304"><span class="linenos">304</span></a><span class="sd">        :param order_by: If given, a &#39;order by {order_by}&#39; clause</span>
+</span><span id="L-305"><a href="#L-305"><span class="linenos">305</span></a><span class="sd">        will be added to the select query.</span>
+</span><span id="L-306"><a href="#L-306"><span class="linenos">306</span></a>
+</span><span id="L-307"><a href="#L-307"><span class="linenos">307</span></a><span class="sd">        :param limit: If given, a &#39;limit {limit}&#39; clause will be</span>
+</span><span id="L-308"><a href="#L-308"><span class="linenos">308</span></a><span class="sd">        added to the select query.</span>
+</span><span id="L-309"><a href="#L-309"><span class="linenos">309</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="L-310"><a href="#L-310"><span class="linenos">310</span></a>
+</span><span id="L-311"><a href="#L-311"><span class="linenos">311</span></a>        <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">columns_to_return</span><span class="p">)</span> <span class="ow">is</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="L-312"><a href="#L-312"><span class="linenos">312</span></a>            <span class="n">columns_to_return</span> <span class="o">=</span> <span class="p">[</span><span class="n">columns_to_return</span><span class="p">]</span>
+</span><span id="L-313"><a href="#L-313"><span class="linenos">313</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;select * from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-314"><a href="#L-314"><span class="linenos">314</span></a>        <span class="n">matches</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="L-315"><a href="#L-315"><span class="linenos">315</span></a>        <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
+</span><span id="L-316"><a href="#L-316"><span class="linenos">316</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; where </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-317"><a href="#L-317"><span class="linenos">317</span></a>        <span class="k">if</span> <span class="n">order_by</span><span class="p">:</span>
+</span><span id="L-318"><a href="#L-318"><span class="linenos">318</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; order by </span><span class="si">{</span><span class="n">order_by</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-319"><a href="#L-319"><span class="linenos">319</span></a>        <span class="k">if</span> <span class="n">limit</span><span class="p">:</span>
+</span><span id="L-320"><a href="#L-320"><span class="linenos">320</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; limit </span><span class="si">{</span><span class="n">limit</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-321"><a href="#L-321"><span class="linenos">321</span></a>        <span class="n">query</span> <span class="o">+=</span> <span class="s2">&quot;;&quot;</span>
+</span><span id="L-322"><a href="#L-322"><span class="linenos">322</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
+</span><span id="L-323"><a href="#L-323"><span class="linenos">323</span></a>        <span class="n">matches</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()</span>
+</span><span id="L-324"><a href="#L-324"><span class="linenos">324</span></a>        <span class="n">results</span> <span class="o">=</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_dict</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">match</span><span class="p">,</span> <span class="n">columns_to_return</span><span class="p">)</span> <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">]</span>
+</span><span id="L-325"><a href="#L-325"><span class="linenos">325</span></a>        <span class="k">if</span> <span class="n">sort_by_column</span><span class="p">:</span>
+</span><span id="L-326"><a href="#L-326"><span class="linenos">326</span></a>            <span class="n">results</span> <span class="o">=</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">results</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="k">lambda</span> <span class="n">x</span><span class="p">:</span> <span class="n">x</span><span class="p">[</span><span class="n">sort_by_column</span><span class="p">])</span>
+</span><span id="L-327"><a href="#L-327"><span class="linenos">327</span></a>        <span class="k">if</span> <span class="n">return_as_dataframe</span><span class="p">:</span>
+</span><span id="L-328"><a href="#L-328"><span class="linenos">328</span></a>            <span class="k">return</span> <span class="n">pandas</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">(</span><span class="n">results</span><span class="p">)</span>
+</span><span id="L-329"><a href="#L-329"><span class="linenos">329</span></a>        <span class="k">if</span> <span class="n">values_only</span><span class="p">:</span>
+</span><span id="L-330"><a href="#L-330"><span class="linenos">330</span></a>            <span class="k">return</span> <span class="p">[</span><span class="nb">tuple</span><span class="p">(</span><span class="n">row</span><span class="o">.</span><span class="n">values</span><span class="p">())</span> <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">results</span><span class="p">]</span>
+</span><span id="L-331"><a href="#L-331"><span class="linenos">331</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-332"><a href="#L-332"><span class="linenos">332</span></a>            <span class="k">return</span> <span class="n">results</span>
+</span><span id="L-333"><a href="#L-333"><span class="linenos">333</span></a>
+</span><span id="L-334"><a href="#L-334"><span class="linenos">334</span></a>    <span class="nd">@_connect</span>
+</span><span id="L-335"><a href="#L-335"><span class="linenos">335</span></a>    <span class="k">def</span> <span class="nf">find</span><span class="p">(</span>
+</span><span id="L-336"><a href="#L-336"><span class="linenos">336</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">query_string</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">columns</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="L-337"><a href="#L-337"><span class="linenos">337</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]:</span>
+</span><span id="L-338"><a href="#L-338"><span class="linenos">338</span></a>        <span class="sd">&quot;&quot;&quot;Search for rows that contain query_string as a substring</span>
+</span><span id="L-339"><a href="#L-339"><span class="linenos">339</span></a><span class="sd">        of any column.</span>
+</span><span id="L-340"><a href="#L-340"><span class="linenos">340</span></a>
+</span><span id="L-341"><a href="#L-341"><span class="linenos">341</span></a><span class="sd">        :param table: The table to search.</span>
+</span><span id="L-342"><a href="#L-342"><span class="linenos">342</span></a>
+</span><span id="L-343"><a href="#L-343"><span class="linenos">343</span></a><span class="sd">        :param query_string: The substring to search for in all columns.</span>
+</span><span id="L-344"><a href="#L-344"><span class="linenos">344</span></a>
+</span><span id="L-345"><a href="#L-345"><span class="linenos">345</span></a><span class="sd">        :param columns: A list of columns to search for query_string.</span>
+</span><span id="L-346"><a href="#L-346"><span class="linenos">346</span></a><span class="sd">        If None, all columns in the table will be searched.</span>
+</span><span id="L-347"><a href="#L-347"><span class="linenos">347</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="L-348"><a href="#L-348"><span class="linenos">348</span></a>        <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">columns</span><span class="p">)</span> <span class="ow">is</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="L-349"><a href="#L-349"><span class="linenos">349</span></a>            <span class="n">columns</span> <span class="o">=</span> <span class="p">[</span><span class="n">columns</span><span class="p">]</span>
+</span><span id="L-350"><a href="#L-350"><span class="linenos">350</span></a>        <span class="n">results</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="L-351"><a href="#L-351"><span class="linenos">351</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">columns</span><span class="p">:</span>
+</span><span id="L-352"><a href="#L-352"><span class="linenos">352</span></a>            <span class="n">columns</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_column_names</span><span class="p">(</span><span class="n">table</span><span class="p">)</span>
+</span><span id="L-353"><a href="#L-353"><span class="linenos">353</span></a>        <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span><span class="p">:</span>
+</span><span id="L-354"><a href="#L-354"><span class="linenos">354</span></a>            <span class="n">results</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span>
+</span><span id="L-355"><a href="#L-355"><span class="linenos">355</span></a>                <span class="p">[</span>
+</span><span id="L-356"><a href="#L-356"><span class="linenos">356</span></a>                    <span class="n">row</span>
+</span><span id="L-357"><a href="#L-357"><span class="linenos">357</span></a>                    <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_rows</span><span class="p">(</span>
+</span><span id="L-358"><a href="#L-358"><span class="linenos">358</span></a>                        <span class="n">table</span><span class="p">,</span> <span class="p">[(</span><span class="n">column</span><span class="p">,</span> <span class="n">query_string</span><span class="p">)],</span> <span class="n">exact_match</span><span class="o">=</span><span class="kc">False</span>
+</span><span id="L-359"><a href="#L-359"><span class="linenos">359</span></a>                    <span class="p">)</span>
+</span><span id="L-360"><a href="#L-360"><span class="linenos">360</span></a>                    <span class="k">if</span> <span class="n">row</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">results</span>
+</span><span id="L-361"><a href="#L-361"><span class="linenos">361</span></a>                <span class="p">]</span>
+</span><span id="L-362"><a href="#L-362"><span class="linenos">362</span></a>            <span class="p">)</span>
+</span><span id="L-363"><a href="#L-363"><span class="linenos">363</span></a>        <span class="k">return</span> <span class="n">results</span>
+</span><span id="L-364"><a href="#L-364"><span class="linenos">364</span></a>
+</span><span id="L-365"><a href="#L-365"><span class="linenos">365</span></a>    <span class="nd">@_connect</span>
+</span><span id="L-366"><a href="#L-366"><span class="linenos">366</span></a>    <span class="k">def</span> <span class="nf">delete</span><span class="p">(</span>
+</span><span id="L-367"><a href="#L-367"><span class="linenos">367</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="L-368"><a href="#L-368"><span class="linenos">368</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-369"><a href="#L-369"><span class="linenos">369</span></a>        <span class="sd">&quot;&quot;&quot;Delete records from table.</span>
 </span><span id="L-370"><a href="#L-370"><span class="linenos">370</span></a>
-</span><span id="L-371"><a href="#L-371"><span class="linenos">371</span></a>    <span class="nd">@_connect</span>
-</span><span id="L-372"><a href="#L-372"><span class="linenos">372</span></a>    <span class="k">def</span> <span class="nf">delete</span><span class="p">(</span>
-</span><span id="L-373"><a href="#L-373"><span class="linenos">373</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="L-374"><a href="#L-374"><span class="linenos">374</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-375"><a href="#L-375"><span class="linenos">375</span></a>        <span class="sd">&quot;&quot;&quot;Delete records from table.</span>
+</span><span id="L-371"><a href="#L-371"><span class="linenos">371</span></a><span class="sd">        Returns number of deleted records.</span>
+</span><span id="L-372"><a href="#L-372"><span class="linenos">372</span></a>
+</span><span id="L-373"><a href="#L-373"><span class="linenos">373</span></a><span class="sd">        :param match_criteria: Can be a list of 2-tuples where each</span>
+</span><span id="L-374"><a href="#L-374"><span class="linenos">374</span></a><span class="sd">        tuple is (columnName, rowValue) or a dictionary where</span>
+</span><span id="L-375"><a href="#L-375"><span class="linenos">375</span></a><span class="sd">        keys are column names and values are row values.</span>
 </span><span id="L-376"><a href="#L-376"><span class="linenos">376</span></a>
-</span><span id="L-377"><a href="#L-377"><span class="linenos">377</span></a><span class="sd">        Returns number of deleted records.</span>
-</span><span id="L-378"><a href="#L-378"><span class="linenos">378</span></a>
-</span><span id="L-379"><a href="#L-379"><span class="linenos">379</span></a><span class="sd">        :param match_criteria: Can be a list of 2-tuples where each</span>
-</span><span id="L-380"><a href="#L-380"><span class="linenos">380</span></a><span class="sd">        tuple is (columnName, rowValue) or a dictionary where</span>
-</span><span id="L-381"><a href="#L-381"><span class="linenos">381</span></a><span class="sd">        keys are column names and values are row values.</span>
-</span><span id="L-382"><a href="#L-382"><span class="linenos">382</span></a>
-</span><span id="L-383"><a href="#L-383"><span class="linenos">383</span></a><span class="sd">        :param exact_match: If False, the rowValue for a give column</span>
-</span><span id="L-384"><a href="#L-384"><span class="linenos">384</span></a><span class="sd">        will be matched as a substring.</span>
-</span><span id="L-385"><a href="#L-385"><span class="linenos">385</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="L-386"><a href="#L-386"><span class="linenos">386</span></a>        <span class="n">num_matches</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">count</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span>
-</span><span id="L-387"><a href="#L-387"><span class="linenos">387</span></a>        <span class="n">conditions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span>
-</span><span id="L-388"><a href="#L-388"><span class="linenos">388</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="L-389"><a href="#L-389"><span class="linenos">389</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;delete from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-390"><a href="#L-390"><span class="linenos">390</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
-</span><span id="L-391"><a href="#L-391"><span class="linenos">391</span></a>                <span class="sa">f</span><span class="s1">&#39;Deleted </span><span class="si">{</span><span class="n">num_matches</span><span class="si">}</span><span class="s1"> from &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&quot;.&#39;</span>
-</span><span id="L-392"><a href="#L-392"><span class="linenos">392</span></a>            <span class="p">)</span>
-</span><span id="L-393"><a href="#L-393"><span class="linenos">393</span></a>            <span class="k">return</span> <span class="n">num_matches</span>
-</span><span id="L-394"><a href="#L-394"><span class="linenos">394</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-395"><a href="#L-395"><span class="linenos">395</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">debug</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Error deleting from &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">.</span><span class="se">\n</span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s1">&#39;</span><span class="p">)</span>
-</span><span id="L-396"><a href="#L-396"><span class="linenos">396</span></a>            <span class="k">return</span> <span class="mi">0</span>
-</span><span id="L-397"><a href="#L-397"><span class="linenos">397</span></a>
-</span><span id="L-398"><a href="#L-398"><span class="linenos">398</span></a>    <span class="nd">@_connect</span>
-</span><span id="L-399"><a href="#L-399"><span class="linenos">399</span></a>    <span class="k">def</span> <span class="nf">update</span><span class="p">(</span>
-</span><span id="L-400"><a href="#L-400"><span class="linenos">400</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="L-401"><a href="#L-401"><span class="linenos">401</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
-</span><span id="L-402"><a href="#L-402"><span class="linenos">402</span></a>        <span class="n">column_to_update</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
-</span><span id="L-403"><a href="#L-403"><span class="linenos">403</span></a>        <span class="n">new_value</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
-</span><span id="L-404"><a href="#L-404"><span class="linenos">404</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="L-405"><a href="#L-405"><span class="linenos">405</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="L-406"><a href="#L-406"><span class="linenos">406</span></a>        <span class="sd">&quot;&quot;&quot;Update row value for entry matched with match_criteria.</span>
-</span><span id="L-407"><a href="#L-407"><span class="linenos">407</span></a>
-</span><span id="L-408"><a href="#L-408"><span class="linenos">408</span></a><span class="sd">        :param column_to_update: The column to be updated in the matched row.</span>
-</span><span id="L-409"><a href="#L-409"><span class="linenos">409</span></a>
-</span><span id="L-410"><a href="#L-410"><span class="linenos">410</span></a><span class="sd">        :param new_value: The new value to insert.</span>
-</span><span id="L-411"><a href="#L-411"><span class="linenos">411</span></a>
-</span><span id="L-412"><a href="#L-412"><span class="linenos">412</span></a><span class="sd">        :param match_criteria: Can be a list of 2-tuples where each</span>
-</span><span id="L-413"><a href="#L-413"><span class="linenos">413</span></a><span class="sd">        tuple is (columnName, rowValue) or a dictionary where</span>
-</span><span id="L-414"><a href="#L-414"><span class="linenos">414</span></a><span class="sd">        keys are column names and values are row values.</span>
-</span><span id="L-415"><a href="#L-415"><span class="linenos">415</span></a><span class="sd">        If None, every row will be updated.</span>
-</span><span id="L-416"><a href="#L-416"><span class="linenos">416</span></a>
-</span><span id="L-417"><a href="#L-417"><span class="linenos">417</span></a><span class="sd">        Returns True if successful, False if not.&quot;&quot;&quot;</span>
-</span><span id="L-418"><a href="#L-418"><span class="linenos">418</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;update </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> set </span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s2"> = ?&quot;</span>
-</span><span id="L-419"><a href="#L-419"><span class="linenos">419</span></a>        <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
-</span><span id="L-420"><a href="#L-420"><span class="linenos">420</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">count</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="L-421"><a href="#L-421"><span class="linenos">421</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
-</span><span id="L-422"><a href="#L-422"><span class="linenos">422</span></a>                    <span class="sa">f</span><span class="s2">&quot;Couldn&#39;t find matching records in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table to update to &#39;</span><span class="si">{</span><span class="n">new_value</span><span class="si">}</span><span class="s2">&#39;&quot;</span>
-</span><span id="L-423"><a href="#L-423"><span class="linenos">423</span></a>                <span class="p">)</span>
-</span><span id="L-424"><a href="#L-424"><span class="linenos">424</span></a>                <span class="k">return</span> <span class="kc">False</span>
-</span><span id="L-425"><a href="#L-425"><span class="linenos">425</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">)</span>
-</span><span id="L-426"><a href="#L-426"><span class="linenos">426</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-427"><a href="#L-427"><span class="linenos">427</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="L-428"><a href="#L-428"><span class="linenos">428</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="L-429"><a href="#L-429"><span class="linenos">429</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="L-430"><a href="#L-430"><span class="linenos">430</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="L-431"><a href="#L-431"><span class="linenos">431</span></a>                <span class="n">query</span><span class="p">,</span>
-</span><span id="L-432"><a href="#L-432"><span class="linenos">432</span></a>                <span class="p">(</span><span class="n">new_value</span><span class="p">,),</span>
-</span><span id="L-433"><a href="#L-433"><span class="linenos">433</span></a>            <span class="p">)</span>
-</span><span id="L-434"><a href="#L-434"><span class="linenos">434</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
-</span><span id="L-435"><a href="#L-435"><span class="linenos">435</span></a>                <span class="sa">f</span><span class="s1">&#39;Updated &quot;</span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s1">&quot; in &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table to &quot;</span><span class="si">{</span><span class="n">new_value</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&#39;</span>
+</span><span id="L-377"><a href="#L-377"><span class="linenos">377</span></a><span class="sd">        :param exact_match: If False, the rowValue for a give column</span>
+</span><span id="L-378"><a href="#L-378"><span class="linenos">378</span></a><span class="sd">        will be matched as a substring.</span>
+</span><span id="L-379"><a href="#L-379"><span class="linenos">379</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="L-380"><a href="#L-380"><span class="linenos">380</span></a>        <span class="n">num_matches</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">count</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span>
+</span><span id="L-381"><a href="#L-381"><span class="linenos">381</span></a>        <span class="n">conditions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span>
+</span><span id="L-382"><a href="#L-382"><span class="linenos">382</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="L-383"><a href="#L-383"><span class="linenos">383</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;delete from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-384"><a href="#L-384"><span class="linenos">384</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
+</span><span id="L-385"><a href="#L-385"><span class="linenos">385</span></a>                <span class="sa">f</span><span class="s1">&#39;Deleted </span><span class="si">{</span><span class="n">num_matches</span><span class="si">}</span><span class="s1"> from &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&quot;.&#39;</span>
+</span><span id="L-386"><a href="#L-386"><span class="linenos">386</span></a>            <span class="p">)</span>
+</span><span id="L-387"><a href="#L-387"><span class="linenos">387</span></a>            <span class="k">return</span> <span class="n">num_matches</span>
+</span><span id="L-388"><a href="#L-388"><span class="linenos">388</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-389"><a href="#L-389"><span class="linenos">389</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">debug</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Error deleting from &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">.</span><span class="se">\n</span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s1">&#39;</span><span class="p">)</span>
+</span><span id="L-390"><a href="#L-390"><span class="linenos">390</span></a>            <span class="k">return</span> <span class="mi">0</span>
+</span><span id="L-391"><a href="#L-391"><span class="linenos">391</span></a>
+</span><span id="L-392"><a href="#L-392"><span class="linenos">392</span></a>    <span class="nd">@_connect</span>
+</span><span id="L-393"><a href="#L-393"><span class="linenos">393</span></a>    <span class="k">def</span> <span class="nf">update</span><span class="p">(</span>
+</span><span id="L-394"><a href="#L-394"><span class="linenos">394</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="L-395"><a href="#L-395"><span class="linenos">395</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
+</span><span id="L-396"><a href="#L-396"><span class="linenos">396</span></a>        <span class="n">column_to_update</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
+</span><span id="L-397"><a href="#L-397"><span class="linenos">397</span></a>        <span class="n">new_value</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
+</span><span id="L-398"><a href="#L-398"><span class="linenos">398</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="L-399"><a href="#L-399"><span class="linenos">399</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="L-400"><a href="#L-400"><span class="linenos">400</span></a>        <span class="sd">&quot;&quot;&quot;Update row value for entry matched with match_criteria.</span>
+</span><span id="L-401"><a href="#L-401"><span class="linenos">401</span></a>
+</span><span id="L-402"><a href="#L-402"><span class="linenos">402</span></a><span class="sd">        :param column_to_update: The column to be updated in the matched row.</span>
+</span><span id="L-403"><a href="#L-403"><span class="linenos">403</span></a>
+</span><span id="L-404"><a href="#L-404"><span class="linenos">404</span></a><span class="sd">        :param new_value: The new value to insert.</span>
+</span><span id="L-405"><a href="#L-405"><span class="linenos">405</span></a>
+</span><span id="L-406"><a href="#L-406"><span class="linenos">406</span></a><span class="sd">        :param match_criteria: Can be a list of 2-tuples where each</span>
+</span><span id="L-407"><a href="#L-407"><span class="linenos">407</span></a><span class="sd">        tuple is (columnName, rowValue) or a dictionary where</span>
+</span><span id="L-408"><a href="#L-408"><span class="linenos">408</span></a><span class="sd">        keys are column names and values are row values.</span>
+</span><span id="L-409"><a href="#L-409"><span class="linenos">409</span></a><span class="sd">        If None, every row will be updated.</span>
+</span><span id="L-410"><a href="#L-410"><span class="linenos">410</span></a>
+</span><span id="L-411"><a href="#L-411"><span class="linenos">411</span></a><span class="sd">        Returns True if successful, False if not.&quot;&quot;&quot;</span>
+</span><span id="L-412"><a href="#L-412"><span class="linenos">412</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;update </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> set </span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s2"> = ?&quot;</span>
+</span><span id="L-413"><a href="#L-413"><span class="linenos">413</span></a>        <span class="n">conditions</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="L-414"><a href="#L-414"><span class="linenos">414</span></a>        <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
+</span><span id="L-415"><a href="#L-415"><span class="linenos">415</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">count</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="L-416"><a href="#L-416"><span class="linenos">416</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
+</span><span id="L-417"><a href="#L-417"><span class="linenos">417</span></a>                    <span class="sa">f</span><span class="s2">&quot;Couldn&#39;t find matching records in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table to update to &#39;</span><span class="si">{</span><span class="n">new_value</span><span class="si">}</span><span class="s2">&#39;&quot;</span>
+</span><span id="L-418"><a href="#L-418"><span class="linenos">418</span></a>                <span class="p">)</span>
+</span><span id="L-419"><a href="#L-419"><span class="linenos">419</span></a>                <span class="k">return</span> <span class="kc">False</span>
+</span><span id="L-420"><a href="#L-420"><span class="linenos">420</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">)</span>
+</span><span id="L-421"><a href="#L-421"><span class="linenos">421</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-422"><a href="#L-422"><span class="linenos">422</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-423"><a href="#L-423"><span class="linenos">423</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="L-424"><a href="#L-424"><span class="linenos">424</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="L-425"><a href="#L-425"><span class="linenos">425</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="L-426"><a href="#L-426"><span class="linenos">426</span></a>                <span class="n">query</span><span class="p">,</span>
+</span><span id="L-427"><a href="#L-427"><span class="linenos">427</span></a>                <span class="p">(</span><span class="n">new_value</span><span class="p">,),</span>
+</span><span id="L-428"><a href="#L-428"><span class="linenos">428</span></a>            <span class="p">)</span>
+</span><span id="L-429"><a href="#L-429"><span class="linenos">429</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
+</span><span id="L-430"><a href="#L-430"><span class="linenos">430</span></a>                <span class="sa">f</span><span class="s1">&#39;Updated &quot;</span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s1">&quot; in &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table to &quot;</span><span class="si">{</span><span class="n">new_value</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&#39;</span>
+</span><span id="L-431"><a href="#L-431"><span class="linenos">431</span></a>            <span class="p">)</span>
+</span><span id="L-432"><a href="#L-432"><span class="linenos">432</span></a>            <span class="k">return</span> <span class="kc">True</span>
+</span><span id="L-433"><a href="#L-433"><span class="linenos">433</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-434"><a href="#L-434"><span class="linenos">434</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span>
+</span><span id="L-435"><a href="#L-435"><span class="linenos">435</span></a>                <span class="sa">f</span><span class="s1">&#39;Failed to update &quot;</span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s1">&quot; in &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table to &quot;</span><span class="si">{</span><span class="n">new_value</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&quot;</span><span class="se">\n</span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s1">&#39;</span>
 </span><span id="L-436"><a href="#L-436"><span class="linenos">436</span></a>            <span class="p">)</span>
-</span><span id="L-437"><a href="#L-437"><span class="linenos">437</span></a>            <span class="k">return</span> <span class="kc">True</span>
-</span><span id="L-438"><a href="#L-438"><span class="linenos">438</span></a>        <span class="k">except</span> <span class="ne">UnboundLocalError</span><span class="p">:</span>
-</span><span id="L-439"><a href="#L-439"><span class="linenos">439</span></a>            <span class="n">table_filter_string</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
-</span><span id="L-440"><a href="#L-440"><span class="linenos">440</span></a>                <span class="n">table_filter</span> <span class="k">for</span> <span class="n">table_filter</span> <span class="ow">in</span> <span class="n">match_criteria</span>
-</span><span id="L-441"><a href="#L-441"><span class="linenos">441</span></a>            <span class="p">)</span>
-</span><span id="L-442"><a href="#L-442"><span class="linenos">442</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span>
-</span><span id="L-443"><a href="#L-443"><span class="linenos">443</span></a>                <span class="sa">f</span><span class="s2">&quot;No records found matching filters: </span><span class="si">{</span><span class="n">table_filter_string</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-444"><a href="#L-444"><span class="linenos">444</span></a>            <span class="p">)</span>
-</span><span id="L-445"><a href="#L-445"><span class="linenos">445</span></a>            <span class="k">return</span> <span class="kc">False</span>
-</span><span id="L-446"><a href="#L-446"><span class="linenos">446</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-447"><a href="#L-447"><span class="linenos">447</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span>
-</span><span id="L-448"><a href="#L-448"><span class="linenos">448</span></a>                <span class="sa">f</span><span class="s1">&#39;Failed to update &quot;</span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s1">&quot; in &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table to &quot;</span><span class="si">{</span><span class="n">new_value</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&quot;</span><span class="se">\n</span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s1">&#39;</span>
-</span><span id="L-449"><a href="#L-449"><span class="linenos">449</span></a>            <span class="p">)</span>
-</span><span id="L-450"><a href="#L-450"><span class="linenos">450</span></a>            <span class="k">return</span> <span class="kc">False</span>
-</span><span id="L-451"><a href="#L-451"><span class="linenos">451</span></a>
-</span><span id="L-452"><a href="#L-452"><span class="linenos">452</span></a>    <span class="nd">@_connect</span>
-</span><span id="L-453"><a href="#L-453"><span class="linenos">453</span></a>    <span class="k">def</span> <span class="nf">drop_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="L-454"><a href="#L-454"><span class="linenos">454</span></a>        <span class="sd">&quot;&quot;&quot;Drop a table from the database.</span>
-</span><span id="L-455"><a href="#L-455"><span class="linenos">455</span></a>
-</span><span id="L-456"><a href="#L-456"><span class="linenos">456</span></a><span class="sd">        Returns True if successful, False if not.&quot;&quot;&quot;</span>
-</span><span id="L-457"><a href="#L-457"><span class="linenos">457</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="L-458"><a href="#L-458"><span class="linenos">458</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;drop Table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-459"><a href="#L-459"><span class="linenos">459</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Dropped table &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
-</span><span id="L-460"><a href="#L-460"><span class="linenos">460</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-461"><a href="#L-461"><span class="linenos">461</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
-</span><span id="L-462"><a href="#L-462"><span class="linenos">462</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Failed to drop table &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
-</span><span id="L-463"><a href="#L-463"><span class="linenos">463</span></a>
-</span><span id="L-464"><a href="#L-464"><span class="linenos">464</span></a>    <span class="nd">@_connect</span>
-</span><span id="L-465"><a href="#L-465"><span class="linenos">465</span></a>    <span class="k">def</span> <span class="nf">add_column</span><span class="p">(</span>
-</span><span id="L-466"><a href="#L-466"><span class="linenos">466</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">column</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">_type</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">default_value</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="L-467"><a href="#L-467"><span class="linenos">467</span></a>    <span class="p">):</span>
-</span><span id="L-468"><a href="#L-468"><span class="linenos">468</span></a>        <span class="sd">&quot;&quot;&quot;Add a new column to table.</span>
-</span><span id="L-469"><a href="#L-469"><span class="linenos">469</span></a>
-</span><span id="L-470"><a href="#L-470"><span class="linenos">470</span></a><span class="sd">        :param column: Name of the column to add.</span>
-</span><span id="L-471"><a href="#L-471"><span class="linenos">471</span></a>
-</span><span id="L-472"><a href="#L-472"><span class="linenos">472</span></a><span class="sd">        :param _type: The data type of the new column.</span>
-</span><span id="L-473"><a href="#L-473"><span class="linenos">473</span></a>
-</span><span id="L-474"><a href="#L-474"><span class="linenos">474</span></a><span class="sd">        :param default_value: Optional default value for the column.&quot;&quot;&quot;</span>
-</span><span id="L-475"><a href="#L-475"><span class="linenos">475</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="L-476"><a href="#L-476"><span class="linenos">476</span></a>            <span class="k">if</span> <span class="n">default_value</span><span class="p">:</span>
-</span><span id="L-477"><a href="#L-477"><span class="linenos">477</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="L-478"><a href="#L-478"><span class="linenos">478</span></a>                    <span class="sa">f</span><span class="s2">&quot;alter table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> add column </span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">_type</span><span class="si">}</span><span class="s2"> default </span><span class="si">{</span><span class="n">default_value</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-479"><a href="#L-479"><span class="linenos">479</span></a>                <span class="p">)</span>
-</span><span id="L-480"><a href="#L-480"><span class="linenos">480</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="L-481"><a href="#L-481"><span class="linenos">481</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;alter table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> add column </span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">_type</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-482"><a href="#L-482"><span class="linenos">482</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Added column &quot;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1">&quot; to &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table.&#39;</span><span class="p">)</span>
-</span><span id="L-483"><a href="#L-483"><span class="linenos">483</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-484"><a href="#L-484"><span class="linenos">484</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Failed to add column &quot;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1">&quot; to &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table.&#39;</span><span class="p">)</span>
+</span><span id="L-437"><a href="#L-437"><span class="linenos">437</span></a>            <span class="k">return</span> <span class="kc">False</span>
+</span><span id="L-438"><a href="#L-438"><span class="linenos">438</span></a>
+</span><span id="L-439"><a href="#L-439"><span class="linenos">439</span></a>    <span class="nd">@_connect</span>
+</span><span id="L-440"><a href="#L-440"><span class="linenos">440</span></a>    <span class="k">def</span> <span class="nf">drop_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="L-441"><a href="#L-441"><span class="linenos">441</span></a>        <span class="sd">&quot;&quot;&quot;Drop a table from the database.</span>
+</span><span id="L-442"><a href="#L-442"><span class="linenos">442</span></a>
+</span><span id="L-443"><a href="#L-443"><span class="linenos">443</span></a><span class="sd">        Returns True if successful, False if not.&quot;&quot;&quot;</span>
+</span><span id="L-444"><a href="#L-444"><span class="linenos">444</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="L-445"><a href="#L-445"><span class="linenos">445</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;drop Table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-446"><a href="#L-446"><span class="linenos">446</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Dropped table &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
+</span><span id="L-447"><a href="#L-447"><span class="linenos">447</span></a>            <span class="k">return</span> <span class="kc">True</span>
+</span><span id="L-448"><a href="#L-448"><span class="linenos">448</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-449"><a href="#L-449"><span class="linenos">449</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
+</span><span id="L-450"><a href="#L-450"><span class="linenos">450</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Failed to drop table &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
+</span><span id="L-451"><a href="#L-451"><span class="linenos">451</span></a>            <span class="k">return</span> <span class="kc">False</span>
+</span><span id="L-452"><a href="#L-452"><span class="linenos">452</span></a>
+</span><span id="L-453"><a href="#L-453"><span class="linenos">453</span></a>    <span class="nd">@_connect</span>
+</span><span id="L-454"><a href="#L-454"><span class="linenos">454</span></a>    <span class="k">def</span> <span class="nf">add_column</span><span class="p">(</span>
+</span><span id="L-455"><a href="#L-455"><span class="linenos">455</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">column</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">_type</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">default_value</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="L-456"><a href="#L-456"><span class="linenos">456</span></a>    <span class="p">):</span>
+</span><span id="L-457"><a href="#L-457"><span class="linenos">457</span></a>        <span class="sd">&quot;&quot;&quot;Add a new column to table.</span>
+</span><span id="L-458"><a href="#L-458"><span class="linenos">458</span></a>
+</span><span id="L-459"><a href="#L-459"><span class="linenos">459</span></a><span class="sd">        :param column: Name of the column to add.</span>
+</span><span id="L-460"><a href="#L-460"><span class="linenos">460</span></a>
+</span><span id="L-461"><a href="#L-461"><span class="linenos">461</span></a><span class="sd">        :param _type: The data type of the new column.</span>
+</span><span id="L-462"><a href="#L-462"><span class="linenos">462</span></a>
+</span><span id="L-463"><a href="#L-463"><span class="linenos">463</span></a><span class="sd">        :param default_value: Optional default value for the column.&quot;&quot;&quot;</span>
+</span><span id="L-464"><a href="#L-464"><span class="linenos">464</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="L-465"><a href="#L-465"><span class="linenos">465</span></a>            <span class="k">if</span> <span class="n">default_value</span><span class="p">:</span>
+</span><span id="L-466"><a href="#L-466"><span class="linenos">466</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="L-467"><a href="#L-467"><span class="linenos">467</span></a>                    <span class="sa">f</span><span class="s2">&quot;alter table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> add column </span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">_type</span><span class="si">}</span><span class="s2"> default </span><span class="si">{</span><span class="n">default_value</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-468"><a href="#L-468"><span class="linenos">468</span></a>                <span class="p">)</span>
+</span><span id="L-469"><a href="#L-469"><span class="linenos">469</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="L-470"><a href="#L-470"><span class="linenos">470</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;alter table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> add column </span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">_type</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-471"><a href="#L-471"><span class="linenos">471</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Added column &quot;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1">&quot; to &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table.&#39;</span><span class="p">)</span>
+</span><span id="L-472"><a href="#L-472"><span class="linenos">472</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-473"><a href="#L-473"><span class="linenos">473</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Failed to add column &quot;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1">&quot; to &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table.&#39;</span><span class="p">)</span>
+</span><span id="L-474"><a href="#L-474"><span class="linenos">474</span></a>
+</span><span id="L-475"><a href="#L-475"><span class="linenos">475</span></a>    <span class="nd">@staticmethod</span>
+</span><span id="L-476"><a href="#L-476"><span class="linenos">476</span></a>    <span class="k">def</span> <span class="nf">data_to_string</span><span class="p">(</span>
+</span><span id="L-477"><a href="#L-477"><span class="linenos">477</span></a>        <span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">],</span> <span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="L-478"><a href="#L-478"><span class="linenos">478</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="L-479"><a href="#L-479"><span class="linenos">479</span></a>        <span class="sd">&quot;&quot;&quot;Uses tabulate to produce pretty string output</span>
+</span><span id="L-480"><a href="#L-480"><span class="linenos">480</span></a><span class="sd">        from a list of dictionaries.</span>
+</span><span id="L-481"><a href="#L-481"><span class="linenos">481</span></a>
+</span><span id="L-482"><a href="#L-482"><span class="linenos">482</span></a><span class="sd">        :param data: Assumes all dictionaries in list have the same set of keys.</span>
+</span><span id="L-483"><a href="#L-483"><span class="linenos">483</span></a>
+</span><span id="L-484"><a href="#L-484"><span class="linenos">484</span></a><span class="sd">        :param sort_key: Optional dictionary key to sort data with.</span>
 </span><span id="L-485"><a href="#L-485"><span class="linenos">485</span></a>
-</span><span id="L-486"><a href="#L-486"><span class="linenos">486</span></a>    <span class="nd">@staticmethod</span>
-</span><span id="L-487"><a href="#L-487"><span class="linenos">487</span></a>    <span class="k">def</span> <span class="nf">data_to_string</span><span class="p">(</span>
-</span><span id="L-488"><a href="#L-488"><span class="linenos">488</span></a>        <span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">],</span> <span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="L-489"><a href="#L-489"><span class="linenos">489</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="L-490"><a href="#L-490"><span class="linenos">490</span></a>        <span class="sd">&quot;&quot;&quot;Uses tabulate to produce pretty string output</span>
-</span><span id="L-491"><a href="#L-491"><span class="linenos">491</span></a><span class="sd">        from a list of dictionaries.</span>
-</span><span id="L-492"><a href="#L-492"><span class="linenos">492</span></a>
-</span><span id="L-493"><a href="#L-493"><span class="linenos">493</span></a><span class="sd">        :param data: Assumes all dictionaries in list have the same set of keys.</span>
-</span><span id="L-494"><a href="#L-494"><span class="linenos">494</span></a>
-</span><span id="L-495"><a href="#L-495"><span class="linenos">495</span></a><span class="sd">        :param sort_key: Optional dictionary key to sort data with.</span>
+</span><span id="L-486"><a href="#L-486"><span class="linenos">486</span></a><span class="sd">        :param wrap_to_terminal: If True, the table width will be wrapped</span>
+</span><span id="L-487"><a href="#L-487"><span class="linenos">487</span></a><span class="sd">        to fit within the current terminal window. Set to False</span>
+</span><span id="L-488"><a href="#L-488"><span class="linenos">488</span></a><span class="sd">        if the output is going into something like a txt file.&quot;&quot;&quot;</span>
+</span><span id="L-489"><a href="#L-489"><span class="linenos">489</span></a>        <span class="k">return</span> <span class="n">data_to_string</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">sort_key</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">)</span>
+</span><span id="L-490"><a href="#L-490"><span class="linenos">490</span></a>
+</span><span id="L-491"><a href="#L-491"><span class="linenos">491</span></a>
+</span><span id="L-492"><a href="#L-492"><span class="linenos">492</span></a><span class="k">def</span> <span class="nf">data_to_string</span><span class="p">(</span>
+</span><span id="L-493"><a href="#L-493"><span class="linenos">493</span></a>    <span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">],</span> <span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="L-494"><a href="#L-494"><span class="linenos">494</span></a><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="L-495"><a href="#L-495"><span class="linenos">495</span></a>    <span class="sd">&quot;&quot;&quot;Use tabulate to produce grid output from a list of dictionaries.</span>
 </span><span id="L-496"><a href="#L-496"><span class="linenos">496</span></a>
-</span><span id="L-497"><a href="#L-497"><span class="linenos">497</span></a><span class="sd">        :param wrap_to_terminal: If True, the table width will be wrapped</span>
-</span><span id="L-498"><a href="#L-498"><span class="linenos">498</span></a><span class="sd">        to fit within the current terminal window. Set to False</span>
-</span><span id="L-499"><a href="#L-499"><span class="linenos">499</span></a><span class="sd">        if the output is going into something like a txt file.&quot;&quot;&quot;</span>
-</span><span id="L-500"><a href="#L-500"><span class="linenos">500</span></a>        <span class="k">return</span> <span class="n">data_to_string</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">sort_key</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">)</span>
-</span><span id="L-501"><a href="#L-501"><span class="linenos">501</span></a>
-</span><span id="L-502"><a href="#L-502"><span class="linenos">502</span></a>
-</span><span id="L-503"><a href="#L-503"><span class="linenos">503</span></a><span class="k">def</span> <span class="nf">data_to_string</span><span class="p">(</span>
-</span><span id="L-504"><a href="#L-504"><span class="linenos">504</span></a>    <span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">],</span> <span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="L-505"><a href="#L-505"><span class="linenos">505</span></a><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="L-506"><a href="#L-506"><span class="linenos">506</span></a>    <span class="sd">&quot;&quot;&quot;Use tabulate to produce grid output from a list of dictionaries.</span>
-</span><span id="L-507"><a href="#L-507"><span class="linenos">507</span></a>
-</span><span id="L-508"><a href="#L-508"><span class="linenos">508</span></a><span class="sd">    :param data: Assumes all dictionaries in list have the same set of keys.</span>
-</span><span id="L-509"><a href="#L-509"><span class="linenos">509</span></a>
-</span><span id="L-510"><a href="#L-510"><span class="linenos">510</span></a><span class="sd">    :param sort_key: Optional dictionary key to sort data with.</span>
+</span><span id="L-497"><a href="#L-497"><span class="linenos">497</span></a><span class="sd">    :param data: Assumes all dictionaries in list have the same set of keys.</span>
+</span><span id="L-498"><a href="#L-498"><span class="linenos">498</span></a>
+</span><span id="L-499"><a href="#L-499"><span class="linenos">499</span></a><span class="sd">    :param sort_key: Optional dictionary key to sort data with.</span>
+</span><span id="L-500"><a href="#L-500"><span class="linenos">500</span></a>
+</span><span id="L-501"><a href="#L-501"><span class="linenos">501</span></a><span class="sd">    :param wrap_to_terminal: If True, the column widths will be reduced so the grid fits</span>
+</span><span id="L-502"><a href="#L-502"><span class="linenos">502</span></a><span class="sd">    within the current terminal window without wrapping. If the column widths have reduced to 1</span>
+</span><span id="L-503"><a href="#L-503"><span class="linenos">503</span></a><span class="sd">    and the grid is still too wide, str(data) will be returned.&quot;&quot;&quot;</span>
+</span><span id="L-504"><a href="#L-504"><span class="linenos">504</span></a>    <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">data</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="L-505"><a href="#L-505"><span class="linenos">505</span></a>        <span class="k">return</span> <span class="s2">&quot;&quot;</span>
+</span><span id="L-506"><a href="#L-506"><span class="linenos">506</span></a>    <span class="k">if</span> <span class="n">sort_key</span><span class="p">:</span>
+</span><span id="L-507"><a href="#L-507"><span class="linenos">507</span></a>        <span class="n">data</span> <span class="o">=</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="k">lambda</span> <span class="n">d</span><span class="p">:</span> <span class="n">d</span><span class="p">[</span><span class="n">sort_key</span><span class="p">])</span>
+</span><span id="L-508"><a href="#L-508"><span class="linenos">508</span></a>    <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">d</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">data</span><span class="p">):</span>
+</span><span id="L-509"><a href="#L-509"><span class="linenos">509</span></a>        <span class="k">for</span> <span class="n">k</span> <span class="ow">in</span> <span class="n">d</span><span class="p">:</span>
+</span><span id="L-510"><a href="#L-510"><span class="linenos">510</span></a>            <span class="n">data</span><span class="p">[</span><span class="n">i</span><span class="p">][</span><span class="n">k</span><span class="p">]</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="n">data</span><span class="p">[</span><span class="n">i</span><span class="p">][</span><span class="n">k</span><span class="p">])</span>
 </span><span id="L-511"><a href="#L-511"><span class="linenos">511</span></a>
-</span><span id="L-512"><a href="#L-512"><span class="linenos">512</span></a><span class="sd">    :param wrap_to_terminal: If True, the column widths will be reduced so the grid fits</span>
-</span><span id="L-513"><a href="#L-513"><span class="linenos">513</span></a><span class="sd">    within the current terminal window without wrapping. If the column widths have reduced to 1</span>
-</span><span id="L-514"><a href="#L-514"><span class="linenos">514</span></a><span class="sd">    and the grid is still too wide, str(data) will be returned.&quot;&quot;&quot;</span>
-</span><span id="L-515"><a href="#L-515"><span class="linenos">515</span></a>    <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">data</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="L-516"><a href="#L-516"><span class="linenos">516</span></a>        <span class="k">return</span> <span class="s2">&quot;&quot;</span>
-</span><span id="L-517"><a href="#L-517"><span class="linenos">517</span></a>    <span class="k">if</span> <span class="n">sort_key</span><span class="p">:</span>
-</span><span id="L-518"><a href="#L-518"><span class="linenos">518</span></a>        <span class="n">data</span> <span class="o">=</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="k">lambda</span> <span class="n">d</span><span class="p">:</span> <span class="n">d</span><span class="p">[</span><span class="n">sort_key</span><span class="p">])</span>
-</span><span id="L-519"><a href="#L-519"><span class="linenos">519</span></a>    <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">d</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">data</span><span class="p">):</span>
-</span><span id="L-520"><a href="#L-520"><span class="linenos">520</span></a>        <span class="k">for</span> <span class="n">k</span> <span class="ow">in</span> <span class="n">d</span><span class="p">:</span>
-</span><span id="L-521"><a href="#L-521"><span class="linenos">521</span></a>            <span class="n">data</span><span class="p">[</span><span class="n">i</span><span class="p">][</span><span class="n">k</span><span class="p">]</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="n">data</span><span class="p">[</span><span class="n">i</span><span class="p">][</span><span class="n">k</span><span class="p">])</span>
-</span><span id="L-522"><a href="#L-522"><span class="linenos">522</span></a>
-</span><span id="L-523"><a href="#L-523"><span class="linenos">523</span></a>    <span class="n">too_wide</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="L-524"><a href="#L-524"><span class="linenos">524</span></a>    <span class="n">terminal_width</span> <span class="o">=</span> <span class="n">os</span><span class="o">.</span><span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span>
-</span><span id="L-525"><a href="#L-525"><span class="linenos">525</span></a>    <span class="n">max_col_widths</span> <span class="o">=</span> <span class="n">terminal_width</span>
-</span><span id="L-526"><a href="#L-526"><span class="linenos">526</span></a>    <span class="c1"># Make an output with effectively unrestricted column widths</span>
-</span><span id="L-527"><a href="#L-527"><span class="linenos">527</span></a>    <span class="c1"># to see if shrinking is necessary</span>
-</span><span id="L-528"><a href="#L-528"><span class="linenos">528</span></a>    <span class="n">output</span> <span class="o">=</span> <span class="n">tabulate</span><span class="p">(</span>
-</span><span id="L-529"><a href="#L-529"><span class="linenos">529</span></a>        <span class="n">data</span><span class="p">,</span>
-</span><span id="L-530"><a href="#L-530"><span class="linenos">530</span></a>        <span class="n">headers</span><span class="o">=</span><span class="s2">&quot;keys&quot;</span><span class="p">,</span>
-</span><span id="L-531"><a href="#L-531"><span class="linenos">531</span></a>        <span class="n">disable_numparse</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
-</span><span id="L-532"><a href="#L-532"><span class="linenos">532</span></a>        <span class="n">tablefmt</span><span class="o">=</span><span class="s2">&quot;grid&quot;</span><span class="p">,</span>
-</span><span id="L-533"><a href="#L-533"><span class="linenos">533</span></a>        <span class="n">maxcolwidths</span><span class="o">=</span><span class="n">max_col_widths</span><span class="p">,</span>
-</span><span id="L-534"><a href="#L-534"><span class="linenos">534</span></a>    <span class="p">)</span>
-</span><span id="L-535"><a href="#L-535"><span class="linenos">535</span></a>    <span class="n">current_width</span> <span class="o">=</span> <span class="n">output</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-536"><a href="#L-536"><span class="linenos">536</span></a>    <span class="k">if</span> <span class="n">current_width</span> <span class="o">&lt;</span> <span class="n">terminal_width</span><span class="p">:</span>
-</span><span id="L-537"><a href="#L-537"><span class="linenos">537</span></a>        <span class="n">too_wide</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="L-538"><a href="#L-538"><span class="linenos">538</span></a>    <span class="k">if</span> <span class="n">wrap_to_terminal</span> <span class="ow">and</span> <span class="n">too_wide</span><span class="p">:</span>
-</span><span id="L-539"><a href="#L-539"><span class="linenos">539</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Resizing grid to fit within the terminal...&quot;</span><span class="p">)</span>
-</span><span id="L-540"><a href="#L-540"><span class="linenos">540</span></a>        <span class="n">previous_col_widths</span> <span class="o">=</span> <span class="n">max_col_widths</span>
-</span><span id="L-541"><a href="#L-541"><span class="linenos">541</span></a>        <span class="n">acceptable_width</span> <span class="o">=</span> <span class="n">terminal_width</span> <span class="o">-</span> <span class="mi">10</span>
-</span><span id="L-542"><a href="#L-542"><span class="linenos">542</span></a>        <span class="k">while</span> <span class="n">too_wide</span> <span class="ow">and</span> <span class="n">max_col_widths</span> <span class="o">&gt;</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="L-543"><a href="#L-543"><span class="linenos">543</span></a>            <span class="k">if</span> <span class="n">current_width</span> <span class="o">&gt;</span> <span class="n">terminal_width</span><span class="p">:</span>
-</span><span id="L-544"><a href="#L-544"><span class="linenos">544</span></a>                <span class="n">previous_col_widths</span> <span class="o">=</span> <span class="n">max_col_widths</span>
-</span><span id="L-545"><a href="#L-545"><span class="linenos">545</span></a>                <span class="n">max_col_widths</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="n">max_col_widths</span> <span class="o">*</span> <span class="mf">0.5</span><span class="p">)</span>
-</span><span id="L-546"><a href="#L-546"><span class="linenos">546</span></a>            <span class="k">elif</span> <span class="n">current_width</span> <span class="o">&lt;</span> <span class="n">terminal_width</span><span class="p">:</span>
-</span><span id="L-547"><a href="#L-547"><span class="linenos">547</span></a>                <span class="c1"># Without lowering acceptable_width, this condition will cause infinite loop</span>
-</span><span id="L-548"><a href="#L-548"><span class="linenos">548</span></a>                <span class="k">if</span> <span class="n">max_col_widths</span> <span class="o">==</span> <span class="n">previous_col_widths</span> <span class="o">-</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="L-549"><a href="#L-549"><span class="linenos">549</span></a>                    <span class="n">acceptable_width</span> <span class="o">-=</span> <span class="mi">10</span>
-</span><span id="L-550"><a href="#L-550"><span class="linenos">550</span></a>                <span class="n">max_col_widths</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span>
-</span><span id="L-551"><a href="#L-551"><span class="linenos">551</span></a>                    <span class="n">max_col_widths</span> <span class="o">+</span> <span class="p">(</span><span class="mf">0.5</span> <span class="o">*</span> <span class="p">(</span><span class="n">previous_col_widths</span> <span class="o">-</span> <span class="n">max_col_widths</span><span class="p">))</span>
-</span><span id="L-552"><a href="#L-552"><span class="linenos">552</span></a>                <span class="p">)</span>
-</span><span id="L-553"><a href="#L-553"><span class="linenos">553</span></a>            <span class="n">output</span> <span class="o">=</span> <span class="n">tabulate</span><span class="p">(</span>
-</span><span id="L-554"><a href="#L-554"><span class="linenos">554</span></a>                <span class="n">data</span><span class="p">,</span>
-</span><span id="L-555"><a href="#L-555"><span class="linenos">555</span></a>                <span class="n">headers</span><span class="o">=</span><span class="s2">&quot;keys&quot;</span><span class="p">,</span>
-</span><span id="L-556"><a href="#L-556"><span class="linenos">556</span></a>                <span class="n">disable_numparse</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
-</span><span id="L-557"><a href="#L-557"><span class="linenos">557</span></a>                <span class="n">tablefmt</span><span class="o">=</span><span class="s2">&quot;grid&quot;</span><span class="p">,</span>
-</span><span id="L-558"><a href="#L-558"><span class="linenos">558</span></a>                <span class="n">maxcolwidths</span><span class="o">=</span><span class="n">max_col_widths</span><span class="p">,</span>
-</span><span id="L-559"><a href="#L-559"><span class="linenos">559</span></a>            <span class="p">)</span>
-</span><span id="L-560"><a href="#L-560"><span class="linenos">560</span></a>            <span class="n">current_width</span> <span class="o">=</span> <span class="n">output</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-561"><a href="#L-561"><span class="linenos">561</span></a>            <span class="k">if</span> <span class="n">acceptable_width</span> <span class="o">&lt;</span> <span class="n">current_width</span> <span class="o">&lt;</span> <span class="n">terminal_width</span><span class="p">:</span>
-</span><span id="L-562"><a href="#L-562"><span class="linenos">562</span></a>                <span class="n">too_wide</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="L-563"><a href="#L-563"><span class="linenos">563</span></a>        <span class="k">if</span> <span class="n">too_wide</span><span class="p">:</span>
-</span><span id="L-564"><a href="#L-564"><span class="linenos">564</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Couldn&#39;t resize grid to fit within the terminal.&quot;</span><span class="p">)</span>
-</span><span id="L-565"><a href="#L-565"><span class="linenos">565</span></a>            <span class="k">return</span> <span class="nb">str</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
-</span><span id="L-566"><a href="#L-566"><span class="linenos">566</span></a>    <span class="k">return</span> <span class="n">output</span>
+</span><span id="L-512"><a href="#L-512"><span class="linenos">512</span></a>    <span class="n">too_wide</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="L-513"><a href="#L-513"><span class="linenos">513</span></a>    <span class="n">terminal_width</span> <span class="o">=</span> <span class="n">os</span><span class="o">.</span><span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span>
+</span><span id="L-514"><a href="#L-514"><span class="linenos">514</span></a>    <span class="n">max_col_widths</span> <span class="o">=</span> <span class="n">terminal_width</span>
+</span><span id="L-515"><a href="#L-515"><span class="linenos">515</span></a>    <span class="c1"># Make an output with effectively unrestricted column widths</span>
+</span><span id="L-516"><a href="#L-516"><span class="linenos">516</span></a>    <span class="c1"># to see if shrinking is necessary</span>
+</span><span id="L-517"><a href="#L-517"><span class="linenos">517</span></a>    <span class="n">output</span> <span class="o">=</span> <span class="n">tabulate</span><span class="p">(</span>
+</span><span id="L-518"><a href="#L-518"><span class="linenos">518</span></a>        <span class="n">data</span><span class="p">,</span>
+</span><span id="L-519"><a href="#L-519"><span class="linenos">519</span></a>        <span class="n">headers</span><span class="o">=</span><span class="s2">&quot;keys&quot;</span><span class="p">,</span>
+</span><span id="L-520"><a href="#L-520"><span class="linenos">520</span></a>        <span class="n">disable_numparse</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
+</span><span id="L-521"><a href="#L-521"><span class="linenos">521</span></a>        <span class="n">tablefmt</span><span class="o">=</span><span class="s2">&quot;grid&quot;</span><span class="p">,</span>
+</span><span id="L-522"><a href="#L-522"><span class="linenos">522</span></a>        <span class="n">maxcolwidths</span><span class="o">=</span><span class="n">max_col_widths</span><span class="p">,</span>
+</span><span id="L-523"><a href="#L-523"><span class="linenos">523</span></a>    <span class="p">)</span>
+</span><span id="L-524"><a href="#L-524"><span class="linenos">524</span></a>    <span class="n">current_width</span> <span class="o">=</span> <span class="n">output</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-525"><a href="#L-525"><span class="linenos">525</span></a>    <span class="k">if</span> <span class="n">current_width</span> <span class="o">&lt;</span> <span class="n">terminal_width</span><span class="p">:</span>
+</span><span id="L-526"><a href="#L-526"><span class="linenos">526</span></a>        <span class="n">too_wide</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="L-527"><a href="#L-527"><span class="linenos">527</span></a>    <span class="k">if</span> <span class="n">wrap_to_terminal</span> <span class="ow">and</span> <span class="n">too_wide</span><span class="p">:</span>
+</span><span id="L-528"><a href="#L-528"><span class="linenos">528</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Resizing grid to fit within the terminal...&quot;</span><span class="p">)</span>
+</span><span id="L-529"><a href="#L-529"><span class="linenos">529</span></a>        <span class="n">previous_col_widths</span> <span class="o">=</span> <span class="n">max_col_widths</span>
+</span><span id="L-530"><a href="#L-530"><span class="linenos">530</span></a>        <span class="n">acceptable_width</span> <span class="o">=</span> <span class="n">terminal_width</span> <span class="o">-</span> <span class="mi">10</span>
+</span><span id="L-531"><a href="#L-531"><span class="linenos">531</span></a>        <span class="k">while</span> <span class="n">too_wide</span> <span class="ow">and</span> <span class="n">max_col_widths</span> <span class="o">&gt;</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="L-532"><a href="#L-532"><span class="linenos">532</span></a>            <span class="k">if</span> <span class="n">current_width</span> <span class="o">&gt;</span> <span class="n">terminal_width</span><span class="p">:</span>
+</span><span id="L-533"><a href="#L-533"><span class="linenos">533</span></a>                <span class="n">previous_col_widths</span> <span class="o">=</span> <span class="n">max_col_widths</span>
+</span><span id="L-534"><a href="#L-534"><span class="linenos">534</span></a>                <span class="n">max_col_widths</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="n">max_col_widths</span> <span class="o">*</span> <span class="mf">0.5</span><span class="p">)</span>
+</span><span id="L-535"><a href="#L-535"><span class="linenos">535</span></a>            <span class="k">elif</span> <span class="n">current_width</span> <span class="o">&lt;</span> <span class="n">terminal_width</span><span class="p">:</span>
+</span><span id="L-536"><a href="#L-536"><span class="linenos">536</span></a>                <span class="c1"># Without lowering acceptable_width, this condition will cause infinite loop</span>
+</span><span id="L-537"><a href="#L-537"><span class="linenos">537</span></a>                <span class="k">if</span> <span class="n">max_col_widths</span> <span class="o">==</span> <span class="n">previous_col_widths</span> <span class="o">-</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="L-538"><a href="#L-538"><span class="linenos">538</span></a>                    <span class="n">acceptable_width</span> <span class="o">-=</span> <span class="mi">10</span>
+</span><span id="L-539"><a href="#L-539"><span class="linenos">539</span></a>                <span class="n">max_col_widths</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span>
+</span><span id="L-540"><a href="#L-540"><span class="linenos">540</span></a>                    <span class="n">max_col_widths</span> <span class="o">+</span> <span class="p">(</span><span class="mf">0.5</span> <span class="o">*</span> <span class="p">(</span><span class="n">previous_col_widths</span> <span class="o">-</span> <span class="n">max_col_widths</span><span class="p">))</span>
+</span><span id="L-541"><a href="#L-541"><span class="linenos">541</span></a>                <span class="p">)</span>
+</span><span id="L-542"><a href="#L-542"><span class="linenos">542</span></a>            <span class="n">output</span> <span class="o">=</span> <span class="n">tabulate</span><span class="p">(</span>
+</span><span id="L-543"><a href="#L-543"><span class="linenos">543</span></a>                <span class="n">data</span><span class="p">,</span>
+</span><span id="L-544"><a href="#L-544"><span class="linenos">544</span></a>                <span class="n">headers</span><span class="o">=</span><span class="s2">&quot;keys&quot;</span><span class="p">,</span>
+</span><span id="L-545"><a href="#L-545"><span class="linenos">545</span></a>                <span class="n">disable_numparse</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
+</span><span id="L-546"><a href="#L-546"><span class="linenos">546</span></a>                <span class="n">tablefmt</span><span class="o">=</span><span class="s2">&quot;grid&quot;</span><span class="p">,</span>
+</span><span id="L-547"><a href="#L-547"><span class="linenos">547</span></a>                <span class="n">maxcolwidths</span><span class="o">=</span><span class="n">max_col_widths</span><span class="p">,</span>
+</span><span id="L-548"><a href="#L-548"><span class="linenos">548</span></a>            <span class="p">)</span>
+</span><span id="L-549"><a href="#L-549"><span class="linenos">549</span></a>            <span class="n">current_width</span> <span class="o">=</span> <span class="n">output</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-550"><a href="#L-550"><span class="linenos">550</span></a>            <span class="k">if</span> <span class="n">acceptable_width</span> <span class="o">&lt;</span> <span class="n">current_width</span> <span class="o">&lt;</span> <span class="n">terminal_width</span><span class="p">:</span>
+</span><span id="L-551"><a href="#L-551"><span class="linenos">551</span></a>                <span class="n">too_wide</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="L-552"><a href="#L-552"><span class="linenos">552</span></a>        <span class="k">if</span> <span class="n">too_wide</span><span class="p">:</span>
+</span><span id="L-553"><a href="#L-553"><span class="linenos">553</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Couldn&#39;t resize grid to fit within the terminal.&quot;</span><span class="p">)</span>
+</span><span id="L-554"><a href="#L-554"><span class="linenos">554</span></a>            <span class="k">return</span> <span class="nb">str</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
+</span><span id="L-555"><a href="#L-555"><span class="linenos">555</span></a>    <span class="k">return</span> <span class="n">output</span>
 </span></pre></div>
 
 
             </section>
                 <section id="DataBased">
                             <input id="DataBased-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr class">
@@ -700,480 +686,469 @@
 </span><span id="DataBased-29"><a href="#DataBased-29"><span class="linenos"> 29</span></a>
 </span><span id="DataBased-30"><a href="#DataBased-30"><span class="linenos"> 30</span></a><span class="sd">    Supports saving and reading dates as datetime objects.</span>
 </span><span id="DataBased-31"><a href="#DataBased-31"><span class="linenos"> 31</span></a>
 </span><span id="DataBased-32"><a href="#DataBased-32"><span class="linenos"> 32</span></a><span class="sd">    Supports using a context manager.&quot;&quot;&quot;</span>
 </span><span id="DataBased-33"><a href="#DataBased-33"><span class="linenos"> 33</span></a>
 </span><span id="DataBased-34"><a href="#DataBased-34"><span class="linenos"> 34</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
 </span><span id="DataBased-35"><a href="#DataBased-35"><span class="linenos"> 35</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="DataBased-36"><a href="#DataBased-36"><span class="linenos"> 36</span></a>        <span class="n">dbpath</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="n">Path</span><span class="p">,</span>
+</span><span id="DataBased-36"><a href="#DataBased-36"><span class="linenos"> 36</span></a>        <span class="n">dbpath</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="n">Pathier</span><span class="p">,</span>
 </span><span id="DataBased-37"><a href="#DataBased-37"><span class="linenos"> 37</span></a>        <span class="n">logger_encoding</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;utf-8&quot;</span><span class="p">,</span>
 </span><span id="DataBased-38"><a href="#DataBased-38"><span class="linenos"> 38</span></a>        <span class="n">logger_message_format</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="si">{levelname}</span><span class="s2">|-|</span><span class="si">{asctime}</span><span class="s2">|-|</span><span class="si">{message}</span><span class="s2">&quot;</span><span class="p">,</span>
 </span><span id="DataBased-39"><a href="#DataBased-39"><span class="linenos"> 39</span></a>    <span class="p">):</span>
 </span><span id="DataBased-40"><a href="#DataBased-40"><span class="linenos"> 40</span></a>        <span class="sd">&quot;&quot;&quot;</span>
 </span><span id="DataBased-41"><a href="#DataBased-41"><span class="linenos"> 41</span></a><span class="sd">        :param dbpath: String or Path object to database file.</span>
 </span><span id="DataBased-42"><a href="#DataBased-42"><span class="linenos"> 42</span></a><span class="sd">        If a relative path is given, it will be relative to the</span>
 </span><span id="DataBased-43"><a href="#DataBased-43"><span class="linenos"> 43</span></a><span class="sd">        current working directory. The log file will be saved to the</span>
 </span><span id="DataBased-44"><a href="#DataBased-44"><span class="linenos"> 44</span></a><span class="sd">        same directory.</span>
 </span><span id="DataBased-45"><a href="#DataBased-45"><span class="linenos"> 45</span></a>
 </span><span id="DataBased-46"><a href="#DataBased-46"><span class="linenos"> 46</span></a><span class="sd">        :param logger_message_format: &#39;{&#39; style format string</span>
 </span><span id="DataBased-47"><a href="#DataBased-47"><span class="linenos"> 47</span></a><span class="sd">        for the logger object.&quot;&quot;&quot;</span>
-</span><span id="DataBased-48"><a href="#DataBased-48"><span class="linenos"> 48</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Path</span><span class="p">(</span><span class="n">dbpath</span><span class="p">)</span>
-</span><span id="DataBased-49"><a href="#DataBased-49"><span class="linenos"> 49</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">dbname</span> <span class="o">=</span> <span class="n">Path</span><span class="p">(</span><span class="n">dbpath</span><span class="p">)</span><span class="o">.</span><span class="n">name</span>
+</span><span id="DataBased-48"><a href="#DataBased-48"><span class="linenos"> 48</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">dbpath</span><span class="p">)</span>
+</span><span id="DataBased-49"><a href="#DataBased-49"><span class="linenos"> 49</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">dbname</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">dbpath</span><span class="p">)</span><span class="o">.</span><span class="n">name</span>
 </span><span id="DataBased-50"><a href="#DataBased-50"><span class="linenos"> 50</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
 </span><span id="DataBased-51"><a href="#DataBased-51"><span class="linenos"> 51</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_logger_init</span><span class="p">(</span>
 </span><span id="DataBased-52"><a href="#DataBased-52"><span class="linenos"> 52</span></a>            <span class="n">encoding</span><span class="o">=</span><span class="n">logger_encoding</span><span class="p">,</span> <span class="n">message_format</span><span class="o">=</span><span class="n">logger_message_format</span>
 </span><span id="DataBased-53"><a href="#DataBased-53"><span class="linenos"> 53</span></a>        <span class="p">)</span>
 </span><span id="DataBased-54"><a href="#DataBased-54"><span class="linenos"> 54</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">connection_open</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="DataBased-55"><a href="#DataBased-55"><span class="linenos"> 55</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">create_manager</span><span class="p">()</span>
-</span><span id="DataBased-56"><a href="#DataBased-56"><span class="linenos"> 56</span></a>
-</span><span id="DataBased-57"><a href="#DataBased-57"><span class="linenos"> 57</span></a>    <span class="k">def</span> <span class="fm">__enter__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="DataBased-58"><a href="#DataBased-58"><span class="linenos"> 58</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">open</span><span class="p">()</span>
-</span><span id="DataBased-59"><a href="#DataBased-59"><span class="linenos"> 59</span></a>        <span class="k">return</span> <span class="bp">self</span>
-</span><span id="DataBased-60"><a href="#DataBased-60"><span class="linenos"> 60</span></a>
-</span><span id="DataBased-61"><a href="#DataBased-61"><span class="linenos"> 61</span></a>    <span class="k">def</span> <span class="fm">__exit__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">exception_type</span><span class="p">,</span> <span class="n">exception_value</span><span class="p">,</span> <span class="n">exception_traceback</span><span class="p">):</span>
-</span><span id="DataBased-62"><a href="#DataBased-62"><span class="linenos"> 62</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">close</span><span class="p">()</span>
-</span><span id="DataBased-63"><a href="#DataBased-63"><span class="linenos"> 63</span></a>
-</span><span id="DataBased-64"><a href="#DataBased-64"><span class="linenos"> 64</span></a>    <span class="k">def</span> <span class="nf">create_manager</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="DataBased-65"><a href="#DataBased-65"><span class="linenos"> 65</span></a>        <span class="sd">&quot;&quot;&quot;Create dbmanager.py in the same directory</span>
-</span><span id="DataBased-66"><a href="#DataBased-66"><span class="linenos"> 66</span></a><span class="sd">        as the database file if it doesn&#39;t exist.&quot;&quot;&quot;</span>
-</span><span id="DataBased-67"><a href="#DataBased-67"><span class="linenos"> 67</span></a>        <span class="n">manager_path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">parent</span> <span class="o">/</span> <span class="s2">&quot;dbmanager.py&quot;</span>
-</span><span id="DataBased-68"><a href="#DataBased-68"><span class="linenos"> 68</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">manager_path</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="DataBased-69"><a href="#DataBased-69"><span class="linenos"> 69</span></a>            <span class="n">manager_template</span> <span class="o">=</span> <span class="p">(</span><span class="n">Path</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span><span class="o">.</span><span class="n">parent</span> <span class="o">/</span> <span class="s2">&quot;dbmanager.py&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
-</span><span id="DataBased-70"><a href="#DataBased-70"><span class="linenos"> 70</span></a>            <span class="n">manager_path</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">manager_template</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;$dbname&quot;</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbname</span><span class="p">))</span>
-</span><span id="DataBased-71"><a href="#DataBased-71"><span class="linenos"> 71</span></a>
-</span><span id="DataBased-72"><a href="#DataBased-72"><span class="linenos"> 72</span></a>    <span class="k">def</span> <span class="nf">open</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="DataBased-73"><a href="#DataBased-73"><span class="linenos"> 73</span></a>        <span class="sd">&quot;&quot;&quot;Open connection to db.&quot;&quot;&quot;</span>
-</span><span id="DataBased-74"><a href="#DataBased-74"><span class="linenos"> 74</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">connection</span> <span class="o">=</span> <span class="n">sqlite3</span><span class="o">.</span><span class="n">connect</span><span class="p">(</span>
-</span><span id="DataBased-75"><a href="#DataBased-75"><span class="linenos"> 75</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">,</span>
-</span><span id="DataBased-76"><a href="#DataBased-76"><span class="linenos"> 76</span></a>            <span class="n">detect_types</span><span class="o">=</span><span class="n">sqlite3</span><span class="o">.</span><span class="n">PARSE_DECLTYPES</span> <span class="o">|</span> <span class="n">sqlite3</span><span class="o">.</span><span class="n">PARSE_COLNAMES</span><span class="p">,</span>
-</span><span id="DataBased-77"><a href="#DataBased-77"><span class="linenos"> 77</span></a>            <span class="n">timeout</span><span class="o">=</span><span class="mi">10</span><span class="p">,</span>
-</span><span id="DataBased-78"><a href="#DataBased-78"><span class="linenos"> 78</span></a>        <span class="p">)</span>
-</span><span id="DataBased-79"><a href="#DataBased-79"><span class="linenos"> 79</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">connection</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="s2">&quot;pragma foreign_keys = 1&quot;</span><span class="p">)</span>
-</span><span id="DataBased-80"><a href="#DataBased-80"><span class="linenos"> 80</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">connection</span><span class="o">.</span><span class="n">cursor</span><span class="p">()</span>
-</span><span id="DataBased-81"><a href="#DataBased-81"><span class="linenos"> 81</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">connection_open</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="DataBased-82"><a href="#DataBased-82"><span class="linenos"> 82</span></a>
-</span><span id="DataBased-83"><a href="#DataBased-83"><span class="linenos"> 83</span></a>    <span class="k">def</span> <span class="nf">close</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="DataBased-84"><a href="#DataBased-84"><span class="linenos"> 84</span></a>        <span class="sd">&quot;&quot;&quot;Save and close connection to db.</span>
-</span><span id="DataBased-85"><a href="#DataBased-85"><span class="linenos"> 85</span></a>
-</span><span id="DataBased-86"><a href="#DataBased-86"><span class="linenos"> 86</span></a><span class="sd">        Call this as soon as you are done using the database if you have</span>
-</span><span id="DataBased-87"><a href="#DataBased-87"><span class="linenos"> 87</span></a><span class="sd">        multiple threads or processes using the same database.&quot;&quot;&quot;</span>
-</span><span id="DataBased-88"><a href="#DataBased-88"><span class="linenos"> 88</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">connection_open</span><span class="p">:</span>
-</span><span id="DataBased-89"><a href="#DataBased-89"><span class="linenos"> 89</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">connection</span><span class="o">.</span><span class="n">commit</span><span class="p">()</span>
-</span><span id="DataBased-90"><a href="#DataBased-90"><span class="linenos"> 90</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">connection</span><span class="o">.</span><span class="n">close</span><span class="p">()</span>
-</span><span id="DataBased-91"><a href="#DataBased-91"><span class="linenos"> 91</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">connection_open</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="DataBased-92"><a href="#DataBased-92"><span class="linenos"> 92</span></a>
-</span><span id="DataBased-93"><a href="#DataBased-93"><span class="linenos"> 93</span></a>    <span class="k">def</span> <span class="nf">_logger_init</span><span class="p">(</span>
-</span><span id="DataBased-94"><a href="#DataBased-94"><span class="linenos"> 94</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="DataBased-95"><a href="#DataBased-95"><span class="linenos"> 95</span></a>        <span class="n">message_format</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="si">{levelname}</span><span class="s2">|-|</span><span class="si">{asctime}</span><span class="s2">|-|</span><span class="si">{message}</span><span class="s2">&quot;</span><span class="p">,</span>
-</span><span id="DataBased-96"><a href="#DataBased-96"><span class="linenos"> 96</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;utf-8&quot;</span><span class="p">,</span>
-</span><span id="DataBased-97"><a href="#DataBased-97"><span class="linenos"> 97</span></a>    <span class="p">):</span>
-</span><span id="DataBased-98"><a href="#DataBased-98"><span class="linenos"> 98</span></a>        <span class="sd">&quot;&quot;&quot;:param message_format: &#39;{&#39; style format string&quot;&quot;&quot;</span>
-</span><span id="DataBased-99"><a href="#DataBased-99"><span class="linenos"> 99</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">logger</span> <span class="o">=</span> <span class="n">logging</span><span class="o">.</span><span class="n">getLogger</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbname</span><span class="p">)</span>
-</span><span id="DataBased-100"><a href="#DataBased-100"><span class="linenos">100</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">hasHandlers</span><span class="p">():</span>
-</span><span id="DataBased-101"><a href="#DataBased-101"><span class="linenos">101</span></a>            <span class="n">handler</span> <span class="o">=</span> <span class="n">logging</span><span class="o">.</span><span class="n">FileHandler</span><span class="p">(</span>
-</span><span id="DataBased-102"><a href="#DataBased-102"><span class="linenos">102</span></a>                <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">,</span> <span class="s2">&quot;&quot;</span><span class="p">)</span> <span class="o">+</span> <span class="s2">&quot;.log&quot;</span><span class="p">,</span> <span class="n">encoding</span><span class="o">=</span><span class="n">encoding</span>
-</span><span id="DataBased-103"><a href="#DataBased-103"><span class="linenos">103</span></a>            <span class="p">)</span>
-</span><span id="DataBased-104"><a href="#DataBased-104"><span class="linenos">104</span></a>            <span class="n">handler</span><span class="o">.</span><span class="n">setFormatter</span><span class="p">(</span>
-</span><span id="DataBased-105"><a href="#DataBased-105"><span class="linenos">105</span></a>                <span class="n">logging</span><span class="o">.</span><span class="n">Formatter</span><span class="p">(</span>
-</span><span id="DataBased-106"><a href="#DataBased-106"><span class="linenos">106</span></a>                    <span class="n">message_format</span><span class="p">,</span> <span class="n">style</span><span class="o">=</span><span class="s2">&quot;{&quot;</span><span class="p">,</span> <span class="n">datefmt</span><span class="o">=</span><span class="s2">&quot;%m/</span><span class="si">%d</span><span class="s2">/%Y %I:%M:%S %p&quot;</span>
-</span><span id="DataBased-107"><a href="#DataBased-107"><span class="linenos">107</span></a>                <span class="p">)</span>
-</span><span id="DataBased-108"><a href="#DataBased-108"><span class="linenos">108</span></a>            <span class="p">)</span>
-</span><span id="DataBased-109"><a href="#DataBased-109"><span class="linenos">109</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">addHandler</span><span class="p">(</span><span class="n">handler</span><span class="p">)</span>
-</span><span id="DataBased-110"><a href="#DataBased-110"><span class="linenos">110</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">setLevel</span><span class="p">(</span><span class="n">logging</span><span class="o">.</span><span class="n">INFO</span><span class="p">)</span>
-</span><span id="DataBased-111"><a href="#DataBased-111"><span class="linenos">111</span></a>
-</span><span id="DataBased-112"><a href="#DataBased-112"><span class="linenos">112</span></a>    <span class="k">def</span> <span class="nf">_get_dict</span><span class="p">(</span>
-</span><span id="DataBased-113"><a href="#DataBased-113"><span class="linenos">113</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="nb">list</span><span class="p">,</span> <span class="n">columns_to_return</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="DataBased-114"><a href="#DataBased-114"><span class="linenos">114</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">dict</span><span class="p">:</span>
-</span><span id="DataBased-115"><a href="#DataBased-115"><span class="linenos">115</span></a>        <span class="sd">&quot;&quot;&quot;Converts the values of a row into a dictionary with column names as keys.</span>
-</span><span id="DataBased-116"><a href="#DataBased-116"><span class="linenos">116</span></a>
-</span><span id="DataBased-117"><a href="#DataBased-117"><span class="linenos">117</span></a><span class="sd">        :param table: The table that values were pulled from.</span>
-</span><span id="DataBased-118"><a href="#DataBased-118"><span class="linenos">118</span></a>
-</span><span id="DataBased-119"><a href="#DataBased-119"><span class="linenos">119</span></a><span class="sd">        :param values: List of values expected to be the same quantity</span>
-</span><span id="DataBased-120"><a href="#DataBased-120"><span class="linenos">120</span></a><span class="sd">        and in the same order as the column names of table.</span>
+</span><span id="DataBased-55"><a href="#DataBased-55"><span class="linenos"> 55</span></a>
+</span><span id="DataBased-56"><a href="#DataBased-56"><span class="linenos"> 56</span></a>    <span class="k">def</span> <span class="fm">__enter__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="DataBased-57"><a href="#DataBased-57"><span class="linenos"> 57</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">open</span><span class="p">()</span>
+</span><span id="DataBased-58"><a href="#DataBased-58"><span class="linenos"> 58</span></a>        <span class="k">return</span> <span class="bp">self</span>
+</span><span id="DataBased-59"><a href="#DataBased-59"><span class="linenos"> 59</span></a>
+</span><span id="DataBased-60"><a href="#DataBased-60"><span class="linenos"> 60</span></a>    <span class="k">def</span> <span class="fm">__exit__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">exception_type</span><span class="p">,</span> <span class="n">exception_value</span><span class="p">,</span> <span class="n">exception_traceback</span><span class="p">):</span>
+</span><span id="DataBased-61"><a href="#DataBased-61"><span class="linenos"> 61</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">close</span><span class="p">()</span>
+</span><span id="DataBased-62"><a href="#DataBased-62"><span class="linenos"> 62</span></a>
+</span><span id="DataBased-63"><a href="#DataBased-63"><span class="linenos"> 63</span></a>    <span class="k">def</span> <span class="nf">open</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="DataBased-64"><a href="#DataBased-64"><span class="linenos"> 64</span></a>        <span class="sd">&quot;&quot;&quot;Open connection to db.&quot;&quot;&quot;</span>
+</span><span id="DataBased-65"><a href="#DataBased-65"><span class="linenos"> 65</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">connection</span> <span class="o">=</span> <span class="n">sqlite3</span><span class="o">.</span><span class="n">connect</span><span class="p">(</span>
+</span><span id="DataBased-66"><a href="#DataBased-66"><span class="linenos"> 66</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">,</span>
+</span><span id="DataBased-67"><a href="#DataBased-67"><span class="linenos"> 67</span></a>            <span class="n">detect_types</span><span class="o">=</span><span class="n">sqlite3</span><span class="o">.</span><span class="n">PARSE_DECLTYPES</span> <span class="o">|</span> <span class="n">sqlite3</span><span class="o">.</span><span class="n">PARSE_COLNAMES</span><span class="p">,</span>
+</span><span id="DataBased-68"><a href="#DataBased-68"><span class="linenos"> 68</span></a>            <span class="n">timeout</span><span class="o">=</span><span class="mi">10</span><span class="p">,</span>
+</span><span id="DataBased-69"><a href="#DataBased-69"><span class="linenos"> 69</span></a>        <span class="p">)</span>
+</span><span id="DataBased-70"><a href="#DataBased-70"><span class="linenos"> 70</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">connection</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="s2">&quot;pragma foreign_keys = 1&quot;</span><span class="p">)</span>
+</span><span id="DataBased-71"><a href="#DataBased-71"><span class="linenos"> 71</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">connection</span><span class="o">.</span><span class="n">cursor</span><span class="p">()</span>
+</span><span id="DataBased-72"><a href="#DataBased-72"><span class="linenos"> 72</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">connection_open</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="DataBased-73"><a href="#DataBased-73"><span class="linenos"> 73</span></a>
+</span><span id="DataBased-74"><a href="#DataBased-74"><span class="linenos"> 74</span></a>    <span class="k">def</span> <span class="nf">close</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="DataBased-75"><a href="#DataBased-75"><span class="linenos"> 75</span></a>        <span class="sd">&quot;&quot;&quot;Save and close connection to db.</span>
+</span><span id="DataBased-76"><a href="#DataBased-76"><span class="linenos"> 76</span></a>
+</span><span id="DataBased-77"><a href="#DataBased-77"><span class="linenos"> 77</span></a><span class="sd">        Call this as soon as you are done using the database if you have</span>
+</span><span id="DataBased-78"><a href="#DataBased-78"><span class="linenos"> 78</span></a><span class="sd">        multiple threads or processes using the same database.&quot;&quot;&quot;</span>
+</span><span id="DataBased-79"><a href="#DataBased-79"><span class="linenos"> 79</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">connection_open</span><span class="p">:</span>
+</span><span id="DataBased-80"><a href="#DataBased-80"><span class="linenos"> 80</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">connection</span><span class="o">.</span><span class="n">commit</span><span class="p">()</span>
+</span><span id="DataBased-81"><a href="#DataBased-81"><span class="linenos"> 81</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">connection</span><span class="o">.</span><span class="n">close</span><span class="p">()</span>
+</span><span id="DataBased-82"><a href="#DataBased-82"><span class="linenos"> 82</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">connection_open</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="DataBased-83"><a href="#DataBased-83"><span class="linenos"> 83</span></a>
+</span><span id="DataBased-84"><a href="#DataBased-84"><span class="linenos"> 84</span></a>    <span class="k">def</span> <span class="nf">_logger_init</span><span class="p">(</span>
+</span><span id="DataBased-85"><a href="#DataBased-85"><span class="linenos"> 85</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="DataBased-86"><a href="#DataBased-86"><span class="linenos"> 86</span></a>        <span class="n">message_format</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="si">{levelname}</span><span class="s2">|-|</span><span class="si">{asctime}</span><span class="s2">|-|</span><span class="si">{message}</span><span class="s2">&quot;</span><span class="p">,</span>
+</span><span id="DataBased-87"><a href="#DataBased-87"><span class="linenos"> 87</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;utf-8&quot;</span><span class="p">,</span>
+</span><span id="DataBased-88"><a href="#DataBased-88"><span class="linenos"> 88</span></a>    <span class="p">):</span>
+</span><span id="DataBased-89"><a href="#DataBased-89"><span class="linenos"> 89</span></a>        <span class="sd">&quot;&quot;&quot;:param message_format: &#39;{&#39; style format string&quot;&quot;&quot;</span>
+</span><span id="DataBased-90"><a href="#DataBased-90"><span class="linenos"> 90</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">logger</span> <span class="o">=</span> <span class="n">logging</span><span class="o">.</span><span class="n">getLogger</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbname</span><span class="p">)</span>
+</span><span id="DataBased-91"><a href="#DataBased-91"><span class="linenos"> 91</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">hasHandlers</span><span class="p">():</span>
+</span><span id="DataBased-92"><a href="#DataBased-92"><span class="linenos"> 92</span></a>            <span class="n">handler</span> <span class="o">=</span> <span class="n">logging</span><span class="o">.</span><span class="n">FileHandler</span><span class="p">(</span>
+</span><span id="DataBased-93"><a href="#DataBased-93"><span class="linenos"> 93</span></a>                <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">,</span> <span class="s2">&quot;&quot;</span><span class="p">)</span> <span class="o">+</span> <span class="s2">&quot;.log&quot;</span><span class="p">,</span> <span class="n">encoding</span><span class="o">=</span><span class="n">encoding</span>
+</span><span id="DataBased-94"><a href="#DataBased-94"><span class="linenos"> 94</span></a>            <span class="p">)</span>
+</span><span id="DataBased-95"><a href="#DataBased-95"><span class="linenos"> 95</span></a>            <span class="n">handler</span><span class="o">.</span><span class="n">setFormatter</span><span class="p">(</span>
+</span><span id="DataBased-96"><a href="#DataBased-96"><span class="linenos"> 96</span></a>                <span class="n">logging</span><span class="o">.</span><span class="n">Formatter</span><span class="p">(</span>
+</span><span id="DataBased-97"><a href="#DataBased-97"><span class="linenos"> 97</span></a>                    <span class="n">message_format</span><span class="p">,</span> <span class="n">style</span><span class="o">=</span><span class="s2">&quot;{&quot;</span><span class="p">,</span> <span class="n">datefmt</span><span class="o">=</span><span class="s2">&quot;%m/</span><span class="si">%d</span><span class="s2">/%Y %I:%M:%S %p&quot;</span>
+</span><span id="DataBased-98"><a href="#DataBased-98"><span class="linenos"> 98</span></a>                <span class="p">)</span>
+</span><span id="DataBased-99"><a href="#DataBased-99"><span class="linenos"> 99</span></a>            <span class="p">)</span>
+</span><span id="DataBased-100"><a href="#DataBased-100"><span class="linenos">100</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">addHandler</span><span class="p">(</span><span class="n">handler</span><span class="p">)</span>
+</span><span id="DataBased-101"><a href="#DataBased-101"><span class="linenos">101</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">setLevel</span><span class="p">(</span><span class="n">logging</span><span class="o">.</span><span class="n">INFO</span><span class="p">)</span>
+</span><span id="DataBased-102"><a href="#DataBased-102"><span class="linenos">102</span></a>
+</span><span id="DataBased-103"><a href="#DataBased-103"><span class="linenos">103</span></a>    <span class="k">def</span> <span class="nf">_get_dict</span><span class="p">(</span>
+</span><span id="DataBased-104"><a href="#DataBased-104"><span class="linenos">104</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="nb">list</span><span class="p">,</span> <span class="n">columns_to_return</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="DataBased-105"><a href="#DataBased-105"><span class="linenos">105</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">dict</span><span class="p">:</span>
+</span><span id="DataBased-106"><a href="#DataBased-106"><span class="linenos">106</span></a>        <span class="sd">&quot;&quot;&quot;Converts the values of a row into a dictionary with column names as keys.</span>
+</span><span id="DataBased-107"><a href="#DataBased-107"><span class="linenos">107</span></a>
+</span><span id="DataBased-108"><a href="#DataBased-108"><span class="linenos">108</span></a><span class="sd">        :param table: The table that values were pulled from.</span>
+</span><span id="DataBased-109"><a href="#DataBased-109"><span class="linenos">109</span></a>
+</span><span id="DataBased-110"><a href="#DataBased-110"><span class="linenos">110</span></a><span class="sd">        :param values: List of values expected to be the same quantity</span>
+</span><span id="DataBased-111"><a href="#DataBased-111"><span class="linenos">111</span></a><span class="sd">        and in the same order as the column names of table.</span>
+</span><span id="DataBased-112"><a href="#DataBased-112"><span class="linenos">112</span></a>
+</span><span id="DataBased-113"><a href="#DataBased-113"><span class="linenos">113</span></a><span class="sd">        :param columns_to_return: An optional list of column names.</span>
+</span><span id="DataBased-114"><a href="#DataBased-114"><span class="linenos">114</span></a><span class="sd">        If given, only these columns will be included in the returned dictionary.</span>
+</span><span id="DataBased-115"><a href="#DataBased-115"><span class="linenos">115</span></a><span class="sd">        Otherwise all columns and values are returned.&quot;&quot;&quot;</span>
+</span><span id="DataBased-116"><a href="#DataBased-116"><span class="linenos">116</span></a>        <span class="k">return</span> <span class="p">{</span>
+</span><span id="DataBased-117"><a href="#DataBased-117"><span class="linenos">117</span></a>            <span class="n">column</span><span class="p">:</span> <span class="n">value</span>
+</span><span id="DataBased-118"><a href="#DataBased-118"><span class="linenos">118</span></a>            <span class="k">for</span> <span class="n">column</span><span class="p">,</span> <span class="n">value</span> <span class="ow">in</span> <span class="nb">zip</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">get_column_names</span><span class="p">(</span><span class="n">table</span><span class="p">),</span> <span class="n">values</span><span class="p">)</span>
+</span><span id="DataBased-119"><a href="#DataBased-119"><span class="linenos">119</span></a>            <span class="k">if</span> <span class="ow">not</span> <span class="n">columns_to_return</span> <span class="ow">or</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns_to_return</span>
+</span><span id="DataBased-120"><a href="#DataBased-120"><span class="linenos">120</span></a>        <span class="p">}</span>
 </span><span id="DataBased-121"><a href="#DataBased-121"><span class="linenos">121</span></a>
-</span><span id="DataBased-122"><a href="#DataBased-122"><span class="linenos">122</span></a><span class="sd">        :param columns_to_return: An optional list of column names.</span>
-</span><span id="DataBased-123"><a href="#DataBased-123"><span class="linenos">123</span></a><span class="sd">        If given, only these columns will be included in the returned dictionary.</span>
-</span><span id="DataBased-124"><a href="#DataBased-124"><span class="linenos">124</span></a><span class="sd">        Otherwise all columns and values are returned.&quot;&quot;&quot;</span>
-</span><span id="DataBased-125"><a href="#DataBased-125"><span class="linenos">125</span></a>        <span class="k">return</span> <span class="p">{</span>
-</span><span id="DataBased-126"><a href="#DataBased-126"><span class="linenos">126</span></a>            <span class="n">column</span><span class="p">:</span> <span class="n">value</span>
-</span><span id="DataBased-127"><a href="#DataBased-127"><span class="linenos">127</span></a>            <span class="k">for</span> <span class="n">column</span><span class="p">,</span> <span class="n">value</span> <span class="ow">in</span> <span class="nb">zip</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">get_column_names</span><span class="p">(</span><span class="n">table</span><span class="p">),</span> <span class="n">values</span><span class="p">)</span>
-</span><span id="DataBased-128"><a href="#DataBased-128"><span class="linenos">128</span></a>            <span class="k">if</span> <span class="ow">not</span> <span class="n">columns_to_return</span> <span class="ow">or</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns_to_return</span>
-</span><span id="DataBased-129"><a href="#DataBased-129"><span class="linenos">129</span></a>        <span class="p">}</span>
+</span><span id="DataBased-122"><a href="#DataBased-122"><span class="linenos">122</span></a>    <span class="k">def</span> <span class="nf">_get_conditions</span><span class="p">(</span>
+</span><span id="DataBased-123"><a href="#DataBased-123"><span class="linenos">123</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="DataBased-124"><a href="#DataBased-124"><span class="linenos">124</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="DataBased-125"><a href="#DataBased-125"><span class="linenos">125</span></a>        <span class="sd">&quot;&quot;&quot;Builds and returns the conditional portion of a query.</span>
+</span><span id="DataBased-126"><a href="#DataBased-126"><span class="linenos">126</span></a>
+</span><span id="DataBased-127"><a href="#DataBased-127"><span class="linenos">127</span></a><span class="sd">        :param match_criteria: Can be a list of 2-tuples where each</span>
+</span><span id="DataBased-128"><a href="#DataBased-128"><span class="linenos">128</span></a><span class="sd">        tuple is (columnName, rowValue) or a dictionary where</span>
+</span><span id="DataBased-129"><a href="#DataBased-129"><span class="linenos">129</span></a><span class="sd">        keys are column names and values are row values.</span>
 </span><span id="DataBased-130"><a href="#DataBased-130"><span class="linenos">130</span></a>
-</span><span id="DataBased-131"><a href="#DataBased-131"><span class="linenos">131</span></a>    <span class="k">def</span> <span class="nf">_get_conditions</span><span class="p">(</span>
-</span><span id="DataBased-132"><a href="#DataBased-132"><span class="linenos">132</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="DataBased-133"><a href="#DataBased-133"><span class="linenos">133</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="DataBased-134"><a href="#DataBased-134"><span class="linenos">134</span></a>        <span class="sd">&quot;&quot;&quot;Builds and returns the conditional portion of a query.</span>
+</span><span id="DataBased-131"><a href="#DataBased-131"><span class="linenos">131</span></a><span class="sd">        :param exact_match: If False, the rowValue for a give column</span>
+</span><span id="DataBased-132"><a href="#DataBased-132"><span class="linenos">132</span></a><span class="sd">        will be matched as a substring.</span>
+</span><span id="DataBased-133"><a href="#DataBased-133"><span class="linenos">133</span></a>
+</span><span id="DataBased-134"><a href="#DataBased-134"><span class="linenos">134</span></a><span class="sd">        Usage e.g.:</span>
 </span><span id="DataBased-135"><a href="#DataBased-135"><span class="linenos">135</span></a>
-</span><span id="DataBased-136"><a href="#DataBased-136"><span class="linenos">136</span></a><span class="sd">        :param match_criteria: Can be a list of 2-tuples where each</span>
-</span><span id="DataBased-137"><a href="#DataBased-137"><span class="linenos">137</span></a><span class="sd">        tuple is (columnName, rowValue) or a dictionary where</span>
-</span><span id="DataBased-138"><a href="#DataBased-138"><span class="linenos">138</span></a><span class="sd">        keys are column names and values are row values.</span>
-</span><span id="DataBased-139"><a href="#DataBased-139"><span class="linenos">139</span></a>
-</span><span id="DataBased-140"><a href="#DataBased-140"><span class="linenos">140</span></a><span class="sd">        :param exact_match: If False, the rowValue for a give column</span>
-</span><span id="DataBased-141"><a href="#DataBased-141"><span class="linenos">141</span></a><span class="sd">        will be matched as a substring.</span>
-</span><span id="DataBased-142"><a href="#DataBased-142"><span class="linenos">142</span></a>
-</span><span id="DataBased-143"><a href="#DataBased-143"><span class="linenos">143</span></a><span class="sd">        Usage e.g.:</span>
-</span><span id="DataBased-144"><a href="#DataBased-144"><span class="linenos">144</span></a>
-</span><span id="DataBased-145"><a href="#DataBased-145"><span class="linenos">145</span></a><span class="sd">        self.cursor.execute(f&#39;select * from {table} where {conditions}&#39;)&quot;&quot;&quot;</span>
-</span><span id="DataBased-146"><a href="#DataBased-146"><span class="linenos">146</span></a>        <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">)</span> <span class="o">==</span> <span class="nb">dict</span><span class="p">:</span>
-</span><span id="DataBased-147"><a href="#DataBased-147"><span class="linenos">147</span></a>            <span class="n">match_criteria</span> <span class="o">=</span> <span class="p">[(</span><span class="n">k</span><span class="p">,</span> <span class="n">v</span><span class="p">)</span> <span class="k">for</span> <span class="n">k</span><span class="p">,</span> <span class="n">v</span> <span class="ow">in</span> <span class="n">match_criteria</span><span class="o">.</span><span class="n">items</span><span class="p">()]</span>
-</span><span id="DataBased-148"><a href="#DataBased-148"><span class="linenos">148</span></a>        <span class="k">if</span> <span class="n">exact_match</span><span class="p">:</span>
-</span><span id="DataBased-149"><a href="#DataBased-149"><span class="linenos">149</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="s2">&quot; and &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
-</span><span id="DataBased-150"><a href="#DataBased-150"><span class="linenos">150</span></a>                <span class="sa">f</span><span class="s1">&#39;&quot;</span><span class="si">{</span><span class="n">column_row</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s1">&quot; = &quot;</span><span class="si">{</span><span class="n">column_row</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s1">&quot;&#39;</span>
-</span><span id="DataBased-151"><a href="#DataBased-151"><span class="linenos">151</span></a>                <span class="k">for</span> <span class="n">column_row</span> <span class="ow">in</span> <span class="n">match_criteria</span>
-</span><span id="DataBased-152"><a href="#DataBased-152"><span class="linenos">152</span></a>            <span class="p">)</span>
-</span><span id="DataBased-153"><a href="#DataBased-153"><span class="linenos">153</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="DataBased-154"><a href="#DataBased-154"><span class="linenos">154</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="s2">&quot; and &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
-</span><span id="DataBased-155"><a href="#DataBased-155"><span class="linenos">155</span></a>                <span class="sa">f</span><span class="s1">&#39;&quot;</span><span class="si">{</span><span class="n">column_row</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s1">&quot; like &quot;%</span><span class="si">{</span><span class="n">column_row</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s1">%&quot;&#39;</span>
-</span><span id="DataBased-156"><a href="#DataBased-156"><span class="linenos">156</span></a>                <span class="k">for</span> <span class="n">column_row</span> <span class="ow">in</span> <span class="n">match_criteria</span>
-</span><span id="DataBased-157"><a href="#DataBased-157"><span class="linenos">157</span></a>            <span class="p">)</span>
-</span><span id="DataBased-158"><a href="#DataBased-158"><span class="linenos">158</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;(</span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">)&quot;</span>
-</span><span id="DataBased-159"><a href="#DataBased-159"><span class="linenos">159</span></a>
-</span><span id="DataBased-160"><a href="#DataBased-160"><span class="linenos">160</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased-161"><a href="#DataBased-161"><span class="linenos">161</span></a>    <span class="k">def</span> <span class="nf">query</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">query_</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]:</span>
-</span><span id="DataBased-162"><a href="#DataBased-162"><span class="linenos">162</span></a>        <span class="sd">&quot;&quot;&quot;Execute an arbitrary query and</span>
-</span><span id="DataBased-163"><a href="#DataBased-163"><span class="linenos">163</span></a><span class="sd">        return the results.&quot;&quot;&quot;</span>
-</span><span id="DataBased-164"><a href="#DataBased-164"><span class="linenos">164</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query_</span><span class="p">)</span>
-</span><span id="DataBased-165"><a href="#DataBased-165"><span class="linenos">165</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()</span>
-</span><span id="DataBased-166"><a href="#DataBased-166"><span class="linenos">166</span></a>
-</span><span id="DataBased-167"><a href="#DataBased-167"><span class="linenos">167</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased-168"><a href="#DataBased-168"><span class="linenos">168</span></a>    <span class="k">def</span> <span class="nf">create_tables</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table_querys</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="p">[]):</span>
-</span><span id="DataBased-169"><a href="#DataBased-169"><span class="linenos">169</span></a>        <span class="sd">&quot;&quot;&quot;Create tables if they don&#39;t exist.</span>
+</span><span id="DataBased-136"><a href="#DataBased-136"><span class="linenos">136</span></a><span class="sd">        self.cursor.execute(f&#39;select * from {table} where {conditions}&#39;)&quot;&quot;&quot;</span>
+</span><span id="DataBased-137"><a href="#DataBased-137"><span class="linenos">137</span></a>        <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">)</span> <span class="o">==</span> <span class="nb">dict</span><span class="p">:</span>
+</span><span id="DataBased-138"><a href="#DataBased-138"><span class="linenos">138</span></a>            <span class="n">match_criteria</span> <span class="o">=</span> <span class="p">[(</span><span class="n">k</span><span class="p">,</span> <span class="n">v</span><span class="p">)</span> <span class="k">for</span> <span class="n">k</span><span class="p">,</span> <span class="n">v</span> <span class="ow">in</span> <span class="n">match_criteria</span><span class="o">.</span><span class="n">items</span><span class="p">()]</span>
+</span><span id="DataBased-139"><a href="#DataBased-139"><span class="linenos">139</span></a>        <span class="k">if</span> <span class="n">exact_match</span><span class="p">:</span>
+</span><span id="DataBased-140"><a href="#DataBased-140"><span class="linenos">140</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="s2">&quot; and &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
+</span><span id="DataBased-141"><a href="#DataBased-141"><span class="linenos">141</span></a>                <span class="sa">f</span><span class="s1">&#39;&quot;</span><span class="si">{</span><span class="n">column_row</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s1">&quot; = &quot;</span><span class="si">{</span><span class="n">column_row</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s1">&quot;&#39;</span>
+</span><span id="DataBased-142"><a href="#DataBased-142"><span class="linenos">142</span></a>                <span class="k">for</span> <span class="n">column_row</span> <span class="ow">in</span> <span class="n">match_criteria</span>
+</span><span id="DataBased-143"><a href="#DataBased-143"><span class="linenos">143</span></a>            <span class="p">)</span>
+</span><span id="DataBased-144"><a href="#DataBased-144"><span class="linenos">144</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="DataBased-145"><a href="#DataBased-145"><span class="linenos">145</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="s2">&quot; and &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
+</span><span id="DataBased-146"><a href="#DataBased-146"><span class="linenos">146</span></a>                <span class="sa">f</span><span class="s1">&#39;&quot;</span><span class="si">{</span><span class="n">column_row</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s1">&quot; like &quot;%</span><span class="si">{</span><span class="n">column_row</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s1">%&quot;&#39;</span>
+</span><span id="DataBased-147"><a href="#DataBased-147"><span class="linenos">147</span></a>                <span class="k">for</span> <span class="n">column_row</span> <span class="ow">in</span> <span class="n">match_criteria</span>
+</span><span id="DataBased-148"><a href="#DataBased-148"><span class="linenos">148</span></a>            <span class="p">)</span>
+</span><span id="DataBased-149"><a href="#DataBased-149"><span class="linenos">149</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;(</span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">)&quot;</span>
+</span><span id="DataBased-150"><a href="#DataBased-150"><span class="linenos">150</span></a>
+</span><span id="DataBased-151"><a href="#DataBased-151"><span class="linenos">151</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased-152"><a href="#DataBased-152"><span class="linenos">152</span></a>    <span class="k">def</span> <span class="nf">query</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">query_</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]:</span>
+</span><span id="DataBased-153"><a href="#DataBased-153"><span class="linenos">153</span></a>        <span class="sd">&quot;&quot;&quot;Execute an arbitrary query and</span>
+</span><span id="DataBased-154"><a href="#DataBased-154"><span class="linenos">154</span></a><span class="sd">        return the results.&quot;&quot;&quot;</span>
+</span><span id="DataBased-155"><a href="#DataBased-155"><span class="linenos">155</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query_</span><span class="p">)</span>
+</span><span id="DataBased-156"><a href="#DataBased-156"><span class="linenos">156</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()</span>
+</span><span id="DataBased-157"><a href="#DataBased-157"><span class="linenos">157</span></a>
+</span><span id="DataBased-158"><a href="#DataBased-158"><span class="linenos">158</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased-159"><a href="#DataBased-159"><span class="linenos">159</span></a>    <span class="k">def</span> <span class="nf">create_tables</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table_querys</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="p">[]):</span>
+</span><span id="DataBased-160"><a href="#DataBased-160"><span class="linenos">160</span></a>        <span class="sd">&quot;&quot;&quot;Create tables if they don&#39;t exist.</span>
+</span><span id="DataBased-161"><a href="#DataBased-161"><span class="linenos">161</span></a>
+</span><span id="DataBased-162"><a href="#DataBased-162"><span class="linenos">162</span></a><span class="sd">        :param table_querys: Each query should be</span>
+</span><span id="DataBased-163"><a href="#DataBased-163"><span class="linenos">163</span></a><span class="sd">        in the form &#39;tableName(columnDefinitions)&#39;&quot;&quot;&quot;</span>
+</span><span id="DataBased-164"><a href="#DataBased-164"><span class="linenos">164</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">table_querys</span><span class="p">)</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="DataBased-165"><a href="#DataBased-165"><span class="linenos">165</span></a>            <span class="n">table_names</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
+</span><span id="DataBased-166"><a href="#DataBased-166"><span class="linenos">166</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">table_querys</span><span class="p">:</span>
+</span><span id="DataBased-167"><a href="#DataBased-167"><span class="linenos">167</span></a>                <span class="k">if</span> <span class="n">table</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;(&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">table_names</span><span class="p">:</span>
+</span><span id="DataBased-168"><a href="#DataBased-168"><span class="linenos">168</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;create table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DataBased-169"><a href="#DataBased-169"><span class="linenos">169</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;</span><span class="si">{</span><span class="n">table</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;(&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s1"> table created.&#39;</span><span class="p">)</span>
 </span><span id="DataBased-170"><a href="#DataBased-170"><span class="linenos">170</span></a>
-</span><span id="DataBased-171"><a href="#DataBased-171"><span class="linenos">171</span></a><span class="sd">        :param table_querys: Each query should be</span>
-</span><span id="DataBased-172"><a href="#DataBased-172"><span class="linenos">172</span></a><span class="sd">        in the form &#39;tableName(columnDefinitions)&#39;&quot;&quot;&quot;</span>
-</span><span id="DataBased-173"><a href="#DataBased-173"><span class="linenos">173</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">table_querys</span><span class="p">)</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="DataBased-174"><a href="#DataBased-174"><span class="linenos">174</span></a>            <span class="n">table_names</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
-</span><span id="DataBased-175"><a href="#DataBased-175"><span class="linenos">175</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">table_querys</span><span class="p">:</span>
-</span><span id="DataBased-176"><a href="#DataBased-176"><span class="linenos">176</span></a>                <span class="k">if</span> <span class="n">table</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;(&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">table_names</span><span class="p">:</span>
-</span><span id="DataBased-177"><a href="#DataBased-177"><span class="linenos">177</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;create table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DataBased-178"><a href="#DataBased-178"><span class="linenos">178</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;</span><span class="si">{</span><span class="n">table</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;(&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s1"> table created.&#39;</span><span class="p">)</span>
-</span><span id="DataBased-179"><a href="#DataBased-179"><span class="linenos">179</span></a>
-</span><span id="DataBased-180"><a href="#DataBased-180"><span class="linenos">180</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased-181"><a href="#DataBased-181"><span class="linenos">181</span></a>    <span class="k">def</span> <span class="nf">create_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">column_defs</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]):</span>
-</span><span id="DataBased-182"><a href="#DataBased-182"><span class="linenos">182</span></a>        <span class="sd">&quot;&quot;&quot;Create a table if it doesn&#39;t exist.</span>
-</span><span id="DataBased-183"><a href="#DataBased-183"><span class="linenos">183</span></a>
-</span><span id="DataBased-184"><a href="#DataBased-184"><span class="linenos">184</span></a><span class="sd">        :param table: Name of the table to create.</span>
-</span><span id="DataBased-185"><a href="#DataBased-185"><span class="linenos">185</span></a>
-</span><span id="DataBased-186"><a href="#DataBased-186"><span class="linenos">186</span></a><span class="sd">        :param column_defs: List of column definitions in</span>
-</span><span id="DataBased-187"><a href="#DataBased-187"><span class="linenos">187</span></a><span class="sd">        proper Sqlite3 sytax.</span>
-</span><span id="DataBased-188"><a href="#DataBased-188"><span class="linenos">188</span></a><span class="sd">        i.e. &quot;columnName text unique&quot; or &quot;columnName int primary key&quot; etc.&quot;&quot;&quot;</span>
-</span><span id="DataBased-189"><a href="#DataBased-189"><span class="linenos">189</span></a>        <span class="k">if</span> <span class="n">table</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">():</span>
-</span><span id="DataBased-190"><a href="#DataBased-190"><span class="linenos">190</span></a>            <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;create table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">(</span><span class="si">{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">column_defs</span><span class="p">)</span><span class="si">}</span><span class="s2">)&quot;</span>
-</span><span id="DataBased-191"><a href="#DataBased-191"><span class="linenos">191</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
-</span><span id="DataBased-192"><a href="#DataBased-192"><span class="linenos">192</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;&#39;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&#39; table created.&quot;</span><span class="p">)</span>
-</span><span id="DataBased-193"><a href="#DataBased-193"><span class="linenos">193</span></a>
-</span><span id="DataBased-194"><a href="#DataBased-194"><span class="linenos">194</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased-195"><a href="#DataBased-195"><span class="linenos">195</span></a>    <span class="k">def</span> <span class="nf">get_table_names</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
-</span><span id="DataBased-196"><a href="#DataBased-196"><span class="linenos">196</span></a>        <span class="sd">&quot;&quot;&quot;Returns a list of table names from database.&quot;&quot;&quot;</span>
-</span><span id="DataBased-197"><a href="#DataBased-197"><span class="linenos">197</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="DataBased-198"><a href="#DataBased-198"><span class="linenos">198</span></a>            <span class="s1">&#39;select name from sqlite_Schema where type = &quot;table&quot; and name not like &quot;sqlite_%&quot;&#39;</span>
-</span><span id="DataBased-199"><a href="#DataBased-199"><span class="linenos">199</span></a>        <span class="p">)</span>
-</span><span id="DataBased-200"><a href="#DataBased-200"><span class="linenos">200</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">result</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()]</span>
-</span><span id="DataBased-201"><a href="#DataBased-201"><span class="linenos">201</span></a>
-</span><span id="DataBased-202"><a href="#DataBased-202"><span class="linenos">202</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased-203"><a href="#DataBased-203"><span class="linenos">203</span></a>    <span class="k">def</span> <span class="nf">get_column_names</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
-</span><span id="DataBased-204"><a href="#DataBased-204"><span class="linenos">204</span></a>        <span class="sd">&quot;&quot;&quot;Return a list of column names from a table.&quot;&quot;&quot;</span>
-</span><span id="DataBased-205"><a href="#DataBased-205"><span class="linenos">205</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;select * from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> where 1=0&quot;</span><span class="p">)</span>
-</span><span id="DataBased-206"><a href="#DataBased-206"><span class="linenos">206</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">description</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="k">for</span> <span class="n">description</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">description</span><span class="p">]</span>
+</span><span id="DataBased-171"><a href="#DataBased-171"><span class="linenos">171</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased-172"><a href="#DataBased-172"><span class="linenos">172</span></a>    <span class="k">def</span> <span class="nf">create_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">column_defs</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]):</span>
+</span><span id="DataBased-173"><a href="#DataBased-173"><span class="linenos">173</span></a>        <span class="sd">&quot;&quot;&quot;Create a table if it doesn&#39;t exist.</span>
+</span><span id="DataBased-174"><a href="#DataBased-174"><span class="linenos">174</span></a>
+</span><span id="DataBased-175"><a href="#DataBased-175"><span class="linenos">175</span></a><span class="sd">        :param table: Name of the table to create.</span>
+</span><span id="DataBased-176"><a href="#DataBased-176"><span class="linenos">176</span></a>
+</span><span id="DataBased-177"><a href="#DataBased-177"><span class="linenos">177</span></a><span class="sd">        :param column_defs: List of column definitions in</span>
+</span><span id="DataBased-178"><a href="#DataBased-178"><span class="linenos">178</span></a><span class="sd">        proper Sqlite3 sytax.</span>
+</span><span id="DataBased-179"><a href="#DataBased-179"><span class="linenos">179</span></a><span class="sd">        i.e. &quot;columnName text unique&quot; or &quot;columnName int primary key&quot; etc.&quot;&quot;&quot;</span>
+</span><span id="DataBased-180"><a href="#DataBased-180"><span class="linenos">180</span></a>        <span class="k">if</span> <span class="n">table</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">():</span>
+</span><span id="DataBased-181"><a href="#DataBased-181"><span class="linenos">181</span></a>            <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;create table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">(</span><span class="si">{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">column_defs</span><span class="p">)</span><span class="si">}</span><span class="s2">)&quot;</span>
+</span><span id="DataBased-182"><a href="#DataBased-182"><span class="linenos">182</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
+</span><span id="DataBased-183"><a href="#DataBased-183"><span class="linenos">183</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;&#39;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&#39; table created.&quot;</span><span class="p">)</span>
+</span><span id="DataBased-184"><a href="#DataBased-184"><span class="linenos">184</span></a>
+</span><span id="DataBased-185"><a href="#DataBased-185"><span class="linenos">185</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased-186"><a href="#DataBased-186"><span class="linenos">186</span></a>    <span class="k">def</span> <span class="nf">get_table_names</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
+</span><span id="DataBased-187"><a href="#DataBased-187"><span class="linenos">187</span></a>        <span class="sd">&quot;&quot;&quot;Returns a list of table names from database.&quot;&quot;&quot;</span>
+</span><span id="DataBased-188"><a href="#DataBased-188"><span class="linenos">188</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="DataBased-189"><a href="#DataBased-189"><span class="linenos">189</span></a>            <span class="s1">&#39;select name from sqlite_Schema where type = &quot;table&quot; and name not like &quot;sqlite_%&quot;&#39;</span>
+</span><span id="DataBased-190"><a href="#DataBased-190"><span class="linenos">190</span></a>        <span class="p">)</span>
+</span><span id="DataBased-191"><a href="#DataBased-191"><span class="linenos">191</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">result</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()]</span>
+</span><span id="DataBased-192"><a href="#DataBased-192"><span class="linenos">192</span></a>
+</span><span id="DataBased-193"><a href="#DataBased-193"><span class="linenos">193</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased-194"><a href="#DataBased-194"><span class="linenos">194</span></a>    <span class="k">def</span> <span class="nf">get_column_names</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
+</span><span id="DataBased-195"><a href="#DataBased-195"><span class="linenos">195</span></a>        <span class="sd">&quot;&quot;&quot;Return a list of column names from a table.&quot;&quot;&quot;</span>
+</span><span id="DataBased-196"><a href="#DataBased-196"><span class="linenos">196</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;select * from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> where 1=0&quot;</span><span class="p">)</span>
+</span><span id="DataBased-197"><a href="#DataBased-197"><span class="linenos">197</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">description</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="k">for</span> <span class="n">description</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">description</span><span class="p">]</span>
+</span><span id="DataBased-198"><a href="#DataBased-198"><span class="linenos">198</span></a>
+</span><span id="DataBased-199"><a href="#DataBased-199"><span class="linenos">199</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased-200"><a href="#DataBased-200"><span class="linenos">200</span></a>    <span class="k">def</span> <span class="nf">count</span><span class="p">(</span>
+</span><span id="DataBased-201"><a href="#DataBased-201"><span class="linenos">201</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="DataBased-202"><a href="#DataBased-202"><span class="linenos">202</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
+</span><span id="DataBased-203"><a href="#DataBased-203"><span class="linenos">203</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="DataBased-204"><a href="#DataBased-204"><span class="linenos">204</span></a>        <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="DataBased-205"><a href="#DataBased-205"><span class="linenos">205</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="DataBased-206"><a href="#DataBased-206"><span class="linenos">206</span></a>        <span class="sd">&quot;&quot;&quot;Return number of items in table.</span>
 </span><span id="DataBased-207"><a href="#DataBased-207"><span class="linenos">207</span></a>
-</span><span id="DataBased-208"><a href="#DataBased-208"><span class="linenos">208</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased-209"><a href="#DataBased-209"><span class="linenos">209</span></a>    <span class="k">def</span> <span class="nf">count</span><span class="p">(</span>
-</span><span id="DataBased-210"><a href="#DataBased-210"><span class="linenos">210</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="DataBased-211"><a href="#DataBased-211"><span class="linenos">211</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
-</span><span id="DataBased-212"><a href="#DataBased-212"><span class="linenos">212</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="DataBased-213"><a href="#DataBased-213"><span class="linenos">213</span></a>        <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="DataBased-214"><a href="#DataBased-214"><span class="linenos">214</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="DataBased-215"><a href="#DataBased-215"><span class="linenos">215</span></a>        <span class="sd">&quot;&quot;&quot;Return number of items in table.</span>
-</span><span id="DataBased-216"><a href="#DataBased-216"><span class="linenos">216</span></a>
-</span><span id="DataBased-217"><a href="#DataBased-217"><span class="linenos">217</span></a><span class="sd">        :param match_criteria: Can be a list of 2-tuples where each</span>
-</span><span id="DataBased-218"><a href="#DataBased-218"><span class="linenos">218</span></a><span class="sd">        tuple is (columnName, rowValue) or a dictionary where</span>
-</span><span id="DataBased-219"><a href="#DataBased-219"><span class="linenos">219</span></a><span class="sd">        keys are column names and values are row values.</span>
-</span><span id="DataBased-220"><a href="#DataBased-220"><span class="linenos">220</span></a><span class="sd">        If None, all rows from the table will be counted.</span>
-</span><span id="DataBased-221"><a href="#DataBased-221"><span class="linenos">221</span></a>
-</span><span id="DataBased-222"><a href="#DataBased-222"><span class="linenos">222</span></a><span class="sd">        :param exact_match: If False, the row value for a give column</span>
-</span><span id="DataBased-223"><a href="#DataBased-223"><span class="linenos">223</span></a><span class="sd">        in match_criteria will be matched as a substring. Has no effect if</span>
-</span><span id="DataBased-224"><a href="#DataBased-224"><span class="linenos">224</span></a><span class="sd">        match_criteria is None.</span>
-</span><span id="DataBased-225"><a href="#DataBased-225"><span class="linenos">225</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="DataBased-226"><a href="#DataBased-226"><span class="linenos">226</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;select count(_rowid_) from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="DataBased-227"><a href="#DataBased-227"><span class="linenos">227</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="DataBased-228"><a href="#DataBased-228"><span class="linenos">228</span></a>            <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
-</span><span id="DataBased-229"><a href="#DataBased-229"><span class="linenos">229</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="DataBased-230"><a href="#DataBased-230"><span class="linenos">230</span></a>                    <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">query</span><span class="si">}</span><span class="s2"> where </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="DataBased-231"><a href="#DataBased-231"><span class="linenos">231</span></a>                <span class="p">)</span>
-</span><span id="DataBased-232"><a href="#DataBased-232"><span class="linenos">232</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="DataBased-233"><a href="#DataBased-233"><span class="linenos">233</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">query</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DataBased-234"><a href="#DataBased-234"><span class="linenos">234</span></a>            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchone</span><span class="p">()[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="DataBased-235"><a href="#DataBased-235"><span class="linenos">235</span></a>        <span class="k">except</span><span class="p">:</span>
-</span><span id="DataBased-236"><a href="#DataBased-236"><span class="linenos">236</span></a>            <span class="k">return</span> <span class="mi">0</span>
-</span><span id="DataBased-237"><a href="#DataBased-237"><span class="linenos">237</span></a>
-</span><span id="DataBased-238"><a href="#DataBased-238"><span class="linenos">238</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased-239"><a href="#DataBased-239"><span class="linenos">239</span></a>    <span class="k">def</span> <span class="nf">add_row</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="nb">any</span><span class="p">],</span> <span class="n">columns</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="DataBased-240"><a href="#DataBased-240"><span class="linenos">240</span></a>        <span class="sd">&quot;&quot;&quot;Add row of values to table.</span>
-</span><span id="DataBased-241"><a href="#DataBased-241"><span class="linenos">241</span></a>
-</span><span id="DataBased-242"><a href="#DataBased-242"><span class="linenos">242</span></a><span class="sd">        :param table: The table to insert into.</span>
-</span><span id="DataBased-243"><a href="#DataBased-243"><span class="linenos">243</span></a>
-</span><span id="DataBased-244"><a href="#DataBased-244"><span class="linenos">244</span></a><span class="sd">        :param values: A tuple of values to be inserted into the table.</span>
-</span><span id="DataBased-245"><a href="#DataBased-245"><span class="linenos">245</span></a>
-</span><span id="DataBased-246"><a href="#DataBased-246"><span class="linenos">246</span></a><span class="sd">        :param columns: If None, values param is expected to supply</span>
-</span><span id="DataBased-247"><a href="#DataBased-247"><span class="linenos">247</span></a><span class="sd">        a value for every column in the table. If columns is</span>
-</span><span id="DataBased-248"><a href="#DataBased-248"><span class="linenos">248</span></a><span class="sd">        provided, it should contain the same number of elements as values.&quot;&quot;&quot;</span>
-</span><span id="DataBased-249"><a href="#DataBased-249"><span class="linenos">249</span></a>        <span class="n">parameterizer</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="s2">&quot;?&quot;</span> <span class="k">for</span> <span class="n">_</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
-</span><span id="DataBased-250"><a href="#DataBased-250"><span class="linenos">250</span></a>        <span class="n">logger_values</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
-</span><span id="DataBased-251"><a href="#DataBased-251"><span class="linenos">251</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="DataBased-252"><a href="#DataBased-252"><span class="linenos">252</span></a>            <span class="k">if</span> <span class="n">columns</span><span class="p">:</span>
-</span><span id="DataBased-253"><a href="#DataBased-253"><span class="linenos">253</span></a>                <span class="n">columns</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">column</span> <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span><span class="p">)</span>
-</span><span id="DataBased-254"><a href="#DataBased-254"><span class="linenos">254</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="DataBased-255"><a href="#DataBased-255"><span class="linenos">255</span></a>                    <span class="sa">f</span><span class="s2">&quot;insert into </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> (</span><span class="si">{</span><span class="n">columns</span><span class="si">}</span><span class="s2">) values(</span><span class="si">{</span><span class="n">parameterizer</span><span class="si">}</span><span class="s2">)&quot;</span><span class="p">,</span> <span class="n">values</span>
-</span><span id="DataBased-256"><a href="#DataBased-256"><span class="linenos">256</span></a>                <span class="p">)</span>
-</span><span id="DataBased-257"><a href="#DataBased-257"><span class="linenos">257</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="DataBased-258"><a href="#DataBased-258"><span class="linenos">258</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="DataBased-259"><a href="#DataBased-259"><span class="linenos">259</span></a>                    <span class="sa">f</span><span class="s2">&quot;insert into </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> values(</span><span class="si">{</span><span class="n">parameterizer</span><span class="si">}</span><span class="s2">)&quot;</span><span class="p">,</span> <span class="n">values</span>
+</span><span id="DataBased-208"><a href="#DataBased-208"><span class="linenos">208</span></a><span class="sd">        :param match_criteria: Can be a list of 2-tuples where each</span>
+</span><span id="DataBased-209"><a href="#DataBased-209"><span class="linenos">209</span></a><span class="sd">        tuple is (columnName, rowValue) or a dictionary where</span>
+</span><span id="DataBased-210"><a href="#DataBased-210"><span class="linenos">210</span></a><span class="sd">        keys are column names and values are row values.</span>
+</span><span id="DataBased-211"><a href="#DataBased-211"><span class="linenos">211</span></a><span class="sd">        If None, all rows from the table will be counted.</span>
+</span><span id="DataBased-212"><a href="#DataBased-212"><span class="linenos">212</span></a>
+</span><span id="DataBased-213"><a href="#DataBased-213"><span class="linenos">213</span></a><span class="sd">        :param exact_match: If False, the row value for a give column</span>
+</span><span id="DataBased-214"><a href="#DataBased-214"><span class="linenos">214</span></a><span class="sd">        in match_criteria will be matched as a substring. Has no effect if</span>
+</span><span id="DataBased-215"><a href="#DataBased-215"><span class="linenos">215</span></a><span class="sd">        match_criteria is None.</span>
+</span><span id="DataBased-216"><a href="#DataBased-216"><span class="linenos">216</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="DataBased-217"><a href="#DataBased-217"><span class="linenos">217</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;select count(_rowid_) from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="DataBased-218"><a href="#DataBased-218"><span class="linenos">218</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="DataBased-219"><a href="#DataBased-219"><span class="linenos">219</span></a>            <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
+</span><span id="DataBased-220"><a href="#DataBased-220"><span class="linenos">220</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="DataBased-221"><a href="#DataBased-221"><span class="linenos">221</span></a>                    <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">query</span><span class="si">}</span><span class="s2"> where </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="DataBased-222"><a href="#DataBased-222"><span class="linenos">222</span></a>                <span class="p">)</span>
+</span><span id="DataBased-223"><a href="#DataBased-223"><span class="linenos">223</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="DataBased-224"><a href="#DataBased-224"><span class="linenos">224</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">query</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DataBased-225"><a href="#DataBased-225"><span class="linenos">225</span></a>            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchone</span><span class="p">()[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="DataBased-226"><a href="#DataBased-226"><span class="linenos">226</span></a>        <span class="k">except</span><span class="p">:</span>
+</span><span id="DataBased-227"><a href="#DataBased-227"><span class="linenos">227</span></a>            <span class="k">return</span> <span class="mi">0</span>
+</span><span id="DataBased-228"><a href="#DataBased-228"><span class="linenos">228</span></a>
+</span><span id="DataBased-229"><a href="#DataBased-229"><span class="linenos">229</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased-230"><a href="#DataBased-230"><span class="linenos">230</span></a>    <span class="k">def</span> <span class="nf">add_row</span><span class="p">(</span>
+</span><span id="DataBased-231"><a href="#DataBased-231"><span class="linenos">231</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="n">Any</span><span class="p">],</span> <span class="n">columns</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="DataBased-232"><a href="#DataBased-232"><span class="linenos">232</span></a>    <span class="p">):</span>
+</span><span id="DataBased-233"><a href="#DataBased-233"><span class="linenos">233</span></a>        <span class="sd">&quot;&quot;&quot;Add row of values to table.</span>
+</span><span id="DataBased-234"><a href="#DataBased-234"><span class="linenos">234</span></a>
+</span><span id="DataBased-235"><a href="#DataBased-235"><span class="linenos">235</span></a><span class="sd">        :param table: The table to insert into.</span>
+</span><span id="DataBased-236"><a href="#DataBased-236"><span class="linenos">236</span></a>
+</span><span id="DataBased-237"><a href="#DataBased-237"><span class="linenos">237</span></a><span class="sd">        :param values: A tuple of values to be inserted into the table.</span>
+</span><span id="DataBased-238"><a href="#DataBased-238"><span class="linenos">238</span></a>
+</span><span id="DataBased-239"><a href="#DataBased-239"><span class="linenos">239</span></a><span class="sd">        :param columns: If None, values param is expected to supply</span>
+</span><span id="DataBased-240"><a href="#DataBased-240"><span class="linenos">240</span></a><span class="sd">        a value for every column in the table. If columns is</span>
+</span><span id="DataBased-241"><a href="#DataBased-241"><span class="linenos">241</span></a><span class="sd">        provided, it should contain the same number of elements as values.&quot;&quot;&quot;</span>
+</span><span id="DataBased-242"><a href="#DataBased-242"><span class="linenos">242</span></a>        <span class="n">parameterizer</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="s2">&quot;?&quot;</span> <span class="k">for</span> <span class="n">_</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
+</span><span id="DataBased-243"><a href="#DataBased-243"><span class="linenos">243</span></a>        <span class="n">logger_values</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
+</span><span id="DataBased-244"><a href="#DataBased-244"><span class="linenos">244</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="DataBased-245"><a href="#DataBased-245"><span class="linenos">245</span></a>            <span class="k">if</span> <span class="n">columns</span><span class="p">:</span>
+</span><span id="DataBased-246"><a href="#DataBased-246"><span class="linenos">246</span></a>                <span class="n">columns_query</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">column</span> <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span><span class="p">)</span>
+</span><span id="DataBased-247"><a href="#DataBased-247"><span class="linenos">247</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="DataBased-248"><a href="#DataBased-248"><span class="linenos">248</span></a>                    <span class="sa">f</span><span class="s2">&quot;insert into </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> (</span><span class="si">{</span><span class="n">columns_query</span><span class="si">}</span><span class="s2">) values(</span><span class="si">{</span><span class="n">parameterizer</span><span class="si">}</span><span class="s2">)&quot;</span><span class="p">,</span>
+</span><span id="DataBased-249"><a href="#DataBased-249"><span class="linenos">249</span></a>                    <span class="n">values</span><span class="p">,</span>
+</span><span id="DataBased-250"><a href="#DataBased-250"><span class="linenos">250</span></a>                <span class="p">)</span>
+</span><span id="DataBased-251"><a href="#DataBased-251"><span class="linenos">251</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="DataBased-252"><a href="#DataBased-252"><span class="linenos">252</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="DataBased-253"><a href="#DataBased-253"><span class="linenos">253</span></a>                    <span class="sa">f</span><span class="s2">&quot;insert into </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> values(</span><span class="si">{</span><span class="n">parameterizer</span><span class="si">}</span><span class="s2">)&quot;</span><span class="p">,</span> <span class="n">values</span>
+</span><span id="DataBased-254"><a href="#DataBased-254"><span class="linenos">254</span></a>                <span class="p">)</span>
+</span><span id="DataBased-255"><a href="#DataBased-255"><span class="linenos">255</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Added &quot;</span><span class="si">{</span><span class="n">logger_values</span><span class="si">}</span><span class="s1">&quot; to </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1"> table.&#39;</span><span class="p">)</span>
+</span><span id="DataBased-256"><a href="#DataBased-256"><span class="linenos">256</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DataBased-257"><a href="#DataBased-257"><span class="linenos">257</span></a>            <span class="k">if</span> <span class="s2">&quot;constraint&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">)</span><span class="o">.</span><span class="n">lower</span><span class="p">():</span>
+</span><span id="DataBased-258"><a href="#DataBased-258"><span class="linenos">258</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">exception</span><span class="p">(</span>
+</span><span id="DataBased-259"><a href="#DataBased-259"><span class="linenos">259</span></a>                    <span class="sa">f</span><span class="s1">&#39;Error adding &quot;</span><span class="si">{</span><span class="n">logger_values</span><span class="si">}</span><span class="s1">&quot; to </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1"> table.&#39;</span>
 </span><span id="DataBased-260"><a href="#DataBased-260"><span class="linenos">260</span></a>                <span class="p">)</span>
-</span><span id="DataBased-261"><a href="#DataBased-261"><span class="linenos">261</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Added &quot;</span><span class="si">{</span><span class="n">logger_values</span><span class="si">}</span><span class="s1">&quot; to </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1"> table.&#39;</span><span class="p">)</span>
-</span><span id="DataBased-262"><a href="#DataBased-262"><span class="linenos">262</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="DataBased-263"><a href="#DataBased-263"><span class="linenos">263</span></a>            <span class="k">if</span> <span class="s2">&quot;constraint&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">)</span><span class="o">.</span><span class="n">lower</span><span class="p">():</span>
-</span><span id="DataBased-264"><a href="#DataBased-264"><span class="linenos">264</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">exception</span><span class="p">(</span>
-</span><span id="DataBased-265"><a href="#DataBased-265"><span class="linenos">265</span></a>                    <span class="sa">f</span><span class="s1">&#39;Error adding &quot;</span><span class="si">{</span><span class="n">logger_values</span><span class="si">}</span><span class="s1">&quot; to </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1"> table.&#39;</span>
-</span><span id="DataBased-266"><a href="#DataBased-266"><span class="linenos">266</span></a>                <span class="p">)</span>
-</span><span id="DataBased-267"><a href="#DataBased-267"><span class="linenos">267</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="DataBased-268"><a href="#DataBased-268"><span class="linenos">268</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">debug</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">))</span>
-</span><span id="DataBased-269"><a href="#DataBased-269"><span class="linenos">269</span></a>
-</span><span id="DataBased-270"><a href="#DataBased-270"><span class="linenos">270</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased-271"><a href="#DataBased-271"><span class="linenos">271</span></a>    <span class="k">def</span> <span class="nf">get_rows</span><span class="p">(</span>
-</span><span id="DataBased-272"><a href="#DataBased-272"><span class="linenos">272</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="DataBased-273"><a href="#DataBased-273"><span class="linenos">273</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
-</span><span id="DataBased-274"><a href="#DataBased-274"><span class="linenos">274</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="DataBased-275"><a href="#DataBased-275"><span class="linenos">275</span></a>        <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="DataBased-276"><a href="#DataBased-276"><span class="linenos">276</span></a>        <span class="n">sort_by_column</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="DataBased-277"><a href="#DataBased-277"><span class="linenos">277</span></a>        <span class="n">columns_to_return</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="DataBased-278"><a href="#DataBased-278"><span class="linenos">278</span></a>        <span class="n">return_as_dataframe</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
-</span><span id="DataBased-279"><a href="#DataBased-279"><span class="linenos">279</span></a>        <span class="n">values_only</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
-</span><span id="DataBased-280"><a href="#DataBased-280"><span class="linenos">280</span></a>        <span class="n">order_by</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="DataBased-281"><a href="#DataBased-281"><span class="linenos">281</span></a>        <span class="n">limit</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="DataBased-282"><a href="#DataBased-282"><span class="linenos">282</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]</span> <span class="o">|</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="n">pandas</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">:</span>
-</span><span id="DataBased-283"><a href="#DataBased-283"><span class="linenos">283</span></a>        <span class="sd">&quot;&quot;&quot;Returns rows from table as a list of dictionaries</span>
-</span><span id="DataBased-284"><a href="#DataBased-284"><span class="linenos">284</span></a><span class="sd">        where the key-value pairs of the dictionaries are</span>
-</span><span id="DataBased-285"><a href="#DataBased-285"><span class="linenos">285</span></a><span class="sd">        column name: row value.</span>
-</span><span id="DataBased-286"><a href="#DataBased-286"><span class="linenos">286</span></a>
-</span><span id="DataBased-287"><a href="#DataBased-287"><span class="linenos">287</span></a><span class="sd">        :param match_criteria: Can be a list of 2-tuples where each</span>
-</span><span id="DataBased-288"><a href="#DataBased-288"><span class="linenos">288</span></a><span class="sd">        tuple is (columnName, rowValue) or a dictionary where</span>
-</span><span id="DataBased-289"><a href="#DataBased-289"><span class="linenos">289</span></a><span class="sd">        keys are column names and values are row values.</span>
-</span><span id="DataBased-290"><a href="#DataBased-290"><span class="linenos">290</span></a>
-</span><span id="DataBased-291"><a href="#DataBased-291"><span class="linenos">291</span></a><span class="sd">        :param exact_match: If False, the rowValue for a give column</span>
-</span><span id="DataBased-292"><a href="#DataBased-292"><span class="linenos">292</span></a><span class="sd">        will be matched as a substring.</span>
-</span><span id="DataBased-293"><a href="#DataBased-293"><span class="linenos">293</span></a>
-</span><span id="DataBased-294"><a href="#DataBased-294"><span class="linenos">294</span></a><span class="sd">        :param sort_by_column: A column name to sort the results by.</span>
-</span><span id="DataBased-295"><a href="#DataBased-295"><span class="linenos">295</span></a><span class="sd">        This will sort results in Python after retrieving them from the db.</span>
-</span><span id="DataBased-296"><a href="#DataBased-296"><span class="linenos">296</span></a><span class="sd">        Use the &#39;order_by&#39; param to use SQLite engine for ordering.</span>
-</span><span id="DataBased-297"><a href="#DataBased-297"><span class="linenos">297</span></a>
-</span><span id="DataBased-298"><a href="#DataBased-298"><span class="linenos">298</span></a><span class="sd">        :param columns_to_return: Optional list of column names.</span>
-</span><span id="DataBased-299"><a href="#DataBased-299"><span class="linenos">299</span></a><span class="sd">        If provided, the elements returned by get_rows() will</span>
-</span><span id="DataBased-300"><a href="#DataBased-300"><span class="linenos">300</span></a><span class="sd">        only contain the provided columns. Otherwise every column</span>
-</span><span id="DataBased-301"><a href="#DataBased-301"><span class="linenos">301</span></a><span class="sd">        in the row is returned.</span>
-</span><span id="DataBased-302"><a href="#DataBased-302"><span class="linenos">302</span></a>
-</span><span id="DataBased-303"><a href="#DataBased-303"><span class="linenos">303</span></a><span class="sd">        :param return_as_dataframe: If True,</span>
-</span><span id="DataBased-304"><a href="#DataBased-304"><span class="linenos">304</span></a><span class="sd">        the results will be returned as a pandas.DataFrame object.</span>
-</span><span id="DataBased-305"><a href="#DataBased-305"><span class="linenos">305</span></a>
-</span><span id="DataBased-306"><a href="#DataBased-306"><span class="linenos">306</span></a><span class="sd">        :param values_only: Return the results as a list of tuples</span>
-</span><span id="DataBased-307"><a href="#DataBased-307"><span class="linenos">307</span></a><span class="sd">        instead of a list of dictionaries that have column names as keys.</span>
-</span><span id="DataBased-308"><a href="#DataBased-308"><span class="linenos">308</span></a><span class="sd">        The results will still be sorted according to sort_by_column if</span>
-</span><span id="DataBased-309"><a href="#DataBased-309"><span class="linenos">309</span></a><span class="sd">        one is provided.</span>
-</span><span id="DataBased-310"><a href="#DataBased-310"><span class="linenos">310</span></a>
-</span><span id="DataBased-311"><a href="#DataBased-311"><span class="linenos">311</span></a><span class="sd">        :param order_by: If given, a &#39;order by {order_by}&#39; clause</span>
-</span><span id="DataBased-312"><a href="#DataBased-312"><span class="linenos">312</span></a><span class="sd">        will be added to the select query.</span>
-</span><span id="DataBased-313"><a href="#DataBased-313"><span class="linenos">313</span></a>
-</span><span id="DataBased-314"><a href="#DataBased-314"><span class="linenos">314</span></a><span class="sd">        :param limit: If given, a &#39;limit {limit}&#39; clause will be</span>
-</span><span id="DataBased-315"><a href="#DataBased-315"><span class="linenos">315</span></a><span class="sd">        added to the select query.</span>
-</span><span id="DataBased-316"><a href="#DataBased-316"><span class="linenos">316</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="DataBased-317"><a href="#DataBased-317"><span class="linenos">317</span></a>
-</span><span id="DataBased-318"><a href="#DataBased-318"><span class="linenos">318</span></a>        <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">columns_to_return</span><span class="p">)</span> <span class="ow">is</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="DataBased-319"><a href="#DataBased-319"><span class="linenos">319</span></a>            <span class="n">columns_to_return</span> <span class="o">=</span> <span class="p">[</span><span class="n">columns_to_return</span><span class="p">]</span>
-</span><span id="DataBased-320"><a href="#DataBased-320"><span class="linenos">320</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;select * from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="DataBased-321"><a href="#DataBased-321"><span class="linenos">321</span></a>        <span class="n">matches</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="DataBased-322"><a href="#DataBased-322"><span class="linenos">322</span></a>        <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
-</span><span id="DataBased-323"><a href="#DataBased-323"><span class="linenos">323</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; where </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="DataBased-324"><a href="#DataBased-324"><span class="linenos">324</span></a>        <span class="k">if</span> <span class="n">order_by</span><span class="p">:</span>
-</span><span id="DataBased-325"><a href="#DataBased-325"><span class="linenos">325</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; order by </span><span class="si">{</span><span class="n">order_by</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="DataBased-326"><a href="#DataBased-326"><span class="linenos">326</span></a>        <span class="k">if</span> <span class="n">limit</span><span class="p">:</span>
-</span><span id="DataBased-327"><a href="#DataBased-327"><span class="linenos">327</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; limit </span><span class="si">{</span><span class="n">limit</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="DataBased-328"><a href="#DataBased-328"><span class="linenos">328</span></a>        <span class="n">query</span> <span class="o">+=</span> <span class="s2">&quot;;&quot;</span>
-</span><span id="DataBased-329"><a href="#DataBased-329"><span class="linenos">329</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
-</span><span id="DataBased-330"><a href="#DataBased-330"><span class="linenos">330</span></a>        <span class="n">matches</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()</span>
-</span><span id="DataBased-331"><a href="#DataBased-331"><span class="linenos">331</span></a>        <span class="n">results</span> <span class="o">=</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_dict</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">match</span><span class="p">,</span> <span class="n">columns_to_return</span><span class="p">)</span> <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">]</span>
-</span><span id="DataBased-332"><a href="#DataBased-332"><span class="linenos">332</span></a>        <span class="k">if</span> <span class="n">sort_by_column</span><span class="p">:</span>
-</span><span id="DataBased-333"><a href="#DataBased-333"><span class="linenos">333</span></a>            <span class="n">results</span> <span class="o">=</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">results</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="k">lambda</span> <span class="n">x</span><span class="p">:</span> <span class="n">x</span><span class="p">[</span><span class="n">sort_by_column</span><span class="p">])</span>
-</span><span id="DataBased-334"><a href="#DataBased-334"><span class="linenos">334</span></a>        <span class="k">if</span> <span class="n">return_as_dataframe</span><span class="p">:</span>
-</span><span id="DataBased-335"><a href="#DataBased-335"><span class="linenos">335</span></a>            <span class="k">return</span> <span class="n">pandas</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">(</span><span class="n">results</span><span class="p">)</span>
-</span><span id="DataBased-336"><a href="#DataBased-336"><span class="linenos">336</span></a>        <span class="k">if</span> <span class="n">values_only</span><span class="p">:</span>
-</span><span id="DataBased-337"><a href="#DataBased-337"><span class="linenos">337</span></a>            <span class="k">return</span> <span class="p">[</span><span class="nb">tuple</span><span class="p">(</span><span class="n">row</span><span class="o">.</span><span class="n">values</span><span class="p">())</span> <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">results</span><span class="p">]</span>
-</span><span id="DataBased-338"><a href="#DataBased-338"><span class="linenos">338</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="DataBased-339"><a href="#DataBased-339"><span class="linenos">339</span></a>            <span class="k">return</span> <span class="n">results</span>
-</span><span id="DataBased-340"><a href="#DataBased-340"><span class="linenos">340</span></a>
-</span><span id="DataBased-341"><a href="#DataBased-341"><span class="linenos">341</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased-342"><a href="#DataBased-342"><span class="linenos">342</span></a>    <span class="k">def</span> <span class="nf">find</span><span class="p">(</span>
-</span><span id="DataBased-343"><a href="#DataBased-343"><span class="linenos">343</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">query_string</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">columns</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="DataBased-344"><a href="#DataBased-344"><span class="linenos">344</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">tuple</span><span class="p">[</span><span class="nb">dict</span><span class="p">]:</span>
-</span><span id="DataBased-345"><a href="#DataBased-345"><span class="linenos">345</span></a>        <span class="sd">&quot;&quot;&quot;Search for rows that contain query_string as a substring</span>
-</span><span id="DataBased-346"><a href="#DataBased-346"><span class="linenos">346</span></a><span class="sd">        of any column.</span>
-</span><span id="DataBased-347"><a href="#DataBased-347"><span class="linenos">347</span></a>
-</span><span id="DataBased-348"><a href="#DataBased-348"><span class="linenos">348</span></a><span class="sd">        :param table: The table to search.</span>
-</span><span id="DataBased-349"><a href="#DataBased-349"><span class="linenos">349</span></a>
-</span><span id="DataBased-350"><a href="#DataBased-350"><span class="linenos">350</span></a><span class="sd">        :param query_string: The substring to search for in all columns.</span>
-</span><span id="DataBased-351"><a href="#DataBased-351"><span class="linenos">351</span></a>
-</span><span id="DataBased-352"><a href="#DataBased-352"><span class="linenos">352</span></a><span class="sd">        :param columns: A list of columns to search for query_string.</span>
-</span><span id="DataBased-353"><a href="#DataBased-353"><span class="linenos">353</span></a><span class="sd">        If None, all columns in the table will be searched.</span>
-</span><span id="DataBased-354"><a href="#DataBased-354"><span class="linenos">354</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="DataBased-355"><a href="#DataBased-355"><span class="linenos">355</span></a>        <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">columns</span><span class="p">)</span> <span class="ow">is</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="DataBased-356"><a href="#DataBased-356"><span class="linenos">356</span></a>            <span class="n">columns</span> <span class="o">=</span> <span class="p">[</span><span class="n">columns</span><span class="p">]</span>
-</span><span id="DataBased-357"><a href="#DataBased-357"><span class="linenos">357</span></a>        <span class="n">results</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="DataBased-358"><a href="#DataBased-358"><span class="linenos">358</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">columns</span><span class="p">:</span>
-</span><span id="DataBased-359"><a href="#DataBased-359"><span class="linenos">359</span></a>            <span class="n">columns</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_column_names</span><span class="p">(</span><span class="n">table</span><span class="p">)</span>
-</span><span id="DataBased-360"><a href="#DataBased-360"><span class="linenos">360</span></a>        <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span><span class="p">:</span>
-</span><span id="DataBased-361"><a href="#DataBased-361"><span class="linenos">361</span></a>            <span class="n">results</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span>
-</span><span id="DataBased-362"><a href="#DataBased-362"><span class="linenos">362</span></a>                <span class="p">[</span>
-</span><span id="DataBased-363"><a href="#DataBased-363"><span class="linenos">363</span></a>                    <span class="n">row</span>
-</span><span id="DataBased-364"><a href="#DataBased-364"><span class="linenos">364</span></a>                    <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_rows</span><span class="p">(</span>
-</span><span id="DataBased-365"><a href="#DataBased-365"><span class="linenos">365</span></a>                        <span class="n">table</span><span class="p">,</span> <span class="p">[(</span><span class="n">column</span><span class="p">,</span> <span class="n">query_string</span><span class="p">)],</span> <span class="n">exact_match</span><span class="o">=</span><span class="kc">False</span>
-</span><span id="DataBased-366"><a href="#DataBased-366"><span class="linenos">366</span></a>                    <span class="p">)</span>
-</span><span id="DataBased-367"><a href="#DataBased-367"><span class="linenos">367</span></a>                    <span class="k">if</span> <span class="n">row</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">results</span>
-</span><span id="DataBased-368"><a href="#DataBased-368"><span class="linenos">368</span></a>                <span class="p">]</span>
-</span><span id="DataBased-369"><a href="#DataBased-369"><span class="linenos">369</span></a>            <span class="p">)</span>
-</span><span id="DataBased-370"><a href="#DataBased-370"><span class="linenos">370</span></a>        <span class="k">return</span> <span class="n">results</span>
+</span><span id="DataBased-261"><a href="#DataBased-261"><span class="linenos">261</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="DataBased-262"><a href="#DataBased-262"><span class="linenos">262</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">debug</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">))</span>
+</span><span id="DataBased-263"><a href="#DataBased-263"><span class="linenos">263</span></a>
+</span><span id="DataBased-264"><a href="#DataBased-264"><span class="linenos">264</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased-265"><a href="#DataBased-265"><span class="linenos">265</span></a>    <span class="k">def</span> <span class="nf">get_rows</span><span class="p">(</span>
+</span><span id="DataBased-266"><a href="#DataBased-266"><span class="linenos">266</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="DataBased-267"><a href="#DataBased-267"><span class="linenos">267</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
+</span><span id="DataBased-268"><a href="#DataBased-268"><span class="linenos">268</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="DataBased-269"><a href="#DataBased-269"><span class="linenos">269</span></a>        <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="DataBased-270"><a href="#DataBased-270"><span class="linenos">270</span></a>        <span class="n">sort_by_column</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="DataBased-271"><a href="#DataBased-271"><span class="linenos">271</span></a>        <span class="n">columns_to_return</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="DataBased-272"><a href="#DataBased-272"><span class="linenos">272</span></a>        <span class="n">return_as_dataframe</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
+</span><span id="DataBased-273"><a href="#DataBased-273"><span class="linenos">273</span></a>        <span class="n">values_only</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
+</span><span id="DataBased-274"><a href="#DataBased-274"><span class="linenos">274</span></a>        <span class="n">order_by</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="DataBased-275"><a href="#DataBased-275"><span class="linenos">275</span></a>        <span class="n">limit</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="DataBased-276"><a href="#DataBased-276"><span class="linenos">276</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]</span> <span class="o">|</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="n">pandas</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">:</span>
+</span><span id="DataBased-277"><a href="#DataBased-277"><span class="linenos">277</span></a>        <span class="sd">&quot;&quot;&quot;Returns rows from table as a list of dictionaries</span>
+</span><span id="DataBased-278"><a href="#DataBased-278"><span class="linenos">278</span></a><span class="sd">        where the key-value pairs of the dictionaries are</span>
+</span><span id="DataBased-279"><a href="#DataBased-279"><span class="linenos">279</span></a><span class="sd">        column name: row value.</span>
+</span><span id="DataBased-280"><a href="#DataBased-280"><span class="linenos">280</span></a>
+</span><span id="DataBased-281"><a href="#DataBased-281"><span class="linenos">281</span></a><span class="sd">        :param match_criteria: Can be a list of 2-tuples where each</span>
+</span><span id="DataBased-282"><a href="#DataBased-282"><span class="linenos">282</span></a><span class="sd">        tuple is (columnName, rowValue) or a dictionary where</span>
+</span><span id="DataBased-283"><a href="#DataBased-283"><span class="linenos">283</span></a><span class="sd">        keys are column names and values are row values.</span>
+</span><span id="DataBased-284"><a href="#DataBased-284"><span class="linenos">284</span></a>
+</span><span id="DataBased-285"><a href="#DataBased-285"><span class="linenos">285</span></a><span class="sd">        :param exact_match: If False, the rowValue for a give column</span>
+</span><span id="DataBased-286"><a href="#DataBased-286"><span class="linenos">286</span></a><span class="sd">        will be matched as a substring.</span>
+</span><span id="DataBased-287"><a href="#DataBased-287"><span class="linenos">287</span></a>
+</span><span id="DataBased-288"><a href="#DataBased-288"><span class="linenos">288</span></a><span class="sd">        :param sort_by_column: A column name to sort the results by.</span>
+</span><span id="DataBased-289"><a href="#DataBased-289"><span class="linenos">289</span></a><span class="sd">        This will sort results in Python after retrieving them from the db.</span>
+</span><span id="DataBased-290"><a href="#DataBased-290"><span class="linenos">290</span></a><span class="sd">        Use the &#39;order_by&#39; param to use SQLite engine for ordering.</span>
+</span><span id="DataBased-291"><a href="#DataBased-291"><span class="linenos">291</span></a>
+</span><span id="DataBased-292"><a href="#DataBased-292"><span class="linenos">292</span></a><span class="sd">        :param columns_to_return: Optional list of column names.</span>
+</span><span id="DataBased-293"><a href="#DataBased-293"><span class="linenos">293</span></a><span class="sd">        If provided, the elements returned by get_rows() will</span>
+</span><span id="DataBased-294"><a href="#DataBased-294"><span class="linenos">294</span></a><span class="sd">        only contain the provided columns. Otherwise every column</span>
+</span><span id="DataBased-295"><a href="#DataBased-295"><span class="linenos">295</span></a><span class="sd">        in the row is returned.</span>
+</span><span id="DataBased-296"><a href="#DataBased-296"><span class="linenos">296</span></a>
+</span><span id="DataBased-297"><a href="#DataBased-297"><span class="linenos">297</span></a><span class="sd">        :param return_as_dataframe: If True,</span>
+</span><span id="DataBased-298"><a href="#DataBased-298"><span class="linenos">298</span></a><span class="sd">        the results will be returned as a pandas.DataFrame object.</span>
+</span><span id="DataBased-299"><a href="#DataBased-299"><span class="linenos">299</span></a>
+</span><span id="DataBased-300"><a href="#DataBased-300"><span class="linenos">300</span></a><span class="sd">        :param values_only: Return the results as a list of tuples</span>
+</span><span id="DataBased-301"><a href="#DataBased-301"><span class="linenos">301</span></a><span class="sd">        instead of a list of dictionaries that have column names as keys.</span>
+</span><span id="DataBased-302"><a href="#DataBased-302"><span class="linenos">302</span></a><span class="sd">        The results will still be sorted according to sort_by_column if</span>
+</span><span id="DataBased-303"><a href="#DataBased-303"><span class="linenos">303</span></a><span class="sd">        one is provided.</span>
+</span><span id="DataBased-304"><a href="#DataBased-304"><span class="linenos">304</span></a>
+</span><span id="DataBased-305"><a href="#DataBased-305"><span class="linenos">305</span></a><span class="sd">        :param order_by: If given, a &#39;order by {order_by}&#39; clause</span>
+</span><span id="DataBased-306"><a href="#DataBased-306"><span class="linenos">306</span></a><span class="sd">        will be added to the select query.</span>
+</span><span id="DataBased-307"><a href="#DataBased-307"><span class="linenos">307</span></a>
+</span><span id="DataBased-308"><a href="#DataBased-308"><span class="linenos">308</span></a><span class="sd">        :param limit: If given, a &#39;limit {limit}&#39; clause will be</span>
+</span><span id="DataBased-309"><a href="#DataBased-309"><span class="linenos">309</span></a><span class="sd">        added to the select query.</span>
+</span><span id="DataBased-310"><a href="#DataBased-310"><span class="linenos">310</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="DataBased-311"><a href="#DataBased-311"><span class="linenos">311</span></a>
+</span><span id="DataBased-312"><a href="#DataBased-312"><span class="linenos">312</span></a>        <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">columns_to_return</span><span class="p">)</span> <span class="ow">is</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="DataBased-313"><a href="#DataBased-313"><span class="linenos">313</span></a>            <span class="n">columns_to_return</span> <span class="o">=</span> <span class="p">[</span><span class="n">columns_to_return</span><span class="p">]</span>
+</span><span id="DataBased-314"><a href="#DataBased-314"><span class="linenos">314</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;select * from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="DataBased-315"><a href="#DataBased-315"><span class="linenos">315</span></a>        <span class="n">matches</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="DataBased-316"><a href="#DataBased-316"><span class="linenos">316</span></a>        <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
+</span><span id="DataBased-317"><a href="#DataBased-317"><span class="linenos">317</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; where </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="DataBased-318"><a href="#DataBased-318"><span class="linenos">318</span></a>        <span class="k">if</span> <span class="n">order_by</span><span class="p">:</span>
+</span><span id="DataBased-319"><a href="#DataBased-319"><span class="linenos">319</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; order by </span><span class="si">{</span><span class="n">order_by</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="DataBased-320"><a href="#DataBased-320"><span class="linenos">320</span></a>        <span class="k">if</span> <span class="n">limit</span><span class="p">:</span>
+</span><span id="DataBased-321"><a href="#DataBased-321"><span class="linenos">321</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; limit </span><span class="si">{</span><span class="n">limit</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="DataBased-322"><a href="#DataBased-322"><span class="linenos">322</span></a>        <span class="n">query</span> <span class="o">+=</span> <span class="s2">&quot;;&quot;</span>
+</span><span id="DataBased-323"><a href="#DataBased-323"><span class="linenos">323</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
+</span><span id="DataBased-324"><a href="#DataBased-324"><span class="linenos">324</span></a>        <span class="n">matches</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()</span>
+</span><span id="DataBased-325"><a href="#DataBased-325"><span class="linenos">325</span></a>        <span class="n">results</span> <span class="o">=</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_dict</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">match</span><span class="p">,</span> <span class="n">columns_to_return</span><span class="p">)</span> <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">]</span>
+</span><span id="DataBased-326"><a href="#DataBased-326"><span class="linenos">326</span></a>        <span class="k">if</span> <span class="n">sort_by_column</span><span class="p">:</span>
+</span><span id="DataBased-327"><a href="#DataBased-327"><span class="linenos">327</span></a>            <span class="n">results</span> <span class="o">=</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">results</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="k">lambda</span> <span class="n">x</span><span class="p">:</span> <span class="n">x</span><span class="p">[</span><span class="n">sort_by_column</span><span class="p">])</span>
+</span><span id="DataBased-328"><a href="#DataBased-328"><span class="linenos">328</span></a>        <span class="k">if</span> <span class="n">return_as_dataframe</span><span class="p">:</span>
+</span><span id="DataBased-329"><a href="#DataBased-329"><span class="linenos">329</span></a>            <span class="k">return</span> <span class="n">pandas</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">(</span><span class="n">results</span><span class="p">)</span>
+</span><span id="DataBased-330"><a href="#DataBased-330"><span class="linenos">330</span></a>        <span class="k">if</span> <span class="n">values_only</span><span class="p">:</span>
+</span><span id="DataBased-331"><a href="#DataBased-331"><span class="linenos">331</span></a>            <span class="k">return</span> <span class="p">[</span><span class="nb">tuple</span><span class="p">(</span><span class="n">row</span><span class="o">.</span><span class="n">values</span><span class="p">())</span> <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">results</span><span class="p">]</span>
+</span><span id="DataBased-332"><a href="#DataBased-332"><span class="linenos">332</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="DataBased-333"><a href="#DataBased-333"><span class="linenos">333</span></a>            <span class="k">return</span> <span class="n">results</span>
+</span><span id="DataBased-334"><a href="#DataBased-334"><span class="linenos">334</span></a>
+</span><span id="DataBased-335"><a href="#DataBased-335"><span class="linenos">335</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased-336"><a href="#DataBased-336"><span class="linenos">336</span></a>    <span class="k">def</span> <span class="nf">find</span><span class="p">(</span>
+</span><span id="DataBased-337"><a href="#DataBased-337"><span class="linenos">337</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">query_string</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">columns</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="DataBased-338"><a href="#DataBased-338"><span class="linenos">338</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]:</span>
+</span><span id="DataBased-339"><a href="#DataBased-339"><span class="linenos">339</span></a>        <span class="sd">&quot;&quot;&quot;Search for rows that contain query_string as a substring</span>
+</span><span id="DataBased-340"><a href="#DataBased-340"><span class="linenos">340</span></a><span class="sd">        of any column.</span>
+</span><span id="DataBased-341"><a href="#DataBased-341"><span class="linenos">341</span></a>
+</span><span id="DataBased-342"><a href="#DataBased-342"><span class="linenos">342</span></a><span class="sd">        :param table: The table to search.</span>
+</span><span id="DataBased-343"><a href="#DataBased-343"><span class="linenos">343</span></a>
+</span><span id="DataBased-344"><a href="#DataBased-344"><span class="linenos">344</span></a><span class="sd">        :param query_string: The substring to search for in all columns.</span>
+</span><span id="DataBased-345"><a href="#DataBased-345"><span class="linenos">345</span></a>
+</span><span id="DataBased-346"><a href="#DataBased-346"><span class="linenos">346</span></a><span class="sd">        :param columns: A list of columns to search for query_string.</span>
+</span><span id="DataBased-347"><a href="#DataBased-347"><span class="linenos">347</span></a><span class="sd">        If None, all columns in the table will be searched.</span>
+</span><span id="DataBased-348"><a href="#DataBased-348"><span class="linenos">348</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="DataBased-349"><a href="#DataBased-349"><span class="linenos">349</span></a>        <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">columns</span><span class="p">)</span> <span class="ow">is</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="DataBased-350"><a href="#DataBased-350"><span class="linenos">350</span></a>            <span class="n">columns</span> <span class="o">=</span> <span class="p">[</span><span class="n">columns</span><span class="p">]</span>
+</span><span id="DataBased-351"><a href="#DataBased-351"><span class="linenos">351</span></a>        <span class="n">results</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="DataBased-352"><a href="#DataBased-352"><span class="linenos">352</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">columns</span><span class="p">:</span>
+</span><span id="DataBased-353"><a href="#DataBased-353"><span class="linenos">353</span></a>            <span class="n">columns</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_column_names</span><span class="p">(</span><span class="n">table</span><span class="p">)</span>
+</span><span id="DataBased-354"><a href="#DataBased-354"><span class="linenos">354</span></a>        <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span><span class="p">:</span>
+</span><span id="DataBased-355"><a href="#DataBased-355"><span class="linenos">355</span></a>            <span class="n">results</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span>
+</span><span id="DataBased-356"><a href="#DataBased-356"><span class="linenos">356</span></a>                <span class="p">[</span>
+</span><span id="DataBased-357"><a href="#DataBased-357"><span class="linenos">357</span></a>                    <span class="n">row</span>
+</span><span id="DataBased-358"><a href="#DataBased-358"><span class="linenos">358</span></a>                    <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_rows</span><span class="p">(</span>
+</span><span id="DataBased-359"><a href="#DataBased-359"><span class="linenos">359</span></a>                        <span class="n">table</span><span class="p">,</span> <span class="p">[(</span><span class="n">column</span><span class="p">,</span> <span class="n">query_string</span><span class="p">)],</span> <span class="n">exact_match</span><span class="o">=</span><span class="kc">False</span>
+</span><span id="DataBased-360"><a href="#DataBased-360"><span class="linenos">360</span></a>                    <span class="p">)</span>
+</span><span id="DataBased-361"><a href="#DataBased-361"><span class="linenos">361</span></a>                    <span class="k">if</span> <span class="n">row</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">results</span>
+</span><span id="DataBased-362"><a href="#DataBased-362"><span class="linenos">362</span></a>                <span class="p">]</span>
+</span><span id="DataBased-363"><a href="#DataBased-363"><span class="linenos">363</span></a>            <span class="p">)</span>
+</span><span id="DataBased-364"><a href="#DataBased-364"><span class="linenos">364</span></a>        <span class="k">return</span> <span class="n">results</span>
+</span><span id="DataBased-365"><a href="#DataBased-365"><span class="linenos">365</span></a>
+</span><span id="DataBased-366"><a href="#DataBased-366"><span class="linenos">366</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased-367"><a href="#DataBased-367"><span class="linenos">367</span></a>    <span class="k">def</span> <span class="nf">delete</span><span class="p">(</span>
+</span><span id="DataBased-368"><a href="#DataBased-368"><span class="linenos">368</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="DataBased-369"><a href="#DataBased-369"><span class="linenos">369</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="DataBased-370"><a href="#DataBased-370"><span class="linenos">370</span></a>        <span class="sd">&quot;&quot;&quot;Delete records from table.</span>
 </span><span id="DataBased-371"><a href="#DataBased-371"><span class="linenos">371</span></a>
-</span><span id="DataBased-372"><a href="#DataBased-372"><span class="linenos">372</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased-373"><a href="#DataBased-373"><span class="linenos">373</span></a>    <span class="k">def</span> <span class="nf">delete</span><span class="p">(</span>
-</span><span id="DataBased-374"><a href="#DataBased-374"><span class="linenos">374</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="DataBased-375"><a href="#DataBased-375"><span class="linenos">375</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="DataBased-376"><a href="#DataBased-376"><span class="linenos">376</span></a>        <span class="sd">&quot;&quot;&quot;Delete records from table.</span>
+</span><span id="DataBased-372"><a href="#DataBased-372"><span class="linenos">372</span></a><span class="sd">        Returns number of deleted records.</span>
+</span><span id="DataBased-373"><a href="#DataBased-373"><span class="linenos">373</span></a>
+</span><span id="DataBased-374"><a href="#DataBased-374"><span class="linenos">374</span></a><span class="sd">        :param match_criteria: Can be a list of 2-tuples where each</span>
+</span><span id="DataBased-375"><a href="#DataBased-375"><span class="linenos">375</span></a><span class="sd">        tuple is (columnName, rowValue) or a dictionary where</span>
+</span><span id="DataBased-376"><a href="#DataBased-376"><span class="linenos">376</span></a><span class="sd">        keys are column names and values are row values.</span>
 </span><span id="DataBased-377"><a href="#DataBased-377"><span class="linenos">377</span></a>
-</span><span id="DataBased-378"><a href="#DataBased-378"><span class="linenos">378</span></a><span class="sd">        Returns number of deleted records.</span>
-</span><span id="DataBased-379"><a href="#DataBased-379"><span class="linenos">379</span></a>
-</span><span id="DataBased-380"><a href="#DataBased-380"><span class="linenos">380</span></a><span class="sd">        :param match_criteria: Can be a list of 2-tuples where each</span>
-</span><span id="DataBased-381"><a href="#DataBased-381"><span class="linenos">381</span></a><span class="sd">        tuple is (columnName, rowValue) or a dictionary where</span>
-</span><span id="DataBased-382"><a href="#DataBased-382"><span class="linenos">382</span></a><span class="sd">        keys are column names and values are row values.</span>
-</span><span id="DataBased-383"><a href="#DataBased-383"><span class="linenos">383</span></a>
-</span><span id="DataBased-384"><a href="#DataBased-384"><span class="linenos">384</span></a><span class="sd">        :param exact_match: If False, the rowValue for a give column</span>
-</span><span id="DataBased-385"><a href="#DataBased-385"><span class="linenos">385</span></a><span class="sd">        will be matched as a substring.</span>
-</span><span id="DataBased-386"><a href="#DataBased-386"><span class="linenos">386</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="DataBased-387"><a href="#DataBased-387"><span class="linenos">387</span></a>        <span class="n">num_matches</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">count</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span>
-</span><span id="DataBased-388"><a href="#DataBased-388"><span class="linenos">388</span></a>        <span class="n">conditions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span>
-</span><span id="DataBased-389"><a href="#DataBased-389"><span class="linenos">389</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="DataBased-390"><a href="#DataBased-390"><span class="linenos">390</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;delete from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DataBased-391"><a href="#DataBased-391"><span class="linenos">391</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
-</span><span id="DataBased-392"><a href="#DataBased-392"><span class="linenos">392</span></a>                <span class="sa">f</span><span class="s1">&#39;Deleted </span><span class="si">{</span><span class="n">num_matches</span><span class="si">}</span><span class="s1"> from &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&quot;.&#39;</span>
-</span><span id="DataBased-393"><a href="#DataBased-393"><span class="linenos">393</span></a>            <span class="p">)</span>
-</span><span id="DataBased-394"><a href="#DataBased-394"><span class="linenos">394</span></a>            <span class="k">return</span> <span class="n">num_matches</span>
-</span><span id="DataBased-395"><a href="#DataBased-395"><span class="linenos">395</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="DataBased-396"><a href="#DataBased-396"><span class="linenos">396</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">debug</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Error deleting from &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">.</span><span class="se">\n</span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s1">&#39;</span><span class="p">)</span>
-</span><span id="DataBased-397"><a href="#DataBased-397"><span class="linenos">397</span></a>            <span class="k">return</span> <span class="mi">0</span>
-</span><span id="DataBased-398"><a href="#DataBased-398"><span class="linenos">398</span></a>
-</span><span id="DataBased-399"><a href="#DataBased-399"><span class="linenos">399</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased-400"><a href="#DataBased-400"><span class="linenos">400</span></a>    <span class="k">def</span> <span class="nf">update</span><span class="p">(</span>
-</span><span id="DataBased-401"><a href="#DataBased-401"><span class="linenos">401</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="DataBased-402"><a href="#DataBased-402"><span class="linenos">402</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
-</span><span id="DataBased-403"><a href="#DataBased-403"><span class="linenos">403</span></a>        <span class="n">column_to_update</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
-</span><span id="DataBased-404"><a href="#DataBased-404"><span class="linenos">404</span></a>        <span class="n">new_value</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
-</span><span id="DataBased-405"><a href="#DataBased-405"><span class="linenos">405</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="DataBased-406"><a href="#DataBased-406"><span class="linenos">406</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="DataBased-407"><a href="#DataBased-407"><span class="linenos">407</span></a>        <span class="sd">&quot;&quot;&quot;Update row value for entry matched with match_criteria.</span>
-</span><span id="DataBased-408"><a href="#DataBased-408"><span class="linenos">408</span></a>
-</span><span id="DataBased-409"><a href="#DataBased-409"><span class="linenos">409</span></a><span class="sd">        :param column_to_update: The column to be updated in the matched row.</span>
-</span><span id="DataBased-410"><a href="#DataBased-410"><span class="linenos">410</span></a>
-</span><span id="DataBased-411"><a href="#DataBased-411"><span class="linenos">411</span></a><span class="sd">        :param new_value: The new value to insert.</span>
-</span><span id="DataBased-412"><a href="#DataBased-412"><span class="linenos">412</span></a>
-</span><span id="DataBased-413"><a href="#DataBased-413"><span class="linenos">413</span></a><span class="sd">        :param match_criteria: Can be a list of 2-tuples where each</span>
-</span><span id="DataBased-414"><a href="#DataBased-414"><span class="linenos">414</span></a><span class="sd">        tuple is (columnName, rowValue) or a dictionary where</span>
-</span><span id="DataBased-415"><a href="#DataBased-415"><span class="linenos">415</span></a><span class="sd">        keys are column names and values are row values.</span>
-</span><span id="DataBased-416"><a href="#DataBased-416"><span class="linenos">416</span></a><span class="sd">        If None, every row will be updated.</span>
-</span><span id="DataBased-417"><a href="#DataBased-417"><span class="linenos">417</span></a>
-</span><span id="DataBased-418"><a href="#DataBased-418"><span class="linenos">418</span></a><span class="sd">        Returns True if successful, False if not.&quot;&quot;&quot;</span>
-</span><span id="DataBased-419"><a href="#DataBased-419"><span class="linenos">419</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;update </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> set </span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s2"> = ?&quot;</span>
-</span><span id="DataBased-420"><a href="#DataBased-420"><span class="linenos">420</span></a>        <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
-</span><span id="DataBased-421"><a href="#DataBased-421"><span class="linenos">421</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">count</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="DataBased-422"><a href="#DataBased-422"><span class="linenos">422</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
-</span><span id="DataBased-423"><a href="#DataBased-423"><span class="linenos">423</span></a>                    <span class="sa">f</span><span class="s2">&quot;Couldn&#39;t find matching records in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table to update to &#39;</span><span class="si">{</span><span class="n">new_value</span><span class="si">}</span><span class="s2">&#39;&quot;</span>
-</span><span id="DataBased-424"><a href="#DataBased-424"><span class="linenos">424</span></a>                <span class="p">)</span>
-</span><span id="DataBased-425"><a href="#DataBased-425"><span class="linenos">425</span></a>                <span class="k">return</span> <span class="kc">False</span>
-</span><span id="DataBased-426"><a href="#DataBased-426"><span class="linenos">426</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">)</span>
-</span><span id="DataBased-427"><a href="#DataBased-427"><span class="linenos">427</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="DataBased-428"><a href="#DataBased-428"><span class="linenos">428</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="DataBased-429"><a href="#DataBased-429"><span class="linenos">429</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="DataBased-430"><a href="#DataBased-430"><span class="linenos">430</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="DataBased-431"><a href="#DataBased-431"><span class="linenos">431</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="DataBased-432"><a href="#DataBased-432"><span class="linenos">432</span></a>                <span class="n">query</span><span class="p">,</span>
-</span><span id="DataBased-433"><a href="#DataBased-433"><span class="linenos">433</span></a>                <span class="p">(</span><span class="n">new_value</span><span class="p">,),</span>
-</span><span id="DataBased-434"><a href="#DataBased-434"><span class="linenos">434</span></a>            <span class="p">)</span>
-</span><span id="DataBased-435"><a href="#DataBased-435"><span class="linenos">435</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
-</span><span id="DataBased-436"><a href="#DataBased-436"><span class="linenos">436</span></a>                <span class="sa">f</span><span class="s1">&#39;Updated &quot;</span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s1">&quot; in &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table to &quot;</span><span class="si">{</span><span class="n">new_value</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&#39;</span>
+</span><span id="DataBased-378"><a href="#DataBased-378"><span class="linenos">378</span></a><span class="sd">        :param exact_match: If False, the rowValue for a give column</span>
+</span><span id="DataBased-379"><a href="#DataBased-379"><span class="linenos">379</span></a><span class="sd">        will be matched as a substring.</span>
+</span><span id="DataBased-380"><a href="#DataBased-380"><span class="linenos">380</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="DataBased-381"><a href="#DataBased-381"><span class="linenos">381</span></a>        <span class="n">num_matches</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">count</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span>
+</span><span id="DataBased-382"><a href="#DataBased-382"><span class="linenos">382</span></a>        <span class="n">conditions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span>
+</span><span id="DataBased-383"><a href="#DataBased-383"><span class="linenos">383</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="DataBased-384"><a href="#DataBased-384"><span class="linenos">384</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;delete from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DataBased-385"><a href="#DataBased-385"><span class="linenos">385</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
+</span><span id="DataBased-386"><a href="#DataBased-386"><span class="linenos">386</span></a>                <span class="sa">f</span><span class="s1">&#39;Deleted </span><span class="si">{</span><span class="n">num_matches</span><span class="si">}</span><span class="s1"> from &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&quot;.&#39;</span>
+</span><span id="DataBased-387"><a href="#DataBased-387"><span class="linenos">387</span></a>            <span class="p">)</span>
+</span><span id="DataBased-388"><a href="#DataBased-388"><span class="linenos">388</span></a>            <span class="k">return</span> <span class="n">num_matches</span>
+</span><span id="DataBased-389"><a href="#DataBased-389"><span class="linenos">389</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DataBased-390"><a href="#DataBased-390"><span class="linenos">390</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">debug</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Error deleting from &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">.</span><span class="se">\n</span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s1">&#39;</span><span class="p">)</span>
+</span><span id="DataBased-391"><a href="#DataBased-391"><span class="linenos">391</span></a>            <span class="k">return</span> <span class="mi">0</span>
+</span><span id="DataBased-392"><a href="#DataBased-392"><span class="linenos">392</span></a>
+</span><span id="DataBased-393"><a href="#DataBased-393"><span class="linenos">393</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased-394"><a href="#DataBased-394"><span class="linenos">394</span></a>    <span class="k">def</span> <span class="nf">update</span><span class="p">(</span>
+</span><span id="DataBased-395"><a href="#DataBased-395"><span class="linenos">395</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="DataBased-396"><a href="#DataBased-396"><span class="linenos">396</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
+</span><span id="DataBased-397"><a href="#DataBased-397"><span class="linenos">397</span></a>        <span class="n">column_to_update</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
+</span><span id="DataBased-398"><a href="#DataBased-398"><span class="linenos">398</span></a>        <span class="n">new_value</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
+</span><span id="DataBased-399"><a href="#DataBased-399"><span class="linenos">399</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="DataBased-400"><a href="#DataBased-400"><span class="linenos">400</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="DataBased-401"><a href="#DataBased-401"><span class="linenos">401</span></a>        <span class="sd">&quot;&quot;&quot;Update row value for entry matched with match_criteria.</span>
+</span><span id="DataBased-402"><a href="#DataBased-402"><span class="linenos">402</span></a>
+</span><span id="DataBased-403"><a href="#DataBased-403"><span class="linenos">403</span></a><span class="sd">        :param column_to_update: The column to be updated in the matched row.</span>
+</span><span id="DataBased-404"><a href="#DataBased-404"><span class="linenos">404</span></a>
+</span><span id="DataBased-405"><a href="#DataBased-405"><span class="linenos">405</span></a><span class="sd">        :param new_value: The new value to insert.</span>
+</span><span id="DataBased-406"><a href="#DataBased-406"><span class="linenos">406</span></a>
+</span><span id="DataBased-407"><a href="#DataBased-407"><span class="linenos">407</span></a><span class="sd">        :param match_criteria: Can be a list of 2-tuples where each</span>
+</span><span id="DataBased-408"><a href="#DataBased-408"><span class="linenos">408</span></a><span class="sd">        tuple is (columnName, rowValue) or a dictionary where</span>
+</span><span id="DataBased-409"><a href="#DataBased-409"><span class="linenos">409</span></a><span class="sd">        keys are column names and values are row values.</span>
+</span><span id="DataBased-410"><a href="#DataBased-410"><span class="linenos">410</span></a><span class="sd">        If None, every row will be updated.</span>
+</span><span id="DataBased-411"><a href="#DataBased-411"><span class="linenos">411</span></a>
+</span><span id="DataBased-412"><a href="#DataBased-412"><span class="linenos">412</span></a><span class="sd">        Returns True if successful, False if not.&quot;&quot;&quot;</span>
+</span><span id="DataBased-413"><a href="#DataBased-413"><span class="linenos">413</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;update </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> set </span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s2"> = ?&quot;</span>
+</span><span id="DataBased-414"><a href="#DataBased-414"><span class="linenos">414</span></a>        <span class="n">conditions</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="DataBased-415"><a href="#DataBased-415"><span class="linenos">415</span></a>        <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
+</span><span id="DataBased-416"><a href="#DataBased-416"><span class="linenos">416</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">count</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="DataBased-417"><a href="#DataBased-417"><span class="linenos">417</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
+</span><span id="DataBased-418"><a href="#DataBased-418"><span class="linenos">418</span></a>                    <span class="sa">f</span><span class="s2">&quot;Couldn&#39;t find matching records in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table to update to &#39;</span><span class="si">{</span><span class="n">new_value</span><span class="si">}</span><span class="s2">&#39;&quot;</span>
+</span><span id="DataBased-419"><a href="#DataBased-419"><span class="linenos">419</span></a>                <span class="p">)</span>
+</span><span id="DataBased-420"><a href="#DataBased-420"><span class="linenos">420</span></a>                <span class="k">return</span> <span class="kc">False</span>
+</span><span id="DataBased-421"><a href="#DataBased-421"><span class="linenos">421</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">)</span>
+</span><span id="DataBased-422"><a href="#DataBased-422"><span class="linenos">422</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="DataBased-423"><a href="#DataBased-423"><span class="linenos">423</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="DataBased-424"><a href="#DataBased-424"><span class="linenos">424</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="DataBased-425"><a href="#DataBased-425"><span class="linenos">425</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="DataBased-426"><a href="#DataBased-426"><span class="linenos">426</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="DataBased-427"><a href="#DataBased-427"><span class="linenos">427</span></a>                <span class="n">query</span><span class="p">,</span>
+</span><span id="DataBased-428"><a href="#DataBased-428"><span class="linenos">428</span></a>                <span class="p">(</span><span class="n">new_value</span><span class="p">,),</span>
+</span><span id="DataBased-429"><a href="#DataBased-429"><span class="linenos">429</span></a>            <span class="p">)</span>
+</span><span id="DataBased-430"><a href="#DataBased-430"><span class="linenos">430</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
+</span><span id="DataBased-431"><a href="#DataBased-431"><span class="linenos">431</span></a>                <span class="sa">f</span><span class="s1">&#39;Updated &quot;</span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s1">&quot; in &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table to &quot;</span><span class="si">{</span><span class="n">new_value</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&#39;</span>
+</span><span id="DataBased-432"><a href="#DataBased-432"><span class="linenos">432</span></a>            <span class="p">)</span>
+</span><span id="DataBased-433"><a href="#DataBased-433"><span class="linenos">433</span></a>            <span class="k">return</span> <span class="kc">True</span>
+</span><span id="DataBased-434"><a href="#DataBased-434"><span class="linenos">434</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DataBased-435"><a href="#DataBased-435"><span class="linenos">435</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span>
+</span><span id="DataBased-436"><a href="#DataBased-436"><span class="linenos">436</span></a>                <span class="sa">f</span><span class="s1">&#39;Failed to update &quot;</span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s1">&quot; in &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table to &quot;</span><span class="si">{</span><span class="n">new_value</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&quot;</span><span class="se">\n</span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s1">&#39;</span>
 </span><span id="DataBased-437"><a href="#DataBased-437"><span class="linenos">437</span></a>            <span class="p">)</span>
-</span><span id="DataBased-438"><a href="#DataBased-438"><span class="linenos">438</span></a>            <span class="k">return</span> <span class="kc">True</span>
-</span><span id="DataBased-439"><a href="#DataBased-439"><span class="linenos">439</span></a>        <span class="k">except</span> <span class="ne">UnboundLocalError</span><span class="p">:</span>
-</span><span id="DataBased-440"><a href="#DataBased-440"><span class="linenos">440</span></a>            <span class="n">table_filter_string</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
-</span><span id="DataBased-441"><a href="#DataBased-441"><span class="linenos">441</span></a>                <span class="n">table_filter</span> <span class="k">for</span> <span class="n">table_filter</span> <span class="ow">in</span> <span class="n">match_criteria</span>
-</span><span id="DataBased-442"><a href="#DataBased-442"><span class="linenos">442</span></a>            <span class="p">)</span>
-</span><span id="DataBased-443"><a href="#DataBased-443"><span class="linenos">443</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span>
-</span><span id="DataBased-444"><a href="#DataBased-444"><span class="linenos">444</span></a>                <span class="sa">f</span><span class="s2">&quot;No records found matching filters: </span><span class="si">{</span><span class="n">table_filter_string</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="DataBased-445"><a href="#DataBased-445"><span class="linenos">445</span></a>            <span class="p">)</span>
-</span><span id="DataBased-446"><a href="#DataBased-446"><span class="linenos">446</span></a>            <span class="k">return</span> <span class="kc">False</span>
-</span><span id="DataBased-447"><a href="#DataBased-447"><span class="linenos">447</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="DataBased-448"><a href="#DataBased-448"><span class="linenos">448</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span>
-</span><span id="DataBased-449"><a href="#DataBased-449"><span class="linenos">449</span></a>                <span class="sa">f</span><span class="s1">&#39;Failed to update &quot;</span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s1">&quot; in &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table to &quot;</span><span class="si">{</span><span class="n">new_value</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&quot;</span><span class="se">\n</span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s1">&#39;</span>
-</span><span id="DataBased-450"><a href="#DataBased-450"><span class="linenos">450</span></a>            <span class="p">)</span>
-</span><span id="DataBased-451"><a href="#DataBased-451"><span class="linenos">451</span></a>            <span class="k">return</span> <span class="kc">False</span>
-</span><span id="DataBased-452"><a href="#DataBased-452"><span class="linenos">452</span></a>
-</span><span id="DataBased-453"><a href="#DataBased-453"><span class="linenos">453</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased-454"><a href="#DataBased-454"><span class="linenos">454</span></a>    <span class="k">def</span> <span class="nf">drop_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="DataBased-455"><a href="#DataBased-455"><span class="linenos">455</span></a>        <span class="sd">&quot;&quot;&quot;Drop a table from the database.</span>
-</span><span id="DataBased-456"><a href="#DataBased-456"><span class="linenos">456</span></a>
-</span><span id="DataBased-457"><a href="#DataBased-457"><span class="linenos">457</span></a><span class="sd">        Returns True if successful, False if not.&quot;&quot;&quot;</span>
-</span><span id="DataBased-458"><a href="#DataBased-458"><span class="linenos">458</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="DataBased-459"><a href="#DataBased-459"><span class="linenos">459</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;drop Table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DataBased-460"><a href="#DataBased-460"><span class="linenos">460</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Dropped table &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
-</span><span id="DataBased-461"><a href="#DataBased-461"><span class="linenos">461</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="DataBased-462"><a href="#DataBased-462"><span class="linenos">462</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
-</span><span id="DataBased-463"><a href="#DataBased-463"><span class="linenos">463</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Failed to drop table &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
-</span><span id="DataBased-464"><a href="#DataBased-464"><span class="linenos">464</span></a>
-</span><span id="DataBased-465"><a href="#DataBased-465"><span class="linenos">465</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased-466"><a href="#DataBased-466"><span class="linenos">466</span></a>    <span class="k">def</span> <span class="nf">add_column</span><span class="p">(</span>
-</span><span id="DataBased-467"><a href="#DataBased-467"><span class="linenos">467</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">column</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">_type</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">default_value</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="DataBased-468"><a href="#DataBased-468"><span class="linenos">468</span></a>    <span class="p">):</span>
-</span><span id="DataBased-469"><a href="#DataBased-469"><span class="linenos">469</span></a>        <span class="sd">&quot;&quot;&quot;Add a new column to table.</span>
-</span><span id="DataBased-470"><a href="#DataBased-470"><span class="linenos">470</span></a>
-</span><span id="DataBased-471"><a href="#DataBased-471"><span class="linenos">471</span></a><span class="sd">        :param column: Name of the column to add.</span>
-</span><span id="DataBased-472"><a href="#DataBased-472"><span class="linenos">472</span></a>
-</span><span id="DataBased-473"><a href="#DataBased-473"><span class="linenos">473</span></a><span class="sd">        :param _type: The data type of the new column.</span>
-</span><span id="DataBased-474"><a href="#DataBased-474"><span class="linenos">474</span></a>
-</span><span id="DataBased-475"><a href="#DataBased-475"><span class="linenos">475</span></a><span class="sd">        :param default_value: Optional default value for the column.&quot;&quot;&quot;</span>
-</span><span id="DataBased-476"><a href="#DataBased-476"><span class="linenos">476</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="DataBased-477"><a href="#DataBased-477"><span class="linenos">477</span></a>            <span class="k">if</span> <span class="n">default_value</span><span class="p">:</span>
-</span><span id="DataBased-478"><a href="#DataBased-478"><span class="linenos">478</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="DataBased-479"><a href="#DataBased-479"><span class="linenos">479</span></a>                    <span class="sa">f</span><span class="s2">&quot;alter table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> add column </span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">_type</span><span class="si">}</span><span class="s2"> default </span><span class="si">{</span><span class="n">default_value</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="DataBased-480"><a href="#DataBased-480"><span class="linenos">480</span></a>                <span class="p">)</span>
-</span><span id="DataBased-481"><a href="#DataBased-481"><span class="linenos">481</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="DataBased-482"><a href="#DataBased-482"><span class="linenos">482</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;alter table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> add column </span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">_type</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DataBased-483"><a href="#DataBased-483"><span class="linenos">483</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Added column &quot;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1">&quot; to &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table.&#39;</span><span class="p">)</span>
-</span><span id="DataBased-484"><a href="#DataBased-484"><span class="linenos">484</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="DataBased-485"><a href="#DataBased-485"><span class="linenos">485</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Failed to add column &quot;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1">&quot; to &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table.&#39;</span><span class="p">)</span>
+</span><span id="DataBased-438"><a href="#DataBased-438"><span class="linenos">438</span></a>            <span class="k">return</span> <span class="kc">False</span>
+</span><span id="DataBased-439"><a href="#DataBased-439"><span class="linenos">439</span></a>
+</span><span id="DataBased-440"><a href="#DataBased-440"><span class="linenos">440</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased-441"><a href="#DataBased-441"><span class="linenos">441</span></a>    <span class="k">def</span> <span class="nf">drop_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="DataBased-442"><a href="#DataBased-442"><span class="linenos">442</span></a>        <span class="sd">&quot;&quot;&quot;Drop a table from the database.</span>
+</span><span id="DataBased-443"><a href="#DataBased-443"><span class="linenos">443</span></a>
+</span><span id="DataBased-444"><a href="#DataBased-444"><span class="linenos">444</span></a><span class="sd">        Returns True if successful, False if not.&quot;&quot;&quot;</span>
+</span><span id="DataBased-445"><a href="#DataBased-445"><span class="linenos">445</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="DataBased-446"><a href="#DataBased-446"><span class="linenos">446</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;drop Table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DataBased-447"><a href="#DataBased-447"><span class="linenos">447</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Dropped table &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
+</span><span id="DataBased-448"><a href="#DataBased-448"><span class="linenos">448</span></a>            <span class="k">return</span> <span class="kc">True</span>
+</span><span id="DataBased-449"><a href="#DataBased-449"><span class="linenos">449</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DataBased-450"><a href="#DataBased-450"><span class="linenos">450</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
+</span><span id="DataBased-451"><a href="#DataBased-451"><span class="linenos">451</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Failed to drop table &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
+</span><span id="DataBased-452"><a href="#DataBased-452"><span class="linenos">452</span></a>            <span class="k">return</span> <span class="kc">False</span>
+</span><span id="DataBased-453"><a href="#DataBased-453"><span class="linenos">453</span></a>
+</span><span id="DataBased-454"><a href="#DataBased-454"><span class="linenos">454</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased-455"><a href="#DataBased-455"><span class="linenos">455</span></a>    <span class="k">def</span> <span class="nf">add_column</span><span class="p">(</span>
+</span><span id="DataBased-456"><a href="#DataBased-456"><span class="linenos">456</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">column</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">_type</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">default_value</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="DataBased-457"><a href="#DataBased-457"><span class="linenos">457</span></a>    <span class="p">):</span>
+</span><span id="DataBased-458"><a href="#DataBased-458"><span class="linenos">458</span></a>        <span class="sd">&quot;&quot;&quot;Add a new column to table.</span>
+</span><span id="DataBased-459"><a href="#DataBased-459"><span class="linenos">459</span></a>
+</span><span id="DataBased-460"><a href="#DataBased-460"><span class="linenos">460</span></a><span class="sd">        :param column: Name of the column to add.</span>
+</span><span id="DataBased-461"><a href="#DataBased-461"><span class="linenos">461</span></a>
+</span><span id="DataBased-462"><a href="#DataBased-462"><span class="linenos">462</span></a><span class="sd">        :param _type: The data type of the new column.</span>
+</span><span id="DataBased-463"><a href="#DataBased-463"><span class="linenos">463</span></a>
+</span><span id="DataBased-464"><a href="#DataBased-464"><span class="linenos">464</span></a><span class="sd">        :param default_value: Optional default value for the column.&quot;&quot;&quot;</span>
+</span><span id="DataBased-465"><a href="#DataBased-465"><span class="linenos">465</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="DataBased-466"><a href="#DataBased-466"><span class="linenos">466</span></a>            <span class="k">if</span> <span class="n">default_value</span><span class="p">:</span>
+</span><span id="DataBased-467"><a href="#DataBased-467"><span class="linenos">467</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="DataBased-468"><a href="#DataBased-468"><span class="linenos">468</span></a>                    <span class="sa">f</span><span class="s2">&quot;alter table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> add column </span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">_type</span><span class="si">}</span><span class="s2"> default </span><span class="si">{</span><span class="n">default_value</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="DataBased-469"><a href="#DataBased-469"><span class="linenos">469</span></a>                <span class="p">)</span>
+</span><span id="DataBased-470"><a href="#DataBased-470"><span class="linenos">470</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="DataBased-471"><a href="#DataBased-471"><span class="linenos">471</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;alter table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> add column </span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">_type</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DataBased-472"><a href="#DataBased-472"><span class="linenos">472</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Added column &quot;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1">&quot; to &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table.&#39;</span><span class="p">)</span>
+</span><span id="DataBased-473"><a href="#DataBased-473"><span class="linenos">473</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DataBased-474"><a href="#DataBased-474"><span class="linenos">474</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Failed to add column &quot;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1">&quot; to &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table.&#39;</span><span class="p">)</span>
+</span><span id="DataBased-475"><a href="#DataBased-475"><span class="linenos">475</span></a>
+</span><span id="DataBased-476"><a href="#DataBased-476"><span class="linenos">476</span></a>    <span class="nd">@staticmethod</span>
+</span><span id="DataBased-477"><a href="#DataBased-477"><span class="linenos">477</span></a>    <span class="k">def</span> <span class="nf">data_to_string</span><span class="p">(</span>
+</span><span id="DataBased-478"><a href="#DataBased-478"><span class="linenos">478</span></a>        <span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">],</span> <span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="DataBased-479"><a href="#DataBased-479"><span class="linenos">479</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="DataBased-480"><a href="#DataBased-480"><span class="linenos">480</span></a>        <span class="sd">&quot;&quot;&quot;Uses tabulate to produce pretty string output</span>
+</span><span id="DataBased-481"><a href="#DataBased-481"><span class="linenos">481</span></a><span class="sd">        from a list of dictionaries.</span>
+</span><span id="DataBased-482"><a href="#DataBased-482"><span class="linenos">482</span></a>
+</span><span id="DataBased-483"><a href="#DataBased-483"><span class="linenos">483</span></a><span class="sd">        :param data: Assumes all dictionaries in list have the same set of keys.</span>
+</span><span id="DataBased-484"><a href="#DataBased-484"><span class="linenos">484</span></a>
+</span><span id="DataBased-485"><a href="#DataBased-485"><span class="linenos">485</span></a><span class="sd">        :param sort_key: Optional dictionary key to sort data with.</span>
 </span><span id="DataBased-486"><a href="#DataBased-486"><span class="linenos">486</span></a>
-</span><span id="DataBased-487"><a href="#DataBased-487"><span class="linenos">487</span></a>    <span class="nd">@staticmethod</span>
-</span><span id="DataBased-488"><a href="#DataBased-488"><span class="linenos">488</span></a>    <span class="k">def</span> <span class="nf">data_to_string</span><span class="p">(</span>
-</span><span id="DataBased-489"><a href="#DataBased-489"><span class="linenos">489</span></a>        <span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">],</span> <span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="DataBased-490"><a href="#DataBased-490"><span class="linenos">490</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="DataBased-491"><a href="#DataBased-491"><span class="linenos">491</span></a>        <span class="sd">&quot;&quot;&quot;Uses tabulate to produce pretty string output</span>
-</span><span id="DataBased-492"><a href="#DataBased-492"><span class="linenos">492</span></a><span class="sd">        from a list of dictionaries.</span>
-</span><span id="DataBased-493"><a href="#DataBased-493"><span class="linenos">493</span></a>
-</span><span id="DataBased-494"><a href="#DataBased-494"><span class="linenos">494</span></a><span class="sd">        :param data: Assumes all dictionaries in list have the same set of keys.</span>
-</span><span id="DataBased-495"><a href="#DataBased-495"><span class="linenos">495</span></a>
-</span><span id="DataBased-496"><a href="#DataBased-496"><span class="linenos">496</span></a><span class="sd">        :param sort_key: Optional dictionary key to sort data with.</span>
-</span><span id="DataBased-497"><a href="#DataBased-497"><span class="linenos">497</span></a>
-</span><span id="DataBased-498"><a href="#DataBased-498"><span class="linenos">498</span></a><span class="sd">        :param wrap_to_terminal: If True, the table width will be wrapped</span>
-</span><span id="DataBased-499"><a href="#DataBased-499"><span class="linenos">499</span></a><span class="sd">        to fit within the current terminal window. Set to False</span>
-</span><span id="DataBased-500"><a href="#DataBased-500"><span class="linenos">500</span></a><span class="sd">        if the output is going into something like a txt file.&quot;&quot;&quot;</span>
-</span><span id="DataBased-501"><a href="#DataBased-501"><span class="linenos">501</span></a>        <span class="k">return</span> <span class="n">data_to_string</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">sort_key</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">)</span>
+</span><span id="DataBased-487"><a href="#DataBased-487"><span class="linenos">487</span></a><span class="sd">        :param wrap_to_terminal: If True, the table width will be wrapped</span>
+</span><span id="DataBased-488"><a href="#DataBased-488"><span class="linenos">488</span></a><span class="sd">        to fit within the current terminal window. Set to False</span>
+</span><span id="DataBased-489"><a href="#DataBased-489"><span class="linenos">489</span></a><span class="sd">        if the output is going into something like a txt file.&quot;&quot;&quot;</span>
+</span><span id="DataBased-490"><a href="#DataBased-490"><span class="linenos">490</span></a>        <span class="k">return</span> <span class="n">data_to_string</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">sort_key</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Sqli wrapper so queries don't need to be written except table definitions.</p>
 
 <p>Supports saving and reading dates as datetime objects.</p>
 
@@ -1181,42 +1156,41 @@
 </div>
 
 
                             <div id="DataBased.__init__" class="classattr">
                                         <input id="DataBased.__init__-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
-        <span class="name">DataBased</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="n">dbpath</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span>,</span><span class="param">	<span class="n">logger_encoding</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;utf-8&#39;</span>,</span><span class="param">	<span class="n">logger_message_format</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;</span><span class="si">{levelname}</span><span class="s1">|-|</span><span class="si">{asctime}</span><span class="s1">|-|</span><span class="si">{message}</span><span class="s1">&#39;</span></span>)</span>
+        <span class="name">DataBased</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="n">dbpath</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span>,</span><span class="param">	<span class="n">logger_encoding</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;utf-8&#39;</span>,</span><span class="param">	<span class="n">logger_message_format</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;</span><span class="si">{levelname}</span><span class="s1">|-|</span><span class="si">{asctime}</span><span class="s1">|-|</span><span class="si">{message}</span><span class="s1">&#39;</span></span>)</span>
 
                 <label class="view-source-button" for="DataBased.__init__-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.__init__"></a>
             <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.__init__-34"><a href="#DataBased.__init__-34"><span class="linenos">34</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
 </span><span id="DataBased.__init__-35"><a href="#DataBased.__init__-35"><span class="linenos">35</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="DataBased.__init__-36"><a href="#DataBased.__init__-36"><span class="linenos">36</span></a>        <span class="n">dbpath</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="n">Path</span><span class="p">,</span>
+</span><span id="DataBased.__init__-36"><a href="#DataBased.__init__-36"><span class="linenos">36</span></a>        <span class="n">dbpath</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="n">Pathier</span><span class="p">,</span>
 </span><span id="DataBased.__init__-37"><a href="#DataBased.__init__-37"><span class="linenos">37</span></a>        <span class="n">logger_encoding</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;utf-8&quot;</span><span class="p">,</span>
 </span><span id="DataBased.__init__-38"><a href="#DataBased.__init__-38"><span class="linenos">38</span></a>        <span class="n">logger_message_format</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="si">{levelname}</span><span class="s2">|-|</span><span class="si">{asctime}</span><span class="s2">|-|</span><span class="si">{message}</span><span class="s2">&quot;</span><span class="p">,</span>
 </span><span id="DataBased.__init__-39"><a href="#DataBased.__init__-39"><span class="linenos">39</span></a>    <span class="p">):</span>
 </span><span id="DataBased.__init__-40"><a href="#DataBased.__init__-40"><span class="linenos">40</span></a>        <span class="sd">&quot;&quot;&quot;</span>
 </span><span id="DataBased.__init__-41"><a href="#DataBased.__init__-41"><span class="linenos">41</span></a><span class="sd">        :param dbpath: String or Path object to database file.</span>
 </span><span id="DataBased.__init__-42"><a href="#DataBased.__init__-42"><span class="linenos">42</span></a><span class="sd">        If a relative path is given, it will be relative to the</span>
 </span><span id="DataBased.__init__-43"><a href="#DataBased.__init__-43"><span class="linenos">43</span></a><span class="sd">        current working directory. The log file will be saved to the</span>
 </span><span id="DataBased.__init__-44"><a href="#DataBased.__init__-44"><span class="linenos">44</span></a><span class="sd">        same directory.</span>
 </span><span id="DataBased.__init__-45"><a href="#DataBased.__init__-45"><span class="linenos">45</span></a>
 </span><span id="DataBased.__init__-46"><a href="#DataBased.__init__-46"><span class="linenos">46</span></a><span class="sd">        :param logger_message_format: &#39;{&#39; style format string</span>
 </span><span id="DataBased.__init__-47"><a href="#DataBased.__init__-47"><span class="linenos">47</span></a><span class="sd">        for the logger object.&quot;&quot;&quot;</span>
-</span><span id="DataBased.__init__-48"><a href="#DataBased.__init__-48"><span class="linenos">48</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Path</span><span class="p">(</span><span class="n">dbpath</span><span class="p">)</span>
-</span><span id="DataBased.__init__-49"><a href="#DataBased.__init__-49"><span class="linenos">49</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">dbname</span> <span class="o">=</span> <span class="n">Path</span><span class="p">(</span><span class="n">dbpath</span><span class="p">)</span><span class="o">.</span><span class="n">name</span>
+</span><span id="DataBased.__init__-48"><a href="#DataBased.__init__-48"><span class="linenos">48</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">dbpath</span><span class="p">)</span>
+</span><span id="DataBased.__init__-49"><a href="#DataBased.__init__-49"><span class="linenos">49</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">dbname</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">dbpath</span><span class="p">)</span><span class="o">.</span><span class="n">name</span>
 </span><span id="DataBased.__init__-50"><a href="#DataBased.__init__-50"><span class="linenos">50</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
 </span><span id="DataBased.__init__-51"><a href="#DataBased.__init__-51"><span class="linenos">51</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_logger_init</span><span class="p">(</span>
 </span><span id="DataBased.__init__-52"><a href="#DataBased.__init__-52"><span class="linenos">52</span></a>            <span class="n">encoding</span><span class="o">=</span><span class="n">logger_encoding</span><span class="p">,</span> <span class="n">message_format</span><span class="o">=</span><span class="n">logger_message_format</span>
 </span><span id="DataBased.__init__-53"><a href="#DataBased.__init__-53"><span class="linenos">53</span></a>        <span class="p">)</span>
 </span><span id="DataBased.__init__-54"><a href="#DataBased.__init__-54"><span class="linenos">54</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">connection_open</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="DataBased.__init__-55"><a href="#DataBased.__init__-55"><span class="linenos">55</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">create_manager</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><h6 id="parameters">Parameters</h6>
 
 <ul>
 <li><p><strong>dbpath</strong>:  String or Path object to database file.
@@ -1226,62 +1200,35 @@
 <li><p><strong>logger_message_format</strong>:  '{' style format string
 for the logger object.</p></li>
 </ul>
 </div>
 
 
                             </div>
-                            <div id="DataBased.create_manager" class="classattr">
-                                        <input id="DataBased.create_manager-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
-<div class="attr function">
-            
-        <span class="def">def</span>
-        <span class="name">create_manager</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">):</span></span>
-
-                <label class="view-source-button" for="DataBased.create_manager-view-source"><span>View Source</span></label>
-
-    </div>
-    <a class="headerlink" href="#DataBased.create_manager"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.create_manager-64"><a href="#DataBased.create_manager-64"><span class="linenos">64</span></a>    <span class="k">def</span> <span class="nf">create_manager</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="DataBased.create_manager-65"><a href="#DataBased.create_manager-65"><span class="linenos">65</span></a>        <span class="sd">&quot;&quot;&quot;Create dbmanager.py in the same directory</span>
-</span><span id="DataBased.create_manager-66"><a href="#DataBased.create_manager-66"><span class="linenos">66</span></a><span class="sd">        as the database file if it doesn&#39;t exist.&quot;&quot;&quot;</span>
-</span><span id="DataBased.create_manager-67"><a href="#DataBased.create_manager-67"><span class="linenos">67</span></a>        <span class="n">manager_path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">parent</span> <span class="o">/</span> <span class="s2">&quot;dbmanager.py&quot;</span>
-</span><span id="DataBased.create_manager-68"><a href="#DataBased.create_manager-68"><span class="linenos">68</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">manager_path</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="DataBased.create_manager-69"><a href="#DataBased.create_manager-69"><span class="linenos">69</span></a>            <span class="n">manager_template</span> <span class="o">=</span> <span class="p">(</span><span class="n">Path</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span><span class="o">.</span><span class="n">parent</span> <span class="o">/</span> <span class="s2">&quot;dbmanager.py&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
-</span><span id="DataBased.create_manager-70"><a href="#DataBased.create_manager-70"><span class="linenos">70</span></a>            <span class="n">manager_path</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">manager_template</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;$dbname&quot;</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbname</span><span class="p">))</span>
-</span></pre></div>
-
-
-            <div class="docstring"><p>Create dbmanager.py in the same directory
-as the database file if it doesn't exist.</p>
-</div>
-
-
-                            </div>
                             <div id="DataBased.open" class="classattr">
                                         <input id="DataBased.open-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
         <span class="name">open</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DataBased.open-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.open"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.open-72"><a href="#DataBased.open-72"><span class="linenos">72</span></a>    <span class="k">def</span> <span class="nf">open</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="DataBased.open-73"><a href="#DataBased.open-73"><span class="linenos">73</span></a>        <span class="sd">&quot;&quot;&quot;Open connection to db.&quot;&quot;&quot;</span>
-</span><span id="DataBased.open-74"><a href="#DataBased.open-74"><span class="linenos">74</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">connection</span> <span class="o">=</span> <span class="n">sqlite3</span><span class="o">.</span><span class="n">connect</span><span class="p">(</span>
-</span><span id="DataBased.open-75"><a href="#DataBased.open-75"><span class="linenos">75</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">,</span>
-</span><span id="DataBased.open-76"><a href="#DataBased.open-76"><span class="linenos">76</span></a>            <span class="n">detect_types</span><span class="o">=</span><span class="n">sqlite3</span><span class="o">.</span><span class="n">PARSE_DECLTYPES</span> <span class="o">|</span> <span class="n">sqlite3</span><span class="o">.</span><span class="n">PARSE_COLNAMES</span><span class="p">,</span>
-</span><span id="DataBased.open-77"><a href="#DataBased.open-77"><span class="linenos">77</span></a>            <span class="n">timeout</span><span class="o">=</span><span class="mi">10</span><span class="p">,</span>
-</span><span id="DataBased.open-78"><a href="#DataBased.open-78"><span class="linenos">78</span></a>        <span class="p">)</span>
-</span><span id="DataBased.open-79"><a href="#DataBased.open-79"><span class="linenos">79</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">connection</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="s2">&quot;pragma foreign_keys = 1&quot;</span><span class="p">)</span>
-</span><span id="DataBased.open-80"><a href="#DataBased.open-80"><span class="linenos">80</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">connection</span><span class="o">.</span><span class="n">cursor</span><span class="p">()</span>
-</span><span id="DataBased.open-81"><a href="#DataBased.open-81"><span class="linenos">81</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">connection_open</span> <span class="o">=</span> <span class="kc">True</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.open-63"><a href="#DataBased.open-63"><span class="linenos">63</span></a>    <span class="k">def</span> <span class="nf">open</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="DataBased.open-64"><a href="#DataBased.open-64"><span class="linenos">64</span></a>        <span class="sd">&quot;&quot;&quot;Open connection to db.&quot;&quot;&quot;</span>
+</span><span id="DataBased.open-65"><a href="#DataBased.open-65"><span class="linenos">65</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">connection</span> <span class="o">=</span> <span class="n">sqlite3</span><span class="o">.</span><span class="n">connect</span><span class="p">(</span>
+</span><span id="DataBased.open-66"><a href="#DataBased.open-66"><span class="linenos">66</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">,</span>
+</span><span id="DataBased.open-67"><a href="#DataBased.open-67"><span class="linenos">67</span></a>            <span class="n">detect_types</span><span class="o">=</span><span class="n">sqlite3</span><span class="o">.</span><span class="n">PARSE_DECLTYPES</span> <span class="o">|</span> <span class="n">sqlite3</span><span class="o">.</span><span class="n">PARSE_COLNAMES</span><span class="p">,</span>
+</span><span id="DataBased.open-68"><a href="#DataBased.open-68"><span class="linenos">68</span></a>            <span class="n">timeout</span><span class="o">=</span><span class="mi">10</span><span class="p">,</span>
+</span><span id="DataBased.open-69"><a href="#DataBased.open-69"><span class="linenos">69</span></a>        <span class="p">)</span>
+</span><span id="DataBased.open-70"><a href="#DataBased.open-70"><span class="linenos">70</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">connection</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="s2">&quot;pragma foreign_keys = 1&quot;</span><span class="p">)</span>
+</span><span id="DataBased.open-71"><a href="#DataBased.open-71"><span class="linenos">71</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">connection</span><span class="o">.</span><span class="n">cursor</span><span class="p">()</span>
+</span><span id="DataBased.open-72"><a href="#DataBased.open-72"><span class="linenos">72</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">connection_open</span> <span class="o">=</span> <span class="kc">True</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Open connection to db.</p>
 </div>
 
 
@@ -1293,23 +1240,23 @@
         <span class="def">def</span>
         <span class="name">close</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DataBased.close-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.close"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.close-83"><a href="#DataBased.close-83"><span class="linenos">83</span></a>    <span class="k">def</span> <span class="nf">close</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="DataBased.close-84"><a href="#DataBased.close-84"><span class="linenos">84</span></a>        <span class="sd">&quot;&quot;&quot;Save and close connection to db.</span>
-</span><span id="DataBased.close-85"><a href="#DataBased.close-85"><span class="linenos">85</span></a>
-</span><span id="DataBased.close-86"><a href="#DataBased.close-86"><span class="linenos">86</span></a><span class="sd">        Call this as soon as you are done using the database if you have</span>
-</span><span id="DataBased.close-87"><a href="#DataBased.close-87"><span class="linenos">87</span></a><span class="sd">        multiple threads or processes using the same database.&quot;&quot;&quot;</span>
-</span><span id="DataBased.close-88"><a href="#DataBased.close-88"><span class="linenos">88</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">connection_open</span><span class="p">:</span>
-</span><span id="DataBased.close-89"><a href="#DataBased.close-89"><span class="linenos">89</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">connection</span><span class="o">.</span><span class="n">commit</span><span class="p">()</span>
-</span><span id="DataBased.close-90"><a href="#DataBased.close-90"><span class="linenos">90</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">connection</span><span class="o">.</span><span class="n">close</span><span class="p">()</span>
-</span><span id="DataBased.close-91"><a href="#DataBased.close-91"><span class="linenos">91</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">connection_open</span> <span class="o">=</span> <span class="kc">False</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.close-74"><a href="#DataBased.close-74"><span class="linenos">74</span></a>    <span class="k">def</span> <span class="nf">close</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="DataBased.close-75"><a href="#DataBased.close-75"><span class="linenos">75</span></a>        <span class="sd">&quot;&quot;&quot;Save and close connection to db.</span>
+</span><span id="DataBased.close-76"><a href="#DataBased.close-76"><span class="linenos">76</span></a>
+</span><span id="DataBased.close-77"><a href="#DataBased.close-77"><span class="linenos">77</span></a><span class="sd">        Call this as soon as you are done using the database if you have</span>
+</span><span id="DataBased.close-78"><a href="#DataBased.close-78"><span class="linenos">78</span></a><span class="sd">        multiple threads or processes using the same database.&quot;&quot;&quot;</span>
+</span><span id="DataBased.close-79"><a href="#DataBased.close-79"><span class="linenos">79</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">connection_open</span><span class="p">:</span>
+</span><span id="DataBased.close-80"><a href="#DataBased.close-80"><span class="linenos">80</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">connection</span><span class="o">.</span><span class="n">commit</span><span class="p">()</span>
+</span><span id="DataBased.close-81"><a href="#DataBased.close-81"><span class="linenos">81</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">connection</span><span class="o">.</span><span class="n">close</span><span class="p">()</span>
+</span><span id="DataBased.close-82"><a href="#DataBased.close-82"><span class="linenos">82</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">connection_open</span> <span class="o">=</span> <span class="kc">False</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Save and close connection to db.</p>
 
 <p>Call this as soon as you are done using the database if you have
 multiple threads or processes using the same database.</p>
@@ -1324,20 +1271,20 @@
         <span class="def">def</span>
         <span class="name">query</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">query_</span></span><span class="return-annotation">) -> <span class="nb">list</span><span class="p">[</span><span class="n">typing</span><span class="o">.</span><span class="n">Any</span><span class="p">]</span>:</span></span>
 
                 <label class="view-source-button" for="DataBased.query-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.query"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.query-160"><a href="#DataBased.query-160"><span class="linenos">160</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased.query-161"><a href="#DataBased.query-161"><span class="linenos">161</span></a>    <span class="k">def</span> <span class="nf">query</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">query_</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]:</span>
-</span><span id="DataBased.query-162"><a href="#DataBased.query-162"><span class="linenos">162</span></a>        <span class="sd">&quot;&quot;&quot;Execute an arbitrary query and</span>
-</span><span id="DataBased.query-163"><a href="#DataBased.query-163"><span class="linenos">163</span></a><span class="sd">        return the results.&quot;&quot;&quot;</span>
-</span><span id="DataBased.query-164"><a href="#DataBased.query-164"><span class="linenos">164</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query_</span><span class="p">)</span>
-</span><span id="DataBased.query-165"><a href="#DataBased.query-165"><span class="linenos">165</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.query-151"><a href="#DataBased.query-151"><span class="linenos">151</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased.query-152"><a href="#DataBased.query-152"><span class="linenos">152</span></a>    <span class="k">def</span> <span class="nf">query</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">query_</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]:</span>
+</span><span id="DataBased.query-153"><a href="#DataBased.query-153"><span class="linenos">153</span></a>        <span class="sd">&quot;&quot;&quot;Execute an arbitrary query and</span>
+</span><span id="DataBased.query-154"><a href="#DataBased.query-154"><span class="linenos">154</span></a><span class="sd">        return the results.&quot;&quot;&quot;</span>
+</span><span id="DataBased.query-155"><a href="#DataBased.query-155"><span class="linenos">155</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query_</span><span class="p">)</span>
+</span><span id="DataBased.query-156"><a href="#DataBased.query-156"><span class="linenos">156</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Execute an arbitrary query and
 return the results.</p>
 </div>
 
@@ -1350,26 +1297,26 @@
         <span class="def">def</span>
         <span class="name">create_tables</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">table_querys</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="p">[]</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DataBased.create_tables-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.create_tables"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.create_tables-167"><a href="#DataBased.create_tables-167"><span class="linenos">167</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased.create_tables-168"><a href="#DataBased.create_tables-168"><span class="linenos">168</span></a>    <span class="k">def</span> <span class="nf">create_tables</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table_querys</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="p">[]):</span>
-</span><span id="DataBased.create_tables-169"><a href="#DataBased.create_tables-169"><span class="linenos">169</span></a>        <span class="sd">&quot;&quot;&quot;Create tables if they don&#39;t exist.</span>
-</span><span id="DataBased.create_tables-170"><a href="#DataBased.create_tables-170"><span class="linenos">170</span></a>
-</span><span id="DataBased.create_tables-171"><a href="#DataBased.create_tables-171"><span class="linenos">171</span></a><span class="sd">        :param table_querys: Each query should be</span>
-</span><span id="DataBased.create_tables-172"><a href="#DataBased.create_tables-172"><span class="linenos">172</span></a><span class="sd">        in the form &#39;tableName(columnDefinitions)&#39;&quot;&quot;&quot;</span>
-</span><span id="DataBased.create_tables-173"><a href="#DataBased.create_tables-173"><span class="linenos">173</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">table_querys</span><span class="p">)</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="DataBased.create_tables-174"><a href="#DataBased.create_tables-174"><span class="linenos">174</span></a>            <span class="n">table_names</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
-</span><span id="DataBased.create_tables-175"><a href="#DataBased.create_tables-175"><span class="linenos">175</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">table_querys</span><span class="p">:</span>
-</span><span id="DataBased.create_tables-176"><a href="#DataBased.create_tables-176"><span class="linenos">176</span></a>                <span class="k">if</span> <span class="n">table</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;(&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">table_names</span><span class="p">:</span>
-</span><span id="DataBased.create_tables-177"><a href="#DataBased.create_tables-177"><span class="linenos">177</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;create table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DataBased.create_tables-178"><a href="#DataBased.create_tables-178"><span class="linenos">178</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;</span><span class="si">{</span><span class="n">table</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;(&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s1"> table created.&#39;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.create_tables-158"><a href="#DataBased.create_tables-158"><span class="linenos">158</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased.create_tables-159"><a href="#DataBased.create_tables-159"><span class="linenos">159</span></a>    <span class="k">def</span> <span class="nf">create_tables</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table_querys</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="p">[]):</span>
+</span><span id="DataBased.create_tables-160"><a href="#DataBased.create_tables-160"><span class="linenos">160</span></a>        <span class="sd">&quot;&quot;&quot;Create tables if they don&#39;t exist.</span>
+</span><span id="DataBased.create_tables-161"><a href="#DataBased.create_tables-161"><span class="linenos">161</span></a>
+</span><span id="DataBased.create_tables-162"><a href="#DataBased.create_tables-162"><span class="linenos">162</span></a><span class="sd">        :param table_querys: Each query should be</span>
+</span><span id="DataBased.create_tables-163"><a href="#DataBased.create_tables-163"><span class="linenos">163</span></a><span class="sd">        in the form &#39;tableName(columnDefinitions)&#39;&quot;&quot;&quot;</span>
+</span><span id="DataBased.create_tables-164"><a href="#DataBased.create_tables-164"><span class="linenos">164</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">table_querys</span><span class="p">)</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="DataBased.create_tables-165"><a href="#DataBased.create_tables-165"><span class="linenos">165</span></a>            <span class="n">table_names</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
+</span><span id="DataBased.create_tables-166"><a href="#DataBased.create_tables-166"><span class="linenos">166</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">table_querys</span><span class="p">:</span>
+</span><span id="DataBased.create_tables-167"><a href="#DataBased.create_tables-167"><span class="linenos">167</span></a>                <span class="k">if</span> <span class="n">table</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;(&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">table_names</span><span class="p">:</span>
+</span><span id="DataBased.create_tables-168"><a href="#DataBased.create_tables-168"><span class="linenos">168</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;create table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DataBased.create_tables-169"><a href="#DataBased.create_tables-169"><span class="linenos">169</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;</span><span class="si">{</span><span class="n">table</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;(&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s1"> table created.&#39;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Create tables if they don't exist.</p>
 
 <h6 id="parameters">Parameters</h6>
 
@@ -1388,27 +1335,27 @@
         <span class="def">def</span>
         <span class="name">create_table</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">table</span><span class="p">:</span> <span class="nb">str</span>, </span><span class="param"><span class="n">column_defs</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DataBased.create_table-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.create_table"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.create_table-180"><a href="#DataBased.create_table-180"><span class="linenos">180</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased.create_table-181"><a href="#DataBased.create_table-181"><span class="linenos">181</span></a>    <span class="k">def</span> <span class="nf">create_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">column_defs</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]):</span>
-</span><span id="DataBased.create_table-182"><a href="#DataBased.create_table-182"><span class="linenos">182</span></a>        <span class="sd">&quot;&quot;&quot;Create a table if it doesn&#39;t exist.</span>
-</span><span id="DataBased.create_table-183"><a href="#DataBased.create_table-183"><span class="linenos">183</span></a>
-</span><span id="DataBased.create_table-184"><a href="#DataBased.create_table-184"><span class="linenos">184</span></a><span class="sd">        :param table: Name of the table to create.</span>
-</span><span id="DataBased.create_table-185"><a href="#DataBased.create_table-185"><span class="linenos">185</span></a>
-</span><span id="DataBased.create_table-186"><a href="#DataBased.create_table-186"><span class="linenos">186</span></a><span class="sd">        :param column_defs: List of column definitions in</span>
-</span><span id="DataBased.create_table-187"><a href="#DataBased.create_table-187"><span class="linenos">187</span></a><span class="sd">        proper Sqlite3 sytax.</span>
-</span><span id="DataBased.create_table-188"><a href="#DataBased.create_table-188"><span class="linenos">188</span></a><span class="sd">        i.e. &quot;columnName text unique&quot; or &quot;columnName int primary key&quot; etc.&quot;&quot;&quot;</span>
-</span><span id="DataBased.create_table-189"><a href="#DataBased.create_table-189"><span class="linenos">189</span></a>        <span class="k">if</span> <span class="n">table</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">():</span>
-</span><span id="DataBased.create_table-190"><a href="#DataBased.create_table-190"><span class="linenos">190</span></a>            <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;create table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">(</span><span class="si">{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">column_defs</span><span class="p">)</span><span class="si">}</span><span class="s2">)&quot;</span>
-</span><span id="DataBased.create_table-191"><a href="#DataBased.create_table-191"><span class="linenos">191</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
-</span><span id="DataBased.create_table-192"><a href="#DataBased.create_table-192"><span class="linenos">192</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;&#39;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&#39; table created.&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.create_table-171"><a href="#DataBased.create_table-171"><span class="linenos">171</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased.create_table-172"><a href="#DataBased.create_table-172"><span class="linenos">172</span></a>    <span class="k">def</span> <span class="nf">create_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">column_defs</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]):</span>
+</span><span id="DataBased.create_table-173"><a href="#DataBased.create_table-173"><span class="linenos">173</span></a>        <span class="sd">&quot;&quot;&quot;Create a table if it doesn&#39;t exist.</span>
+</span><span id="DataBased.create_table-174"><a href="#DataBased.create_table-174"><span class="linenos">174</span></a>
+</span><span id="DataBased.create_table-175"><a href="#DataBased.create_table-175"><span class="linenos">175</span></a><span class="sd">        :param table: Name of the table to create.</span>
+</span><span id="DataBased.create_table-176"><a href="#DataBased.create_table-176"><span class="linenos">176</span></a>
+</span><span id="DataBased.create_table-177"><a href="#DataBased.create_table-177"><span class="linenos">177</span></a><span class="sd">        :param column_defs: List of column definitions in</span>
+</span><span id="DataBased.create_table-178"><a href="#DataBased.create_table-178"><span class="linenos">178</span></a><span class="sd">        proper Sqlite3 sytax.</span>
+</span><span id="DataBased.create_table-179"><a href="#DataBased.create_table-179"><span class="linenos">179</span></a><span class="sd">        i.e. &quot;columnName text unique&quot; or &quot;columnName int primary key&quot; etc.&quot;&quot;&quot;</span>
+</span><span id="DataBased.create_table-180"><a href="#DataBased.create_table-180"><span class="linenos">180</span></a>        <span class="k">if</span> <span class="n">table</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">():</span>
+</span><span id="DataBased.create_table-181"><a href="#DataBased.create_table-181"><span class="linenos">181</span></a>            <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;create table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">(</span><span class="si">{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">column_defs</span><span class="p">)</span><span class="si">}</span><span class="s2">)&quot;</span>
+</span><span id="DataBased.create_table-182"><a href="#DataBased.create_table-182"><span class="linenos">182</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
+</span><span id="DataBased.create_table-183"><a href="#DataBased.create_table-183"><span class="linenos">183</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;&#39;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&#39; table created.&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Create a table if it doesn't exist.</p>
 
 <h6 id="parameters">Parameters</h6>
 
@@ -1429,21 +1376,21 @@
         <span class="def">def</span>
         <span class="name">get_table_names</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">) -> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span>:</span></span>
 
                 <label class="view-source-button" for="DataBased.get_table_names-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.get_table_names"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.get_table_names-194"><a href="#DataBased.get_table_names-194"><span class="linenos">194</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased.get_table_names-195"><a href="#DataBased.get_table_names-195"><span class="linenos">195</span></a>    <span class="k">def</span> <span class="nf">get_table_names</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
-</span><span id="DataBased.get_table_names-196"><a href="#DataBased.get_table_names-196"><span class="linenos">196</span></a>        <span class="sd">&quot;&quot;&quot;Returns a list of table names from database.&quot;&quot;&quot;</span>
-</span><span id="DataBased.get_table_names-197"><a href="#DataBased.get_table_names-197"><span class="linenos">197</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="DataBased.get_table_names-198"><a href="#DataBased.get_table_names-198"><span class="linenos">198</span></a>            <span class="s1">&#39;select name from sqlite_Schema where type = &quot;table&quot; and name not like &quot;sqlite_%&quot;&#39;</span>
-</span><span id="DataBased.get_table_names-199"><a href="#DataBased.get_table_names-199"><span class="linenos">199</span></a>        <span class="p">)</span>
-</span><span id="DataBased.get_table_names-200"><a href="#DataBased.get_table_names-200"><span class="linenos">200</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">result</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()]</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.get_table_names-185"><a href="#DataBased.get_table_names-185"><span class="linenos">185</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased.get_table_names-186"><a href="#DataBased.get_table_names-186"><span class="linenos">186</span></a>    <span class="k">def</span> <span class="nf">get_table_names</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
+</span><span id="DataBased.get_table_names-187"><a href="#DataBased.get_table_names-187"><span class="linenos">187</span></a>        <span class="sd">&quot;&quot;&quot;Returns a list of table names from database.&quot;&quot;&quot;</span>
+</span><span id="DataBased.get_table_names-188"><a href="#DataBased.get_table_names-188"><span class="linenos">188</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="DataBased.get_table_names-189"><a href="#DataBased.get_table_names-189"><span class="linenos">189</span></a>            <span class="s1">&#39;select name from sqlite_Schema where type = &quot;table&quot; and name not like &quot;sqlite_%&quot;&#39;</span>
+</span><span id="DataBased.get_table_names-190"><a href="#DataBased.get_table_names-190"><span class="linenos">190</span></a>        <span class="p">)</span>
+</span><span id="DataBased.get_table_names-191"><a href="#DataBased.get_table_names-191"><span class="linenos">191</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">result</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()]</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Returns a list of table names from database.</p>
 </div>
 
 
@@ -1455,67 +1402,67 @@
         <span class="def">def</span>
         <span class="name">get_column_names</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">table</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span>:</span></span>
 
                 <label class="view-source-button" for="DataBased.get_column_names-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.get_column_names"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.get_column_names-202"><a href="#DataBased.get_column_names-202"><span class="linenos">202</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased.get_column_names-203"><a href="#DataBased.get_column_names-203"><span class="linenos">203</span></a>    <span class="k">def</span> <span class="nf">get_column_names</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
-</span><span id="DataBased.get_column_names-204"><a href="#DataBased.get_column_names-204"><span class="linenos">204</span></a>        <span class="sd">&quot;&quot;&quot;Return a list of column names from a table.&quot;&quot;&quot;</span>
-</span><span id="DataBased.get_column_names-205"><a href="#DataBased.get_column_names-205"><span class="linenos">205</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;select * from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> where 1=0&quot;</span><span class="p">)</span>
-</span><span id="DataBased.get_column_names-206"><a href="#DataBased.get_column_names-206"><span class="linenos">206</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">description</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="k">for</span> <span class="n">description</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">description</span><span class="p">]</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.get_column_names-193"><a href="#DataBased.get_column_names-193"><span class="linenos">193</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased.get_column_names-194"><a href="#DataBased.get_column_names-194"><span class="linenos">194</span></a>    <span class="k">def</span> <span class="nf">get_column_names</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
+</span><span id="DataBased.get_column_names-195"><a href="#DataBased.get_column_names-195"><span class="linenos">195</span></a>        <span class="sd">&quot;&quot;&quot;Return a list of column names from a table.&quot;&quot;&quot;</span>
+</span><span id="DataBased.get_column_names-196"><a href="#DataBased.get_column_names-196"><span class="linenos">196</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;select * from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> where 1=0&quot;</span><span class="p">)</span>
+</span><span id="DataBased.get_column_names-197"><a href="#DataBased.get_column_names-197"><span class="linenos">197</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">description</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="k">for</span> <span class="n">description</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">description</span><span class="p">]</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Return a list of column names from a table.</p>
 </div>
 
 
                             </div>
                             <div id="DataBased.count" class="classattr">
                                         <input id="DataBased.count-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">count</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">table</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">) -> <span class="nb">int</span>:</span></span>
+        <span class="name">count</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">table</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">) -> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="DataBased.count-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.count"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.count-208"><a href="#DataBased.count-208"><span class="linenos">208</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased.count-209"><a href="#DataBased.count-209"><span class="linenos">209</span></a>    <span class="k">def</span> <span class="nf">count</span><span class="p">(</span>
-</span><span id="DataBased.count-210"><a href="#DataBased.count-210"><span class="linenos">210</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="DataBased.count-211"><a href="#DataBased.count-211"><span class="linenos">211</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
-</span><span id="DataBased.count-212"><a href="#DataBased.count-212"><span class="linenos">212</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="DataBased.count-213"><a href="#DataBased.count-213"><span class="linenos">213</span></a>        <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="DataBased.count-214"><a href="#DataBased.count-214"><span class="linenos">214</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="DataBased.count-215"><a href="#DataBased.count-215"><span class="linenos">215</span></a>        <span class="sd">&quot;&quot;&quot;Return number of items in table.</span>
-</span><span id="DataBased.count-216"><a href="#DataBased.count-216"><span class="linenos">216</span></a>
-</span><span id="DataBased.count-217"><a href="#DataBased.count-217"><span class="linenos">217</span></a><span class="sd">        :param match_criteria: Can be a list of 2-tuples where each</span>
-</span><span id="DataBased.count-218"><a href="#DataBased.count-218"><span class="linenos">218</span></a><span class="sd">        tuple is (columnName, rowValue) or a dictionary where</span>
-</span><span id="DataBased.count-219"><a href="#DataBased.count-219"><span class="linenos">219</span></a><span class="sd">        keys are column names and values are row values.</span>
-</span><span id="DataBased.count-220"><a href="#DataBased.count-220"><span class="linenos">220</span></a><span class="sd">        If None, all rows from the table will be counted.</span>
-</span><span id="DataBased.count-221"><a href="#DataBased.count-221"><span class="linenos">221</span></a>
-</span><span id="DataBased.count-222"><a href="#DataBased.count-222"><span class="linenos">222</span></a><span class="sd">        :param exact_match: If False, the row value for a give column</span>
-</span><span id="DataBased.count-223"><a href="#DataBased.count-223"><span class="linenos">223</span></a><span class="sd">        in match_criteria will be matched as a substring. Has no effect if</span>
-</span><span id="DataBased.count-224"><a href="#DataBased.count-224"><span class="linenos">224</span></a><span class="sd">        match_criteria is None.</span>
-</span><span id="DataBased.count-225"><a href="#DataBased.count-225"><span class="linenos">225</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="DataBased.count-226"><a href="#DataBased.count-226"><span class="linenos">226</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;select count(_rowid_) from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="DataBased.count-227"><a href="#DataBased.count-227"><span class="linenos">227</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="DataBased.count-228"><a href="#DataBased.count-228"><span class="linenos">228</span></a>            <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
-</span><span id="DataBased.count-229"><a href="#DataBased.count-229"><span class="linenos">229</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="DataBased.count-230"><a href="#DataBased.count-230"><span class="linenos">230</span></a>                    <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">query</span><span class="si">}</span><span class="s2"> where </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="DataBased.count-231"><a href="#DataBased.count-231"><span class="linenos">231</span></a>                <span class="p">)</span>
-</span><span id="DataBased.count-232"><a href="#DataBased.count-232"><span class="linenos">232</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="DataBased.count-233"><a href="#DataBased.count-233"><span class="linenos">233</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">query</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DataBased.count-234"><a href="#DataBased.count-234"><span class="linenos">234</span></a>            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchone</span><span class="p">()[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="DataBased.count-235"><a href="#DataBased.count-235"><span class="linenos">235</span></a>        <span class="k">except</span><span class="p">:</span>
-</span><span id="DataBased.count-236"><a href="#DataBased.count-236"><span class="linenos">236</span></a>            <span class="k">return</span> <span class="mi">0</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.count-199"><a href="#DataBased.count-199"><span class="linenos">199</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased.count-200"><a href="#DataBased.count-200"><span class="linenos">200</span></a>    <span class="k">def</span> <span class="nf">count</span><span class="p">(</span>
+</span><span id="DataBased.count-201"><a href="#DataBased.count-201"><span class="linenos">201</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="DataBased.count-202"><a href="#DataBased.count-202"><span class="linenos">202</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
+</span><span id="DataBased.count-203"><a href="#DataBased.count-203"><span class="linenos">203</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="DataBased.count-204"><a href="#DataBased.count-204"><span class="linenos">204</span></a>        <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="DataBased.count-205"><a href="#DataBased.count-205"><span class="linenos">205</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="DataBased.count-206"><a href="#DataBased.count-206"><span class="linenos">206</span></a>        <span class="sd">&quot;&quot;&quot;Return number of items in table.</span>
+</span><span id="DataBased.count-207"><a href="#DataBased.count-207"><span class="linenos">207</span></a>
+</span><span id="DataBased.count-208"><a href="#DataBased.count-208"><span class="linenos">208</span></a><span class="sd">        :param match_criteria: Can be a list of 2-tuples where each</span>
+</span><span id="DataBased.count-209"><a href="#DataBased.count-209"><span class="linenos">209</span></a><span class="sd">        tuple is (columnName, rowValue) or a dictionary where</span>
+</span><span id="DataBased.count-210"><a href="#DataBased.count-210"><span class="linenos">210</span></a><span class="sd">        keys are column names and values are row values.</span>
+</span><span id="DataBased.count-211"><a href="#DataBased.count-211"><span class="linenos">211</span></a><span class="sd">        If None, all rows from the table will be counted.</span>
+</span><span id="DataBased.count-212"><a href="#DataBased.count-212"><span class="linenos">212</span></a>
+</span><span id="DataBased.count-213"><a href="#DataBased.count-213"><span class="linenos">213</span></a><span class="sd">        :param exact_match: If False, the row value for a give column</span>
+</span><span id="DataBased.count-214"><a href="#DataBased.count-214"><span class="linenos">214</span></a><span class="sd">        in match_criteria will be matched as a substring. Has no effect if</span>
+</span><span id="DataBased.count-215"><a href="#DataBased.count-215"><span class="linenos">215</span></a><span class="sd">        match_criteria is None.</span>
+</span><span id="DataBased.count-216"><a href="#DataBased.count-216"><span class="linenos">216</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="DataBased.count-217"><a href="#DataBased.count-217"><span class="linenos">217</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;select count(_rowid_) from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="DataBased.count-218"><a href="#DataBased.count-218"><span class="linenos">218</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="DataBased.count-219"><a href="#DataBased.count-219"><span class="linenos">219</span></a>            <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
+</span><span id="DataBased.count-220"><a href="#DataBased.count-220"><span class="linenos">220</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="DataBased.count-221"><a href="#DataBased.count-221"><span class="linenos">221</span></a>                    <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">query</span><span class="si">}</span><span class="s2"> where </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="DataBased.count-222"><a href="#DataBased.count-222"><span class="linenos">222</span></a>                <span class="p">)</span>
+</span><span id="DataBased.count-223"><a href="#DataBased.count-223"><span class="linenos">223</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="DataBased.count-224"><a href="#DataBased.count-224"><span class="linenos">224</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">query</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DataBased.count-225"><a href="#DataBased.count-225"><span class="linenos">225</span></a>            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchone</span><span class="p">()[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="DataBased.count-226"><a href="#DataBased.count-226"><span class="linenos">226</span></a>        <span class="k">except</span><span class="p">:</span>
+</span><span id="DataBased.count-227"><a href="#DataBased.count-227"><span class="linenos">227</span></a>            <span class="k">return</span> <span class="mi">0</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Return number of items in table.</p>
 
 <h6 id="parameters">Parameters</h6>
 
@@ -1533,51 +1480,54 @@
 
                             </div>
                             <div id="DataBased.add_row" class="classattr">
                                         <input id="DataBased.add_row-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">add_row</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">table</span><span class="p">:</span> <span class="nb">str</span>, </span><span class="param"><span class="n">values</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="nb">any</span><span class="p">]</span>, </span><span class="param"><span class="n">columns</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">):</span></span>
+        <span class="name">add_row</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">table</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">values</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="n">typing</span><span class="o">.</span><span class="n">Any</span><span class="p">]</span>,</span><span class="param">	<span class="n">columns</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DataBased.add_row-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.add_row"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.add_row-238"><a href="#DataBased.add_row-238"><span class="linenos">238</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased.add_row-239"><a href="#DataBased.add_row-239"><span class="linenos">239</span></a>    <span class="k">def</span> <span class="nf">add_row</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="nb">any</span><span class="p">],</span> <span class="n">columns</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="DataBased.add_row-240"><a href="#DataBased.add_row-240"><span class="linenos">240</span></a>        <span class="sd">&quot;&quot;&quot;Add row of values to table.</span>
-</span><span id="DataBased.add_row-241"><a href="#DataBased.add_row-241"><span class="linenos">241</span></a>
-</span><span id="DataBased.add_row-242"><a href="#DataBased.add_row-242"><span class="linenos">242</span></a><span class="sd">        :param table: The table to insert into.</span>
-</span><span id="DataBased.add_row-243"><a href="#DataBased.add_row-243"><span class="linenos">243</span></a>
-</span><span id="DataBased.add_row-244"><a href="#DataBased.add_row-244"><span class="linenos">244</span></a><span class="sd">        :param values: A tuple of values to be inserted into the table.</span>
-</span><span id="DataBased.add_row-245"><a href="#DataBased.add_row-245"><span class="linenos">245</span></a>
-</span><span id="DataBased.add_row-246"><a href="#DataBased.add_row-246"><span class="linenos">246</span></a><span class="sd">        :param columns: If None, values param is expected to supply</span>
-</span><span id="DataBased.add_row-247"><a href="#DataBased.add_row-247"><span class="linenos">247</span></a><span class="sd">        a value for every column in the table. If columns is</span>
-</span><span id="DataBased.add_row-248"><a href="#DataBased.add_row-248"><span class="linenos">248</span></a><span class="sd">        provided, it should contain the same number of elements as values.&quot;&quot;&quot;</span>
-</span><span id="DataBased.add_row-249"><a href="#DataBased.add_row-249"><span class="linenos">249</span></a>        <span class="n">parameterizer</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="s2">&quot;?&quot;</span> <span class="k">for</span> <span class="n">_</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
-</span><span id="DataBased.add_row-250"><a href="#DataBased.add_row-250"><span class="linenos">250</span></a>        <span class="n">logger_values</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
-</span><span id="DataBased.add_row-251"><a href="#DataBased.add_row-251"><span class="linenos">251</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="DataBased.add_row-252"><a href="#DataBased.add_row-252"><span class="linenos">252</span></a>            <span class="k">if</span> <span class="n">columns</span><span class="p">:</span>
-</span><span id="DataBased.add_row-253"><a href="#DataBased.add_row-253"><span class="linenos">253</span></a>                <span class="n">columns</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">column</span> <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span><span class="p">)</span>
-</span><span id="DataBased.add_row-254"><a href="#DataBased.add_row-254"><span class="linenos">254</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="DataBased.add_row-255"><a href="#DataBased.add_row-255"><span class="linenos">255</span></a>                    <span class="sa">f</span><span class="s2">&quot;insert into </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> (</span><span class="si">{</span><span class="n">columns</span><span class="si">}</span><span class="s2">) values(</span><span class="si">{</span><span class="n">parameterizer</span><span class="si">}</span><span class="s2">)&quot;</span><span class="p">,</span> <span class="n">values</span>
-</span><span id="DataBased.add_row-256"><a href="#DataBased.add_row-256"><span class="linenos">256</span></a>                <span class="p">)</span>
-</span><span id="DataBased.add_row-257"><a href="#DataBased.add_row-257"><span class="linenos">257</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="DataBased.add_row-258"><a href="#DataBased.add_row-258"><span class="linenos">258</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="DataBased.add_row-259"><a href="#DataBased.add_row-259"><span class="linenos">259</span></a>                    <span class="sa">f</span><span class="s2">&quot;insert into </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> values(</span><span class="si">{</span><span class="n">parameterizer</span><span class="si">}</span><span class="s2">)&quot;</span><span class="p">,</span> <span class="n">values</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.add_row-229"><a href="#DataBased.add_row-229"><span class="linenos">229</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased.add_row-230"><a href="#DataBased.add_row-230"><span class="linenos">230</span></a>    <span class="k">def</span> <span class="nf">add_row</span><span class="p">(</span>
+</span><span id="DataBased.add_row-231"><a href="#DataBased.add_row-231"><span class="linenos">231</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="n">Any</span><span class="p">],</span> <span class="n">columns</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="DataBased.add_row-232"><a href="#DataBased.add_row-232"><span class="linenos">232</span></a>    <span class="p">):</span>
+</span><span id="DataBased.add_row-233"><a href="#DataBased.add_row-233"><span class="linenos">233</span></a>        <span class="sd">&quot;&quot;&quot;Add row of values to table.</span>
+</span><span id="DataBased.add_row-234"><a href="#DataBased.add_row-234"><span class="linenos">234</span></a>
+</span><span id="DataBased.add_row-235"><a href="#DataBased.add_row-235"><span class="linenos">235</span></a><span class="sd">        :param table: The table to insert into.</span>
+</span><span id="DataBased.add_row-236"><a href="#DataBased.add_row-236"><span class="linenos">236</span></a>
+</span><span id="DataBased.add_row-237"><a href="#DataBased.add_row-237"><span class="linenos">237</span></a><span class="sd">        :param values: A tuple of values to be inserted into the table.</span>
+</span><span id="DataBased.add_row-238"><a href="#DataBased.add_row-238"><span class="linenos">238</span></a>
+</span><span id="DataBased.add_row-239"><a href="#DataBased.add_row-239"><span class="linenos">239</span></a><span class="sd">        :param columns: If None, values param is expected to supply</span>
+</span><span id="DataBased.add_row-240"><a href="#DataBased.add_row-240"><span class="linenos">240</span></a><span class="sd">        a value for every column in the table. If columns is</span>
+</span><span id="DataBased.add_row-241"><a href="#DataBased.add_row-241"><span class="linenos">241</span></a><span class="sd">        provided, it should contain the same number of elements as values.&quot;&quot;&quot;</span>
+</span><span id="DataBased.add_row-242"><a href="#DataBased.add_row-242"><span class="linenos">242</span></a>        <span class="n">parameterizer</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="s2">&quot;?&quot;</span> <span class="k">for</span> <span class="n">_</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
+</span><span id="DataBased.add_row-243"><a href="#DataBased.add_row-243"><span class="linenos">243</span></a>        <span class="n">logger_values</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
+</span><span id="DataBased.add_row-244"><a href="#DataBased.add_row-244"><span class="linenos">244</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="DataBased.add_row-245"><a href="#DataBased.add_row-245"><span class="linenos">245</span></a>            <span class="k">if</span> <span class="n">columns</span><span class="p">:</span>
+</span><span id="DataBased.add_row-246"><a href="#DataBased.add_row-246"><span class="linenos">246</span></a>                <span class="n">columns_query</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">column</span> <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span><span class="p">)</span>
+</span><span id="DataBased.add_row-247"><a href="#DataBased.add_row-247"><span class="linenos">247</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="DataBased.add_row-248"><a href="#DataBased.add_row-248"><span class="linenos">248</span></a>                    <span class="sa">f</span><span class="s2">&quot;insert into </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> (</span><span class="si">{</span><span class="n">columns_query</span><span class="si">}</span><span class="s2">) values(</span><span class="si">{</span><span class="n">parameterizer</span><span class="si">}</span><span class="s2">)&quot;</span><span class="p">,</span>
+</span><span id="DataBased.add_row-249"><a href="#DataBased.add_row-249"><span class="linenos">249</span></a>                    <span class="n">values</span><span class="p">,</span>
+</span><span id="DataBased.add_row-250"><a href="#DataBased.add_row-250"><span class="linenos">250</span></a>                <span class="p">)</span>
+</span><span id="DataBased.add_row-251"><a href="#DataBased.add_row-251"><span class="linenos">251</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="DataBased.add_row-252"><a href="#DataBased.add_row-252"><span class="linenos">252</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="DataBased.add_row-253"><a href="#DataBased.add_row-253"><span class="linenos">253</span></a>                    <span class="sa">f</span><span class="s2">&quot;insert into </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> values(</span><span class="si">{</span><span class="n">parameterizer</span><span class="si">}</span><span class="s2">)&quot;</span><span class="p">,</span> <span class="n">values</span>
+</span><span id="DataBased.add_row-254"><a href="#DataBased.add_row-254"><span class="linenos">254</span></a>                <span class="p">)</span>
+</span><span id="DataBased.add_row-255"><a href="#DataBased.add_row-255"><span class="linenos">255</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Added &quot;</span><span class="si">{</span><span class="n">logger_values</span><span class="si">}</span><span class="s1">&quot; to </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1"> table.&#39;</span><span class="p">)</span>
+</span><span id="DataBased.add_row-256"><a href="#DataBased.add_row-256"><span class="linenos">256</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DataBased.add_row-257"><a href="#DataBased.add_row-257"><span class="linenos">257</span></a>            <span class="k">if</span> <span class="s2">&quot;constraint&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">)</span><span class="o">.</span><span class="n">lower</span><span class="p">():</span>
+</span><span id="DataBased.add_row-258"><a href="#DataBased.add_row-258"><span class="linenos">258</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">exception</span><span class="p">(</span>
+</span><span id="DataBased.add_row-259"><a href="#DataBased.add_row-259"><span class="linenos">259</span></a>                    <span class="sa">f</span><span class="s1">&#39;Error adding &quot;</span><span class="si">{</span><span class="n">logger_values</span><span class="si">}</span><span class="s1">&quot; to </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1"> table.&#39;</span>
 </span><span id="DataBased.add_row-260"><a href="#DataBased.add_row-260"><span class="linenos">260</span></a>                <span class="p">)</span>
-</span><span id="DataBased.add_row-261"><a href="#DataBased.add_row-261"><span class="linenos">261</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Added &quot;</span><span class="si">{</span><span class="n">logger_values</span><span class="si">}</span><span class="s1">&quot; to </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1"> table.&#39;</span><span class="p">)</span>
-</span><span id="DataBased.add_row-262"><a href="#DataBased.add_row-262"><span class="linenos">262</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="DataBased.add_row-263"><a href="#DataBased.add_row-263"><span class="linenos">263</span></a>            <span class="k">if</span> <span class="s2">&quot;constraint&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">)</span><span class="o">.</span><span class="n">lower</span><span class="p">():</span>
-</span><span id="DataBased.add_row-264"><a href="#DataBased.add_row-264"><span class="linenos">264</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">exception</span><span class="p">(</span>
-</span><span id="DataBased.add_row-265"><a href="#DataBased.add_row-265"><span class="linenos">265</span></a>                    <span class="sa">f</span><span class="s1">&#39;Error adding &quot;</span><span class="si">{</span><span class="n">logger_values</span><span class="si">}</span><span class="s1">&quot; to </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1"> table.&#39;</span>
-</span><span id="DataBased.add_row-266"><a href="#DataBased.add_row-266"><span class="linenos">266</span></a>                <span class="p">)</span>
-</span><span id="DataBased.add_row-267"><a href="#DataBased.add_row-267"><span class="linenos">267</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="DataBased.add_row-268"><a href="#DataBased.add_row-268"><span class="linenos">268</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">debug</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">))</span>
+</span><span id="DataBased.add_row-261"><a href="#DataBased.add_row-261"><span class="linenos">261</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="DataBased.add_row-262"><a href="#DataBased.add_row-262"><span class="linenos">262</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">debug</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">))</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Add row of values to table.</p>
 
 <h6 id="parameters">Parameters</h6>
 
@@ -1593,90 +1543,90 @@
 
                             </div>
                             <div id="DataBased.get_rows" class="classattr">
                                         <input id="DataBased.get_rows-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">get_rows</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">table</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>,</span><span class="param">	<span class="n">sort_by_column</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">columns_to_return</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">return_as_dataframe</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>,</span><span class="param">	<span class="n">values_only</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>,</span><span class="param">	<span class="n">order_by</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">limit</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">) -> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]</span> <span class="o">|</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="n">pandas</span><span class="o">.</span><span class="n">core</span><span class="o">.</span><span class="n">frame</span><span class="o">.</span><span class="n">DataFrame</span>:</span></span>
+        <span class="name">get_rows</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">table</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>,</span><span class="param">	<span class="n">sort_by_column</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">columns_to_return</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">return_as_dataframe</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>,</span><span class="param">	<span class="n">values_only</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>,</span><span class="param">	<span class="n">order_by</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">limit</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">) -> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]</span> <span class="o">|</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="n">pandas</span><span class="o">.</span><span class="n">core</span><span class="o">.</span><span class="n">frame</span><span class="o">.</span><span class="n">DataFrame</span>:</span></span>
 
                 <label class="view-source-button" for="DataBased.get_rows-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.get_rows"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.get_rows-270"><a href="#DataBased.get_rows-270"><span class="linenos">270</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased.get_rows-271"><a href="#DataBased.get_rows-271"><span class="linenos">271</span></a>    <span class="k">def</span> <span class="nf">get_rows</span><span class="p">(</span>
-</span><span id="DataBased.get_rows-272"><a href="#DataBased.get_rows-272"><span class="linenos">272</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="DataBased.get_rows-273"><a href="#DataBased.get_rows-273"><span class="linenos">273</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
-</span><span id="DataBased.get_rows-274"><a href="#DataBased.get_rows-274"><span class="linenos">274</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="DataBased.get_rows-275"><a href="#DataBased.get_rows-275"><span class="linenos">275</span></a>        <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="DataBased.get_rows-276"><a href="#DataBased.get_rows-276"><span class="linenos">276</span></a>        <span class="n">sort_by_column</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="DataBased.get_rows-277"><a href="#DataBased.get_rows-277"><span class="linenos">277</span></a>        <span class="n">columns_to_return</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="DataBased.get_rows-278"><a href="#DataBased.get_rows-278"><span class="linenos">278</span></a>        <span class="n">return_as_dataframe</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
-</span><span id="DataBased.get_rows-279"><a href="#DataBased.get_rows-279"><span class="linenos">279</span></a>        <span class="n">values_only</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
-</span><span id="DataBased.get_rows-280"><a href="#DataBased.get_rows-280"><span class="linenos">280</span></a>        <span class="n">order_by</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="DataBased.get_rows-281"><a href="#DataBased.get_rows-281"><span class="linenos">281</span></a>        <span class="n">limit</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="DataBased.get_rows-282"><a href="#DataBased.get_rows-282"><span class="linenos">282</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]</span> <span class="o">|</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="n">pandas</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">:</span>
-</span><span id="DataBased.get_rows-283"><a href="#DataBased.get_rows-283"><span class="linenos">283</span></a>        <span class="sd">&quot;&quot;&quot;Returns rows from table as a list of dictionaries</span>
-</span><span id="DataBased.get_rows-284"><a href="#DataBased.get_rows-284"><span class="linenos">284</span></a><span class="sd">        where the key-value pairs of the dictionaries are</span>
-</span><span id="DataBased.get_rows-285"><a href="#DataBased.get_rows-285"><span class="linenos">285</span></a><span class="sd">        column name: row value.</span>
-</span><span id="DataBased.get_rows-286"><a href="#DataBased.get_rows-286"><span class="linenos">286</span></a>
-</span><span id="DataBased.get_rows-287"><a href="#DataBased.get_rows-287"><span class="linenos">287</span></a><span class="sd">        :param match_criteria: Can be a list of 2-tuples where each</span>
-</span><span id="DataBased.get_rows-288"><a href="#DataBased.get_rows-288"><span class="linenos">288</span></a><span class="sd">        tuple is (columnName, rowValue) or a dictionary where</span>
-</span><span id="DataBased.get_rows-289"><a href="#DataBased.get_rows-289"><span class="linenos">289</span></a><span class="sd">        keys are column names and values are row values.</span>
-</span><span id="DataBased.get_rows-290"><a href="#DataBased.get_rows-290"><span class="linenos">290</span></a>
-</span><span id="DataBased.get_rows-291"><a href="#DataBased.get_rows-291"><span class="linenos">291</span></a><span class="sd">        :param exact_match: If False, the rowValue for a give column</span>
-</span><span id="DataBased.get_rows-292"><a href="#DataBased.get_rows-292"><span class="linenos">292</span></a><span class="sd">        will be matched as a substring.</span>
-</span><span id="DataBased.get_rows-293"><a href="#DataBased.get_rows-293"><span class="linenos">293</span></a>
-</span><span id="DataBased.get_rows-294"><a href="#DataBased.get_rows-294"><span class="linenos">294</span></a><span class="sd">        :param sort_by_column: A column name to sort the results by.</span>
-</span><span id="DataBased.get_rows-295"><a href="#DataBased.get_rows-295"><span class="linenos">295</span></a><span class="sd">        This will sort results in Python after retrieving them from the db.</span>
-</span><span id="DataBased.get_rows-296"><a href="#DataBased.get_rows-296"><span class="linenos">296</span></a><span class="sd">        Use the &#39;order_by&#39; param to use SQLite engine for ordering.</span>
-</span><span id="DataBased.get_rows-297"><a href="#DataBased.get_rows-297"><span class="linenos">297</span></a>
-</span><span id="DataBased.get_rows-298"><a href="#DataBased.get_rows-298"><span class="linenos">298</span></a><span class="sd">        :param columns_to_return: Optional list of column names.</span>
-</span><span id="DataBased.get_rows-299"><a href="#DataBased.get_rows-299"><span class="linenos">299</span></a><span class="sd">        If provided, the elements returned by get_rows() will</span>
-</span><span id="DataBased.get_rows-300"><a href="#DataBased.get_rows-300"><span class="linenos">300</span></a><span class="sd">        only contain the provided columns. Otherwise every column</span>
-</span><span id="DataBased.get_rows-301"><a href="#DataBased.get_rows-301"><span class="linenos">301</span></a><span class="sd">        in the row is returned.</span>
-</span><span id="DataBased.get_rows-302"><a href="#DataBased.get_rows-302"><span class="linenos">302</span></a>
-</span><span id="DataBased.get_rows-303"><a href="#DataBased.get_rows-303"><span class="linenos">303</span></a><span class="sd">        :param return_as_dataframe: If True,</span>
-</span><span id="DataBased.get_rows-304"><a href="#DataBased.get_rows-304"><span class="linenos">304</span></a><span class="sd">        the results will be returned as a pandas.DataFrame object.</span>
-</span><span id="DataBased.get_rows-305"><a href="#DataBased.get_rows-305"><span class="linenos">305</span></a>
-</span><span id="DataBased.get_rows-306"><a href="#DataBased.get_rows-306"><span class="linenos">306</span></a><span class="sd">        :param values_only: Return the results as a list of tuples</span>
-</span><span id="DataBased.get_rows-307"><a href="#DataBased.get_rows-307"><span class="linenos">307</span></a><span class="sd">        instead of a list of dictionaries that have column names as keys.</span>
-</span><span id="DataBased.get_rows-308"><a href="#DataBased.get_rows-308"><span class="linenos">308</span></a><span class="sd">        The results will still be sorted according to sort_by_column if</span>
-</span><span id="DataBased.get_rows-309"><a href="#DataBased.get_rows-309"><span class="linenos">309</span></a><span class="sd">        one is provided.</span>
-</span><span id="DataBased.get_rows-310"><a href="#DataBased.get_rows-310"><span class="linenos">310</span></a>
-</span><span id="DataBased.get_rows-311"><a href="#DataBased.get_rows-311"><span class="linenos">311</span></a><span class="sd">        :param order_by: If given, a &#39;order by {order_by}&#39; clause</span>
-</span><span id="DataBased.get_rows-312"><a href="#DataBased.get_rows-312"><span class="linenos">312</span></a><span class="sd">        will be added to the select query.</span>
-</span><span id="DataBased.get_rows-313"><a href="#DataBased.get_rows-313"><span class="linenos">313</span></a>
-</span><span id="DataBased.get_rows-314"><a href="#DataBased.get_rows-314"><span class="linenos">314</span></a><span class="sd">        :param limit: If given, a &#39;limit {limit}&#39; clause will be</span>
-</span><span id="DataBased.get_rows-315"><a href="#DataBased.get_rows-315"><span class="linenos">315</span></a><span class="sd">        added to the select query.</span>
-</span><span id="DataBased.get_rows-316"><a href="#DataBased.get_rows-316"><span class="linenos">316</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="DataBased.get_rows-317"><a href="#DataBased.get_rows-317"><span class="linenos">317</span></a>
-</span><span id="DataBased.get_rows-318"><a href="#DataBased.get_rows-318"><span class="linenos">318</span></a>        <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">columns_to_return</span><span class="p">)</span> <span class="ow">is</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="DataBased.get_rows-319"><a href="#DataBased.get_rows-319"><span class="linenos">319</span></a>            <span class="n">columns_to_return</span> <span class="o">=</span> <span class="p">[</span><span class="n">columns_to_return</span><span class="p">]</span>
-</span><span id="DataBased.get_rows-320"><a href="#DataBased.get_rows-320"><span class="linenos">320</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;select * from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="DataBased.get_rows-321"><a href="#DataBased.get_rows-321"><span class="linenos">321</span></a>        <span class="n">matches</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="DataBased.get_rows-322"><a href="#DataBased.get_rows-322"><span class="linenos">322</span></a>        <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
-</span><span id="DataBased.get_rows-323"><a href="#DataBased.get_rows-323"><span class="linenos">323</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; where </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="DataBased.get_rows-324"><a href="#DataBased.get_rows-324"><span class="linenos">324</span></a>        <span class="k">if</span> <span class="n">order_by</span><span class="p">:</span>
-</span><span id="DataBased.get_rows-325"><a href="#DataBased.get_rows-325"><span class="linenos">325</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; order by </span><span class="si">{</span><span class="n">order_by</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="DataBased.get_rows-326"><a href="#DataBased.get_rows-326"><span class="linenos">326</span></a>        <span class="k">if</span> <span class="n">limit</span><span class="p">:</span>
-</span><span id="DataBased.get_rows-327"><a href="#DataBased.get_rows-327"><span class="linenos">327</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; limit </span><span class="si">{</span><span class="n">limit</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="DataBased.get_rows-328"><a href="#DataBased.get_rows-328"><span class="linenos">328</span></a>        <span class="n">query</span> <span class="o">+=</span> <span class="s2">&quot;;&quot;</span>
-</span><span id="DataBased.get_rows-329"><a href="#DataBased.get_rows-329"><span class="linenos">329</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
-</span><span id="DataBased.get_rows-330"><a href="#DataBased.get_rows-330"><span class="linenos">330</span></a>        <span class="n">matches</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()</span>
-</span><span id="DataBased.get_rows-331"><a href="#DataBased.get_rows-331"><span class="linenos">331</span></a>        <span class="n">results</span> <span class="o">=</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_dict</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">match</span><span class="p">,</span> <span class="n">columns_to_return</span><span class="p">)</span> <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">]</span>
-</span><span id="DataBased.get_rows-332"><a href="#DataBased.get_rows-332"><span class="linenos">332</span></a>        <span class="k">if</span> <span class="n">sort_by_column</span><span class="p">:</span>
-</span><span id="DataBased.get_rows-333"><a href="#DataBased.get_rows-333"><span class="linenos">333</span></a>            <span class="n">results</span> <span class="o">=</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">results</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="k">lambda</span> <span class="n">x</span><span class="p">:</span> <span class="n">x</span><span class="p">[</span><span class="n">sort_by_column</span><span class="p">])</span>
-</span><span id="DataBased.get_rows-334"><a href="#DataBased.get_rows-334"><span class="linenos">334</span></a>        <span class="k">if</span> <span class="n">return_as_dataframe</span><span class="p">:</span>
-</span><span id="DataBased.get_rows-335"><a href="#DataBased.get_rows-335"><span class="linenos">335</span></a>            <span class="k">return</span> <span class="n">pandas</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">(</span><span class="n">results</span><span class="p">)</span>
-</span><span id="DataBased.get_rows-336"><a href="#DataBased.get_rows-336"><span class="linenos">336</span></a>        <span class="k">if</span> <span class="n">values_only</span><span class="p">:</span>
-</span><span id="DataBased.get_rows-337"><a href="#DataBased.get_rows-337"><span class="linenos">337</span></a>            <span class="k">return</span> <span class="p">[</span><span class="nb">tuple</span><span class="p">(</span><span class="n">row</span><span class="o">.</span><span class="n">values</span><span class="p">())</span> <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">results</span><span class="p">]</span>
-</span><span id="DataBased.get_rows-338"><a href="#DataBased.get_rows-338"><span class="linenos">338</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="DataBased.get_rows-339"><a href="#DataBased.get_rows-339"><span class="linenos">339</span></a>            <span class="k">return</span> <span class="n">results</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.get_rows-264"><a href="#DataBased.get_rows-264"><span class="linenos">264</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased.get_rows-265"><a href="#DataBased.get_rows-265"><span class="linenos">265</span></a>    <span class="k">def</span> <span class="nf">get_rows</span><span class="p">(</span>
+</span><span id="DataBased.get_rows-266"><a href="#DataBased.get_rows-266"><span class="linenos">266</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="DataBased.get_rows-267"><a href="#DataBased.get_rows-267"><span class="linenos">267</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
+</span><span id="DataBased.get_rows-268"><a href="#DataBased.get_rows-268"><span class="linenos">268</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="DataBased.get_rows-269"><a href="#DataBased.get_rows-269"><span class="linenos">269</span></a>        <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="DataBased.get_rows-270"><a href="#DataBased.get_rows-270"><span class="linenos">270</span></a>        <span class="n">sort_by_column</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="DataBased.get_rows-271"><a href="#DataBased.get_rows-271"><span class="linenos">271</span></a>        <span class="n">columns_to_return</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="DataBased.get_rows-272"><a href="#DataBased.get_rows-272"><span class="linenos">272</span></a>        <span class="n">return_as_dataframe</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
+</span><span id="DataBased.get_rows-273"><a href="#DataBased.get_rows-273"><span class="linenos">273</span></a>        <span class="n">values_only</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
+</span><span id="DataBased.get_rows-274"><a href="#DataBased.get_rows-274"><span class="linenos">274</span></a>        <span class="n">order_by</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="DataBased.get_rows-275"><a href="#DataBased.get_rows-275"><span class="linenos">275</span></a>        <span class="n">limit</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="DataBased.get_rows-276"><a href="#DataBased.get_rows-276"><span class="linenos">276</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]</span> <span class="o">|</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="n">pandas</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">:</span>
+</span><span id="DataBased.get_rows-277"><a href="#DataBased.get_rows-277"><span class="linenos">277</span></a>        <span class="sd">&quot;&quot;&quot;Returns rows from table as a list of dictionaries</span>
+</span><span id="DataBased.get_rows-278"><a href="#DataBased.get_rows-278"><span class="linenos">278</span></a><span class="sd">        where the key-value pairs of the dictionaries are</span>
+</span><span id="DataBased.get_rows-279"><a href="#DataBased.get_rows-279"><span class="linenos">279</span></a><span class="sd">        column name: row value.</span>
+</span><span id="DataBased.get_rows-280"><a href="#DataBased.get_rows-280"><span class="linenos">280</span></a>
+</span><span id="DataBased.get_rows-281"><a href="#DataBased.get_rows-281"><span class="linenos">281</span></a><span class="sd">        :param match_criteria: Can be a list of 2-tuples where each</span>
+</span><span id="DataBased.get_rows-282"><a href="#DataBased.get_rows-282"><span class="linenos">282</span></a><span class="sd">        tuple is (columnName, rowValue) or a dictionary where</span>
+</span><span id="DataBased.get_rows-283"><a href="#DataBased.get_rows-283"><span class="linenos">283</span></a><span class="sd">        keys are column names and values are row values.</span>
+</span><span id="DataBased.get_rows-284"><a href="#DataBased.get_rows-284"><span class="linenos">284</span></a>
+</span><span id="DataBased.get_rows-285"><a href="#DataBased.get_rows-285"><span class="linenos">285</span></a><span class="sd">        :param exact_match: If False, the rowValue for a give column</span>
+</span><span id="DataBased.get_rows-286"><a href="#DataBased.get_rows-286"><span class="linenos">286</span></a><span class="sd">        will be matched as a substring.</span>
+</span><span id="DataBased.get_rows-287"><a href="#DataBased.get_rows-287"><span class="linenos">287</span></a>
+</span><span id="DataBased.get_rows-288"><a href="#DataBased.get_rows-288"><span class="linenos">288</span></a><span class="sd">        :param sort_by_column: A column name to sort the results by.</span>
+</span><span id="DataBased.get_rows-289"><a href="#DataBased.get_rows-289"><span class="linenos">289</span></a><span class="sd">        This will sort results in Python after retrieving them from the db.</span>
+</span><span id="DataBased.get_rows-290"><a href="#DataBased.get_rows-290"><span class="linenos">290</span></a><span class="sd">        Use the &#39;order_by&#39; param to use SQLite engine for ordering.</span>
+</span><span id="DataBased.get_rows-291"><a href="#DataBased.get_rows-291"><span class="linenos">291</span></a>
+</span><span id="DataBased.get_rows-292"><a href="#DataBased.get_rows-292"><span class="linenos">292</span></a><span class="sd">        :param columns_to_return: Optional list of column names.</span>
+</span><span id="DataBased.get_rows-293"><a href="#DataBased.get_rows-293"><span class="linenos">293</span></a><span class="sd">        If provided, the elements returned by get_rows() will</span>
+</span><span id="DataBased.get_rows-294"><a href="#DataBased.get_rows-294"><span class="linenos">294</span></a><span class="sd">        only contain the provided columns. Otherwise every column</span>
+</span><span id="DataBased.get_rows-295"><a href="#DataBased.get_rows-295"><span class="linenos">295</span></a><span class="sd">        in the row is returned.</span>
+</span><span id="DataBased.get_rows-296"><a href="#DataBased.get_rows-296"><span class="linenos">296</span></a>
+</span><span id="DataBased.get_rows-297"><a href="#DataBased.get_rows-297"><span class="linenos">297</span></a><span class="sd">        :param return_as_dataframe: If True,</span>
+</span><span id="DataBased.get_rows-298"><a href="#DataBased.get_rows-298"><span class="linenos">298</span></a><span class="sd">        the results will be returned as a pandas.DataFrame object.</span>
+</span><span id="DataBased.get_rows-299"><a href="#DataBased.get_rows-299"><span class="linenos">299</span></a>
+</span><span id="DataBased.get_rows-300"><a href="#DataBased.get_rows-300"><span class="linenos">300</span></a><span class="sd">        :param values_only: Return the results as a list of tuples</span>
+</span><span id="DataBased.get_rows-301"><a href="#DataBased.get_rows-301"><span class="linenos">301</span></a><span class="sd">        instead of a list of dictionaries that have column names as keys.</span>
+</span><span id="DataBased.get_rows-302"><a href="#DataBased.get_rows-302"><span class="linenos">302</span></a><span class="sd">        The results will still be sorted according to sort_by_column if</span>
+</span><span id="DataBased.get_rows-303"><a href="#DataBased.get_rows-303"><span class="linenos">303</span></a><span class="sd">        one is provided.</span>
+</span><span id="DataBased.get_rows-304"><a href="#DataBased.get_rows-304"><span class="linenos">304</span></a>
+</span><span id="DataBased.get_rows-305"><a href="#DataBased.get_rows-305"><span class="linenos">305</span></a><span class="sd">        :param order_by: If given, a &#39;order by {order_by}&#39; clause</span>
+</span><span id="DataBased.get_rows-306"><a href="#DataBased.get_rows-306"><span class="linenos">306</span></a><span class="sd">        will be added to the select query.</span>
+</span><span id="DataBased.get_rows-307"><a href="#DataBased.get_rows-307"><span class="linenos">307</span></a>
+</span><span id="DataBased.get_rows-308"><a href="#DataBased.get_rows-308"><span class="linenos">308</span></a><span class="sd">        :param limit: If given, a &#39;limit {limit}&#39; clause will be</span>
+</span><span id="DataBased.get_rows-309"><a href="#DataBased.get_rows-309"><span class="linenos">309</span></a><span class="sd">        added to the select query.</span>
+</span><span id="DataBased.get_rows-310"><a href="#DataBased.get_rows-310"><span class="linenos">310</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="DataBased.get_rows-311"><a href="#DataBased.get_rows-311"><span class="linenos">311</span></a>
+</span><span id="DataBased.get_rows-312"><a href="#DataBased.get_rows-312"><span class="linenos">312</span></a>        <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">columns_to_return</span><span class="p">)</span> <span class="ow">is</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="DataBased.get_rows-313"><a href="#DataBased.get_rows-313"><span class="linenos">313</span></a>            <span class="n">columns_to_return</span> <span class="o">=</span> <span class="p">[</span><span class="n">columns_to_return</span><span class="p">]</span>
+</span><span id="DataBased.get_rows-314"><a href="#DataBased.get_rows-314"><span class="linenos">314</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;select * from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="DataBased.get_rows-315"><a href="#DataBased.get_rows-315"><span class="linenos">315</span></a>        <span class="n">matches</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="DataBased.get_rows-316"><a href="#DataBased.get_rows-316"><span class="linenos">316</span></a>        <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
+</span><span id="DataBased.get_rows-317"><a href="#DataBased.get_rows-317"><span class="linenos">317</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; where </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="DataBased.get_rows-318"><a href="#DataBased.get_rows-318"><span class="linenos">318</span></a>        <span class="k">if</span> <span class="n">order_by</span><span class="p">:</span>
+</span><span id="DataBased.get_rows-319"><a href="#DataBased.get_rows-319"><span class="linenos">319</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; order by </span><span class="si">{</span><span class="n">order_by</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="DataBased.get_rows-320"><a href="#DataBased.get_rows-320"><span class="linenos">320</span></a>        <span class="k">if</span> <span class="n">limit</span><span class="p">:</span>
+</span><span id="DataBased.get_rows-321"><a href="#DataBased.get_rows-321"><span class="linenos">321</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; limit </span><span class="si">{</span><span class="n">limit</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="DataBased.get_rows-322"><a href="#DataBased.get_rows-322"><span class="linenos">322</span></a>        <span class="n">query</span> <span class="o">+=</span> <span class="s2">&quot;;&quot;</span>
+</span><span id="DataBased.get_rows-323"><a href="#DataBased.get_rows-323"><span class="linenos">323</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
+</span><span id="DataBased.get_rows-324"><a href="#DataBased.get_rows-324"><span class="linenos">324</span></a>        <span class="n">matches</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()</span>
+</span><span id="DataBased.get_rows-325"><a href="#DataBased.get_rows-325"><span class="linenos">325</span></a>        <span class="n">results</span> <span class="o">=</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_dict</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">match</span><span class="p">,</span> <span class="n">columns_to_return</span><span class="p">)</span> <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">]</span>
+</span><span id="DataBased.get_rows-326"><a href="#DataBased.get_rows-326"><span class="linenos">326</span></a>        <span class="k">if</span> <span class="n">sort_by_column</span><span class="p">:</span>
+</span><span id="DataBased.get_rows-327"><a href="#DataBased.get_rows-327"><span class="linenos">327</span></a>            <span class="n">results</span> <span class="o">=</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">results</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="k">lambda</span> <span class="n">x</span><span class="p">:</span> <span class="n">x</span><span class="p">[</span><span class="n">sort_by_column</span><span class="p">])</span>
+</span><span id="DataBased.get_rows-328"><a href="#DataBased.get_rows-328"><span class="linenos">328</span></a>        <span class="k">if</span> <span class="n">return_as_dataframe</span><span class="p">:</span>
+</span><span id="DataBased.get_rows-329"><a href="#DataBased.get_rows-329"><span class="linenos">329</span></a>            <span class="k">return</span> <span class="n">pandas</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">(</span><span class="n">results</span><span class="p">)</span>
+</span><span id="DataBased.get_rows-330"><a href="#DataBased.get_rows-330"><span class="linenos">330</span></a>        <span class="k">if</span> <span class="n">values_only</span><span class="p">:</span>
+</span><span id="DataBased.get_rows-331"><a href="#DataBased.get_rows-331"><span class="linenos">331</span></a>            <span class="k">return</span> <span class="p">[</span><span class="nb">tuple</span><span class="p">(</span><span class="n">row</span><span class="o">.</span><span class="n">values</span><span class="p">())</span> <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">results</span><span class="p">]</span>
+</span><span id="DataBased.get_rows-332"><a href="#DataBased.get_rows-332"><span class="linenos">332</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="DataBased.get_rows-333"><a href="#DataBased.get_rows-333"><span class="linenos">333</span></a>            <span class="k">return</span> <span class="n">results</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Returns rows from table as a list of dictionaries
 where the key-value pairs of the dictionaries are
 column name: row value.</p>
 
@@ -1711,50 +1661,50 @@
 
                             </div>
                             <div id="DataBased.find" class="classattr">
                                         <input id="DataBased.find-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">find</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">table</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">query_string</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">columns</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">) -> <span class="nb">tuple</span><span class="p">[</span><span class="nb">dict</span><span class="p">]</span>:</span></span>
+        <span class="name">find</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">table</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">query_string</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">columns</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">) -> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]</span>:</span></span>
 
                 <label class="view-source-button" for="DataBased.find-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.find"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.find-341"><a href="#DataBased.find-341"><span class="linenos">341</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased.find-342"><a href="#DataBased.find-342"><span class="linenos">342</span></a>    <span class="k">def</span> <span class="nf">find</span><span class="p">(</span>
-</span><span id="DataBased.find-343"><a href="#DataBased.find-343"><span class="linenos">343</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">query_string</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">columns</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="DataBased.find-344"><a href="#DataBased.find-344"><span class="linenos">344</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">tuple</span><span class="p">[</span><span class="nb">dict</span><span class="p">]:</span>
-</span><span id="DataBased.find-345"><a href="#DataBased.find-345"><span class="linenos">345</span></a>        <span class="sd">&quot;&quot;&quot;Search for rows that contain query_string as a substring</span>
-</span><span id="DataBased.find-346"><a href="#DataBased.find-346"><span class="linenos">346</span></a><span class="sd">        of any column.</span>
-</span><span id="DataBased.find-347"><a href="#DataBased.find-347"><span class="linenos">347</span></a>
-</span><span id="DataBased.find-348"><a href="#DataBased.find-348"><span class="linenos">348</span></a><span class="sd">        :param table: The table to search.</span>
-</span><span id="DataBased.find-349"><a href="#DataBased.find-349"><span class="linenos">349</span></a>
-</span><span id="DataBased.find-350"><a href="#DataBased.find-350"><span class="linenos">350</span></a><span class="sd">        :param query_string: The substring to search for in all columns.</span>
-</span><span id="DataBased.find-351"><a href="#DataBased.find-351"><span class="linenos">351</span></a>
-</span><span id="DataBased.find-352"><a href="#DataBased.find-352"><span class="linenos">352</span></a><span class="sd">        :param columns: A list of columns to search for query_string.</span>
-</span><span id="DataBased.find-353"><a href="#DataBased.find-353"><span class="linenos">353</span></a><span class="sd">        If None, all columns in the table will be searched.</span>
-</span><span id="DataBased.find-354"><a href="#DataBased.find-354"><span class="linenos">354</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="DataBased.find-355"><a href="#DataBased.find-355"><span class="linenos">355</span></a>        <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">columns</span><span class="p">)</span> <span class="ow">is</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="DataBased.find-356"><a href="#DataBased.find-356"><span class="linenos">356</span></a>            <span class="n">columns</span> <span class="o">=</span> <span class="p">[</span><span class="n">columns</span><span class="p">]</span>
-</span><span id="DataBased.find-357"><a href="#DataBased.find-357"><span class="linenos">357</span></a>        <span class="n">results</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="DataBased.find-358"><a href="#DataBased.find-358"><span class="linenos">358</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">columns</span><span class="p">:</span>
-</span><span id="DataBased.find-359"><a href="#DataBased.find-359"><span class="linenos">359</span></a>            <span class="n">columns</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_column_names</span><span class="p">(</span><span class="n">table</span><span class="p">)</span>
-</span><span id="DataBased.find-360"><a href="#DataBased.find-360"><span class="linenos">360</span></a>        <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span><span class="p">:</span>
-</span><span id="DataBased.find-361"><a href="#DataBased.find-361"><span class="linenos">361</span></a>            <span class="n">results</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span>
-</span><span id="DataBased.find-362"><a href="#DataBased.find-362"><span class="linenos">362</span></a>                <span class="p">[</span>
-</span><span id="DataBased.find-363"><a href="#DataBased.find-363"><span class="linenos">363</span></a>                    <span class="n">row</span>
-</span><span id="DataBased.find-364"><a href="#DataBased.find-364"><span class="linenos">364</span></a>                    <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_rows</span><span class="p">(</span>
-</span><span id="DataBased.find-365"><a href="#DataBased.find-365"><span class="linenos">365</span></a>                        <span class="n">table</span><span class="p">,</span> <span class="p">[(</span><span class="n">column</span><span class="p">,</span> <span class="n">query_string</span><span class="p">)],</span> <span class="n">exact_match</span><span class="o">=</span><span class="kc">False</span>
-</span><span id="DataBased.find-366"><a href="#DataBased.find-366"><span class="linenos">366</span></a>                    <span class="p">)</span>
-</span><span id="DataBased.find-367"><a href="#DataBased.find-367"><span class="linenos">367</span></a>                    <span class="k">if</span> <span class="n">row</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">results</span>
-</span><span id="DataBased.find-368"><a href="#DataBased.find-368"><span class="linenos">368</span></a>                <span class="p">]</span>
-</span><span id="DataBased.find-369"><a href="#DataBased.find-369"><span class="linenos">369</span></a>            <span class="p">)</span>
-</span><span id="DataBased.find-370"><a href="#DataBased.find-370"><span class="linenos">370</span></a>        <span class="k">return</span> <span class="n">results</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.find-335"><a href="#DataBased.find-335"><span class="linenos">335</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased.find-336"><a href="#DataBased.find-336"><span class="linenos">336</span></a>    <span class="k">def</span> <span class="nf">find</span><span class="p">(</span>
+</span><span id="DataBased.find-337"><a href="#DataBased.find-337"><span class="linenos">337</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">query_string</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">columns</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="DataBased.find-338"><a href="#DataBased.find-338"><span class="linenos">338</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]:</span>
+</span><span id="DataBased.find-339"><a href="#DataBased.find-339"><span class="linenos">339</span></a>        <span class="sd">&quot;&quot;&quot;Search for rows that contain query_string as a substring</span>
+</span><span id="DataBased.find-340"><a href="#DataBased.find-340"><span class="linenos">340</span></a><span class="sd">        of any column.</span>
+</span><span id="DataBased.find-341"><a href="#DataBased.find-341"><span class="linenos">341</span></a>
+</span><span id="DataBased.find-342"><a href="#DataBased.find-342"><span class="linenos">342</span></a><span class="sd">        :param table: The table to search.</span>
+</span><span id="DataBased.find-343"><a href="#DataBased.find-343"><span class="linenos">343</span></a>
+</span><span id="DataBased.find-344"><a href="#DataBased.find-344"><span class="linenos">344</span></a><span class="sd">        :param query_string: The substring to search for in all columns.</span>
+</span><span id="DataBased.find-345"><a href="#DataBased.find-345"><span class="linenos">345</span></a>
+</span><span id="DataBased.find-346"><a href="#DataBased.find-346"><span class="linenos">346</span></a><span class="sd">        :param columns: A list of columns to search for query_string.</span>
+</span><span id="DataBased.find-347"><a href="#DataBased.find-347"><span class="linenos">347</span></a><span class="sd">        If None, all columns in the table will be searched.</span>
+</span><span id="DataBased.find-348"><a href="#DataBased.find-348"><span class="linenos">348</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="DataBased.find-349"><a href="#DataBased.find-349"><span class="linenos">349</span></a>        <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">columns</span><span class="p">)</span> <span class="ow">is</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="DataBased.find-350"><a href="#DataBased.find-350"><span class="linenos">350</span></a>            <span class="n">columns</span> <span class="o">=</span> <span class="p">[</span><span class="n">columns</span><span class="p">]</span>
+</span><span id="DataBased.find-351"><a href="#DataBased.find-351"><span class="linenos">351</span></a>        <span class="n">results</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="DataBased.find-352"><a href="#DataBased.find-352"><span class="linenos">352</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">columns</span><span class="p">:</span>
+</span><span id="DataBased.find-353"><a href="#DataBased.find-353"><span class="linenos">353</span></a>            <span class="n">columns</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_column_names</span><span class="p">(</span><span class="n">table</span><span class="p">)</span>
+</span><span id="DataBased.find-354"><a href="#DataBased.find-354"><span class="linenos">354</span></a>        <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span><span class="p">:</span>
+</span><span id="DataBased.find-355"><a href="#DataBased.find-355"><span class="linenos">355</span></a>            <span class="n">results</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span>
+</span><span id="DataBased.find-356"><a href="#DataBased.find-356"><span class="linenos">356</span></a>                <span class="p">[</span>
+</span><span id="DataBased.find-357"><a href="#DataBased.find-357"><span class="linenos">357</span></a>                    <span class="n">row</span>
+</span><span id="DataBased.find-358"><a href="#DataBased.find-358"><span class="linenos">358</span></a>                    <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_rows</span><span class="p">(</span>
+</span><span id="DataBased.find-359"><a href="#DataBased.find-359"><span class="linenos">359</span></a>                        <span class="n">table</span><span class="p">,</span> <span class="p">[(</span><span class="n">column</span><span class="p">,</span> <span class="n">query_string</span><span class="p">)],</span> <span class="n">exact_match</span><span class="o">=</span><span class="kc">False</span>
+</span><span id="DataBased.find-360"><a href="#DataBased.find-360"><span class="linenos">360</span></a>                    <span class="p">)</span>
+</span><span id="DataBased.find-361"><a href="#DataBased.find-361"><span class="linenos">361</span></a>                    <span class="k">if</span> <span class="n">row</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">results</span>
+</span><span id="DataBased.find-362"><a href="#DataBased.find-362"><span class="linenos">362</span></a>                <span class="p">]</span>
+</span><span id="DataBased.find-363"><a href="#DataBased.find-363"><span class="linenos">363</span></a>            <span class="p">)</span>
+</span><span id="DataBased.find-364"><a href="#DataBased.find-364"><span class="linenos">364</span></a>        <span class="k">return</span> <span class="n">results</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Search for rows that contain query_string as a substring
 of any column.</p>
 
 <h6 id="parameters">Parameters</h6>
@@ -1776,40 +1726,40 @@
         <span class="def">def</span>
         <span class="name">delete</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">table</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span>,</span><span class="param">	<span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">) -> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="DataBased.delete-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.delete"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.delete-372"><a href="#DataBased.delete-372"><span class="linenos">372</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased.delete-373"><a href="#DataBased.delete-373"><span class="linenos">373</span></a>    <span class="k">def</span> <span class="nf">delete</span><span class="p">(</span>
-</span><span id="DataBased.delete-374"><a href="#DataBased.delete-374"><span class="linenos">374</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="DataBased.delete-375"><a href="#DataBased.delete-375"><span class="linenos">375</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="DataBased.delete-376"><a href="#DataBased.delete-376"><span class="linenos">376</span></a>        <span class="sd">&quot;&quot;&quot;Delete records from table.</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.delete-366"><a href="#DataBased.delete-366"><span class="linenos">366</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased.delete-367"><a href="#DataBased.delete-367"><span class="linenos">367</span></a>    <span class="k">def</span> <span class="nf">delete</span><span class="p">(</span>
+</span><span id="DataBased.delete-368"><a href="#DataBased.delete-368"><span class="linenos">368</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="DataBased.delete-369"><a href="#DataBased.delete-369"><span class="linenos">369</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="DataBased.delete-370"><a href="#DataBased.delete-370"><span class="linenos">370</span></a>        <span class="sd">&quot;&quot;&quot;Delete records from table.</span>
+</span><span id="DataBased.delete-371"><a href="#DataBased.delete-371"><span class="linenos">371</span></a>
+</span><span id="DataBased.delete-372"><a href="#DataBased.delete-372"><span class="linenos">372</span></a><span class="sd">        Returns number of deleted records.</span>
+</span><span id="DataBased.delete-373"><a href="#DataBased.delete-373"><span class="linenos">373</span></a>
+</span><span id="DataBased.delete-374"><a href="#DataBased.delete-374"><span class="linenos">374</span></a><span class="sd">        :param match_criteria: Can be a list of 2-tuples where each</span>
+</span><span id="DataBased.delete-375"><a href="#DataBased.delete-375"><span class="linenos">375</span></a><span class="sd">        tuple is (columnName, rowValue) or a dictionary where</span>
+</span><span id="DataBased.delete-376"><a href="#DataBased.delete-376"><span class="linenos">376</span></a><span class="sd">        keys are column names and values are row values.</span>
 </span><span id="DataBased.delete-377"><a href="#DataBased.delete-377"><span class="linenos">377</span></a>
-</span><span id="DataBased.delete-378"><a href="#DataBased.delete-378"><span class="linenos">378</span></a><span class="sd">        Returns number of deleted records.</span>
-</span><span id="DataBased.delete-379"><a href="#DataBased.delete-379"><span class="linenos">379</span></a>
-</span><span id="DataBased.delete-380"><a href="#DataBased.delete-380"><span class="linenos">380</span></a><span class="sd">        :param match_criteria: Can be a list of 2-tuples where each</span>
-</span><span id="DataBased.delete-381"><a href="#DataBased.delete-381"><span class="linenos">381</span></a><span class="sd">        tuple is (columnName, rowValue) or a dictionary where</span>
-</span><span id="DataBased.delete-382"><a href="#DataBased.delete-382"><span class="linenos">382</span></a><span class="sd">        keys are column names and values are row values.</span>
-</span><span id="DataBased.delete-383"><a href="#DataBased.delete-383"><span class="linenos">383</span></a>
-</span><span id="DataBased.delete-384"><a href="#DataBased.delete-384"><span class="linenos">384</span></a><span class="sd">        :param exact_match: If False, the rowValue for a give column</span>
-</span><span id="DataBased.delete-385"><a href="#DataBased.delete-385"><span class="linenos">385</span></a><span class="sd">        will be matched as a substring.</span>
-</span><span id="DataBased.delete-386"><a href="#DataBased.delete-386"><span class="linenos">386</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="DataBased.delete-387"><a href="#DataBased.delete-387"><span class="linenos">387</span></a>        <span class="n">num_matches</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">count</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span>
-</span><span id="DataBased.delete-388"><a href="#DataBased.delete-388"><span class="linenos">388</span></a>        <span class="n">conditions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span>
-</span><span id="DataBased.delete-389"><a href="#DataBased.delete-389"><span class="linenos">389</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="DataBased.delete-390"><a href="#DataBased.delete-390"><span class="linenos">390</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;delete from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DataBased.delete-391"><a href="#DataBased.delete-391"><span class="linenos">391</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
-</span><span id="DataBased.delete-392"><a href="#DataBased.delete-392"><span class="linenos">392</span></a>                <span class="sa">f</span><span class="s1">&#39;Deleted </span><span class="si">{</span><span class="n">num_matches</span><span class="si">}</span><span class="s1"> from &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&quot;.&#39;</span>
-</span><span id="DataBased.delete-393"><a href="#DataBased.delete-393"><span class="linenos">393</span></a>            <span class="p">)</span>
-</span><span id="DataBased.delete-394"><a href="#DataBased.delete-394"><span class="linenos">394</span></a>            <span class="k">return</span> <span class="n">num_matches</span>
-</span><span id="DataBased.delete-395"><a href="#DataBased.delete-395"><span class="linenos">395</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="DataBased.delete-396"><a href="#DataBased.delete-396"><span class="linenos">396</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">debug</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Error deleting from &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">.</span><span class="se">\n</span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s1">&#39;</span><span class="p">)</span>
-</span><span id="DataBased.delete-397"><a href="#DataBased.delete-397"><span class="linenos">397</span></a>            <span class="k">return</span> <span class="mi">0</span>
+</span><span id="DataBased.delete-378"><a href="#DataBased.delete-378"><span class="linenos">378</span></a><span class="sd">        :param exact_match: If False, the rowValue for a give column</span>
+</span><span id="DataBased.delete-379"><a href="#DataBased.delete-379"><span class="linenos">379</span></a><span class="sd">        will be matched as a substring.</span>
+</span><span id="DataBased.delete-380"><a href="#DataBased.delete-380"><span class="linenos">380</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="DataBased.delete-381"><a href="#DataBased.delete-381"><span class="linenos">381</span></a>        <span class="n">num_matches</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">count</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span>
+</span><span id="DataBased.delete-382"><a href="#DataBased.delete-382"><span class="linenos">382</span></a>        <span class="n">conditions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span>
+</span><span id="DataBased.delete-383"><a href="#DataBased.delete-383"><span class="linenos">383</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="DataBased.delete-384"><a href="#DataBased.delete-384"><span class="linenos">384</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;delete from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DataBased.delete-385"><a href="#DataBased.delete-385"><span class="linenos">385</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
+</span><span id="DataBased.delete-386"><a href="#DataBased.delete-386"><span class="linenos">386</span></a>                <span class="sa">f</span><span class="s1">&#39;Deleted </span><span class="si">{</span><span class="n">num_matches</span><span class="si">}</span><span class="s1"> from &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&quot;.&#39;</span>
+</span><span id="DataBased.delete-387"><a href="#DataBased.delete-387"><span class="linenos">387</span></a>            <span class="p">)</span>
+</span><span id="DataBased.delete-388"><a href="#DataBased.delete-388"><span class="linenos">388</span></a>            <span class="k">return</span> <span class="n">num_matches</span>
+</span><span id="DataBased.delete-389"><a href="#DataBased.delete-389"><span class="linenos">389</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DataBased.delete-390"><a href="#DataBased.delete-390"><span class="linenos">390</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">debug</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Error deleting from &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">.</span><span class="se">\n</span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s1">&#39;</span><span class="p">)</span>
+</span><span id="DataBased.delete-391"><a href="#DataBased.delete-391"><span class="linenos">391</span></a>            <span class="k">return</span> <span class="mi">0</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Delete records from table.</p>
 
 <p>Returns number of deleted records.</p>
 
@@ -1827,73 +1777,66 @@
 
                             </div>
                             <div id="DataBased.update" class="classattr">
                                         <input id="DataBased.update-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">update</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">table</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">column_to_update</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">new_value</span><span class="p">:</span> <span class="n">Any</span>,</span><span class="param">	<span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">) -> <span class="nb">bool</span>:</span></span>
+        <span class="name">update</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">table</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">column_to_update</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">new_value</span><span class="p">:</span> <span class="n">Any</span>,</span><span class="param">	<span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">) -> <span class="nb">bool</span>:</span></span>
 
                 <label class="view-source-button" for="DataBased.update-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.update"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.update-399"><a href="#DataBased.update-399"><span class="linenos">399</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased.update-400"><a href="#DataBased.update-400"><span class="linenos">400</span></a>    <span class="k">def</span> <span class="nf">update</span><span class="p">(</span>
-</span><span id="DataBased.update-401"><a href="#DataBased.update-401"><span class="linenos">401</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="DataBased.update-402"><a href="#DataBased.update-402"><span class="linenos">402</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
-</span><span id="DataBased.update-403"><a href="#DataBased.update-403"><span class="linenos">403</span></a>        <span class="n">column_to_update</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
-</span><span id="DataBased.update-404"><a href="#DataBased.update-404"><span class="linenos">404</span></a>        <span class="n">new_value</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
-</span><span id="DataBased.update-405"><a href="#DataBased.update-405"><span class="linenos">405</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="DataBased.update-406"><a href="#DataBased.update-406"><span class="linenos">406</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="DataBased.update-407"><a href="#DataBased.update-407"><span class="linenos">407</span></a>        <span class="sd">&quot;&quot;&quot;Update row value for entry matched with match_criteria.</span>
-</span><span id="DataBased.update-408"><a href="#DataBased.update-408"><span class="linenos">408</span></a>
-</span><span id="DataBased.update-409"><a href="#DataBased.update-409"><span class="linenos">409</span></a><span class="sd">        :param column_to_update: The column to be updated in the matched row.</span>
-</span><span id="DataBased.update-410"><a href="#DataBased.update-410"><span class="linenos">410</span></a>
-</span><span id="DataBased.update-411"><a href="#DataBased.update-411"><span class="linenos">411</span></a><span class="sd">        :param new_value: The new value to insert.</span>
-</span><span id="DataBased.update-412"><a href="#DataBased.update-412"><span class="linenos">412</span></a>
-</span><span id="DataBased.update-413"><a href="#DataBased.update-413"><span class="linenos">413</span></a><span class="sd">        :param match_criteria: Can be a list of 2-tuples where each</span>
-</span><span id="DataBased.update-414"><a href="#DataBased.update-414"><span class="linenos">414</span></a><span class="sd">        tuple is (columnName, rowValue) or a dictionary where</span>
-</span><span id="DataBased.update-415"><a href="#DataBased.update-415"><span class="linenos">415</span></a><span class="sd">        keys are column names and values are row values.</span>
-</span><span id="DataBased.update-416"><a href="#DataBased.update-416"><span class="linenos">416</span></a><span class="sd">        If None, every row will be updated.</span>
-</span><span id="DataBased.update-417"><a href="#DataBased.update-417"><span class="linenos">417</span></a>
-</span><span id="DataBased.update-418"><a href="#DataBased.update-418"><span class="linenos">418</span></a><span class="sd">        Returns True if successful, False if not.&quot;&quot;&quot;</span>
-</span><span id="DataBased.update-419"><a href="#DataBased.update-419"><span class="linenos">419</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;update </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> set </span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s2"> = ?&quot;</span>
-</span><span id="DataBased.update-420"><a href="#DataBased.update-420"><span class="linenos">420</span></a>        <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
-</span><span id="DataBased.update-421"><a href="#DataBased.update-421"><span class="linenos">421</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">count</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="DataBased.update-422"><a href="#DataBased.update-422"><span class="linenos">422</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
-</span><span id="DataBased.update-423"><a href="#DataBased.update-423"><span class="linenos">423</span></a>                    <span class="sa">f</span><span class="s2">&quot;Couldn&#39;t find matching records in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table to update to &#39;</span><span class="si">{</span><span class="n">new_value</span><span class="si">}</span><span class="s2">&#39;&quot;</span>
-</span><span id="DataBased.update-424"><a href="#DataBased.update-424"><span class="linenos">424</span></a>                <span class="p">)</span>
-</span><span id="DataBased.update-425"><a href="#DataBased.update-425"><span class="linenos">425</span></a>                <span class="k">return</span> <span class="kc">False</span>
-</span><span id="DataBased.update-426"><a href="#DataBased.update-426"><span class="linenos">426</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">)</span>
-</span><span id="DataBased.update-427"><a href="#DataBased.update-427"><span class="linenos">427</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="DataBased.update-428"><a href="#DataBased.update-428"><span class="linenos">428</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="DataBased.update-429"><a href="#DataBased.update-429"><span class="linenos">429</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="DataBased.update-430"><a href="#DataBased.update-430"><span class="linenos">430</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="DataBased.update-431"><a href="#DataBased.update-431"><span class="linenos">431</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="DataBased.update-432"><a href="#DataBased.update-432"><span class="linenos">432</span></a>                <span class="n">query</span><span class="p">,</span>
-</span><span id="DataBased.update-433"><a href="#DataBased.update-433"><span class="linenos">433</span></a>                <span class="p">(</span><span class="n">new_value</span><span class="p">,),</span>
-</span><span id="DataBased.update-434"><a href="#DataBased.update-434"><span class="linenos">434</span></a>            <span class="p">)</span>
-</span><span id="DataBased.update-435"><a href="#DataBased.update-435"><span class="linenos">435</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
-</span><span id="DataBased.update-436"><a href="#DataBased.update-436"><span class="linenos">436</span></a>                <span class="sa">f</span><span class="s1">&#39;Updated &quot;</span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s1">&quot; in &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table to &quot;</span><span class="si">{</span><span class="n">new_value</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&#39;</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.update-393"><a href="#DataBased.update-393"><span class="linenos">393</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased.update-394"><a href="#DataBased.update-394"><span class="linenos">394</span></a>    <span class="k">def</span> <span class="nf">update</span><span class="p">(</span>
+</span><span id="DataBased.update-395"><a href="#DataBased.update-395"><span class="linenos">395</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="DataBased.update-396"><a href="#DataBased.update-396"><span class="linenos">396</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
+</span><span id="DataBased.update-397"><a href="#DataBased.update-397"><span class="linenos">397</span></a>        <span class="n">column_to_update</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
+</span><span id="DataBased.update-398"><a href="#DataBased.update-398"><span class="linenos">398</span></a>        <span class="n">new_value</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
+</span><span id="DataBased.update-399"><a href="#DataBased.update-399"><span class="linenos">399</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="DataBased.update-400"><a href="#DataBased.update-400"><span class="linenos">400</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="DataBased.update-401"><a href="#DataBased.update-401"><span class="linenos">401</span></a>        <span class="sd">&quot;&quot;&quot;Update row value for entry matched with match_criteria.</span>
+</span><span id="DataBased.update-402"><a href="#DataBased.update-402"><span class="linenos">402</span></a>
+</span><span id="DataBased.update-403"><a href="#DataBased.update-403"><span class="linenos">403</span></a><span class="sd">        :param column_to_update: The column to be updated in the matched row.</span>
+</span><span id="DataBased.update-404"><a href="#DataBased.update-404"><span class="linenos">404</span></a>
+</span><span id="DataBased.update-405"><a href="#DataBased.update-405"><span class="linenos">405</span></a><span class="sd">        :param new_value: The new value to insert.</span>
+</span><span id="DataBased.update-406"><a href="#DataBased.update-406"><span class="linenos">406</span></a>
+</span><span id="DataBased.update-407"><a href="#DataBased.update-407"><span class="linenos">407</span></a><span class="sd">        :param match_criteria: Can be a list of 2-tuples where each</span>
+</span><span id="DataBased.update-408"><a href="#DataBased.update-408"><span class="linenos">408</span></a><span class="sd">        tuple is (columnName, rowValue) or a dictionary where</span>
+</span><span id="DataBased.update-409"><a href="#DataBased.update-409"><span class="linenos">409</span></a><span class="sd">        keys are column names and values are row values.</span>
+</span><span id="DataBased.update-410"><a href="#DataBased.update-410"><span class="linenos">410</span></a><span class="sd">        If None, every row will be updated.</span>
+</span><span id="DataBased.update-411"><a href="#DataBased.update-411"><span class="linenos">411</span></a>
+</span><span id="DataBased.update-412"><a href="#DataBased.update-412"><span class="linenos">412</span></a><span class="sd">        Returns True if successful, False if not.&quot;&quot;&quot;</span>
+</span><span id="DataBased.update-413"><a href="#DataBased.update-413"><span class="linenos">413</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;update </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> set </span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s2"> = ?&quot;</span>
+</span><span id="DataBased.update-414"><a href="#DataBased.update-414"><span class="linenos">414</span></a>        <span class="n">conditions</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="DataBased.update-415"><a href="#DataBased.update-415"><span class="linenos">415</span></a>        <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
+</span><span id="DataBased.update-416"><a href="#DataBased.update-416"><span class="linenos">416</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">count</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="DataBased.update-417"><a href="#DataBased.update-417"><span class="linenos">417</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
+</span><span id="DataBased.update-418"><a href="#DataBased.update-418"><span class="linenos">418</span></a>                    <span class="sa">f</span><span class="s2">&quot;Couldn&#39;t find matching records in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table to update to &#39;</span><span class="si">{</span><span class="n">new_value</span><span class="si">}</span><span class="s2">&#39;&quot;</span>
+</span><span id="DataBased.update-419"><a href="#DataBased.update-419"><span class="linenos">419</span></a>                <span class="p">)</span>
+</span><span id="DataBased.update-420"><a href="#DataBased.update-420"><span class="linenos">420</span></a>                <span class="k">return</span> <span class="kc">False</span>
+</span><span id="DataBased.update-421"><a href="#DataBased.update-421"><span class="linenos">421</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">)</span>
+</span><span id="DataBased.update-422"><a href="#DataBased.update-422"><span class="linenos">422</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="DataBased.update-423"><a href="#DataBased.update-423"><span class="linenos">423</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="DataBased.update-424"><a href="#DataBased.update-424"><span class="linenos">424</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="DataBased.update-425"><a href="#DataBased.update-425"><span class="linenos">425</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="DataBased.update-426"><a href="#DataBased.update-426"><span class="linenos">426</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="DataBased.update-427"><a href="#DataBased.update-427"><span class="linenos">427</span></a>                <span class="n">query</span><span class="p">,</span>
+</span><span id="DataBased.update-428"><a href="#DataBased.update-428"><span class="linenos">428</span></a>                <span class="p">(</span><span class="n">new_value</span><span class="p">,),</span>
+</span><span id="DataBased.update-429"><a href="#DataBased.update-429"><span class="linenos">429</span></a>            <span class="p">)</span>
+</span><span id="DataBased.update-430"><a href="#DataBased.update-430"><span class="linenos">430</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
+</span><span id="DataBased.update-431"><a href="#DataBased.update-431"><span class="linenos">431</span></a>                <span class="sa">f</span><span class="s1">&#39;Updated &quot;</span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s1">&quot; in &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table to &quot;</span><span class="si">{</span><span class="n">new_value</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&#39;</span>
+</span><span id="DataBased.update-432"><a href="#DataBased.update-432"><span class="linenos">432</span></a>            <span class="p">)</span>
+</span><span id="DataBased.update-433"><a href="#DataBased.update-433"><span class="linenos">433</span></a>            <span class="k">return</span> <span class="kc">True</span>
+</span><span id="DataBased.update-434"><a href="#DataBased.update-434"><span class="linenos">434</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DataBased.update-435"><a href="#DataBased.update-435"><span class="linenos">435</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span>
+</span><span id="DataBased.update-436"><a href="#DataBased.update-436"><span class="linenos">436</span></a>                <span class="sa">f</span><span class="s1">&#39;Failed to update &quot;</span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s1">&quot; in &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table to &quot;</span><span class="si">{</span><span class="n">new_value</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&quot;</span><span class="se">\n</span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s1">&#39;</span>
 </span><span id="DataBased.update-437"><a href="#DataBased.update-437"><span class="linenos">437</span></a>            <span class="p">)</span>
-</span><span id="DataBased.update-438"><a href="#DataBased.update-438"><span class="linenos">438</span></a>            <span class="k">return</span> <span class="kc">True</span>
-</span><span id="DataBased.update-439"><a href="#DataBased.update-439"><span class="linenos">439</span></a>        <span class="k">except</span> <span class="ne">UnboundLocalError</span><span class="p">:</span>
-</span><span id="DataBased.update-440"><a href="#DataBased.update-440"><span class="linenos">440</span></a>            <span class="n">table_filter_string</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
-</span><span id="DataBased.update-441"><a href="#DataBased.update-441"><span class="linenos">441</span></a>                <span class="n">table_filter</span> <span class="k">for</span> <span class="n">table_filter</span> <span class="ow">in</span> <span class="n">match_criteria</span>
-</span><span id="DataBased.update-442"><a href="#DataBased.update-442"><span class="linenos">442</span></a>            <span class="p">)</span>
-</span><span id="DataBased.update-443"><a href="#DataBased.update-443"><span class="linenos">443</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span>
-</span><span id="DataBased.update-444"><a href="#DataBased.update-444"><span class="linenos">444</span></a>                <span class="sa">f</span><span class="s2">&quot;No records found matching filters: </span><span class="si">{</span><span class="n">table_filter_string</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="DataBased.update-445"><a href="#DataBased.update-445"><span class="linenos">445</span></a>            <span class="p">)</span>
-</span><span id="DataBased.update-446"><a href="#DataBased.update-446"><span class="linenos">446</span></a>            <span class="k">return</span> <span class="kc">False</span>
-</span><span id="DataBased.update-447"><a href="#DataBased.update-447"><span class="linenos">447</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="DataBased.update-448"><a href="#DataBased.update-448"><span class="linenos">448</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span>
-</span><span id="DataBased.update-449"><a href="#DataBased.update-449"><span class="linenos">449</span></a>                <span class="sa">f</span><span class="s1">&#39;Failed to update &quot;</span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s1">&quot; in &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table to &quot;</span><span class="si">{</span><span class="n">new_value</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&quot;</span><span class="se">\n</span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s1">&#39;</span>
-</span><span id="DataBased.update-450"><a href="#DataBased.update-450"><span class="linenos">450</span></a>            <span class="p">)</span>
-</span><span id="DataBased.update-451"><a href="#DataBased.update-451"><span class="linenos">451</span></a>            <span class="k">return</span> <span class="kc">False</span>
+</span><span id="DataBased.update-438"><a href="#DataBased.update-438"><span class="linenos">438</span></a>            <span class="k">return</span> <span class="kc">False</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Update row value for entry matched with match_criteria.</p>
 
 <h6 id="parameters">Parameters</h6>
 
@@ -1918,25 +1861,27 @@
         <span class="def">def</span>
         <span class="name">drop_table</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">table</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">bool</span>:</span></span>
 
                 <label class="view-source-button" for="DataBased.drop_table-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.drop_table"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.drop_table-453"><a href="#DataBased.drop_table-453"><span class="linenos">453</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased.drop_table-454"><a href="#DataBased.drop_table-454"><span class="linenos">454</span></a>    <span class="k">def</span> <span class="nf">drop_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="DataBased.drop_table-455"><a href="#DataBased.drop_table-455"><span class="linenos">455</span></a>        <span class="sd">&quot;&quot;&quot;Drop a table from the database.</span>
-</span><span id="DataBased.drop_table-456"><a href="#DataBased.drop_table-456"><span class="linenos">456</span></a>
-</span><span id="DataBased.drop_table-457"><a href="#DataBased.drop_table-457"><span class="linenos">457</span></a><span class="sd">        Returns True if successful, False if not.&quot;&quot;&quot;</span>
-</span><span id="DataBased.drop_table-458"><a href="#DataBased.drop_table-458"><span class="linenos">458</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="DataBased.drop_table-459"><a href="#DataBased.drop_table-459"><span class="linenos">459</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;drop Table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DataBased.drop_table-460"><a href="#DataBased.drop_table-460"><span class="linenos">460</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Dropped table &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
-</span><span id="DataBased.drop_table-461"><a href="#DataBased.drop_table-461"><span class="linenos">461</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="DataBased.drop_table-462"><a href="#DataBased.drop_table-462"><span class="linenos">462</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
-</span><span id="DataBased.drop_table-463"><a href="#DataBased.drop_table-463"><span class="linenos">463</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Failed to drop table &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.drop_table-440"><a href="#DataBased.drop_table-440"><span class="linenos">440</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased.drop_table-441"><a href="#DataBased.drop_table-441"><span class="linenos">441</span></a>    <span class="k">def</span> <span class="nf">drop_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="DataBased.drop_table-442"><a href="#DataBased.drop_table-442"><span class="linenos">442</span></a>        <span class="sd">&quot;&quot;&quot;Drop a table from the database.</span>
+</span><span id="DataBased.drop_table-443"><a href="#DataBased.drop_table-443"><span class="linenos">443</span></a>
+</span><span id="DataBased.drop_table-444"><a href="#DataBased.drop_table-444"><span class="linenos">444</span></a><span class="sd">        Returns True if successful, False if not.&quot;&quot;&quot;</span>
+</span><span id="DataBased.drop_table-445"><a href="#DataBased.drop_table-445"><span class="linenos">445</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="DataBased.drop_table-446"><a href="#DataBased.drop_table-446"><span class="linenos">446</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;drop Table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DataBased.drop_table-447"><a href="#DataBased.drop_table-447"><span class="linenos">447</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Dropped table &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
+</span><span id="DataBased.drop_table-448"><a href="#DataBased.drop_table-448"><span class="linenos">448</span></a>            <span class="k">return</span> <span class="kc">True</span>
+</span><span id="DataBased.drop_table-449"><a href="#DataBased.drop_table-449"><span class="linenos">449</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DataBased.drop_table-450"><a href="#DataBased.drop_table-450"><span class="linenos">450</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
+</span><span id="DataBased.drop_table-451"><a href="#DataBased.drop_table-451"><span class="linenos">451</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Failed to drop table &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
+</span><span id="DataBased.drop_table-452"><a href="#DataBased.drop_table-452"><span class="linenos">452</span></a>            <span class="k">return</span> <span class="kc">False</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Drop a table from the database.</p>
 
 <p>Returns True if successful, False if not.</p>
 </div>
@@ -1944,41 +1889,41 @@
 
                             </div>
                             <div id="DataBased.add_column" class="classattr">
                                         <input id="DataBased.add_column-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">add_column</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">table</span><span class="p">:</span> <span class="nb">str</span>, </span><span class="param"><span class="n">column</span><span class="p">:</span> <span class="nb">str</span>, </span><span class="param"><span class="n">_type</span><span class="p">:</span> <span class="nb">str</span>, </span><span class="param"><span class="n">default_value</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">):</span></span>
+        <span class="name">add_column</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">table</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">column</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">_type</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">default_value</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DataBased.add_column-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.add_column"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.add_column-465"><a href="#DataBased.add_column-465"><span class="linenos">465</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased.add_column-466"><a href="#DataBased.add_column-466"><span class="linenos">466</span></a>    <span class="k">def</span> <span class="nf">add_column</span><span class="p">(</span>
-</span><span id="DataBased.add_column-467"><a href="#DataBased.add_column-467"><span class="linenos">467</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">column</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">_type</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">default_value</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="DataBased.add_column-468"><a href="#DataBased.add_column-468"><span class="linenos">468</span></a>    <span class="p">):</span>
-</span><span id="DataBased.add_column-469"><a href="#DataBased.add_column-469"><span class="linenos">469</span></a>        <span class="sd">&quot;&quot;&quot;Add a new column to table.</span>
-</span><span id="DataBased.add_column-470"><a href="#DataBased.add_column-470"><span class="linenos">470</span></a>
-</span><span id="DataBased.add_column-471"><a href="#DataBased.add_column-471"><span class="linenos">471</span></a><span class="sd">        :param column: Name of the column to add.</span>
-</span><span id="DataBased.add_column-472"><a href="#DataBased.add_column-472"><span class="linenos">472</span></a>
-</span><span id="DataBased.add_column-473"><a href="#DataBased.add_column-473"><span class="linenos">473</span></a><span class="sd">        :param _type: The data type of the new column.</span>
-</span><span id="DataBased.add_column-474"><a href="#DataBased.add_column-474"><span class="linenos">474</span></a>
-</span><span id="DataBased.add_column-475"><a href="#DataBased.add_column-475"><span class="linenos">475</span></a><span class="sd">        :param default_value: Optional default value for the column.&quot;&quot;&quot;</span>
-</span><span id="DataBased.add_column-476"><a href="#DataBased.add_column-476"><span class="linenos">476</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="DataBased.add_column-477"><a href="#DataBased.add_column-477"><span class="linenos">477</span></a>            <span class="k">if</span> <span class="n">default_value</span><span class="p">:</span>
-</span><span id="DataBased.add_column-478"><a href="#DataBased.add_column-478"><span class="linenos">478</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="DataBased.add_column-479"><a href="#DataBased.add_column-479"><span class="linenos">479</span></a>                    <span class="sa">f</span><span class="s2">&quot;alter table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> add column </span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">_type</span><span class="si">}</span><span class="s2"> default </span><span class="si">{</span><span class="n">default_value</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="DataBased.add_column-480"><a href="#DataBased.add_column-480"><span class="linenos">480</span></a>                <span class="p">)</span>
-</span><span id="DataBased.add_column-481"><a href="#DataBased.add_column-481"><span class="linenos">481</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="DataBased.add_column-482"><a href="#DataBased.add_column-482"><span class="linenos">482</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;alter table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> add column </span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">_type</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DataBased.add_column-483"><a href="#DataBased.add_column-483"><span class="linenos">483</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Added column &quot;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1">&quot; to &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table.&#39;</span><span class="p">)</span>
-</span><span id="DataBased.add_column-484"><a href="#DataBased.add_column-484"><span class="linenos">484</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="DataBased.add_column-485"><a href="#DataBased.add_column-485"><span class="linenos">485</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Failed to add column &quot;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1">&quot; to &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table.&#39;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.add_column-454"><a href="#DataBased.add_column-454"><span class="linenos">454</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased.add_column-455"><a href="#DataBased.add_column-455"><span class="linenos">455</span></a>    <span class="k">def</span> <span class="nf">add_column</span><span class="p">(</span>
+</span><span id="DataBased.add_column-456"><a href="#DataBased.add_column-456"><span class="linenos">456</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">column</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">_type</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">default_value</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="DataBased.add_column-457"><a href="#DataBased.add_column-457"><span class="linenos">457</span></a>    <span class="p">):</span>
+</span><span id="DataBased.add_column-458"><a href="#DataBased.add_column-458"><span class="linenos">458</span></a>        <span class="sd">&quot;&quot;&quot;Add a new column to table.</span>
+</span><span id="DataBased.add_column-459"><a href="#DataBased.add_column-459"><span class="linenos">459</span></a>
+</span><span id="DataBased.add_column-460"><a href="#DataBased.add_column-460"><span class="linenos">460</span></a><span class="sd">        :param column: Name of the column to add.</span>
+</span><span id="DataBased.add_column-461"><a href="#DataBased.add_column-461"><span class="linenos">461</span></a>
+</span><span id="DataBased.add_column-462"><a href="#DataBased.add_column-462"><span class="linenos">462</span></a><span class="sd">        :param _type: The data type of the new column.</span>
+</span><span id="DataBased.add_column-463"><a href="#DataBased.add_column-463"><span class="linenos">463</span></a>
+</span><span id="DataBased.add_column-464"><a href="#DataBased.add_column-464"><span class="linenos">464</span></a><span class="sd">        :param default_value: Optional default value for the column.&quot;&quot;&quot;</span>
+</span><span id="DataBased.add_column-465"><a href="#DataBased.add_column-465"><span class="linenos">465</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="DataBased.add_column-466"><a href="#DataBased.add_column-466"><span class="linenos">466</span></a>            <span class="k">if</span> <span class="n">default_value</span><span class="p">:</span>
+</span><span id="DataBased.add_column-467"><a href="#DataBased.add_column-467"><span class="linenos">467</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="DataBased.add_column-468"><a href="#DataBased.add_column-468"><span class="linenos">468</span></a>                    <span class="sa">f</span><span class="s2">&quot;alter table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> add column </span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">_type</span><span class="si">}</span><span class="s2"> default </span><span class="si">{</span><span class="n">default_value</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="DataBased.add_column-469"><a href="#DataBased.add_column-469"><span class="linenos">469</span></a>                <span class="p">)</span>
+</span><span id="DataBased.add_column-470"><a href="#DataBased.add_column-470"><span class="linenos">470</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="DataBased.add_column-471"><a href="#DataBased.add_column-471"><span class="linenos">471</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;alter table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> add column </span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">_type</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DataBased.add_column-472"><a href="#DataBased.add_column-472"><span class="linenos">472</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Added column &quot;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1">&quot; to &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table.&#39;</span><span class="p">)</span>
+</span><span id="DataBased.add_column-473"><a href="#DataBased.add_column-473"><span class="linenos">473</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DataBased.add_column-474"><a href="#DataBased.add_column-474"><span class="linenos">474</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Failed to add column &quot;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1">&quot; to &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table.&#39;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Add a new column to table.</p>
 
 <h6 id="parameters">Parameters</h6>
 
@@ -1993,35 +1938,35 @@
                             </div>
                             <div id="DataBased.data_to_string" class="classattr">
                                         <input id="DataBased.data_to_string-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
                     <div class="decorator">@staticmethod</div>
 
         <span class="def">def</span>
-        <span class="name">data_to_string</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]</span>,</span><span class="param">	<span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">) -> <span class="nb">str</span>:</span></span>
+        <span class="name">data_to_string</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]</span>,</span><span class="param">	<span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">) -> <span class="nb">str</span>:</span></span>
 
                 <label class="view-source-button" for="DataBased.data_to_string-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.data_to_string"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.data_to_string-487"><a href="#DataBased.data_to_string-487"><span class="linenos">487</span></a>    <span class="nd">@staticmethod</span>
-</span><span id="DataBased.data_to_string-488"><a href="#DataBased.data_to_string-488"><span class="linenos">488</span></a>    <span class="k">def</span> <span class="nf">data_to_string</span><span class="p">(</span>
-</span><span id="DataBased.data_to_string-489"><a href="#DataBased.data_to_string-489"><span class="linenos">489</span></a>        <span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">],</span> <span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="DataBased.data_to_string-490"><a href="#DataBased.data_to_string-490"><span class="linenos">490</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="DataBased.data_to_string-491"><a href="#DataBased.data_to_string-491"><span class="linenos">491</span></a>        <span class="sd">&quot;&quot;&quot;Uses tabulate to produce pretty string output</span>
-</span><span id="DataBased.data_to_string-492"><a href="#DataBased.data_to_string-492"><span class="linenos">492</span></a><span class="sd">        from a list of dictionaries.</span>
-</span><span id="DataBased.data_to_string-493"><a href="#DataBased.data_to_string-493"><span class="linenos">493</span></a>
-</span><span id="DataBased.data_to_string-494"><a href="#DataBased.data_to_string-494"><span class="linenos">494</span></a><span class="sd">        :param data: Assumes all dictionaries in list have the same set of keys.</span>
-</span><span id="DataBased.data_to_string-495"><a href="#DataBased.data_to_string-495"><span class="linenos">495</span></a>
-</span><span id="DataBased.data_to_string-496"><a href="#DataBased.data_to_string-496"><span class="linenos">496</span></a><span class="sd">        :param sort_key: Optional dictionary key to sort data with.</span>
-</span><span id="DataBased.data_to_string-497"><a href="#DataBased.data_to_string-497"><span class="linenos">497</span></a>
-</span><span id="DataBased.data_to_string-498"><a href="#DataBased.data_to_string-498"><span class="linenos">498</span></a><span class="sd">        :param wrap_to_terminal: If True, the table width will be wrapped</span>
-</span><span id="DataBased.data_to_string-499"><a href="#DataBased.data_to_string-499"><span class="linenos">499</span></a><span class="sd">        to fit within the current terminal window. Set to False</span>
-</span><span id="DataBased.data_to_string-500"><a href="#DataBased.data_to_string-500"><span class="linenos">500</span></a><span class="sd">        if the output is going into something like a txt file.&quot;&quot;&quot;</span>
-</span><span id="DataBased.data_to_string-501"><a href="#DataBased.data_to_string-501"><span class="linenos">501</span></a>        <span class="k">return</span> <span class="n">data_to_string</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">sort_key</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.data_to_string-476"><a href="#DataBased.data_to_string-476"><span class="linenos">476</span></a>    <span class="nd">@staticmethod</span>
+</span><span id="DataBased.data_to_string-477"><a href="#DataBased.data_to_string-477"><span class="linenos">477</span></a>    <span class="k">def</span> <span class="nf">data_to_string</span><span class="p">(</span>
+</span><span id="DataBased.data_to_string-478"><a href="#DataBased.data_to_string-478"><span class="linenos">478</span></a>        <span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">],</span> <span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="DataBased.data_to_string-479"><a href="#DataBased.data_to_string-479"><span class="linenos">479</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="DataBased.data_to_string-480"><a href="#DataBased.data_to_string-480"><span class="linenos">480</span></a>        <span class="sd">&quot;&quot;&quot;Uses tabulate to produce pretty string output</span>
+</span><span id="DataBased.data_to_string-481"><a href="#DataBased.data_to_string-481"><span class="linenos">481</span></a><span class="sd">        from a list of dictionaries.</span>
+</span><span id="DataBased.data_to_string-482"><a href="#DataBased.data_to_string-482"><span class="linenos">482</span></a>
+</span><span id="DataBased.data_to_string-483"><a href="#DataBased.data_to_string-483"><span class="linenos">483</span></a><span class="sd">        :param data: Assumes all dictionaries in list have the same set of keys.</span>
+</span><span id="DataBased.data_to_string-484"><a href="#DataBased.data_to_string-484"><span class="linenos">484</span></a>
+</span><span id="DataBased.data_to_string-485"><a href="#DataBased.data_to_string-485"><span class="linenos">485</span></a><span class="sd">        :param sort_key: Optional dictionary key to sort data with.</span>
+</span><span id="DataBased.data_to_string-486"><a href="#DataBased.data_to_string-486"><span class="linenos">486</span></a>
+</span><span id="DataBased.data_to_string-487"><a href="#DataBased.data_to_string-487"><span class="linenos">487</span></a><span class="sd">        :param wrap_to_terminal: If True, the table width will be wrapped</span>
+</span><span id="DataBased.data_to_string-488"><a href="#DataBased.data_to_string-488"><span class="linenos">488</span></a><span class="sd">        to fit within the current terminal window. Set to False</span>
+</span><span id="DataBased.data_to_string-489"><a href="#DataBased.data_to_string-489"><span class="linenos">489</span></a><span class="sd">        if the output is going into something like a txt file.&quot;&quot;&quot;</span>
+</span><span id="DataBased.data_to_string-490"><a href="#DataBased.data_to_string-490"><span class="linenos">490</span></a>        <span class="k">return</span> <span class="n">data_to_string</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">sort_key</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Uses tabulate to produce pretty string output
 from a list of dictionaries.</p>
 
 <h6 id="parameters">Parameters</h6>
@@ -2039,84 +1984,84 @@
                             </div>
                 </section>
                 <section id="data_to_string">
                             <input id="data_to_string-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">data_to_string</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]</span>,</span><span class="param">	<span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">) -> <span class="nb">str</span>:</span></span>
+        <span class="name">data_to_string</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]</span>,</span><span class="param">	<span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">) -> <span class="nb">str</span>:</span></span>
 
                 <label class="view-source-button" for="data_to_string-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#data_to_string"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="data_to_string-504"><a href="#data_to_string-504"><span class="linenos">504</span></a><span class="k">def</span> <span class="nf">data_to_string</span><span class="p">(</span>
-</span><span id="data_to_string-505"><a href="#data_to_string-505"><span class="linenos">505</span></a>    <span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">],</span> <span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="data_to_string-506"><a href="#data_to_string-506"><span class="linenos">506</span></a><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="data_to_string-507"><a href="#data_to_string-507"><span class="linenos">507</span></a>    <span class="sd">&quot;&quot;&quot;Use tabulate to produce grid output from a list of dictionaries.</span>
-</span><span id="data_to_string-508"><a href="#data_to_string-508"><span class="linenos">508</span></a>
-</span><span id="data_to_string-509"><a href="#data_to_string-509"><span class="linenos">509</span></a><span class="sd">    :param data: Assumes all dictionaries in list have the same set of keys.</span>
-</span><span id="data_to_string-510"><a href="#data_to_string-510"><span class="linenos">510</span></a>
-</span><span id="data_to_string-511"><a href="#data_to_string-511"><span class="linenos">511</span></a><span class="sd">    :param sort_key: Optional dictionary key to sort data with.</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="data_to_string-493"><a href="#data_to_string-493"><span class="linenos">493</span></a><span class="k">def</span> <span class="nf">data_to_string</span><span class="p">(</span>
+</span><span id="data_to_string-494"><a href="#data_to_string-494"><span class="linenos">494</span></a>    <span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">],</span> <span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="data_to_string-495"><a href="#data_to_string-495"><span class="linenos">495</span></a><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="data_to_string-496"><a href="#data_to_string-496"><span class="linenos">496</span></a>    <span class="sd">&quot;&quot;&quot;Use tabulate to produce grid output from a list of dictionaries.</span>
+</span><span id="data_to_string-497"><a href="#data_to_string-497"><span class="linenos">497</span></a>
+</span><span id="data_to_string-498"><a href="#data_to_string-498"><span class="linenos">498</span></a><span class="sd">    :param data: Assumes all dictionaries in list have the same set of keys.</span>
+</span><span id="data_to_string-499"><a href="#data_to_string-499"><span class="linenos">499</span></a>
+</span><span id="data_to_string-500"><a href="#data_to_string-500"><span class="linenos">500</span></a><span class="sd">    :param sort_key: Optional dictionary key to sort data with.</span>
+</span><span id="data_to_string-501"><a href="#data_to_string-501"><span class="linenos">501</span></a>
+</span><span id="data_to_string-502"><a href="#data_to_string-502"><span class="linenos">502</span></a><span class="sd">    :param wrap_to_terminal: If True, the column widths will be reduced so the grid fits</span>
+</span><span id="data_to_string-503"><a href="#data_to_string-503"><span class="linenos">503</span></a><span class="sd">    within the current terminal window without wrapping. If the column widths have reduced to 1</span>
+</span><span id="data_to_string-504"><a href="#data_to_string-504"><span class="linenos">504</span></a><span class="sd">    and the grid is still too wide, str(data) will be returned.&quot;&quot;&quot;</span>
+</span><span id="data_to_string-505"><a href="#data_to_string-505"><span class="linenos">505</span></a>    <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">data</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="data_to_string-506"><a href="#data_to_string-506"><span class="linenos">506</span></a>        <span class="k">return</span> <span class="s2">&quot;&quot;</span>
+</span><span id="data_to_string-507"><a href="#data_to_string-507"><span class="linenos">507</span></a>    <span class="k">if</span> <span class="n">sort_key</span><span class="p">:</span>
+</span><span id="data_to_string-508"><a href="#data_to_string-508"><span class="linenos">508</span></a>        <span class="n">data</span> <span class="o">=</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="k">lambda</span> <span class="n">d</span><span class="p">:</span> <span class="n">d</span><span class="p">[</span><span class="n">sort_key</span><span class="p">])</span>
+</span><span id="data_to_string-509"><a href="#data_to_string-509"><span class="linenos">509</span></a>    <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">d</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">data</span><span class="p">):</span>
+</span><span id="data_to_string-510"><a href="#data_to_string-510"><span class="linenos">510</span></a>        <span class="k">for</span> <span class="n">k</span> <span class="ow">in</span> <span class="n">d</span><span class="p">:</span>
+</span><span id="data_to_string-511"><a href="#data_to_string-511"><span class="linenos">511</span></a>            <span class="n">data</span><span class="p">[</span><span class="n">i</span><span class="p">][</span><span class="n">k</span><span class="p">]</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="n">data</span><span class="p">[</span><span class="n">i</span><span class="p">][</span><span class="n">k</span><span class="p">])</span>
 </span><span id="data_to_string-512"><a href="#data_to_string-512"><span class="linenos">512</span></a>
-</span><span id="data_to_string-513"><a href="#data_to_string-513"><span class="linenos">513</span></a><span class="sd">    :param wrap_to_terminal: If True, the column widths will be reduced so the grid fits</span>
-</span><span id="data_to_string-514"><a href="#data_to_string-514"><span class="linenos">514</span></a><span class="sd">    within the current terminal window without wrapping. If the column widths have reduced to 1</span>
-</span><span id="data_to_string-515"><a href="#data_to_string-515"><span class="linenos">515</span></a><span class="sd">    and the grid is still too wide, str(data) will be returned.&quot;&quot;&quot;</span>
-</span><span id="data_to_string-516"><a href="#data_to_string-516"><span class="linenos">516</span></a>    <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">data</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="data_to_string-517"><a href="#data_to_string-517"><span class="linenos">517</span></a>        <span class="k">return</span> <span class="s2">&quot;&quot;</span>
-</span><span id="data_to_string-518"><a href="#data_to_string-518"><span class="linenos">518</span></a>    <span class="k">if</span> <span class="n">sort_key</span><span class="p">:</span>
-</span><span id="data_to_string-519"><a href="#data_to_string-519"><span class="linenos">519</span></a>        <span class="n">data</span> <span class="o">=</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="k">lambda</span> <span class="n">d</span><span class="p">:</span> <span class="n">d</span><span class="p">[</span><span class="n">sort_key</span><span class="p">])</span>
-</span><span id="data_to_string-520"><a href="#data_to_string-520"><span class="linenos">520</span></a>    <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">d</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">data</span><span class="p">):</span>
-</span><span id="data_to_string-521"><a href="#data_to_string-521"><span class="linenos">521</span></a>        <span class="k">for</span> <span class="n">k</span> <span class="ow">in</span> <span class="n">d</span><span class="p">:</span>
-</span><span id="data_to_string-522"><a href="#data_to_string-522"><span class="linenos">522</span></a>            <span class="n">data</span><span class="p">[</span><span class="n">i</span><span class="p">][</span><span class="n">k</span><span class="p">]</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="n">data</span><span class="p">[</span><span class="n">i</span><span class="p">][</span><span class="n">k</span><span class="p">])</span>
-</span><span id="data_to_string-523"><a href="#data_to_string-523"><span class="linenos">523</span></a>
-</span><span id="data_to_string-524"><a href="#data_to_string-524"><span class="linenos">524</span></a>    <span class="n">too_wide</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="data_to_string-525"><a href="#data_to_string-525"><span class="linenos">525</span></a>    <span class="n">terminal_width</span> <span class="o">=</span> <span class="n">os</span><span class="o">.</span><span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span>
-</span><span id="data_to_string-526"><a href="#data_to_string-526"><span class="linenos">526</span></a>    <span class="n">max_col_widths</span> <span class="o">=</span> <span class="n">terminal_width</span>
-</span><span id="data_to_string-527"><a href="#data_to_string-527"><span class="linenos">527</span></a>    <span class="c1"># Make an output with effectively unrestricted column widths</span>
-</span><span id="data_to_string-528"><a href="#data_to_string-528"><span class="linenos">528</span></a>    <span class="c1"># to see if shrinking is necessary</span>
-</span><span id="data_to_string-529"><a href="#data_to_string-529"><span class="linenos">529</span></a>    <span class="n">output</span> <span class="o">=</span> <span class="n">tabulate</span><span class="p">(</span>
-</span><span id="data_to_string-530"><a href="#data_to_string-530"><span class="linenos">530</span></a>        <span class="n">data</span><span class="p">,</span>
-</span><span id="data_to_string-531"><a href="#data_to_string-531"><span class="linenos">531</span></a>        <span class="n">headers</span><span class="o">=</span><span class="s2">&quot;keys&quot;</span><span class="p">,</span>
-</span><span id="data_to_string-532"><a href="#data_to_string-532"><span class="linenos">532</span></a>        <span class="n">disable_numparse</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
-</span><span id="data_to_string-533"><a href="#data_to_string-533"><span class="linenos">533</span></a>        <span class="n">tablefmt</span><span class="o">=</span><span class="s2">&quot;grid&quot;</span><span class="p">,</span>
-</span><span id="data_to_string-534"><a href="#data_to_string-534"><span class="linenos">534</span></a>        <span class="n">maxcolwidths</span><span class="o">=</span><span class="n">max_col_widths</span><span class="p">,</span>
-</span><span id="data_to_string-535"><a href="#data_to_string-535"><span class="linenos">535</span></a>    <span class="p">)</span>
-</span><span id="data_to_string-536"><a href="#data_to_string-536"><span class="linenos">536</span></a>    <span class="n">current_width</span> <span class="o">=</span> <span class="n">output</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="data_to_string-537"><a href="#data_to_string-537"><span class="linenos">537</span></a>    <span class="k">if</span> <span class="n">current_width</span> <span class="o">&lt;</span> <span class="n">terminal_width</span><span class="p">:</span>
-</span><span id="data_to_string-538"><a href="#data_to_string-538"><span class="linenos">538</span></a>        <span class="n">too_wide</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="data_to_string-539"><a href="#data_to_string-539"><span class="linenos">539</span></a>    <span class="k">if</span> <span class="n">wrap_to_terminal</span> <span class="ow">and</span> <span class="n">too_wide</span><span class="p">:</span>
-</span><span id="data_to_string-540"><a href="#data_to_string-540"><span class="linenos">540</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Resizing grid to fit within the terminal...&quot;</span><span class="p">)</span>
-</span><span id="data_to_string-541"><a href="#data_to_string-541"><span class="linenos">541</span></a>        <span class="n">previous_col_widths</span> <span class="o">=</span> <span class="n">max_col_widths</span>
-</span><span id="data_to_string-542"><a href="#data_to_string-542"><span class="linenos">542</span></a>        <span class="n">acceptable_width</span> <span class="o">=</span> <span class="n">terminal_width</span> <span class="o">-</span> <span class="mi">10</span>
-</span><span id="data_to_string-543"><a href="#data_to_string-543"><span class="linenos">543</span></a>        <span class="k">while</span> <span class="n">too_wide</span> <span class="ow">and</span> <span class="n">max_col_widths</span> <span class="o">&gt;</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="data_to_string-544"><a href="#data_to_string-544"><span class="linenos">544</span></a>            <span class="k">if</span> <span class="n">current_width</span> <span class="o">&gt;</span> <span class="n">terminal_width</span><span class="p">:</span>
-</span><span id="data_to_string-545"><a href="#data_to_string-545"><span class="linenos">545</span></a>                <span class="n">previous_col_widths</span> <span class="o">=</span> <span class="n">max_col_widths</span>
-</span><span id="data_to_string-546"><a href="#data_to_string-546"><span class="linenos">546</span></a>                <span class="n">max_col_widths</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="n">max_col_widths</span> <span class="o">*</span> <span class="mf">0.5</span><span class="p">)</span>
-</span><span id="data_to_string-547"><a href="#data_to_string-547"><span class="linenos">547</span></a>            <span class="k">elif</span> <span class="n">current_width</span> <span class="o">&lt;</span> <span class="n">terminal_width</span><span class="p">:</span>
-</span><span id="data_to_string-548"><a href="#data_to_string-548"><span class="linenos">548</span></a>                <span class="c1"># Without lowering acceptable_width, this condition will cause infinite loop</span>
-</span><span id="data_to_string-549"><a href="#data_to_string-549"><span class="linenos">549</span></a>                <span class="k">if</span> <span class="n">max_col_widths</span> <span class="o">==</span> <span class="n">previous_col_widths</span> <span class="o">-</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="data_to_string-550"><a href="#data_to_string-550"><span class="linenos">550</span></a>                    <span class="n">acceptable_width</span> <span class="o">-=</span> <span class="mi">10</span>
-</span><span id="data_to_string-551"><a href="#data_to_string-551"><span class="linenos">551</span></a>                <span class="n">max_col_widths</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span>
-</span><span id="data_to_string-552"><a href="#data_to_string-552"><span class="linenos">552</span></a>                    <span class="n">max_col_widths</span> <span class="o">+</span> <span class="p">(</span><span class="mf">0.5</span> <span class="o">*</span> <span class="p">(</span><span class="n">previous_col_widths</span> <span class="o">-</span> <span class="n">max_col_widths</span><span class="p">))</span>
-</span><span id="data_to_string-553"><a href="#data_to_string-553"><span class="linenos">553</span></a>                <span class="p">)</span>
-</span><span id="data_to_string-554"><a href="#data_to_string-554"><span class="linenos">554</span></a>            <span class="n">output</span> <span class="o">=</span> <span class="n">tabulate</span><span class="p">(</span>
-</span><span id="data_to_string-555"><a href="#data_to_string-555"><span class="linenos">555</span></a>                <span class="n">data</span><span class="p">,</span>
-</span><span id="data_to_string-556"><a href="#data_to_string-556"><span class="linenos">556</span></a>                <span class="n">headers</span><span class="o">=</span><span class="s2">&quot;keys&quot;</span><span class="p">,</span>
-</span><span id="data_to_string-557"><a href="#data_to_string-557"><span class="linenos">557</span></a>                <span class="n">disable_numparse</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
-</span><span id="data_to_string-558"><a href="#data_to_string-558"><span class="linenos">558</span></a>                <span class="n">tablefmt</span><span class="o">=</span><span class="s2">&quot;grid&quot;</span><span class="p">,</span>
-</span><span id="data_to_string-559"><a href="#data_to_string-559"><span class="linenos">559</span></a>                <span class="n">maxcolwidths</span><span class="o">=</span><span class="n">max_col_widths</span><span class="p">,</span>
-</span><span id="data_to_string-560"><a href="#data_to_string-560"><span class="linenos">560</span></a>            <span class="p">)</span>
-</span><span id="data_to_string-561"><a href="#data_to_string-561"><span class="linenos">561</span></a>            <span class="n">current_width</span> <span class="o">=</span> <span class="n">output</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="data_to_string-562"><a href="#data_to_string-562"><span class="linenos">562</span></a>            <span class="k">if</span> <span class="n">acceptable_width</span> <span class="o">&lt;</span> <span class="n">current_width</span> <span class="o">&lt;</span> <span class="n">terminal_width</span><span class="p">:</span>
-</span><span id="data_to_string-563"><a href="#data_to_string-563"><span class="linenos">563</span></a>                <span class="n">too_wide</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="data_to_string-564"><a href="#data_to_string-564"><span class="linenos">564</span></a>        <span class="k">if</span> <span class="n">too_wide</span><span class="p">:</span>
-</span><span id="data_to_string-565"><a href="#data_to_string-565"><span class="linenos">565</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Couldn&#39;t resize grid to fit within the terminal.&quot;</span><span class="p">)</span>
-</span><span id="data_to_string-566"><a href="#data_to_string-566"><span class="linenos">566</span></a>            <span class="k">return</span> <span class="nb">str</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
-</span><span id="data_to_string-567"><a href="#data_to_string-567"><span class="linenos">567</span></a>    <span class="k">return</span> <span class="n">output</span>
+</span><span id="data_to_string-513"><a href="#data_to_string-513"><span class="linenos">513</span></a>    <span class="n">too_wide</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="data_to_string-514"><a href="#data_to_string-514"><span class="linenos">514</span></a>    <span class="n">terminal_width</span> <span class="o">=</span> <span class="n">os</span><span class="o">.</span><span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span>
+</span><span id="data_to_string-515"><a href="#data_to_string-515"><span class="linenos">515</span></a>    <span class="n">max_col_widths</span> <span class="o">=</span> <span class="n">terminal_width</span>
+</span><span id="data_to_string-516"><a href="#data_to_string-516"><span class="linenos">516</span></a>    <span class="c1"># Make an output with effectively unrestricted column widths</span>
+</span><span id="data_to_string-517"><a href="#data_to_string-517"><span class="linenos">517</span></a>    <span class="c1"># to see if shrinking is necessary</span>
+</span><span id="data_to_string-518"><a href="#data_to_string-518"><span class="linenos">518</span></a>    <span class="n">output</span> <span class="o">=</span> <span class="n">tabulate</span><span class="p">(</span>
+</span><span id="data_to_string-519"><a href="#data_to_string-519"><span class="linenos">519</span></a>        <span class="n">data</span><span class="p">,</span>
+</span><span id="data_to_string-520"><a href="#data_to_string-520"><span class="linenos">520</span></a>        <span class="n">headers</span><span class="o">=</span><span class="s2">&quot;keys&quot;</span><span class="p">,</span>
+</span><span id="data_to_string-521"><a href="#data_to_string-521"><span class="linenos">521</span></a>        <span class="n">disable_numparse</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
+</span><span id="data_to_string-522"><a href="#data_to_string-522"><span class="linenos">522</span></a>        <span class="n">tablefmt</span><span class="o">=</span><span class="s2">&quot;grid&quot;</span><span class="p">,</span>
+</span><span id="data_to_string-523"><a href="#data_to_string-523"><span class="linenos">523</span></a>        <span class="n">maxcolwidths</span><span class="o">=</span><span class="n">max_col_widths</span><span class="p">,</span>
+</span><span id="data_to_string-524"><a href="#data_to_string-524"><span class="linenos">524</span></a>    <span class="p">)</span>
+</span><span id="data_to_string-525"><a href="#data_to_string-525"><span class="linenos">525</span></a>    <span class="n">current_width</span> <span class="o">=</span> <span class="n">output</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="data_to_string-526"><a href="#data_to_string-526"><span class="linenos">526</span></a>    <span class="k">if</span> <span class="n">current_width</span> <span class="o">&lt;</span> <span class="n">terminal_width</span><span class="p">:</span>
+</span><span id="data_to_string-527"><a href="#data_to_string-527"><span class="linenos">527</span></a>        <span class="n">too_wide</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="data_to_string-528"><a href="#data_to_string-528"><span class="linenos">528</span></a>    <span class="k">if</span> <span class="n">wrap_to_terminal</span> <span class="ow">and</span> <span class="n">too_wide</span><span class="p">:</span>
+</span><span id="data_to_string-529"><a href="#data_to_string-529"><span class="linenos">529</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Resizing grid to fit within the terminal...&quot;</span><span class="p">)</span>
+</span><span id="data_to_string-530"><a href="#data_to_string-530"><span class="linenos">530</span></a>        <span class="n">previous_col_widths</span> <span class="o">=</span> <span class="n">max_col_widths</span>
+</span><span id="data_to_string-531"><a href="#data_to_string-531"><span class="linenos">531</span></a>        <span class="n">acceptable_width</span> <span class="o">=</span> <span class="n">terminal_width</span> <span class="o">-</span> <span class="mi">10</span>
+</span><span id="data_to_string-532"><a href="#data_to_string-532"><span class="linenos">532</span></a>        <span class="k">while</span> <span class="n">too_wide</span> <span class="ow">and</span> <span class="n">max_col_widths</span> <span class="o">&gt;</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="data_to_string-533"><a href="#data_to_string-533"><span class="linenos">533</span></a>            <span class="k">if</span> <span class="n">current_width</span> <span class="o">&gt;</span> <span class="n">terminal_width</span><span class="p">:</span>
+</span><span id="data_to_string-534"><a href="#data_to_string-534"><span class="linenos">534</span></a>                <span class="n">previous_col_widths</span> <span class="o">=</span> <span class="n">max_col_widths</span>
+</span><span id="data_to_string-535"><a href="#data_to_string-535"><span class="linenos">535</span></a>                <span class="n">max_col_widths</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="n">max_col_widths</span> <span class="o">*</span> <span class="mf">0.5</span><span class="p">)</span>
+</span><span id="data_to_string-536"><a href="#data_to_string-536"><span class="linenos">536</span></a>            <span class="k">elif</span> <span class="n">current_width</span> <span class="o">&lt;</span> <span class="n">terminal_width</span><span class="p">:</span>
+</span><span id="data_to_string-537"><a href="#data_to_string-537"><span class="linenos">537</span></a>                <span class="c1"># Without lowering acceptable_width, this condition will cause infinite loop</span>
+</span><span id="data_to_string-538"><a href="#data_to_string-538"><span class="linenos">538</span></a>                <span class="k">if</span> <span class="n">max_col_widths</span> <span class="o">==</span> <span class="n">previous_col_widths</span> <span class="o">-</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="data_to_string-539"><a href="#data_to_string-539"><span class="linenos">539</span></a>                    <span class="n">acceptable_width</span> <span class="o">-=</span> <span class="mi">10</span>
+</span><span id="data_to_string-540"><a href="#data_to_string-540"><span class="linenos">540</span></a>                <span class="n">max_col_widths</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span>
+</span><span id="data_to_string-541"><a href="#data_to_string-541"><span class="linenos">541</span></a>                    <span class="n">max_col_widths</span> <span class="o">+</span> <span class="p">(</span><span class="mf">0.5</span> <span class="o">*</span> <span class="p">(</span><span class="n">previous_col_widths</span> <span class="o">-</span> <span class="n">max_col_widths</span><span class="p">))</span>
+</span><span id="data_to_string-542"><a href="#data_to_string-542"><span class="linenos">542</span></a>                <span class="p">)</span>
+</span><span id="data_to_string-543"><a href="#data_to_string-543"><span class="linenos">543</span></a>            <span class="n">output</span> <span class="o">=</span> <span class="n">tabulate</span><span class="p">(</span>
+</span><span id="data_to_string-544"><a href="#data_to_string-544"><span class="linenos">544</span></a>                <span class="n">data</span><span class="p">,</span>
+</span><span id="data_to_string-545"><a href="#data_to_string-545"><span class="linenos">545</span></a>                <span class="n">headers</span><span class="o">=</span><span class="s2">&quot;keys&quot;</span><span class="p">,</span>
+</span><span id="data_to_string-546"><a href="#data_to_string-546"><span class="linenos">546</span></a>                <span class="n">disable_numparse</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
+</span><span id="data_to_string-547"><a href="#data_to_string-547"><span class="linenos">547</span></a>                <span class="n">tablefmt</span><span class="o">=</span><span class="s2">&quot;grid&quot;</span><span class="p">,</span>
+</span><span id="data_to_string-548"><a href="#data_to_string-548"><span class="linenos">548</span></a>                <span class="n">maxcolwidths</span><span class="o">=</span><span class="n">max_col_widths</span><span class="p">,</span>
+</span><span id="data_to_string-549"><a href="#data_to_string-549"><span class="linenos">549</span></a>            <span class="p">)</span>
+</span><span id="data_to_string-550"><a href="#data_to_string-550"><span class="linenos">550</span></a>            <span class="n">current_width</span> <span class="o">=</span> <span class="n">output</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="data_to_string-551"><a href="#data_to_string-551"><span class="linenos">551</span></a>            <span class="k">if</span> <span class="n">acceptable_width</span> <span class="o">&lt;</span> <span class="n">current_width</span> <span class="o">&lt;</span> <span class="n">terminal_width</span><span class="p">:</span>
+</span><span id="data_to_string-552"><a href="#data_to_string-552"><span class="linenos">552</span></a>                <span class="n">too_wide</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="data_to_string-553"><a href="#data_to_string-553"><span class="linenos">553</span></a>        <span class="k">if</span> <span class="n">too_wide</span><span class="p">:</span>
+</span><span id="data_to_string-554"><a href="#data_to_string-554"><span class="linenos">554</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Couldn&#39;t resize grid to fit within the terminal.&quot;</span><span class="p">)</span>
+</span><span id="data_to_string-555"><a href="#data_to_string-555"><span class="linenos">555</span></a>            <span class="k">return</span> <span class="nb">str</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
+</span><span id="data_to_string-556"><a href="#data_to_string-556"><span class="linenos">556</span></a>    <span class="k">return</span> <span class="n">output</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Use tabulate to produce grid output from a list of dictionaries.</p>
 
 <h6 id="parameters">Parameters</h6>
```

#### html2text {}

```diff
@@ -1,15 +1,14 @@
 
 
   ⁰
 ____ databased [Unknown INPUT type]
 ***** API Documentation *****
     * DataBased
           o DataBased
-          o create_manager
           o open
           o close
           o query
           o create_tables
           o create_table
           o get_table_names
           o get_column_names
@@ -28,18 +27,18 @@
 ****** databased.databased ******
 ⁰ View Source
 __1import logging
 __2import os
 __3import sqlite3
 __4from datetime import datetime
 __5from functools import wraps
-__6from pathlib import Path
-__7from typing import Any
-__8
-__9import pandas
+__6from typing import Any
+__7
+__8import pandas
+__9from pathier import Pathier
 _10from tabulate import tabulate
 _11
 _12
 _13def _connect(func):
 _14    """Decorator to open db connection if it isn't already open."""
 _15
 _16    @wraps(func)
@@ -58,1397 +57,1370 @@
 _28
 _29    Supports saving and reading dates as datetime objects.
 _30
 _31    Supports using a context manager."""
 _32
 _33    def __init__(
 _34        self,
-_35        dbpath: str | Path,
+_35        dbpath: str | Pathier,
 _36        logger_encoding: str = "utf-8",
 _37        logger_message_format: str = "{levelname}|-|{asctime}|-|{message}",
 _38    ):
 _39        """
 _40        :param dbpath: String or Path object to database file.
 _41        If a relative path is given, it will be relative to the
 _42        current working directory. The log file will be saved to the
 _43        same directory.
 _44
 _45        :param logger_message_format: '{' style format string
 _46        for the logger object."""
-_47        self.dbpath = Path(dbpath)
-_48        self.dbname = Path(dbpath).name
+_47        self.dbpath = Pathier(dbpath)
+_48        self.dbname = Pathier(dbpath).name
 _49        self.dbpath.parent.mkdir(parents=True, exist_ok=True)
 _50        self._logger_init(
 _51            encoding=logger_encoding, message_format=logger_message_format
 _52        )
 _53        self.connection_open = False
-_54        self.create_manager()
-_55
-_56    def __enter__(self):
-_57        self.open()
-_58        return self
-_59
-_60    def __exit__(self, exception_type, exception_value,
+_54
+_55    def __enter__(self):
+_56        self.open()
+_57        return self
+_58
+_59    def __exit__(self, exception_type, exception_value,
 exception_traceback):
-_61        self.close()
-_62
-_63    def create_manager(self):
-_64        """Create dbmanager.py in the same directory
-_65        as the database file if it doesn't exist."""
-_66        manager_path = self.dbpath.parent / "dbmanager.py"
-_67        if not manager_path.exists():
-_68            manager_template = (Path(__file__).parent /
-"dbmanager.py").read_text()
-_69            manager_path.write_text(manager_template.replace("$dbname",
-self.dbname))
-_70
-_71    def open(self):
-_72        """Open connection to db."""
-_73        self.connection = sqlite3.connect(
-_74            self.dbpath,
-_75            detect_types=sqlite3.PARSE_DECLTYPES | sqlite3.PARSE_COLNAMES,
-_76            timeout=10,
-_77        )
-_78        self.connection.execute("pragma foreign_keys = 1")
-_79        self.cursor = self.connection.cursor()
-_80        self.connection_open = True
-_81
-_82    def close(self):
-_83        """Save and close connection to db.
-_84
-_85        Call this as soon as you are done using the database if you have
-_86        multiple threads or processes using the same database."""
-_87        if self.connection_open:
-_88            self.connection.commit()
-_89            self.connection.close()
-_90            self.connection_open = False
-_91
-_92    def _logger_init(
-_93        self,
-_94        message_format: str = "{levelname}|-|{asctime}|-|{message}",
-_95        encoding: str = "utf-8",
-_96    ):
-_97        """:param message_format: '{' style format string"""
-_98        self.logger = logging.getLogger(self.dbname)
-_99        if not self.logger.hasHandlers():
-100            handler = logging.FileHandler(
-101                str(self.dbpath).replace(".", "") + ".log",
+_60        self.close()
+_61
+_62    def open(self):
+_63        """Open connection to db."""
+_64        self.connection = sqlite3.connect(
+_65            self.dbpath,
+_66            detect_types=sqlite3.PARSE_DECLTYPES | sqlite3.PARSE_COLNAMES,
+_67            timeout=10,
+_68        )
+_69        self.connection.execute("pragma foreign_keys = 1")
+_70        self.cursor = self.connection.cursor()
+_71        self.connection_open = True
+_72
+_73    def close(self):
+_74        """Save and close connection to db.
+_75
+_76        Call this as soon as you are done using the database if you have
+_77        multiple threads or processes using the same database."""
+_78        if self.connection_open:
+_79            self.connection.commit()
+_80            self.connection.close()
+_81            self.connection_open = False
+_82
+_83    def _logger_init(
+_84        self,
+_85        message_format: str = "{levelname}|-|{asctime}|-|{message}",
+_86        encoding: str = "utf-8",
+_87    ):
+_88        """:param message_format: '{' style format string"""
+_89        self.logger = logging.getLogger(self.dbname)
+_90        if not self.logger.hasHandlers():
+_91            handler = logging.FileHandler(
+_92                str(self.dbpath).replace(".", "") + ".log",
 encoding=encoding
-102            )
-103            handler.setFormatter(
-104                logging.Formatter(
-105                    message_format, style="{", datefmt="%m/%d/%Y %I:%M:%S
+_93            )
+_94            handler.setFormatter(
+_95                logging.Formatter(
+_96                    message_format, style="{", datefmt="%m/%d/%Y %I:%M:%S
 %p"
-106                )
-107            )
-108            self.logger.addHandler(handler)
-109            self.logger.setLevel(logging.INFO)
-110
-111    def _get_dict(
-112        self, table: str, values: list, columns_to_return: list[str] = None
-113    ) -> dict:
-114        """Converts the values of a row into a dictionary with column names
+_97                )
+_98            )
+_99            self.logger.addHandler(handler)
+100            self.logger.setLevel(logging.INFO)
+101
+102    def _get_dict(
+103        self, table: str, values: list, columns_to_return: list[str] | None
+= None
+104    ) -> dict:
+105        """Converts the values of a row into a dictionary with column names
 as keys.
-115
-116        :param table: The table that values were pulled from.
-117
-118        :param values: List of values expected to be the same quantity
-119        and in the same order as the column names of table.
-120
-121        :param columns_to_return: An optional list of column names.
-122        If given, only these columns will be included in the returned
+106
+107        :param table: The table that values were pulled from.
+108
+109        :param values: List of values expected to be the same quantity
+110        and in the same order as the column names of table.
+111
+112        :param columns_to_return: An optional list of column names.
+113        If given, only these columns will be included in the returned
 dictionary.
-123        Otherwise all columns and values are returned."""
-124        return {
-125            column: value
-126            for column, value in zip(self.get_column_names(table), values)
-127            if not columns_to_return or column in columns_to_return
-128        }
+114        Otherwise all columns and values are returned."""
+115        return {
+116            column: value
+117            for column, value in zip(self.get_column_names(table), values)
+118            if not columns_to_return or column in columns_to_return
+119        }
+120
+121    def _get_conditions(
+122        self, match_criteria: list[tuple] | dict, exact_match: bool = True
+123    ) -> str:
+124        """Builds and returns the conditional portion of a query.
+125
+126        :param match_criteria: Can be a list of 2-tuples where each
+127        tuple is (columnName, rowValue) or a dictionary where
+128        keys are column names and values are row values.
 129
-130    def _get_conditions(
-131        self, match_criteria: list[tuple] | dict, exact_match: bool = True
-132    ) -> str:
-133        """Builds and returns the conditional portion of a query.
+130        :param exact_match: If False, the rowValue for a give column
+131        will be matched as a substring.
+132
+133        Usage e.g.:
 134
-135        :param match_criteria: Can be a list of 2-tuples where each
-136        tuple is (columnName, rowValue) or a dictionary where
-137        keys are column names and values are row values.
-138
-139        :param exact_match: If False, the rowValue for a give column
-140        will be matched as a substring.
-141
-142        Usage e.g.:
-143
-144        self.cursor.execute(f'select * from {table} where {conditions}')"""
-145        if type(match_criteria) == dict:
-146            match_criteria = [(k, v) for k, v in match_criteria.items()]
-147        if exact_match:
-148            conditions = " and ".join(
-149                f'"{column_row[0]}" = "{column_row[1]}"'
-150                for column_row in match_criteria
-151            )
-152        else:
-153            conditions = " and ".join(
-154                f'"{column_row[0]}" like "%{column_row[1]}%"'
-155                for column_row in match_criteria
-156            )
-157        return f"({conditions})"
-158
-159    @_connect
-160    def query(self, query_) -> list[Any]:
-161        """Execute an arbitrary query and
-162        return the results."""
-163        self.cursor.execute(query_)
-164        return self.cursor.fetchall()
-165
-166    @_connect
-167    def create_tables(self, table_querys: list[str] = []):
-168        """Create tables if they don't exist.
-169
-170        :param table_querys: Each query should be
-171        in the form 'tableName(columnDefinitions)'"""
-172        if len(table_querys) > 0:
-173            table_names = self.get_table_names()
-174            for table in table_querys:
-175                if table.split("(")[0].strip() not in table_names:
-176                    self.cursor.execute(f"create table {table}")
-177                    self.logger.info(f'{table.split("(")[0]} table
+135        self.cursor.execute(f'select * from {table} where {conditions}')"""
+136        if type(match_criteria) == dict:
+137            match_criteria = [(k, v) for k, v in match_criteria.items()]
+138        if exact_match:
+139            conditions = " and ".join(
+140                f'"{column_row[0]}" = "{column_row[1]}"'
+141                for column_row in match_criteria
+142            )
+143        else:
+144            conditions = " and ".join(
+145                f'"{column_row[0]}" like "%{column_row[1]}%"'
+146                for column_row in match_criteria
+147            )
+148        return f"({conditions})"
+149
+150    @_connect
+151    def query(self, query_) -> list[Any]:
+152        """Execute an arbitrary query and
+153        return the results."""
+154        self.cursor.execute(query_)
+155        return self.cursor.fetchall()
+156
+157    @_connect
+158    def create_tables(self, table_querys: list[str] = []):
+159        """Create tables if they don't exist.
+160
+161        :param table_querys: Each query should be
+162        in the form 'tableName(columnDefinitions)'"""
+163        if len(table_querys) > 0:
+164            table_names = self.get_table_names()
+165            for table in table_querys:
+166                if table.split("(")[0].strip() not in table_names:
+167                    self.cursor.execute(f"create table {table}")
+168                    self.logger.info(f'{table.split("(")[0]} table
 created.')
-178
-179    @_connect
-180    def create_table(self, table: str, column_defs: list[str]):
-181        """Create a table if it doesn't exist.
-182
-183        :param table: Name of the table to create.
-184
-185        :param column_defs: List of column definitions in
-186        proper Sqlite3 sytax.
-187        i.e. "columnName text unique" or "columnName int primary key"
+169
+170    @_connect
+171    def create_table(self, table: str, column_defs: list[str]):
+172        """Create a table if it doesn't exist.
+173
+174        :param table: Name of the table to create.
+175
+176        :param column_defs: List of column definitions in
+177        proper Sqlite3 sytax.
+178        i.e. "columnName text unique" or "columnName int primary key"
 etc."""
-188        if table not in self.get_table_names():
-189            query = f"create table {table}({', '.join(column_defs)})"
-190            self.cursor.execute(query)
-191            self.logger.info(f"'{table}' table created.")
-192
-193    @_connect
-194    def get_table_names(self) -> list[str]:
-195        """Returns a list of table names from database."""
-196        self.cursor.execute(
-197            'select name from sqlite_Schema where type = "table" and name
+179        if table not in self.get_table_names():
+180            query = f"create table {table}({', '.join(column_defs)})"
+181            self.cursor.execute(query)
+182            self.logger.info(f"'{table}' table created.")
+183
+184    @_connect
+185    def get_table_names(self) -> list[str]:
+186        """Returns a list of table names from database."""
+187        self.cursor.execute(
+188            'select name from sqlite_Schema where type = "table" and name
 not like "sqlite_%"'
-198        )
-199        return [result[0] for result in self.cursor.fetchall()]
-200
-201    @_connect
-202    def get_column_names(self, table: str) -> list[str]:
-203        """Return a list of column names from a table."""
-204        self.cursor.execute(f"select * from {table} where 1=0")
-205        return [description[0] for description in self.cursor.description]
+189        )
+190        return [result[0] for result in self.cursor.fetchall()]
+191
+192    @_connect
+193    def get_column_names(self, table: str) -> list[str]:
+194        """Return a list of column names from a table."""
+195        self.cursor.execute(f"select * from {table} where 1=0")
+196        return [description[0] for description in self.cursor.description]
+197
+198    @_connect
+199    def count(
+200        self,
+201        table: str,
+202        match_criteria: list[tuple] | dict | None = None,
+203        exact_match: bool = True,
+204    ) -> int:
+205        """Return number of items in table.
 206
-207    @_connect
-208    def count(
-209        self,
-210        table: str,
-211        match_criteria: list[tuple] | dict = None,
-212        exact_match: bool = True,
-213    ) -> int:
-214        """Return number of items in table.
-215
-216        :param match_criteria: Can be a list of 2-tuples where each
-217        tuple is (columnName, rowValue) or a dictionary where
-218        keys are column names and values are row values.
-219        If None, all rows from the table will be counted.
-220
-221        :param exact_match: If False, the row value for a give column
-222        in match_criteria will be matched as a substring. Has no effect if
-223        match_criteria is None.
-224        """
-225        query = f"select count(_rowid_) from {table}"
-226        try:
-227            if match_criteria:
-228                self.cursor.execute(
-229                    f"{query} where {self._get_conditions(match_criteria,
+207        :param match_criteria: Can be a list of 2-tuples where each
+208        tuple is (columnName, rowValue) or a dictionary where
+209        keys are column names and values are row values.
+210        If None, all rows from the table will be counted.
+211
+212        :param exact_match: If False, the row value for a give column
+213        in match_criteria will be matched as a substring. Has no effect if
+214        match_criteria is None.
+215        """
+216        query = f"select count(_rowid_) from {table}"
+217        try:
+218            if match_criteria:
+219                self.cursor.execute(
+220                    f"{query} where {self._get_conditions(match_criteria,
 exact_match)}"
-230                )
-231            else:
-232                self.cursor.execute(f"{query}")
-233            return self.cursor.fetchone()[0]
-234        except:
-235            return 0
-236
-237    @_connect
-238    def add_row(self, table: str, values: tuple[any], columns: tuple[str] =
-None):
-239        """Add row of values to table.
-240
-241        :param table: The table to insert into.
-242
-243        :param values: A tuple of values to be inserted into the table.
-244
-245        :param columns: If None, values param is expected to supply
-246        a value for every column in the table. If columns is
-247        provided, it should contain the same number of elements as
+221                )
+222            else:
+223                self.cursor.execute(f"{query}")
+224            return self.cursor.fetchone()[0]
+225        except:
+226            return 0
+227
+228    @_connect
+229    def add_row(
+230        self, table: str, values: tuple[Any], columns: tuple[str] | None =
+None
+231    ):
+232        """Add row of values to table.
+233
+234        :param table: The table to insert into.
+235
+236        :param values: A tuple of values to be inserted into the table.
+237
+238        :param columns: If None, values param is expected to supply
+239        a value for every column in the table. If columns is
+240        provided, it should contain the same number of elements as
 values."""
-248        parameterizer = ", ".join("?" for _ in values)
-249        logger_values = ", ".join(str(value) for value in values)
-250        try:
-251            if columns:
-252                columns = ", ".join(column for column in columns)
-253                self.cursor.execute(
-254                    f"insert into {table} ({columns}) values(
-{parameterizer})", values
-255                )
-256            else:
-257                self.cursor.execute(
-258                    f"insert into {table} values({parameterizer})", values
+241        parameterizer = ", ".join("?" for _ in values)
+242        logger_values = ", ".join(str(value) for value in values)
+243        try:
+244            if columns:
+245                columns_query = ", ".join(column for column in columns)
+246                self.cursor.execute(
+247                    f"insert into {table} ({columns_query}) values(
+{parameterizer})",
+248                    values,
+249                )
+250            else:
+251                self.cursor.execute(
+252                    f"insert into {table} values({parameterizer})", values
+253                )
+254            self.logger.info(f'Added "{logger_values}" to {table} table.')
+255        except Exception as e:
+256            if "constraint" not in str(e).lower():
+257                self.logger.exception(
+258                    f'Error adding "{logger_values}" to {table} table.'
 259                )
-260            self.logger.info(f'Added "{logger_values}" to {table} table.')
-261        except Exception as e:
-262            if "constraint" not in str(e).lower():
-263                self.logger.exception(
-264                    f'Error adding "{logger_values}" to {table} table.'
-265                )
-266            else:
-267                self.logger.debug(str(e))
-268
-269    @_connect
-270    def get_rows(
-271        self,
-272        table: str,
-273        match_criteria: list[tuple] | dict = None,
-274        exact_match: bool = True,
-275        sort_by_column: str = None,
-276        columns_to_return: list[str] = None,
-277        return_as_dataframe: bool = False,
-278        values_only: bool = False,
-279        order_by: str = None,
-280        limit: str | int = None,
-281    ) -> list[dict] | list[tuple] | pandas.DataFrame:
-282        """Returns rows from table as a list of dictionaries
-283        where the key-value pairs of the dictionaries are
-284        column name: row value.
-285
-286        :param match_criteria: Can be a list of 2-tuples where each
-287        tuple is (columnName, rowValue) or a dictionary where
-288        keys are column names and values are row values.
-289
-290        :param exact_match: If False, the rowValue for a give column
-291        will be matched as a substring.
-292
-293        :param sort_by_column: A column name to sort the results by.
-294        This will sort results in Python after retrieving them from the db.
-295        Use the 'order_by' param to use SQLite engine for ordering.
-296
-297        :param columns_to_return: Optional list of column names.
-298        If provided, the elements returned by get_rows() will
-299        only contain the provided columns. Otherwise every column
-300        in the row is returned.
-301
-302        :param return_as_dataframe: If True,
-303        the results will be returned as a pandas.DataFrame object.
-304
-305        :param values_only: Return the results as a list of tuples
-306        instead of a list of dictionaries that have column names as keys.
-307        The results will still be sorted according to sort_by_column if
-308        one is provided.
-309
-310        :param order_by: If given, a 'order by {order_by}' clause
-311        will be added to the select query.
-312
-313        :param limit: If given, a 'limit {limit}' clause will be
-314        added to the select query.
-315        """
-316
-317        if type(columns_to_return) is str:
-318            columns_to_return = [columns_to_return]
-319        query = f"select * from {table}"
-320        matches = []
-321        if match_criteria:
-322            query += f" where {self._get_conditions(match_criteria,
+260            else:
+261                self.logger.debug(str(e))
+262
+263    @_connect
+264    def get_rows(
+265        self,
+266        table: str,
+267        match_criteria: list[tuple] | dict | None = None,
+268        exact_match: bool = True,
+269        sort_by_column: str | None = None,
+270        columns_to_return: list[str] | None = None,
+271        return_as_dataframe: bool = False,
+272        values_only: bool = False,
+273        order_by: str | None = None,
+274        limit: str | int | None = None,
+275    ) -> list[dict] | list[tuple] | pandas.DataFrame:
+276        """Returns rows from table as a list of dictionaries
+277        where the key-value pairs of the dictionaries are
+278        column name: row value.
+279
+280        :param match_criteria: Can be a list of 2-tuples where each
+281        tuple is (columnName, rowValue) or a dictionary where
+282        keys are column names and values are row values.
+283
+284        :param exact_match: If False, the rowValue for a give column
+285        will be matched as a substring.
+286
+287        :param sort_by_column: A column name to sort the results by.
+288        This will sort results in Python after retrieving them from the db.
+289        Use the 'order_by' param to use SQLite engine for ordering.
+290
+291        :param columns_to_return: Optional list of column names.
+292        If provided, the elements returned by get_rows() will
+293        only contain the provided columns. Otherwise every column
+294        in the row is returned.
+295
+296        :param return_as_dataframe: If True,
+297        the results will be returned as a pandas.DataFrame object.
+298
+299        :param values_only: Return the results as a list of tuples
+300        instead of a list of dictionaries that have column names as keys.
+301        The results will still be sorted according to sort_by_column if
+302        one is provided.
+303
+304        :param order_by: If given, a 'order by {order_by}' clause
+305        will be added to the select query.
+306
+307        :param limit: If given, a 'limit {limit}' clause will be
+308        added to the select query.
+309        """
+310
+311        if type(columns_to_return) is str:
+312            columns_to_return = [columns_to_return]
+313        query = f"select * from {table}"
+314        matches = []
+315        if match_criteria:
+316            query += f" where {self._get_conditions(match_criteria,
 exact_match)}"
-323        if order_by:
-324            query += f" order by {order_by}"
-325        if limit:
-326            query += f" limit {limit}"
-327        query += ";"
-328        self.cursor.execute(query)
-329        matches = self.cursor.fetchall()
-330        results = [self._get_dict(table, match, columns_to_return) for match
+317        if order_by:
+318            query += f" order by {order_by}"
+319        if limit:
+320            query += f" limit {limit}"
+321        query += ";"
+322        self.cursor.execute(query)
+323        matches = self.cursor.fetchall()
+324        results = [self._get_dict(table, match, columns_to_return) for match
 in matches]
-331        if sort_by_column:
-332            results = sorted(results, key=lambda x: x[sort_by_column])
-333        if return_as_dataframe:
-334            return pandas.DataFrame(results)
-335        if values_only:
-336            return [tuple(row.values()) for row in results]
-337        else:
-338            return results
-339
-340    @_connect
-341    def find(
-342        self, table: str, query_string: str, columns: list[str] = None
-343    ) -> tuple[dict]:
-344        """Search for rows that contain query_string as a substring
-345        of any column.
-346
-347        :param table: The table to search.
-348
-349        :param query_string: The substring to search for in all columns.
-350
-351        :param columns: A list of columns to search for query_string.
-352        If None, all columns in the table will be searched.
-353        """
-354        if type(columns) is str:
-355            columns = [columns]
-356        results = []
-357        if not columns:
-358            columns = self.get_column_names(table)
-359        for column in columns:
-360            results.extend(
-361                [
-362                    row
-363                    for row in self.get_rows(
-364                        table, [(column, query_string)], exact_match=False
-365                    )
-366                    if row not in results
-367                ]
-368            )
-369        return results
-370
-371    @_connect
-372    def delete(
-373        self, table: str, match_criteria: list[tuple] | dict, exact_match:
+325        if sort_by_column:
+326            results = sorted(results, key=lambda x: x[sort_by_column])
+327        if return_as_dataframe:
+328            return pandas.DataFrame(results)
+329        if values_only:
+330            return [tuple(row.values()) for row in results]
+331        else:
+332            return results
+333
+334    @_connect
+335    def find(
+336        self, table: str, query_string: str, columns: list[str] | None =
+None
+337    ) -> list[dict]:
+338        """Search for rows that contain query_string as a substring
+339        of any column.
+340
+341        :param table: The table to search.
+342
+343        :param query_string: The substring to search for in all columns.
+344
+345        :param columns: A list of columns to search for query_string.
+346        If None, all columns in the table will be searched.
+347        """
+348        if type(columns) is str:
+349            columns = [columns]
+350        results = []
+351        if not columns:
+352            columns = self.get_column_names(table)
+353        for column in columns:
+354            results.extend(
+355                [
+356                    row
+357                    for row in self.get_rows(
+358                        table, [(column, query_string)], exact_match=False
+359                    )
+360                    if row not in results
+361                ]
+362            )
+363        return results
+364
+365    @_connect
+366    def delete(
+367        self, table: str, match_criteria: list[tuple] | dict, exact_match:
 bool = True
-374    ) -> int:
-375        """Delete records from table.
+368    ) -> int:
+369        """Delete records from table.
+370
+371        Returns number of deleted records.
+372
+373        :param match_criteria: Can be a list of 2-tuples where each
+374        tuple is (columnName, rowValue) or a dictionary where
+375        keys are column names and values are row values.
 376
-377        Returns number of deleted records.
-378
-379        :param match_criteria: Can be a list of 2-tuples where each
-380        tuple is (columnName, rowValue) or a dictionary where
-381        keys are column names and values are row values.
-382
-383        :param exact_match: If False, the rowValue for a give column
-384        will be matched as a substring.
-385        """
-386        num_matches = self.count(table, match_criteria, exact_match)
-387        conditions = self._get_conditions(match_criteria, exact_match)
-388        try:
-389            self.cursor.execute(f"delete from {table} where {conditions}")
-390            self.logger.info(
-391                f'Deleted {num_matches} from "{table}" where {conditions}".'
-392            )
-393            return num_matches
-394        except Exception as e:
-395            self.logger.debug(f'Error deleting from "{table}" where
+377        :param exact_match: If False, the rowValue for a give column
+378        will be matched as a substring.
+379        """
+380        num_matches = self.count(table, match_criteria, exact_match)
+381        conditions = self._get_conditions(match_criteria, exact_match)
+382        try:
+383            self.cursor.execute(f"delete from {table} where {conditions}")
+384            self.logger.info(
+385                f'Deleted {num_matches} from "{table}" where {conditions}".'
+386            )
+387            return num_matches
+388        except Exception as e:
+389            self.logger.debug(f'Error deleting from "{table}" where
 {conditions}.\n{e}')
-396            return 0
-397
-398    @_connect
-399    def update(
-400        self,
-401        table: str,
-402        column_to_update: str,
-403        new_value: Any,
-404        match_criteria: list[tuple] | dict = None,
-405    ) -> bool:
-406        """Update row value for entry matched with match_criteria.
-407
-408        :param column_to_update: The column to be updated in the matched
+390            return 0
+391
+392    @_connect
+393    def update(
+394        self,
+395        table: str,
+396        column_to_update: str,
+397        new_value: Any,
+398        match_criteria: list[tuple] | dict | None = None,
+399    ) -> bool:
+400        """Update row value for entry matched with match_criteria.
+401
+402        :param column_to_update: The column to be updated in the matched
 row.
-409
-410        :param new_value: The new value to insert.
-411
-412        :param match_criteria: Can be a list of 2-tuples where each
-413        tuple is (columnName, rowValue) or a dictionary where
-414        keys are column names and values are row values.
-415        If None, every row will be updated.
-416
-417        Returns True if successful, False if not."""
-418        query = f"update {table} set {column_to_update} = ?"
-419        if match_criteria:
-420            if self.count(table, match_criteria) == 0:
-421                self.logger.info(
-422                    f"Couldn't find matching records in {table} table to
+403
+404        :param new_value: The new value to insert.
+405
+406        :param match_criteria: Can be a list of 2-tuples where each
+407        tuple is (columnName, rowValue) or a dictionary where
+408        keys are column names and values are row values.
+409        If None, every row will be updated.
+410
+411        Returns True if successful, False if not."""
+412        query = f"update {table} set {column_to_update} = ?"
+413        conditions = ""
+414        if match_criteria:
+415            if self.count(table, match_criteria) == 0:
+416                self.logger.info(
+417                    f"Couldn't find matching records in {table} table to
 update to '{new_value}'"
-423                )
-424                return False
-425            conditions = self._get_conditions(match_criteria)
-426            query += f" where {conditions}"
-427        else:
-428            conditions = None
-429        try:
-430            self.cursor.execute(
-431                query,
-432                (new_value,),
-433            )
-434            self.logger.info(
-435                f'Updated "{column_to_update}" in "{table}" table to "
+418                )
+419                return False
+420            conditions = self._get_conditions(match_criteria)
+421            query += f" where {conditions}"
+422        else:
+423            conditions = None
+424        try:
+425            self.cursor.execute(
+426                query,
+427                (new_value,),
+428            )
+429            self.logger.info(
+430                f'Updated "{column_to_update}" in "{table}" table to "
 {new_value}" where {conditions}'
-436            )
-437            return True
-438        except UnboundLocalError:
-439            table_filter_string = "\n".join(
-440                table_filter for table_filter in match_criteria
-441            )
-442            self.logger.error(
-443                f"No records found matching filters: {table_filter_string}"
-444            )
-445            return False
-446        except Exception as e:
-447            self.logger.error(
-448                f'Failed to update "{column_to_update}" in "{table}" table
+431            )
+432            return True
+433        except Exception as e:
+434            self.logger.error(
+435                f'Failed to update "{column_to_update}" in "{table}" table
 to "{new_value}" where {conditions}"\n{e}'
-449            )
-450            return False
-451
-452    @_connect
-453    def drop_table(self, table: str) -> bool:
-454        """Drop a table from the database.
-455
-456        Returns True if successful, False if not."""
-457        try:
-458            self.cursor.execute(f"drop Table {table}")
-459            self.logger.info(f'Dropped table "{table}"')
-460        except Exception as e:
-461            print(e)
-462            self.logger.error(f'Failed to drop table "{table}"')
-463
-464    @_connect
-465    def add_column(
-466        self, table: str, column: str, _type: str, default_value: str = None
-467    ):
-468        """Add a new column to table.
-469
-470        :param column: Name of the column to add.
-471
-472        :param _type: The data type of the new column.
-473
-474        :param default_value: Optional default value for the column."""
-475        try:
-476            if default_value:
-477                self.cursor.execute(
-478                    f"alter table {table} add column {column} {_type}
+436            )
+437            return False
+438
+439    @_connect
+440    def drop_table(self, table: str) -> bool:
+441        """Drop a table from the database.
+442
+443        Returns True if successful, False if not."""
+444        try:
+445            self.cursor.execute(f"drop Table {table}")
+446            self.logger.info(f'Dropped table "{table}"')
+447            return True
+448        except Exception as e:
+449            print(e)
+450            self.logger.error(f'Failed to drop table "{table}"')
+451            return False
+452
+453    @_connect
+454    def add_column(
+455        self, table: str, column: str, _type: str, default_value: str | None
+= None
+456    ):
+457        """Add a new column to table.
+458
+459        :param column: Name of the column to add.
+460
+461        :param _type: The data type of the new column.
+462
+463        :param default_value: Optional default value for the column."""
+464        try:
+465            if default_value:
+466                self.cursor.execute(
+467                    f"alter table {table} add column {column} {_type}
 default {default_value}"
-479                )
-480            else:
-481                self.cursor.execute(f"alter table {table} add column
+468                )
+469            else:
+470                self.cursor.execute(f"alter table {table} add column
 {column} {_type}")
-482            self.logger.info(f'Added column "{column}" to "{table}" table.')
-483        except Exception as e:
-484            self.logger.error(f'Failed to add column "{column}" to "{table}"
+471            self.logger.info(f'Added column "{column}" to "{table}" table.')
+472        except Exception as e:
+473            self.logger.error(f'Failed to add column "{column}" to "{table}"
 table.')
+474
+475    @staticmethod
+476    def data_to_string(
+477        data: list[dict], sort_key: str | None = None, wrap_to_terminal:
+bool = True
+478    ) -> str:
+479        """Uses tabulate to produce pretty string output
+480        from a list of dictionaries.
+481
+482        :param data: Assumes all dictionaries in list have the same set of
+keys.
+483
+484        :param sort_key: Optional dictionary key to sort data with.
 485
-486    @staticmethod
-487    def data_to_string(
-488        data: list[dict], sort_key: str = None, wrap_to_terminal: bool =
+486        :param wrap_to_terminal: If True, the table width will be wrapped
+487        to fit within the current terminal window. Set to False
+488        if the output is going into something like a txt file."""
+489        return data_to_string(data, sort_key, wrap_to_terminal)
+490
+491
+492def data_to_string(
+493    data: list[dict], sort_key: str | None = None, wrap_to_terminal: bool =
 True
-489    ) -> str:
-490        """Uses tabulate to produce pretty string output
-491        from a list of dictionaries.
-492
-493        :param data: Assumes all dictionaries in list have the same set of
-keys.
-494
-495        :param sort_key: Optional dictionary key to sort data with.
+494) -> str:
+495    """Use tabulate to produce grid output from a list of dictionaries.
 496
-497        :param wrap_to_terminal: If True, the table width will be wrapped
-498        to fit within the current terminal window. Set to False
-499        if the output is going into something like a txt file."""
-500        return data_to_string(data, sort_key, wrap_to_terminal)
-501
-502
-503def data_to_string(
-504    data: list[dict], sort_key: str = None, wrap_to_terminal: bool = True
-505) -> str:
-506    """Use tabulate to produce grid output from a list of dictionaries.
-507
-508    :param data: Assumes all dictionaries in list have the same set of keys.
-509
-510    :param sort_key: Optional dictionary key to sort data with.
-511
-512    :param wrap_to_terminal: If True, the column widths will be reduced so
+497    :param data: Assumes all dictionaries in list have the same set of keys.
+498
+499    :param sort_key: Optional dictionary key to sort data with.
+500
+501    :param wrap_to_terminal: If True, the column widths will be reduced so
 the grid fits
-513    within the current terminal window without wrapping. If the column
+502    within the current terminal window without wrapping. If the column
 widths have reduced to 1
-514    and the grid is still too wide, str(data) will be returned."""
-515    if len(data) == 0:
-516        return ""
-517    if sort_key:
-518        data = sorted(data, key=lambda d: d[sort_key])
-519    for i, d in enumerate(data):
-520        for k in d:
-521            data[i][k] = str(data[i][k])
-522
-523    too_wide = True
-524    terminal_width = os.get_terminal_size().columns
-525    max_col_widths = terminal_width
-526    # Make an output with effectively unrestricted column widths
-527    # to see if shrinking is necessary
-528    output = tabulate(
-529        data,
-530        headers="keys",
-531        disable_numparse=True,
-532        tablefmt="grid",
-533        maxcolwidths=max_col_widths,
-534    )
-535    current_width = output.index("\n")
-536    if current_width < terminal_width:
-537        too_wide = False
-538    if wrap_to_terminal and too_wide:
-539        print("Resizing grid to fit within the terminal...")
-540        previous_col_widths = max_col_widths
-541        acceptable_width = terminal_width - 10
-542        while too_wide and max_col_widths > 1:
-543            if current_width > terminal_width:
-544                previous_col_widths = max_col_widths
-545                max_col_widths = int(max_col_widths * 0.5)
-546            elif current_width < terminal_width:
-547                # Without lowering acceptable_width, this condition will
+503    and the grid is still too wide, str(data) will be returned."""
+504    if len(data) == 0:
+505        return ""
+506    if sort_key:
+507        data = sorted(data, key=lambda d: d[sort_key])
+508    for i, d in enumerate(data):
+509        for k in d:
+510            data[i][k] = str(data[i][k])
+511
+512    too_wide = True
+513    terminal_width = os.get_terminal_size().columns
+514    max_col_widths = terminal_width
+515    # Make an output with effectively unrestricted column widths
+516    # to see if shrinking is necessary
+517    output = tabulate(
+518        data,
+519        headers="keys",
+520        disable_numparse=True,
+521        tablefmt="grid",
+522        maxcolwidths=max_col_widths,
+523    )
+524    current_width = output.index("\n")
+525    if current_width < terminal_width:
+526        too_wide = False
+527    if wrap_to_terminal and too_wide:
+528        print("Resizing grid to fit within the terminal...")
+529        previous_col_widths = max_col_widths
+530        acceptable_width = terminal_width - 10
+531        while too_wide and max_col_widths > 1:
+532            if current_width > terminal_width:
+533                previous_col_widths = max_col_widths
+534                max_col_widths = int(max_col_widths * 0.5)
+535            elif current_width < terminal_width:
+536                # Without lowering acceptable_width, this condition will
 cause infinite loop
-548                if max_col_widths == previous_col_widths - 1:
-549                    acceptable_width -= 10
-550                max_col_widths = int(
-551                    max_col_widths + (0.5 * (previous_col_widths -
+537                if max_col_widths == previous_col_widths - 1:
+538                    acceptable_width -= 10
+539                max_col_widths = int(
+540                    max_col_widths + (0.5 * (previous_col_widths -
 max_col_widths))
-552                )
-553            output = tabulate(
-554                data,
-555                headers="keys",
-556                disable_numparse=True,
-557                tablefmt="grid",
-558                maxcolwidths=max_col_widths,
-559            )
-560            current_width = output.index("\n")
-561            if acceptable_width < current_width < terminal_width:
-562                too_wide = False
-563        if too_wide:
-564            print("Couldn't resize grid to fit within the terminal.")
-565            return str(data)
-566    return output
+541                )
+542            output = tabulate(
+543                data,
+544                headers="keys",
+545                disable_numparse=True,
+546                tablefmt="grid",
+547                maxcolwidths=max_col_widths,
+548            )
+549            current_width = output.index("\n")
+550            if acceptable_width < current_width < terminal_width:
+551                too_wide = False
+552        if too_wide:
+553            print("Couldn't resize grid to fit within the terminal.")
+554            return str(data)
+555    return output
   ⁰
 class DataBased: View Source
 _27class DataBased:
 _28    """Sqli wrapper so queries don't need to be written except table
 definitions.
 _29
 _30    Supports saving and reading dates as datetime objects.
 _31
 _32    Supports using a context manager."""
 _33
 _34    def __init__(
 _35        self,
-_36        dbpath: str | Path,
+_36        dbpath: str | Pathier,
 _37        logger_encoding: str = "utf-8",
 _38        logger_message_format: str = "{levelname}|-|{asctime}|-|{message}",
 _39    ):
 _40        """
 _41        :param dbpath: String or Path object to database file.
 _42        If a relative path is given, it will be relative to the
 _43        current working directory. The log file will be saved to the
 _44        same directory.
 _45
 _46        :param logger_message_format: '{' style format string
 _47        for the logger object."""
-_48        self.dbpath = Path(dbpath)
-_49        self.dbname = Path(dbpath).name
+_48        self.dbpath = Pathier(dbpath)
+_49        self.dbname = Pathier(dbpath).name
 _50        self.dbpath.parent.mkdir(parents=True, exist_ok=True)
 _51        self._logger_init(
 _52            encoding=logger_encoding, message_format=logger_message_format
 _53        )
 _54        self.connection_open = False
-_55        self.create_manager()
-_56
-_57    def __enter__(self):
-_58        self.open()
-_59        return self
-_60
-_61    def __exit__(self, exception_type, exception_value,
+_55
+_56    def __enter__(self):
+_57        self.open()
+_58        return self
+_59
+_60    def __exit__(self, exception_type, exception_value,
 exception_traceback):
-_62        self.close()
-_63
-_64    def create_manager(self):
-_65        """Create dbmanager.py in the same directory
-_66        as the database file if it doesn't exist."""
-_67        manager_path = self.dbpath.parent / "dbmanager.py"
-_68        if not manager_path.exists():
-_69            manager_template = (Path(__file__).parent /
-"dbmanager.py").read_text()
-_70            manager_path.write_text(manager_template.replace("$dbname",
-self.dbname))
-_71
-_72    def open(self):
-_73        """Open connection to db."""
-_74        self.connection = sqlite3.connect(
-_75            self.dbpath,
-_76            detect_types=sqlite3.PARSE_DECLTYPES | sqlite3.PARSE_COLNAMES,
-_77            timeout=10,
-_78        )
-_79        self.connection.execute("pragma foreign_keys = 1")
-_80        self.cursor = self.connection.cursor()
-_81        self.connection_open = True
-_82
-_83    def close(self):
-_84        """Save and close connection to db.
-_85
-_86        Call this as soon as you are done using the database if you have
-_87        multiple threads or processes using the same database."""
-_88        if self.connection_open:
-_89            self.connection.commit()
-_90            self.connection.close()
-_91            self.connection_open = False
-_92
-_93    def _logger_init(
-_94        self,
-_95        message_format: str = "{levelname}|-|{asctime}|-|{message}",
-_96        encoding: str = "utf-8",
-_97    ):
-_98        """:param message_format: '{' style format string"""
-_99        self.logger = logging.getLogger(self.dbname)
-100        if not self.logger.hasHandlers():
-101            handler = logging.FileHandler(
-102                str(self.dbpath).replace(".", "") + ".log",
+_61        self.close()
+_62
+_63    def open(self):
+_64        """Open connection to db."""
+_65        self.connection = sqlite3.connect(
+_66            self.dbpath,
+_67            detect_types=sqlite3.PARSE_DECLTYPES | sqlite3.PARSE_COLNAMES,
+_68            timeout=10,
+_69        )
+_70        self.connection.execute("pragma foreign_keys = 1")
+_71        self.cursor = self.connection.cursor()
+_72        self.connection_open = True
+_73
+_74    def close(self):
+_75        """Save and close connection to db.
+_76
+_77        Call this as soon as you are done using the database if you have
+_78        multiple threads or processes using the same database."""
+_79        if self.connection_open:
+_80            self.connection.commit()
+_81            self.connection.close()
+_82            self.connection_open = False
+_83
+_84    def _logger_init(
+_85        self,
+_86        message_format: str = "{levelname}|-|{asctime}|-|{message}",
+_87        encoding: str = "utf-8",
+_88    ):
+_89        """:param message_format: '{' style format string"""
+_90        self.logger = logging.getLogger(self.dbname)
+_91        if not self.logger.hasHandlers():
+_92            handler = logging.FileHandler(
+_93                str(self.dbpath).replace(".", "") + ".log",
 encoding=encoding
-103            )
-104            handler.setFormatter(
-105                logging.Formatter(
-106                    message_format, style="{", datefmt="%m/%d/%Y %I:%M:%S
+_94            )
+_95            handler.setFormatter(
+_96                logging.Formatter(
+_97                    message_format, style="{", datefmt="%m/%d/%Y %I:%M:%S
 %p"
-107                )
-108            )
-109            self.logger.addHandler(handler)
-110            self.logger.setLevel(logging.INFO)
-111
-112    def _get_dict(
-113        self, table: str, values: list, columns_to_return: list[str] = None
-114    ) -> dict:
-115        """Converts the values of a row into a dictionary with column names
+_98                )
+_99            )
+100            self.logger.addHandler(handler)
+101            self.logger.setLevel(logging.INFO)
+102
+103    def _get_dict(
+104        self, table: str, values: list, columns_to_return: list[str] | None
+= None
+105    ) -> dict:
+106        """Converts the values of a row into a dictionary with column names
 as keys.
-116
-117        :param table: The table that values were pulled from.
-118
-119        :param values: List of values expected to be the same quantity
-120        and in the same order as the column names of table.
-121
-122        :param columns_to_return: An optional list of column names.
-123        If given, only these columns will be included in the returned
+107
+108        :param table: The table that values were pulled from.
+109
+110        :param values: List of values expected to be the same quantity
+111        and in the same order as the column names of table.
+112
+113        :param columns_to_return: An optional list of column names.
+114        If given, only these columns will be included in the returned
 dictionary.
-124        Otherwise all columns and values are returned."""
-125        return {
-126            column: value
-127            for column, value in zip(self.get_column_names(table), values)
-128            if not columns_to_return or column in columns_to_return
-129        }
+115        Otherwise all columns and values are returned."""
+116        return {
+117            column: value
+118            for column, value in zip(self.get_column_names(table), values)
+119            if not columns_to_return or column in columns_to_return
+120        }
+121
+122    def _get_conditions(
+123        self, match_criteria: list[tuple] | dict, exact_match: bool = True
+124    ) -> str:
+125        """Builds and returns the conditional portion of a query.
+126
+127        :param match_criteria: Can be a list of 2-tuples where each
+128        tuple is (columnName, rowValue) or a dictionary where
+129        keys are column names and values are row values.
 130
-131    def _get_conditions(
-132        self, match_criteria: list[tuple] | dict, exact_match: bool = True
-133    ) -> str:
-134        """Builds and returns the conditional portion of a query.
+131        :param exact_match: If False, the rowValue for a give column
+132        will be matched as a substring.
+133
+134        Usage e.g.:
 135
-136        :param match_criteria: Can be a list of 2-tuples where each
-137        tuple is (columnName, rowValue) or a dictionary where
-138        keys are column names and values are row values.
-139
-140        :param exact_match: If False, the rowValue for a give column
-141        will be matched as a substring.
-142
-143        Usage e.g.:
-144
-145        self.cursor.execute(f'select * from {table} where {conditions}')"""
-146        if type(match_criteria) == dict:
-147            match_criteria = [(k, v) for k, v in match_criteria.items()]
-148        if exact_match:
-149            conditions = " and ".join(
-150                f'"{column_row[0]}" = "{column_row[1]}"'
-151                for column_row in match_criteria
-152            )
-153        else:
-154            conditions = " and ".join(
-155                f'"{column_row[0]}" like "%{column_row[1]}%"'
-156                for column_row in match_criteria
-157            )
-158        return f"({conditions})"
-159
-160    @_connect
-161    def query(self, query_) -> list[Any]:
-162        """Execute an arbitrary query and
-163        return the results."""
-164        self.cursor.execute(query_)
-165        return self.cursor.fetchall()
-166
-167    @_connect
-168    def create_tables(self, table_querys: list[str] = []):
-169        """Create tables if they don't exist.
-170
-171        :param table_querys: Each query should be
-172        in the form 'tableName(columnDefinitions)'"""
-173        if len(table_querys) > 0:
-174            table_names = self.get_table_names()
-175            for table in table_querys:
-176                if table.split("(")[0].strip() not in table_names:
-177                    self.cursor.execute(f"create table {table}")
-178                    self.logger.info(f'{table.split("(")[0]} table
+136        self.cursor.execute(f'select * from {table} where {conditions}')"""
+137        if type(match_criteria) == dict:
+138            match_criteria = [(k, v) for k, v in match_criteria.items()]
+139        if exact_match:
+140            conditions = " and ".join(
+141                f'"{column_row[0]}" = "{column_row[1]}"'
+142                for column_row in match_criteria
+143            )
+144        else:
+145            conditions = " and ".join(
+146                f'"{column_row[0]}" like "%{column_row[1]}%"'
+147                for column_row in match_criteria
+148            )
+149        return f"({conditions})"
+150
+151    @_connect
+152    def query(self, query_) -> list[Any]:
+153        """Execute an arbitrary query and
+154        return the results."""
+155        self.cursor.execute(query_)
+156        return self.cursor.fetchall()
+157
+158    @_connect
+159    def create_tables(self, table_querys: list[str] = []):
+160        """Create tables if they don't exist.
+161
+162        :param table_querys: Each query should be
+163        in the form 'tableName(columnDefinitions)'"""
+164        if len(table_querys) > 0:
+165            table_names = self.get_table_names()
+166            for table in table_querys:
+167                if table.split("(")[0].strip() not in table_names:
+168                    self.cursor.execute(f"create table {table}")
+169                    self.logger.info(f'{table.split("(")[0]} table
 created.')
-179
-180    @_connect
-181    def create_table(self, table: str, column_defs: list[str]):
-182        """Create a table if it doesn't exist.
-183
-184        :param table: Name of the table to create.
-185
-186        :param column_defs: List of column definitions in
-187        proper Sqlite3 sytax.
-188        i.e. "columnName text unique" or "columnName int primary key"
+170
+171    @_connect
+172    def create_table(self, table: str, column_defs: list[str]):
+173        """Create a table if it doesn't exist.
+174
+175        :param table: Name of the table to create.
+176
+177        :param column_defs: List of column definitions in
+178        proper Sqlite3 sytax.
+179        i.e. "columnName text unique" or "columnName int primary key"
 etc."""
-189        if table not in self.get_table_names():
-190            query = f"create table {table}({', '.join(column_defs)})"
-191            self.cursor.execute(query)
-192            self.logger.info(f"'{table}' table created.")
-193
-194    @_connect
-195    def get_table_names(self) -> list[str]:
-196        """Returns a list of table names from database."""
-197        self.cursor.execute(
-198            'select name from sqlite_Schema where type = "table" and name
+180        if table not in self.get_table_names():
+181            query = f"create table {table}({', '.join(column_defs)})"
+182            self.cursor.execute(query)
+183            self.logger.info(f"'{table}' table created.")
+184
+185    @_connect
+186    def get_table_names(self) -> list[str]:
+187        """Returns a list of table names from database."""
+188        self.cursor.execute(
+189            'select name from sqlite_Schema where type = "table" and name
 not like "sqlite_%"'
-199        )
-200        return [result[0] for result in self.cursor.fetchall()]
-201
-202    @_connect
-203    def get_column_names(self, table: str) -> list[str]:
-204        """Return a list of column names from a table."""
-205        self.cursor.execute(f"select * from {table} where 1=0")
-206        return [description[0] for description in self.cursor.description]
+190        )
+191        return [result[0] for result in self.cursor.fetchall()]
+192
+193    @_connect
+194    def get_column_names(self, table: str) -> list[str]:
+195        """Return a list of column names from a table."""
+196        self.cursor.execute(f"select * from {table} where 1=0")
+197        return [description[0] for description in self.cursor.description]
+198
+199    @_connect
+200    def count(
+201        self,
+202        table: str,
+203        match_criteria: list[tuple] | dict | None = None,
+204        exact_match: bool = True,
+205    ) -> int:
+206        """Return number of items in table.
 207
-208    @_connect
-209    def count(
-210        self,
-211        table: str,
-212        match_criteria: list[tuple] | dict = None,
-213        exact_match: bool = True,
-214    ) -> int:
-215        """Return number of items in table.
-216
-217        :param match_criteria: Can be a list of 2-tuples where each
-218        tuple is (columnName, rowValue) or a dictionary where
-219        keys are column names and values are row values.
-220        If None, all rows from the table will be counted.
-221
-222        :param exact_match: If False, the row value for a give column
-223        in match_criteria will be matched as a substring. Has no effect if
-224        match_criteria is None.
-225        """
-226        query = f"select count(_rowid_) from {table}"
-227        try:
-228            if match_criteria:
-229                self.cursor.execute(
-230                    f"{query} where {self._get_conditions(match_criteria,
+208        :param match_criteria: Can be a list of 2-tuples where each
+209        tuple is (columnName, rowValue) or a dictionary where
+210        keys are column names and values are row values.
+211        If None, all rows from the table will be counted.
+212
+213        :param exact_match: If False, the row value for a give column
+214        in match_criteria will be matched as a substring. Has no effect if
+215        match_criteria is None.
+216        """
+217        query = f"select count(_rowid_) from {table}"
+218        try:
+219            if match_criteria:
+220                self.cursor.execute(
+221                    f"{query} where {self._get_conditions(match_criteria,
 exact_match)}"
-231                )
-232            else:
-233                self.cursor.execute(f"{query}")
-234            return self.cursor.fetchone()[0]
-235        except:
-236            return 0
-237
-238    @_connect
-239    def add_row(self, table: str, values: tuple[any], columns: tuple[str] =
-None):
-240        """Add row of values to table.
-241
-242        :param table: The table to insert into.
-243
-244        :param values: A tuple of values to be inserted into the table.
-245
-246        :param columns: If None, values param is expected to supply
-247        a value for every column in the table. If columns is
-248        provided, it should contain the same number of elements as
+222                )
+223            else:
+224                self.cursor.execute(f"{query}")
+225            return self.cursor.fetchone()[0]
+226        except:
+227            return 0
+228
+229    @_connect
+230    def add_row(
+231        self, table: str, values: tuple[Any], columns: tuple[str] | None =
+None
+232    ):
+233        """Add row of values to table.
+234
+235        :param table: The table to insert into.
+236
+237        :param values: A tuple of values to be inserted into the table.
+238
+239        :param columns: If None, values param is expected to supply
+240        a value for every column in the table. If columns is
+241        provided, it should contain the same number of elements as
 values."""
-249        parameterizer = ", ".join("?" for _ in values)
-250        logger_values = ", ".join(str(value) for value in values)
-251        try:
-252            if columns:
-253                columns = ", ".join(column for column in columns)
-254                self.cursor.execute(
-255                    f"insert into {table} ({columns}) values(
-{parameterizer})", values
-256                )
-257            else:
-258                self.cursor.execute(
-259                    f"insert into {table} values({parameterizer})", values
+242        parameterizer = ", ".join("?" for _ in values)
+243        logger_values = ", ".join(str(value) for value in values)
+244        try:
+245            if columns:
+246                columns_query = ", ".join(column for column in columns)
+247                self.cursor.execute(
+248                    f"insert into {table} ({columns_query}) values(
+{parameterizer})",
+249                    values,
+250                )
+251            else:
+252                self.cursor.execute(
+253                    f"insert into {table} values({parameterizer})", values
+254                )
+255            self.logger.info(f'Added "{logger_values}" to {table} table.')
+256        except Exception as e:
+257            if "constraint" not in str(e).lower():
+258                self.logger.exception(
+259                    f'Error adding "{logger_values}" to {table} table.'
 260                )
-261            self.logger.info(f'Added "{logger_values}" to {table} table.')
-262        except Exception as e:
-263            if "constraint" not in str(e).lower():
-264                self.logger.exception(
-265                    f'Error adding "{logger_values}" to {table} table.'
-266                )
-267            else:
-268                self.logger.debug(str(e))
-269
-270    @_connect
-271    def get_rows(
-272        self,
-273        table: str,
-274        match_criteria: list[tuple] | dict = None,
-275        exact_match: bool = True,
-276        sort_by_column: str = None,
-277        columns_to_return: list[str] = None,
-278        return_as_dataframe: bool = False,
-279        values_only: bool = False,
-280        order_by: str = None,
-281        limit: str | int = None,
-282    ) -> list[dict] | list[tuple] | pandas.DataFrame:
-283        """Returns rows from table as a list of dictionaries
-284        where the key-value pairs of the dictionaries are
-285        column name: row value.
-286
-287        :param match_criteria: Can be a list of 2-tuples where each
-288        tuple is (columnName, rowValue) or a dictionary where
-289        keys are column names and values are row values.
-290
-291        :param exact_match: If False, the rowValue for a give column
-292        will be matched as a substring.
-293
-294        :param sort_by_column: A column name to sort the results by.
-295        This will sort results in Python after retrieving them from the db.
-296        Use the 'order_by' param to use SQLite engine for ordering.
-297
-298        :param columns_to_return: Optional list of column names.
-299        If provided, the elements returned by get_rows() will
-300        only contain the provided columns. Otherwise every column
-301        in the row is returned.
-302
-303        :param return_as_dataframe: If True,
-304        the results will be returned as a pandas.DataFrame object.
-305
-306        :param values_only: Return the results as a list of tuples
-307        instead of a list of dictionaries that have column names as keys.
-308        The results will still be sorted according to sort_by_column if
-309        one is provided.
-310
-311        :param order_by: If given, a 'order by {order_by}' clause
-312        will be added to the select query.
-313
-314        :param limit: If given, a 'limit {limit}' clause will be
-315        added to the select query.
-316        """
-317
-318        if type(columns_to_return) is str:
-319            columns_to_return = [columns_to_return]
-320        query = f"select * from {table}"
-321        matches = []
-322        if match_criteria:
-323            query += f" where {self._get_conditions(match_criteria,
+261            else:
+262                self.logger.debug(str(e))
+263
+264    @_connect
+265    def get_rows(
+266        self,
+267        table: str,
+268        match_criteria: list[tuple] | dict | None = None,
+269        exact_match: bool = True,
+270        sort_by_column: str | None = None,
+271        columns_to_return: list[str] | None = None,
+272        return_as_dataframe: bool = False,
+273        values_only: bool = False,
+274        order_by: str | None = None,
+275        limit: str | int | None = None,
+276    ) -> list[dict] | list[tuple] | pandas.DataFrame:
+277        """Returns rows from table as a list of dictionaries
+278        where the key-value pairs of the dictionaries are
+279        column name: row value.
+280
+281        :param match_criteria: Can be a list of 2-tuples where each
+282        tuple is (columnName, rowValue) or a dictionary where
+283        keys are column names and values are row values.
+284
+285        :param exact_match: If False, the rowValue for a give column
+286        will be matched as a substring.
+287
+288        :param sort_by_column: A column name to sort the results by.
+289        This will sort results in Python after retrieving them from the db.
+290        Use the 'order_by' param to use SQLite engine for ordering.
+291
+292        :param columns_to_return: Optional list of column names.
+293        If provided, the elements returned by get_rows() will
+294        only contain the provided columns. Otherwise every column
+295        in the row is returned.
+296
+297        :param return_as_dataframe: If True,
+298        the results will be returned as a pandas.DataFrame object.
+299
+300        :param values_only: Return the results as a list of tuples
+301        instead of a list of dictionaries that have column names as keys.
+302        The results will still be sorted according to sort_by_column if
+303        one is provided.
+304
+305        :param order_by: If given, a 'order by {order_by}' clause
+306        will be added to the select query.
+307
+308        :param limit: If given, a 'limit {limit}' clause will be
+309        added to the select query.
+310        """
+311
+312        if type(columns_to_return) is str:
+313            columns_to_return = [columns_to_return]
+314        query = f"select * from {table}"
+315        matches = []
+316        if match_criteria:
+317            query += f" where {self._get_conditions(match_criteria,
 exact_match)}"
-324        if order_by:
-325            query += f" order by {order_by}"
-326        if limit:
-327            query += f" limit {limit}"
-328        query += ";"
-329        self.cursor.execute(query)
-330        matches = self.cursor.fetchall()
-331        results = [self._get_dict(table, match, columns_to_return) for match
+318        if order_by:
+319            query += f" order by {order_by}"
+320        if limit:
+321            query += f" limit {limit}"
+322        query += ";"
+323        self.cursor.execute(query)
+324        matches = self.cursor.fetchall()
+325        results = [self._get_dict(table, match, columns_to_return) for match
 in matches]
-332        if sort_by_column:
-333            results = sorted(results, key=lambda x: x[sort_by_column])
-334        if return_as_dataframe:
-335            return pandas.DataFrame(results)
-336        if values_only:
-337            return [tuple(row.values()) for row in results]
-338        else:
-339            return results
-340
-341    @_connect
-342    def find(
-343        self, table: str, query_string: str, columns: list[str] = None
-344    ) -> tuple[dict]:
-345        """Search for rows that contain query_string as a substring
-346        of any column.
-347
-348        :param table: The table to search.
-349
-350        :param query_string: The substring to search for in all columns.
-351
-352        :param columns: A list of columns to search for query_string.
-353        If None, all columns in the table will be searched.
-354        """
-355        if type(columns) is str:
-356            columns = [columns]
-357        results = []
-358        if not columns:
-359            columns = self.get_column_names(table)
-360        for column in columns:
-361            results.extend(
-362                [
-363                    row
-364                    for row in self.get_rows(
-365                        table, [(column, query_string)], exact_match=False
-366                    )
-367                    if row not in results
-368                ]
-369            )
-370        return results
-371
-372    @_connect
-373    def delete(
-374        self, table: str, match_criteria: list[tuple] | dict, exact_match:
+326        if sort_by_column:
+327            results = sorted(results, key=lambda x: x[sort_by_column])
+328        if return_as_dataframe:
+329            return pandas.DataFrame(results)
+330        if values_only:
+331            return [tuple(row.values()) for row in results]
+332        else:
+333            return results
+334
+335    @_connect
+336    def find(
+337        self, table: str, query_string: str, columns: list[str] | None =
+None
+338    ) -> list[dict]:
+339        """Search for rows that contain query_string as a substring
+340        of any column.
+341
+342        :param table: The table to search.
+343
+344        :param query_string: The substring to search for in all columns.
+345
+346        :param columns: A list of columns to search for query_string.
+347        If None, all columns in the table will be searched.
+348        """
+349        if type(columns) is str:
+350            columns = [columns]
+351        results = []
+352        if not columns:
+353            columns = self.get_column_names(table)
+354        for column in columns:
+355            results.extend(
+356                [
+357                    row
+358                    for row in self.get_rows(
+359                        table, [(column, query_string)], exact_match=False
+360                    )
+361                    if row not in results
+362                ]
+363            )
+364        return results
+365
+366    @_connect
+367    def delete(
+368        self, table: str, match_criteria: list[tuple] | dict, exact_match:
 bool = True
-375    ) -> int:
-376        """Delete records from table.
+369    ) -> int:
+370        """Delete records from table.
+371
+372        Returns number of deleted records.
+373
+374        :param match_criteria: Can be a list of 2-tuples where each
+375        tuple is (columnName, rowValue) or a dictionary where
+376        keys are column names and values are row values.
 377
-378        Returns number of deleted records.
-379
-380        :param match_criteria: Can be a list of 2-tuples where each
-381        tuple is (columnName, rowValue) or a dictionary where
-382        keys are column names and values are row values.
-383
-384        :param exact_match: If False, the rowValue for a give column
-385        will be matched as a substring.
-386        """
-387        num_matches = self.count(table, match_criteria, exact_match)
-388        conditions = self._get_conditions(match_criteria, exact_match)
-389        try:
-390            self.cursor.execute(f"delete from {table} where {conditions}")
-391            self.logger.info(
-392                f'Deleted {num_matches} from "{table}" where {conditions}".'
-393            )
-394            return num_matches
-395        except Exception as e:
-396            self.logger.debug(f'Error deleting from "{table}" where
+378        :param exact_match: If False, the rowValue for a give column
+379        will be matched as a substring.
+380        """
+381        num_matches = self.count(table, match_criteria, exact_match)
+382        conditions = self._get_conditions(match_criteria, exact_match)
+383        try:
+384            self.cursor.execute(f"delete from {table} where {conditions}")
+385            self.logger.info(
+386                f'Deleted {num_matches} from "{table}" where {conditions}".'
+387            )
+388            return num_matches
+389        except Exception as e:
+390            self.logger.debug(f'Error deleting from "{table}" where
 {conditions}.\n{e}')
-397            return 0
-398
-399    @_connect
-400    def update(
-401        self,
-402        table: str,
-403        column_to_update: str,
-404        new_value: Any,
-405        match_criteria: list[tuple] | dict = None,
-406    ) -> bool:
-407        """Update row value for entry matched with match_criteria.
-408
-409        :param column_to_update: The column to be updated in the matched
+391            return 0
+392
+393    @_connect
+394    def update(
+395        self,
+396        table: str,
+397        column_to_update: str,
+398        new_value: Any,
+399        match_criteria: list[tuple] | dict | None = None,
+400    ) -> bool:
+401        """Update row value for entry matched with match_criteria.
+402
+403        :param column_to_update: The column to be updated in the matched
 row.
-410
-411        :param new_value: The new value to insert.
-412
-413        :param match_criteria: Can be a list of 2-tuples where each
-414        tuple is (columnName, rowValue) or a dictionary where
-415        keys are column names and values are row values.
-416        If None, every row will be updated.
-417
-418        Returns True if successful, False if not."""
-419        query = f"update {table} set {column_to_update} = ?"
-420        if match_criteria:
-421            if self.count(table, match_criteria) == 0:
-422                self.logger.info(
-423                    f"Couldn't find matching records in {table} table to
+404
+405        :param new_value: The new value to insert.
+406
+407        :param match_criteria: Can be a list of 2-tuples where each
+408        tuple is (columnName, rowValue) or a dictionary where
+409        keys are column names and values are row values.
+410        If None, every row will be updated.
+411
+412        Returns True if successful, False if not."""
+413        query = f"update {table} set {column_to_update} = ?"
+414        conditions = ""
+415        if match_criteria:
+416            if self.count(table, match_criteria) == 0:
+417                self.logger.info(
+418                    f"Couldn't find matching records in {table} table to
 update to '{new_value}'"
-424                )
-425                return False
-426            conditions = self._get_conditions(match_criteria)
-427            query += f" where {conditions}"
-428        else:
-429            conditions = None
-430        try:
-431            self.cursor.execute(
-432                query,
-433                (new_value,),
-434            )
-435            self.logger.info(
-436                f'Updated "{column_to_update}" in "{table}" table to "
+419                )
+420                return False
+421            conditions = self._get_conditions(match_criteria)
+422            query += f" where {conditions}"
+423        else:
+424            conditions = None
+425        try:
+426            self.cursor.execute(
+427                query,
+428                (new_value,),
+429            )
+430            self.logger.info(
+431                f'Updated "{column_to_update}" in "{table}" table to "
 {new_value}" where {conditions}'
-437            )
-438            return True
-439        except UnboundLocalError:
-440            table_filter_string = "\n".join(
-441                table_filter for table_filter in match_criteria
-442            )
-443            self.logger.error(
-444                f"No records found matching filters: {table_filter_string}"
-445            )
-446            return False
-447        except Exception as e:
-448            self.logger.error(
-449                f'Failed to update "{column_to_update}" in "{table}" table
+432            )
+433            return True
+434        except Exception as e:
+435            self.logger.error(
+436                f'Failed to update "{column_to_update}" in "{table}" table
 to "{new_value}" where {conditions}"\n{e}'
-450            )
-451            return False
-452
-453    @_connect
-454    def drop_table(self, table: str) -> bool:
-455        """Drop a table from the database.
-456
-457        Returns True if successful, False if not."""
-458        try:
-459            self.cursor.execute(f"drop Table {table}")
-460            self.logger.info(f'Dropped table "{table}"')
-461        except Exception as e:
-462            print(e)
-463            self.logger.error(f'Failed to drop table "{table}"')
-464
-465    @_connect
-466    def add_column(
-467        self, table: str, column: str, _type: str, default_value: str = None
-468    ):
-469        """Add a new column to table.
-470
-471        :param column: Name of the column to add.
-472
-473        :param _type: The data type of the new column.
-474
-475        :param default_value: Optional default value for the column."""
-476        try:
-477            if default_value:
-478                self.cursor.execute(
-479                    f"alter table {table} add column {column} {_type}
+437            )
+438            return False
+439
+440    @_connect
+441    def drop_table(self, table: str) -> bool:
+442        """Drop a table from the database.
+443
+444        Returns True if successful, False if not."""
+445        try:
+446            self.cursor.execute(f"drop Table {table}")
+447            self.logger.info(f'Dropped table "{table}"')
+448            return True
+449        except Exception as e:
+450            print(e)
+451            self.logger.error(f'Failed to drop table "{table}"')
+452            return False
+453
+454    @_connect
+455    def add_column(
+456        self, table: str, column: str, _type: str, default_value: str | None
+= None
+457    ):
+458        """Add a new column to table.
+459
+460        :param column: Name of the column to add.
+461
+462        :param _type: The data type of the new column.
+463
+464        :param default_value: Optional default value for the column."""
+465        try:
+466            if default_value:
+467                self.cursor.execute(
+468                    f"alter table {table} add column {column} {_type}
 default {default_value}"
-480                )
-481            else:
-482                self.cursor.execute(f"alter table {table} add column
+469                )
+470            else:
+471                self.cursor.execute(f"alter table {table} add column
 {column} {_type}")
-483            self.logger.info(f'Added column "{column}" to "{table}" table.')
-484        except Exception as e:
-485            self.logger.error(f'Failed to add column "{column}" to "{table}"
+472            self.logger.info(f'Added column "{column}" to "{table}" table.')
+473        except Exception as e:
+474            self.logger.error(f'Failed to add column "{column}" to "{table}"
 table.')
-486
-487    @staticmethod
-488    def data_to_string(
-489        data: list[dict], sort_key: str = None, wrap_to_terminal: bool =
-True
-490    ) -> str:
-491        """Uses tabulate to produce pretty string output
-492        from a list of dictionaries.
-493
-494        :param data: Assumes all dictionaries in list have the same set of
+475
+476    @staticmethod
+477    def data_to_string(
+478        data: list[dict], sort_key: str | None = None, wrap_to_terminal:
+bool = True
+479    ) -> str:
+480        """Uses tabulate to produce pretty string output
+481        from a list of dictionaries.
+482
+483        :param data: Assumes all dictionaries in list have the same set of
 keys.
-495
-496        :param sort_key: Optional dictionary key to sort data with.
-497
-498        :param wrap_to_terminal: If True, the table width will be wrapped
-499        to fit within the current terminal window. Set to False
-500        if the output is going into something like a txt file."""
-501        return data_to_string(data, sort_key, wrap_to_terminal)
+484
+485        :param sort_key: Optional dictionary key to sort data with.
+486
+487        :param wrap_to_terminal: If True, the table width will be wrapped
+488        to fit within the current terminal window. Set to False
+489        if the output is going into something like a txt file."""
+490        return data_to_string(data, sort_key, wrap_to_terminal)
 Sqli wrapper so queries don't need to be written except table definitions.
 Supports saving and reading dates as datetime objects.
 Supports using a context manager.
 ⁰
 DataBased(
-dbpath: str | pathlib.Path,
+dbpath: str | pathier.pathier.Pathier,
 logger_encoding: str = 'utf-8',
 logger_message_format: str = '{levelname}|-|{asctime}|-|{message}') View Source
 34    def __init__(
 35        self,
-36        dbpath: str | Path,
+36        dbpath: str | Pathier,
 37        logger_encoding: str = "utf-8",
 38        logger_message_format: str = "{levelname}|-|{asctime}|-|{message}",
 39    ):
 40        """
 41        :param dbpath: String or Path object to database file.
 42        If a relative path is given, it will be relative to the
 43        current working directory. The log file will be saved to the
 44        same directory.
 45
 46        :param logger_message_format: '{' style format string
 47        for the logger object."""
-48        self.dbpath = Path(dbpath)
-49        self.dbname = Path(dbpath).name
+48        self.dbpath = Pathier(dbpath)
+49        self.dbname = Pathier(dbpath).name
 50        self.dbpath.parent.mkdir(parents=True, exist_ok=True)
 51        self._logger_init(
 52            encoding=logger_encoding, message_format=logger_message_format
 53        )
 54        self.connection_open = False
-55        self.create_manager()
 * Parameters *
     * dbpath: String or Path object to database file. If a relative path is
       given, it will be relative to the current working directory. The log file
       will be saved to the same directory.
     * logger_message_format: '{' style format string for the logger object.
 ⁰
-def create_manager(self): View Source
-64    def create_manager(self):
-65        """Create dbmanager.py in the same directory
-66        as the database file if it doesn't exist."""
-67        manager_path = self.dbpath.parent / "dbmanager.py"
-68        if not manager_path.exists():
-69            manager_template = (Path(__file__).parent /
-"dbmanager.py").read_text()
-70            manager_path.write_text(manager_template.replace("$dbname",
-self.dbname))
-Create dbmanager.py in the same directory as the database file if it doesn't
-exist.
-⁰
 def open(self): View Source
-72    def open(self):
-73        """Open connection to db."""
-74        self.connection = sqlite3.connect(
-75            self.dbpath,
-76            detect_types=sqlite3.PARSE_DECLTYPES | sqlite3.PARSE_COLNAMES,
-77            timeout=10,
-78        )
-79        self.connection.execute("pragma foreign_keys = 1")
-80        self.cursor = self.connection.cursor()
-81        self.connection_open = True
+63    def open(self):
+64        """Open connection to db."""
+65        self.connection = sqlite3.connect(
+66            self.dbpath,
+67            detect_types=sqlite3.PARSE_DECLTYPES | sqlite3.PARSE_COLNAMES,
+68            timeout=10,
+69        )
+70        self.connection.execute("pragma foreign_keys = 1")
+71        self.cursor = self.connection.cursor()
+72        self.connection_open = True
 Open connection to db.
 ⁰
 def close(self): View Source
-83    def close(self):
-84        """Save and close connection to db.
-85
-86        Call this as soon as you are done using the database if you have
-87        multiple threads or processes using the same database."""
-88        if self.connection_open:
-89            self.connection.commit()
-90            self.connection.close()
-91            self.connection_open = False
+74    def close(self):
+75        """Save and close connection to db.
+76
+77        Call this as soon as you are done using the database if you have
+78        multiple threads or processes using the same database."""
+79        if self.connection_open:
+80            self.connection.commit()
+81            self.connection.close()
+82            self.connection_open = False
 Save and close connection to db.
 Call this as soon as you are done using the database if you have multiple
 threads or processes using the same database.
 ⁰
 def query(self, query_) -> list[typing.Any]: View Source
-160    @_connect
-161    def query(self, query_) -> list[Any]:
-162        """Execute an arbitrary query and
-163        return the results."""
-164        self.cursor.execute(query_)
-165        return self.cursor.fetchall()
+151    @_connect
+152    def query(self, query_) -> list[Any]:
+153        """Execute an arbitrary query and
+154        return the results."""
+155        self.cursor.execute(query_)
+156        return self.cursor.fetchall()
 Execute an arbitrary query and return the results.
 ⁰
 def create_tables(self, table_querys: list[str] = []): View Source
-167    @_connect
-168    def create_tables(self, table_querys: list[str] = []):
-169        """Create tables if they don't exist.
-170
-171        :param table_querys: Each query should be
-172        in the form 'tableName(columnDefinitions)'"""
-173        if len(table_querys) > 0:
-174            table_names = self.get_table_names()
-175            for table in table_querys:
-176                if table.split("(")[0].strip() not in table_names:
-177                    self.cursor.execute(f"create table {table}")
-178                    self.logger.info(f'{table.split("(")[0]} table
+158    @_connect
+159    def create_tables(self, table_querys: list[str] = []):
+160        """Create tables if they don't exist.
+161
+162        :param table_querys: Each query should be
+163        in the form 'tableName(columnDefinitions)'"""
+164        if len(table_querys) > 0:
+165            table_names = self.get_table_names()
+166            for table in table_querys:
+167                if table.split("(")[0].strip() not in table_names:
+168                    self.cursor.execute(f"create table {table}")
+169                    self.logger.info(f'{table.split("(")[0]} table
 created.')
 Create tables if they don't exist.
 * Parameters *
     * table_querys: Each query should be in the form 'tableName
       (columnDefinitions)'
 ⁰
 def create_table(self, table: str, column_defs: list[str]): View Source
-180    @_connect
-181    def create_table(self, table: str, column_defs: list[str]):
-182        """Create a table if it doesn't exist.
-183
-184        :param table: Name of the table to create.
-185
-186        :param column_defs: List of column definitions in
-187        proper Sqlite3 sytax.
-188        i.e. "columnName text unique" or "columnName int primary key"
+171    @_connect
+172    def create_table(self, table: str, column_defs: list[str]):
+173        """Create a table if it doesn't exist.
+174
+175        :param table: Name of the table to create.
+176
+177        :param column_defs: List of column definitions in
+178        proper Sqlite3 sytax.
+179        i.e. "columnName text unique" or "columnName int primary key"
 etc."""
-189        if table not in self.get_table_names():
-190            query = f"create table {table}({', '.join(column_defs)})"
-191            self.cursor.execute(query)
-192            self.logger.info(f"'{table}' table created.")
+180        if table not in self.get_table_names():
+181            query = f"create table {table}({', '.join(column_defs)})"
+182            self.cursor.execute(query)
+183            self.logger.info(f"'{table}' table created.")
 Create a table if it doesn't exist.
 * Parameters *
     * table: Name of the table to create.
     * column_defs: List of column definitions in proper Sqlite3 sytax. i.e.
       "columnName text unique" or "columnName int primary key" etc.
 ⁰
 def get_table_names(self) -> list[str]: View Source
-194    @_connect
-195    def get_table_names(self) -> list[str]:
-196        """Returns a list of table names from database."""
-197        self.cursor.execute(
-198            'select name from sqlite_Schema where type = "table" and name
+185    @_connect
+186    def get_table_names(self) -> list[str]:
+187        """Returns a list of table names from database."""
+188        self.cursor.execute(
+189            'select name from sqlite_Schema where type = "table" and name
 not like "sqlite_%"'
-199        )
-200        return [result[0] for result in self.cursor.fetchall()]
+190        )
+191        return [result[0] for result in self.cursor.fetchall()]
 Returns a list of table names from database.
 ⁰
 def get_column_names(self, table: str) -> list[str]: View Source
-202    @_connect
-203    def get_column_names(self, table: str) -> list[str]:
-204        """Return a list of column names from a table."""
-205        self.cursor.execute(f"select * from {table} where 1=0")
-206        return [description[0] for description in self.cursor.description]
+193    @_connect
+194    def get_column_names(self, table: str) -> list[str]:
+195        """Return a list of column names from a table."""
+196        self.cursor.execute(f"select * from {table} where 1=0")
+197        return [description[0] for description in self.cursor.description]
 Return a list of column names from a table.
 ⁰
 def count(
 self,
 table: str,
-match_criteria: list[tuple] | dict = None,
+match_criteria: list[tuple] | dict | None = None,
 exact_match: bool = True) -> int: View Source
-208    @_connect
-209    def count(
-210        self,
-211        table: str,
-212        match_criteria: list[tuple] | dict = None,
-213        exact_match: bool = True,
-214    ) -> int:
-215        """Return number of items in table.
-216
-217        :param match_criteria: Can be a list of 2-tuples where each
-218        tuple is (columnName, rowValue) or a dictionary where
-219        keys are column names and values are row values.
-220        If None, all rows from the table will be counted.
-221
-222        :param exact_match: If False, the row value for a give column
-223        in match_criteria will be matched as a substring. Has no effect if
-224        match_criteria is None.
-225        """
-226        query = f"select count(_rowid_) from {table}"
-227        try:
-228            if match_criteria:
-229                self.cursor.execute(
-230                    f"{query} where {self._get_conditions(match_criteria,
+199    @_connect
+200    def count(
+201        self,
+202        table: str,
+203        match_criteria: list[tuple] | dict | None = None,
+204        exact_match: bool = True,
+205    ) -> int:
+206        """Return number of items in table.
+207
+208        :param match_criteria: Can be a list of 2-tuples where each
+209        tuple is (columnName, rowValue) or a dictionary where
+210        keys are column names and values are row values.
+211        If None, all rows from the table will be counted.
+212
+213        :param exact_match: If False, the row value for a give column
+214        in match_criteria will be matched as a substring. Has no effect if
+215        match_criteria is None.
+216        """
+217        query = f"select count(_rowid_) from {table}"
+218        try:
+219            if match_criteria:
+220                self.cursor.execute(
+221                    f"{query} where {self._get_conditions(match_criteria,
 exact_match)}"
-231                )
-232            else:
-233                self.cursor.execute(f"{query}")
-234            return self.cursor.fetchone()[0]
-235        except:
-236            return 0
+222                )
+223            else:
+224                self.cursor.execute(f"{query}")
+225            return self.cursor.fetchone()[0]
+226        except:
+227            return 0
 Return number of items in table.
 * Parameters *
     * match_criteria: Can be a list of 2-tuples where each tuple is
       (columnName, rowValue) or a dictionary where keys are column names and
       values are row values. If None, all rows from the table will be counted.
     * exact_match: If False, the row value for a give column in match_criteria
       will be matched as a substring. Has no effect if match_criteria is None.
 ⁰
-def add_row(self, table: str, values: tuple[any], columns: tuple[str] = None):
-View Source
-238    @_connect
-239    def add_row(self, table: str, values: tuple[any], columns: tuple[str] =
-None):
-240        """Add row of values to table.
-241
-242        :param table: The table to insert into.
-243
-244        :param values: A tuple of values to be inserted into the table.
-245
-246        :param columns: If None, values param is expected to supply
-247        a value for every column in the table. If columns is
-248        provided, it should contain the same number of elements as
+def add_row(
+self,
+table: str,
+values: tuple[typing.Any],
+columns: tuple[str] | None = None): View Source
+229    @_connect
+230    def add_row(
+231        self, table: str, values: tuple[Any], columns: tuple[str] | None =
+None
+232    ):
+233        """Add row of values to table.
+234
+235        :param table: The table to insert into.
+236
+237        :param values: A tuple of values to be inserted into the table.
+238
+239        :param columns: If None, values param is expected to supply
+240        a value for every column in the table. If columns is
+241        provided, it should contain the same number of elements as
 values."""
-249        parameterizer = ", ".join("?" for _ in values)
-250        logger_values = ", ".join(str(value) for value in values)
-251        try:
-252            if columns:
-253                columns = ", ".join(column for column in columns)
-254                self.cursor.execute(
-255                    f"insert into {table} ({columns}) values(
-{parameterizer})", values
-256                )
-257            else:
-258                self.cursor.execute(
-259                    f"insert into {table} values({parameterizer})", values
+242        parameterizer = ", ".join("?" for _ in values)
+243        logger_values = ", ".join(str(value) for value in values)
+244        try:
+245            if columns:
+246                columns_query = ", ".join(column for column in columns)
+247                self.cursor.execute(
+248                    f"insert into {table} ({columns_query}) values(
+{parameterizer})",
+249                    values,
+250                )
+251            else:
+252                self.cursor.execute(
+253                    f"insert into {table} values({parameterizer})", values
+254                )
+255            self.logger.info(f'Added "{logger_values}" to {table} table.')
+256        except Exception as e:
+257            if "constraint" not in str(e).lower():
+258                self.logger.exception(
+259                    f'Error adding "{logger_values}" to {table} table.'
 260                )
-261            self.logger.info(f'Added "{logger_values}" to {table} table.')
-262        except Exception as e:
-263            if "constraint" not in str(e).lower():
-264                self.logger.exception(
-265                    f'Error adding "{logger_values}" to {table} table.'
-266                )
-267            else:
-268                self.logger.debug(str(e))
+261            else:
+262                self.logger.debug(str(e))
 Add row of values to table.
 * Parameters *
     * table: The table to insert into.
     * values: A tuple of values to be inserted into the table.
     * columns: If None, values param is expected to supply a value for every
       column in the table. If columns is provided, it should contain the same
       number of elements as values.
 ⁰
 def get_rows(
 self,
 table: str,
-match_criteria: list[tuple] | dict = None,
+match_criteria: list[tuple] | dict | None = None,
 exact_match: bool = True,
-sort_by_column: str = None,
-columns_to_return: list[str] = None,
+sort_by_column: str | None = None,
+columns_to_return: list[str] | None = None,
 return_as_dataframe: bool = False,
 values_only: bool = False,
-order_by: str = None,
-limit: str | int = None) -> list[dict] | list[tuple] |
+order_by: str | None = None,
+limit: str | int | None = None) -> list[dict] | list[tuple] |
 pandas.core.frame.DataFrame: View Source
-270    @_connect
-271    def get_rows(
-272        self,
-273        table: str,
-274        match_criteria: list[tuple] | dict = None,
-275        exact_match: bool = True,
-276        sort_by_column: str = None,
-277        columns_to_return: list[str] = None,
-278        return_as_dataframe: bool = False,
-279        values_only: bool = False,
-280        order_by: str = None,
-281        limit: str | int = None,
-282    ) -> list[dict] | list[tuple] | pandas.DataFrame:
-283        """Returns rows from table as a list of dictionaries
-284        where the key-value pairs of the dictionaries are
-285        column name: row value.
-286
-287        :param match_criteria: Can be a list of 2-tuples where each
-288        tuple is (columnName, rowValue) or a dictionary where
-289        keys are column names and values are row values.
-290
-291        :param exact_match: If False, the rowValue for a give column
-292        will be matched as a substring.
-293
-294        :param sort_by_column: A column name to sort the results by.
-295        This will sort results in Python after retrieving them from the db.
-296        Use the 'order_by' param to use SQLite engine for ordering.
-297
-298        :param columns_to_return: Optional list of column names.
-299        If provided, the elements returned by get_rows() will
-300        only contain the provided columns. Otherwise every column
-301        in the row is returned.
-302
-303        :param return_as_dataframe: If True,
-304        the results will be returned as a pandas.DataFrame object.
-305
-306        :param values_only: Return the results as a list of tuples
-307        instead of a list of dictionaries that have column names as keys.
-308        The results will still be sorted according to sort_by_column if
-309        one is provided.
-310
-311        :param order_by: If given, a 'order by {order_by}' clause
-312        will be added to the select query.
-313
-314        :param limit: If given, a 'limit {limit}' clause will be
-315        added to the select query.
-316        """
-317
-318        if type(columns_to_return) is str:
-319            columns_to_return = [columns_to_return]
-320        query = f"select * from {table}"
-321        matches = []
-322        if match_criteria:
-323            query += f" where {self._get_conditions(match_criteria,
+264    @_connect
+265    def get_rows(
+266        self,
+267        table: str,
+268        match_criteria: list[tuple] | dict | None = None,
+269        exact_match: bool = True,
+270        sort_by_column: str | None = None,
+271        columns_to_return: list[str] | None = None,
+272        return_as_dataframe: bool = False,
+273        values_only: bool = False,
+274        order_by: str | None = None,
+275        limit: str | int | None = None,
+276    ) -> list[dict] | list[tuple] | pandas.DataFrame:
+277        """Returns rows from table as a list of dictionaries
+278        where the key-value pairs of the dictionaries are
+279        column name: row value.
+280
+281        :param match_criteria: Can be a list of 2-tuples where each
+282        tuple is (columnName, rowValue) or a dictionary where
+283        keys are column names and values are row values.
+284
+285        :param exact_match: If False, the rowValue for a give column
+286        will be matched as a substring.
+287
+288        :param sort_by_column: A column name to sort the results by.
+289        This will sort results in Python after retrieving them from the db.
+290        Use the 'order_by' param to use SQLite engine for ordering.
+291
+292        :param columns_to_return: Optional list of column names.
+293        If provided, the elements returned by get_rows() will
+294        only contain the provided columns. Otherwise every column
+295        in the row is returned.
+296
+297        :param return_as_dataframe: If True,
+298        the results will be returned as a pandas.DataFrame object.
+299
+300        :param values_only: Return the results as a list of tuples
+301        instead of a list of dictionaries that have column names as keys.
+302        The results will still be sorted according to sort_by_column if
+303        one is provided.
+304
+305        :param order_by: If given, a 'order by {order_by}' clause
+306        will be added to the select query.
+307
+308        :param limit: If given, a 'limit {limit}' clause will be
+309        added to the select query.
+310        """
+311
+312        if type(columns_to_return) is str:
+313            columns_to_return = [columns_to_return]
+314        query = f"select * from {table}"
+315        matches = []
+316        if match_criteria:
+317            query += f" where {self._get_conditions(match_criteria,
 exact_match)}"
-324        if order_by:
-325            query += f" order by {order_by}"
-326        if limit:
-327            query += f" limit {limit}"
-328        query += ";"
-329        self.cursor.execute(query)
-330        matches = self.cursor.fetchall()
-331        results = [self._get_dict(table, match, columns_to_return) for match
+318        if order_by:
+319            query += f" order by {order_by}"
+320        if limit:
+321            query += f" limit {limit}"
+322        query += ";"
+323        self.cursor.execute(query)
+324        matches = self.cursor.fetchall()
+325        results = [self._get_dict(table, match, columns_to_return) for match
 in matches]
-332        if sort_by_column:
-333            results = sorted(results, key=lambda x: x[sort_by_column])
-334        if return_as_dataframe:
-335            return pandas.DataFrame(results)
-336        if values_only:
-337            return [tuple(row.values()) for row in results]
-338        else:
-339            return results
+326        if sort_by_column:
+327            results = sorted(results, key=lambda x: x[sort_by_column])
+328        if return_as_dataframe:
+329            return pandas.DataFrame(results)
+330        if values_only:
+331            return [tuple(row.values()) for row in results]
+332        else:
+333            return results
 Returns rows from table as a list of dictionaries where the key-value pairs of
 the dictionaries are column name: row value.
 * Parameters *
     * match_criteria: Can be a list of 2-tuples where each tuple is
       (columnName, rowValue) or a dictionary where keys are column names and
       values are row values.
     * exact_match: If False, the rowValue for a give column will be matched as
@@ -1469,315 +1441,317 @@
     * limit: If given, a 'limit {limit}' clause will be added to the select
       query.
 ⁰
 def find(
 self,
 table: str,
 query_string: str,
-columns: list[str] = None) -> tuple[dict]: View Source
-341    @_connect
-342    def find(
-343        self, table: str, query_string: str, columns: list[str] = None
-344    ) -> tuple[dict]:
-345        """Search for rows that contain query_string as a substring
-346        of any column.
-347
-348        :param table: The table to search.
-349
-350        :param query_string: The substring to search for in all columns.
-351
-352        :param columns: A list of columns to search for query_string.
-353        If None, all columns in the table will be searched.
-354        """
-355        if type(columns) is str:
-356            columns = [columns]
-357        results = []
-358        if not columns:
-359            columns = self.get_column_names(table)
-360        for column in columns:
-361            results.extend(
-362                [
-363                    row
-364                    for row in self.get_rows(
-365                        table, [(column, query_string)], exact_match=False
-366                    )
-367                    if row not in results
-368                ]
-369            )
-370        return results
+columns: list[str] | None = None) -> list[dict]: View Source
+335    @_connect
+336    def find(
+337        self, table: str, query_string: str, columns: list[str] | None =
+None
+338    ) -> list[dict]:
+339        """Search for rows that contain query_string as a substring
+340        of any column.
+341
+342        :param table: The table to search.
+343
+344        :param query_string: The substring to search for in all columns.
+345
+346        :param columns: A list of columns to search for query_string.
+347        If None, all columns in the table will be searched.
+348        """
+349        if type(columns) is str:
+350            columns = [columns]
+351        results = []
+352        if not columns:
+353            columns = self.get_column_names(table)
+354        for column in columns:
+355            results.extend(
+356                [
+357                    row
+358                    for row in self.get_rows(
+359                        table, [(column, query_string)], exact_match=False
+360                    )
+361                    if row not in results
+362                ]
+363            )
+364        return results
 Search for rows that contain query_string as a substring of any column.
 * Parameters *
     * table: The table to search.
     * query_string: The substring to search for in all columns.
     * columns: A list of columns to search for query_string. If None, all
       columns in the table will be searched.
 ⁰
 def delete(
 self,
 table: str,
 match_criteria: list[tuple] | dict,
 exact_match: bool = True) -> int: View Source
-372    @_connect
-373    def delete(
-374        self, table: str, match_criteria: list[tuple] | dict, exact_match:
+366    @_connect
+367    def delete(
+368        self, table: str, match_criteria: list[tuple] | dict, exact_match:
 bool = True
-375    ) -> int:
-376        """Delete records from table.
+369    ) -> int:
+370        """Delete records from table.
+371
+372        Returns number of deleted records.
+373
+374        :param match_criteria: Can be a list of 2-tuples where each
+375        tuple is (columnName, rowValue) or a dictionary where
+376        keys are column names and values are row values.
 377
-378        Returns number of deleted records.
-379
-380        :param match_criteria: Can be a list of 2-tuples where each
-381        tuple is (columnName, rowValue) or a dictionary where
-382        keys are column names and values are row values.
-383
-384        :param exact_match: If False, the rowValue for a give column
-385        will be matched as a substring.
-386        """
-387        num_matches = self.count(table, match_criteria, exact_match)
-388        conditions = self._get_conditions(match_criteria, exact_match)
-389        try:
-390            self.cursor.execute(f"delete from {table} where {conditions}")
-391            self.logger.info(
-392                f'Deleted {num_matches} from "{table}" where {conditions}".'
-393            )
-394            return num_matches
-395        except Exception as e:
-396            self.logger.debug(f'Error deleting from "{table}" where
+378        :param exact_match: If False, the rowValue for a give column
+379        will be matched as a substring.
+380        """
+381        num_matches = self.count(table, match_criteria, exact_match)
+382        conditions = self._get_conditions(match_criteria, exact_match)
+383        try:
+384            self.cursor.execute(f"delete from {table} where {conditions}")
+385            self.logger.info(
+386                f'Deleted {num_matches} from "{table}" where {conditions}".'
+387            )
+388            return num_matches
+389        except Exception as e:
+390            self.logger.debug(f'Error deleting from "{table}" where
 {conditions}.\n{e}')
-397            return 0
+391            return 0
 Delete records from table.
 Returns number of deleted records.
 * Parameters *
     * match_criteria: Can be a list of 2-tuples where each tuple is
       (columnName, rowValue) or a dictionary where keys are column names and
       values are row values.
     * exact_match: If False, the rowValue for a give column will be matched as
       a substring.
 ⁰
 def update(
 self,
 table: str,
 column_to_update: str,
 new_value: Any,
-match_criteria: list[tuple] | dict = None) -> bool: View Source
-399    @_connect
-400    def update(
-401        self,
-402        table: str,
-403        column_to_update: str,
-404        new_value: Any,
-405        match_criteria: list[tuple] | dict = None,
-406    ) -> bool:
-407        """Update row value for entry matched with match_criteria.
-408
-409        :param column_to_update: The column to be updated in the matched
+match_criteria: list[tuple] | dict | None = None) -> bool: View Source
+393    @_connect
+394    def update(
+395        self,
+396        table: str,
+397        column_to_update: str,
+398        new_value: Any,
+399        match_criteria: list[tuple] | dict | None = None,
+400    ) -> bool:
+401        """Update row value for entry matched with match_criteria.
+402
+403        :param column_to_update: The column to be updated in the matched
 row.
-410
-411        :param new_value: The new value to insert.
-412
-413        :param match_criteria: Can be a list of 2-tuples where each
-414        tuple is (columnName, rowValue) or a dictionary where
-415        keys are column names and values are row values.
-416        If None, every row will be updated.
-417
-418        Returns True if successful, False if not."""
-419        query = f"update {table} set {column_to_update} = ?"
-420        if match_criteria:
-421            if self.count(table, match_criteria) == 0:
-422                self.logger.info(
-423                    f"Couldn't find matching records in {table} table to
+404
+405        :param new_value: The new value to insert.
+406
+407        :param match_criteria: Can be a list of 2-tuples where each
+408        tuple is (columnName, rowValue) or a dictionary where
+409        keys are column names and values are row values.
+410        If None, every row will be updated.
+411
+412        Returns True if successful, False if not."""
+413        query = f"update {table} set {column_to_update} = ?"
+414        conditions = ""
+415        if match_criteria:
+416            if self.count(table, match_criteria) == 0:
+417                self.logger.info(
+418                    f"Couldn't find matching records in {table} table to
 update to '{new_value}'"
-424                )
-425                return False
-426            conditions = self._get_conditions(match_criteria)
-427            query += f" where {conditions}"
-428        else:
-429            conditions = None
-430        try:
-431            self.cursor.execute(
-432                query,
-433                (new_value,),
-434            )
-435            self.logger.info(
-436                f'Updated "{column_to_update}" in "{table}" table to "
+419                )
+420                return False
+421            conditions = self._get_conditions(match_criteria)
+422            query += f" where {conditions}"
+423        else:
+424            conditions = None
+425        try:
+426            self.cursor.execute(
+427                query,
+428                (new_value,),
+429            )
+430            self.logger.info(
+431                f'Updated "{column_to_update}" in "{table}" table to "
 {new_value}" where {conditions}'
-437            )
-438            return True
-439        except UnboundLocalError:
-440            table_filter_string = "\n".join(
-441                table_filter for table_filter in match_criteria
-442            )
-443            self.logger.error(
-444                f"No records found matching filters: {table_filter_string}"
-445            )
-446            return False
-447        except Exception as e:
-448            self.logger.error(
-449                f'Failed to update "{column_to_update}" in "{table}" table
+432            )
+433            return True
+434        except Exception as e:
+435            self.logger.error(
+436                f'Failed to update "{column_to_update}" in "{table}" table
 to "{new_value}" where {conditions}"\n{e}'
-450            )
-451            return False
+437            )
+438            return False
 Update row value for entry matched with match_criteria.
 * Parameters *
     * column_to_update: The column to be updated in the matched row.
     * new_value: The new value to insert.
     * match_criteria: Can be a list of 2-tuples where each tuple is
       (columnName, rowValue) or a dictionary where keys are column names and
       values are row values. If None, every row will be updated.
 Returns True if successful, False if not.
 ⁰
 def drop_table(self, table: str) -> bool: View Source
-453    @_connect
-454    def drop_table(self, table: str) -> bool:
-455        """Drop a table from the database.
-456
-457        Returns True if successful, False if not."""
-458        try:
-459            self.cursor.execute(f"drop Table {table}")
-460            self.logger.info(f'Dropped table "{table}"')
-461        except Exception as e:
-462            print(e)
-463            self.logger.error(f'Failed to drop table "{table}"')
+440    @_connect
+441    def drop_table(self, table: str) -> bool:
+442        """Drop a table from the database.
+443
+444        Returns True if successful, False if not."""
+445        try:
+446            self.cursor.execute(f"drop Table {table}")
+447            self.logger.info(f'Dropped table "{table}"')
+448            return True
+449        except Exception as e:
+450            print(e)
+451            self.logger.error(f'Failed to drop table "{table}"')
+452            return False
 Drop a table from the database.
 Returns True if successful, False if not.
 ⁰
-def add_column(self, table: str, column: str, _type: str, default_value: str =
-None): View Source
-465    @_connect
-466    def add_column(
-467        self, table: str, column: str, _type: str, default_value: str = None
-468    ):
-469        """Add a new column to table.
-470
-471        :param column: Name of the column to add.
-472
-473        :param _type: The data type of the new column.
-474
-475        :param default_value: Optional default value for the column."""
-476        try:
-477            if default_value:
-478                self.cursor.execute(
-479                    f"alter table {table} add column {column} {_type}
+def add_column(
+self,
+table: str,
+column: str,
+_type: str,
+default_value: str | None = None): View Source
+454    @_connect
+455    def add_column(
+456        self, table: str, column: str, _type: str, default_value: str | None
+= None
+457    ):
+458        """Add a new column to table.
+459
+460        :param column: Name of the column to add.
+461
+462        :param _type: The data type of the new column.
+463
+464        :param default_value: Optional default value for the column."""
+465        try:
+466            if default_value:
+467                self.cursor.execute(
+468                    f"alter table {table} add column {column} {_type}
 default {default_value}"
-480                )
-481            else:
-482                self.cursor.execute(f"alter table {table} add column
+469                )
+470            else:
+471                self.cursor.execute(f"alter table {table} add column
 {column} {_type}")
-483            self.logger.info(f'Added column "{column}" to "{table}" table.')
-484        except Exception as e:
-485            self.logger.error(f'Failed to add column "{column}" to "{table}"
+472            self.logger.info(f'Added column "{column}" to "{table}" table.')
+473        except Exception as e:
+474            self.logger.error(f'Failed to add column "{column}" to "{table}"
 table.')
 Add a new column to table.
 * Parameters *
     * column: Name of the column to add.
     * _type: The data type of the new column.
     * default_value: Optional default value for the column.
 ⁰
 @staticmethod
 def data_to_string(
 data: list[dict],
-sort_key: str = None,
+sort_key: str | None = None,
 wrap_to_terminal: bool = True) -> str: View Source
-487    @staticmethod
-488    def data_to_string(
-489        data: list[dict], sort_key: str = None, wrap_to_terminal: bool =
-True
-490    ) -> str:
-491        """Uses tabulate to produce pretty string output
-492        from a list of dictionaries.
-493
-494        :param data: Assumes all dictionaries in list have the same set of
+476    @staticmethod
+477    def data_to_string(
+478        data: list[dict], sort_key: str | None = None, wrap_to_terminal:
+bool = True
+479    ) -> str:
+480        """Uses tabulate to produce pretty string output
+481        from a list of dictionaries.
+482
+483        :param data: Assumes all dictionaries in list have the same set of
 keys.
-495
-496        :param sort_key: Optional dictionary key to sort data with.
-497
-498        :param wrap_to_terminal: If True, the table width will be wrapped
-499        to fit within the current terminal window. Set to False
-500        if the output is going into something like a txt file."""
-501        return data_to_string(data, sort_key, wrap_to_terminal)
+484
+485        :param sort_key: Optional dictionary key to sort data with.
+486
+487        :param wrap_to_terminal: If True, the table width will be wrapped
+488        to fit within the current terminal window. Set to False
+489        if the output is going into something like a txt file."""
+490        return data_to_string(data, sort_key, wrap_to_terminal)
 Uses tabulate to produce pretty string output from a list of dictionaries.
 * Parameters *
     * data: Assumes all dictionaries in list have the same set of keys.
     * sort_key: Optional dictionary key to sort data with.
     * wrap_to_terminal: If True, the table width will be wrapped to fit within
       the current terminal window. Set to False if the output is going into
       something like a txt file.
   ⁰
 def data_to_string(
 data: list[dict],
-sort_key: str = None,
+sort_key: str | None = None,
 wrap_to_terminal: bool = True) -> str: View Source
-504def data_to_string(
-505    data: list[dict], sort_key: str = None, wrap_to_terminal: bool = True
-506) -> str:
-507    """Use tabulate to produce grid output from a list of dictionaries.
-508
-509    :param data: Assumes all dictionaries in list have the same set of keys.
-510
-511    :param sort_key: Optional dictionary key to sort data with.
-512
-513    :param wrap_to_terminal: If True, the column widths will be reduced so
+493def data_to_string(
+494    data: list[dict], sort_key: str | None = None, wrap_to_terminal: bool =
+True
+495) -> str:
+496    """Use tabulate to produce grid output from a list of dictionaries.
+497
+498    :param data: Assumes all dictionaries in list have the same set of keys.
+499
+500    :param sort_key: Optional dictionary key to sort data with.
+501
+502    :param wrap_to_terminal: If True, the column widths will be reduced so
 the grid fits
-514    within the current terminal window without wrapping. If the column
+503    within the current terminal window without wrapping. If the column
 widths have reduced to 1
-515    and the grid is still too wide, str(data) will be returned."""
-516    if len(data) == 0:
-517        return ""
-518    if sort_key:
-519        data = sorted(data, key=lambda d: d[sort_key])
-520    for i, d in enumerate(data):
-521        for k in d:
-522            data[i][k] = str(data[i][k])
-523
-524    too_wide = True
-525    terminal_width = os.get_terminal_size().columns
-526    max_col_widths = terminal_width
-527    # Make an output with effectively unrestricted column widths
-528    # to see if shrinking is necessary
-529    output = tabulate(
-530        data,
-531        headers="keys",
-532        disable_numparse=True,
-533        tablefmt="grid",
-534        maxcolwidths=max_col_widths,
-535    )
-536    current_width = output.index("\n")
-537    if current_width < terminal_width:
-538        too_wide = False
-539    if wrap_to_terminal and too_wide:
-540        print("Resizing grid to fit within the terminal...")
-541        previous_col_widths = max_col_widths
-542        acceptable_width = terminal_width - 10
-543        while too_wide and max_col_widths > 1:
-544            if current_width > terminal_width:
-545                previous_col_widths = max_col_widths
-546                max_col_widths = int(max_col_widths * 0.5)
-547            elif current_width < terminal_width:
-548                # Without lowering acceptable_width, this condition will
+504    and the grid is still too wide, str(data) will be returned."""
+505    if len(data) == 0:
+506        return ""
+507    if sort_key:
+508        data = sorted(data, key=lambda d: d[sort_key])
+509    for i, d in enumerate(data):
+510        for k in d:
+511            data[i][k] = str(data[i][k])
+512
+513    too_wide = True
+514    terminal_width = os.get_terminal_size().columns
+515    max_col_widths = terminal_width
+516    # Make an output with effectively unrestricted column widths
+517    # to see if shrinking is necessary
+518    output = tabulate(
+519        data,
+520        headers="keys",
+521        disable_numparse=True,
+522        tablefmt="grid",
+523        maxcolwidths=max_col_widths,
+524    )
+525    current_width = output.index("\n")
+526    if current_width < terminal_width:
+527        too_wide = False
+528    if wrap_to_terminal and too_wide:
+529        print("Resizing grid to fit within the terminal...")
+530        previous_col_widths = max_col_widths
+531        acceptable_width = terminal_width - 10
+532        while too_wide and max_col_widths > 1:
+533            if current_width > terminal_width:
+534                previous_col_widths = max_col_widths
+535                max_col_widths = int(max_col_widths * 0.5)
+536            elif current_width < terminal_width:
+537                # Without lowering acceptable_width, this condition will
 cause infinite loop
-549                if max_col_widths == previous_col_widths - 1:
-550                    acceptable_width -= 10
-551                max_col_widths = int(
-552                    max_col_widths + (0.5 * (previous_col_widths -
+538                if max_col_widths == previous_col_widths - 1:
+539                    acceptable_width -= 10
+540                max_col_widths = int(
+541                    max_col_widths + (0.5 * (previous_col_widths -
 max_col_widths))
-553                )
-554            output = tabulate(
-555                data,
-556                headers="keys",
-557                disable_numparse=True,
-558                tablefmt="grid",
-559                maxcolwidths=max_col_widths,
-560            )
-561            current_width = output.index("\n")
-562            if acceptable_width < current_width < terminal_width:
-563                too_wide = False
-564        if too_wide:
-565            print("Couldn't resize grid to fit within the terminal.")
-566            return str(data)
-567    return output
+542                )
+543            output = tabulate(
+544                data,
+545                headers="keys",
+546                disable_numparse=True,
+547                tablefmt="grid",
+548                maxcolwidths=max_col_widths,
+549            )
+550            current_width = output.index("\n")
+551            if acceptable_width < current_width < terminal_width:
+552                too_wide = False
+553        if too_wide:
+554            print("Couldn't resize grid to fit within the terminal.")
+555            return str(data)
+556    return output
 Use tabulate to produce grid output from a list of dictionaries.
 * Parameters *
     * data: Assumes all dictionaries in list have the same set of keys.
     * sort_key: Optional dictionary key to sort data with.
     * wrap_to_terminal: If True, the column widths will be reduced so the grid
       fits within the current terminal window without wrapping. If the column
       widths have reduced to 1 and the grid is still too wide, str(data) will
```

### Comparing `databased-1.4.5/src/databased/databased.py` & `databased-1.5.0/src/databased/databased.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 import os
 import sqlite3
 from datetime import datetime
 from functools import wraps
-from pathlib import Path
 from typing import Any
 
 import pandas
+from pathier import Pathier
 from tabulate import tabulate
 
 
 def _connect(func):
     """Decorator to open db connection if it isn't already open."""
 
     @wraps(func)
@@ -28,50 +28,41 @@
 
     Supports saving and reading dates as datetime objects.
 
     Supports using a context manager."""
 
     def __init__(
         self,
-        dbpath: str | Path,
+        dbpath: str | Pathier,
         logger_encoding: str = "utf-8",
         logger_message_format: str = "{levelname}|-|{asctime}|-|{message}",
     ):
         """
         :param dbpath: String or Path object to database file.
         If a relative path is given, it will be relative to the
         current working directory. The log file will be saved to the
         same directory.
 
         :param logger_message_format: '{' style format string
         for the logger object."""
-        self.dbpath = Path(dbpath)
-        self.dbname = Path(dbpath).name
+        self.dbpath = Pathier(dbpath)
+        self.dbname = Pathier(dbpath).name
         self.dbpath.parent.mkdir(parents=True, exist_ok=True)
         self._logger_init(
             encoding=logger_encoding, message_format=logger_message_format
         )
         self.connection_open = False
-        self.create_manager()
 
     def __enter__(self):
         self.open()
         return self
 
     def __exit__(self, exception_type, exception_value, exception_traceback):
         self.close()
 
-    def create_manager(self):
-        """Create dbmanager.py in the same directory
-        as the database file if it doesn't exist."""
-        manager_path = self.dbpath.parent / "dbmanager.py"
-        if not manager_path.exists():
-            manager_template = (Path(__file__).parent / "dbmanager.py").read_text()
-            manager_path.write_text(manager_template.replace("$dbname", self.dbname))
-
     def open(self):
         """Open connection to db."""
         self.connection = sqlite3.connect(
             self.dbpath,
             detect_types=sqlite3.PARSE_DECLTYPES | sqlite3.PARSE_COLNAMES,
             timeout=10,
         )
@@ -105,15 +96,15 @@
                     message_format, style="{", datefmt="%m/%d/%Y %I:%M:%S %p"
                 )
             )
             self.logger.addHandler(handler)
             self.logger.setLevel(logging.INFO)
 
     def _get_dict(
-        self, table: str, values: list, columns_to_return: list[str] = None
+        self, table: str, values: list, columns_to_return: list[str] | None = None
     ) -> dict:
         """Converts the values of a row into a dictionary with column names as keys.
 
         :param table: The table that values were pulled from.
 
         :param values: List of values expected to be the same quantity
         and in the same order as the column names of table.
@@ -204,15 +195,15 @@
         self.cursor.execute(f"select * from {table} where 1=0")
         return [description[0] for description in self.cursor.description]
 
     @_connect
     def count(
         self,
         table: str,
-        match_criteria: list[tuple] | dict = None,
+        match_criteria: list[tuple] | dict | None = None,
         exact_match: bool = True,
     ) -> int:
         """Return number of items in table.
 
         :param match_criteria: Can be a list of 2-tuples where each
         tuple is (columnName, rowValue) or a dictionary where
         keys are column names and values are row values.
@@ -231,31 +222,34 @@
             else:
                 self.cursor.execute(f"{query}")
             return self.cursor.fetchone()[0]
         except:
             return 0
 
     @_connect
-    def add_row(self, table: str, values: tuple[any], columns: tuple[str] = None):
+    def add_row(
+        self, table: str, values: tuple[Any], columns: tuple[str] | None = None
+    ):
         """Add row of values to table.
 
         :param table: The table to insert into.
 
         :param values: A tuple of values to be inserted into the table.
 
         :param columns: If None, values param is expected to supply
         a value for every column in the table. If columns is
         provided, it should contain the same number of elements as values."""
         parameterizer = ", ".join("?" for _ in values)
         logger_values = ", ".join(str(value) for value in values)
         try:
             if columns:
-                columns = ", ".join(column for column in columns)
+                columns_query = ", ".join(column for column in columns)
                 self.cursor.execute(
-                    f"insert into {table} ({columns}) values({parameterizer})", values
+                    f"insert into {table} ({columns_query}) values({parameterizer})",
+                    values,
                 )
             else:
                 self.cursor.execute(
                     f"insert into {table} values({parameterizer})", values
                 )
             self.logger.info(f'Added "{logger_values}" to {table} table.')
         except Exception as e:
@@ -266,22 +260,22 @@
             else:
                 self.logger.debug(str(e))
 
     @_connect
     def get_rows(
         self,
         table: str,
-        match_criteria: list[tuple] | dict = None,
+        match_criteria: list[tuple] | dict | None = None,
         exact_match: bool = True,
-        sort_by_column: str = None,
-        columns_to_return: list[str] = None,
+        sort_by_column: str | None = None,
+        columns_to_return: list[str] | None = None,
         return_as_dataframe: bool = False,
         values_only: bool = False,
-        order_by: str = None,
-        limit: str | int = None,
+        order_by: str | None = None,
+        limit: str | int | None = None,
     ) -> list[dict] | list[tuple] | pandas.DataFrame:
         """Returns rows from table as a list of dictionaries
         where the key-value pairs of the dictionaries are
         column name: row value.
 
         :param match_criteria: Can be a list of 2-tuples where each
         tuple is (columnName, rowValue) or a dictionary where
@@ -335,16 +329,16 @@
         if values_only:
             return [tuple(row.values()) for row in results]
         else:
             return results
 
     @_connect
     def find(
-        self, table: str, query_string: str, columns: list[str] = None
-    ) -> tuple[dict]:
+        self, table: str, query_string: str, columns: list[str] | None = None
+    ) -> list[dict]:
         """Search for rows that contain query_string as a substring
         of any column.
 
         :param table: The table to search.
 
         :param query_string: The substring to search for in all columns.
 
@@ -397,29 +391,30 @@
 
     @_connect
     def update(
         self,
         table: str,
         column_to_update: str,
         new_value: Any,
-        match_criteria: list[tuple] | dict = None,
+        match_criteria: list[tuple] | dict | None = None,
     ) -> bool:
         """Update row value for entry matched with match_criteria.
 
         :param column_to_update: The column to be updated in the matched row.
 
         :param new_value: The new value to insert.
 
         :param match_criteria: Can be a list of 2-tuples where each
         tuple is (columnName, rowValue) or a dictionary where
         keys are column names and values are row values.
         If None, every row will be updated.
 
         Returns True if successful, False if not."""
         query = f"update {table} set {column_to_update} = ?"
+        conditions = ""
         if match_criteria:
             if self.count(table, match_criteria) == 0:
                 self.logger.info(
                     f"Couldn't find matching records in {table} table to update to '{new_value}'"
                 )
                 return False
             conditions = self._get_conditions(match_criteria)
@@ -431,43 +426,37 @@
                 query,
                 (new_value,),
             )
             self.logger.info(
                 f'Updated "{column_to_update}" in "{table}" table to "{new_value}" where {conditions}'
             )
             return True
-        except UnboundLocalError:
-            table_filter_string = "\n".join(
-                table_filter for table_filter in match_criteria
-            )
-            self.logger.error(
-                f"No records found matching filters: {table_filter_string}"
-            )
-            return False
         except Exception as e:
             self.logger.error(
                 f'Failed to update "{column_to_update}" in "{table}" table to "{new_value}" where {conditions}"\n{e}'
             )
             return False
 
     @_connect
     def drop_table(self, table: str) -> bool:
         """Drop a table from the database.
 
         Returns True if successful, False if not."""
         try:
             self.cursor.execute(f"drop Table {table}")
             self.logger.info(f'Dropped table "{table}"')
+            return True
         except Exception as e:
             print(e)
             self.logger.error(f'Failed to drop table "{table}"')
+            return False
 
     @_connect
     def add_column(
-        self, table: str, column: str, _type: str, default_value: str = None
+        self, table: str, column: str, _type: str, default_value: str | None = None
     ):
         """Add a new column to table.
 
         :param column: Name of the column to add.
 
         :param _type: The data type of the new column.
 
@@ -481,15 +470,15 @@
                 self.cursor.execute(f"alter table {table} add column {column} {_type}")
             self.logger.info(f'Added column "{column}" to "{table}" table.')
         except Exception as e:
             self.logger.error(f'Failed to add column "{column}" to "{table}" table.')
 
     @staticmethod
     def data_to_string(
-        data: list[dict], sort_key: str = None, wrap_to_terminal: bool = True
+        data: list[dict], sort_key: str | None = None, wrap_to_terminal: bool = True
     ) -> str:
         """Uses tabulate to produce pretty string output
         from a list of dictionaries.
 
         :param data: Assumes all dictionaries in list have the same set of keys.
 
         :param sort_key: Optional dictionary key to sort data with.
@@ -497,15 +486,15 @@
         :param wrap_to_terminal: If True, the table width will be wrapped
         to fit within the current terminal window. Set to False
         if the output is going into something like a txt file."""
         return data_to_string(data, sort_key, wrap_to_terminal)
 
 
 def data_to_string(
-    data: list[dict], sort_key: str = None, wrap_to_terminal: bool = True
+    data: list[dict], sort_key: str | None = None, wrap_to_terminal: bool = True
 ) -> str:
     """Use tabulate to produce grid output from a list of dictionaries.
 
     :param data: Assumes all dictionaries in list have the same set of keys.
 
     :param sort_key: Optional dictionary key to sort data with.
```

### Comparing `databased-1.4.5/src/databased/dbmanager.py` & `databased-1.5.0/src/databased/dbmanager.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,286 +1,267 @@
-import argparse
-import shlex
-import sys
-from pathlib import Path
-
-from databased import DataBased, data_to_string
-
-""" A command line tool to interact with a database file.
-Works like a standard argparse based cli
-except it will ask you for arguments indefinitely in a loop
-instead of having to invoke the script with arguments over and over.
-I.e. instead of "python dbManager.py -db database.db -f someString -t someTable",
-just invoke "python dbManager.py" then a repeating "Enter command: " prompt will appear
-and "-db database.db -f someString -t someTable" can be entered.
-Note: a -db arg only needs to be provided once (if there is no default set) unless
-you wish to change databases. So a subsequent command to the above
-can just be entered as "-f someOtherString -t someTable".
-
-This is just a quick template and can be customized by adding arguments and adding/overriding functions
-for specific database projects."""
-
-# Subclassing to prevent program exit when the -h/--help arg is passed.
-class ArgParser(argparse.ArgumentParser):
-    def exit(self, status=0, message=None):
-        if message:
-            self._print_message(message, sys.stderr)
-
-
-def get_args(command: str) -> argparse.Namespace:
-    parser = ArgParser()
-
-    parser.add_argument(
-        "-db",
-        "--dbname",
-        type=str,
-        default=None,
-        help="""Name of database file to use.
-        Required on the first loop if no default is set,
-        but subsequent loops will resuse the same database
-        unless a new one is provided through this arg.""",
-    )
-
-    parser.add_argument(
-        "-i",
-        "--info",
-        action="store_true",
-        help=""" Display table names, their respective columns, and how many records they contain.
-        If a -t/--tables arg is passed, just the columns and row count for those tables will be shown.""",
-    )
-
-    parser.add_argument(
-        "-t",
-        "--tables",
-        type=str,
-        nargs="*",
-        default=[],
-        help="""Limits commands to a specific list of tables.
-        Optional for some commands, required for others.
-        If this is the only arg given (besides -db if not already set),
-        the whole table will be printed to the terminal.""",
-    )
-
-    parser.add_argument(
-        "-c",
-        "--columns",
-        type=str,
-        nargs="*",
-        default=[],
-        help=""" Limits commands to a specific list of columns.
-        Optional for some commands, required for others.
-        If this and -t are the only args given 
-        (besides -db if not already set), the whole table will be printed
-        to the terminal, but with only the columns provided with this arg.""",
-    )
+import argshell
+from pathier import Pathier
 
-    parser.add_argument(
-        "-f",
-        "--find",
-        type=str,
-        default=None,
-        help=""" A substring to search the database for. 
-        If a -c/--columns arg(s) is not given, the values will be matched against all columns.
-        Similarly, if a -t/--tables arg(s) is not given, the values will be searched for in all tables.""",
-    )
-
-    parser.add_argument(
-        "-sco",
-        "--show_count_only",
-        action="store_true",
-        help=""" Show the number of results returned by -f/--find,
-        but don't print the results to the terminal.""",
-    )
+from databased import DataBased, dbparsers
 
-    parser.add_argument(
-        "-d",
-        "--delete",
-        type=str,
-        nargs="*",
-        default=[],
-        help=""" A list of values to be deleted from the database.
-        A -c/--columns arg must be supplied.
-        A -t/--tables arg must be supplied.""",
-    )
 
-    parser.add_argument(
-        "-u",
-        "--update",
-        type=str,
-        default=None,
-        nargs="*",
-        help=""" Update a record in the database.
-        Expects the first argument to be the new value and interprets
-        subsequent arguements as pairs of 'column' and 'value' to use
-        when selecting which rows to update. The -c/--columns arg will
-        be the column that is updated with the new value for matching rows.
-        A -c/--columns arg must be supplied.
-        A -t/--tables arg must be supplied.
-        e.g '-t birds -c last_seen -u today name sparrow migratory 0'
-        will update the 'last_seen' column of the 'birds' table to 'today'
-        for all rows that have either/both of their 'name' and 'migratory'
-        columns set to 'sparrow' and '0', respectively.""",
-    )
+class DBManager(argshell.ArgShell):
+    intro = "Starting dbmanager (enter help or ? for arg info)..."
+    prompt = "based>"
+    dbpath: Pathier = None  # type: ignore
+
+    def do_use_db(self, arg: str):
+        """Set which database file to use."""
+        dbpath = Pathier(arg)
+        if not dbpath.exists():
+            print(f"{dbpath} does not exist.")
+            print(f"Still using {self.dbpath}")
+        elif not dbpath.is_file():
+            print(f"{dbpath} is not a file.")
+            print(f"Still using {self.dbpath}")
+        else:
+            self.dbpath = dbpath
 
-    parser.add_argument(
-        "-sb", "--sort_by", type=str, default=None, help="Column to sort results by."
-    )
+    def do_dbpath(self, arg: str):
+        """Print the .db file in use."""
+        print(self.dbpath)
+
+    def do_backup(self, arg: str):
+        """Create a backup of the current db file."""
+        print(f"Creating a back up for {self.dbpath}...")
+        backup_path = self.dbpath.with_stem(f"{self.dbpath.stem}_bckup")
+        self.dbpath.copy(backup_path, True)
+        print("Creating backup is complete.")
+        print(f"Backup path: {backup_path}")
+
+    def do_size(self, arg: str):
+        """Display the size of the the current db file."""
+        print(f"{self.dbpath.name} is {self.dbpath.size(True)}.")
+
+    @argshell.with_parser(dbparsers.get_create_table_parser)
+    def do_create_table(self, args: argshell.Namespace):
+        """Create a table."""
+        with DataBased(self.dbpath) as db:
+            db.create_table(args.table_name, args.columns)
+
+    def do_drop_table(self, arg: str):
+        """Drop the specified table."""
+        with DataBased(self.dbpath) as db:
+            db.drop_table(arg)
 
-    parser.add_argument(
-        "-q",
-        "--query",
-        type=str,
-        default=None,
-        help=""" Directly execute a query against the database. """,
+    @argshell.with_parser(
+        dbparsers.get_add_row_parser, [dbparsers.verify_matching_length]
     )
+    def do_add_row(self, args: argshell.Namespace):
+        """Add a row to a table."""
+        with DataBased(self.dbpath) as db:
+            db.add_row(args.table_name, args.values, args.columns or None)
+
+    def do_info(self, arg: str):
+        """Print out the names of the database tables, their columns, and the number of rows.
+        Pass a space-separated list of table names to only print info for those specific tables,
+        otherwise all tables will be printed."""
+        print("Getting database info...")
+        with DataBased(self.dbpath) as db:
+            tables = arg.split() or db.get_table_names()
+            info = [
+                {
+                    "Table Name": table,
+                    "Columns": ", ".join(db.get_column_names(table)),
+                    "Number of Rows": db.count(table),
+                }
+                for table in tables
+            ]
+        print(DataBased.data_to_string(info))
+
+    @argshell.with_parser(dbparsers.get_lookup_parser, [dbparsers.convert_match_pairs])
+    def do_find(self, args: argshell.Namespace):
+        """Find and print rows from the database.
+        Use the -t/--tables, -m/--match_pairs, and -l/--limit flags to limit the search.
+        Use the -c/--columns flag to limit what columns are printed.
+        Use the -o/--order_by flag to order the results.
+        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs
+        Pass -h/--help flag for parser help."""
+        print("Finding records... ")
+        if len(args.columns) == 0:
+            args.columns = None
+        with DataBased(self.dbpath) as db:
+            tables = args.tables or db.get_table_names()
+            for table in tables:
+                results = db.get_rows(
+                    table,
+                    args.match_pairs,
+                    columns_to_return=args.columns,
+                    order_by=args.order_by,
+                    limit=args.limit,
+                    exact_match=not args.partial_matching,
+                )
+                db.close()
+                print(f"{len(results)} matching rows in {table} table:")
+                try:
+                    print(DataBased.data_to_string(results))  # type: ignore
+                except Exception as e:
+                    print("Couldn't fit data into a grid.")
+                    print(*results, sep="\n")
+                print()
+
+    @argshell.with_parser(dbparsers.get_search_parser)
+    def do_search(self, args: argshell.Namespace):
+        """Search and return any rows containg the searched substring in any of its columns.
+        Use the -t/--tables flag to limit the search to a specific table(s).
+        Use the -c/--columns flag to limit the search to a specific column(s)."""
+        print(f"Searching for {args.search_string}...")
+        with DataBased(self.dbpath) as db:
+            tables = args.tables or db.get_table_names()
+            for table in tables:
+                columns = args.columns or db.get_column_names(table)
+                matcher = " OR ".join(
+                    f'{column} LIKE "%{args.search_string}%"' for column in columns
+                )
+                query = f"SELECT * FROM {table} WHERE {matcher};"
+                results = db.query(query)
+                results = [db._get_dict(table, result) for result in results]
+                print(f"Found {len(results)} results in {table} table.")
+                print(DataBased.data_to_string(results))
+
+    @argshell.with_parser(dbparsers.get_lookup_parser, [dbparsers.convert_match_pairs])
+    def do_count(self, args: argshell.Namespace):
+        """Print the number of rows in the database.
+        Use the -t/--tables flag to limit results to a specific table(s).
+        Use the -m/--match_pairs flag to limit the results to rows matching these criteria.
+        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs.
+        Pass -h/--help flag for parser help."""
+        print("Counting rows...")
+        with DataBased(self.dbpath) as db:
+            tables = args.tables or db.get_table_names()
+            for table in tables:
+                num_rows = db.count(table, args.match_pairs, not args.partial_matching)
+                print(f"{num_rows} matching rows in {table} table.")
+
+    def do_query(self, arg: str):
+        """Execute a query against the current database."""
+        print(f"Executing {arg}")
+        with DataBased(self.dbpath) as db:
+            results = db.query(arg)
+        try:
+            for result in results:
+                print(*result, sep="|-|")
+        except Exception as e:
+            print(f"{type(e).__name__}: {e}")
 
-    args = parser.parse_args(command)
-
-    if args.dbname and not Path(args.dbname).exists():
-        raise Exception(f"{args.dbname} does not exist.")
-
-    return args
+    @argshell.with_parser(dbparsers.get_update_parser, [dbparsers.convert_match_pairs])
+    def do_update(self, args: argshell.Namespace):
+        """Update a column to a new value.
+        Two required args: the column (-c/--column) to update and the value (-v/--value) to update to.
+        Use the -t/--tables flag to limit what tables are updated.
+        Use the -m/--match_pairs flag to specify which rows are updated.
+        >>> based>update -c username -v big_chungus -t users -m username lil_chungus
+
+        ^will update the username in the users 'table' to 'big_chungus' where the username is currently 'lil_chungus'^"""
+        print("Updating rows...")
+        with DataBased(self.dbpath) as db:
+            tables = args.tables or db.get_table_names()
+            for table in tables:
+                if db.update(table, args.column, args.new_value, args.match_pairs):
+                    print(f"Updating rows in {table} table successful.")
+                else:
+                    print(f"Failed to update rows in {table} table.")
 
+    @argshell.with_parser(dbparsers.get_lookup_parser, [dbparsers.convert_match_pairs])
+    def do_delete(self, args: argshell.Namespace):
+        """Delete rows from the database.
+        Use the -t/--tables flag to limit what tables rows are deleted from.
+        Use the -m/--match_pairs flag to specify which rows are deleted.
+        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs.
+        >>> based>delete -t users -m username chungus -p
+
+        ^will delete all rows in the 'users' table whose username contains 'chungus'^"""
+        print("Deleting records...")
+        with DataBased(self.dbpath) as db:
+            tables = args.tables or db.get_table_names()
+            for table in tables:
+                num_rows = db.delete(table, args.match_pairs, not args.partial_matching)
+                print(f"Deleted {num_rows} rows from {table} table.")
+
+    def do_flush_log(self, arg: str):
+        """Clear the log file for this database."""
+        log_path = self.dbpath.with_name(self.dbpath.stem + "db.log")
+        if not log_path.exists():
+            print(f"No log file at path {log_path}")
+        else:
+            print(f"Flushing log...")
+            log_path.write_text("")
 
-def info():
-    print("Getting database info...")
-    print()
-    if not args.tables:
-        args.tables = db.get_table_names()
-    results = []
-    for table in args.tables:
-        count = db.count(table)
-        columns = db.get_column_names(table)
-        results.append(
-            {
-                "table name": table,
-                "columns": ", ".join(columns),
-                "number of rows": count,
-            }
-        )
-    if args.sort_by and args.sort_by in results[0]:
-        results = sorted(results, key=lambda x: x[args.sort_by])
-    print(data_to_string(results))
-
-
-def find():
-    print("Finding records... ")
-    print()
-    if not args.tables:
-        args.tables = db.get_table_names()
-    for table in args.tables:
-        results = db.find(table, args.find, args.columns)
-        if args.sort_by and args.sort_by in results[0]:
-            results = sorted(results, key=lambda x: x[args.sort_by])
-        if args.columns:
+    def do_customize(self, arg: str):
+        """Generate a template file in the current working directory for creating a custom DBManager class.
+        Expects one argument: the name of the custom dbmanager.
+        This will be used to name the generated file as well as several components in the file content."""
+        custom_file = (Pathier.cwd() / arg.replace(" ", "_")).with_suffix(".py")
+        if custom_file.exists():
+            print(f"Error: {custom_file.name} already exists in this location.")
+        else:
+            variable_name = "_".join(word for word in arg.lower().split())
+            class_name = "".join(word.capitalize() for word in arg.split())
+            content = (Pathier(__file__).parent / "custom_manager.py").read_text()
+            content = content.replace("CustomManager", class_name)
+            content = content.replace("custommanager", variable_name)
+            custom_file.write_text(content)
+
+    def _choose_db(self, options: list[Pathier]) -> Pathier:
+        """Prompt the user to select from a list of files."""
+        cwd = Pathier.cwd()
+        paths = [path.separate(cwd.stem) for path in options]
+        while True:
             print(
-                f"{len(results)} results for '{args.find}' in '{', '.join(args.columns)}' column(s) of '{table}' table:"
+                f"DB options:\n{' '.join([f'({i}) {path}' for i,path in enumerate(paths,1)])}"
             )
-        else:
-            print(f"{len(results)} results for '{args.find}' in '{table}' table:")
-        if not args.show_count_only:
+            choice = input("Enter the number of the option to use: ")
             try:
-                print(data_to_string(results))
+                index = int(choice)
+                if not 1 <= index <= len(options):
+                    print("Choice out of range.")
+                    continue
+                return options[index - 1]
             except Exception as e:
-                print("Couldn't fit data into a grid.")
-                print(*results, sep="\n")
-        print()
-
-
-def delete():
-    if not args.tables:
-        raise ValueError("Missing -t/--tables arg for -d/--delete function.")
-    if not args.columns:
-        raise ValueError("Missing -c/--columns arg for -d/--delete function.")
-    print("Deleting records... ")
-    print()
-    num_deleted_records = 0
-    failed_deletions = []
-    for item in args.delete:
-        success = db.delete(args.tables[0], [(args.columns[0], item)])
-        if success:
-            num_deleted_records += success
+                print(f"{choice} is not a valid option.")
+
+    def preloop(self):
+        """Scan the current directory for a .db file to use.
+        If not found, prompt the user for one or to try again recursively."""
+        if self.dbpath:
+            self.dbpath = Pathier(self.dbpath)
+            print(f"Defaulting to database {self.dbpath}")
         else:
-            failed_deletions.append(item)
-    print(f"Deleted {num_deleted_records} record(s) from '{args.tables[0]}' table.")
-    if len(failed_deletions) > 0:
-        print(
-            f"Failed to delete the following {len(failed_deletions)} record(s) from '{args.tables[0]}' table:"
-        )
-        for fail in failed_deletions:
-            print(f"  {fail}")
-
-
-def update():
-    if not args.tables:
-        raise ValueError("Missing -t/--tables arg for -u/--update function.")
-    if not args.columns:
-        raise ValueError("Missing -c/--columns arg for -u/--update function.")
-    print("Updating record... ")
-    print()
-    new_value = args.update[0]
-    if len(args.update) > 1:
-        args.update = args.update[1:]
-        match_criteria = [
-            (args.update[i], args.update[i + 1]) for i in range(0, len(args.update), 2)
-        ]
-    else:
-        match_criteria = None
-    if db.update(
-        args.tables[0],
-        args.columns[0],
-        new_value,
-        match_criteria,
-    ):
-        print(
-            f"Updated '{args.columns[0]}' column to '{new_value}' in '{args.tables[0]}' table for match_criteria {match_criteria}."
-        )
-    else:
-        print(
-            f"Failed to update '{args.columns[0]}' column to '{new_value}' in '{args.tables[0]}' table for match_criteria {match_criteria}."
-        )
-
-
-def print_table():
-    for table in args.tables:
-        rows = db.get_rows(
-            table, columns_to_return=args.columns, sort_by_column=args.sort_by
-        )
-        print(f"{table} table:")
-        print(data_to_string(rows))
-
-
-def query():
-    results = db.query(args.query)
-    try:
-        for result in results:
-            print(*result, sep=" * ")
-    except Exception as e:
-        print(f"Couldn't display results of '{args.query}'.")
-
-
-if __name__ == "__main__":
-    sys.tracebacklimit = 0
-    dbname = "$dbname"
-    while True:
-        try:
-            command = shlex.split(input("Enter command: "))
-            args = get_args(command)
-            if args.dbname:
-                dbname = args.dbname
-            with DataBased(dbpath=dbname) as db:
-                if args.info:
-                    info()
-                elif args.find:
-                    find()
-                elif args.delete:
-                    delete()
-                elif args.update:
-                    update()
-                elif args.query:
-                    query()
-                else:
-                    print_table()
-        except KeyboardInterrupt:
-            break
-        except Exception as e:
-            print(e)
+            print("Searching for database...")
+            cwd = Pathier.cwd()
+            dbs = list(cwd.glob("*.db"))
+            if len(dbs) == 1:
+                self.dbpath = dbs[0]
+                print(f"Using database {self.dbpath}.")
+            elif dbs:
+                self.dbpath = self._choose_db(dbs)
+            else:
+                print(f"Could not find a .db file in {cwd}.")
+                path = input(
+                    "Enter path to .db file to use or press enter to search again recursively: "
+                )
+                if path:
+                    self.dbpath = Pathier(path)
+                elif not path:
+                    print("Searching recursively...")
+                    dbs = list(cwd.rglob("*.db"))
+                    if len(dbs) == 1:
+                        self.dbpath = dbs[0]
+                        print(f"Using database {self.dbpath}.")
+                    elif dbs:
+                        self.dbpath = self._choose_db(dbs)
+                    else:
+                        print("Could not find a .db file.")
+                        self.dbpath = Pathier(input("Enter path to a .db file: "))
+        if not self.dbpath.exists():
+            raise FileNotFoundError(f"{self.dbpath} does not exist.")
+        if not self.dbpath.is_file():
+            raise ValueError(f"{self.dbpath} is not a file.")
+
+
+def main():
+    DBManager().cmdloop()
```

### Comparing `databased-1.4.5/LICENSE.txt` & `databased-1.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `databased-1.4.5/README.md` & `databased-1.5.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 # Databased
 Databased is a package that wraps the standard library Sqlite3 module to make setting up and using a database quicker and easier.<br>
+
 Install with:
 <pre>pip install databased</pre>
-databased is a package that wraps the standard library Sqlite3 module to largely avoid writing queries except for table definitions.<br>
-It consists of the class DataBased and an additional function for displaying information in a grid called data_to_string.<br>
+
+`databased` is a package that wraps the standard library Sqlite3 module to largely avoid writing queries except for table definitions (there is a `query` function that can be used to directly excute queries).<br>
+It primarily consists of the class `DataBased`.<br>
 The DataBased class contains functions for creating databases and tables; inserting, updating, and deleting rows; 
 as well as retrieving data and schema information.<br>
-The data_to_string function uses the [tabulate](https://pypi.org/project/tabulate/) to generate a grid as a string from a list of dictionaries.<br>
+
+There is also a static method called `data_to_string` which uses [tabulate](https://pypi.org/project/tabulate/) to generate a printable grid from a list of dictionaries.<br>
 By default, data_to_string will automatically wrap the width of columns to fit within the current terminal window.<br><br>
-Member functions that require a database connection will
-automatically create one when called if one isn't already open,
-but a manual call to self.close() needs to be called in order to
-save the database file and release the connection.<br>
-If a context manager is used, like in the following example, you don't need to worry about manually opening, saving, or closing the database.<br>
+Member functions that require a database connection will automatically create one when called if one isn't already open.<br>
+If you create a class that inherits from `DataBased`, you will need to decorate member functions that access the database with `@_connect`.<br>
+Unless `DataBased` is used with a context manager, you will need to manually call the `close()` function to close the connection and save the database.
 <br>
 Usage:
 <pre>
-from databased import DataBased, data_to_string
+from databased import DataBased
 from datetime import datetime
 
 # if the .db file specified doesn't exist, it will be created
 # a log file with the same name will be generated and stored in the same directory
 with DataBased(dbpath="records.db") as db:
-    tables = [
-        "kitchen_tables(num_legs int, top_material text, shape text, date_added timestamp)"
-    ]
     # A table will only be created if it doesn't exist. create_tables() will not overwrite an existing table.
-    db.create_tables(tables)
+    db.create_table("kitchen_tables", ["num_legs int", "top_material text", "shape text", "date_added timestamp"])
     kitchen_tables = [
         (4, "birch", "round", datetime.now()),
         (3, "oak", "round", datetime.now()),
         (6, "granite", "rectangle", datetime.now()),
     ]
     for kitchen_table in kitchen_tables:
         db.add_row("kitchen_tables", kitchen_table)
@@ -45,67 +43,82 @@
     db.update(
         "kitchen_tables",
         column_to_update="top_material",
         new_value="glass",
         match_criteria=[("num_legs", 3)],
     )
     print(db.get_rows("kitchen_tables", sort_by_column="num_legs"))
-    print(data_to_string(db.get_rows("kitchen_tables"), sort_key="top_material"))
+    print(db.data_to_string(db.get_rows("kitchen_tables"), sort_key="top_material"))
 </pre>
 produces:
 <pre>
 number of rows: 3
 table names: ['kitchen_tables']
 column names: ['num_legs', 'top_material', 'shape', 'date_added']
 [{'num_legs': 6, 'top_material': 'granite', 'shape': 'rectangle', 'date_added': datetime.datetime(2022, 12, 9, 15, 56, 56, 543549)}]
 [{'num_legs': 3, 'top_material': 'oak', 'shape': 'round', 'date_added': datetime.datetime(2022, 12, 9, 15, 56, 56, 543549)}, {'num_legs': 4, 'top_material': 'birch', 'shape': 'round', 'date_added': datetime.datetime(2022, 12, 9, 15, 56, 56, 543549)}]
 [{'num_legs': 4, 'top_material': 'birch', 'shape': 'round', 'date_added': datetime.datetime(2022, 12, 9, 15, 56, 56, 543549)}]
 [{'num_legs': 3, 'top_material': 'glass', 'shape': 'round', 'date_added': datetime.datetime(2022, 12, 9, 15, 56, 56, 543549)}, {'num_legs': 4, 'top_material': 'birch', 'shape': 
 'round', 'date_added': datetime.datetime(2022, 12, 9, 15, 56, 56, 543549)}, {'num_legs': 6, 'top_material': 'granite', 'shape': 'rectangle', 'date_added': datetime.datetime(2022, 12, 9, 15, 56, 56, 543549)}]
 </pre>
-and the final print() call on the data_to_string() function produces:
+and the final `print()` call on `data_to_string()` produces:
 <pre>
 +------------+----------------+-----------+-----------------------------+
 | num_legs   | top_material   | shape     | date_added                  |
 +============+================+===========+=============================+
 | 4          | birch          | round     | 2022-12-14 18:19:31.501745  |
 +------------+----------------+-----------+-----------------------------+
 | 3          | glass          | round     | 2022-12-14 18:19:31.501745  |
 +------------+----------------+-----------+-----------------------------+
 | 6          | granite        | rectangle | 2022-12-14 18:19:31.501745  |
 +------------+----------------+-----------+-----------------------------+
 </pre>
-When a DataBased object is created, if there is no file named "dbmanager.py"
-in the same directory as the specified database file, one will be created from
-a template.<br>
-"dbmanager.py" is a command line script that provides basic database commands,
-but can be tailored to a given database(s).<br>
-Instead of invoking the script over and over with new commands,
-the script is invoked once and will repetedly prompt the user for commands.<br>
-Invoking the script and then passing the "-h/--help" command:
+
+`databased` also comes with an interactive shell called `dbmanager`, which is built from the [argshell](https://github.com/matt-manes/argshell) package.<br>
+It can be launched from the terminal by entering `dbmanager`
 <pre>
->dbmanager.py
-Enter command: -h
-usage: dbmanager.py [-h] [-db DB_NAME] [-i] [-t [TABLES ...]] [-c [COLUMNS ...]] [-f FIND] [-sco] [-d [DELETE ...]] [-u UPDATE UPDATE] [-sb SORT_BY]
+databased\tests>dbmanager
+Searching for database...
+DB options:
+(1) test.db (2) test_bckup.db
+Enter the number of the option to use: 1
+Starting dbmanager (enter help or ? for arg info)...
+based>help
+
+Documented commands (type help <topic>):
+========================================
+add_row  create_table  delete      flush_log  query   size
+backup   customize     drop_table  help       quit    update
+count    dbpath        find        info       search  use_db
+
+>based help update
+Update a column to a new value.
+        Two required positional args: the column to update and the value to update to.
+        Use the -t/--tables flag to limit what tables are updated.
+        Use the -m/--match_pairs flag to specify which rows are updated.
+        >>> based>update username big_chungus -t users -m username lil_chungus
+
+        ^will update the username in the users 'table' to 'big_chungus' where the username is currently 'lil_chungus'^
+Parser help for update:
+usage: dbmanager [-h] [-t [TABLES ...]] [-m [MATCH_PAIRS ...]] [-p] -c COLUMN -v NEW_VALUE
 
 options:
   -h, --help            show this help message and exit
-  -db DBNAME, --dbname DBNAME
-                        Name of database file to use. Required on the first loop if no default is set, but subsequent loops will resuse the same database unless a new one is provided through this arg.
-  -i, --info            Display table names, their respective columns, and how many records they contain. If a -t/--tables arg is passed, just the columns and row count for those tables will be shown.
   -t [TABLES ...], --tables [TABLES ...]
-                        Limits commands to a specific list of tables. Optional for some commands, required for others. If this is the only arg given (besides -db if not already set), the whole table will be printed to the terminal.
-  -c [COLUMNS ...], --columns [COLUMNS ...]
-                        Limits commands to a specific list of columns. Optional for some commands, required for others. If this and -t are the only args given (besides -db if not already set), the whole table will be printed to the
-                        terminal, but with only the columns provided with this arg.
-  -f FIND, --find FIND  A substring to search the database for. If a -c/--columns arg(s) is not given, the values will be matched against all columns. Similarly, if a -t/--tables arg(s) is not given, the values will be searched for in
-                        all tables.
-  -sco, --show_count_only
-                        Show the number of results returned by -f/--find, but don't print the results to the terminal.
-  -d [DELETE ...], --delete [DELETE ...]
-                        A list of values to be deleted from the database. A -c/--columns arg must be supplied. A -t/--tables arg must be supplied.
-  -u UPDATE UPDATE, --update UPDATE UPDATE
-                        Update a record in the database. Expects two arguments: the current value and the new value. A -c/--columns arg must be supplied. A -t/--tables arg must be supplied.
-  -sb SORT_BY, --sort_by SORT_BY
-                        Column to sort results by.
-Enter command:
-</pre>
+                        Limits command to a specific list of tables
+  -m [MATCH_PAIRS ...], --match_pairs [MATCH_PAIRS ...]
+                        Pairs of columns and values to use for narrowing the scope of row operations. i.e. 'find -t users -m name Bob state Alaska last_login *' will print all rows from the users table that have the name Bob, are from the state Alaska, and last logged in at any
+                        date.
+  -p, --partial_matching
+                        When selecting rows using a string, the string can be a substring instead of an exact match. i.e. "-t names -m first theo" only returns rows from names where the first name is exactly 'theo'. "-t names -m first theo -p" would return rows with first names
+                        of 'theo', but also rows with names like 'theodore'.
+  -c COLUMN, --column COLUMN
+                        The column to update.
+  -v NEW_VALUE, --new_value NEW_VALUE
+                        The new value to update with.
+based>
+</pre>
+The `customize` command can be used to generate a template file in the current directory that subclasses `DBManager`.<br>
+This allows for project specific modification/extension of available commands.
+
+
+
```

### Comparing `databased-1.4.5/pyproject.toml` & `databased-1.5.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "databased"
 authors = [{name="Matt Manes"}]
 description = "Wrapper for the standard library Sqlite3 module to make setting up and using a database quicker and easier."
-version = "1.4.5"
+version = "1.5.0"
 requires-python = ">=3.10"
-dependencies = ["pandas", "tabulate", "pytest"]
+dependencies = ["pandas", "tabulate", "pytest", "argshell", "pathier"]
 readme = "README.md"
 keywords = [
     "database",
     "sqlite",
     "sqlite3"
 ]
 classifiers = [
@@ -34,8 +34,10 @@
 
 [tool.hatch.build.targets.sdist]
 exclude = [
     ".coverage",
     ".pytest_cache",
     ".vscode",
     "tests"
-]
+]
+[project.scripts]
+dbmanager = "databased.dbmanager:main"
```

### Comparing `databased-1.4.5/PKG-INFO` & `databased-1.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 Metadata-Version: 2.1
 Name: databased
-Version: 1.4.5
+Version: 1.5.0
 Summary: Wrapper for the standard library Sqlite3 module to make setting up and using a database quicker and easier.
 Project-URL: Homepage, https://github.com/matt-manes/databased
 Project-URL: Documentation, https://github.com/matt-manes/databased/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/databased/tree/main/src/databased
 Author: Matt Manes
 License-File: LICENSE.txt
 Keywords: database,sqlite,sqlite3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
+Requires-Dist: argshell
 Requires-Dist: pandas
+Requires-Dist: pathier
 Requires-Dist: pytest
 Requires-Dist: tabulate
 Description-Content-Type: text/markdown
 
 # Databased
 Databased is a package that wraps the standard library Sqlite3 module to make setting up and using a database quicker and easier.<br>
+
 Install with:
 <pre>pip install databased</pre>
-databased is a package that wraps the standard library Sqlite3 module to largely avoid writing queries except for table definitions.<br>
-It consists of the class DataBased and an additional function for displaying information in a grid called data_to_string.<br>
+
+`databased` is a package that wraps the standard library Sqlite3 module to largely avoid writing queries except for table definitions (there is a `query` function that can be used to directly excute queries).<br>
+It primarily consists of the class `DataBased`.<br>
 The DataBased class contains functions for creating databases and tables; inserting, updating, and deleting rows; 
 as well as retrieving data and schema information.<br>
-The data_to_string function uses the [tabulate](https://pypi.org/project/tabulate/) to generate a grid as a string from a list of dictionaries.<br>
+
+There is also a static method called `data_to_string` which uses [tabulate](https://pypi.org/project/tabulate/) to generate a printable grid from a list of dictionaries.<br>
 By default, data_to_string will automatically wrap the width of columns to fit within the current terminal window.<br><br>
-Member functions that require a database connection will
-automatically create one when called if one isn't already open,
-but a manual call to self.close() needs to be called in order to
-save the database file and release the connection.<br>
-If a context manager is used, like in the following example, you don't need to worry about manually opening, saving, or closing the database.<br>
+Member functions that require a database connection will automatically create one when called if one isn't already open.<br>
+If you create a class that inherits from `DataBased`, you will need to decorate member functions that access the database with `@_connect`.<br>
+Unless `DataBased` is used with a context manager, you will need to manually call the `close()` function to close the connection and save the database.
 <br>
 Usage:
 <pre>
-from databased import DataBased, data_to_string
+from databased import DataBased
 from datetime import datetime
 
 # if the .db file specified doesn't exist, it will be created
 # a log file with the same name will be generated and stored in the same directory
 with DataBased(dbpath="records.db") as db:
-    tables = [
-        "kitchen_tables(num_legs int, top_material text, shape text, date_added timestamp)"
-    ]
     # A table will only be created if it doesn't exist. create_tables() will not overwrite an existing table.
-    db.create_tables(tables)
+    db.create_table("kitchen_tables", ["num_legs int", "top_material text", "shape text", "date_added timestamp"])
     kitchen_tables = [
         (4, "birch", "round", datetime.now()),
         (3, "oak", "round", datetime.now()),
         (6, "granite", "rectangle", datetime.now()),
     ]
     for kitchen_table in kitchen_tables:
         db.add_row("kitchen_tables", kitchen_table)
@@ -64,67 +64,82 @@
     db.update(
         "kitchen_tables",
         column_to_update="top_material",
         new_value="glass",
         match_criteria=[("num_legs", 3)],
     )
     print(db.get_rows("kitchen_tables", sort_by_column="num_legs"))
-    print(data_to_string(db.get_rows("kitchen_tables"), sort_key="top_material"))
+    print(db.data_to_string(db.get_rows("kitchen_tables"), sort_key="top_material"))
 </pre>
 produces:
 <pre>
 number of rows: 3
 table names: ['kitchen_tables']
 column names: ['num_legs', 'top_material', 'shape', 'date_added']
 [{'num_legs': 6, 'top_material': 'granite', 'shape': 'rectangle', 'date_added': datetime.datetime(2022, 12, 9, 15, 56, 56, 543549)}]
 [{'num_legs': 3, 'top_material': 'oak', 'shape': 'round', 'date_added': datetime.datetime(2022, 12, 9, 15, 56, 56, 543549)}, {'num_legs': 4, 'top_material': 'birch', 'shape': 'round', 'date_added': datetime.datetime(2022, 12, 9, 15, 56, 56, 543549)}]
 [{'num_legs': 4, 'top_material': 'birch', 'shape': 'round', 'date_added': datetime.datetime(2022, 12, 9, 15, 56, 56, 543549)}]
 [{'num_legs': 3, 'top_material': 'glass', 'shape': 'round', 'date_added': datetime.datetime(2022, 12, 9, 15, 56, 56, 543549)}, {'num_legs': 4, 'top_material': 'birch', 'shape': 
 'round', 'date_added': datetime.datetime(2022, 12, 9, 15, 56, 56, 543549)}, {'num_legs': 6, 'top_material': 'granite', 'shape': 'rectangle', 'date_added': datetime.datetime(2022, 12, 9, 15, 56, 56, 543549)}]
 </pre>
-and the final print() call on the data_to_string() function produces:
+and the final `print()` call on `data_to_string()` produces:
 <pre>
 +------------+----------------+-----------+-----------------------------+
 | num_legs   | top_material   | shape     | date_added                  |
 +============+================+===========+=============================+
 | 4          | birch          | round     | 2022-12-14 18:19:31.501745  |
 +------------+----------------+-----------+-----------------------------+
 | 3          | glass          | round     | 2022-12-14 18:19:31.501745  |
 +------------+----------------+-----------+-----------------------------+
 | 6          | granite        | rectangle | 2022-12-14 18:19:31.501745  |
 +------------+----------------+-----------+-----------------------------+
 </pre>
-When a DataBased object is created, if there is no file named "dbmanager.py"
-in the same directory as the specified database file, one will be created from
-a template.<br>
-"dbmanager.py" is a command line script that provides basic database commands,
-but can be tailored to a given database(s).<br>
-Instead of invoking the script over and over with new commands,
-the script is invoked once and will repetedly prompt the user for commands.<br>
-Invoking the script and then passing the "-h/--help" command:
+
+`databased` also comes with an interactive shell called `dbmanager`, which is built from the [argshell](https://github.com/matt-manes/argshell) package.<br>
+It can be launched from the terminal by entering `dbmanager`
 <pre>
->dbmanager.py
-Enter command: -h
-usage: dbmanager.py [-h] [-db DB_NAME] [-i] [-t [TABLES ...]] [-c [COLUMNS ...]] [-f FIND] [-sco] [-d [DELETE ...]] [-u UPDATE UPDATE] [-sb SORT_BY]
+databased\tests>dbmanager
+Searching for database...
+DB options:
+(1) test.db (2) test_bckup.db
+Enter the number of the option to use: 1
+Starting dbmanager (enter help or ? for arg info)...
+based>help
+
+Documented commands (type help <topic>):
+========================================
+add_row  create_table  delete      flush_log  query   size
+backup   customize     drop_table  help       quit    update
+count    dbpath        find        info       search  use_db
+
+>based help update
+Update a column to a new value.
+        Two required positional args: the column to update and the value to update to.
+        Use the -t/--tables flag to limit what tables are updated.
+        Use the -m/--match_pairs flag to specify which rows are updated.
+        >>> based>update username big_chungus -t users -m username lil_chungus
+
+        ^will update the username in the users 'table' to 'big_chungus' where the username is currently 'lil_chungus'^
+Parser help for update:
+usage: dbmanager [-h] [-t [TABLES ...]] [-m [MATCH_PAIRS ...]] [-p] -c COLUMN -v NEW_VALUE
 
 options:
   -h, --help            show this help message and exit
-  -db DBNAME, --dbname DBNAME
-                        Name of database file to use. Required on the first loop if no default is set, but subsequent loops will resuse the same database unless a new one is provided through this arg.
-  -i, --info            Display table names, their respective columns, and how many records they contain. If a -t/--tables arg is passed, just the columns and row count for those tables will be shown.
   -t [TABLES ...], --tables [TABLES ...]
-                        Limits commands to a specific list of tables. Optional for some commands, required for others. If this is the only arg given (besides -db if not already set), the whole table will be printed to the terminal.
-  -c [COLUMNS ...], --columns [COLUMNS ...]
-                        Limits commands to a specific list of columns. Optional for some commands, required for others. If this and -t are the only args given (besides -db if not already set), the whole table will be printed to the
-                        terminal, but with only the columns provided with this arg.
-  -f FIND, --find FIND  A substring to search the database for. If a -c/--columns arg(s) is not given, the values will be matched against all columns. Similarly, if a -t/--tables arg(s) is not given, the values will be searched for in
-                        all tables.
-  -sco, --show_count_only
-                        Show the number of results returned by -f/--find, but don't print the results to the terminal.
-  -d [DELETE ...], --delete [DELETE ...]
-                        A list of values to be deleted from the database. A -c/--columns arg must be supplied. A -t/--tables arg must be supplied.
-  -u UPDATE UPDATE, --update UPDATE UPDATE
-                        Update a record in the database. Expects two arguments: the current value and the new value. A -c/--columns arg must be supplied. A -t/--tables arg must be supplied.
-  -sb SORT_BY, --sort_by SORT_BY
-                        Column to sort results by.
-Enter command:
-</pre>
+                        Limits command to a specific list of tables
+  -m [MATCH_PAIRS ...], --match_pairs [MATCH_PAIRS ...]
+                        Pairs of columns and values to use for narrowing the scope of row operations. i.e. 'find -t users -m name Bob state Alaska last_login *' will print all rows from the users table that have the name Bob, are from the state Alaska, and last logged in at any
+                        date.
+  -p, --partial_matching
+                        When selecting rows using a string, the string can be a substring instead of an exact match. i.e. "-t names -m first theo" only returns rows from names where the first name is exactly 'theo'. "-t names -m first theo -p" would return rows with first names
+                        of 'theo', but also rows with names like 'theodore'.
+  -c COLUMN, --column COLUMN
+                        The column to update.
+  -v NEW_VALUE, --new_value NEW_VALUE
+                        The new value to update with.
+based>
+</pre>
+The `customize` command can be used to generate a template file in the current directory that subclasses `DBManager`.<br>
+This allows for project specific modification/extension of available commands.
+
+
+
```

