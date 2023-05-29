# Comparing `tmp/parsetypes-0.2.4.tar.gz` & `tmp/parsetypes-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsetypes-0.2.4.tar", last modified: Sun May 28 23:01:21 2023, max compression
+gzip compressed data, was "parsetypes-0.2.5.tar", last modified: Mon May 29 03:58:43 2023, max compression
```

## Comparing `parsetypes-0.2.4.tar` & `parsetypes-0.2.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 23:01:21.080304 parsetypes-0.2.4/
--rw-rw-rw-   0        0        0      863 2023-05-28 23:00:42.000000 parsetypes-0.2.4/CHANGELOG.md
--rw-rw-rw-   0        0        0       22 2023-05-28 02:54:36.000000 parsetypes-0.2.4/MANIFEST.in
--rw-rw-rw-   0        0        0     6751 2023-05-28 23:01:21.080304 parsetypes-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     4183 2023-05-28 23:00:42.000000 parsetypes-0.2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 23:01:21.066302 parsetypes-0.2.4/docs/
-drwxrwxrwx   0        0        0        0 2023-05-28 23:01:21.072307 parsetypes-0.2.4/docs/html/
--rw-rw-rw-   0        0        0     1729 2023-05-28 23:01:12.000000 parsetypes-0.2.4/docs/html/favicon.png
--rw-rw-rw-   0        0        0      141 2023-05-28 23:01:11.000000 parsetypes-0.2.4/docs/html/index.html
--rw-rw-rw-   0        0        0   529187 2023-05-28 23:01:11.000000 parsetypes-0.2.4/docs/html/parsetypes.html
--rw-rw-rw-   0        0        0   217429 2023-05-28 23:01:12.000000 parsetypes-0.2.4/docs/html/search.js
--rw-rw-rw-   0        0        0     2297 2023-05-28 04:48:55.000000 parsetypes-0.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-28 23:01:21.081303 parsetypes-0.2.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-28 23:01:21.067305 parsetypes-0.2.4/src/
-drwxrwxrwx   0        0        0        0 2023-05-28 23:01:21.075305 parsetypes-0.2.4/src/parsetypes/
--rw-rw-rw-   0        0        0      621 2023-05-28 23:00:42.000000 parsetypes-0.2.4/src/parsetypes/__init__.py
--rw-rw-rw-   0        0        0     1254 2023-05-28 05:37:03.000000 parsetypes-0.2.4/src/parsetypes/_common.py
--rw-rw-rw-   0        0        0      348 2023-05-28 04:48:55.000000 parsetypes-0.2.4/src/parsetypes/_compat.py
--rw-rw-rw-   0        0        0    35474 2023-05-28 23:00:42.000000 parsetypes-0.2.4/src/parsetypes/_parser.py
--rw-rw-rw-   0        0        0     5203 2023-05-28 05:32:22.000000 parsetypes-0.2.4/src/parsetypes/_reduce_types.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:01:21.078306 parsetypes-0.2.4/src/parsetypes.egg-info/
--rw-rw-rw-   0        0        0     6751 2023-05-28 23:01:21.000000 parsetypes-0.2.4/src/parsetypes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      512 2023-05-28 23:01:21.000000 parsetypes-0.2.4/src/parsetypes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 23:01:21.000000 parsetypes-0.2.4/src/parsetypes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      296 2023-05-28 23:01:21.000000 parsetypes-0.2.4/src/parsetypes.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-28 23:01:21.000000 parsetypes-0.2.4/src/parsetypes.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-28 23:01:21.079304 parsetypes-0.2.4/tests/
--rw-rw-rw-   0        0        0    67890 2023-05-28 23:00:42.000000 parsetypes-0.2.4/tests/test_parser.py
--rw-rw-rw-   0        0        0     8837 2023-05-28 04:48:55.000000 parsetypes-0.2.4/tests/test_reduce_types.py
+drwxrwxrwx   0        0        0        0 2023-05-29 03:58:43.700784 parsetypes-0.2.5/
+-rw-rw-rw-   0        0        0      898 2023-05-29 03:57:56.000000 parsetypes-0.2.5/CHANGELOG.md
+-rw-rw-rw-   0        0        0       22 2023-05-28 02:54:36.000000 parsetypes-0.2.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     6786 2023-05-29 03:58:43.700784 parsetypes-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4183 2023-05-28 23:00:42.000000 parsetypes-0.2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 03:58:43.683601 parsetypes-0.2.5/docs/
+drwxrwxrwx   0        0        0        0 2023-05-29 03:58:43.691800 parsetypes-0.2.5/docs/html/
+-rw-rw-rw-   0        0        0     1729 2023-05-29 03:58:34.000000 parsetypes-0.2.5/docs/html/favicon.png
+-rw-rw-rw-   0        0        0      141 2023-05-29 03:58:34.000000 parsetypes-0.2.5/docs/html/index.html
+-rw-rw-rw-   0        0        0   529234 2023-05-29 03:58:34.000000 parsetypes-0.2.5/docs/html/parsetypes.html
+-rw-rw-rw-   0        0        0   217649 2023-05-29 03:58:34.000000 parsetypes-0.2.5/docs/html/search.js
+-rw-rw-rw-   0        0        0     2297 2023-05-28 04:48:55.000000 parsetypes-0.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-29 03:58:43.700784 parsetypes-0.2.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-29 03:58:43.684594 parsetypes-0.2.5/src/
+drwxrwxrwx   0        0        0        0 2023-05-29 03:58:43.694786 parsetypes-0.2.5/src/parsetypes/
+-rw-rw-rw-   0        0        0      621 2023-05-29 03:58:00.000000 parsetypes-0.2.5/src/parsetypes/__init__.py
+-rw-rw-rw-   0        0        0     1254 2023-05-28 05:37:03.000000 parsetypes-0.2.5/src/parsetypes/_common.py
+-rw-rw-rw-   0        0        0      348 2023-05-28 04:48:55.000000 parsetypes-0.2.5/src/parsetypes/_compat.py
+-rw-rw-rw-   0        0        0    35499 2023-05-29 03:56:49.000000 parsetypes-0.2.5/src/parsetypes/_parser.py
+-rw-rw-rw-   0        0        0     5203 2023-05-28 05:32:22.000000 parsetypes-0.2.5/src/parsetypes/_reduce_types.py
+drwxrwxrwx   0        0        0        0 2023-05-29 03:58:43.697786 parsetypes-0.2.5/src/parsetypes.egg-info/
+-rw-rw-rw-   0        0        0     6786 2023-05-29 03:58:43.000000 parsetypes-0.2.5/src/parsetypes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2023-05-29 03:58:43.000000 parsetypes-0.2.5/src/parsetypes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 03:58:43.000000 parsetypes-0.2.5/src/parsetypes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      296 2023-05-29 03:58:43.000000 parsetypes-0.2.5/src/parsetypes.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-29 03:58:43.000000 parsetypes-0.2.5/src/parsetypes.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-29 03:58:43.698786 parsetypes-0.2.5/tests/
+-rw-rw-rw-   0        0        0    67890 2023-05-28 23:00:42.000000 parsetypes-0.2.5/tests/test_parser.py
+-rw-rw-rw-   0        0        0     8837 2023-05-28 04:48:55.000000 parsetypes-0.2.5/tests/test_reduce_types.py
```

### Comparing `parsetypes-0.2.4/PKG-INFO` & `parsetypes-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsetypes
-Version: 0.2.4
+Version: 0.2.5
 Summary: Parse serialised data to recover their original underlying types
 Author-email: Yu Shiyang <yu.shiyang@gnayihs.uy>
 License: MPL-2.0
 Project-URL: Homepage, https://github.com/yushiyangk/parsetypes
 Project-URL: Documentation, https://parsetypes.gnayihs.uy/
 Project-URL: Issues, https://github.com/yushiyangk/parsetypes/issues
 Keywords: python,str,string,types,conversion
@@ -158,19 +158,23 @@
 
 ## Changelog
 
 This project follows [PEP 440](https://peps.python.org/pep-0440/) and [Semantic Versioning (SemVer)](https://semver.org/spec/v2.0.0.html). In addition to the guarantees specified by SemVer, for versions before 1.0, this project guarantees backwards compatibility of the API for patch version updates (0.<var>y</var>.<b><var>z</var></b>).
 
 The recommended version specifier is <code>parsetypes ~= <var>x</var>.<var>y</var></code> for version 1.0 and later, and <code>parsetypes ~= <var>0</var>.<var>y</var>.<var>z</var></code> for versions prior to 1.0.
 
+### 0.2.5
+
+- Fixed documentation
+
 ### 0.2.4
 
 - Added <code><var>parser</var>.convert()</code>
 
-### 0.2.1, 0.2.2 and 0.2.3
+### 0.2.1, 0.2.2, 0.2.3
 
 - Fixed documentation
 
 ### 0.2
 
 - Added support for Python version 3.9; previously only 3.10 and 3.11 were supported
```

### Comparing `parsetypes-0.2.4/README.md` & `parsetypes-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `parsetypes-0.2.4/docs/html/favicon.png` & `parsetypes-0.2.5/docs/html/favicon.png`

 * *Files identical despite different names*

### Comparing `parsetypes-0.2.4/docs/html/parsetypes.html` & `parsetypes-0.2.5/docs/html/parsetypes.html`

 * *Files 0% similar despite different names*

```diff
@@ -204,15 +204,15 @@
 </span><span id="L-4"><a href="#L-4"><span class="linenos"> 4</span></a><span class="sd">	The `TypeParser` class provides configurable type inference and parsing. This can be initialised with different settings to, for example:</span>
 </span><span id="L-5"><a href="#L-5"><span class="linenos"> 5</span></a><span class="sd">	- treat `inf` as either a float or a normal string</span>
 </span><span id="L-6"><a href="#L-6"><span class="linenos"> 6</span></a><span class="sd">	- give exact Decimal values instead of floats</span>
 </span><span id="L-7"><a href="#L-7"><span class="linenos"> 7</span></a><span class="sd">	- detect inline lists</span>
 </span><span id="L-8"><a href="#L-8"><span class="linenos"> 8</span></a><span class="sd">&quot;&quot;&quot;</span>
 </span><span id="L-9"><a href="#L-9"><span class="linenos"> 9</span></a>
 </span><span id="L-10"><a href="#L-10"><span class="linenos">10</span></a>
-</span><span id="L-11"><a href="#L-11"><span class="linenos">11</span></a><span class="n">__version__</span> <span class="o">=</span> <span class="s2">&quot;0.2.4&quot;</span>
+</span><span id="L-11"><a href="#L-11"><span class="linenos">11</span></a><span class="n">__version__</span> <span class="o">=</span> <span class="s2">&quot;0.2.5&quot;</span>
 </span><span id="L-12"><a href="#L-12"><span class="linenos">12</span></a>
 </span><span id="L-13"><a href="#L-13"><span class="linenos">13</span></a><span class="kn">from</span> <span class="nn">._common</span> <span class="kn">import</span> <span class="n">AnyScalar</span><span class="p">,</span> <span class="n">AnyScalarType</span><span class="p">,</span> <span class="n">AnyValue</span><span class="p">,</span> <span class="n">AnyValueType</span><span class="p">,</span> <span class="n">GenericValue</span><span class="p">,</span> <span class="n">Nullable</span>
 </span><span id="L-14"><a href="#L-14"><span class="linenos">14</span></a><span class="kn">from</span> <span class="nn">._parser</span> <span class="kn">import</span> <span class="n">TypeParser</span>
 </span><span id="L-15"><a href="#L-15"><span class="linenos">15</span></a><span class="kn">from</span> <span class="nn">._reduce_types</span> <span class="kn">import</span> <span class="n">reduce_types</span>
 </span><span id="L-16"><a href="#L-16"><span class="linenos">16</span></a>
 </span><span id="L-17"><a href="#L-17"><span class="linenos">17</span></a><span class="n">__all__</span> <span class="o">=</span> <span class="p">(</span><span class="s1">&#39;TypeParser&#39;</span><span class="p">,</span> <span class="s1">&#39;reduce_types&#39;</span><span class="p">)</span>
 </span></pre></div>
@@ -461,31 +461,31 @@
 </span><span id="TypeParser-287"><a href="#TypeParser-287"><span class="linenos"> 287</span></a>			<span class="k">return</span> <span class="kc">True</span>
 </span><span id="TypeParser-288"><a href="#TypeParser-288"><span class="linenos"> 288</span></a>		<span class="k">if</span> <span class="n">value</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">false_values</span><span class="p">:</span>
 </span><span id="TypeParser-289"><a href="#TypeParser-289"><span class="linenos"> 289</span></a>			<span class="k">return</span> <span class="kc">True</span>
 </span><span id="TypeParser-290"><a href="#TypeParser-290"><span class="linenos"> 290</span></a>
 </span><span id="TypeParser-291"><a href="#TypeParser-291"><span class="linenos"> 291</span></a>		<span class="k">return</span> <span class="kc">False</span>
 </span><span id="TypeParser-292"><a href="#TypeParser-292"><span class="linenos"> 292</span></a>
 </span><span id="TypeParser-293"><a href="#TypeParser-293"><span class="linenos"> 293</span></a>
-</span><span id="TypeParser-294"><a href="#TypeParser-294"><span class="linenos"> 294</span></a>	<span class="k">def</span> <span class="nf">is_int</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="o">*</span><span class="p">,</span> <span class="n">allow_sign</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_negative</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="TypeParser-294"><a href="#TypeParser-294"><span class="linenos"> 294</span></a>	<span class="k">def</span> <span class="nf">is_int</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="o">*</span><span class="p">,</span> <span class="n">allow_negative</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_sign</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
 </span><span id="TypeParser-295"><a href="#TypeParser-295"><span class="linenos"> 295</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
 </span><span id="TypeParser-296"><a href="#TypeParser-296"><span class="linenos"> 296</span></a><span class="sd">			Check if a string represents an int</span>
 </span><span id="TypeParser-297"><a href="#TypeParser-297"><span class="linenos"> 297</span></a>
 </span><span id="TypeParser-298"><a href="#TypeParser-298"><span class="linenos"> 298</span></a><span class="sd">			Parameters</span>
 </span><span id="TypeParser-299"><a href="#TypeParser-299"><span class="linenos"> 299</span></a><span class="sd">			----------</span>
 </span><span id="TypeParser-300"><a href="#TypeParser-300"><span class="linenos"> 300</span></a><span class="sd">			`value`</span>
 </span><span id="TypeParser-301"><a href="#TypeParser-301"><span class="linenos"> 301</span></a><span class="sd">			: string to be checked</span>
 </span><span id="TypeParser-302"><a href="#TypeParser-302"><span class="linenos"> 302</span></a>
 </span><span id="TypeParser-303"><a href="#TypeParser-303"><span class="linenos"> 303</span></a><span class="sd">			`allow_negative`</span>
 </span><span id="TypeParser-304"><a href="#TypeParser-304"><span class="linenos"> 304</span></a><span class="sd">			: whether to accept negative values</span>
 </span><span id="TypeParser-305"><a href="#TypeParser-305"><span class="linenos"> 305</span></a>
 </span><span id="TypeParser-306"><a href="#TypeParser-306"><span class="linenos"> 306</span></a><span class="sd">			`allow_sign`</span>
-</span><span id="TypeParser-307"><a href="#TypeParser-307"><span class="linenos"> 307</span></a><span class="sd">			: whether to accept signed values. If False, it implies that `allow_negative` is False also.</span>
+</span><span id="TypeParser-307"><a href="#TypeParser-307"><span class="linenos"> 307</span></a><span class="sd">			: whether to accept values prepended with a sign character. If False, it implies that `allow_negative` is False also.</span>
 </span><span id="TypeParser-308"><a href="#TypeParser-308"><span class="linenos"> 308</span></a>
 </span><span id="TypeParser-309"><a href="#TypeParser-309"><span class="linenos"> 309</span></a><span class="sd">			`allow_scientific`</span>
-</span><span id="TypeParser-310"><a href="#TypeParser-310"><span class="linenos"> 310</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form &lt;code&gt;&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;&lt;/code&gt; will be interpreted as the expression &lt;code&gt;&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)&lt;/code&gt;, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note &lt;var&gt;M&lt;/var&gt; *must* be an integer and &lt;var&gt;X&lt;/var&gt; *must* be a non-negative integer, even in cases where the above expression evaluates mathematically to an integer.</span>
+</span><span id="TypeParser-310"><a href="#TypeParser-310"><span class="linenos"> 310</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form &lt;code&gt;&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;&lt;/code&gt; will be interpreted as the expression &lt;code&gt;&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)&lt;/code&gt;, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note that &lt;var&gt;M&lt;/var&gt; must be an integer and &lt;var&gt;X&lt;/var&gt; must be a non-negative integer, even in cases where the expression would evaluate mathematically to an integer.</span>
 </span><span id="TypeParser-311"><a href="#TypeParser-311"><span class="linenos"> 311</span></a>
 </span><span id="TypeParser-312"><a href="#TypeParser-312"><span class="linenos"> 312</span></a><span class="sd">			Returns</span>
 </span><span id="TypeParser-313"><a href="#TypeParser-313"><span class="linenos"> 313</span></a><span class="sd">			-------</span>
 </span><span id="TypeParser-314"><a href="#TypeParser-314"><span class="linenos"> 314</span></a><span class="sd">			whether it is an int</span>
 </span><span id="TypeParser-315"><a href="#TypeParser-315"><span class="linenos"> 315</span></a>
 </span><span id="TypeParser-316"><a href="#TypeParser-316"><span class="linenos"> 316</span></a><span class="sd">			Examples</span>
 </span><span id="TypeParser-317"><a href="#TypeParser-317"><span class="linenos"> 317</span></a><span class="sd">			--------</span>
@@ -698,15 +698,15 @@
 </span><span id="TypeParser-524"><a href="#TypeParser-524"><span class="linenos"> 524</span></a>
 </span><span id="TypeParser-525"><a href="#TypeParser-525"><span class="linenos"> 525</span></a><span class="sd">			Parameters</span>
 </span><span id="TypeParser-526"><a href="#TypeParser-526"><span class="linenos"> 526</span></a><span class="sd">			----------</span>
 </span><span id="TypeParser-527"><a href="#TypeParser-527"><span class="linenos"> 527</span></a><span class="sd">			`value`</span>
 </span><span id="TypeParser-528"><a href="#TypeParser-528"><span class="linenos"> 528</span></a><span class="sd">			: string to be parsed</span>
 </span><span id="TypeParser-529"><a href="#TypeParser-529"><span class="linenos"> 529</span></a>
 </span><span id="TypeParser-530"><a href="#TypeParser-530"><span class="linenos"> 530</span></a><span class="sd">			`allow_scientific`</span>
-</span><span id="TypeParser-531"><a href="#TypeParser-531"><span class="linenos"> 531</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form &lt;code&gt;&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;&lt;/code&gt; will be interpreted as the expression &lt;code&gt;&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)&lt;/code&gt;, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note &lt;var&gt;M&lt;/var&gt; *must* be an integer and &lt;var&gt;X&lt;/var&gt; *must* be a non-negative integer, even in cases where the above expression evaluates mathematically to an integer.</span>
+</span><span id="TypeParser-531"><a href="#TypeParser-531"><span class="linenos"> 531</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form &lt;code&gt;&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;&lt;/code&gt; will be interpreted as the expression &lt;code&gt;&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)&lt;/code&gt;, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note that &lt;var&gt;M&lt;/var&gt; must be an integer and &lt;var&gt;X&lt;/var&gt; must be a non-negative integer, even in cases where the expression would evaluate mathematically to an integer.</span>
 </span><span id="TypeParser-532"><a href="#TypeParser-532"><span class="linenos"> 532</span></a>
 </span><span id="TypeParser-533"><a href="#TypeParser-533"><span class="linenos"> 533</span></a><span class="sd">			Returns</span>
 </span><span id="TypeParser-534"><a href="#TypeParser-534"><span class="linenos"> 534</span></a><span class="sd">			-------</span>
 </span><span id="TypeParser-535"><a href="#TypeParser-535"><span class="linenos"> 535</span></a><span class="sd">			parsed int value</span>
 </span><span id="TypeParser-536"><a href="#TypeParser-536"><span class="linenos"> 536</span></a>
 </span><span id="TypeParser-537"><a href="#TypeParser-537"><span class="linenos"> 537</span></a><span class="sd">			Raises</span>
 </span><span id="TypeParser-538"><a href="#TypeParser-538"><span class="linenos"> 538</span></a><span class="sd">			------</span>
@@ -1583,38 +1583,38 @@
 
                             </div>
                             <div id="TypeParser.is_int" class="classattr">
                                         <input id="TypeParser.is_int-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">is_int</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">value</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="o">*</span>,</span><span class="param">	<span class="n">allow_sign</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>,</span><span class="param">	<span class="n">allow_negative</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>,</span><span class="param">	<span class="n">allow_scientific</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">) -> <span class="nb">bool</span>:</span></span>
+        <span class="name">is_int</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">value</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="o">*</span>,</span><span class="param">	<span class="n">allow_negative</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>,</span><span class="param">	<span class="n">allow_sign</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>,</span><span class="param">	<span class="n">allow_scientific</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">) -> <span class="nb">bool</span>:</span></span>
 
 
                 <label class="view-source-button" for="TypeParser.is_int-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#TypeParser.is_int"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.is_int-294"><a href="#TypeParser.is_int-294"><span class="linenos">294</span></a>	<span class="k">def</span> <span class="nf">is_int</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="o">*</span><span class="p">,</span> <span class="n">allow_sign</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_negative</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.is_int-294"><a href="#TypeParser.is_int-294"><span class="linenos">294</span></a>	<span class="k">def</span> <span class="nf">is_int</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="o">*</span><span class="p">,</span> <span class="n">allow_negative</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_sign</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
 </span><span id="TypeParser.is_int-295"><a href="#TypeParser.is_int-295"><span class="linenos">295</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
 </span><span id="TypeParser.is_int-296"><a href="#TypeParser.is_int-296"><span class="linenos">296</span></a><span class="sd">			Check if a string represents an int</span>
 </span><span id="TypeParser.is_int-297"><a href="#TypeParser.is_int-297"><span class="linenos">297</span></a>
 </span><span id="TypeParser.is_int-298"><a href="#TypeParser.is_int-298"><span class="linenos">298</span></a><span class="sd">			Parameters</span>
 </span><span id="TypeParser.is_int-299"><a href="#TypeParser.is_int-299"><span class="linenos">299</span></a><span class="sd">			----------</span>
 </span><span id="TypeParser.is_int-300"><a href="#TypeParser.is_int-300"><span class="linenos">300</span></a><span class="sd">			`value`</span>
 </span><span id="TypeParser.is_int-301"><a href="#TypeParser.is_int-301"><span class="linenos">301</span></a><span class="sd">			: string to be checked</span>
 </span><span id="TypeParser.is_int-302"><a href="#TypeParser.is_int-302"><span class="linenos">302</span></a>
 </span><span id="TypeParser.is_int-303"><a href="#TypeParser.is_int-303"><span class="linenos">303</span></a><span class="sd">			`allow_negative`</span>
 </span><span id="TypeParser.is_int-304"><a href="#TypeParser.is_int-304"><span class="linenos">304</span></a><span class="sd">			: whether to accept negative values</span>
 </span><span id="TypeParser.is_int-305"><a href="#TypeParser.is_int-305"><span class="linenos">305</span></a>
 </span><span id="TypeParser.is_int-306"><a href="#TypeParser.is_int-306"><span class="linenos">306</span></a><span class="sd">			`allow_sign`</span>
-</span><span id="TypeParser.is_int-307"><a href="#TypeParser.is_int-307"><span class="linenos">307</span></a><span class="sd">			: whether to accept signed values. If False, it implies that `allow_negative` is False also.</span>
+</span><span id="TypeParser.is_int-307"><a href="#TypeParser.is_int-307"><span class="linenos">307</span></a><span class="sd">			: whether to accept values prepended with a sign character. If False, it implies that `allow_negative` is False also.</span>
 </span><span id="TypeParser.is_int-308"><a href="#TypeParser.is_int-308"><span class="linenos">308</span></a>
 </span><span id="TypeParser.is_int-309"><a href="#TypeParser.is_int-309"><span class="linenos">309</span></a><span class="sd">			`allow_scientific`</span>
-</span><span id="TypeParser.is_int-310"><a href="#TypeParser.is_int-310"><span class="linenos">310</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form &lt;code&gt;&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;&lt;/code&gt; will be interpreted as the expression &lt;code&gt;&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)&lt;/code&gt;, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note &lt;var&gt;M&lt;/var&gt; *must* be an integer and &lt;var&gt;X&lt;/var&gt; *must* be a non-negative integer, even in cases where the above expression evaluates mathematically to an integer.</span>
+</span><span id="TypeParser.is_int-310"><a href="#TypeParser.is_int-310"><span class="linenos">310</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form &lt;code&gt;&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;&lt;/code&gt; will be interpreted as the expression &lt;code&gt;&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)&lt;/code&gt;, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note that &lt;var&gt;M&lt;/var&gt; must be an integer and &lt;var&gt;X&lt;/var&gt; must be a non-negative integer, even in cases where the expression would evaluate mathematically to an integer.</span>
 </span><span id="TypeParser.is_int-311"><a href="#TypeParser.is_int-311"><span class="linenos">311</span></a>
 </span><span id="TypeParser.is_int-312"><a href="#TypeParser.is_int-312"><span class="linenos">312</span></a><span class="sd">			Returns</span>
 </span><span id="TypeParser.is_int-313"><a href="#TypeParser.is_int-313"><span class="linenos">313</span></a><span class="sd">			-------</span>
 </span><span id="TypeParser.is_int-314"><a href="#TypeParser.is_int-314"><span class="linenos">314</span></a><span class="sd">			whether it is an int</span>
 </span><span id="TypeParser.is_int-315"><a href="#TypeParser.is_int-315"><span class="linenos">315</span></a>
 </span><span id="TypeParser.is_int-316"><a href="#TypeParser.is_int-316"><span class="linenos">316</span></a><span class="sd">			Examples</span>
 </span><span id="TypeParser.is_int-317"><a href="#TypeParser.is_int-317"><span class="linenos">317</span></a><span class="sd">			--------</span>
@@ -1674,18 +1674,18 @@
 <p><code>value</code>
 : string to be checked</p>
 
 <p><code>allow_negative</code>
 : whether to accept negative values</p>
 
 <p><code>allow_sign</code>
-: whether to accept signed values. If False, it implies that <code>allow_negative</code> is False also.</p>
+: whether to accept values prepended with a sign character. If False, it implies that <code>allow_negative</code> is False also.</p>
 
 <p><code>allow_scientific</code>
-: whether to accept scientific notation. If True, strings of the form <code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression <code><var>M</var> * (10 <em>* <var>X</var>)</code>, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note <var>M</var> *must</em> be an integer and <var>X</var> <em>must</em> be a non-negative integer, even in cases where the above expression evaluates mathematically to an integer.</p>
+: whether to accept scientific notation. If True, strings of the form <code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression <code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note that <var>M</var> must be an integer and <var>X</var> must be a non-negative integer, even in cases where the expression would evaluate mathematically to an integer.</p>
 
 <h2 id="returns">Returns</h2>
 
 <p>whether it is an int</p>
 
 <h2 id="examples">Examples</h2>
 
@@ -2032,15 +2032,15 @@
 </span><span id="TypeParser.parse_int-524"><a href="#TypeParser.parse_int-524"><span class="linenos">524</span></a>
 </span><span id="TypeParser.parse_int-525"><a href="#TypeParser.parse_int-525"><span class="linenos">525</span></a><span class="sd">			Parameters</span>
 </span><span id="TypeParser.parse_int-526"><a href="#TypeParser.parse_int-526"><span class="linenos">526</span></a><span class="sd">			----------</span>
 </span><span id="TypeParser.parse_int-527"><a href="#TypeParser.parse_int-527"><span class="linenos">527</span></a><span class="sd">			`value`</span>
 </span><span id="TypeParser.parse_int-528"><a href="#TypeParser.parse_int-528"><span class="linenos">528</span></a><span class="sd">			: string to be parsed</span>
 </span><span id="TypeParser.parse_int-529"><a href="#TypeParser.parse_int-529"><span class="linenos">529</span></a>
 </span><span id="TypeParser.parse_int-530"><a href="#TypeParser.parse_int-530"><span class="linenos">530</span></a><span class="sd">			`allow_scientific`</span>
-</span><span id="TypeParser.parse_int-531"><a href="#TypeParser.parse_int-531"><span class="linenos">531</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form &lt;code&gt;&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;&lt;/code&gt; will be interpreted as the expression &lt;code&gt;&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)&lt;/code&gt;, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note &lt;var&gt;M&lt;/var&gt; *must* be an integer and &lt;var&gt;X&lt;/var&gt; *must* be a non-negative integer, even in cases where the above expression evaluates mathematically to an integer.</span>
+</span><span id="TypeParser.parse_int-531"><a href="#TypeParser.parse_int-531"><span class="linenos">531</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form &lt;code&gt;&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;&lt;/code&gt; will be interpreted as the expression &lt;code&gt;&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)&lt;/code&gt;, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note that &lt;var&gt;M&lt;/var&gt; must be an integer and &lt;var&gt;X&lt;/var&gt; must be a non-negative integer, even in cases where the expression would evaluate mathematically to an integer.</span>
 </span><span id="TypeParser.parse_int-532"><a href="#TypeParser.parse_int-532"><span class="linenos">532</span></a>
 </span><span id="TypeParser.parse_int-533"><a href="#TypeParser.parse_int-533"><span class="linenos">533</span></a><span class="sd">			Returns</span>
 </span><span id="TypeParser.parse_int-534"><a href="#TypeParser.parse_int-534"><span class="linenos">534</span></a><span class="sd">			-------</span>
 </span><span id="TypeParser.parse_int-535"><a href="#TypeParser.parse_int-535"><span class="linenos">535</span></a><span class="sd">			parsed int value</span>
 </span><span id="TypeParser.parse_int-536"><a href="#TypeParser.parse_int-536"><span class="linenos">536</span></a>
 </span><span id="TypeParser.parse_int-537"><a href="#TypeParser.parse_int-537"><span class="linenos">537</span></a><span class="sd">			Raises</span>
 </span><span id="TypeParser.parse_int-538"><a href="#TypeParser.parse_int-538"><span class="linenos">538</span></a><span class="sd">			------</span>
@@ -2084,15 +2084,15 @@
 
 <h2 id="parameters">Parameters</h2>
 
 <p><code>value</code>
 : string to be parsed</p>
 
 <p><code>allow_scientific</code>
-: whether to accept scientific notation. If True, strings of the form <code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression <code><var>M</var> * (10 <em>* <var>X</var>)</code>, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note <var>M</var> *must</em> be an integer and <var>X</var> <em>must</em> be a non-negative integer, even in cases where the above expression evaluates mathematically to an integer.</p>
+: whether to accept scientific notation. If True, strings of the form <code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression <code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note that <var>M</var> must be an integer and <var>X</var> must be a non-negative integer, even in cases where the expression would evaluate mathematically to an integer.</p>
 
 <h2 id="returns">Returns</h2>
 
 <p>parsed int value</p>
 
 <h2 id="raises">Raises</h2>
```

#### html2text {}

```diff
@@ -47,15 +47,15 @@
 _6
 - give exact Decimal values instead of floats
 _7
 - detect inline lists
 _8"""
 _9
 10
-11__version__ = "0.2.4"
+11__version__ = "0.2.5"
 12
 13from ._common import AnyScalar, AnyScalarType, AnyValue, AnyValueType,
 GenericValue, Nullable
 14from ._parser import TypeParser
 15from ._reduce_types import reduce_types
 16
 17__all__ = ('TypeParser', 'reduce_types')
@@ -514,15 +514,15 @@
 return True
 _290
 _291
 return False
 _292
 _293
 _294
-def is_int(self, value: str, *, allow_sign: bool=True, allow_negative:
+def is_int(self, value: str, *, allow_negative: bool=True, allow_sign:
 bool=True, allow_scientific: bool=True) -> bool:
 _295
 """
 _296
 Check if a string represents an int
 _297
 _298
@@ -538,26 +538,26 @@
 `allow_negative`
 _304
 : whether to accept negative values
 _305
 _306
 `allow_sign`
 _307
-: whether to accept signed values. If False, it implies that `allow_negative`
-is False also.
+: whether to accept values prepended with a sign character. If False, it
+implies that `allow_negative` is False also.
 _308
 _309
 `allow_scientific`
 _310
 : whether to accept scientific notation. If True, strings of the form
 <code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression
 <code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the
-mantissa/significand and <var>X</var> is the exponent. Note <var>M</var> *must*
-be an integer and <var>X</var> *must* be a non-negative integer, even in cases
-where the above expression evaluates mathematically to an integer.
+mantissa/significand and <var>X</var> is the exponent. Note that <var>M</var>
+must be an integer and <var>X</var> must be a non-negative integer, even in
+cases where the expression would evaluate mathematically to an integer.
 _311
 _312
 Returns
 _313
 -------
 _314
 whether it is an int
@@ -978,17 +978,17 @@
 _529
 _530
 `allow_scientific`
 _531
 : whether to accept scientific notation. If True, strings of the form
 <code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression
 <code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the
-mantissa/significand and <var>X</var> is the exponent. Note <var>M</var> *must*
-be an integer and <var>X</var> *must* be a non-negative integer, even in cases
-where the above expression evaluates mathematically to an integer.
+mantissa/significand and <var>X</var> is the exponent. Note that <var>M</var>
+must be an integer and <var>X</var> must be a non-negative integer, even in
+cases where the expression would evaluate mathematically to an integer.
 _532
 _533
 Returns
 _534
 -------
 _535
 parsed int value
@@ -2480,19 +2480,19 @@
 parser.is_bool("")      # True
 parser.is_bool("abc")   # False
 ⁰
 def is_int(
 self,
 value: str,
 *,
-allow_sign: bool = True,
 allow_negative: bool = True,
+allow_sign: bool = True,
 allow_scientific: bool = True) -> bool: View Source
 294
-def is_int(self, value: str, *, allow_sign: bool=True, allow_negative:
+def is_int(self, value: str, *, allow_negative: bool=True, allow_sign:
 bool=True, allow_scientific: bool=True) -> bool:
 295
 """
 296
 Check if a string represents an int
 297
 298
@@ -2508,26 +2508,26 @@
 `allow_negative`
 304
 : whether to accept negative values
 305
 306
 `allow_sign`
 307
-: whether to accept signed values. If False, it implies that `allow_negative`
-is False also.
+: whether to accept values prepended with a sign character. If False, it
+implies that `allow_negative` is False also.
 308
 309
 `allow_scientific`
 310
 : whether to accept scientific notation. If True, strings of the form
 <code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression
 <code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the
-mantissa/significand and <var>X</var> is the exponent. Note <var>M</var> *must*
-be an integer and <var>X</var> *must* be a non-negative integer, even in cases
-where the above expression evaluates mathematically to an integer.
+mantissa/significand and <var>X</var> is the exponent. Note that <var>M</var>
+must be an integer and <var>X</var> must be a non-negative integer, even in
+cases where the expression would evaluate mathematically to an integer.
 311
 312
 Returns
 313
 -------
 314
 whether it is an int
@@ -2623,21 +2623,21 @@
 return False
 362
 return True
 Check if a string represents an int
 ***** Parameters *****
 value : string to be checked
 allow_negative : whether to accept negative values
-allow_sign : whether to accept signed values. If False, it implies that
-allow_negative is False also.
+allow_sign : whether to accept values prepended with a sign character. If
+False, it implies that allow_negative is False also.
 allow_scientific : whether to accept scientific notation. If True, strings of
-the form "MeX" will be interpreted as the expression M * (10 * X), where M is
-the mantissa/significand and X is the exponent. Note M *must
- be an integer and X must be a non-negative integer, even in cases where the
-above expression evaluates mathematically to an integer.
+the form "MeX" will be interpreted as the expression M * (10 ** X), where M is
+the mantissa/significand and X is the exponent. Note that M must be an integer
+and X must be a non-negative integer, even in cases where the expression would
+evaluate mathematically to an integer.
 ***** Returns *****
 whether it is an int
 ***** Examples *****
 parser = TypeParser()
 parser.is_int("0")    # True
 parser.is_int("-1")   # True
 parser.is_int("abc")  # False
@@ -3037,17 +3037,17 @@
 529
 530
 `allow_scientific`
 531
 : whether to accept scientific notation. If True, strings of the form
 <code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression
 <code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the
-mantissa/significand and <var>X</var> is the exponent. Note <var>M</var> *must*
-be an integer and <var>X</var> *must* be a non-negative integer, even in cases
-where the above expression evaluates mathematically to an integer.
+mantissa/significand and <var>X</var> is the exponent. Note that <var>M</var>
+must be an integer and <var>X</var> must be a non-negative integer, even in
+cases where the expression would evaluate mathematically to an integer.
 532
 533
 Returns
 534
 -------
 535
 parsed int value
@@ -3116,18 +3116,18 @@
 raise ValueError(f"not an integer: {value}")
 Parse a string and return it as an int if possible
 If the string represents a bool, it will be converted to 1 for True and 0 for
 False.
 ***** Parameters *****
 value : string to be parsed
 allow_scientific : whether to accept scientific notation. If True, strings of
-the form "MeX" will be interpreted as the expression M * (10 * X), where M is
-the mantissa/significand and X is the exponent. Note M *must
- be an integer and X must be a non-negative integer, even in cases where the
-above expression evaluates mathematically to an integer.
+the form "MeX" will be interpreted as the expression M * (10 ** X), where M is
+the mantissa/significand and X is the exponent. Note that M must be an integer
+and X must be a non-negative integer, even in cases where the expression would
+evaluate mathematically to an integer.
 ***** Returns *****
 parsed int value
 ***** Raises *****
 ValueError if value cannot be parsed
 ***** Examples *****
 parser = TypeParser()
 parser.parse_int("0")    # 0
```

### Comparing `parsetypes-0.2.4/docs/html/search.js` & `parsetypes-0.2.5/docs/html/search.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -728,16 +728,16 @@
                     "funcdef": "def"
                 },
                 "parsetypes.TypeParser.is_int": {
                     "fullname": "parsetypes.TypeParser.is_int",
                     "modulename": "parsetypes",
                     "qualname": "TypeParser.is_int",
                     "kind": "function",
-                    "doc": "<p>Check if a string represents an int</p>\n\n<h2 id=\"parameters\">Parameters</h2>\n\n<p><code>value</code>\n: string to be checked</p>\n\n<p><code>allow_negative</code>\n: whether to accept negative values</p>\n\n<p><code>allow_sign</code>\n: whether to accept signed values. If False, it implies that <code>allow_negative</code> is False also.</p>\n\n<p><code>allow_scientific</code>\n: whether to accept scientific notation. If True, strings of the form <code>\"<var>M</var>e<var>X</var>\"</code> will be interpreted as the expression <code><var>M</var> * (10 <em>* <var>X</var>)</code>, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note <var>M</var> *must</em> be an integer and <var>X</var> <em>must</em> be a non-negative integer, even in cases where the above expression evaluates mathematically to an integer.</p>\n\n<h2 id=\"returns\">Returns</h2>\n\n<p>whether it is an int</p>\n\n<h2 id=\"examples\">Examples</h2>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"n\">parser</span> <span class=\"o\">=</span> <span class=\"n\">TypeParser</span><span class=\"p\">()</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">is_int</span><span class=\"p\">(</span><span class=\"s2\">&quot;0&quot;</span><span class=\"p\">)</span>    <span class=\"c1\"># True</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">is_int</span><span class=\"p\">(</span><span class=\"s2\">&quot;-1&quot;</span><span class=\"p\">)</span>   <span class=\"c1\"># True</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">is_int</span><span class=\"p\">(</span><span class=\"s2\">&quot;abc&quot;</span><span class=\"p\">)</span>  <span class=\"c1\"># False</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">is_int</span><span class=\"p\">(</span><span class=\"s2\">&quot;&quot;</span><span class=\"p\">)</span>     <span class=\"c1\"># False</span>\n</code></pre>\n</div>\n",
-                    "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"bp\">self</span>,</span><span class=\"param\">\t<span class=\"n\">value</span><span class=\"p\">:</span> <span class=\"nb\">str</span>,</span><span class=\"param\">\t<span class=\"o\">*</span>,</span><span class=\"param\">\t<span class=\"n\">allow_sign</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">True</span>,</span><span class=\"param\">\t<span class=\"n\">allow_negative</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">True</span>,</span><span class=\"param\">\t<span class=\"n\">allow_scientific</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">True</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">bool</span>:</span></span>",
+                    "doc": "<p>Check if a string represents an int</p>\n\n<h2 id=\"parameters\">Parameters</h2>\n\n<p><code>value</code>\n: string to be checked</p>\n\n<p><code>allow_negative</code>\n: whether to accept negative values</p>\n\n<p><code>allow_sign</code>\n: whether to accept values prepended with a sign character. If False, it implies that <code>allow_negative</code> is False also.</p>\n\n<p><code>allow_scientific</code>\n: whether to accept scientific notation. If True, strings of the form <code>\"<var>M</var>e<var>X</var>\"</code> will be interpreted as the expression <code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note that <var>M</var> must be an integer and <var>X</var> must be a non-negative integer, even in cases where the expression would evaluate mathematically to an integer.</p>\n\n<h2 id=\"returns\">Returns</h2>\n\n<p>whether it is an int</p>\n\n<h2 id=\"examples\">Examples</h2>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"n\">parser</span> <span class=\"o\">=</span> <span class=\"n\">TypeParser</span><span class=\"p\">()</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">is_int</span><span class=\"p\">(</span><span class=\"s2\">&quot;0&quot;</span><span class=\"p\">)</span>    <span class=\"c1\"># True</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">is_int</span><span class=\"p\">(</span><span class=\"s2\">&quot;-1&quot;</span><span class=\"p\">)</span>   <span class=\"c1\"># True</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">is_int</span><span class=\"p\">(</span><span class=\"s2\">&quot;abc&quot;</span><span class=\"p\">)</span>  <span class=\"c1\"># False</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">is_int</span><span class=\"p\">(</span><span class=\"s2\">&quot;&quot;</span><span class=\"p\">)</span>     <span class=\"c1\"># False</span>\n</code></pre>\n</div>\n",
+                    "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"bp\">self</span>,</span><span class=\"param\">\t<span class=\"n\">value</span><span class=\"p\">:</span> <span class=\"nb\">str</span>,</span><span class=\"param\">\t<span class=\"o\">*</span>,</span><span class=\"param\">\t<span class=\"n\">allow_negative</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">True</span>,</span><span class=\"param\">\t<span class=\"n\">allow_sign</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">True</span>,</span><span class=\"param\">\t<span class=\"n\">allow_scientific</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">True</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">bool</span>:</span></span>",
                     "funcdef": "def"
                 },
                 "parsetypes.TypeParser.is_float": {
                     "fullname": "parsetypes.TypeParser.is_float",
                     "modulename": "parsetypes",
                     "qualname": "TypeParser.is_float",
                     "kind": "function",
@@ -773,15 +773,15 @@
                     "funcdef": "def"
                 },
                 "parsetypes.TypeParser.parse_int": {
                     "fullname": "parsetypes.TypeParser.parse_int",
                     "modulename": "parsetypes",
                     "qualname": "TypeParser.parse_int",
                     "kind": "function",
-                    "doc": "<p>Parse a string and return it as an int if possible</p>\n\n<p>If the string represents a bool, it will be converted to <code>1</code> for True and <code>0</code> for False.</p>\n\n<h2 id=\"parameters\">Parameters</h2>\n\n<p><code>value</code>\n: string to be parsed</p>\n\n<p><code>allow_scientific</code>\n: whether to accept scientific notation. If True, strings of the form <code>\"<var>M</var>e<var>X</var>\"</code> will be interpreted as the expression <code><var>M</var> * (10 <em>* <var>X</var>)</code>, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note <var>M</var> *must</em> be an integer and <var>X</var> <em>must</em> be a non-negative integer, even in cases where the above expression evaluates mathematically to an integer.</p>\n\n<h2 id=\"returns\">Returns</h2>\n\n<p>parsed int value</p>\n\n<h2 id=\"raises\">Raises</h2>\n\n<p><code>ValueError</code> if <code>value</code> cannot be parsed</p>\n\n<h2 id=\"examples\">Examples</h2>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"n\">parser</span> <span class=\"o\">=</span> <span class=\"n\">TypeParser</span><span class=\"p\">()</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">parse_int</span><span class=\"p\">(</span><span class=\"s2\">&quot;0&quot;</span><span class=\"p\">)</span>    <span class=\"c1\"># 0</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">parse_int</span><span class=\"p\">(</span><span class=\"s2\">&quot;-1&quot;</span><span class=\"p\">)</span>   <span class=\"c1\"># -1</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">parse_int</span><span class=\"p\">(</span><span class=\"s2\">&quot;2e3&quot;</span><span class=\"p\">)</span>  <span class=\"c1\"># 2000</span>\n</code></pre>\n</div>\n",
+                    "doc": "<p>Parse a string and return it as an int if possible</p>\n\n<p>If the string represents a bool, it will be converted to <code>1</code> for True and <code>0</code> for False.</p>\n\n<h2 id=\"parameters\">Parameters</h2>\n\n<p><code>value</code>\n: string to be parsed</p>\n\n<p><code>allow_scientific</code>\n: whether to accept scientific notation. If True, strings of the form <code>\"<var>M</var>e<var>X</var>\"</code> will be interpreted as the expression <code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note that <var>M</var> must be an integer and <var>X</var> must be a non-negative integer, even in cases where the expression would evaluate mathematically to an integer.</p>\n\n<h2 id=\"returns\">Returns</h2>\n\n<p>parsed int value</p>\n\n<h2 id=\"raises\">Raises</h2>\n\n<p><code>ValueError</code> if <code>value</code> cannot be parsed</p>\n\n<h2 id=\"examples\">Examples</h2>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"n\">parser</span> <span class=\"o\">=</span> <span class=\"n\">TypeParser</span><span class=\"p\">()</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">parse_int</span><span class=\"p\">(</span><span class=\"s2\">&quot;0&quot;</span><span class=\"p\">)</span>    <span class=\"c1\"># 0</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">parse_int</span><span class=\"p\">(</span><span class=\"s2\">&quot;-1&quot;</span><span class=\"p\">)</span>   <span class=\"c1\"># -1</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">parse_int</span><span class=\"p\">(</span><span class=\"s2\">&quot;2e3&quot;</span><span class=\"p\">)</span>  <span class=\"c1\"># 2000</span>\n</code></pre>\n</div>\n",
                     "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">value</span><span class=\"p\">:</span> <span class=\"nb\">str</span>, </span><span class=\"param\"><span class=\"o\">*</span>, </span><span class=\"param\"><span class=\"n\">allow_scientific</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">True</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">int</span>:</span></span>",
                     "funcdef": "def"
                 },
                 "parsetypes.TypeParser.parse_float": {
                     "fullname": "parsetypes.TypeParser.parse_float",
                     "modulename": "parsetypes",
                     "qualname": "TypeParser.parse_float",
@@ -930,15 +930,15 @@
                 "parsetypes.TypeParser.is_int": {
                     "qualname": 3,
                     "fullname": 4,
                     "annotation": 0,
                     "default_value": 0,
                     "signature": 89,
                     "bases": 0,
-                    "doc": 289
+                    "doc": 290
                 },
                 "parsetypes.TypeParser.is_float": {
                     "qualname": 3,
                     "fullname": 4,
                     "annotation": 0,
                     "default_value": 0,
                     "signature": 89,
@@ -975,15 +975,15 @@
                 "parsetypes.TypeParser.parse_int": {
                     "qualname": 3,
                     "fullname": 4,
                     "annotation": 0,
                     "default_value": 0,
                     "signature": 47,
                     "bases": 0,
-                    "doc": 270
+                    "doc": 267
                 },
                 "parsetypes.TypeParser.parse_float": {
                     "qualname": 3,
                     "fullname": 4,
                     "annotation": 0,
                     "default_value": 0,
                     "signature": 89,
@@ -3921,30 +3921,30 @@
                         "parsetypes.TypeParser.is_none": {
                             "tf": 9.16515138991168
                         },
                         "parsetypes.TypeParser.is_bool": {
                             "tf": 10.392304845413264
                         },
                         "parsetypes.TypeParser.is_int": {
-                            "tf": 12.449899597988733
+                            "tf": 12.288205727444508
                         },
                         "parsetypes.TypeParser.is_float": {
                             "tf": 12.84523257866513
                         },
                         "parsetypes.TypeParser.is_decimal": {
                             "tf": 2.23606797749979
                         },
                         "parsetypes.TypeParser.parse_none": {
                             "tf": 9.591663046625438
                         },
                         "parsetypes.TypeParser.parse_bool": {
                             "tf": 9.899494936611665
                         },
                         "parsetypes.TypeParser.parse_int": {
-                            "tf": 11.789826122551595
+                            "tf": 11.61895003862225
                         },
                         "parsetypes.TypeParser.parse_float": {
                             "tf": 14.352700094407323
                         },
                         "parsetypes.TypeParser.parse_decimal": {
                             "tf": 14.45683229480096
                         },
@@ -4153,25 +4153,28 @@
                                         "parsetypes.TypeParser.is_none": {
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser.is_bool": {
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser.is_int": {
-                                            "tf": 1
+                                            "tf": 1.4142135623730951
                                         },
                                         "parsetypes.TypeParser.is_float": {
                                             "tf": 1.7320508075688772
                                         },
                                         "parsetypes.TypeParser.parse_none": {
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser.parse_bool": {
                                             "tf": 1
                                         },
+                                        "parsetypes.TypeParser.parse_int": {
+                                            "tf": 1
+                                        },
                                         "parsetypes.TypeParser.parse_float": {
                                             "tf": 2.23606797749979
                                         },
                                         "parsetypes.TypeParser.parse_decimal": {
                                             "tf": 2.23606797749979
                                         },
                                         "parsetypes.TypeParser.infer_series": {
@@ -4189,15 +4192,15 @@
                                         "parsetypes.TypeParser.iterate_table": {
                                             "tf": 2
                                         },
                                         "parsetypes.reduce_types": {
                                             "tf": 1
                                         }
                                     },
-                                    "df": 16
+                                    "df": 17
                                 }
                             }
                         },
                         "o": {
                             "docs": {
                                 "parsetypes": {
                                     "tf": 1.4142135623730951
@@ -5047,25 +5050,28 @@
                                                     "docs": {},
                                                     "df": 0,
                                                     "d": {
                                                         "docs": {
                                                             "parsetypes.TypeParser.__init__": {
                                                                 "tf": 1
                                                             },
+                                                            "parsetypes.TypeParser.is_int": {
+                                                                "tf": 1
+                                                            },
                                                             "parsetypes.TypeParser.is_float": {
                                                                 "tf": 1
                                                             },
                                                             "parsetypes.TypeParser.parse_float": {
                                                                 "tf": 1
                                                             },
                                                             "parsetypes.TypeParser.parse_decimal": {
                                                                 "tf": 1
                                                             }
                                                         },
-                                                        "df": 4
+                                                        "df": 5
                                                     }
                                                 }
                                             }
                                         }
                                     }
                                 }
                             }
@@ -6061,39 +6067,27 @@
                                 "df": 0,
                                 "n": {
                                     "docs": {
                                         "parsetypes.TypeParser.__init__": {
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser.is_int": {
-                                            "tf": 1
+                                            "tf": 1.4142135623730951
                                         },
                                         "parsetypes.TypeParser.is_float": {
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser.parse_float": {
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser.parse_decimal": {
                                             "tf": 1
                                         }
                                     },
-                                    "df": 5,
-                                    "e": {
-                                        "docs": {},
-                                        "df": 0,
-                                        "d": {
-                                            "docs": {
-                                                "parsetypes.TypeParser.is_int": {
-                                                    "tf": 1
-                                                }
-                                            },
-                                            "df": 1
-                                        }
-                                    }
+                                    "df": 5
                                 }
                             },
                             "n": {
                                 "docs": {},
                                 "df": 0,
                                 "g": {
                                     "docs": {},
@@ -7976,14 +7970,46 @@
                                                     }
                                                 },
                                                 "df": 4
                                             }
                                         }
                                     }
                                 }
+                            },
+                            "a": {
+                                "docs": {},
+                                "df": 0,
+                                "r": {
+                                    "docs": {},
+                                    "df": 0,
+                                    "a": {
+                                        "docs": {},
+                                        "df": 0,
+                                        "c": {
+                                            "docs": {},
+                                            "df": 0,
+                                            "t": {
+                                                "docs": {},
+                                                "df": 0,
+                                                "e": {
+                                                    "docs": {},
+                                                    "df": 0,
+                                                    "r": {
+                                                        "docs": {
+                                                            "parsetypes.TypeParser.is_int": {
+                                                                "tf": 1
+                                                            }
+                                                        },
+                                                        "df": 1
+                                                    }
+                                                }
+                                            }
+                                        }
+                                    }
+                                }
                             }
                         },
                         "s": {
                             "docs": {},
                             "df": 0,
                             "v": {
                                 "docs": {
@@ -9006,15 +9032,15 @@
                             "parsetypes.TypeParser.is_none": {
                                 "tf": 1
                             },
                             "parsetypes.TypeParser.is_bool": {
                                 "tf": 1.7320508075688772
                             },
                             "parsetypes.TypeParser.is_int": {
-                                "tf": 1.4142135623730951
+                                "tf": 1.7320508075688772
                             },
                             "parsetypes.TypeParser.is_float": {
                                 "tf": 2.449489742783178
                             },
                             "parsetypes.TypeParser.parse_none": {
                                 "tf": 1
                             },
@@ -9290,29 +9316,14 @@
                                         "docs": {
                                             "parsetypes.TypeParser": {
                                                 "tf": 1
                                             }
                                         },
                                         "df": 1
                                     }
-                                },
-                                "v": {
-                                    "docs": {},
-                                    "df": 0,
-                                    "e": {
-                                        "docs": {
-                                            "parsetypes.TypeParser.is_int": {
-                                                "tf": 1
-                                            },
-                                            "parsetypes.TypeParser.parse_int": {
-                                                "tf": 1
-                                            }
-                                        },
-                                        "df": 2
-                                    }
                                 }
                             },
                             "c": {
                                 "docs": {
                                     "parsetypes.TypeParser.is_none": {
                                         "tf": 1
                                     },
@@ -10124,17 +10135,20 @@
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser": {
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser.__init__": {
                                             "tf": 1
+                                        },
+                                        "parsetypes.TypeParser.is_int": {
+                                            "tf": 1
                                         }
                                     },
-                                    "df": 3
+                                    "df": 4
                                 }
                             },
                             "l": {
                                 "docs": {},
                                 "df": 0,
                                 "l": {
                                     "docs": {
@@ -10396,17 +10410,23 @@
                                 "l": {
                                     "docs": {},
                                     "df": 0,
                                     "d": {
                                         "docs": {
                                             "parsetypes.TypeParser.__init__": {
                                                 "tf": 1
+                                            },
+                                            "parsetypes.TypeParser.is_int": {
+                                                "tf": 1
+                                            },
+                                            "parsetypes.TypeParser.parse_int": {
+                                                "tf": 1
                                             }
                                         },
-                                        "df": 1
+                                        "df": 3
                                     }
                                 }
                             }
                         }
                     },
                     "e": {
                         "docs": {
@@ -10827,27 +10847,23 @@
                                         "a": {
                                             "docs": {},
                                             "df": 0,
                                             "t": {
                                                 "docs": {},
                                                 "df": 0,
                                                 "e": {
-                                                    "docs": {},
-                                                    "df": 0,
-                                                    "s": {
-                                                        "docs": {
-                                                            "parsetypes.TypeParser.is_int": {
-                                                                "tf": 1
-                                                            },
-                                                            "parsetypes.TypeParser.parse_int": {
-                                                                "tf": 1
-                                                            }
+                                                    "docs": {
+                                                        "parsetypes.TypeParser.is_int": {
+                                                            "tf": 1
                                                         },
-                                                        "df": 2
-                                                    }
+                                                        "parsetypes.TypeParser.parse_int": {
+                                                            "tf": 1
+                                                        }
+                                                    },
+                                                    "df": 2
                                                 }
                                             }
                                         }
                                     }
                                 }
                             }
                         },
```

### Comparing `parsetypes-0.2.4/pyproject.toml` & `parsetypes-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `parsetypes-0.2.4/src/parsetypes/__init__.py` & `parsetypes-0.2.5/src/parsetypes/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 	The `TypeParser` class provides configurable type inference and parsing. This can be initialised with different settings to, for example:
 	- treat `inf` as either a float or a normal string
 	- give exact Decimal values instead of floats
 	- detect inline lists
 """
 
 
-__version__ = "0.2.4"
+__version__ = "0.2.5"
 
 from ._common import AnyScalar, AnyScalarType, AnyValue, AnyValueType, GenericValue, Nullable
 from ._parser import TypeParser
 from ._reduce_types import reduce_types
 
 __all__ = ('TypeParser', 'reduce_types')
```

### Comparing `parsetypes-0.2.4/src/parsetypes/_common.py` & `parsetypes-0.2.5/src/parsetypes/_common.py`

 * *Files identical despite different names*

### Comparing `parsetypes-0.2.4/src/parsetypes/_parser.py` & `parsetypes-0.2.5/src/parsetypes/_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,31 +286,31 @@
 			return True
 		if value in self.false_values:
 			return True
 
 		return False
 
 
-	def is_int(self, value: str, *, allow_sign: bool=True, allow_negative: bool=True, allow_scientific: bool=True) -> bool:
+	def is_int(self, value: str, *, allow_negative: bool=True, allow_sign: bool=True, allow_scientific: bool=True) -> bool:
 		"""
 			Check if a string represents an int
 
 			Parameters
 			----------
 			`value`
 			: string to be checked
 
 			`allow_negative`
 			: whether to accept negative values
 
 			`allow_sign`
-			: whether to accept signed values. If False, it implies that `allow_negative` is False also.
+			: whether to accept values prepended with a sign character. If False, it implies that `allow_negative` is False also.
 
 			`allow_scientific`
-			: whether to accept scientific notation. If True, strings of the form <code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression <code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note <var>M</var> *must* be an integer and <var>X</var> *must* be a non-negative integer, even in cases where the above expression evaluates mathematically to an integer.
+			: whether to accept scientific notation. If True, strings of the form <code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression <code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note that <var>M</var> must be an integer and <var>X</var> must be a non-negative integer, even in cases where the expression would evaluate mathematically to an integer.
 
 			Returns
 			-------
 			whether it is an int
 
 			Examples
 			--------
@@ -523,15 +523,15 @@
 
 			Parameters
 			----------
 			`value`
 			: string to be parsed
 
 			`allow_scientific`
-			: whether to accept scientific notation. If True, strings of the form <code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression <code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note <var>M</var> *must* be an integer and <var>X</var> *must* be a non-negative integer, even in cases where the above expression evaluates mathematically to an integer.
+			: whether to accept scientific notation. If True, strings of the form <code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression <code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the mantissa/significand and <var>X</var> is the exponent. Note that <var>M</var> must be an integer and <var>X</var> must be a non-negative integer, even in cases where the expression would evaluate mathematically to an integer.
 
 			Returns
 			-------
 			parsed int value
 
 			Raises
 			------
```

### Comparing `parsetypes-0.2.4/src/parsetypes/_reduce_types.py` & `parsetypes-0.2.5/src/parsetypes/_reduce_types.py`

 * *Files identical despite different names*

### Comparing `parsetypes-0.2.4/src/parsetypes.egg-info/PKG-INFO` & `parsetypes-0.2.5/src/parsetypes.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsetypes
-Version: 0.2.4
+Version: 0.2.5
 Summary: Parse serialised data to recover their original underlying types
 Author-email: Yu Shiyang <yu.shiyang@gnayihs.uy>
 License: MPL-2.0
 Project-URL: Homepage, https://github.com/yushiyangk/parsetypes
 Project-URL: Documentation, https://parsetypes.gnayihs.uy/
 Project-URL: Issues, https://github.com/yushiyangk/parsetypes/issues
 Keywords: python,str,string,types,conversion
@@ -158,19 +158,23 @@
 
 ## Changelog
 
 This project follows [PEP 440](https://peps.python.org/pep-0440/) and [Semantic Versioning (SemVer)](https://semver.org/spec/v2.0.0.html). In addition to the guarantees specified by SemVer, for versions before 1.0, this project guarantees backwards compatibility of the API for patch version updates (0.<var>y</var>.<b><var>z</var></b>).
 
 The recommended version specifier is <code>parsetypes ~= <var>x</var>.<var>y</var></code> for version 1.0 and later, and <code>parsetypes ~= <var>0</var>.<var>y</var>.<var>z</var></code> for versions prior to 1.0.
 
+### 0.2.5
+
+- Fixed documentation
+
 ### 0.2.4
 
 - Added <code><var>parser</var>.convert()</code>
 
-### 0.2.1, 0.2.2 and 0.2.3
+### 0.2.1, 0.2.2, 0.2.3
 
 - Fixed documentation
 
 ### 0.2
 
 - Added support for Python version 3.9; previously only 3.10 and 3.11 were supported
```

### Comparing `parsetypes-0.2.4/src/parsetypes.egg-info/SOURCES.txt` & `parsetypes-0.2.5/src/parsetypes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `parsetypes-0.2.4/tests/test_parser.py` & `parsetypes-0.2.5/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `parsetypes-0.2.4/tests/test_reduce_types.py` & `parsetypes-0.2.5/tests/test_reduce_types.py`

 * *Files identical despite different names*

