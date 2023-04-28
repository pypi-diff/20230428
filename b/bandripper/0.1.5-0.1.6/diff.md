# Comparing `tmp/bandripper-0.1.5.tar.gz` & `tmp/bandripper-0.1.6.tar.gz`

## Comparing `bandripper-0.1.5.tar` & `bandripper-0.1.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 bandripper-0.1.5/CHANGELOG.md
--rw-r--r--   0        0        0    33565 2020-02-02 00:00:00.000000 bandripper-0.1.5/docs/bandripper.html
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bandripper-0.1.5/docs/index.html
--rw-r--r--   0        0        0    30351 2020-02-02 00:00:00.000000 bandripper-0.1.5/docs/search.js
--rw-r--r--   0        0        0   228834 2020-02-02 00:00:00.000000 bandripper-0.1.5/docs/bandripper/bandripper.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bandripper-0.1.5/src/bandripper/__init__.py
--rw-r--r--   0        0        0     9624 2020-02-02 00:00:00.000000 bandripper-0.1.5/src/bandripper/bandripper.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 bandripper-0.1.5/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 bandripper-0.1.5/LICENSE.txt
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 bandripper-0.1.5/README.md
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 bandripper-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 bandripper-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 bandripper-0.1.6/CHANGELOG.md
+-rw-r--r--   0        0        0    33565 2020-02-02 00:00:00.000000 bandripper-0.1.6/docs/bandripper.html
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bandripper-0.1.6/docs/index.html
+-rw-r--r--   0        0        0    30351 2020-02-02 00:00:00.000000 bandripper-0.1.6/docs/search.js
+-rw-r--r--   0        0        0   231747 2020-02-02 00:00:00.000000 bandripper-0.1.6/docs/bandripper/bandripper.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bandripper-0.1.6/src/bandripper/__init__.py
+-rw-r--r--   0        0        0     9756 2020-02-02 00:00:00.000000 bandripper-0.1.6/src/bandripper/bandripper.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 bandripper-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 bandripper-0.1.6/LICENSE.txt
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 bandripper-0.1.6/README.md
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 bandripper-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 bandripper-0.1.6/PKG-INFO
```

### Comparing `bandripper-0.1.5/CHANGELOG.md` & `bandripper-0.1.6/CHANGELOG.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,25 @@
 # Changelog
 
-## 0.1.4 (2023-03-31)
+## 0.1.5 (2023-04-16)
+
+#### Fixes
+
+* update noiftimer usage
+
+
+## v0.1.4 (2023-03-31)
 
 #### Refactorings
 
 * change timer.current_elapsed_time() calls to timer.elapsed_str
+#### Others
+
+* build v0.1.4
+* update changelog
 
 
 ## v0.1.3 (2023-03-22)
 
 #### Fixes
 
 * fix not passing cli switch to constructors
```

### Comparing `bandripper-0.1.5/docs/bandripper.html` & `bandripper-0.1.6/docs/bandripper.html`

 * *Files identical despite different names*

### Comparing `bandripper-0.1.5/docs/search.js` & `bandripper-0.1.6/docs/search.js`

 * *Files identical despite different names*

### Comparing `bandripper-0.1.5/docs/bandripper/bandripper.html` & `bandripper-0.1.6/docs/bandripper/bandripper.html`

 * *Files 0% similar despite different names*

```diff
@@ -257,156 +257,159 @@
 </span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>    <span class="k">def</span> <span class="nf">rip</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
 </span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>        <span class="sd">&quot;&quot;&quot;Download and save the album tracks and album art.&quot;&quot;&quot;</span>
 </span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
 </span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;No public tracks available for </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
 </span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>            <span class="k">return</span> <span class="kc">None</span>
 </span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">make_save_path</span><span class="p">()</span>
 </span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">download_album_art</span><span class="p">()</span>
-</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>        <span class="n">bar</span> <span class="o">=</span> <span class="n">ProgBar</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span><span class="p">)</span> <span class="o">-</span> <span class="mi">1</span><span class="p">,</span> <span class="n">width_ratio</span><span class="o">=</span><span class="mf">0.5</span><span class="p">)</span>
-</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>        <span class="n">fails</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">overwrite</span><span class="p">:</span>
-</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>                <span class="n">track</span> <span class="k">for</span> <span class="n">track</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span> <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">track_exists</span><span class="p">(</span><span class="n">track</span><span class="p">)</span>
-</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>            <span class="p">]</span>
-</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>        <span class="k">for</span> <span class="n">track</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span><span class="p">:</span>
-</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>            <span class="n">bar</span><span class="o">.</span><span class="n">display</span><span class="p">(</span>
-</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>                <span class="n">suffix</span><span class="o">=</span><span class="sa">f</span><span class="s2">&quot;Downloading </span><span class="si">{</span><span class="n">track</span><span class="o">.</span><span class="n">title</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span>
-</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>                <span class="n">counter_override</span><span class="o">=</span><span class="mi">1</span> <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span> <span class="k">else</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>            <span class="p">)</span>
-</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>            <span class="k">try</span><span class="p">:</span>
-</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>                <span class="n">content</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_track_content</span><span class="p">(</span><span class="n">track</span><span class="o">.</span><span class="n">url</span><span class="p">)</span>
-</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">save_track</span><span class="p">(</span>
-</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>                    <span class="n">track</span><span class="o">.</span><span class="n">title</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">no_track_number</span> <span class="k">else</span> <span class="n">track</span><span class="o">.</span><span class="n">numbered_title</span><span class="p">,</span>
-</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>                    <span class="n">content</span><span class="p">,</span>
-</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>                <span class="p">)</span>
-</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>                <span class="n">fails</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="n">track</span><span class="p">,</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">)))</span>
-</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Finished downloading </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="si">}</span><span class="s2"> in </span><span class="si">{</span><span class="n">bar</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">elapsed_str</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>        <span class="k">if</span> <span class="n">fails</span><span class="p">:</span>
-</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;The following tracks failed to download:&quot;</span><span class="p">)</span>
-</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>            <span class="k">for</span> <span class="n">fail</span> <span class="ow">in</span> <span class="n">fails</span><span class="p">:</span>
-</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">fail</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">title</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">fail</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a>
-</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a>
-</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a><span class="k">class</span> <span class="nc">BandRipper</span><span class="p">:</span>
-</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
-</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">band_url</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">no_track_number</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a>    <span class="p">):</span>
-</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">band_url</span> <span class="o">=</span> <span class="n">band_url</span>
-</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">albums</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>        <span class="k">for</span> <span class="n">url</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_album_urls</span><span class="p">(</span><span class="n">band_url</span><span class="p">):</span>
-</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a>            <span class="k">try</span><span class="p">:</span>
-</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">AlbumRipper</span><span class="p">(</span><span class="n">url</span><span class="p">,</span> <span class="n">no_track_number</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">))</span>
-</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>                <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
-</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>
-</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a>    <span class="k">def</span> <span class="nf">get_album_urls</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">band_url</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
-</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>        <span class="sd">&quot;&quot;&quot;Get album urls from the main bandcamp url.&quot;&quot;&quot;</span>
-</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Fetching discography from </span><span class="si">{</span><span class="n">band_url</span><span class="si">}</span><span class="s2">...&quot;</span><span class="p">)</span>
-</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a>        <span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">band_url</span><span class="p">,</span> <span class="n">headers</span><span class="o">=</span><span class="n">whosyouragent</span><span class="o">.</span><span class="n">get_agent</span><span class="p">(</span><span class="n">as_dict</span><span class="o">=</span><span class="kc">True</span><span class="p">))</span>
-</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a>        <span class="k">if</span> <span class="n">response</span><span class="o">.</span><span class="n">status_code</span> <span class="o">!=</span> <span class="mi">200</span><span class="p">:</span>
-</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>            <span class="k">raise</span> <span class="ne">RuntimeError</span><span class="p">(</span>
-</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a>                <span class="sa">f</span><span class="s2">&quot;Getting </span><span class="si">{</span><span class="n">band_url</span><span class="si">}</span><span class="s2"> failed with status code </span><span class="si">{</span><span class="n">response</span><span class="o">.</span><span class="n">status_code</span><span class="si">}</span><span class="s2">.&quot;</span>
-</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>            <span class="p">)</span>
-</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>        <span class="n">soup</span> <span class="o">=</span> <span class="n">BeautifulSoup</span><span class="p">(</span><span class="n">response</span><span class="o">.</span><span class="n">text</span><span class="p">,</span> <span class="s2">&quot;html.parser&quot;</span><span class="p">)</span>
-</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>        <span class="n">grid</span> <span class="o">=</span> <span class="n">soup</span><span class="o">.</span><span class="n">find</span><span class="p">(</span><span class="s2">&quot;ol&quot;</span><span class="p">,</span> <span class="n">attrs</span><span class="o">=</span><span class="p">{</span><span class="s2">&quot;id&quot;</span><span class="p">:</span> <span class="s2">&quot;music-grid&quot;</span><span class="p">})</span>
-</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>        <span class="n">parsed_url</span> <span class="o">=</span> <span class="n">urlparse</span><span class="p">(</span><span class="n">band_url</span><span class="p">)</span>
-</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a>        <span class="n">base_url</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;https://</span><span class="si">{</span><span class="n">parsed_url</span><span class="o">.</span><span class="n">netloc</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">base_url</span> <span class="o">+</span> <span class="n">album</span><span class="o">.</span><span class="n">a</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;href&quot;</span><span class="p">)</span> <span class="k">for</span> <span class="n">album</span> <span class="ow">in</span> <span class="n">grid</span><span class="o">.</span><span class="n">find_all</span><span class="p">(</span><span class="s2">&quot;li&quot;</span><span class="p">)]</span>
-</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a>
-</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>    <span class="k">def</span> <span class="nf">rip</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>        <span class="nb">print</span><span class="p">(</span>
-</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>            <span class="sa">f</span><span class="s2">&quot;Downloading </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">)</span><span class="si">}</span><span class="s2"> albums by </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">artist</span><span class="si">}</span><span class="s2">.&quot;</span>
-</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>        <span class="p">)</span>
-</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a>        <span class="n">timer</span> <span class="o">=</span> <span class="n">Timer</span><span class="p">(</span><span class="n">subsecond_resolution</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>        <span class="n">timer</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
-</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>        <span class="n">fails</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>        <span class="k">for</span> <span class="n">album</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">:</span>
-</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>            <span class="k">try</span><span class="p">:</span>
-</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>                <span class="n">album</span><span class="o">.</span><span class="n">rip</span><span class="p">()</span>
-</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>                <span class="n">fails</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="n">album</span><span class="p">,</span> <span class="n">e</span><span class="p">))</span>
-</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>        <span class="n">timer</span><span class="o">.</span><span class="n">stop</span><span class="p">()</span>
-</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a>        <span class="n">artist</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">artist</span>
-</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>        <span class="nb">print</span><span class="p">(</span>
-</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a>            <span class="sa">f</span><span class="s2">&quot;Finished downloading </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">)</span><span class="si">}</span><span class="s2"> albums by </span><span class="si">{</span><span class="n">artist</span><span class="si">}</span><span class="s2"> in </span><span class="si">{</span><span class="n">timer</span><span class="o">.</span><span class="n">elapsed_str</span><span class="si">}</span><span class="s2">.&quot;</span>
-</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>        <span class="p">)</span>
-</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>        <span class="k">if</span> <span class="n">fails</span><span class="p">:</span>
-</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;The following downloads failed:&quot;</span><span class="p">)</span>
-</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a>            <span class="k">for</span> <span class="n">fail</span> <span class="ow">in</span> <span class="n">fails</span><span class="p">:</span>
-</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">fail</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">fail</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>
-</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a>
-</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a><span class="k">def</span> <span class="nf">page_is_discography</span><span class="p">(</span><span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a>    <span class="sd">&quot;&quot;&quot;Returns whether the url is to a discography page or not.&quot;&quot;&quot;</span>
-</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a>    <span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">url</span><span class="p">,</span> <span class="n">headers</span><span class="o">=</span><span class="n">whosyouragent</span><span class="o">.</span><span class="n">get_agent</span><span class="p">(</span><span class="n">as_dict</span><span class="o">=</span><span class="kc">True</span><span class="p">))</span>
-</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a>    <span class="k">if</span> <span class="n">response</span><span class="o">.</span><span class="n">status_code</span> <span class="o">!=</span> <span class="mi">200</span><span class="p">:</span>
-</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a>        <span class="k">raise</span> <span class="ne">RuntimeError</span><span class="p">(</span>
-</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a>            <span class="sa">f</span><span class="s2">&quot;Getting </span><span class="si">{</span><span class="n">url</span><span class="si">}</span><span class="s2"> failed with status code </span><span class="si">{</span><span class="n">response</span><span class="o">.</span><span class="n">status_code</span><span class="si">}</span><span class="s2">.&quot;</span>
-</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a>        <span class="p">)</span>
-</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a>    <span class="n">soup</span> <span class="o">=</span> <span class="n">BeautifulSoup</span><span class="p">(</span><span class="n">response</span><span class="o">.</span><span class="n">text</span><span class="p">,</span> <span class="s2">&quot;html.parser&quot;</span><span class="p">)</span>
-</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a>    <span class="c1"># Returns None if it doesn&#39;t exist.</span>
-</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a>    <span class="n">grid</span> <span class="o">=</span> <span class="n">soup</span><span class="o">.</span><span class="n">find</span><span class="p">(</span><span class="s2">&quot;ol&quot;</span><span class="p">,</span> <span class="n">attrs</span><span class="o">=</span><span class="p">{</span><span class="s2">&quot;id&quot;</span><span class="p">:</span> <span class="s2">&quot;music-grid&quot;</span><span class="p">})</span>
-</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a>    <span class="k">if</span> <span class="n">grid</span><span class="p">:</span>
-</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>        <span class="k">return</span> <span class="kc">True</span>
-</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a>    <span class="k">return</span> <span class="kc">False</span>
-</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a>
-</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a>
-</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
-</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
+</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>        <span class="n">num_tracks</span> <span class="o">=</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span><span class="p">)</span>
+</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>        <span class="n">bar</span> <span class="o">=</span> <span class="n">ProgBar</span><span class="p">(</span><span class="n">num_tracks</span><span class="p">,</span> <span class="n">width_ratio</span><span class="o">=</span><span class="mf">0.5</span><span class="p">)</span>
+</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>        <span class="n">fails</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">overwrite</span><span class="p">:</span>
+</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>                <span class="n">track</span> <span class="k">for</span> <span class="n">track</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span> <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">track_exists</span><span class="p">(</span><span class="n">track</span><span class="p">)</span>
+</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>            <span class="p">]</span>
+</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>        <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">track</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span><span class="p">,</span> <span class="mi">1</span><span class="p">):</span>
+</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>            <span class="n">bar</span><span class="o">.</span><span class="n">display</span><span class="p">(</span>
+</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>                <span class="n">suffix</span><span class="o">=</span><span class="sa">f</span><span class="s2">&quot;Downloading track </span><span class="si">{</span><span class="n">i</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">num_tracks</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">track</span><span class="o">.</span><span class="n">title</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span>
+</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>                <span class="n">counter_override</span><span class="o">=</span><span class="mi">1</span> <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span> <span class="k">else</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>            <span class="p">)</span>
+</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>            <span class="k">try</span><span class="p">:</span>
+</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>                <span class="n">content</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_track_content</span><span class="p">(</span><span class="n">track</span><span class="o">.</span><span class="n">url</span><span class="p">)</span>
+</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">save_track</span><span class="p">(</span>
+</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>                    <span class="n">track</span><span class="o">.</span><span class="n">title</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">no_track_number</span> <span class="k">else</span> <span class="n">track</span><span class="o">.</span><span class="n">numbered_title</span><span class="p">,</span>
+</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>                    <span class="n">content</span><span class="p">,</span>
+</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>                <span class="p">)</span>
+</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>                <span class="n">fails</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="n">track</span><span class="p">,</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">)))</span>
+</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>        <span class="nb">print</span><span class="p">(</span>
+</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>            <span class="sa">f</span><span class="s2">&quot;Finished downloading </span><span class="si">{</span><span class="n">num_tracks</span> <span class="o">-</span> <span class="nb">len</span><span class="p">(</span><span class="n">fails</span><span class="p">)</span><span class="si">}</span><span class="s2"> tracks from </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="si">}</span><span class="s2"> in </span><span class="si">{</span><span class="n">bar</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">elapsed_str</span><span class="si">}</span><span class="s2">.&quot;</span>
+</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>        <span class="p">)</span>
+</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>        <span class="k">if</span> <span class="n">fails</span><span class="p">:</span>
+</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;The following tracks failed to download:&quot;</span><span class="p">)</span>
+</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a>            <span class="k">for</span> <span class="n">fail</span> <span class="ow">in</span> <span class="n">fails</span><span class="p">:</span>
+</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">fail</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">title</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">fail</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>
+</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a>
+</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a><span class="k">class</span> <span class="nc">BandRipper</span><span class="p">:</span>
+</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
+</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">band_url</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">no_track_number</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>    <span class="p">):</span>
+</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">band_url</span> <span class="o">=</span> <span class="n">band_url</span>
+</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">albums</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>        <span class="k">for</span> <span class="n">url</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_album_urls</span><span class="p">(</span><span class="n">band_url</span><span class="p">):</span>
+</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>            <span class="k">try</span><span class="p">:</span>
+</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">AlbumRipper</span><span class="p">(</span><span class="n">url</span><span class="p">,</span> <span class="n">no_track_number</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">))</span>
+</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>                <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
+</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a>
+</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a>    <span class="k">def</span> <span class="nf">get_album_urls</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">band_url</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
+</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a>        <span class="sd">&quot;&quot;&quot;Get album urls from the main bandcamp url.&quot;&quot;&quot;</span>
+</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Fetching discography from </span><span class="si">{</span><span class="n">band_url</span><span class="si">}</span><span class="s2">...&quot;</span><span class="p">)</span>
+</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a>        <span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">band_url</span><span class="p">,</span> <span class="n">headers</span><span class="o">=</span><span class="n">whosyouragent</span><span class="o">.</span><span class="n">get_agent</span><span class="p">(</span><span class="n">as_dict</span><span class="o">=</span><span class="kc">True</span><span class="p">))</span>
+</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>        <span class="k">if</span> <span class="n">response</span><span class="o">.</span><span class="n">status_code</span> <span class="o">!=</span> <span class="mi">200</span><span class="p">:</span>
+</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>            <span class="k">raise</span> <span class="ne">RuntimeError</span><span class="p">(</span>
+</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>                <span class="sa">f</span><span class="s2">&quot;Getting </span><span class="si">{</span><span class="n">band_url</span><span class="si">}</span><span class="s2"> failed with status code </span><span class="si">{</span><span class="n">response</span><span class="o">.</span><span class="n">status_code</span><span class="si">}</span><span class="s2">.&quot;</span>
+</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>            <span class="p">)</span>
+</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a>        <span class="n">soup</span> <span class="o">=</span> <span class="n">BeautifulSoup</span><span class="p">(</span><span class="n">response</span><span class="o">.</span><span class="n">text</span><span class="p">,</span> <span class="s2">&quot;html.parser&quot;</span><span class="p">)</span>
+</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>        <span class="n">grid</span> <span class="o">=</span> <span class="n">soup</span><span class="o">.</span><span class="n">find</span><span class="p">(</span><span class="s2">&quot;ol&quot;</span><span class="p">,</span> <span class="n">attrs</span><span class="o">=</span><span class="p">{</span><span class="s2">&quot;id&quot;</span><span class="p">:</span> <span class="s2">&quot;music-grid&quot;</span><span class="p">})</span>
+</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a>        <span class="n">parsed_url</span> <span class="o">=</span> <span class="n">urlparse</span><span class="p">(</span><span class="n">band_url</span><span class="p">)</span>
+</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>        <span class="n">base_url</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;https://</span><span class="si">{</span><span class="n">parsed_url</span><span class="o">.</span><span class="n">netloc</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">base_url</span> <span class="o">+</span> <span class="n">album</span><span class="o">.</span><span class="n">a</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;href&quot;</span><span class="p">)</span> <span class="k">for</span> <span class="n">album</span> <span class="ow">in</span> <span class="n">grid</span><span class="o">.</span><span class="n">find_all</span><span class="p">(</span><span class="s2">&quot;li&quot;</span><span class="p">)]</span>
+</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>
+</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>    <span class="k">def</span> <span class="nf">rip</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a>        <span class="nb">print</span><span class="p">(</span>
+</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>            <span class="sa">f</span><span class="s2">&quot;Downloading </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">)</span><span class="si">}</span><span class="s2"> albums by </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">artist</span><span class="si">}</span><span class="s2">.&quot;</span>
+</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>        <span class="p">)</span>
+</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>        <span class="n">timer</span> <span class="o">=</span> <span class="n">Timer</span><span class="p">(</span><span class="n">subsecond_resolution</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>        <span class="n">timer</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
+</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>        <span class="n">fails</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>        <span class="k">for</span> <span class="n">album</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">:</span>
+</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>            <span class="k">try</span><span class="p">:</span>
+</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>                <span class="n">album</span><span class="o">.</span><span class="n">rip</span><span class="p">()</span>
+</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>                <span class="n">fails</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="n">album</span><span class="p">,</span> <span class="n">e</span><span class="p">))</span>
+</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a>        <span class="n">timer</span><span class="o">.</span><span class="n">stop</span><span class="p">()</span>
+</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>        <span class="n">artist</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">artist</span>
+</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>        <span class="nb">print</span><span class="p">(</span>
+</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>            <span class="sa">f</span><span class="s2">&quot;Finished downloading </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">)</span><span class="si">}</span><span class="s2"> albums by </span><span class="si">{</span><span class="n">artist</span><span class="si">}</span><span class="s2"> in </span><span class="si">{</span><span class="n">timer</span><span class="o">.</span><span class="n">elapsed_str</span><span class="si">}</span><span class="s2">.&quot;</span>
+</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a>        <span class="p">)</span>
+</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a>        <span class="k">if</span> <span class="n">fails</span><span class="p">:</span>
+</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;The following downloads failed:&quot;</span><span class="p">)</span>
+</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a>            <span class="k">for</span> <span class="n">fail</span> <span class="ow">in</span> <span class="n">fails</span><span class="p">:</span>
+</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">fail</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">fail</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a>
+</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a>
+</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a><span class="k">def</span> <span class="nf">page_is_discography</span><span class="p">(</span><span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a>    <span class="sd">&quot;&quot;&quot;Returns whether the url is to a discography page or not.&quot;&quot;&quot;</span>
+</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a>    <span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">url</span><span class="p">,</span> <span class="n">headers</span><span class="o">=</span><span class="n">whosyouragent</span><span class="o">.</span><span class="n">get_agent</span><span class="p">(</span><span class="n">as_dict</span><span class="o">=</span><span class="kc">True</span><span class="p">))</span>
+</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a>    <span class="k">if</span> <span class="n">response</span><span class="o">.</span><span class="n">status_code</span> <span class="o">!=</span> <span class="mi">200</span><span class="p">:</span>
+</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a>        <span class="k">raise</span> <span class="ne">RuntimeError</span><span class="p">(</span>
+</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a>            <span class="sa">f</span><span class="s2">&quot;Getting </span><span class="si">{</span><span class="n">url</span><span class="si">}</span><span class="s2"> failed with status code </span><span class="si">{</span><span class="n">response</span><span class="o">.</span><span class="n">status_code</span><span class="si">}</span><span class="s2">.&quot;</span>
+</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a>        <span class="p">)</span>
+</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a>    <span class="n">soup</span> <span class="o">=</span> <span class="n">BeautifulSoup</span><span class="p">(</span><span class="n">response</span><span class="o">.</span><span class="n">text</span><span class="p">,</span> <span class="s2">&quot;html.parser&quot;</span><span class="p">)</span>
+</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>    <span class="c1"># Returns None if it doesn&#39;t exist.</span>
+</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a>    <span class="n">grid</span> <span class="o">=</span> <span class="n">soup</span><span class="o">.</span><span class="n">find</span><span class="p">(</span><span class="s2">&quot;ol&quot;</span><span class="p">,</span> <span class="n">attrs</span><span class="o">=</span><span class="p">{</span><span class="s2">&quot;id&quot;</span><span class="p">:</span> <span class="s2">&quot;music-grid&quot;</span><span class="p">})</span>
+</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a>    <span class="k">if</span> <span class="n">grid</span><span class="p">:</span>
+</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a>        <span class="k">return</span> <span class="kc">True</span>
+</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a>    <span class="k">return</span> <span class="kc">False</span>
+</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a>
 </span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a>
-</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a>        <span class="s2">&quot;urls&quot;</span><span class="p">,</span>
-</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
-</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The bandcamp url(s) for the album or artist.</span>
-</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a><span class="s2">            If the url is to an artists main page,</span>
-</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a><span class="s2">            all albums will be downloaded.</span>
-</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a><span class="s2">            The tracks will be saved to a subdirectory of</span>
-</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a><span class="s2">            your current directory.</span>
-</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a><span class="s2">            If a track can&#39;t be streamed (i.e. private) it</span>
-</span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a><span class="s2">            won&#39;t be downloaded. Multiple urls can be passed.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a>    <span class="p">)</span>
-</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a>
-</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a>        <span class="s2">&quot;-n&quot;</span><span class="p">,</span>
-</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a>        <span class="s2">&quot;--no_track_number&quot;</span><span class="p">,</span>
-</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; By default the track number will be added</span>
-</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a><span class="s2">        to the front of the track title. Pass this switch</span>
-</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a><span class="s2">        to disable the behavior.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a>    <span class="p">)</span>
-</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a>
-</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a>        <span class="s2">&quot;-o&quot;</span><span class="p">,</span>
-</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a>        <span class="s2">&quot;--overwrite&quot;</span><span class="p">,</span>
-</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Pass this flag to overwrite existing files.</span>
-</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a><span class="s2">        Otherwise don&#39;t download tracks that already exist locally.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a>    <span class="p">)</span>
-</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a>
-</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
-</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a>    <span class="n">args</span><span class="o">.</span><span class="n">urls</span> <span class="o">=</span> <span class="p">[</span><span class="n">url</span><span class="o">.</span><span class="n">strip</span><span class="p">(</span><span class="s2">&quot;/&quot;</span><span class="p">)</span> <span class="k">for</span> <span class="n">url</span> <span class="ow">in</span> <span class="n">args</span><span class="o">.</span><span class="n">urls</span><span class="p">]</span>
+</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
+</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
+</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a>
+</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a>        <span class="s2">&quot;urls&quot;</span><span class="p">,</span>
+</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
+</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The bandcamp url(s) for the album or artist.</span>
+</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a><span class="s2">            If the url is to an artists main page,</span>
+</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a><span class="s2">            all albums will be downloaded.</span>
+</span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a><span class="s2">            The tracks will be saved to a subdirectory of</span>
+</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a><span class="s2">            your current directory.</span>
+</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a><span class="s2">            If a track can&#39;t be streamed (i.e. private) it</span>
+</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a><span class="s2">            won&#39;t be downloaded. Multiple urls can be passed.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a>    <span class="p">)</span>
+</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a>
+</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a>        <span class="s2">&quot;-n&quot;</span><span class="p">,</span>
+</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a>        <span class="s2">&quot;--no_track_number&quot;</span><span class="p">,</span>
+</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; By default the track number will be added</span>
+</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a><span class="s2">        to the front of the track title. Pass this switch</span>
+</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a><span class="s2">        to disable the behavior.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a>    <span class="p">)</span>
+</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a>
+</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>        <span class="s2">&quot;-o&quot;</span><span class="p">,</span>
+</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a>        <span class="s2">&quot;--overwrite&quot;</span><span class="p">,</span>
+</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Pass this flag to overwrite existing files.</span>
+</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a><span class="s2">        Otherwise don&#39;t download tracks that already exist locally.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a>    <span class="p">)</span>
 </span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a>
-</span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a>    <span class="k">return</span> <span class="n">args</span>
-</span><span id="L-263"><a href="#L-263"><span class="linenos">263</span></a>
+</span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
+</span><span id="L-263"><a href="#L-263"><span class="linenos">263</span></a>    <span class="n">args</span><span class="o">.</span><span class="n">urls</span> <span class="o">=</span> <span class="p">[</span><span class="n">url</span><span class="o">.</span><span class="n">strip</span><span class="p">(</span><span class="s2">&quot;/&quot;</span><span class="p">)</span> <span class="k">for</span> <span class="n">url</span> <span class="ow">in</span> <span class="n">args</span><span class="o">.</span><span class="n">urls</span><span class="p">]</span>
 </span><span id="L-264"><a href="#L-264"><span class="linenos">264</span></a>
-</span><span id="L-265"><a href="#L-265"><span class="linenos">265</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="L-266"><a href="#L-266"><span class="linenos">266</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
-</span><span id="L-267"><a href="#L-267"><span class="linenos">267</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
-</span><span id="L-268"><a href="#L-268"><span class="linenos">268</span></a>    <span class="k">for</span> <span class="n">url</span> <span class="ow">in</span> <span class="n">args</span><span class="o">.</span><span class="n">urls</span><span class="p">:</span>
-</span><span id="L-269"><a href="#L-269"><span class="linenos">269</span></a>        <span class="k">if</span> <span class="n">page_is_discography</span><span class="p">(</span><span class="n">url</span><span class="p">):</span>
-</span><span id="L-270"><a href="#L-270"><span class="linenos">270</span></a>            <span class="n">ripper</span> <span class="o">=</span> <span class="n">BandRipper</span><span class="p">(</span><span class="n">url</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">no_track_number</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">overwrite</span><span class="p">)</span>
-</span><span id="L-271"><a href="#L-271"><span class="linenos">271</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="L-272"><a href="#L-272"><span class="linenos">272</span></a>            <span class="n">ripper</span> <span class="o">=</span> <span class="n">AlbumRipper</span><span class="p">(</span><span class="n">url</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">no_track_number</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">overwrite</span><span class="p">)</span>
-</span><span id="L-273"><a href="#L-273"><span class="linenos">273</span></a>        <span class="n">ripper</span><span class="o">.</span><span class="n">rip</span><span class="p">()</span>
-</span><span id="L-274"><a href="#L-274"><span class="linenos">274</span></a>
-</span><span id="L-275"><a href="#L-275"><span class="linenos">275</span></a>
-</span><span id="L-276"><a href="#L-276"><span class="linenos">276</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
-</span><span id="L-277"><a href="#L-277"><span class="linenos">277</span></a>    <span class="n">main</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
+</span><span id="L-265"><a href="#L-265"><span class="linenos">265</span></a>    <span class="k">return</span> <span class="n">args</span>
+</span><span id="L-266"><a href="#L-266"><span class="linenos">266</span></a>
+</span><span id="L-267"><a href="#L-267"><span class="linenos">267</span></a>
+</span><span id="L-268"><a href="#L-268"><span class="linenos">268</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="L-269"><a href="#L-269"><span class="linenos">269</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
+</span><span id="L-270"><a href="#L-270"><span class="linenos">270</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="L-271"><a href="#L-271"><span class="linenos">271</span></a>    <span class="k">for</span> <span class="n">url</span> <span class="ow">in</span> <span class="n">args</span><span class="o">.</span><span class="n">urls</span><span class="p">:</span>
+</span><span id="L-272"><a href="#L-272"><span class="linenos">272</span></a>        <span class="k">if</span> <span class="n">page_is_discography</span><span class="p">(</span><span class="n">url</span><span class="p">):</span>
+</span><span id="L-273"><a href="#L-273"><span class="linenos">273</span></a>            <span class="n">ripper</span> <span class="o">=</span> <span class="n">BandRipper</span><span class="p">(</span><span class="n">url</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">no_track_number</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">overwrite</span><span class="p">)</span>
+</span><span id="L-274"><a href="#L-274"><span class="linenos">274</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-275"><a href="#L-275"><span class="linenos">275</span></a>            <span class="n">ripper</span> <span class="o">=</span> <span class="n">AlbumRipper</span><span class="p">(</span><span class="n">url</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">no_track_number</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">overwrite</span><span class="p">)</span>
+</span><span id="L-276"><a href="#L-276"><span class="linenos">276</span></a>        <span class="n">ripper</span><span class="o">.</span><span class="n">rip</span><span class="p">()</span>
+</span><span id="L-277"><a href="#L-277"><span class="linenos">277</span></a>
+</span><span id="L-278"><a href="#L-278"><span class="linenos">278</span></a>
+</span><span id="L-279"><a href="#L-279"><span class="linenos">279</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
+</span><span id="L-280"><a href="#L-280"><span class="linenos">280</span></a>    <span class="n">main</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
 </span></pre></div>
 
 
             </section>
                 <section id="clean_string">
                             <input id="clean_string-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -605,38 +608,41 @@
 </span><span id="AlbumRipper-130"><a href="#AlbumRipper-130"><span class="linenos">130</span></a>    <span class="k">def</span> <span class="nf">rip</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
 </span><span id="AlbumRipper-131"><a href="#AlbumRipper-131"><span class="linenos">131</span></a>        <span class="sd">&quot;&quot;&quot;Download and save the album tracks and album art.&quot;&quot;&quot;</span>
 </span><span id="AlbumRipper-132"><a href="#AlbumRipper-132"><span class="linenos">132</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
 </span><span id="AlbumRipper-133"><a href="#AlbumRipper-133"><span class="linenos">133</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;No public tracks available for </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
 </span><span id="AlbumRipper-134"><a href="#AlbumRipper-134"><span class="linenos">134</span></a>            <span class="k">return</span> <span class="kc">None</span>
 </span><span id="AlbumRipper-135"><a href="#AlbumRipper-135"><span class="linenos">135</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">make_save_path</span><span class="p">()</span>
 </span><span id="AlbumRipper-136"><a href="#AlbumRipper-136"><span class="linenos">136</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">download_album_art</span><span class="p">()</span>
-</span><span id="AlbumRipper-137"><a href="#AlbumRipper-137"><span class="linenos">137</span></a>        <span class="n">bar</span> <span class="o">=</span> <span class="n">ProgBar</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span><span class="p">)</span> <span class="o">-</span> <span class="mi">1</span><span class="p">,</span> <span class="n">width_ratio</span><span class="o">=</span><span class="mf">0.5</span><span class="p">)</span>
-</span><span id="AlbumRipper-138"><a href="#AlbumRipper-138"><span class="linenos">138</span></a>        <span class="n">fails</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="AlbumRipper-139"><a href="#AlbumRipper-139"><span class="linenos">139</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">overwrite</span><span class="p">:</span>
-</span><span id="AlbumRipper-140"><a href="#AlbumRipper-140"><span class="linenos">140</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="AlbumRipper-141"><a href="#AlbumRipper-141"><span class="linenos">141</span></a>                <span class="n">track</span> <span class="k">for</span> <span class="n">track</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span> <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">track_exists</span><span class="p">(</span><span class="n">track</span><span class="p">)</span>
-</span><span id="AlbumRipper-142"><a href="#AlbumRipper-142"><span class="linenos">142</span></a>            <span class="p">]</span>
-</span><span id="AlbumRipper-143"><a href="#AlbumRipper-143"><span class="linenos">143</span></a>        <span class="k">for</span> <span class="n">track</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span><span class="p">:</span>
-</span><span id="AlbumRipper-144"><a href="#AlbumRipper-144"><span class="linenos">144</span></a>            <span class="n">bar</span><span class="o">.</span><span class="n">display</span><span class="p">(</span>
-</span><span id="AlbumRipper-145"><a href="#AlbumRipper-145"><span class="linenos">145</span></a>                <span class="n">suffix</span><span class="o">=</span><span class="sa">f</span><span class="s2">&quot;Downloading </span><span class="si">{</span><span class="n">track</span><span class="o">.</span><span class="n">title</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span>
-</span><span id="AlbumRipper-146"><a href="#AlbumRipper-146"><span class="linenos">146</span></a>                <span class="n">counter_override</span><span class="o">=</span><span class="mi">1</span> <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span> <span class="k">else</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="AlbumRipper-147"><a href="#AlbumRipper-147"><span class="linenos">147</span></a>            <span class="p">)</span>
-</span><span id="AlbumRipper-148"><a href="#AlbumRipper-148"><span class="linenos">148</span></a>            <span class="k">try</span><span class="p">:</span>
-</span><span id="AlbumRipper-149"><a href="#AlbumRipper-149"><span class="linenos">149</span></a>                <span class="n">content</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_track_content</span><span class="p">(</span><span class="n">track</span><span class="o">.</span><span class="n">url</span><span class="p">)</span>
-</span><span id="AlbumRipper-150"><a href="#AlbumRipper-150"><span class="linenos">150</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">save_track</span><span class="p">(</span>
-</span><span id="AlbumRipper-151"><a href="#AlbumRipper-151"><span class="linenos">151</span></a>                    <span class="n">track</span><span class="o">.</span><span class="n">title</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">no_track_number</span> <span class="k">else</span> <span class="n">track</span><span class="o">.</span><span class="n">numbered_title</span><span class="p">,</span>
-</span><span id="AlbumRipper-152"><a href="#AlbumRipper-152"><span class="linenos">152</span></a>                    <span class="n">content</span><span class="p">,</span>
-</span><span id="AlbumRipper-153"><a href="#AlbumRipper-153"><span class="linenos">153</span></a>                <span class="p">)</span>
-</span><span id="AlbumRipper-154"><a href="#AlbumRipper-154"><span class="linenos">154</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="AlbumRipper-155"><a href="#AlbumRipper-155"><span class="linenos">155</span></a>                <span class="n">fails</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="n">track</span><span class="p">,</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">)))</span>
-</span><span id="AlbumRipper-156"><a href="#AlbumRipper-156"><span class="linenos">156</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Finished downloading </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="si">}</span><span class="s2"> in </span><span class="si">{</span><span class="n">bar</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">elapsed_str</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="AlbumRipper-157"><a href="#AlbumRipper-157"><span class="linenos">157</span></a>        <span class="k">if</span> <span class="n">fails</span><span class="p">:</span>
-</span><span id="AlbumRipper-158"><a href="#AlbumRipper-158"><span class="linenos">158</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;The following tracks failed to download:&quot;</span><span class="p">)</span>
-</span><span id="AlbumRipper-159"><a href="#AlbumRipper-159"><span class="linenos">159</span></a>            <span class="k">for</span> <span class="n">fail</span> <span class="ow">in</span> <span class="n">fails</span><span class="p">:</span>
-</span><span id="AlbumRipper-160"><a href="#AlbumRipper-160"><span class="linenos">160</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">fail</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">title</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">fail</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="AlbumRipper-137"><a href="#AlbumRipper-137"><span class="linenos">137</span></a>        <span class="n">num_tracks</span> <span class="o">=</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span><span class="p">)</span>
+</span><span id="AlbumRipper-138"><a href="#AlbumRipper-138"><span class="linenos">138</span></a>        <span class="n">bar</span> <span class="o">=</span> <span class="n">ProgBar</span><span class="p">(</span><span class="n">num_tracks</span><span class="p">,</span> <span class="n">width_ratio</span><span class="o">=</span><span class="mf">0.5</span><span class="p">)</span>
+</span><span id="AlbumRipper-139"><a href="#AlbumRipper-139"><span class="linenos">139</span></a>        <span class="n">fails</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="AlbumRipper-140"><a href="#AlbumRipper-140"><span class="linenos">140</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">overwrite</span><span class="p">:</span>
+</span><span id="AlbumRipper-141"><a href="#AlbumRipper-141"><span class="linenos">141</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="AlbumRipper-142"><a href="#AlbumRipper-142"><span class="linenos">142</span></a>                <span class="n">track</span> <span class="k">for</span> <span class="n">track</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span> <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">track_exists</span><span class="p">(</span><span class="n">track</span><span class="p">)</span>
+</span><span id="AlbumRipper-143"><a href="#AlbumRipper-143"><span class="linenos">143</span></a>            <span class="p">]</span>
+</span><span id="AlbumRipper-144"><a href="#AlbumRipper-144"><span class="linenos">144</span></a>        <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">track</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span><span class="p">,</span> <span class="mi">1</span><span class="p">):</span>
+</span><span id="AlbumRipper-145"><a href="#AlbumRipper-145"><span class="linenos">145</span></a>            <span class="n">bar</span><span class="o">.</span><span class="n">display</span><span class="p">(</span>
+</span><span id="AlbumRipper-146"><a href="#AlbumRipper-146"><span class="linenos">146</span></a>                <span class="n">suffix</span><span class="o">=</span><span class="sa">f</span><span class="s2">&quot;Downloading track </span><span class="si">{</span><span class="n">i</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">num_tracks</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">track</span><span class="o">.</span><span class="n">title</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span>
+</span><span id="AlbumRipper-147"><a href="#AlbumRipper-147"><span class="linenos">147</span></a>                <span class="n">counter_override</span><span class="o">=</span><span class="mi">1</span> <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span> <span class="k">else</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="AlbumRipper-148"><a href="#AlbumRipper-148"><span class="linenos">148</span></a>            <span class="p">)</span>
+</span><span id="AlbumRipper-149"><a href="#AlbumRipper-149"><span class="linenos">149</span></a>            <span class="k">try</span><span class="p">:</span>
+</span><span id="AlbumRipper-150"><a href="#AlbumRipper-150"><span class="linenos">150</span></a>                <span class="n">content</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_track_content</span><span class="p">(</span><span class="n">track</span><span class="o">.</span><span class="n">url</span><span class="p">)</span>
+</span><span id="AlbumRipper-151"><a href="#AlbumRipper-151"><span class="linenos">151</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">save_track</span><span class="p">(</span>
+</span><span id="AlbumRipper-152"><a href="#AlbumRipper-152"><span class="linenos">152</span></a>                    <span class="n">track</span><span class="o">.</span><span class="n">title</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">no_track_number</span> <span class="k">else</span> <span class="n">track</span><span class="o">.</span><span class="n">numbered_title</span><span class="p">,</span>
+</span><span id="AlbumRipper-153"><a href="#AlbumRipper-153"><span class="linenos">153</span></a>                    <span class="n">content</span><span class="p">,</span>
+</span><span id="AlbumRipper-154"><a href="#AlbumRipper-154"><span class="linenos">154</span></a>                <span class="p">)</span>
+</span><span id="AlbumRipper-155"><a href="#AlbumRipper-155"><span class="linenos">155</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="AlbumRipper-156"><a href="#AlbumRipper-156"><span class="linenos">156</span></a>                <span class="n">fails</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="n">track</span><span class="p">,</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">)))</span>
+</span><span id="AlbumRipper-157"><a href="#AlbumRipper-157"><span class="linenos">157</span></a>        <span class="nb">print</span><span class="p">(</span>
+</span><span id="AlbumRipper-158"><a href="#AlbumRipper-158"><span class="linenos">158</span></a>            <span class="sa">f</span><span class="s2">&quot;Finished downloading </span><span class="si">{</span><span class="n">num_tracks</span> <span class="o">-</span> <span class="nb">len</span><span class="p">(</span><span class="n">fails</span><span class="p">)</span><span class="si">}</span><span class="s2"> tracks from </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="si">}</span><span class="s2"> in </span><span class="si">{</span><span class="n">bar</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">elapsed_str</span><span class="si">}</span><span class="s2">.&quot;</span>
+</span><span id="AlbumRipper-159"><a href="#AlbumRipper-159"><span class="linenos">159</span></a>        <span class="p">)</span>
+</span><span id="AlbumRipper-160"><a href="#AlbumRipper-160"><span class="linenos">160</span></a>        <span class="k">if</span> <span class="n">fails</span><span class="p">:</span>
+</span><span id="AlbumRipper-161"><a href="#AlbumRipper-161"><span class="linenos">161</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;The following tracks failed to download:&quot;</span><span class="p">)</span>
+</span><span id="AlbumRipper-162"><a href="#AlbumRipper-162"><span class="linenos">162</span></a>            <span class="k">for</span> <span class="n">fail</span> <span class="ow">in</span> <span class="n">fails</span><span class="p">:</span>
+</span><span id="AlbumRipper-163"><a href="#AlbumRipper-163"><span class="linenos">163</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">fail</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">title</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">fail</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             <div id="AlbumRipper.__init__" class="classattr">
                                         <input id="AlbumRipper.__init__-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
@@ -833,38 +839,41 @@
             <div class="pdoc-code codehilite"><pre><span></span><span id="AlbumRipper.rip-130"><a href="#AlbumRipper.rip-130"><span class="linenos">130</span></a>    <span class="k">def</span> <span class="nf">rip</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
 </span><span id="AlbumRipper.rip-131"><a href="#AlbumRipper.rip-131"><span class="linenos">131</span></a>        <span class="sd">&quot;&quot;&quot;Download and save the album tracks and album art.&quot;&quot;&quot;</span>
 </span><span id="AlbumRipper.rip-132"><a href="#AlbumRipper.rip-132"><span class="linenos">132</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
 </span><span id="AlbumRipper.rip-133"><a href="#AlbumRipper.rip-133"><span class="linenos">133</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;No public tracks available for </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
 </span><span id="AlbumRipper.rip-134"><a href="#AlbumRipper.rip-134"><span class="linenos">134</span></a>            <span class="k">return</span> <span class="kc">None</span>
 </span><span id="AlbumRipper.rip-135"><a href="#AlbumRipper.rip-135"><span class="linenos">135</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">make_save_path</span><span class="p">()</span>
 </span><span id="AlbumRipper.rip-136"><a href="#AlbumRipper.rip-136"><span class="linenos">136</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">download_album_art</span><span class="p">()</span>
-</span><span id="AlbumRipper.rip-137"><a href="#AlbumRipper.rip-137"><span class="linenos">137</span></a>        <span class="n">bar</span> <span class="o">=</span> <span class="n">ProgBar</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span><span class="p">)</span> <span class="o">-</span> <span class="mi">1</span><span class="p">,</span> <span class="n">width_ratio</span><span class="o">=</span><span class="mf">0.5</span><span class="p">)</span>
-</span><span id="AlbumRipper.rip-138"><a href="#AlbumRipper.rip-138"><span class="linenos">138</span></a>        <span class="n">fails</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="AlbumRipper.rip-139"><a href="#AlbumRipper.rip-139"><span class="linenos">139</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">overwrite</span><span class="p">:</span>
-</span><span id="AlbumRipper.rip-140"><a href="#AlbumRipper.rip-140"><span class="linenos">140</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="AlbumRipper.rip-141"><a href="#AlbumRipper.rip-141"><span class="linenos">141</span></a>                <span class="n">track</span> <span class="k">for</span> <span class="n">track</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span> <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">track_exists</span><span class="p">(</span><span class="n">track</span><span class="p">)</span>
-</span><span id="AlbumRipper.rip-142"><a href="#AlbumRipper.rip-142"><span class="linenos">142</span></a>            <span class="p">]</span>
-</span><span id="AlbumRipper.rip-143"><a href="#AlbumRipper.rip-143"><span class="linenos">143</span></a>        <span class="k">for</span> <span class="n">track</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span><span class="p">:</span>
-</span><span id="AlbumRipper.rip-144"><a href="#AlbumRipper.rip-144"><span class="linenos">144</span></a>            <span class="n">bar</span><span class="o">.</span><span class="n">display</span><span class="p">(</span>
-</span><span id="AlbumRipper.rip-145"><a href="#AlbumRipper.rip-145"><span class="linenos">145</span></a>                <span class="n">suffix</span><span class="o">=</span><span class="sa">f</span><span class="s2">&quot;Downloading </span><span class="si">{</span><span class="n">track</span><span class="o">.</span><span class="n">title</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span>
-</span><span id="AlbumRipper.rip-146"><a href="#AlbumRipper.rip-146"><span class="linenos">146</span></a>                <span class="n">counter_override</span><span class="o">=</span><span class="mi">1</span> <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span> <span class="k">else</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="AlbumRipper.rip-147"><a href="#AlbumRipper.rip-147"><span class="linenos">147</span></a>            <span class="p">)</span>
-</span><span id="AlbumRipper.rip-148"><a href="#AlbumRipper.rip-148"><span class="linenos">148</span></a>            <span class="k">try</span><span class="p">:</span>
-</span><span id="AlbumRipper.rip-149"><a href="#AlbumRipper.rip-149"><span class="linenos">149</span></a>                <span class="n">content</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_track_content</span><span class="p">(</span><span class="n">track</span><span class="o">.</span><span class="n">url</span><span class="p">)</span>
-</span><span id="AlbumRipper.rip-150"><a href="#AlbumRipper.rip-150"><span class="linenos">150</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">save_track</span><span class="p">(</span>
-</span><span id="AlbumRipper.rip-151"><a href="#AlbumRipper.rip-151"><span class="linenos">151</span></a>                    <span class="n">track</span><span class="o">.</span><span class="n">title</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">no_track_number</span> <span class="k">else</span> <span class="n">track</span><span class="o">.</span><span class="n">numbered_title</span><span class="p">,</span>
-</span><span id="AlbumRipper.rip-152"><a href="#AlbumRipper.rip-152"><span class="linenos">152</span></a>                    <span class="n">content</span><span class="p">,</span>
-</span><span id="AlbumRipper.rip-153"><a href="#AlbumRipper.rip-153"><span class="linenos">153</span></a>                <span class="p">)</span>
-</span><span id="AlbumRipper.rip-154"><a href="#AlbumRipper.rip-154"><span class="linenos">154</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="AlbumRipper.rip-155"><a href="#AlbumRipper.rip-155"><span class="linenos">155</span></a>                <span class="n">fails</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="n">track</span><span class="p">,</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">)))</span>
-</span><span id="AlbumRipper.rip-156"><a href="#AlbumRipper.rip-156"><span class="linenos">156</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Finished downloading </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="si">}</span><span class="s2"> in </span><span class="si">{</span><span class="n">bar</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">elapsed_str</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="AlbumRipper.rip-157"><a href="#AlbumRipper.rip-157"><span class="linenos">157</span></a>        <span class="k">if</span> <span class="n">fails</span><span class="p">:</span>
-</span><span id="AlbumRipper.rip-158"><a href="#AlbumRipper.rip-158"><span class="linenos">158</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;The following tracks failed to download:&quot;</span><span class="p">)</span>
-</span><span id="AlbumRipper.rip-159"><a href="#AlbumRipper.rip-159"><span class="linenos">159</span></a>            <span class="k">for</span> <span class="n">fail</span> <span class="ow">in</span> <span class="n">fails</span><span class="p">:</span>
-</span><span id="AlbumRipper.rip-160"><a href="#AlbumRipper.rip-160"><span class="linenos">160</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">fail</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">title</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">fail</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="AlbumRipper.rip-137"><a href="#AlbumRipper.rip-137"><span class="linenos">137</span></a>        <span class="n">num_tracks</span> <span class="o">=</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span><span class="p">)</span>
+</span><span id="AlbumRipper.rip-138"><a href="#AlbumRipper.rip-138"><span class="linenos">138</span></a>        <span class="n">bar</span> <span class="o">=</span> <span class="n">ProgBar</span><span class="p">(</span><span class="n">num_tracks</span><span class="p">,</span> <span class="n">width_ratio</span><span class="o">=</span><span class="mf">0.5</span><span class="p">)</span>
+</span><span id="AlbumRipper.rip-139"><a href="#AlbumRipper.rip-139"><span class="linenos">139</span></a>        <span class="n">fails</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="AlbumRipper.rip-140"><a href="#AlbumRipper.rip-140"><span class="linenos">140</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">overwrite</span><span class="p">:</span>
+</span><span id="AlbumRipper.rip-141"><a href="#AlbumRipper.rip-141"><span class="linenos">141</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="AlbumRipper.rip-142"><a href="#AlbumRipper.rip-142"><span class="linenos">142</span></a>                <span class="n">track</span> <span class="k">for</span> <span class="n">track</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span> <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">track_exists</span><span class="p">(</span><span class="n">track</span><span class="p">)</span>
+</span><span id="AlbumRipper.rip-143"><a href="#AlbumRipper.rip-143"><span class="linenos">143</span></a>            <span class="p">]</span>
+</span><span id="AlbumRipper.rip-144"><a href="#AlbumRipper.rip-144"><span class="linenos">144</span></a>        <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">track</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span><span class="p">,</span> <span class="mi">1</span><span class="p">):</span>
+</span><span id="AlbumRipper.rip-145"><a href="#AlbumRipper.rip-145"><span class="linenos">145</span></a>            <span class="n">bar</span><span class="o">.</span><span class="n">display</span><span class="p">(</span>
+</span><span id="AlbumRipper.rip-146"><a href="#AlbumRipper.rip-146"><span class="linenos">146</span></a>                <span class="n">suffix</span><span class="o">=</span><span class="sa">f</span><span class="s2">&quot;Downloading track </span><span class="si">{</span><span class="n">i</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">num_tracks</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">track</span><span class="o">.</span><span class="n">title</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span>
+</span><span id="AlbumRipper.rip-147"><a href="#AlbumRipper.rip-147"><span class="linenos">147</span></a>                <span class="n">counter_override</span><span class="o">=</span><span class="mi">1</span> <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span> <span class="k">else</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="AlbumRipper.rip-148"><a href="#AlbumRipper.rip-148"><span class="linenos">148</span></a>            <span class="p">)</span>
+</span><span id="AlbumRipper.rip-149"><a href="#AlbumRipper.rip-149"><span class="linenos">149</span></a>            <span class="k">try</span><span class="p">:</span>
+</span><span id="AlbumRipper.rip-150"><a href="#AlbumRipper.rip-150"><span class="linenos">150</span></a>                <span class="n">content</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_track_content</span><span class="p">(</span><span class="n">track</span><span class="o">.</span><span class="n">url</span><span class="p">)</span>
+</span><span id="AlbumRipper.rip-151"><a href="#AlbumRipper.rip-151"><span class="linenos">151</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">save_track</span><span class="p">(</span>
+</span><span id="AlbumRipper.rip-152"><a href="#AlbumRipper.rip-152"><span class="linenos">152</span></a>                    <span class="n">track</span><span class="o">.</span><span class="n">title</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">no_track_number</span> <span class="k">else</span> <span class="n">track</span><span class="o">.</span><span class="n">numbered_title</span><span class="p">,</span>
+</span><span id="AlbumRipper.rip-153"><a href="#AlbumRipper.rip-153"><span class="linenos">153</span></a>                    <span class="n">content</span><span class="p">,</span>
+</span><span id="AlbumRipper.rip-154"><a href="#AlbumRipper.rip-154"><span class="linenos">154</span></a>                <span class="p">)</span>
+</span><span id="AlbumRipper.rip-155"><a href="#AlbumRipper.rip-155"><span class="linenos">155</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="AlbumRipper.rip-156"><a href="#AlbumRipper.rip-156"><span class="linenos">156</span></a>                <span class="n">fails</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="n">track</span><span class="p">,</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">)))</span>
+</span><span id="AlbumRipper.rip-157"><a href="#AlbumRipper.rip-157"><span class="linenos">157</span></a>        <span class="nb">print</span><span class="p">(</span>
+</span><span id="AlbumRipper.rip-158"><a href="#AlbumRipper.rip-158"><span class="linenos">158</span></a>            <span class="sa">f</span><span class="s2">&quot;Finished downloading </span><span class="si">{</span><span class="n">num_tracks</span> <span class="o">-</span> <span class="nb">len</span><span class="p">(</span><span class="n">fails</span><span class="p">)</span><span class="si">}</span><span class="s2"> tracks from </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="si">}</span><span class="s2"> in </span><span class="si">{</span><span class="n">bar</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">elapsed_str</span><span class="si">}</span><span class="s2">.&quot;</span>
+</span><span id="AlbumRipper.rip-159"><a href="#AlbumRipper.rip-159"><span class="linenos">159</span></a>        <span class="p">)</span>
+</span><span id="AlbumRipper.rip-160"><a href="#AlbumRipper.rip-160"><span class="linenos">160</span></a>        <span class="k">if</span> <span class="n">fails</span><span class="p">:</span>
+</span><span id="AlbumRipper.rip-161"><a href="#AlbumRipper.rip-161"><span class="linenos">161</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;The following tracks failed to download:&quot;</span><span class="p">)</span>
+</span><span id="AlbumRipper.rip-162"><a href="#AlbumRipper.rip-162"><span class="linenos">162</span></a>            <span class="k">for</span> <span class="n">fail</span> <span class="ow">in</span> <span class="n">fails</span><span class="p">:</span>
+</span><span id="AlbumRipper.rip-163"><a href="#AlbumRipper.rip-163"><span class="linenos">163</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">fail</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">title</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">fail</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Download and save the album tracks and album art.</p>
 </div>
 
 
@@ -877,61 +886,61 @@
     <span class="def">class</span>
     <span class="name">BandRipper</span>:
 
                 <label class="view-source-button" for="BandRipper-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#BandRipper"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="BandRipper-163"><a href="#BandRipper-163"><span class="linenos">163</span></a><span class="k">class</span> <span class="nc">BandRipper</span><span class="p">:</span>
-</span><span id="BandRipper-164"><a href="#BandRipper-164"><span class="linenos">164</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
-</span><span id="BandRipper-165"><a href="#BandRipper-165"><span class="linenos">165</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">band_url</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">no_track_number</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="BandRipper-166"><a href="#BandRipper-166"><span class="linenos">166</span></a>    <span class="p">):</span>
-</span><span id="BandRipper-167"><a href="#BandRipper-167"><span class="linenos">167</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">band_url</span> <span class="o">=</span> <span class="n">band_url</span>
-</span><span id="BandRipper-168"><a href="#BandRipper-168"><span class="linenos">168</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">albums</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="BandRipper-169"><a href="#BandRipper-169"><span class="linenos">169</span></a>        <span class="k">for</span> <span class="n">url</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_album_urls</span><span class="p">(</span><span class="n">band_url</span><span class="p">):</span>
-</span><span id="BandRipper-170"><a href="#BandRipper-170"><span class="linenos">170</span></a>            <span class="k">try</span><span class="p">:</span>
-</span><span id="BandRipper-171"><a href="#BandRipper-171"><span class="linenos">171</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">AlbumRipper</span><span class="p">(</span><span class="n">url</span><span class="p">,</span> <span class="n">no_track_number</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">))</span>
-</span><span id="BandRipper-172"><a href="#BandRipper-172"><span class="linenos">172</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="BandRipper-173"><a href="#BandRipper-173"><span class="linenos">173</span></a>                <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
-</span><span id="BandRipper-174"><a href="#BandRipper-174"><span class="linenos">174</span></a>
-</span><span id="BandRipper-175"><a href="#BandRipper-175"><span class="linenos">175</span></a>    <span class="k">def</span> <span class="nf">get_album_urls</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">band_url</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
-</span><span id="BandRipper-176"><a href="#BandRipper-176"><span class="linenos">176</span></a>        <span class="sd">&quot;&quot;&quot;Get album urls from the main bandcamp url.&quot;&quot;&quot;</span>
-</span><span id="BandRipper-177"><a href="#BandRipper-177"><span class="linenos">177</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Fetching discography from </span><span class="si">{</span><span class="n">band_url</span><span class="si">}</span><span class="s2">...&quot;</span><span class="p">)</span>
-</span><span id="BandRipper-178"><a href="#BandRipper-178"><span class="linenos">178</span></a>        <span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">band_url</span><span class="p">,</span> <span class="n">headers</span><span class="o">=</span><span class="n">whosyouragent</span><span class="o">.</span><span class="n">get_agent</span><span class="p">(</span><span class="n">as_dict</span><span class="o">=</span><span class="kc">True</span><span class="p">))</span>
-</span><span id="BandRipper-179"><a href="#BandRipper-179"><span class="linenos">179</span></a>        <span class="k">if</span> <span class="n">response</span><span class="o">.</span><span class="n">status_code</span> <span class="o">!=</span> <span class="mi">200</span><span class="p">:</span>
-</span><span id="BandRipper-180"><a href="#BandRipper-180"><span class="linenos">180</span></a>            <span class="k">raise</span> <span class="ne">RuntimeError</span><span class="p">(</span>
-</span><span id="BandRipper-181"><a href="#BandRipper-181"><span class="linenos">181</span></a>                <span class="sa">f</span><span class="s2">&quot;Getting </span><span class="si">{</span><span class="n">band_url</span><span class="si">}</span><span class="s2"> failed with status code </span><span class="si">{</span><span class="n">response</span><span class="o">.</span><span class="n">status_code</span><span class="si">}</span><span class="s2">.&quot;</span>
-</span><span id="BandRipper-182"><a href="#BandRipper-182"><span class="linenos">182</span></a>            <span class="p">)</span>
-</span><span id="BandRipper-183"><a href="#BandRipper-183"><span class="linenos">183</span></a>        <span class="n">soup</span> <span class="o">=</span> <span class="n">BeautifulSoup</span><span class="p">(</span><span class="n">response</span><span class="o">.</span><span class="n">text</span><span class="p">,</span> <span class="s2">&quot;html.parser&quot;</span><span class="p">)</span>
-</span><span id="BandRipper-184"><a href="#BandRipper-184"><span class="linenos">184</span></a>        <span class="n">grid</span> <span class="o">=</span> <span class="n">soup</span><span class="o">.</span><span class="n">find</span><span class="p">(</span><span class="s2">&quot;ol&quot;</span><span class="p">,</span> <span class="n">attrs</span><span class="o">=</span><span class="p">{</span><span class="s2">&quot;id&quot;</span><span class="p">:</span> <span class="s2">&quot;music-grid&quot;</span><span class="p">})</span>
-</span><span id="BandRipper-185"><a href="#BandRipper-185"><span class="linenos">185</span></a>        <span class="n">parsed_url</span> <span class="o">=</span> <span class="n">urlparse</span><span class="p">(</span><span class="n">band_url</span><span class="p">)</span>
-</span><span id="BandRipper-186"><a href="#BandRipper-186"><span class="linenos">186</span></a>        <span class="n">base_url</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;https://</span><span class="si">{</span><span class="n">parsed_url</span><span class="o">.</span><span class="n">netloc</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="BandRipper-187"><a href="#BandRipper-187"><span class="linenos">187</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">base_url</span> <span class="o">+</span> <span class="n">album</span><span class="o">.</span><span class="n">a</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;href&quot;</span><span class="p">)</span> <span class="k">for</span> <span class="n">album</span> <span class="ow">in</span> <span class="n">grid</span><span class="o">.</span><span class="n">find_all</span><span class="p">(</span><span class="s2">&quot;li&quot;</span><span class="p">)]</span>
-</span><span id="BandRipper-188"><a href="#BandRipper-188"><span class="linenos">188</span></a>
-</span><span id="BandRipper-189"><a href="#BandRipper-189"><span class="linenos">189</span></a>    <span class="k">def</span> <span class="nf">rip</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="BandRipper-190"><a href="#BandRipper-190"><span class="linenos">190</span></a>        <span class="nb">print</span><span class="p">(</span>
-</span><span id="BandRipper-191"><a href="#BandRipper-191"><span class="linenos">191</span></a>            <span class="sa">f</span><span class="s2">&quot;Downloading </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">)</span><span class="si">}</span><span class="s2"> albums by </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">artist</span><span class="si">}</span><span class="s2">.&quot;</span>
-</span><span id="BandRipper-192"><a href="#BandRipper-192"><span class="linenos">192</span></a>        <span class="p">)</span>
-</span><span id="BandRipper-193"><a href="#BandRipper-193"><span class="linenos">193</span></a>        <span class="n">timer</span> <span class="o">=</span> <span class="n">Timer</span><span class="p">(</span><span class="n">subsecond_resolution</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="BandRipper-194"><a href="#BandRipper-194"><span class="linenos">194</span></a>        <span class="n">timer</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
-</span><span id="BandRipper-195"><a href="#BandRipper-195"><span class="linenos">195</span></a>        <span class="n">fails</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="BandRipper-196"><a href="#BandRipper-196"><span class="linenos">196</span></a>        <span class="k">for</span> <span class="n">album</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">:</span>
-</span><span id="BandRipper-197"><a href="#BandRipper-197"><span class="linenos">197</span></a>            <span class="k">try</span><span class="p">:</span>
-</span><span id="BandRipper-198"><a href="#BandRipper-198"><span class="linenos">198</span></a>                <span class="n">album</span><span class="o">.</span><span class="n">rip</span><span class="p">()</span>
-</span><span id="BandRipper-199"><a href="#BandRipper-199"><span class="linenos">199</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="BandRipper-200"><a href="#BandRipper-200"><span class="linenos">200</span></a>                <span class="n">fails</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="n">album</span><span class="p">,</span> <span class="n">e</span><span class="p">))</span>
-</span><span id="BandRipper-201"><a href="#BandRipper-201"><span class="linenos">201</span></a>        <span class="n">timer</span><span class="o">.</span><span class="n">stop</span><span class="p">()</span>
-</span><span id="BandRipper-202"><a href="#BandRipper-202"><span class="linenos">202</span></a>        <span class="n">artist</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">artist</span>
-</span><span id="BandRipper-203"><a href="#BandRipper-203"><span class="linenos">203</span></a>        <span class="nb">print</span><span class="p">(</span>
-</span><span id="BandRipper-204"><a href="#BandRipper-204"><span class="linenos">204</span></a>            <span class="sa">f</span><span class="s2">&quot;Finished downloading </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">)</span><span class="si">}</span><span class="s2"> albums by </span><span class="si">{</span><span class="n">artist</span><span class="si">}</span><span class="s2"> in </span><span class="si">{</span><span class="n">timer</span><span class="o">.</span><span class="n">elapsed_str</span><span class="si">}</span><span class="s2">.&quot;</span>
-</span><span id="BandRipper-205"><a href="#BandRipper-205"><span class="linenos">205</span></a>        <span class="p">)</span>
-</span><span id="BandRipper-206"><a href="#BandRipper-206"><span class="linenos">206</span></a>        <span class="k">if</span> <span class="n">fails</span><span class="p">:</span>
-</span><span id="BandRipper-207"><a href="#BandRipper-207"><span class="linenos">207</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;The following downloads failed:&quot;</span><span class="p">)</span>
-</span><span id="BandRipper-208"><a href="#BandRipper-208"><span class="linenos">208</span></a>            <span class="k">for</span> <span class="n">fail</span> <span class="ow">in</span> <span class="n">fails</span><span class="p">:</span>
-</span><span id="BandRipper-209"><a href="#BandRipper-209"><span class="linenos">209</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">fail</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">fail</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="BandRipper-166"><a href="#BandRipper-166"><span class="linenos">166</span></a><span class="k">class</span> <span class="nc">BandRipper</span><span class="p">:</span>
+</span><span id="BandRipper-167"><a href="#BandRipper-167"><span class="linenos">167</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
+</span><span id="BandRipper-168"><a href="#BandRipper-168"><span class="linenos">168</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">band_url</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">no_track_number</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="BandRipper-169"><a href="#BandRipper-169"><span class="linenos">169</span></a>    <span class="p">):</span>
+</span><span id="BandRipper-170"><a href="#BandRipper-170"><span class="linenos">170</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">band_url</span> <span class="o">=</span> <span class="n">band_url</span>
+</span><span id="BandRipper-171"><a href="#BandRipper-171"><span class="linenos">171</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">albums</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="BandRipper-172"><a href="#BandRipper-172"><span class="linenos">172</span></a>        <span class="k">for</span> <span class="n">url</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_album_urls</span><span class="p">(</span><span class="n">band_url</span><span class="p">):</span>
+</span><span id="BandRipper-173"><a href="#BandRipper-173"><span class="linenos">173</span></a>            <span class="k">try</span><span class="p">:</span>
+</span><span id="BandRipper-174"><a href="#BandRipper-174"><span class="linenos">174</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">AlbumRipper</span><span class="p">(</span><span class="n">url</span><span class="p">,</span> <span class="n">no_track_number</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">))</span>
+</span><span id="BandRipper-175"><a href="#BandRipper-175"><span class="linenos">175</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="BandRipper-176"><a href="#BandRipper-176"><span class="linenos">176</span></a>                <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
+</span><span id="BandRipper-177"><a href="#BandRipper-177"><span class="linenos">177</span></a>
+</span><span id="BandRipper-178"><a href="#BandRipper-178"><span class="linenos">178</span></a>    <span class="k">def</span> <span class="nf">get_album_urls</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">band_url</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
+</span><span id="BandRipper-179"><a href="#BandRipper-179"><span class="linenos">179</span></a>        <span class="sd">&quot;&quot;&quot;Get album urls from the main bandcamp url.&quot;&quot;&quot;</span>
+</span><span id="BandRipper-180"><a href="#BandRipper-180"><span class="linenos">180</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Fetching discography from </span><span class="si">{</span><span class="n">band_url</span><span class="si">}</span><span class="s2">...&quot;</span><span class="p">)</span>
+</span><span id="BandRipper-181"><a href="#BandRipper-181"><span class="linenos">181</span></a>        <span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">band_url</span><span class="p">,</span> <span class="n">headers</span><span class="o">=</span><span class="n">whosyouragent</span><span class="o">.</span><span class="n">get_agent</span><span class="p">(</span><span class="n">as_dict</span><span class="o">=</span><span class="kc">True</span><span class="p">))</span>
+</span><span id="BandRipper-182"><a href="#BandRipper-182"><span class="linenos">182</span></a>        <span class="k">if</span> <span class="n">response</span><span class="o">.</span><span class="n">status_code</span> <span class="o">!=</span> <span class="mi">200</span><span class="p">:</span>
+</span><span id="BandRipper-183"><a href="#BandRipper-183"><span class="linenos">183</span></a>            <span class="k">raise</span> <span class="ne">RuntimeError</span><span class="p">(</span>
+</span><span id="BandRipper-184"><a href="#BandRipper-184"><span class="linenos">184</span></a>                <span class="sa">f</span><span class="s2">&quot;Getting </span><span class="si">{</span><span class="n">band_url</span><span class="si">}</span><span class="s2"> failed with status code </span><span class="si">{</span><span class="n">response</span><span class="o">.</span><span class="n">status_code</span><span class="si">}</span><span class="s2">.&quot;</span>
+</span><span id="BandRipper-185"><a href="#BandRipper-185"><span class="linenos">185</span></a>            <span class="p">)</span>
+</span><span id="BandRipper-186"><a href="#BandRipper-186"><span class="linenos">186</span></a>        <span class="n">soup</span> <span class="o">=</span> <span class="n">BeautifulSoup</span><span class="p">(</span><span class="n">response</span><span class="o">.</span><span class="n">text</span><span class="p">,</span> <span class="s2">&quot;html.parser&quot;</span><span class="p">)</span>
+</span><span id="BandRipper-187"><a href="#BandRipper-187"><span class="linenos">187</span></a>        <span class="n">grid</span> <span class="o">=</span> <span class="n">soup</span><span class="o">.</span><span class="n">find</span><span class="p">(</span><span class="s2">&quot;ol&quot;</span><span class="p">,</span> <span class="n">attrs</span><span class="o">=</span><span class="p">{</span><span class="s2">&quot;id&quot;</span><span class="p">:</span> <span class="s2">&quot;music-grid&quot;</span><span class="p">})</span>
+</span><span id="BandRipper-188"><a href="#BandRipper-188"><span class="linenos">188</span></a>        <span class="n">parsed_url</span> <span class="o">=</span> <span class="n">urlparse</span><span class="p">(</span><span class="n">band_url</span><span class="p">)</span>
+</span><span id="BandRipper-189"><a href="#BandRipper-189"><span class="linenos">189</span></a>        <span class="n">base_url</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;https://</span><span class="si">{</span><span class="n">parsed_url</span><span class="o">.</span><span class="n">netloc</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="BandRipper-190"><a href="#BandRipper-190"><span class="linenos">190</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">base_url</span> <span class="o">+</span> <span class="n">album</span><span class="o">.</span><span class="n">a</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;href&quot;</span><span class="p">)</span> <span class="k">for</span> <span class="n">album</span> <span class="ow">in</span> <span class="n">grid</span><span class="o">.</span><span class="n">find_all</span><span class="p">(</span><span class="s2">&quot;li&quot;</span><span class="p">)]</span>
+</span><span id="BandRipper-191"><a href="#BandRipper-191"><span class="linenos">191</span></a>
+</span><span id="BandRipper-192"><a href="#BandRipper-192"><span class="linenos">192</span></a>    <span class="k">def</span> <span class="nf">rip</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="BandRipper-193"><a href="#BandRipper-193"><span class="linenos">193</span></a>        <span class="nb">print</span><span class="p">(</span>
+</span><span id="BandRipper-194"><a href="#BandRipper-194"><span class="linenos">194</span></a>            <span class="sa">f</span><span class="s2">&quot;Downloading </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">)</span><span class="si">}</span><span class="s2"> albums by </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">artist</span><span class="si">}</span><span class="s2">.&quot;</span>
+</span><span id="BandRipper-195"><a href="#BandRipper-195"><span class="linenos">195</span></a>        <span class="p">)</span>
+</span><span id="BandRipper-196"><a href="#BandRipper-196"><span class="linenos">196</span></a>        <span class="n">timer</span> <span class="o">=</span> <span class="n">Timer</span><span class="p">(</span><span class="n">subsecond_resolution</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="BandRipper-197"><a href="#BandRipper-197"><span class="linenos">197</span></a>        <span class="n">timer</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
+</span><span id="BandRipper-198"><a href="#BandRipper-198"><span class="linenos">198</span></a>        <span class="n">fails</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="BandRipper-199"><a href="#BandRipper-199"><span class="linenos">199</span></a>        <span class="k">for</span> <span class="n">album</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">:</span>
+</span><span id="BandRipper-200"><a href="#BandRipper-200"><span class="linenos">200</span></a>            <span class="k">try</span><span class="p">:</span>
+</span><span id="BandRipper-201"><a href="#BandRipper-201"><span class="linenos">201</span></a>                <span class="n">album</span><span class="o">.</span><span class="n">rip</span><span class="p">()</span>
+</span><span id="BandRipper-202"><a href="#BandRipper-202"><span class="linenos">202</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="BandRipper-203"><a href="#BandRipper-203"><span class="linenos">203</span></a>                <span class="n">fails</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="n">album</span><span class="p">,</span> <span class="n">e</span><span class="p">))</span>
+</span><span id="BandRipper-204"><a href="#BandRipper-204"><span class="linenos">204</span></a>        <span class="n">timer</span><span class="o">.</span><span class="n">stop</span><span class="p">()</span>
+</span><span id="BandRipper-205"><a href="#BandRipper-205"><span class="linenos">205</span></a>        <span class="n">artist</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">artist</span>
+</span><span id="BandRipper-206"><a href="#BandRipper-206"><span class="linenos">206</span></a>        <span class="nb">print</span><span class="p">(</span>
+</span><span id="BandRipper-207"><a href="#BandRipper-207"><span class="linenos">207</span></a>            <span class="sa">f</span><span class="s2">&quot;Finished downloading </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">)</span><span class="si">}</span><span class="s2"> albums by </span><span class="si">{</span><span class="n">artist</span><span class="si">}</span><span class="s2"> in </span><span class="si">{</span><span class="n">timer</span><span class="o">.</span><span class="n">elapsed_str</span><span class="si">}</span><span class="s2">.&quot;</span>
+</span><span id="BandRipper-208"><a href="#BandRipper-208"><span class="linenos">208</span></a>        <span class="p">)</span>
+</span><span id="BandRipper-209"><a href="#BandRipper-209"><span class="linenos">209</span></a>        <span class="k">if</span> <span class="n">fails</span><span class="p">:</span>
+</span><span id="BandRipper-210"><a href="#BandRipper-210"><span class="linenos">210</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;The following downloads failed:&quot;</span><span class="p">)</span>
+</span><span id="BandRipper-211"><a href="#BandRipper-211"><span class="linenos">211</span></a>            <span class="k">for</span> <span class="n">fail</span> <span class="ow">in</span> <span class="n">fails</span><span class="p">:</span>
+</span><span id="BandRipper-212"><a href="#BandRipper-212"><span class="linenos">212</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">fail</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">fail</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             <div id="BandRipper.__init__" class="classattr">
                                         <input id="BandRipper.__init__-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
@@ -939,24 +948,24 @@
             
         <span class="name">BandRipper</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="n">band_url</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">no_track_number</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>,</span><span class="param">	<span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span></span>)</span>
 
                 <label class="view-source-button" for="BandRipper.__init__-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#BandRipper.__init__"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="BandRipper.__init__-164"><a href="#BandRipper.__init__-164"><span class="linenos">164</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
-</span><span id="BandRipper.__init__-165"><a href="#BandRipper.__init__-165"><span class="linenos">165</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">band_url</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">no_track_number</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="BandRipper.__init__-166"><a href="#BandRipper.__init__-166"><span class="linenos">166</span></a>    <span class="p">):</span>
-</span><span id="BandRipper.__init__-167"><a href="#BandRipper.__init__-167"><span class="linenos">167</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">band_url</span> <span class="o">=</span> <span class="n">band_url</span>
-</span><span id="BandRipper.__init__-168"><a href="#BandRipper.__init__-168"><span class="linenos">168</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">albums</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="BandRipper.__init__-169"><a href="#BandRipper.__init__-169"><span class="linenos">169</span></a>        <span class="k">for</span> <span class="n">url</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_album_urls</span><span class="p">(</span><span class="n">band_url</span><span class="p">):</span>
-</span><span id="BandRipper.__init__-170"><a href="#BandRipper.__init__-170"><span class="linenos">170</span></a>            <span class="k">try</span><span class="p">:</span>
-</span><span id="BandRipper.__init__-171"><a href="#BandRipper.__init__-171"><span class="linenos">171</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">AlbumRipper</span><span class="p">(</span><span class="n">url</span><span class="p">,</span> <span class="n">no_track_number</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">))</span>
-</span><span id="BandRipper.__init__-172"><a href="#BandRipper.__init__-172"><span class="linenos">172</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="BandRipper.__init__-173"><a href="#BandRipper.__init__-173"><span class="linenos">173</span></a>                <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="BandRipper.__init__-167"><a href="#BandRipper.__init__-167"><span class="linenos">167</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
+</span><span id="BandRipper.__init__-168"><a href="#BandRipper.__init__-168"><span class="linenos">168</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">band_url</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">no_track_number</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="BandRipper.__init__-169"><a href="#BandRipper.__init__-169"><span class="linenos">169</span></a>    <span class="p">):</span>
+</span><span id="BandRipper.__init__-170"><a href="#BandRipper.__init__-170"><span class="linenos">170</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">band_url</span> <span class="o">=</span> <span class="n">band_url</span>
+</span><span id="BandRipper.__init__-171"><a href="#BandRipper.__init__-171"><span class="linenos">171</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">albums</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="BandRipper.__init__-172"><a href="#BandRipper.__init__-172"><span class="linenos">172</span></a>        <span class="k">for</span> <span class="n">url</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_album_urls</span><span class="p">(</span><span class="n">band_url</span><span class="p">):</span>
+</span><span id="BandRipper.__init__-173"><a href="#BandRipper.__init__-173"><span class="linenos">173</span></a>            <span class="k">try</span><span class="p">:</span>
+</span><span id="BandRipper.__init__-174"><a href="#BandRipper.__init__-174"><span class="linenos">174</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">AlbumRipper</span><span class="p">(</span><span class="n">url</span><span class="p">,</span> <span class="n">no_track_number</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">))</span>
+</span><span id="BandRipper.__init__-175"><a href="#BandRipper.__init__-175"><span class="linenos">175</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="BandRipper.__init__-176"><a href="#BandRipper.__init__-176"><span class="linenos">176</span></a>                <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
                             <div id="BandRipper.get_album_urls" class="classattr">
@@ -966,27 +975,27 @@
         <span class="def">def</span>
         <span class="name">get_album_urls</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">band_url</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span>:</span></span>
 
                 <label class="view-source-button" for="BandRipper.get_album_urls-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#BandRipper.get_album_urls"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="BandRipper.get_album_urls-175"><a href="#BandRipper.get_album_urls-175"><span class="linenos">175</span></a>    <span class="k">def</span> <span class="nf">get_album_urls</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">band_url</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
-</span><span id="BandRipper.get_album_urls-176"><a href="#BandRipper.get_album_urls-176"><span class="linenos">176</span></a>        <span class="sd">&quot;&quot;&quot;Get album urls from the main bandcamp url.&quot;&quot;&quot;</span>
-</span><span id="BandRipper.get_album_urls-177"><a href="#BandRipper.get_album_urls-177"><span class="linenos">177</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Fetching discography from </span><span class="si">{</span><span class="n">band_url</span><span class="si">}</span><span class="s2">...&quot;</span><span class="p">)</span>
-</span><span id="BandRipper.get_album_urls-178"><a href="#BandRipper.get_album_urls-178"><span class="linenos">178</span></a>        <span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">band_url</span><span class="p">,</span> <span class="n">headers</span><span class="o">=</span><span class="n">whosyouragent</span><span class="o">.</span><span class="n">get_agent</span><span class="p">(</span><span class="n">as_dict</span><span class="o">=</span><span class="kc">True</span><span class="p">))</span>
-</span><span id="BandRipper.get_album_urls-179"><a href="#BandRipper.get_album_urls-179"><span class="linenos">179</span></a>        <span class="k">if</span> <span class="n">response</span><span class="o">.</span><span class="n">status_code</span> <span class="o">!=</span> <span class="mi">200</span><span class="p">:</span>
-</span><span id="BandRipper.get_album_urls-180"><a href="#BandRipper.get_album_urls-180"><span class="linenos">180</span></a>            <span class="k">raise</span> <span class="ne">RuntimeError</span><span class="p">(</span>
-</span><span id="BandRipper.get_album_urls-181"><a href="#BandRipper.get_album_urls-181"><span class="linenos">181</span></a>                <span class="sa">f</span><span class="s2">&quot;Getting </span><span class="si">{</span><span class="n">band_url</span><span class="si">}</span><span class="s2"> failed with status code </span><span class="si">{</span><span class="n">response</span><span class="o">.</span><span class="n">status_code</span><span class="si">}</span><span class="s2">.&quot;</span>
-</span><span id="BandRipper.get_album_urls-182"><a href="#BandRipper.get_album_urls-182"><span class="linenos">182</span></a>            <span class="p">)</span>
-</span><span id="BandRipper.get_album_urls-183"><a href="#BandRipper.get_album_urls-183"><span class="linenos">183</span></a>        <span class="n">soup</span> <span class="o">=</span> <span class="n">BeautifulSoup</span><span class="p">(</span><span class="n">response</span><span class="o">.</span><span class="n">text</span><span class="p">,</span> <span class="s2">&quot;html.parser&quot;</span><span class="p">)</span>
-</span><span id="BandRipper.get_album_urls-184"><a href="#BandRipper.get_album_urls-184"><span class="linenos">184</span></a>        <span class="n">grid</span> <span class="o">=</span> <span class="n">soup</span><span class="o">.</span><span class="n">find</span><span class="p">(</span><span class="s2">&quot;ol&quot;</span><span class="p">,</span> <span class="n">attrs</span><span class="o">=</span><span class="p">{</span><span class="s2">&quot;id&quot;</span><span class="p">:</span> <span class="s2">&quot;music-grid&quot;</span><span class="p">})</span>
-</span><span id="BandRipper.get_album_urls-185"><a href="#BandRipper.get_album_urls-185"><span class="linenos">185</span></a>        <span class="n">parsed_url</span> <span class="o">=</span> <span class="n">urlparse</span><span class="p">(</span><span class="n">band_url</span><span class="p">)</span>
-</span><span id="BandRipper.get_album_urls-186"><a href="#BandRipper.get_album_urls-186"><span class="linenos">186</span></a>        <span class="n">base_url</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;https://</span><span class="si">{</span><span class="n">parsed_url</span><span class="o">.</span><span class="n">netloc</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="BandRipper.get_album_urls-187"><a href="#BandRipper.get_album_urls-187"><span class="linenos">187</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">base_url</span> <span class="o">+</span> <span class="n">album</span><span class="o">.</span><span class="n">a</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;href&quot;</span><span class="p">)</span> <span class="k">for</span> <span class="n">album</span> <span class="ow">in</span> <span class="n">grid</span><span class="o">.</span><span class="n">find_all</span><span class="p">(</span><span class="s2">&quot;li&quot;</span><span class="p">)]</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="BandRipper.get_album_urls-178"><a href="#BandRipper.get_album_urls-178"><span class="linenos">178</span></a>    <span class="k">def</span> <span class="nf">get_album_urls</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">band_url</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
+</span><span id="BandRipper.get_album_urls-179"><a href="#BandRipper.get_album_urls-179"><span class="linenos">179</span></a>        <span class="sd">&quot;&quot;&quot;Get album urls from the main bandcamp url.&quot;&quot;&quot;</span>
+</span><span id="BandRipper.get_album_urls-180"><a href="#BandRipper.get_album_urls-180"><span class="linenos">180</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Fetching discography from </span><span class="si">{</span><span class="n">band_url</span><span class="si">}</span><span class="s2">...&quot;</span><span class="p">)</span>
+</span><span id="BandRipper.get_album_urls-181"><a href="#BandRipper.get_album_urls-181"><span class="linenos">181</span></a>        <span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">band_url</span><span class="p">,</span> <span class="n">headers</span><span class="o">=</span><span class="n">whosyouragent</span><span class="o">.</span><span class="n">get_agent</span><span class="p">(</span><span class="n">as_dict</span><span class="o">=</span><span class="kc">True</span><span class="p">))</span>
+</span><span id="BandRipper.get_album_urls-182"><a href="#BandRipper.get_album_urls-182"><span class="linenos">182</span></a>        <span class="k">if</span> <span class="n">response</span><span class="o">.</span><span class="n">status_code</span> <span class="o">!=</span> <span class="mi">200</span><span class="p">:</span>
+</span><span id="BandRipper.get_album_urls-183"><a href="#BandRipper.get_album_urls-183"><span class="linenos">183</span></a>            <span class="k">raise</span> <span class="ne">RuntimeError</span><span class="p">(</span>
+</span><span id="BandRipper.get_album_urls-184"><a href="#BandRipper.get_album_urls-184"><span class="linenos">184</span></a>                <span class="sa">f</span><span class="s2">&quot;Getting </span><span class="si">{</span><span class="n">band_url</span><span class="si">}</span><span class="s2"> failed with status code </span><span class="si">{</span><span class="n">response</span><span class="o">.</span><span class="n">status_code</span><span class="si">}</span><span class="s2">.&quot;</span>
+</span><span id="BandRipper.get_album_urls-185"><a href="#BandRipper.get_album_urls-185"><span class="linenos">185</span></a>            <span class="p">)</span>
+</span><span id="BandRipper.get_album_urls-186"><a href="#BandRipper.get_album_urls-186"><span class="linenos">186</span></a>        <span class="n">soup</span> <span class="o">=</span> <span class="n">BeautifulSoup</span><span class="p">(</span><span class="n">response</span><span class="o">.</span><span class="n">text</span><span class="p">,</span> <span class="s2">&quot;html.parser&quot;</span><span class="p">)</span>
+</span><span id="BandRipper.get_album_urls-187"><a href="#BandRipper.get_album_urls-187"><span class="linenos">187</span></a>        <span class="n">grid</span> <span class="o">=</span> <span class="n">soup</span><span class="o">.</span><span class="n">find</span><span class="p">(</span><span class="s2">&quot;ol&quot;</span><span class="p">,</span> <span class="n">attrs</span><span class="o">=</span><span class="p">{</span><span class="s2">&quot;id&quot;</span><span class="p">:</span> <span class="s2">&quot;music-grid&quot;</span><span class="p">})</span>
+</span><span id="BandRipper.get_album_urls-188"><a href="#BandRipper.get_album_urls-188"><span class="linenos">188</span></a>        <span class="n">parsed_url</span> <span class="o">=</span> <span class="n">urlparse</span><span class="p">(</span><span class="n">band_url</span><span class="p">)</span>
+</span><span id="BandRipper.get_album_urls-189"><a href="#BandRipper.get_album_urls-189"><span class="linenos">189</span></a>        <span class="n">base_url</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;https://</span><span class="si">{</span><span class="n">parsed_url</span><span class="o">.</span><span class="n">netloc</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="BandRipper.get_album_urls-190"><a href="#BandRipper.get_album_urls-190"><span class="linenos">190</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">base_url</span> <span class="o">+</span> <span class="n">album</span><span class="o">.</span><span class="n">a</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;href&quot;</span><span class="p">)</span> <span class="k">for</span> <span class="n">album</span> <span class="ow">in</span> <span class="n">grid</span><span class="o">.</span><span class="n">find_all</span><span class="p">(</span><span class="s2">&quot;li&quot;</span><span class="p">)]</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Get album urls from the main bandcamp url.</p>
 </div>
 
 
@@ -998,35 +1007,35 @@
         <span class="def">def</span>
         <span class="name">rip</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="BandRipper.rip-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#BandRipper.rip"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="BandRipper.rip-189"><a href="#BandRipper.rip-189"><span class="linenos">189</span></a>    <span class="k">def</span> <span class="nf">rip</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="BandRipper.rip-190"><a href="#BandRipper.rip-190"><span class="linenos">190</span></a>        <span class="nb">print</span><span class="p">(</span>
-</span><span id="BandRipper.rip-191"><a href="#BandRipper.rip-191"><span class="linenos">191</span></a>            <span class="sa">f</span><span class="s2">&quot;Downloading </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">)</span><span class="si">}</span><span class="s2"> albums by </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">artist</span><span class="si">}</span><span class="s2">.&quot;</span>
-</span><span id="BandRipper.rip-192"><a href="#BandRipper.rip-192"><span class="linenos">192</span></a>        <span class="p">)</span>
-</span><span id="BandRipper.rip-193"><a href="#BandRipper.rip-193"><span class="linenos">193</span></a>        <span class="n">timer</span> <span class="o">=</span> <span class="n">Timer</span><span class="p">(</span><span class="n">subsecond_resolution</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="BandRipper.rip-194"><a href="#BandRipper.rip-194"><span class="linenos">194</span></a>        <span class="n">timer</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
-</span><span id="BandRipper.rip-195"><a href="#BandRipper.rip-195"><span class="linenos">195</span></a>        <span class="n">fails</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="BandRipper.rip-196"><a href="#BandRipper.rip-196"><span class="linenos">196</span></a>        <span class="k">for</span> <span class="n">album</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">:</span>
-</span><span id="BandRipper.rip-197"><a href="#BandRipper.rip-197"><span class="linenos">197</span></a>            <span class="k">try</span><span class="p">:</span>
-</span><span id="BandRipper.rip-198"><a href="#BandRipper.rip-198"><span class="linenos">198</span></a>                <span class="n">album</span><span class="o">.</span><span class="n">rip</span><span class="p">()</span>
-</span><span id="BandRipper.rip-199"><a href="#BandRipper.rip-199"><span class="linenos">199</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="BandRipper.rip-200"><a href="#BandRipper.rip-200"><span class="linenos">200</span></a>                <span class="n">fails</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="n">album</span><span class="p">,</span> <span class="n">e</span><span class="p">))</span>
-</span><span id="BandRipper.rip-201"><a href="#BandRipper.rip-201"><span class="linenos">201</span></a>        <span class="n">timer</span><span class="o">.</span><span class="n">stop</span><span class="p">()</span>
-</span><span id="BandRipper.rip-202"><a href="#BandRipper.rip-202"><span class="linenos">202</span></a>        <span class="n">artist</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">artist</span>
-</span><span id="BandRipper.rip-203"><a href="#BandRipper.rip-203"><span class="linenos">203</span></a>        <span class="nb">print</span><span class="p">(</span>
-</span><span id="BandRipper.rip-204"><a href="#BandRipper.rip-204"><span class="linenos">204</span></a>            <span class="sa">f</span><span class="s2">&quot;Finished downloading </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">)</span><span class="si">}</span><span class="s2"> albums by </span><span class="si">{</span><span class="n">artist</span><span class="si">}</span><span class="s2"> in </span><span class="si">{</span><span class="n">timer</span><span class="o">.</span><span class="n">elapsed_str</span><span class="si">}</span><span class="s2">.&quot;</span>
-</span><span id="BandRipper.rip-205"><a href="#BandRipper.rip-205"><span class="linenos">205</span></a>        <span class="p">)</span>
-</span><span id="BandRipper.rip-206"><a href="#BandRipper.rip-206"><span class="linenos">206</span></a>        <span class="k">if</span> <span class="n">fails</span><span class="p">:</span>
-</span><span id="BandRipper.rip-207"><a href="#BandRipper.rip-207"><span class="linenos">207</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;The following downloads failed:&quot;</span><span class="p">)</span>
-</span><span id="BandRipper.rip-208"><a href="#BandRipper.rip-208"><span class="linenos">208</span></a>            <span class="k">for</span> <span class="n">fail</span> <span class="ow">in</span> <span class="n">fails</span><span class="p">:</span>
-</span><span id="BandRipper.rip-209"><a href="#BandRipper.rip-209"><span class="linenos">209</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">fail</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">fail</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="BandRipper.rip-192"><a href="#BandRipper.rip-192"><span class="linenos">192</span></a>    <span class="k">def</span> <span class="nf">rip</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="BandRipper.rip-193"><a href="#BandRipper.rip-193"><span class="linenos">193</span></a>        <span class="nb">print</span><span class="p">(</span>
+</span><span id="BandRipper.rip-194"><a href="#BandRipper.rip-194"><span class="linenos">194</span></a>            <span class="sa">f</span><span class="s2">&quot;Downloading </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">)</span><span class="si">}</span><span class="s2"> albums by </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">artist</span><span class="si">}</span><span class="s2">.&quot;</span>
+</span><span id="BandRipper.rip-195"><a href="#BandRipper.rip-195"><span class="linenos">195</span></a>        <span class="p">)</span>
+</span><span id="BandRipper.rip-196"><a href="#BandRipper.rip-196"><span class="linenos">196</span></a>        <span class="n">timer</span> <span class="o">=</span> <span class="n">Timer</span><span class="p">(</span><span class="n">subsecond_resolution</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="BandRipper.rip-197"><a href="#BandRipper.rip-197"><span class="linenos">197</span></a>        <span class="n">timer</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
+</span><span id="BandRipper.rip-198"><a href="#BandRipper.rip-198"><span class="linenos">198</span></a>        <span class="n">fails</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="BandRipper.rip-199"><a href="#BandRipper.rip-199"><span class="linenos">199</span></a>        <span class="k">for</span> <span class="n">album</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">:</span>
+</span><span id="BandRipper.rip-200"><a href="#BandRipper.rip-200"><span class="linenos">200</span></a>            <span class="k">try</span><span class="p">:</span>
+</span><span id="BandRipper.rip-201"><a href="#BandRipper.rip-201"><span class="linenos">201</span></a>                <span class="n">album</span><span class="o">.</span><span class="n">rip</span><span class="p">()</span>
+</span><span id="BandRipper.rip-202"><a href="#BandRipper.rip-202"><span class="linenos">202</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="BandRipper.rip-203"><a href="#BandRipper.rip-203"><span class="linenos">203</span></a>                <span class="n">fails</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="n">album</span><span class="p">,</span> <span class="n">e</span><span class="p">))</span>
+</span><span id="BandRipper.rip-204"><a href="#BandRipper.rip-204"><span class="linenos">204</span></a>        <span class="n">timer</span><span class="o">.</span><span class="n">stop</span><span class="p">()</span>
+</span><span id="BandRipper.rip-205"><a href="#BandRipper.rip-205"><span class="linenos">205</span></a>        <span class="n">artist</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">artist</span>
+</span><span id="BandRipper.rip-206"><a href="#BandRipper.rip-206"><span class="linenos">206</span></a>        <span class="nb">print</span><span class="p">(</span>
+</span><span id="BandRipper.rip-207"><a href="#BandRipper.rip-207"><span class="linenos">207</span></a>            <span class="sa">f</span><span class="s2">&quot;Finished downloading </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">)</span><span class="si">}</span><span class="s2"> albums by </span><span class="si">{</span><span class="n">artist</span><span class="si">}</span><span class="s2"> in </span><span class="si">{</span><span class="n">timer</span><span class="o">.</span><span class="n">elapsed_str</span><span class="si">}</span><span class="s2">.&quot;</span>
+</span><span id="BandRipper.rip-208"><a href="#BandRipper.rip-208"><span class="linenos">208</span></a>        <span class="p">)</span>
+</span><span id="BandRipper.rip-209"><a href="#BandRipper.rip-209"><span class="linenos">209</span></a>        <span class="k">if</span> <span class="n">fails</span><span class="p">:</span>
+</span><span id="BandRipper.rip-210"><a href="#BandRipper.rip-210"><span class="linenos">210</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;The following downloads failed:&quot;</span><span class="p">)</span>
+</span><span id="BandRipper.rip-211"><a href="#BandRipper.rip-211"><span class="linenos">211</span></a>            <span class="k">for</span> <span class="n">fail</span> <span class="ow">in</span> <span class="n">fails</span><span class="p">:</span>
+</span><span id="BandRipper.rip-212"><a href="#BandRipper.rip-212"><span class="linenos">212</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">fail</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">fail</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
                 </section>
@@ -1037,27 +1046,27 @@
         <span class="def">def</span>
         <span class="name">page_is_discography</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">url</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">bool</span>:</span></span>
 
                 <label class="view-source-button" for="page_is_discography-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#page_is_discography"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="page_is_discography-212"><a href="#page_is_discography-212"><span class="linenos">212</span></a><span class="k">def</span> <span class="nf">page_is_discography</span><span class="p">(</span><span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="page_is_discography-213"><a href="#page_is_discography-213"><span class="linenos">213</span></a>    <span class="sd">&quot;&quot;&quot;Returns whether the url is to a discography page or not.&quot;&quot;&quot;</span>
-</span><span id="page_is_discography-214"><a href="#page_is_discography-214"><span class="linenos">214</span></a>    <span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">url</span><span class="p">,</span> <span class="n">headers</span><span class="o">=</span><span class="n">whosyouragent</span><span class="o">.</span><span class="n">get_agent</span><span class="p">(</span><span class="n">as_dict</span><span class="o">=</span><span class="kc">True</span><span class="p">))</span>
-</span><span id="page_is_discography-215"><a href="#page_is_discography-215"><span class="linenos">215</span></a>    <span class="k">if</span> <span class="n">response</span><span class="o">.</span><span class="n">status_code</span> <span class="o">!=</span> <span class="mi">200</span><span class="p">:</span>
-</span><span id="page_is_discography-216"><a href="#page_is_discography-216"><span class="linenos">216</span></a>        <span class="k">raise</span> <span class="ne">RuntimeError</span><span class="p">(</span>
-</span><span id="page_is_discography-217"><a href="#page_is_discography-217"><span class="linenos">217</span></a>            <span class="sa">f</span><span class="s2">&quot;Getting </span><span class="si">{</span><span class="n">url</span><span class="si">}</span><span class="s2"> failed with status code </span><span class="si">{</span><span class="n">response</span><span class="o">.</span><span class="n">status_code</span><span class="si">}</span><span class="s2">.&quot;</span>
-</span><span id="page_is_discography-218"><a href="#page_is_discography-218"><span class="linenos">218</span></a>        <span class="p">)</span>
-</span><span id="page_is_discography-219"><a href="#page_is_discography-219"><span class="linenos">219</span></a>    <span class="n">soup</span> <span class="o">=</span> <span class="n">BeautifulSoup</span><span class="p">(</span><span class="n">response</span><span class="o">.</span><span class="n">text</span><span class="p">,</span> <span class="s2">&quot;html.parser&quot;</span><span class="p">)</span>
-</span><span id="page_is_discography-220"><a href="#page_is_discography-220"><span class="linenos">220</span></a>    <span class="c1"># Returns None if it doesn&#39;t exist.</span>
-</span><span id="page_is_discography-221"><a href="#page_is_discography-221"><span class="linenos">221</span></a>    <span class="n">grid</span> <span class="o">=</span> <span class="n">soup</span><span class="o">.</span><span class="n">find</span><span class="p">(</span><span class="s2">&quot;ol&quot;</span><span class="p">,</span> <span class="n">attrs</span><span class="o">=</span><span class="p">{</span><span class="s2">&quot;id&quot;</span><span class="p">:</span> <span class="s2">&quot;music-grid&quot;</span><span class="p">})</span>
-</span><span id="page_is_discography-222"><a href="#page_is_discography-222"><span class="linenos">222</span></a>    <span class="k">if</span> <span class="n">grid</span><span class="p">:</span>
-</span><span id="page_is_discography-223"><a href="#page_is_discography-223"><span class="linenos">223</span></a>        <span class="k">return</span> <span class="kc">True</span>
-</span><span id="page_is_discography-224"><a href="#page_is_discography-224"><span class="linenos">224</span></a>    <span class="k">return</span> <span class="kc">False</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="page_is_discography-215"><a href="#page_is_discography-215"><span class="linenos">215</span></a><span class="k">def</span> <span class="nf">page_is_discography</span><span class="p">(</span><span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="page_is_discography-216"><a href="#page_is_discography-216"><span class="linenos">216</span></a>    <span class="sd">&quot;&quot;&quot;Returns whether the url is to a discography page or not.&quot;&quot;&quot;</span>
+</span><span id="page_is_discography-217"><a href="#page_is_discography-217"><span class="linenos">217</span></a>    <span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">url</span><span class="p">,</span> <span class="n">headers</span><span class="o">=</span><span class="n">whosyouragent</span><span class="o">.</span><span class="n">get_agent</span><span class="p">(</span><span class="n">as_dict</span><span class="o">=</span><span class="kc">True</span><span class="p">))</span>
+</span><span id="page_is_discography-218"><a href="#page_is_discography-218"><span class="linenos">218</span></a>    <span class="k">if</span> <span class="n">response</span><span class="o">.</span><span class="n">status_code</span> <span class="o">!=</span> <span class="mi">200</span><span class="p">:</span>
+</span><span id="page_is_discography-219"><a href="#page_is_discography-219"><span class="linenos">219</span></a>        <span class="k">raise</span> <span class="ne">RuntimeError</span><span class="p">(</span>
+</span><span id="page_is_discography-220"><a href="#page_is_discography-220"><span class="linenos">220</span></a>            <span class="sa">f</span><span class="s2">&quot;Getting </span><span class="si">{</span><span class="n">url</span><span class="si">}</span><span class="s2"> failed with status code </span><span class="si">{</span><span class="n">response</span><span class="o">.</span><span class="n">status_code</span><span class="si">}</span><span class="s2">.&quot;</span>
+</span><span id="page_is_discography-221"><a href="#page_is_discography-221"><span class="linenos">221</span></a>        <span class="p">)</span>
+</span><span id="page_is_discography-222"><a href="#page_is_discography-222"><span class="linenos">222</span></a>    <span class="n">soup</span> <span class="o">=</span> <span class="n">BeautifulSoup</span><span class="p">(</span><span class="n">response</span><span class="o">.</span><span class="n">text</span><span class="p">,</span> <span class="s2">&quot;html.parser&quot;</span><span class="p">)</span>
+</span><span id="page_is_discography-223"><a href="#page_is_discography-223"><span class="linenos">223</span></a>    <span class="c1"># Returns None if it doesn&#39;t exist.</span>
+</span><span id="page_is_discography-224"><a href="#page_is_discography-224"><span class="linenos">224</span></a>    <span class="n">grid</span> <span class="o">=</span> <span class="n">soup</span><span class="o">.</span><span class="n">find</span><span class="p">(</span><span class="s2">&quot;ol&quot;</span><span class="p">,</span> <span class="n">attrs</span><span class="o">=</span><span class="p">{</span><span class="s2">&quot;id&quot;</span><span class="p">:</span> <span class="s2">&quot;music-grid&quot;</span><span class="p">})</span>
+</span><span id="page_is_discography-225"><a href="#page_is_discography-225"><span class="linenos">225</span></a>    <span class="k">if</span> <span class="n">grid</span><span class="p">:</span>
+</span><span id="page_is_discography-226"><a href="#page_is_discography-226"><span class="linenos">226</span></a>        <span class="k">return</span> <span class="kc">True</span>
+</span><span id="page_is_discography-227"><a href="#page_is_discography-227"><span class="linenos">227</span></a>    <span class="k">return</span> <span class="kc">False</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Returns whether the url is to a discography page or not.</p>
 </div>
 
 
@@ -1069,51 +1078,51 @@
         <span class="def">def</span>
         <span class="name">get_args</span><span class="signature pdoc-code condensed">(<span class="return-annotation">) -> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span>:</span></span>
 
                 <label class="view-source-button" for="get_args-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#get_args"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="get_args-227"><a href="#get_args-227"><span class="linenos">227</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
-</span><span id="get_args-228"><a href="#get_args-228"><span class="linenos">228</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
-</span><span id="get_args-229"><a href="#get_args-229"><span class="linenos">229</span></a>
-</span><span id="get_args-230"><a href="#get_args-230"><span class="linenos">230</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-231"><a href="#get_args-231"><span class="linenos">231</span></a>        <span class="s2">&quot;urls&quot;</span><span class="p">,</span>
-</span><span id="get_args-232"><a href="#get_args-232"><span class="linenos">232</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="get_args-233"><a href="#get_args-233"><span class="linenos">233</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
-</span><span id="get_args-234"><a href="#get_args-234"><span class="linenos">234</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The bandcamp url(s) for the album or artist.</span>
-</span><span id="get_args-235"><a href="#get_args-235"><span class="linenos">235</span></a><span class="s2">            If the url is to an artists main page,</span>
-</span><span id="get_args-236"><a href="#get_args-236"><span class="linenos">236</span></a><span class="s2">            all albums will be downloaded.</span>
-</span><span id="get_args-237"><a href="#get_args-237"><span class="linenos">237</span></a><span class="s2">            The tracks will be saved to a subdirectory of</span>
-</span><span id="get_args-238"><a href="#get_args-238"><span class="linenos">238</span></a><span class="s2">            your current directory.</span>
-</span><span id="get_args-239"><a href="#get_args-239"><span class="linenos">239</span></a><span class="s2">            If a track can&#39;t be streamed (i.e. private) it</span>
-</span><span id="get_args-240"><a href="#get_args-240"><span class="linenos">240</span></a><span class="s2">            won&#39;t be downloaded. Multiple urls can be passed.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-241"><a href="#get_args-241"><span class="linenos">241</span></a>    <span class="p">)</span>
-</span><span id="get_args-242"><a href="#get_args-242"><span class="linenos">242</span></a>
-</span><span id="get_args-243"><a href="#get_args-243"><span class="linenos">243</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-244"><a href="#get_args-244"><span class="linenos">244</span></a>        <span class="s2">&quot;-n&quot;</span><span class="p">,</span>
-</span><span id="get_args-245"><a href="#get_args-245"><span class="linenos">245</span></a>        <span class="s2">&quot;--no_track_number&quot;</span><span class="p">,</span>
-</span><span id="get_args-246"><a href="#get_args-246"><span class="linenos">246</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="get_args-247"><a href="#get_args-247"><span class="linenos">247</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; By default the track number will be added</span>
-</span><span id="get_args-248"><a href="#get_args-248"><span class="linenos">248</span></a><span class="s2">        to the front of the track title. Pass this switch</span>
-</span><span id="get_args-249"><a href="#get_args-249"><span class="linenos">249</span></a><span class="s2">        to disable the behavior.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-250"><a href="#get_args-250"><span class="linenos">250</span></a>    <span class="p">)</span>
-</span><span id="get_args-251"><a href="#get_args-251"><span class="linenos">251</span></a>
-</span><span id="get_args-252"><a href="#get_args-252"><span class="linenos">252</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-253"><a href="#get_args-253"><span class="linenos">253</span></a>        <span class="s2">&quot;-o&quot;</span><span class="p">,</span>
-</span><span id="get_args-254"><a href="#get_args-254"><span class="linenos">254</span></a>        <span class="s2">&quot;--overwrite&quot;</span><span class="p">,</span>
-</span><span id="get_args-255"><a href="#get_args-255"><span class="linenos">255</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="get_args-256"><a href="#get_args-256"><span class="linenos">256</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Pass this flag to overwrite existing files.</span>
-</span><span id="get_args-257"><a href="#get_args-257"><span class="linenos">257</span></a><span class="s2">        Otherwise don&#39;t download tracks that already exist locally.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-258"><a href="#get_args-258"><span class="linenos">258</span></a>    <span class="p">)</span>
-</span><span id="get_args-259"><a href="#get_args-259"><span class="linenos">259</span></a>
-</span><span id="get_args-260"><a href="#get_args-260"><span class="linenos">260</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
-</span><span id="get_args-261"><a href="#get_args-261"><span class="linenos">261</span></a>    <span class="n">args</span><span class="o">.</span><span class="n">urls</span> <span class="o">=</span> <span class="p">[</span><span class="n">url</span><span class="o">.</span><span class="n">strip</span><span class="p">(</span><span class="s2">&quot;/&quot;</span><span class="p">)</span> <span class="k">for</span> <span class="n">url</span> <span class="ow">in</span> <span class="n">args</span><span class="o">.</span><span class="n">urls</span><span class="p">]</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="get_args-230"><a href="#get_args-230"><span class="linenos">230</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
+</span><span id="get_args-231"><a href="#get_args-231"><span class="linenos">231</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
+</span><span id="get_args-232"><a href="#get_args-232"><span class="linenos">232</span></a>
+</span><span id="get_args-233"><a href="#get_args-233"><span class="linenos">233</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-234"><a href="#get_args-234"><span class="linenos">234</span></a>        <span class="s2">&quot;urls&quot;</span><span class="p">,</span>
+</span><span id="get_args-235"><a href="#get_args-235"><span class="linenos">235</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="get_args-236"><a href="#get_args-236"><span class="linenos">236</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
+</span><span id="get_args-237"><a href="#get_args-237"><span class="linenos">237</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The bandcamp url(s) for the album or artist.</span>
+</span><span id="get_args-238"><a href="#get_args-238"><span class="linenos">238</span></a><span class="s2">            If the url is to an artists main page,</span>
+</span><span id="get_args-239"><a href="#get_args-239"><span class="linenos">239</span></a><span class="s2">            all albums will be downloaded.</span>
+</span><span id="get_args-240"><a href="#get_args-240"><span class="linenos">240</span></a><span class="s2">            The tracks will be saved to a subdirectory of</span>
+</span><span id="get_args-241"><a href="#get_args-241"><span class="linenos">241</span></a><span class="s2">            your current directory.</span>
+</span><span id="get_args-242"><a href="#get_args-242"><span class="linenos">242</span></a><span class="s2">            If a track can&#39;t be streamed (i.e. private) it</span>
+</span><span id="get_args-243"><a href="#get_args-243"><span class="linenos">243</span></a><span class="s2">            won&#39;t be downloaded. Multiple urls can be passed.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-244"><a href="#get_args-244"><span class="linenos">244</span></a>    <span class="p">)</span>
+</span><span id="get_args-245"><a href="#get_args-245"><span class="linenos">245</span></a>
+</span><span id="get_args-246"><a href="#get_args-246"><span class="linenos">246</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-247"><a href="#get_args-247"><span class="linenos">247</span></a>        <span class="s2">&quot;-n&quot;</span><span class="p">,</span>
+</span><span id="get_args-248"><a href="#get_args-248"><span class="linenos">248</span></a>        <span class="s2">&quot;--no_track_number&quot;</span><span class="p">,</span>
+</span><span id="get_args-249"><a href="#get_args-249"><span class="linenos">249</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="get_args-250"><a href="#get_args-250"><span class="linenos">250</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; By default the track number will be added</span>
+</span><span id="get_args-251"><a href="#get_args-251"><span class="linenos">251</span></a><span class="s2">        to the front of the track title. Pass this switch</span>
+</span><span id="get_args-252"><a href="#get_args-252"><span class="linenos">252</span></a><span class="s2">        to disable the behavior.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-253"><a href="#get_args-253"><span class="linenos">253</span></a>    <span class="p">)</span>
+</span><span id="get_args-254"><a href="#get_args-254"><span class="linenos">254</span></a>
+</span><span id="get_args-255"><a href="#get_args-255"><span class="linenos">255</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-256"><a href="#get_args-256"><span class="linenos">256</span></a>        <span class="s2">&quot;-o&quot;</span><span class="p">,</span>
+</span><span id="get_args-257"><a href="#get_args-257"><span class="linenos">257</span></a>        <span class="s2">&quot;--overwrite&quot;</span><span class="p">,</span>
+</span><span id="get_args-258"><a href="#get_args-258"><span class="linenos">258</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="get_args-259"><a href="#get_args-259"><span class="linenos">259</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Pass this flag to overwrite existing files.</span>
+</span><span id="get_args-260"><a href="#get_args-260"><span class="linenos">260</span></a><span class="s2">        Otherwise don&#39;t download tracks that already exist locally.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-261"><a href="#get_args-261"><span class="linenos">261</span></a>    <span class="p">)</span>
 </span><span id="get_args-262"><a href="#get_args-262"><span class="linenos">262</span></a>
-</span><span id="get_args-263"><a href="#get_args-263"><span class="linenos">263</span></a>    <span class="k">return</span> <span class="n">args</span>
+</span><span id="get_args-263"><a href="#get_args-263"><span class="linenos">263</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
+</span><span id="get_args-264"><a href="#get_args-264"><span class="linenos">264</span></a>    <span class="n">args</span><span class="o">.</span><span class="n">urls</span> <span class="o">=</span> <span class="p">[</span><span class="n">url</span><span class="o">.</span><span class="n">strip</span><span class="p">(</span><span class="s2">&quot;/&quot;</span><span class="p">)</span> <span class="k">for</span> <span class="n">url</span> <span class="ow">in</span> <span class="n">args</span><span class="o">.</span><span class="n">urls</span><span class="p">]</span>
+</span><span id="get_args-265"><a href="#get_args-265"><span class="linenos">265</span></a>
+</span><span id="get_args-266"><a href="#get_args-266"><span class="linenos">266</span></a>    <span class="k">return</span> <span class="n">args</span>
 </span></pre></div>
 
 
     
 
                 </section>
                 <section id="main">
@@ -1123,23 +1132,23 @@
         <span class="def">def</span>
         <span class="name">main</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="main-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#main"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="main-266"><a href="#main-266"><span class="linenos">266</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="main-267"><a href="#main-267"><span class="linenos">267</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
-</span><span id="main-268"><a href="#main-268"><span class="linenos">268</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
-</span><span id="main-269"><a href="#main-269"><span class="linenos">269</span></a>    <span class="k">for</span> <span class="n">url</span> <span class="ow">in</span> <span class="n">args</span><span class="o">.</span><span class="n">urls</span><span class="p">:</span>
-</span><span id="main-270"><a href="#main-270"><span class="linenos">270</span></a>        <span class="k">if</span> <span class="n">page_is_discography</span><span class="p">(</span><span class="n">url</span><span class="p">):</span>
-</span><span id="main-271"><a href="#main-271"><span class="linenos">271</span></a>            <span class="n">ripper</span> <span class="o">=</span> <span class="n">BandRipper</span><span class="p">(</span><span class="n">url</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">no_track_number</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">overwrite</span><span class="p">)</span>
-</span><span id="main-272"><a href="#main-272"><span class="linenos">272</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="main-273"><a href="#main-273"><span class="linenos">273</span></a>            <span class="n">ripper</span> <span class="o">=</span> <span class="n">AlbumRipper</span><span class="p">(</span><span class="n">url</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">no_track_number</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">overwrite</span><span class="p">)</span>
-</span><span id="main-274"><a href="#main-274"><span class="linenos">274</span></a>        <span class="n">ripper</span><span class="o">.</span><span class="n">rip</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="main-269"><a href="#main-269"><span class="linenos">269</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="main-270"><a href="#main-270"><span class="linenos">270</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
+</span><span id="main-271"><a href="#main-271"><span class="linenos">271</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="main-272"><a href="#main-272"><span class="linenos">272</span></a>    <span class="k">for</span> <span class="n">url</span> <span class="ow">in</span> <span class="n">args</span><span class="o">.</span><span class="n">urls</span><span class="p">:</span>
+</span><span id="main-273"><a href="#main-273"><span class="linenos">273</span></a>        <span class="k">if</span> <span class="n">page_is_discography</span><span class="p">(</span><span class="n">url</span><span class="p">):</span>
+</span><span id="main-274"><a href="#main-274"><span class="linenos">274</span></a>            <span class="n">ripper</span> <span class="o">=</span> <span class="n">BandRipper</span><span class="p">(</span><span class="n">url</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">no_track_number</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">overwrite</span><span class="p">)</span>
+</span><span id="main-275"><a href="#main-275"><span class="linenos">275</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="main-276"><a href="#main-276"><span class="linenos">276</span></a>            <span class="n">ripper</span> <span class="o">=</span> <span class="n">AlbumRipper</span><span class="p">(</span><span class="n">url</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">no_track_number</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">overwrite</span><span class="p">)</span>
+</span><span id="main-277"><a href="#main-277"><span class="linenos">277</span></a>        <span class="n">ripper</span><span class="o">.</span><span class="n">rip</span><span class="p">()</span>
 </span></pre></div>
 
 
     
 
                 </section>
     </main>
```

#### html2text {}

```diff
@@ -166,167 +166,170 @@
 129    def rip(self):
 130        """Download and save the album tracks and album art."""
 131        if len(self.album.tracks) == 0:
 132            print(f"No public tracks available for {self.album}.")
 133            return None
 134        self.make_save_path()
 135        self.download_album_art()
-136        bar = ProgBar(len(self.album.tracks) - 1, width_ratio=0.5)
-137        fails = []
-138        if not self.overwrite:
-139            self.album.tracks = [
-140                track for track in self.album.tracks if not
+136        num_tracks = len(self.album.tracks)
+137        bar = ProgBar(num_tracks, width_ratio=0.5)
+138        fails = []
+139        if not self.overwrite:
+140            self.album.tracks = [
+141                track for track in self.album.tracks if not
 self.track_exists(track)
-141            ]
-142        for track in self.album.tracks:
-143            bar.display(
-144                suffix=f"Downloading {track.title}",
-145                counter_override=1 if len(self.album.tracks) == 1 else None,
-146            )
-147            try:
-148                content = self.get_track_content(track.url)
-149                self.save_track(
-150                    track.title if self.no_track_number else
+142            ]
+143        for i, track in enumerate(self.album.tracks, 1):
+144            bar.display(
+145                suffix=f"Downloading track {i}/{num_tracks}: {track.title}",
+146                counter_override=1 if len(self.album.tracks) == 1 else None,
+147            )
+148            try:
+149                content = self.get_track_content(track.url)
+150                self.save_track(
+151                    track.title if self.no_track_number else
 track.numbered_title,
-151                    content,
-152                )
-153            except Exception as e:
-154                fails.append((track, str(e)))
-155        print(f"Finished downloading {self.album} in
-{bar.timer.elapsed_str}.")
-156        if fails:
-157            print("The following tracks failed to download:")
-158            for fail in fails:
-159                print(f"{fail[0].title}: {fail[1]}")
-160
-161
-162class BandRipper:
-163    def __init__(
-164        self, band_url: str, no_track_number: bool = False, overwrite: bool
+152                    content,
+153                )
+154            except Exception as e:
+155                fails.append((track, str(e)))
+156        print(
+157            f"Finished downloading {num_tracks - len(fails)} tracks from
+{self.album} in {bar.timer.elapsed_str}."
+158        )
+159        if fails:
+160            print("The following tracks failed to download:")
+161            for fail in fails:
+162                print(f"{fail[0].title}: {fail[1]}")
+163
+164
+165class BandRipper:
+166    def __init__(
+167        self, band_url: str, no_track_number: bool = False, overwrite: bool
 = False
-165    ):
-166        self.band_url = band_url
-167        self.albums = []
-168        for url in self.get_album_urls(band_url):
-169            try:
-170                self.albums.append(AlbumRipper(url, no_track_number,
+168    ):
+169        self.band_url = band_url
+170        self.albums = []
+171        for url in self.get_album_urls(band_url):
+172            try:
+173                self.albums.append(AlbumRipper(url, no_track_number,
 overwrite))
-171            except Exception as e:
-172                print(e)
-173
-174    def get_album_urls(self, band_url: str) -> list[str]:
-175        """Get album urls from the main bandcamp url."""
-176        print(f"Fetching discography from {band_url}...")
-177        response = requests.get(band_url, headers=whosyouragent.get_agent
+174            except Exception as e:
+175                print(e)
+176
+177    def get_album_urls(self, band_url: str) -> list[str]:
+178        """Get album urls from the main bandcamp url."""
+179        print(f"Fetching discography from {band_url}...")
+180        response = requests.get(band_url, headers=whosyouragent.get_agent
 (as_dict=True))
-178        if response.status_code != 200:
-179            raise RuntimeError(
-180                f"Getting {band_url} failed with status code
+181        if response.status_code != 200:
+182            raise RuntimeError(
+183                f"Getting {band_url} failed with status code
 {response.status_code}."
-181            )
-182        soup = BeautifulSoup(response.text, "html.parser")
-183        grid = soup.find("ol", attrs={"id": "music-grid"})
-184        parsed_url = urlparse(band_url)
-185        base_url = f"https://{parsed_url.netloc}"
-186        return [base_url + album.a.get("href") for album in grid.find_all
+184            )
+185        soup = BeautifulSoup(response.text, "html.parser")
+186        grid = soup.find("ol", attrs={"id": "music-grid"})
+187        parsed_url = urlparse(band_url)
+188        base_url = f"https://{parsed_url.netloc}"
+189        return [base_url + album.a.get("href") for album in grid.find_all
 ("li")]
-187
-188    def rip(self):
-189        print(
-190            f"Downloading {len(self.albums)} albums by {self.albums
+190
+191    def rip(self):
+192        print(
+193            f"Downloading {len(self.albums)} albums by {self.albums
 [0].album.artist}."
-191        )
-192        timer = Timer(subsecond_resolution=True)
-193        timer.start()
-194        fails = []
-195        for album in self.albums:
-196            try:
-197                album.rip()
-198            except Exception as e:
-199                fails.append((album, e))
-200        timer.stop()
-201        artist = self.albums[0].album.artist
-202        print(
-203            f"Finished downloading {len(self.albums)} albums by {artist} in
+194        )
+195        timer = Timer(subsecond_resolution=True)
+196        timer.start()
+197        fails = []
+198        for album in self.albums:
+199            try:
+200                album.rip()
+201            except Exception as e:
+202                fails.append((album, e))
+203        timer.stop()
+204        artist = self.albums[0].album.artist
+205        print(
+206            f"Finished downloading {len(self.albums)} albums by {artist} in
 {timer.elapsed_str}."
-204        )
-205        if fails:
-206            print(f"The following downloads failed:")
-207            for fail in fails:
-208                print(f"{fail[0]}: {fail[1]}")
-209
-210
-211def page_is_discography(url: str) -> bool:
-212    """Returns whether the url is to a discography page or not."""
-213    response = requests.get(url, headers=whosyouragent.get_agent
+207        )
+208        if fails:
+209            print(f"The following downloads failed:")
+210            for fail in fails:
+211                print(f"{fail[0]}: {fail[1]}")
+212
+213
+214def page_is_discography(url: str) -> bool:
+215    """Returns whether the url is to a discography page or not."""
+216    response = requests.get(url, headers=whosyouragent.get_agent
 (as_dict=True))
-214    if response.status_code != 200:
-215        raise RuntimeError(
-216            f"Getting {url} failed with status code {response.status_code}."
-217        )
-218    soup = BeautifulSoup(response.text, "html.parser")
-219    # Returns None if it doesn't exist.
-220    grid = soup.find("ol", attrs={"id": "music-grid"})
-221    if grid:
-222        return True
-223    return False
-224
-225
-226def get_args() -> argparse.Namespace:
-227    parser = argparse.ArgumentParser()
+217    if response.status_code != 200:
+218        raise RuntimeError(
+219            f"Getting {url} failed with status code {response.status_code}."
+220        )
+221    soup = BeautifulSoup(response.text, "html.parser")
+222    # Returns None if it doesn't exist.
+223    grid = soup.find("ol", attrs={"id": "music-grid"})
+224    if grid:
+225        return True
+226    return False
+227
 228
-229    parser.add_argument(
-230        "urls",
-231        type=str,
-232        nargs="*",
-233        help=""" The bandcamp url(s) for the album or artist.
-234            If the url is to an artists main page,
-235            all albums will be downloaded.
-236            The tracks will be saved to a subdirectory of
-237            your current directory.
-238            If a track can't be streamed (i.e. private) it
-239            won't be downloaded. Multiple urls can be passed.""",
-240    )
-241
-242    parser.add_argument(
-243        "-n",
-244        "--no_track_number",
-245        action="store_true",
-246        help=""" By default the track number will be added
-247        to the front of the track title. Pass this switch
-248        to disable the behavior.""",
-249    )
-250
-251    parser.add_argument(
-252        "-o",
-253        "--overwrite",
-254        action="store_true",
-255        help=""" Pass this flag to overwrite existing files.
-256        Otherwise don't download tracks that already exist locally.""",
-257    )
-258
-259    args = parser.parse_args()
-260    args.urls = [url.strip("/") for url in args.urls]
+229def get_args() -> argparse.Namespace:
+230    parser = argparse.ArgumentParser()
+231
+232    parser.add_argument(
+233        "urls",
+234        type=str,
+235        nargs="*",
+236        help=""" The bandcamp url(s) for the album or artist.
+237            If the url is to an artists main page,
+238            all albums will be downloaded.
+239            The tracks will be saved to a subdirectory of
+240            your current directory.
+241            If a track can't be streamed (i.e. private) it
+242            won't be downloaded. Multiple urls can be passed.""",
+243    )
+244
+245    parser.add_argument(
+246        "-n",
+247        "--no_track_number",
+248        action="store_true",
+249        help=""" By default the track number will be added
+250        to the front of the track title. Pass this switch
+251        to disable the behavior.""",
+252    )
+253
+254    parser.add_argument(
+255        "-o",
+256        "--overwrite",
+257        action="store_true",
+258        help=""" Pass this flag to overwrite existing files.
+259        Otherwise don't download tracks that already exist locally.""",
+260    )
 261
-262    return args
-263
+262    args = parser.parse_args()
+263    args.urls = [url.strip("/") for url in args.urls]
 264
-265def main(args: argparse.Namespace = None):
-266    if not args:
-267        args = get_args()
-268    for url in args.urls:
-269        if page_is_discography(url):
-270            ripper = BandRipper(url, args.no_track_number, args.overwrite)
-271        else:
-272            ripper = AlbumRipper(url, args.no_track_number, args.overwrite)
-273        ripper.rip()
-274
-275
-276if __name__ == "__main__":
-277    main(get_args())
+265    return args
+266
+267
+268def main(args: argparse.Namespace = None):
+269    if not args:
+270        args = get_args()
+271    for url in args.urls:
+272        if page_is_discography(url):
+273            ripper = BandRipper(url, args.no_track_number, args.overwrite)
+274        else:
+275            ripper = AlbumRipper(url, args.no_track_number, args.overwrite)
+276        ripper.rip()
+277
+278
+279if __name__ == "__main__":
+280    main(get_args())
   ⁰
 def clean_string(text: str) -> str: View Source
 19def clean_string(text: str) -> str:
 20    """Remove punctuation and trailing spaces from text."""
 21    return re.sub(f"[{re.escape(string.punctuation)}]", "", text).strip()
 Remove punctuation and trailing spaces from text.
   ⁰
@@ -455,41 +458,44 @@
 130    def rip(self):
 131        """Download and save the album tracks and album art."""
 132        if len(self.album.tracks) == 0:
 133            print(f"No public tracks available for {self.album}.")
 134            return None
 135        self.make_save_path()
 136        self.download_album_art()
-137        bar = ProgBar(len(self.album.tracks) - 1, width_ratio=0.5)
-138        fails = []
-139        if not self.overwrite:
-140            self.album.tracks = [
-141                track for track in self.album.tracks if not
+137        num_tracks = len(self.album.tracks)
+138        bar = ProgBar(num_tracks, width_ratio=0.5)
+139        fails = []
+140        if not self.overwrite:
+141            self.album.tracks = [
+142                track for track in self.album.tracks if not
 self.track_exists(track)
-142            ]
-143        for track in self.album.tracks:
-144            bar.display(
-145                suffix=f"Downloading {track.title}",
-146                counter_override=1 if len(self.album.tracks) == 1 else None,
-147            )
-148            try:
-149                content = self.get_track_content(track.url)
-150                self.save_track(
-151                    track.title if self.no_track_number else
+143            ]
+144        for i, track in enumerate(self.album.tracks, 1):
+145            bar.display(
+146                suffix=f"Downloading track {i}/{num_tracks}: {track.title}",
+147                counter_override=1 if len(self.album.tracks) == 1 else None,
+148            )
+149            try:
+150                content = self.get_track_content(track.url)
+151                self.save_track(
+152                    track.title if self.no_track_number else
 track.numbered_title,
-152                    content,
-153                )
-154            except Exception as e:
-155                fails.append((track, str(e)))
-156        print(f"Finished downloading {self.album} in
-{bar.timer.elapsed_str}.")
-157        if fails:
-158            print("The following tracks failed to download:")
-159            for fail in fails:
-160                print(f"{fail[0].title}: {fail[1]}")
+153                    content,
+154                )
+155            except Exception as e:
+156                fails.append((track, str(e)))
+157        print(
+158            f"Finished downloading {num_tracks - len(fails)} tracks from
+{self.album} in {bar.timer.elapsed_str}."
+159        )
+160        if fails:
+161            print("The following tracks failed to download:")
+162            for fail in fails:
+163                print(f"{fail[0].title}: {fail[1]}")
 ⁰
 AlbumRipper(
 album_url: str,
 no_track_number: bool = False,
 overwrite: bool = False) View Source
 75    def __init__(
 76        self, album_url: str, no_track_number: bool = False, overwrite: bool
@@ -567,220 +573,223 @@
 130    def rip(self):
 131        """Download and save the album tracks and album art."""
 132        if len(self.album.tracks) == 0:
 133            print(f"No public tracks available for {self.album}.")
 134            return None
 135        self.make_save_path()
 136        self.download_album_art()
-137        bar = ProgBar(len(self.album.tracks) - 1, width_ratio=0.5)
-138        fails = []
-139        if not self.overwrite:
-140            self.album.tracks = [
-141                track for track in self.album.tracks if not
+137        num_tracks = len(self.album.tracks)
+138        bar = ProgBar(num_tracks, width_ratio=0.5)
+139        fails = []
+140        if not self.overwrite:
+141            self.album.tracks = [
+142                track for track in self.album.tracks if not
 self.track_exists(track)
-142            ]
-143        for track in self.album.tracks:
-144            bar.display(
-145                suffix=f"Downloading {track.title}",
-146                counter_override=1 if len(self.album.tracks) == 1 else None,
-147            )
-148            try:
-149                content = self.get_track_content(track.url)
-150                self.save_track(
-151                    track.title if self.no_track_number else
+143            ]
+144        for i, track in enumerate(self.album.tracks, 1):
+145            bar.display(
+146                suffix=f"Downloading track {i}/{num_tracks}: {track.title}",
+147                counter_override=1 if len(self.album.tracks) == 1 else None,
+148            )
+149            try:
+150                content = self.get_track_content(track.url)
+151                self.save_track(
+152                    track.title if self.no_track_number else
 track.numbered_title,
-152                    content,
-153                )
-154            except Exception as e:
-155                fails.append((track, str(e)))
-156        print(f"Finished downloading {self.album} in
-{bar.timer.elapsed_str}.")
-157        if fails:
-158            print("The following tracks failed to download:")
-159            for fail in fails:
-160                print(f"{fail[0].title}: {fail[1]}")
+153                    content,
+154                )
+155            except Exception as e:
+156                fails.append((track, str(e)))
+157        print(
+158            f"Finished downloading {num_tracks - len(fails)} tracks from
+{self.album} in {bar.timer.elapsed_str}."
+159        )
+160        if fails:
+161            print("The following tracks failed to download:")
+162            for fail in fails:
+163                print(f"{fail[0].title}: {fail[1]}")
 Download and save the album tracks and album art.
   ⁰
 class BandRipper: View Source
-163class BandRipper:
-164    def __init__(
-165        self, band_url: str, no_track_number: bool = False, overwrite: bool
+166class BandRipper:
+167    def __init__(
+168        self, band_url: str, no_track_number: bool = False, overwrite: bool
 = False
-166    ):
-167        self.band_url = band_url
-168        self.albums = []
-169        for url in self.get_album_urls(band_url):
-170            try:
-171                self.albums.append(AlbumRipper(url, no_track_number,
+169    ):
+170        self.band_url = band_url
+171        self.albums = []
+172        for url in self.get_album_urls(band_url):
+173            try:
+174                self.albums.append(AlbumRipper(url, no_track_number,
 overwrite))
-172            except Exception as e:
-173                print(e)
-174
-175    def get_album_urls(self, band_url: str) -> list[str]:
-176        """Get album urls from the main bandcamp url."""
-177        print(f"Fetching discography from {band_url}...")
-178        response = requests.get(band_url, headers=whosyouragent.get_agent
+175            except Exception as e:
+176                print(e)
+177
+178    def get_album_urls(self, band_url: str) -> list[str]:
+179        """Get album urls from the main bandcamp url."""
+180        print(f"Fetching discography from {band_url}...")
+181        response = requests.get(band_url, headers=whosyouragent.get_agent
 (as_dict=True))
-179        if response.status_code != 200:
-180            raise RuntimeError(
-181                f"Getting {band_url} failed with status code
+182        if response.status_code != 200:
+183            raise RuntimeError(
+184                f"Getting {band_url} failed with status code
 {response.status_code}."
-182            )
-183        soup = BeautifulSoup(response.text, "html.parser")
-184        grid = soup.find("ol", attrs={"id": "music-grid"})
-185        parsed_url = urlparse(band_url)
-186        base_url = f"https://{parsed_url.netloc}"
-187        return [base_url + album.a.get("href") for album in grid.find_all
+185            )
+186        soup = BeautifulSoup(response.text, "html.parser")
+187        grid = soup.find("ol", attrs={"id": "music-grid"})
+188        parsed_url = urlparse(band_url)
+189        base_url = f"https://{parsed_url.netloc}"
+190        return [base_url + album.a.get("href") for album in grid.find_all
 ("li")]
-188
-189    def rip(self):
-190        print(
-191            f"Downloading {len(self.albums)} albums by {self.albums
+191
+192    def rip(self):
+193        print(
+194            f"Downloading {len(self.albums)} albums by {self.albums
 [0].album.artist}."
-192        )
-193        timer = Timer(subsecond_resolution=True)
-194        timer.start()
-195        fails = []
-196        for album in self.albums:
-197            try:
-198                album.rip()
-199            except Exception as e:
-200                fails.append((album, e))
-201        timer.stop()
-202        artist = self.albums[0].album.artist
-203        print(
-204            f"Finished downloading {len(self.albums)} albums by {artist} in
+195        )
+196        timer = Timer(subsecond_resolution=True)
+197        timer.start()
+198        fails = []
+199        for album in self.albums:
+200            try:
+201                album.rip()
+202            except Exception as e:
+203                fails.append((album, e))
+204        timer.stop()
+205        artist = self.albums[0].album.artist
+206        print(
+207            f"Finished downloading {len(self.albums)} albums by {artist} in
 {timer.elapsed_str}."
-205        )
-206        if fails:
-207            print(f"The following downloads failed:")
-208            for fail in fails:
-209                print(f"{fail[0]}: {fail[1]}")
+208        )
+209        if fails:
+210            print(f"The following downloads failed:")
+211            for fail in fails:
+212                print(f"{fail[0]}: {fail[1]}")
 ⁰
 BandRipper(
 band_url: str,
 no_track_number: bool = False,
 overwrite: bool = False) View Source
-164    def __init__(
-165        self, band_url: str, no_track_number: bool = False, overwrite: bool
+167    def __init__(
+168        self, band_url: str, no_track_number: bool = False, overwrite: bool
 = False
-166    ):
-167        self.band_url = band_url
-168        self.albums = []
-169        for url in self.get_album_urls(band_url):
-170            try:
-171                self.albums.append(AlbumRipper(url, no_track_number,
+169    ):
+170        self.band_url = band_url
+171        self.albums = []
+172        for url in self.get_album_urls(band_url):
+173            try:
+174                self.albums.append(AlbumRipper(url, no_track_number,
 overwrite))
-172            except Exception as e:
-173                print(e)
+175            except Exception as e:
+176                print(e)
 ⁰
 def get_album_urls(self, band_url: str) -> list[str]: View Source
-175    def get_album_urls(self, band_url: str) -> list[str]:
-176        """Get album urls from the main bandcamp url."""
-177        print(f"Fetching discography from {band_url}...")
-178        response = requests.get(band_url, headers=whosyouragent.get_agent
+178    def get_album_urls(self, band_url: str) -> list[str]:
+179        """Get album urls from the main bandcamp url."""
+180        print(f"Fetching discography from {band_url}...")
+181        response = requests.get(band_url, headers=whosyouragent.get_agent
 (as_dict=True))
-179        if response.status_code != 200:
-180            raise RuntimeError(
-181                f"Getting {band_url} failed with status code
+182        if response.status_code != 200:
+183            raise RuntimeError(
+184                f"Getting {band_url} failed with status code
 {response.status_code}."
-182            )
-183        soup = BeautifulSoup(response.text, "html.parser")
-184        grid = soup.find("ol", attrs={"id": "music-grid"})
-185        parsed_url = urlparse(band_url)
-186        base_url = f"https://{parsed_url.netloc}"
-187        return [base_url + album.a.get("href") for album in grid.find_all
+185            )
+186        soup = BeautifulSoup(response.text, "html.parser")
+187        grid = soup.find("ol", attrs={"id": "music-grid"})
+188        parsed_url = urlparse(band_url)
+189        base_url = f"https://{parsed_url.netloc}"
+190        return [base_url + album.a.get("href") for album in grid.find_all
 ("li")]
 Get album urls from the main bandcamp url.
 ⁰
 def rip(self): View Source
-189    def rip(self):
-190        print(
-191            f"Downloading {len(self.albums)} albums by {self.albums
+192    def rip(self):
+193        print(
+194            f"Downloading {len(self.albums)} albums by {self.albums
 [0].album.artist}."
-192        )
-193        timer = Timer(subsecond_resolution=True)
-194        timer.start()
-195        fails = []
-196        for album in self.albums:
-197            try:
-198                album.rip()
-199            except Exception as e:
-200                fails.append((album, e))
-201        timer.stop()
-202        artist = self.albums[0].album.artist
-203        print(
-204            f"Finished downloading {len(self.albums)} albums by {artist} in
+195        )
+196        timer = Timer(subsecond_resolution=True)
+197        timer.start()
+198        fails = []
+199        for album in self.albums:
+200            try:
+201                album.rip()
+202            except Exception as e:
+203                fails.append((album, e))
+204        timer.stop()
+205        artist = self.albums[0].album.artist
+206        print(
+207            f"Finished downloading {len(self.albums)} albums by {artist} in
 {timer.elapsed_str}."
-205        )
-206        if fails:
-207            print(f"The following downloads failed:")
-208            for fail in fails:
-209                print(f"{fail[0]}: {fail[1]}")
+208        )
+209        if fails:
+210            print(f"The following downloads failed:")
+211            for fail in fails:
+212                print(f"{fail[0]}: {fail[1]}")
   ⁰
 def page_is_discography(url: str) -> bool: View Source
-212def page_is_discography(url: str) -> bool:
-213    """Returns whether the url is to a discography page or not."""
-214    response = requests.get(url, headers=whosyouragent.get_agent
+215def page_is_discography(url: str) -> bool:
+216    """Returns whether the url is to a discography page or not."""
+217    response = requests.get(url, headers=whosyouragent.get_agent
 (as_dict=True))
-215    if response.status_code != 200:
-216        raise RuntimeError(
-217            f"Getting {url} failed with status code {response.status_code}."
-218        )
-219    soup = BeautifulSoup(response.text, "html.parser")
-220    # Returns None if it doesn't exist.
-221    grid = soup.find("ol", attrs={"id": "music-grid"})
-222    if grid:
-223        return True
-224    return False
+218    if response.status_code != 200:
+219        raise RuntimeError(
+220            f"Getting {url} failed with status code {response.status_code}."
+221        )
+222    soup = BeautifulSoup(response.text, "html.parser")
+223    # Returns None if it doesn't exist.
+224    grid = soup.find("ol", attrs={"id": "music-grid"})
+225    if grid:
+226        return True
+227    return False
 Returns whether the url is to a discography page or not.
   ⁰
 def get_args() -> argparse.Namespace: View Source
-227def get_args() -> argparse.Namespace:
-228    parser = argparse.ArgumentParser()
-229
-230    parser.add_argument(
-231        "urls",
-232        type=str,
-233        nargs="*",
-234        help=""" The bandcamp url(s) for the album or artist.
-235            If the url is to an artists main page,
-236            all albums will be downloaded.
-237            The tracks will be saved to a subdirectory of
-238            your current directory.
-239            If a track can't be streamed (i.e. private) it
-240            won't be downloaded. Multiple urls can be passed.""",
-241    )
-242
-243    parser.add_argument(
-244        "-n",
-245        "--no_track_number",
-246        action="store_true",
-247        help=""" By default the track number will be added
-248        to the front of the track title. Pass this switch
-249        to disable the behavior.""",
-250    )
-251
-252    parser.add_argument(
-253        "-o",
-254        "--overwrite",
-255        action="store_true",
-256        help=""" Pass this flag to overwrite existing files.
-257        Otherwise don't download tracks that already exist locally.""",
-258    )
-259
-260    args = parser.parse_args()
-261    args.urls = [url.strip("/") for url in args.urls]
+230def get_args() -> argparse.Namespace:
+231    parser = argparse.ArgumentParser()
+232
+233    parser.add_argument(
+234        "urls",
+235        type=str,
+236        nargs="*",
+237        help=""" The bandcamp url(s) for the album or artist.
+238            If the url is to an artists main page,
+239            all albums will be downloaded.
+240            The tracks will be saved to a subdirectory of
+241            your current directory.
+242            If a track can't be streamed (i.e. private) it
+243            won't be downloaded. Multiple urls can be passed.""",
+244    )
+245
+246    parser.add_argument(
+247        "-n",
+248        "--no_track_number",
+249        action="store_true",
+250        help=""" By default the track number will be added
+251        to the front of the track title. Pass this switch
+252        to disable the behavior.""",
+253    )
+254
+255    parser.add_argument(
+256        "-o",
+257        "--overwrite",
+258        action="store_true",
+259        help=""" Pass this flag to overwrite existing files.
+260        Otherwise don't download tracks that already exist locally.""",
+261    )
 262
-263    return args
+263    args = parser.parse_args()
+264    args.urls = [url.strip("/") for url in args.urls]
+265
+266    return args
   ⁰
 def main(args: argparse.Namespace = None): View Source
-266def main(args: argparse.Namespace = None):
-267    if not args:
-268        args = get_args()
-269    for url in args.urls:
-270        if page_is_discography(url):
-271            ripper = BandRipper(url, args.no_track_number, args.overwrite)
-272        else:
-273            ripper = AlbumRipper(url, args.no_track_number, args.overwrite)
-274        ripper.rip()
+269def main(args: argparse.Namespace = None):
+270    if not args:
+271        args = get_args()
+272    for url in args.urls:
+273        if page_is_discography(url):
+274            ripper = BandRipper(url, args.no_track_number, args.overwrite)
+275        else:
+276            ripper = AlbumRipper(url, args.no_track_number, args.overwrite)
+277        ripper.rip()
```

### Comparing `bandripper-0.1.5/src/bandripper/bandripper.py` & `bandripper-0.1.6/src/bandripper/bandripper.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,34 +129,37 @@
     def rip(self):
         """Download and save the album tracks and album art."""
         if len(self.album.tracks) == 0:
             print(f"No public tracks available for {self.album}.")
             return None
         self.make_save_path()
         self.download_album_art()
-        bar = ProgBar(len(self.album.tracks) - 1, width_ratio=0.5)
+        num_tracks = len(self.album.tracks)
+        bar = ProgBar(num_tracks, width_ratio=0.5)
         fails = []
         if not self.overwrite:
             self.album.tracks = [
                 track for track in self.album.tracks if not self.track_exists(track)
             ]
-        for track in self.album.tracks:
+        for i, track in enumerate(self.album.tracks, 1):
             bar.display(
-                suffix=f"Downloading {track.title}",
+                suffix=f"Downloading track {i}/{num_tracks}: {track.title}",
                 counter_override=1 if len(self.album.tracks) == 1 else None,
             )
             try:
                 content = self.get_track_content(track.url)
                 self.save_track(
                     track.title if self.no_track_number else track.numbered_title,
                     content,
                 )
             except Exception as e:
                 fails.append((track, str(e)))
-        print(f"Finished downloading {self.album} in {bar.timer.elapsed_str}.")
+        print(
+            f"Finished downloading {num_tracks - len(fails)} tracks from {self.album} in {bar.timer.elapsed_str}."
+        )
         if fails:
             print("The following tracks failed to download:")
             for fail in fails:
                 print(f"{fail[0].title}: {fail[1]}")
 
 
 class BandRipper:
```

### Comparing `bandripper-0.1.5/LICENSE.txt` & `bandripper-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bandripper-0.1.5/README.md` & `bandripper-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `bandripper-0.1.5/pyproject.toml` & `bandripper-0.1.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 00000030: 6261 636b 656e 6420 3d20 2268 6174 6368  backend = "hatch
 00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 6261 6e64 7269 7070 6572 220d 0a64   "bandripper"..d
 00000070: 6573 6372 6970 7469 6f6e 203d 2022 5269  escription = "Ri
 00000080: 7020 6d70 3373 2066 726f 6d20 6261 6e64  p mp3s from band
 00000090: 6361 6d70 2e22 0d0a 7665 7273 696f 6e20  camp."..version 
-000000a0: 3d20 2230 2e31 2e35 220d 0a72 6571 7569  = "0.1.5"..requi
+000000a0: 3d20 2230 2e31 2e36 220d 0a72 6571 7569  = "0.1.6"..requi
 000000b0: 7265 732d 7079 7468 6f6e 203d 2022 3e3d  res-python = ">=
 000000c0: 332e 3922 0d0a 6465 7065 6e64 656e 6369  3.9"..dependenci
 000000d0: 6573 203d 205b 2272 6571 7565 7374 7322  es = ["requests"
 000000e0: 2c20 2262 7334 222c 2022 7768 6f73 796f  , "bs4", "whosyo
 000000f0: 7572 6167 656e 7422 2c20 226e 6f69 6674  uragent", "noift
 00000100: 696d 6572 222c 2022 7072 696e 7462 7564  imer", "printbud
 00000110: 6469 6573 222c 2022 7079 7465 7374 225d  dies", "pytest"]
```

### Comparing `bandripper-0.1.5/PKG-INFO` & `bandripper-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bandripper
-Version: 0.1.5
+Version: 0.1.6
 Summary: Rip mp3s from bandcamp.
 Project-URL: Homepage, https://github.com/matt-manes/bandripper
 Project-URL: Documentation, https://github.com/matt-manes/bandripper/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/bandripper/tree/main/src/bandripper
 Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
 Keywords: audio,bandcamp,download,downloader,music
```

