# Comparing `tmp/packagelister-1.3.0.tar.gz` & `tmp/packagelister-1.3.1.tar.gz`

## Comparing `packagelister-1.3.0.tar` & `packagelister-1.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 packagelister-1.3.0/CHANGELOG.md
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 packagelister-1.3.0/docs/index.html
--rw-r--r--   0        0        0    34264 2020-02-02 00:00:00.000000 packagelister-1.3.0/docs/packagelister.html
--rw-r--r--   0        0        0    23684 2020-02-02 00:00:00.000000 packagelister-1.3.0/docs/search.js
--rw-r--r--   0        0        0    69384 2020-02-02 00:00:00.000000 packagelister-1.3.0/docs/packagelister/packagelister.html
--rw-r--r--   0        0        0    74342 2020-02-02 00:00:00.000000 packagelister-1.3.0/docs/packagelister/packagelister_cli.html
--rw-r--r--   0        0        0    56419 2020-02-02 00:00:00.000000 packagelister-1.3.0/docs/packagelister/whouses.html
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 packagelister-1.3.0/src/packagelister/__init__.py
--rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 packagelister-1.3.0/src/packagelister/packagelister.py
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 packagelister-1.3.0/src/packagelister/packagelister_cli.py
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 packagelister-1.3.0/src/packagelister/whouses.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 packagelister-1.3.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 packagelister-1.3.0/LICENSE.txt
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 packagelister-1.3.0/README.md
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 packagelister-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 packagelister-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 packagelister-1.3.1/CHANGELOG.md
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 packagelister-1.3.1/docs/index.html
+-rw-r--r--   0        0        0    34264 2020-02-02 00:00:00.000000 packagelister-1.3.1/docs/packagelister.html
+-rw-r--r--   0        0        0    23684 2020-02-02 00:00:00.000000 packagelister-1.3.1/docs/search.js
+-rw-r--r--   0        0        0    69236 2020-02-02 00:00:00.000000 packagelister-1.3.1/docs/packagelister/packagelister.html
+-rw-r--r--   0        0        0    74342 2020-02-02 00:00:00.000000 packagelister-1.3.1/docs/packagelister/packagelister_cli.html
+-rw-r--r--   0        0        0    56419 2020-02-02 00:00:00.000000 packagelister-1.3.1/docs/packagelister/whouses.html
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 packagelister-1.3.1/src/packagelister/__init__.py
+-rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 packagelister-1.3.1/src/packagelister/packagelister.py
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 packagelister-1.3.1/src/packagelister/packagelister_cli.py
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 packagelister-1.3.1/src/packagelister/whouses.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 packagelister-1.3.1/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 packagelister-1.3.1/LICENSE.txt
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 packagelister-1.3.1/README.md
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 packagelister-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 packagelister-1.3.1/PKG-INFO
```

### Comparing `packagelister-1.3.0/CHANGELOG.md` & `packagelister-1.3.1/CHANGELOG.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,28 @@
 # Changelog
 
-## 1.2.0 (2023-04-12)
+## 1.3.0 (2023-04-15)
+
+#### New Features
+
+* add whosuses to scripts table
+#### Refactorings
+
+* move bulk of work into seperate function
+
+
+## v1.2.0 (2023-04-12)
 
 #### New Features
 
 * add switch to add package versions with chosen relation when generating requirements.txt
+#### Others
+
+* build v1.2.0
+* update changelog
 
 
 ## v1.1.3 (2023-03-22)
 
 #### Others
 
 * build v1.1.3
```

### Comparing `packagelister-1.3.0/docs/packagelister.html` & `packagelister-1.3.1/docs/packagelister.html`

 * *Files identical despite different names*

### Comparing `packagelister-1.3.0/docs/search.js` & `packagelister-1.3.1/docs/search.js`

 * *Files identical despite different names*

### Comparing `packagelister-1.3.0/docs/packagelister/packagelister.html` & `packagelister-1.3.1/docs/packagelister/packagelister.html`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 </span><span id="L-34"><a href="#L-34"><span class="linenos">34</span></a>        <span class="k">return</span> <span class="p">{}</span>
 </span><span id="L-35"><a href="#L-35"><span class="linenos">35</span></a>    <span class="c1"># You can scan a non python file one at a time if you reeeally want to.</span>
 </span><span id="L-36"><a href="#L-36"><span class="linenos">36</span></a>    <span class="k">if</span> <span class="n">project_dir</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
 </span><span id="L-37"><a href="#L-37"><span class="linenos">37</span></a>        <span class="n">files</span> <span class="o">=</span> <span class="p">[</span><span class="n">project_dir</span><span class="p">]</span>
 </span><span id="L-38"><a href="#L-38"><span class="linenos">38</span></a>    <span class="k">else</span><span class="p">:</span>
 </span><span id="L-39"><a href="#L-39"><span class="linenos">39</span></a>        <span class="n">files</span> <span class="o">=</span> <span class="p">[</span><span class="n">file</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">crawl</span><span class="p">(</span><span class="n">project_dir</span><span class="p">)</span> <span class="k">if</span> <span class="n">file</span><span class="o">.</span><span class="n">suffix</span> <span class="o">==</span> <span class="s2">&quot;.py&quot;</span><span class="p">]</span>
 </span><span id="L-40"><a href="#L-40"><span class="linenos">40</span></a>
-</span><span id="L-41"><a href="#L-41"><span class="linenos">41</span></a>    <span class="n">bar</span> <span class="o">=</span> <span class="n">ProgBar</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="n">files</span><span class="p">)</span> <span class="o">-</span> <span class="mi">1</span><span class="p">,</span> <span class="n">width_ratio</span><span class="o">=</span><span class="mf">0.33</span><span class="p">)</span>
+</span><span id="L-41"><a href="#L-41"><span class="linenos">41</span></a>    <span class="n">bar</span> <span class="o">=</span> <span class="n">ProgBar</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="n">files</span><span class="p">),</span> <span class="n">width_ratio</span><span class="o">=</span><span class="mf">0.33</span><span class="p">)</span>
 </span><span id="L-42"><a href="#L-42"><span class="linenos">42</span></a>    <span class="c1"># If scanning one file, the progress bar will show 0% complete if bar.counter == 0</span>
 </span><span id="L-43"><a href="#L-43"><span class="linenos">43</span></a>    <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">files</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
 </span><span id="L-44"><a href="#L-44"><span class="linenos">44</span></a>        <span class="n">bar</span><span class="o">.</span><span class="n">counter</span> <span class="o">=</span> <span class="mi">1</span>
 </span><span id="L-45"><a href="#L-45"><span class="linenos">45</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="p">{}</span>
 </span><span id="L-46"><a href="#L-46"><span class="linenos">46</span></a>    <span class="n">standard_lib</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">sys</span><span class="o">.</span><span class="n">stdlib_module_names</span><span class="p">)</span> <span class="k">if</span> <span class="ow">not</span> <span class="n">include_builtins</span> <span class="k">else</span> <span class="p">[]</span>
 </span><span id="L-47"><a href="#L-47"><span class="linenos">47</span></a>    <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">files</span><span class="p">:</span>
 </span><span id="L-48"><a href="#L-48"><span class="linenos">48</span></a>        <span class="n">bar</span><span class="o">.</span><span class="n">display</span><span class="p">(</span><span class="n">suffix</span><span class="o">=</span><span class="sa">f</span><span class="s2">&quot;Scanning </span><span class="si">{</span><span class="n">file</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
@@ -170,15 +170,15 @@
 </span><span id="scan-35"><a href="#scan-35"><span class="linenos">35</span></a>        <span class="k">return</span> <span class="p">{}</span>
 </span><span id="scan-36"><a href="#scan-36"><span class="linenos">36</span></a>    <span class="c1"># You can scan a non python file one at a time if you reeeally want to.</span>
 </span><span id="scan-37"><a href="#scan-37"><span class="linenos">37</span></a>    <span class="k">if</span> <span class="n">project_dir</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
 </span><span id="scan-38"><a href="#scan-38"><span class="linenos">38</span></a>        <span class="n">files</span> <span class="o">=</span> <span class="p">[</span><span class="n">project_dir</span><span class="p">]</span>
 </span><span id="scan-39"><a href="#scan-39"><span class="linenos">39</span></a>    <span class="k">else</span><span class="p">:</span>
 </span><span id="scan-40"><a href="#scan-40"><span class="linenos">40</span></a>        <span class="n">files</span> <span class="o">=</span> <span class="p">[</span><span class="n">file</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">crawl</span><span class="p">(</span><span class="n">project_dir</span><span class="p">)</span> <span class="k">if</span> <span class="n">file</span><span class="o">.</span><span class="n">suffix</span> <span class="o">==</span> <span class="s2">&quot;.py&quot;</span><span class="p">]</span>
 </span><span id="scan-41"><a href="#scan-41"><span class="linenos">41</span></a>
-</span><span id="scan-42"><a href="#scan-42"><span class="linenos">42</span></a>    <span class="n">bar</span> <span class="o">=</span> <span class="n">ProgBar</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="n">files</span><span class="p">)</span> <span class="o">-</span> <span class="mi">1</span><span class="p">,</span> <span class="n">width_ratio</span><span class="o">=</span><span class="mf">0.33</span><span class="p">)</span>
+</span><span id="scan-42"><a href="#scan-42"><span class="linenos">42</span></a>    <span class="n">bar</span> <span class="o">=</span> <span class="n">ProgBar</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="n">files</span><span class="p">),</span> <span class="n">width_ratio</span><span class="o">=</span><span class="mf">0.33</span><span class="p">)</span>
 </span><span id="scan-43"><a href="#scan-43"><span class="linenos">43</span></a>    <span class="c1"># If scanning one file, the progress bar will show 0% complete if bar.counter == 0</span>
 </span><span id="scan-44"><a href="#scan-44"><span class="linenos">44</span></a>    <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">files</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
 </span><span id="scan-45"><a href="#scan-45"><span class="linenos">45</span></a>        <span class="n">bar</span><span class="o">.</span><span class="n">counter</span> <span class="o">=</span> <span class="mi">1</span>
 </span><span id="scan-46"><a href="#scan-46"><span class="linenos">46</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="p">{}</span>
 </span><span id="scan-47"><a href="#scan-47"><span class="linenos">47</span></a>    <span class="n">standard_lib</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">sys</span><span class="o">.</span><span class="n">stdlib_module_names</span><span class="p">)</span> <span class="k">if</span> <span class="ow">not</span> <span class="n">include_builtins</span> <span class="k">else</span> <span class="p">[]</span>
 </span><span id="scan-48"><a href="#scan-48"><span class="linenos">48</span></a>    <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">files</span><span class="p">:</span>
 </span><span id="scan-49"><a href="#scan-49"><span class="linenos">49</span></a>        <span class="n">bar</span><span class="o">.</span><span class="n">display</span><span class="p">(</span><span class="n">suffix</span><span class="o">=</span><span class="sa">f</span><span class="s2">&quot;Scanning </span><span class="si">{</span><span class="n">file</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
```

#### html2text {}

```diff
@@ -46,15 +46,15 @@
 34        return {}
 35    # You can scan a non python file one at a time if you reeeally want to.
 36    if project_dir.is_file():
 37        files = [project_dir]
 38    else:
 39        files = [file for file in crawl(project_dir) if file.suffix == ".py"]
 40
-41    bar = ProgBar(len(files) - 1, width_ratio=0.33)
+41    bar = ProgBar(len(files), width_ratio=0.33)
 42    # If scanning one file, the progress bar will show 0% complete if
 bar.counter == 0
 43    if len(files) == 1:
 44        bar.counter = 1
 45    packages = {}
 46    standard_lib = list(sys.stdlib_module_names) if not include_builtins else
 []
@@ -121,15 +121,15 @@
 35        return {}
 36    # You can scan a non python file one at a time if you reeeally want to.
 37    if project_dir.is_file():
 38        files = [project_dir]
 39    else:
 40        files = [file for file in crawl(project_dir) if file.suffix == ".py"]
 41
-42    bar = ProgBar(len(files) - 1, width_ratio=0.33)
+42    bar = ProgBar(len(files), width_ratio=0.33)
 43    # If scanning one file, the progress bar will show 0% complete if
 bar.counter == 0
 44    if len(files) == 1:
 45        bar.counter = 1
 46    packages = {}
 47    standard_lib = list(sys.stdlib_module_names) if not include_builtins else
 []
```

### Comparing `packagelister-1.3.0/docs/packagelister/packagelister_cli.html` & `packagelister-1.3.1/docs/packagelister/packagelister_cli.html`

 * *Files identical despite different names*

### Comparing `packagelister-1.3.0/docs/packagelister/whouses.html` & `packagelister-1.3.1/docs/packagelister/whouses.html`

 * *Files identical despite different names*

### Comparing `packagelister-1.3.0/src/packagelister/packagelister.py` & `packagelister-1.3.1/src/packagelister/packagelister.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         return {}
     # You can scan a non python file one at a time if you reeeally want to.
     if project_dir.is_file():
         files = [project_dir]
     else:
         files = [file for file in crawl(project_dir) if file.suffix == ".py"]
 
-    bar = ProgBar(len(files) - 1, width_ratio=0.33)
+    bar = ProgBar(len(files), width_ratio=0.33)
     # If scanning one file, the progress bar will show 0% complete if bar.counter == 0
     if len(files) == 1:
         bar.counter = 1
     packages = {}
     standard_lib = list(sys.stdlib_module_names) if not include_builtins else []
     for file in files:
         bar.display(suffix=f"Scanning {file.name}")
```

### Comparing `packagelister-1.3.0/src/packagelister/packagelister_cli.py` & `packagelister-1.3.1/src/packagelister/packagelister_cli.py`

 * *Files identical despite different names*

### Comparing `packagelister-1.3.0/src/packagelister/whouses.py` & `packagelister-1.3.1/src/packagelister/whouses.py`

 * *Files identical despite different names*

### Comparing `packagelister-1.3.0/LICENSE.txt` & `packagelister-1.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `packagelister-1.3.0/README.md` & `packagelister-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `packagelister-1.3.0/pyproject.toml` & `packagelister-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 00000070: 0d0a 6175 7468 6f72 7320 3d20 5b7b 6e61  ..authors = [{na
 00000080: 6d65 3d22 4d61 7474 204d 616e 6573 227d  me="Matt Manes"}
 00000090: 5d0d 0a64 6573 6372 6970 7469 6f6e 203d  ]..description =
 000000a0: 2022 4465 7465 726d 696e 6520 7768 6174   "Determine what
 000000b0: 2033 7264 2d70 6172 7479 2070 6163 6b61   3rd-party packa
 000000c0: 6765 7320 6120 7072 6f6a 6563 7420 696d  ges a project im
 000000d0: 706f 7274 732e 220d 0a76 6572 7369 6f6e  ports."..version
-000000e0: 203d 2022 312e 332e 3022 0d0a 7265 7175   = "1.3.0"..requ
+000000e0: 203d 2022 312e 332e 3122 0d0a 7265 7175   = "1.3.1"..requ
 000000f0: 6972 6573 2d70 7974 686f 6e20 3d20 223e  ires-python = ">
 00000100: 3d33 2e31 3022 0d0a 6465 7065 6e64 656e  =3.10"..dependen
 00000110: 6369 6573 203d 205b 2270 6174 6863 7261  cies = ["pathcra
 00000120: 776c 6572 222c 2022 7072 696e 7462 7564  wler", "printbud
 00000130: 6469 6573 222c 2022 7079 7465 7374 222c  dies", "pytest",
 00000140: 2022 7061 7468 6965 7222 5d0d 0a72 6561   "pathier"]..rea
 00000150: 646d 6520 3d20 2252 4541 444d 452e 6d64  dme = "README.md
```

### Comparing `packagelister-1.3.0/PKG-INFO` & `packagelister-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packagelister
-Version: 1.3.0
+Version: 1.3.1
 Summary: Determine what 3rd-party packages a project imports.
 Project-URL: Homepage, https://github.com/matt-manes/packagelister
 Project-URL: Documentation, https://github.com/matt-manes/packagelister/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/packagelister/tree/main/src/packagelister
 Author: Matt Manes
 License-File: LICENSE.txt
 Keywords: import,module,package
```

