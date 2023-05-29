# Comparing `tmp/parsetypes-0.2.5.tar.gz` & `tmp/parsetypes-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsetypes-0.2.5.tar", last modified: Mon May 29 03:58:43 2023, max compression
+gzip compressed data, was "parsetypes-0.2.6.tar", last modified: Mon May 29 04:17:33 2023, max compression
```

## Comparing `parsetypes-0.2.5.tar` & `parsetypes-0.2.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 03:58:43.700784 parsetypes-0.2.5/
--rw-rw-rw-   0        0        0      898 2023-05-29 03:57:56.000000 parsetypes-0.2.5/CHANGELOG.md
--rw-rw-rw-   0        0        0       22 2023-05-28 02:54:36.000000 parsetypes-0.2.5/MANIFEST.in
--rw-rw-rw-   0        0        0     6786 2023-05-29 03:58:43.700784 parsetypes-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     4183 2023-05-28 23:00:42.000000 parsetypes-0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 03:58:43.683601 parsetypes-0.2.5/docs/
-drwxrwxrwx   0        0        0        0 2023-05-29 03:58:43.691800 parsetypes-0.2.5/docs/html/
--rw-rw-rw-   0        0        0     1729 2023-05-29 03:58:34.000000 parsetypes-0.2.5/docs/html/favicon.png
--rw-rw-rw-   0        0        0      141 2023-05-29 03:58:34.000000 parsetypes-0.2.5/docs/html/index.html
--rw-rw-rw-   0        0        0   529234 2023-05-29 03:58:34.000000 parsetypes-0.2.5/docs/html/parsetypes.html
--rw-rw-rw-   0        0        0   217649 2023-05-29 03:58:34.000000 parsetypes-0.2.5/docs/html/search.js
--rw-rw-rw-   0        0        0     2297 2023-05-28 04:48:55.000000 parsetypes-0.2.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-29 03:58:43.700784 parsetypes-0.2.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-29 03:58:43.684594 parsetypes-0.2.5/src/
-drwxrwxrwx   0        0        0        0 2023-05-29 03:58:43.694786 parsetypes-0.2.5/src/parsetypes/
--rw-rw-rw-   0        0        0      621 2023-05-29 03:58:00.000000 parsetypes-0.2.5/src/parsetypes/__init__.py
--rw-rw-rw-   0        0        0     1254 2023-05-28 05:37:03.000000 parsetypes-0.2.5/src/parsetypes/_common.py
--rw-rw-rw-   0        0        0      348 2023-05-28 04:48:55.000000 parsetypes-0.2.5/src/parsetypes/_compat.py
--rw-rw-rw-   0        0        0    35499 2023-05-29 03:56:49.000000 parsetypes-0.2.5/src/parsetypes/_parser.py
--rw-rw-rw-   0        0        0     5203 2023-05-28 05:32:22.000000 parsetypes-0.2.5/src/parsetypes/_reduce_types.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:58:43.697786 parsetypes-0.2.5/src/parsetypes.egg-info/
--rw-rw-rw-   0        0        0     6786 2023-05-29 03:58:43.000000 parsetypes-0.2.5/src/parsetypes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      512 2023-05-29 03:58:43.000000 parsetypes-0.2.5/src/parsetypes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 03:58:43.000000 parsetypes-0.2.5/src/parsetypes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      296 2023-05-29 03:58:43.000000 parsetypes-0.2.5/src/parsetypes.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-29 03:58:43.000000 parsetypes-0.2.5/src/parsetypes.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-29 03:58:43.698786 parsetypes-0.2.5/tests/
--rw-rw-rw-   0        0        0    67890 2023-05-28 23:00:42.000000 parsetypes-0.2.5/tests/test_parser.py
--rw-rw-rw-   0        0        0     8837 2023-05-28 04:48:55.000000 parsetypes-0.2.5/tests/test_reduce_types.py
+drwxrwxrwx   0        0        0        0 2023-05-29 04:17:33.682238 parsetypes-0.2.6/
+-rw-rw-rw-   0        0        0     1049 2023-05-29 04:16:43.000000 parsetypes-0.2.6/CHANGELOG.md
+-rw-rw-rw-   0        0        0       22 2023-05-28 02:54:36.000000 parsetypes-0.2.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     6937 2023-05-29 04:17:33.682238 parsetypes-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4183 2023-05-28 23:00:42.000000 parsetypes-0.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 04:17:33.664179 parsetypes-0.2.6/docs/
+drwxrwxrwx   0        0        0        0 2023-05-29 04:17:33.673177 parsetypes-0.2.6/docs/html/
+-rw-rw-rw-   0        0        0     1729 2023-05-29 04:17:22.000000 parsetypes-0.2.6/docs/html/favicon.png
+-rw-rw-rw-   0        0        0      141 2023-05-29 04:17:21.000000 parsetypes-0.2.6/docs/html/index.html
+-rw-rw-rw-   0        0        0   534652 2023-05-29 04:17:21.000000 parsetypes-0.2.6/docs/html/parsetypes.html
+-rw-rw-rw-   0        0        0   222730 2023-05-29 04:17:22.000000 parsetypes-0.2.6/docs/html/search.js
+-rw-rw-rw-   0        0        0     2297 2023-05-28 04:48:55.000000 parsetypes-0.2.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-29 04:17:33.683237 parsetypes-0.2.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-29 04:17:33.665177 parsetypes-0.2.6/src/
+drwxrwxrwx   0        0        0        0 2023-05-29 04:17:33.677237 parsetypes-0.2.6/src/parsetypes/
+-rw-rw-rw-   0        0        0      633 2023-05-29 04:16:43.000000 parsetypes-0.2.6/src/parsetypes/__init__.py
+-rw-rw-rw-   0        0        0     1298 2023-05-29 04:16:43.000000 parsetypes-0.2.6/src/parsetypes/_common.py
+-rw-rw-rw-   0        0        0      348 2023-05-28 04:48:55.000000 parsetypes-0.2.6/src/parsetypes/_compat.py
+-rw-rw-rw-   0        0        0    35501 2023-05-29 04:16:43.000000 parsetypes-0.2.6/src/parsetypes/_parser.py
+-rw-rw-rw-   0        0        0     5203 2023-05-28 05:32:22.000000 parsetypes-0.2.6/src/parsetypes/_reduce_types.py
+drwxrwxrwx   0        0        0        0 2023-05-29 04:17:33.680238 parsetypes-0.2.6/src/parsetypes.egg-info/
+-rw-rw-rw-   0        0        0     6937 2023-05-29 04:17:33.000000 parsetypes-0.2.6/src/parsetypes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2023-05-29 04:17:33.000000 parsetypes-0.2.6/src/parsetypes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 04:17:33.000000 parsetypes-0.2.6/src/parsetypes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      296 2023-05-29 04:17:33.000000 parsetypes-0.2.6/src/parsetypes.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-29 04:17:33.000000 parsetypes-0.2.6/src/parsetypes.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-29 04:17:33.681238 parsetypes-0.2.6/tests/
+-rw-rw-rw-   0        0        0    67890 2023-05-28 23:00:42.000000 parsetypes-0.2.6/tests/test_parser.py
+-rw-rw-rw-   0        0        0     8837 2023-05-28 04:48:55.000000 parsetypes-0.2.6/tests/test_reduce_types.py
```

### Comparing `parsetypes-0.2.5/PKG-INFO` & `parsetypes-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsetypes
-Version: 0.2.5
+Version: 0.2.6
 Summary: Parse serialised data to recover their original underlying types
 Author-email: Yu Shiyang <yu.shiyang@gnayihs.uy>
 License: MPL-2.0
 Project-URL: Homepage, https://github.com/yushiyangk/parsetypes
 Project-URL: Documentation, https://parsetypes.gnayihs.uy/
 Project-URL: Issues, https://github.com/yushiyangk/parsetypes/issues
 Keywords: python,str,string,types,conversion
@@ -158,14 +158,18 @@
 
 ## Changelog
 
 This project follows [PEP 440](https://peps.python.org/pep-0440/) and [Semantic Versioning (SemVer)](https://semver.org/spec/v2.0.0.html). In addition to the guarantees specified by SemVer, for versions before 1.0, this project guarantees backwards compatibility of the API for patch version updates (0.<var>y</var>.<b><var>z</var></b>).
 
 The recommended version specifier is <code>parsetypes ~= <var>x</var>.<var>y</var></code> for version 1.0 and later, and <code>parsetypes ~= <var>0</var>.<var>y</var>.<var>z</var></code> for versions prior to 1.0.
 
+### 0.2.6
+
+- Added `Nullable` to automatic imports via `from parsetypes import *` (previously only `TypeParser` and `reduce_types` were imported)
+
 ### 0.2.5
 
 - Fixed documentation
 
 ### 0.2.4
 
 - Added <code><var>parser</var>.convert()</code>
```

### Comparing `parsetypes-0.2.5/README.md` & `parsetypes-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `parsetypes-0.2.5/docs/html/favicon.png` & `parsetypes-0.2.6/docs/html/favicon.png`

 * *Files identical despite different names*

### Comparing `parsetypes-0.2.5/docs/html/parsetypes.html` & `parsetypes-0.2.6/docs/html/parsetypes.html`

 * *Files 2% similar despite different names*

```diff
@@ -161,14 +161,23 @@
             			</li>
             	</ul>
 
 			</li>
 			<li>
 						<a class="function" href="#reduce_types">reduce_types<span class="decorator">()</span></a>
 			</li>
+			<li>
+					<a class="class" href="#Nullable">Nullable</a>
+							<ul class="memberlist">
+            			<li>
+            						<a class="function" href="#Nullable.__init__">Nullable</a>
+            			</li>
+            	</ul>
+
+			</li>
 	</ul>
 
 
 
         <a class="attribution" title="pdoc: Python API documentation generator" href="https://pdoc.dev" target="_blank">
             built with <span class="visually-hidden">pdoc</span><img
                 alt="pdoc logo"
@@ -204,21 +213,21 @@
 </span><span id="L-4"><a href="#L-4"><span class="linenos"> 4</span></a><span class="sd">	The `TypeParser` class provides configurable type inference and parsing. This can be initialised with different settings to, for example:</span>
 </span><span id="L-5"><a href="#L-5"><span class="linenos"> 5</span></a><span class="sd">	- treat `inf` as either a float or a normal string</span>
 </span><span id="L-6"><a href="#L-6"><span class="linenos"> 6</span></a><span class="sd">	- give exact Decimal values instead of floats</span>
 </span><span id="L-7"><a href="#L-7"><span class="linenos"> 7</span></a><span class="sd">	- detect inline lists</span>
 </span><span id="L-8"><a href="#L-8"><span class="linenos"> 8</span></a><span class="sd">&quot;&quot;&quot;</span>
 </span><span id="L-9"><a href="#L-9"><span class="linenos"> 9</span></a>
 </span><span id="L-10"><a href="#L-10"><span class="linenos">10</span></a>
-</span><span id="L-11"><a href="#L-11"><span class="linenos">11</span></a><span class="n">__version__</span> <span class="o">=</span> <span class="s2">&quot;0.2.5&quot;</span>
+</span><span id="L-11"><a href="#L-11"><span class="linenos">11</span></a><span class="n">__version__</span> <span class="o">=</span> <span class="s2">&quot;0.2.6&quot;</span>
 </span><span id="L-12"><a href="#L-12"><span class="linenos">12</span></a>
 </span><span id="L-13"><a href="#L-13"><span class="linenos">13</span></a><span class="kn">from</span> <span class="nn">._common</span> <span class="kn">import</span> <span class="n">AnyScalar</span><span class="p">,</span> <span class="n">AnyScalarType</span><span class="p">,</span> <span class="n">AnyValue</span><span class="p">,</span> <span class="n">AnyValueType</span><span class="p">,</span> <span class="n">GenericValue</span><span class="p">,</span> <span class="n">Nullable</span>
 </span><span id="L-14"><a href="#L-14"><span class="linenos">14</span></a><span class="kn">from</span> <span class="nn">._parser</span> <span class="kn">import</span> <span class="n">TypeParser</span>
 </span><span id="L-15"><a href="#L-15"><span class="linenos">15</span></a><span class="kn">from</span> <span class="nn">._reduce_types</span> <span class="kn">import</span> <span class="n">reduce_types</span>
 </span><span id="L-16"><a href="#L-16"><span class="linenos">16</span></a>
-</span><span id="L-17"><a href="#L-17"><span class="linenos">17</span></a><span class="n">__all__</span> <span class="o">=</span> <span class="p">(</span><span class="s1">&#39;TypeParser&#39;</span><span class="p">,</span> <span class="s1">&#39;reduce_types&#39;</span><span class="p">)</span>
+</span><span id="L-17"><a href="#L-17"><span class="linenos">17</span></a><span class="n">__all__</span> <span class="o">=</span> <span class="p">(</span><span class="s1">&#39;TypeParser&#39;</span><span class="p">,</span> <span class="s1">&#39;reduce_types&#39;</span><span class="p">,</span> <span class="s1">&#39;Nullable&#39;</span><span class="p">)</span>
 </span></pre></div>
 
 
             </section>
                 <section id="TypeParser">
                             <input id="TypeParser-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr class">
@@ -259,15 +268,15 @@
 </span><span id="TypeParser-85"><a href="#TypeParser-85"><span class="linenos">  85</span></a>
 </span><span id="TypeParser-86"><a href="#TypeParser-86"><span class="linenos">  86</span></a><span class="sd">			Parameters</span>
 </span><span id="TypeParser-87"><a href="#TypeParser-87"><span class="linenos">  87</span></a><span class="sd">			----------</span>
 </span><span id="TypeParser-88"><a href="#TypeParser-88"><span class="linenos">  88</span></a><span class="sd">			`trim`</span>
 </span><span id="TypeParser-89"><a href="#TypeParser-89"><span class="linenos">  89</span></a><span class="sd">			: whether leading and trailing whitespace should be stripped from strings</span>
 </span><span id="TypeParser-90"><a href="#TypeParser-90"><span class="linenos">  90</span></a>
 </span><span id="TypeParser-91"><a href="#TypeParser-91"><span class="linenos">  91</span></a><span class="sd">			`use_decimal`</span>
-</span><span id="TypeParser-92"><a href="#TypeParser-92"><span class="linenos">  92</span></a><span class="sd">			: whether non-integer numeric values should be inferred as Decimal (exact values) instead of float (non-exact values). Note that this only applies to methods that attempt to infer type (`infer()` and `infer_*()`), and does not affect methods where the type is explicitly specified (`is_float()`, `is_decimal()`, `parse_float()`, `parse_decimal()`).</span>
+</span><span id="TypeParser-92"><a href="#TypeParser-92"><span class="linenos">  92</span></a><span class="sd">			: whether non-integer numeric values should be inferred to be Decimal (exact values) instead of float (non-exact values). Note that this only applies to methods that attempt to infer type (`infer()` and `infer_*()`), and does not affect methods where the type is explicitly specified (`is_float()`, `is_decimal()`, `parse_float()`, `parse_decimal()`).</span>
 </span><span id="TypeParser-93"><a href="#TypeParser-93"><span class="linenos">  93</span></a>
 </span><span id="TypeParser-94"><a href="#TypeParser-94"><span class="linenos">  94</span></a><span class="sd">			`list_delimiter`</span>
 </span><span id="TypeParser-95"><a href="#TypeParser-95"><span class="linenos">  95</span></a><span class="sd">			: the delimiter used for identifying lists and for separating list items. If set to None, the parser will not attempt to identify lists when inferring types, which usually causes the value to be treated as a str instead.</span>
 </span><span id="TypeParser-96"><a href="#TypeParser-96"><span class="linenos">  96</span></a>
 </span><span id="TypeParser-97"><a href="#TypeParser-97"><span class="linenos">  97</span></a><span class="sd">			`none_values`</span>
 </span><span id="TypeParser-98"><a href="#TypeParser-98"><span class="linenos">  98</span></a><span class="sd">			: list of strings that represent the value None</span>
 </span><span id="TypeParser-99"><a href="#TypeParser-99"><span class="linenos">  99</span></a>
@@ -1051,15 +1060,15 @@
 </span><span id="TypeParser-877"><a href="#TypeParser-877"><span class="linenos"> 877</span></a>			<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_float</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
 </span><span id="TypeParser-878"><a href="#TypeParser-878"><span class="linenos"> 878</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">str</span><span class="p">:</span>
 </span><span id="TypeParser-879"><a href="#TypeParser-879"><span class="linenos"> 879</span></a>			<span class="k">return</span> <span class="n">value</span>
 </span><span id="TypeParser-880"><a href="#TypeParser-880"><span class="linenos"> 880</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="n">Nullable</span><span class="p">:</span>
 </span><span id="TypeParser-881"><a href="#TypeParser-881"><span class="linenos"> 881</span></a>			<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_none</span><span class="p">(</span><span class="n">value</span><span class="p">):</span>
 </span><span id="TypeParser-882"><a href="#TypeParser-882"><span class="linenos"> 882</span></a>				<span class="k">return</span> <span class="kc">None</span>
 </span><span id="TypeParser-883"><a href="#TypeParser-883"><span class="linenos"> 883</span></a>			<span class="k">else</span><span class="p">:</span>
-</span><span id="TypeParser-884"><a href="#TypeParser-884"><span class="linenos"> 884</span></a>				<span class="k">if</span> <span class="n">type_args</span> <span class="ow">is</span> <span class="ow">not</span>  <span class="kc">None</span> <span class="ow">and</span> <span class="nb">len</span><span class="p">(</span><span class="n">type_args</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span> <span class="ow">and</span> <span class="n">type_args</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">!=</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="TypeParser-884"><a href="#TypeParser-884"><span class="linenos"> 884</span></a>				<span class="k">if</span> <span class="n">type_args</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span> <span class="ow">and</span> <span class="nb">len</span><span class="p">(</span><span class="n">type_args</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span> <span class="ow">and</span> <span class="n">type_args</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">!=</span> <span class="nb">str</span><span class="p">:</span>
 </span><span id="TypeParser-885"><a href="#TypeParser-885"><span class="linenos"> 885</span></a>					<span class="n">inner_type</span> <span class="o">=</span> <span class="n">type_args</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
 </span><span id="TypeParser-886"><a href="#TypeParser-886"><span class="linenos"> 886</span></a>					<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">convert</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">inner_type</span><span class="p">)</span>
 </span><span id="TypeParser-887"><a href="#TypeParser-887"><span class="linenos"> 887</span></a>				<span class="k">else</span><span class="p">:</span>
 </span><span id="TypeParser-888"><a href="#TypeParser-888"><span class="linenos"> 888</span></a>					<span class="k">return</span> <span class="n">value</span>
 </span><span id="TypeParser-889"><a href="#TypeParser-889"><span class="linenos"> 889</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">list</span><span class="p">:</span>
 </span><span id="TypeParser-890"><a href="#TypeParser-890"><span class="linenos"> 890</span></a>			<span class="n">subvalues</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">list_delimiter</span><span class="p">)</span>
 </span><span id="TypeParser-891"><a href="#TypeParser-891"><span class="linenos"> 891</span></a>			<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">trim</span><span class="p">:</span>
@@ -1245,15 +1254,15 @@
 </span><span id="TypeParser.__init__-85"><a href="#TypeParser.__init__-85"><span class="linenos"> 85</span></a>
 </span><span id="TypeParser.__init__-86"><a href="#TypeParser.__init__-86"><span class="linenos"> 86</span></a><span class="sd">			Parameters</span>
 </span><span id="TypeParser.__init__-87"><a href="#TypeParser.__init__-87"><span class="linenos"> 87</span></a><span class="sd">			----------</span>
 </span><span id="TypeParser.__init__-88"><a href="#TypeParser.__init__-88"><span class="linenos"> 88</span></a><span class="sd">			`trim`</span>
 </span><span id="TypeParser.__init__-89"><a href="#TypeParser.__init__-89"><span class="linenos"> 89</span></a><span class="sd">			: whether leading and trailing whitespace should be stripped from strings</span>
 </span><span id="TypeParser.__init__-90"><a href="#TypeParser.__init__-90"><span class="linenos"> 90</span></a>
 </span><span id="TypeParser.__init__-91"><a href="#TypeParser.__init__-91"><span class="linenos"> 91</span></a><span class="sd">			`use_decimal`</span>
-</span><span id="TypeParser.__init__-92"><a href="#TypeParser.__init__-92"><span class="linenos"> 92</span></a><span class="sd">			: whether non-integer numeric values should be inferred as Decimal (exact values) instead of float (non-exact values). Note that this only applies to methods that attempt to infer type (`infer()` and `infer_*()`), and does not affect methods where the type is explicitly specified (`is_float()`, `is_decimal()`, `parse_float()`, `parse_decimal()`).</span>
+</span><span id="TypeParser.__init__-92"><a href="#TypeParser.__init__-92"><span class="linenos"> 92</span></a><span class="sd">			: whether non-integer numeric values should be inferred to be Decimal (exact values) instead of float (non-exact values). Note that this only applies to methods that attempt to infer type (`infer()` and `infer_*()`), and does not affect methods where the type is explicitly specified (`is_float()`, `is_decimal()`, `parse_float()`, `parse_decimal()`).</span>
 </span><span id="TypeParser.__init__-93"><a href="#TypeParser.__init__-93"><span class="linenos"> 93</span></a>
 </span><span id="TypeParser.__init__-94"><a href="#TypeParser.__init__-94"><span class="linenos"> 94</span></a><span class="sd">			`list_delimiter`</span>
 </span><span id="TypeParser.__init__-95"><a href="#TypeParser.__init__-95"><span class="linenos"> 95</span></a><span class="sd">			: the delimiter used for identifying lists and for separating list items. If set to None, the parser will not attempt to identify lists when inferring types, which usually causes the value to be treated as a str instead.</span>
 </span><span id="TypeParser.__init__-96"><a href="#TypeParser.__init__-96"><span class="linenos"> 96</span></a>
 </span><span id="TypeParser.__init__-97"><a href="#TypeParser.__init__-97"><span class="linenos"> 97</span></a><span class="sd">			`none_values`</span>
 </span><span id="TypeParser.__init__-98"><a href="#TypeParser.__init__-98"><span class="linenos"> 98</span></a><span class="sd">			: list of strings that represent the value None</span>
 </span><span id="TypeParser.__init__-99"><a href="#TypeParser.__init__-99"><span class="linenos"> 99</span></a>
@@ -1386,15 +1395,15 @@
 
 <h2 id="parameters">Parameters</h2>
 
 <p><code>trim</code>
 : whether leading and trailing whitespace should be stripped from strings</p>
 
 <p><code>use_decimal</code>
-: whether non-integer numeric values should be inferred as Decimal (exact values) instead of float (non-exact values). Note that this only applies to methods that attempt to infer type (<code><a href="#TypeParser.infer">infer()</a></code> and <code>infer_*()</code>), and does not affect methods where the type is explicitly specified (<code><a href="#TypeParser.is_float">is_float()</a></code>, <code><a href="#TypeParser.is_decimal">is_decimal()</a></code>, <code><a href="#TypeParser.parse_float">parse_float()</a></code>, <code><a href="#TypeParser.parse_decimal">parse_decimal()</a></code>).</p>
+: whether non-integer numeric values should be inferred to be Decimal (exact values) instead of float (non-exact values). Note that this only applies to methods that attempt to infer type (<code><a href="#TypeParser.infer">infer()</a></code> and <code>infer_*()</code>), and does not affect methods where the type is explicitly specified (<code><a href="#TypeParser.is_float">is_float()</a></code>, <code><a href="#TypeParser.is_decimal">is_decimal()</a></code>, <code><a href="#TypeParser.parse_float">parse_float()</a></code>, <code><a href="#TypeParser.parse_decimal">parse_decimal()</a></code>).</p>
 
 <p><code>list_delimiter</code>
 : the delimiter used for identifying lists and for separating list items. If set to None, the parser will not attempt to identify lists when inferring types, which usually causes the value to be treated as a str instead.</p>
 
 <p><code>none_values</code>
 : list of strings that represent the value None</p>
 
@@ -2318,15 +2327,15 @@
 
                             </div>
                             <div id="TypeParser.infer" class="classattr">
                                         <input id="TypeParser.infer-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">infer</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">value</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="n">Type</span><span class="p">[</span><span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">,</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">NoneType</span><span class="p">,</span> <span class="n">Nullable</span><span class="p">,</span> <span class="nb">list</span><span class="p">]]</span>:</span></span>
+        <span class="name">infer</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">value</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="n">Type</span><span class="p">[</span><span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">,</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">NoneType</span><span class="p">,</span> <span class="n"><a href="#Nullable">Nullable</a></span><span class="p">,</span> <span class="nb">list</span><span class="p">]]</span>:</span></span>
 
 
                 <label class="view-source-button" for="TypeParser.infer-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#TypeParser.infer"></a>
             <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.infer-710"><a href="#TypeParser.infer-710"><span class="linenos">710</span></a>	<span class="k">def</span> <span class="nf">infer</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">AnyValueType</span><span class="p">:</span>
@@ -2408,15 +2417,15 @@
 
                             </div>
                             <div id="TypeParser.infer_series" class="classattr">
                                         <input id="TypeParser.infer_series-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">infer_series</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">values</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span></span><span class="return-annotation">) -> <span class="n">Type</span><span class="p">[</span><span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">,</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">NoneType</span><span class="p">,</span> <span class="n">Nullable</span><span class="p">,</span> <span class="nb">list</span><span class="p">]]</span>:</span></span>
+        <span class="name">infer_series</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">values</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span></span><span class="return-annotation">) -> <span class="n">Type</span><span class="p">[</span><span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">,</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">NoneType</span><span class="p">,</span> <span class="n"><a href="#Nullable">Nullable</a></span><span class="p">,</span> <span class="nb">list</span><span class="p">]]</span>:</span></span>
 
 
                 <label class="view-source-button" for="TypeParser.infer_series-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#TypeParser.infer_series"></a>
             <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.infer_series-760"><a href="#TypeParser.infer_series-760"><span class="linenos">760</span></a>	<span class="k">def</span> <span class="nf">infer_series</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="n">AnyValueType</span><span class="p">:</span>
@@ -2475,15 +2484,15 @@
 
                             </div>
                             <div id="TypeParser.infer_table" class="classattr">
                                         <input id="TypeParser.infer_table-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">infer_table</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">rows</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]]</span></span><span class="return-annotation">) -> <span class="nb">list</span><span class="p">[</span><span class="n">typing</span><span class="o">.</span><span class="n">Type</span><span class="p">[</span><span class="n">typing</span><span class="o">.</span><span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">,</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">NoneType</span><span class="p">,</span> <span class="n">Nullable</span><span class="p">,</span> <span class="nb">list</span><span class="p">]]]</span>:</span></span>
+        <span class="name">infer_table</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">rows</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]]</span></span><span class="return-annotation">) -> <span class="nb">list</span><span class="p">[</span><span class="n">typing</span><span class="o">.</span><span class="n">Type</span><span class="p">[</span><span class="n">typing</span><span class="o">.</span><span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">,</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">NoneType</span><span class="p">,</span> <span class="n"><a href="#Nullable">Nullable</a></span><span class="p">,</span> <span class="nb">list</span><span class="p">]]]</span>:</span></span>
 
 
                 <label class="view-source-button" for="TypeParser.infer_table-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#TypeParser.infer_table"></a>
             <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.infer_table-787"><a href="#TypeParser.infer_table-787"><span class="linenos">787</span></a>	<span class="k">def</span> <span class="nf">infer_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">rows</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">AnyValueType</span><span class="p">]:</span>
@@ -2565,15 +2574,15 @@
 
                             </div>
                             <div id="TypeParser.convert" class="classattr">
                                         <input id="TypeParser.convert-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">convert</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">value</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">target_type</span><span class="p">:</span> <span class="n">Type</span><span class="p">[</span><span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">,</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">NoneType</span><span class="p">,</span> <span class="n">Nullable</span><span class="p">,</span> <span class="nb">list</span><span class="p">]]</span></span><span class="return-annotation">) -> <span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">,</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">NoneType</span><span class="p">,</span> <span class="nb">list</span><span class="p">]</span>:</span></span>
+        <span class="name">convert</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">value</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">target_type</span><span class="p">:</span> <span class="n">Type</span><span class="p">[</span><span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">,</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">NoneType</span><span class="p">,</span> <span class="n"><a href="#Nullable">Nullable</a></span><span class="p">,</span> <span class="nb">list</span><span class="p">]]</span></span><span class="return-annotation">) -> <span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">,</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">NoneType</span><span class="p">,</span> <span class="nb">list</span><span class="p">]</span>:</span></span>
 
 
                 <label class="view-source-button" for="TypeParser.convert-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#TypeParser.convert"></a>
             <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.convert-832"><a href="#TypeParser.convert-832"><span class="linenos">832</span></a>	<span class="k">def</span> <span class="nf">convert</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">target_type</span><span class="p">:</span> <span class="n">AnyValueType</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">AnyValue</span><span class="p">:</span>
@@ -2624,15 +2633,15 @@
 </span><span id="TypeParser.convert-877"><a href="#TypeParser.convert-877"><span class="linenos">877</span></a>			<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_float</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
 </span><span id="TypeParser.convert-878"><a href="#TypeParser.convert-878"><span class="linenos">878</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">str</span><span class="p">:</span>
 </span><span id="TypeParser.convert-879"><a href="#TypeParser.convert-879"><span class="linenos">879</span></a>			<span class="k">return</span> <span class="n">value</span>
 </span><span id="TypeParser.convert-880"><a href="#TypeParser.convert-880"><span class="linenos">880</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="n">Nullable</span><span class="p">:</span>
 </span><span id="TypeParser.convert-881"><a href="#TypeParser.convert-881"><span class="linenos">881</span></a>			<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_none</span><span class="p">(</span><span class="n">value</span><span class="p">):</span>
 </span><span id="TypeParser.convert-882"><a href="#TypeParser.convert-882"><span class="linenos">882</span></a>				<span class="k">return</span> <span class="kc">None</span>
 </span><span id="TypeParser.convert-883"><a href="#TypeParser.convert-883"><span class="linenos">883</span></a>			<span class="k">else</span><span class="p">:</span>
-</span><span id="TypeParser.convert-884"><a href="#TypeParser.convert-884"><span class="linenos">884</span></a>				<span class="k">if</span> <span class="n">type_args</span> <span class="ow">is</span> <span class="ow">not</span>  <span class="kc">None</span> <span class="ow">and</span> <span class="nb">len</span><span class="p">(</span><span class="n">type_args</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span> <span class="ow">and</span> <span class="n">type_args</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">!=</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="TypeParser.convert-884"><a href="#TypeParser.convert-884"><span class="linenos">884</span></a>				<span class="k">if</span> <span class="n">type_args</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span> <span class="ow">and</span> <span class="nb">len</span><span class="p">(</span><span class="n">type_args</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span> <span class="ow">and</span> <span class="n">type_args</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">!=</span> <span class="nb">str</span><span class="p">:</span>
 </span><span id="TypeParser.convert-885"><a href="#TypeParser.convert-885"><span class="linenos">885</span></a>					<span class="n">inner_type</span> <span class="o">=</span> <span class="n">type_args</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
 </span><span id="TypeParser.convert-886"><a href="#TypeParser.convert-886"><span class="linenos">886</span></a>					<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">convert</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">inner_type</span><span class="p">)</span>
 </span><span id="TypeParser.convert-887"><a href="#TypeParser.convert-887"><span class="linenos">887</span></a>				<span class="k">else</span><span class="p">:</span>
 </span><span id="TypeParser.convert-888"><a href="#TypeParser.convert-888"><span class="linenos">888</span></a>					<span class="k">return</span> <span class="n">value</span>
 </span><span id="TypeParser.convert-889"><a href="#TypeParser.convert-889"><span class="linenos">889</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">list</span><span class="p">:</span>
 </span><span id="TypeParser.convert-890"><a href="#TypeParser.convert-890"><span class="linenos">890</span></a>			<span class="n">subvalues</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">list_delimiter</span><span class="p">)</span>
 </span><span id="TypeParser.convert-891"><a href="#TypeParser.convert-891"><span class="linenos">891</span></a>			<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">trim</span><span class="p">:</span>
@@ -3028,15 +3037,15 @@
                             </div>
                 </section>
                 <section id="reduce_types">
                             <input id="reduce_types-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">reduce_types</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="n">types</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Type</span><span class="p">[</span><span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">,</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">NoneType</span><span class="p">,</span> <span class="n">Nullable</span><span class="p">,</span> <span class="nb">list</span><span class="p">]]]</span></span><span class="return-annotation">) -> <span class="n">Type</span><span class="p">[</span><span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">,</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">NoneType</span><span class="p">,</span> <span class="n">Nullable</span><span class="p">,</span> <span class="nb">list</span><span class="p">]]</span>:</span></span>
+        <span class="name">reduce_types</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="n">types</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Type</span><span class="p">[</span><span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">,</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">NoneType</span><span class="p">,</span> <span class="n"><a href="#Nullable">Nullable</a></span><span class="p">,</span> <span class="nb">list</span><span class="p">]]]</span></span><span class="return-annotation">) -> <span class="n">Type</span><span class="p">[</span><span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">,</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">NoneType</span><span class="p">,</span> <span class="n"><a href="#Nullable">Nullable</a></span><span class="p">,</span> <span class="nb">list</span><span class="p">]]</span>:</span></span>
 
 
                 <label class="view-source-button" for="reduce_types-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#reduce_types"></a>
             <div class="pdoc-code codehilite"><pre><span></span><span id="reduce_types-156"><a href="#reduce_types-156"><span class="linenos">156</span></a><span class="k">def</span> <span class="nf">reduce_types</span><span class="p">(</span><span class="n">types</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">AnyValueType</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="n">AnyValueType</span><span class="p">:</span>
@@ -3105,10 +3114,90 @@
 <span class="n">reduce_types</span><span class="p">([</span><span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="nb">str</span><span class="p">])</span>   <span class="c1"># str</span>
 </code></pre>
 </div></div>
 
 
 
                 </section>
+                <section id="Nullable">
+                            <input id="Nullable-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+<div class="attr class">
+            
+    <span class="def">class</span>
+    <span class="name">Nullable</span><wbr>(<span class="base">typing.Generic[~S]</span>):
+
+
+                <label class="view-source-button" for="Nullable-view-source"><span>View Source</span></label>
+
+    </div>
+    <a class="headerlink" href="#Nullable"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Nullable-22"><a href="#Nullable-22"><span class="linenos">22</span></a><span class="k">class</span> <span class="nc">Nullable</span><span class="p">(</span><span class="n">Generic</span><span class="p">[</span><span class="n">S</span><span class="p">]):</span>
+</span><span id="Nullable-23"><a href="#Nullable-23"><span class="linenos">23</span></a><span class="w">	</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="Nullable-24"><a href="#Nullable-24"><span class="linenos">24</span></a><span class="sd">		Dummy container type that represents a scalar (`S`) that could also be None</span>
+</span><span id="Nullable-25"><a href="#Nullable-25"><span class="linenos">25</span></a>
+</span><span id="Nullable-26"><a href="#Nullable-26"><span class="linenos">26</span></a><span class="sd">		The type annotation `Nullable[S]` is treated as equivalent to `Union[S, types.NoneType]`, which will accept either a value of type `S` or the value `None`.</span>
+</span><span id="Nullable-27"><a href="#Nullable-27"><span class="linenos">27</span></a>
+</span><span id="Nullable-28"><a href="#Nullable-28"><span class="linenos">28</span></a><span class="sd">		This class should not be instantiated.</span>
+</span><span id="Nullable-29"><a href="#Nullable-29"><span class="linenos">29</span></a><span class="sd">	&quot;&quot;&quot;</span>
+</span><span id="Nullable-30"><a href="#Nullable-30"><span class="linenos">30</span></a>	<span class="k">pass</span>
+</span></pre></div>
+
+
+    <div class="docstring">
+<p>Dummy container type that represents a scalar (<code>S</code>) that could also be None</p>
+
+<p>The type annotation <code>Nullable[S]</code> is treated as equivalent to <code>Union[S, types.NoneType]</code>, which will accept either a value of type <code>S</code> or the value <code>None</code>.</p>
+
+<p>This class should not be instantiated.</p></div>
+
+
+
+                            <div id="Nullable.__init__" class="classattr">
+                                <div class="attr function">
+            
+        <span class="name">Nullable</span><span class="signature pdoc-code condensed">()</span>
+
+
+        
+    </div>
+    <a class="headerlink" href="#Nullable.__init__"></a>
+    
+    
+
+                            </div>
+                            <div class="inherited">
+                                <h5>Inherited Members</h5>
+                                <dl>
+                                    <div><dt>typing.Generic</dt>
+                                <dd id="Nullable.__class_getitem__" class="function">__class_getitem__</dd>
+                <dd id="Nullable.__init_subclass__" class="function">__init_subclass__</dd>
+
+            </div>
+            <div><dt>builtins.object</dt>
+                                <dd id="Nullable.__new__" class="function">__new__</dd>
+                <dd id="Nullable.__repr__" class="function">__repr__</dd>
+                <dd id="Nullable.__hash__" class="function">__hash__</dd>
+                <dd id="Nullable.__str__" class="function">__str__</dd>
+                <dd id="Nullable.__getattribute__" class="function">__getattribute__</dd>
+                <dd id="Nullable.__setattr__" class="function">__setattr__</dd>
+                <dd id="Nullable.__delattr__" class="function">__delattr__</dd>
+                <dd id="Nullable.__lt__" class="function">__lt__</dd>
+                <dd id="Nullable.__le__" class="function">__le__</dd>
+                <dd id="Nullable.__eq__" class="function">__eq__</dd>
+                <dd id="Nullable.__ne__" class="function">__ne__</dd>
+                <dd id="Nullable.__gt__" class="function">__gt__</dd>
+                <dd id="Nullable.__ge__" class="function">__ge__</dd>
+                <dd id="Nullable.__reduce_ex__" class="function">__reduce_ex__</dd>
+                <dd id="Nullable.__reduce__" class="function">__reduce__</dd>
+                <dd id="Nullable.__getstate__" class="function">__getstate__</dd>
+                <dd id="Nullable.__subclasshook__" class="function">__subclasshook__</dd>
+                <dd id="Nullable.__format__" class="function">__format__</dd>
+                <dd id="Nullable.__sizeof__" class="function">__sizeof__</dd>
+                <dd id="Nullable.__dir__" class="function">__dir__</dd>
+
+            </div>
+                                </dl>
+                            </div>
+                </section>
     </main>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -19,14 +19,16 @@
           o infer_table()
           o convert()
           o parse()
           o parse_series()
           o parse_table()
           o iterate_table()
     * reduce_types()
+    * Nullable
+          o Nullable
 built_with_pdoc[pdoc_logo]
    Edit_on_GitHub
 ****** parsetypes ******
 This package provides tools for parsing serialised data to recover their
 original underlying types.
 The TypeParser class provides configurable type inference and parsing. This can
 be initialised with different settings to, for example:
@@ -47,22 +49,22 @@
 _6
 - give exact Decimal values instead of floats
 _7
 - detect inline lists
 _8"""
 _9
 10
-11__version__ = "0.2.5"
+11__version__ = "0.2.6"
 12
 13from ._common import AnyScalar, AnyScalarType, AnyValue, AnyValueType,
 GenericValue, Nullable
 14from ._parser import TypeParser
 15from ._reduce_types import reduce_types
 16
-17__all__ = ('TypeParser', 'reduce_types')
+17__all__ = ('TypeParser', 'reduce_types', 'Nullable')
   ⁰
 class TypeParser: View Source
 __60class TypeParser:
 __61
 """
 __62
 A parser that can be used to infer the underlying types of data serialised as
@@ -120,15 +122,15 @@
 `trim`
 __89
 : whether leading and trailing whitespace should be stripped from strings
 __90
 __91
 `use_decimal`
 __92
-: whether non-integer numeric values should be inferred as Decimal (exact
+: whether non-integer numeric values should be inferred to be Decimal (exact
 values) instead of float (non-exact values). Note that this only applies to
 methods that attempt to infer type (`infer()` and `infer_*()`), and does not
 affect methods where the type is explicitly specified (`is_float()`,
 `is_decimal()`, `parse_float()`, `parse_decimal()`).
 __93
 __94
 `list_delimiter`
@@ -1661,15 +1663,15 @@
 _881
 if self.is_none(value):
 _882
 return None
 _883
 else:
 _884
-if type_args is not  None and len(type_args) == 1 and type_args[0] != str:
+if type_args is not None and len(type_args) == 1 and type_args[0] != str:
 _885
 inner_type = type_args[0]
 _886
 return self.convert(value, inner_type)
 _887
 else:
 _888
@@ -2022,15 +2024,15 @@
 `trim`
 _89
 : whether leading and trailing whitespace should be stripped from strings
 _90
 _91
 `use_decimal`
 _92
-: whether non-integer numeric values should be inferred as Decimal (exact
+: whether non-integer numeric values should be inferred to be Decimal (exact
 values) instead of float (non-exact values). Note that this only applies to
 methods that attempt to infer type (`infer()` and `infer_*()`), and does not
 affect methods where the type is explicitly specified (`is_float()`,
 `is_decimal()`, `parse_float()`, `parse_decimal()`).
 _93
 _94
 `list_delimiter`
@@ -2283,19 +2285,19 @@
 219
 ):
 220
 raise ValueError(f"cannot use float value as {name}: {special_value}")
 Initialise a new parser
 ***** Parameters *****
 trim : whether leading and trailing whitespace should be stripped from strings
-use_decimal : whether non-integer numeric values should be inferred as Decimal
-(exact values) instead of float (non-exact values). Note that this only applies
-to methods that attempt to infer type (infer() and infer_*()), and does not
-affect methods where the type is explicitly specified (is_float(), is_decimal
-(), parse_float(), parse_decimal()).
+use_decimal : whether non-integer numeric values should be inferred to be
+Decimal (exact values) instead of float (non-exact values). Note that this only
+applies to methods that attempt to infer type (infer() and infer_*()), and does
+not affect methods where the type is explicitly specified (is_float(),
+is_decimal(), parse_float(), parse_decimal()).
 list_delimiter : the delimiter used for identifying lists and for separating
 list items. If set to None, the parser will not attempt to identify lists when
 inferring types, which usually causes the value to be treated as a str instead.
 none_values : list of strings that represent the value None
 none_case_sensitive : whether matches against none_values should be made in a
 case-sensitive manner
 true_values : list of strings that represent the bool value True
@@ -3782,15 +3784,15 @@
 881
 if self.is_none(value):
 882
 return None
 883
 else:
 884
-if type_args is not  None and len(type_args) == 1 and type_args[0] != str:
+if type_args is not None and len(type_args) == 1 and type_args[0] != str:
 885
 inner_type = type_args[0]
 886
 return self.convert(value, inner_type)
 887
 else:
 888
@@ -4278,8 +4280,33 @@
 types : types to be reduced
 ***** Returns *****
 common reduced type
 ***** Examples *****
 reduce_types([int, float])        # float
 reduce_types([bool, int])         # int
 reduce_types([int, float, str])   # str
+  ⁰
+class Nullable(typing.Generic[~S]): View Source
+22class Nullable(Generic[S]):
+23
+"""
+24
+Dummy container type that represents a scalar (`S`) that could also be None
+25
+26
+The type annotation `Nullable[S]` is treated as equivalent to `Union[S,
+types.NoneType]`, which will accept either a value of type `S` or the value
+`None`.
+27
+28
+This class should not be instantiated.
+29
+"""
+30
+pass
+Dummy container type that represents a scalar (S) that could also be None
+The type annotation Nullable[S] is treated as equivalent to Union[S,
+types.NoneType], which will accept either a value of type S or the value None.
+This class should not be instantiated.
+Nullable()
+** Inherited Members **
```

### Comparing `parsetypes-0.2.5/docs/html/search.js` & `parsetypes-0.2.6/docs/html/search.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -702,15 +702,15 @@
                     "doc": "<p>A parser that can be used to infer the underlying types of data serialised as strings, and to convert them into their original underlying types.</p>\n\n<p>Instances of this class can be configured with different settings for the parser and inferrer. See the constructor for more details about the available options.</p>\n"
                 },
                 "parsetypes.TypeParser.__init__": {
                     "fullname": "parsetypes.TypeParser.__init__",
                     "modulename": "parsetypes",
                     "qualname": "TypeParser.__init__",
                     "kind": "function",
-                    "doc": "<p>Initialise a new parser</p>\n\n<h2 id=\"parameters\">Parameters</h2>\n\n<p><code>trim</code>\n: whether leading and trailing whitespace should be stripped from strings</p>\n\n<p><code>use_decimal</code>\n: whether non-integer numeric values should be inferred as Decimal (exact values) instead of float (non-exact values). Note that this only applies to methods that attempt to infer type (<code>infer()</code> and <code>infer_*()</code>), and does not affect methods where the type is explicitly specified (<code>is_float()</code>, <code>is_decimal()</code>, <code>parse_float()</code>, <code>parse_decimal()</code>).</p>\n\n<p><code>list_delimiter</code>\n: the delimiter used for identifying lists and for separating list items. If set to None, the parser will not attempt to identify lists when inferring types, which usually causes the value to be treated as a str instead.</p>\n\n<p><code>none_values</code>\n: list of strings that represent the value None</p>\n\n<p><code>none_case_sensitive</code>\n: whether matches against <code>none_values</code> should be made in a case-sensitive manner</p>\n\n<p><code>true_values</code>\n: list of strings that represent the bool value True</p>\n\n<p><code>false_values</code>\n: list of strings that represent the bool value False</p>\n\n<p><code>bool_case_sensitive</code>\n: whether matches against <code>true_values</code> and <code>false_values</code> should be made in a case-sensitive manner</p>\n\n<p><code>int_case_sensitive</code>\n: whether checks for int should be done in a case-sensitive manner. This usually only applies to values given in scientific notation, where the mantissa and exponent usually are separated by <code>e</code>.</p>\n\n<p><code>inf_values</code>\n: list of strings that represent the float or Decimal value of infinity. Each of the strings can be prepended with a negative sign to represent negative infinity also.</p>\n\n<p><code>nan_values</code>\n: list of strings that represent a float or Decimal that is NaN (not a number)</p>\n\n<p><code>float_case_sensitive</code>\n: whether checks for float should be done in a case-sensitive manner. This applies to matches against <code>inf_values</code> and <code>nan_values</code>, as well as to values given in scientific notation, where the mantissa and exponent are usually separated by <code>e</code>.</p>\n\n<p><code>case_sensitive</code>\n: whether all matches should be made in a case-sensitive manner. Sets all of <code>none_case_sensitive</code>, <code>bool_case_sensitive</code>, <code>int_case_sensitive</code>, <code>float_case_sensitive</code> to the same value, ignoring any individual settings.</p>\n\n<h2 id=\"raises\">Raises</h2>\n\n<p><code>ValueError</code> if any of the options would lead to ambiguities during parsing</p>\n",
+                    "doc": "<p>Initialise a new parser</p>\n\n<h2 id=\"parameters\">Parameters</h2>\n\n<p><code>trim</code>\n: whether leading and trailing whitespace should be stripped from strings</p>\n\n<p><code>use_decimal</code>\n: whether non-integer numeric values should be inferred to be Decimal (exact values) instead of float (non-exact values). Note that this only applies to methods that attempt to infer type (<code>infer()</code> and <code>infer_*()</code>), and does not affect methods where the type is explicitly specified (<code>is_float()</code>, <code>is_decimal()</code>, <code>parse_float()</code>, <code>parse_decimal()</code>).</p>\n\n<p><code>list_delimiter</code>\n: the delimiter used for identifying lists and for separating list items. If set to None, the parser will not attempt to identify lists when inferring types, which usually causes the value to be treated as a str instead.</p>\n\n<p><code>none_values</code>\n: list of strings that represent the value None</p>\n\n<p><code>none_case_sensitive</code>\n: whether matches against <code>none_values</code> should be made in a case-sensitive manner</p>\n\n<p><code>true_values</code>\n: list of strings that represent the bool value True</p>\n\n<p><code>false_values</code>\n: list of strings that represent the bool value False</p>\n\n<p><code>bool_case_sensitive</code>\n: whether matches against <code>true_values</code> and <code>false_values</code> should be made in a case-sensitive manner</p>\n\n<p><code>int_case_sensitive</code>\n: whether checks for int should be done in a case-sensitive manner. This usually only applies to values given in scientific notation, where the mantissa and exponent usually are separated by <code>e</code>.</p>\n\n<p><code>inf_values</code>\n: list of strings that represent the float or Decimal value of infinity. Each of the strings can be prepended with a negative sign to represent negative infinity also.</p>\n\n<p><code>nan_values</code>\n: list of strings that represent a float or Decimal that is NaN (not a number)</p>\n\n<p><code>float_case_sensitive</code>\n: whether checks for float should be done in a case-sensitive manner. This applies to matches against <code>inf_values</code> and <code>nan_values</code>, as well as to values given in scientific notation, where the mantissa and exponent are usually separated by <code>e</code>.</p>\n\n<p><code>case_sensitive</code>\n: whether all matches should be made in a case-sensitive manner. Sets all of <code>none_case_sensitive</code>, <code>bool_case_sensitive</code>, <code>int_case_sensitive</code>, <code>float_case_sensitive</code> to the same value, ignoring any individual settings.</p>\n\n<h2 id=\"raises\">Raises</h2>\n\n<p><code>ValueError</code> if any of the options would lead to ambiguities during parsing</p>\n",
                     "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"o\">*</span>,</span><span class=\"param\">\t<span class=\"n\">trim</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">True</span>,</span><span class=\"param\">\t<span class=\"n\">use_decimal</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">False</span>,</span><span class=\"param\">\t<span class=\"n\">list_delimiter</span><span class=\"p\">:</span> <span class=\"n\">Optional</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]</span> <span class=\"o\">=</span> <span class=\"kc\">None</span>,</span><span class=\"param\">\t<span class=\"n\">none_values</span><span class=\"p\">:</span> <span class=\"n\">Iterable</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]</span> <span class=\"o\">=</span> <span class=\"p\">[</span><span class=\"s1\">&#39;&#39;</span><span class=\"p\">]</span>,</span><span class=\"param\">\t<span class=\"n\">none_case_sensitive</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">False</span>,</span><span class=\"param\">\t<span class=\"n\">true_values</span><span class=\"p\">:</span> <span class=\"n\">Iterable</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]</span> <span class=\"o\">=</span> <span class=\"p\">[</span><span class=\"s1\">&#39;true&#39;</span><span class=\"p\">]</span>,</span><span class=\"param\">\t<span class=\"n\">false_values</span><span class=\"p\">:</span> <span class=\"n\">Iterable</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]</span> <span class=\"o\">=</span> <span class=\"p\">[</span><span class=\"s1\">&#39;false&#39;</span><span class=\"p\">]</span>,</span><span class=\"param\">\t<span class=\"n\">bool_case_sensitive</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">False</span>,</span><span class=\"param\">\t<span class=\"n\">int_case_sensitive</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">False</span>,</span><span class=\"param\">\t<span class=\"n\">inf_values</span><span class=\"p\">:</span> <span class=\"n\">Iterable</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]</span> <span class=\"o\">=</span> <span class=\"p\">[]</span>,</span><span class=\"param\">\t<span class=\"n\">nan_values</span><span class=\"p\">:</span> <span class=\"n\">Iterable</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]</span> <span class=\"o\">=</span> <span class=\"p\">[]</span>,</span><span class=\"param\">\t<span class=\"n\">float_case_sensitive</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">False</span>,</span><span class=\"param\">\t<span class=\"n\">case_sensitive</span><span class=\"p\">:</span> <span class=\"n\">Optional</span><span class=\"p\">[</span><span class=\"nb\">bool</span><span class=\"p\">]</span> <span class=\"o\">=</span> <span class=\"kc\">None</span></span>)</span>"
                 },
                 "parsetypes.TypeParser.is_none": {
                     "fullname": "parsetypes.TypeParser.is_none",
                     "modulename": "parsetypes",
                     "qualname": "TypeParser.is_none",
                     "kind": "function",
@@ -875,14 +875,30 @@
                     "fullname": "parsetypes.reduce_types",
                     "modulename": "parsetypes",
                     "qualname": "reduce_types",
                     "kind": "function",
                     "doc": "<p>Reduce multiple types into a single common type.</p>\n\n<p>If the input types are not all the same, the resulting type will be narrowest possible type that will encompass all of the input types.</p>\n\n<p>This operation is useful in cases such as parsing a CSV file where each column should have a consistent type, but where the individual values in a column could be interpreted variously as ints or floats (or other types).</p>\n\n<h2 id=\"parameters\">Parameters</h2>\n\n<p><code>types</code>\n: types to be reduced</p>\n\n<h2 id=\"returns\">Returns</h2>\n\n<p>common reduced type</p>\n\n<h2 id=\"examples\">Examples</h2>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"n\">reduce_types</span><span class=\"p\">([</span><span class=\"nb\">int</span><span class=\"p\">,</span> <span class=\"nb\">float</span><span class=\"p\">])</span>        <span class=\"c1\"># float</span>\n<span class=\"n\">reduce_types</span><span class=\"p\">([</span><span class=\"nb\">bool</span><span class=\"p\">,</span> <span class=\"nb\">int</span><span class=\"p\">])</span>         <span class=\"c1\"># int</span>\n<span class=\"n\">reduce_types</span><span class=\"p\">([</span><span class=\"nb\">int</span><span class=\"p\">,</span> <span class=\"nb\">float</span><span class=\"p\">,</span> <span class=\"nb\">str</span><span class=\"p\">])</span>   <span class=\"c1\"># str</span>\n</code></pre>\n</div>\n",
                     "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"n\">types</span><span class=\"p\">:</span> <span class=\"n\">Iterable</span><span class=\"p\">[</span><span class=\"n\">Type</span><span class=\"p\">[</span><span class=\"n\">Union</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">,</span> <span class=\"nb\">int</span><span class=\"p\">,</span> <span class=\"nb\">float</span><span class=\"p\">,</span> <span class=\"n\">decimal</span><span class=\"o\">.</span><span class=\"n\">Decimal</span><span class=\"p\">,</span> <span class=\"nb\">bool</span><span class=\"p\">,</span> <span class=\"n\">NoneType</span><span class=\"p\">,</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">,</span> <span class=\"nb\">list</span><span class=\"p\">]]]</span></span><span class=\"return-annotation\">) -> <span class=\"n\">Type</span><span class=\"p\">[</span><span class=\"n\">Union</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">,</span> <span class=\"nb\">int</span><span class=\"p\">,</span> <span class=\"nb\">float</span><span class=\"p\">,</span> <span class=\"n\">decimal</span><span class=\"o\">.</span><span class=\"n\">Decimal</span><span class=\"p\">,</span> <span class=\"nb\">bool</span><span class=\"p\">,</span> <span class=\"n\">NoneType</span><span class=\"p\">,</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">,</span> <span class=\"nb\">list</span><span class=\"p\">]]</span>:</span></span>",
                     "funcdef": "def"
+                },
+                "parsetypes.Nullable": {
+                    "fullname": "parsetypes.Nullable",
+                    "modulename": "parsetypes",
+                    "qualname": "Nullable",
+                    "kind": "class",
+                    "doc": "<p>Dummy container type that represents a scalar (<code>S</code>) that could also be None</p>\n\n<p>The type annotation <code>Nullable[S]</code> is treated as equivalent to <code>Union[S, types.NoneType]</code>, which will accept either a value of type <code>S</code> or the value <code>None</code>.</p>\n\n<p>This class should not be instantiated.</p>\n",
+                    "bases": "typing.Generic[~S]"
+                },
+                "parsetypes.Nullable.__init__": {
+                    "fullname": "parsetypes.Nullable.__init__",
+                    "modulename": "parsetypes",
+                    "qualname": "Nullable.__init__",
+                    "kind": "function",
+                    "doc": "<p></p>\n",
+                    "signature": "<span class=\"signature pdoc-code condensed\">()</span>"
                 }
             },
             "docInfo": {
                 "parsetypes": {
                     "qualname": 0,
                     "fullname": 1,
                     "annotation": 0,
@@ -903,15 +919,15 @@
                 "parsetypes.TypeParser.__init__": {
                     "qualname": 3,
                     "fullname": 4,
                     "annotation": 0,
                     "default_value": 0,
                     "signature": 325,
                     "bases": 0,
-                    "doc": 475
+                    "doc": 476
                 },
                 "parsetypes.TypeParser.is_none": {
                     "qualname": 3,
                     "fullname": 4,
                     "annotation": 0,
                     "default_value": 0,
                     "signature": 24,
@@ -1075,28 +1091,49 @@
                     "qualname": 2,
                     "fullname": 3,
                     "annotation": 0,
                     "default_value": 0,
                     "signature": 160,
                     "bases": 0,
                     "doc": 188
+                },
+                "parsetypes.Nullable": {
+                    "qualname": 1,
+                    "fullname": 2,
+                    "annotation": 0,
+                    "default_value": 0,
+                    "signature": 0,
+                    "bases": 2,
+                    "doc": 62
+                },
+                "parsetypes.Nullable.__init__": {
+                    "qualname": 3,
+                    "fullname": 4,
+                    "annotation": 0,
+                    "default_value": 0,
+                    "signature": 4,
+                    "bases": 0,
+                    "doc": 3
                 }
             },
-            "length": 22,
+            "length": 24,
             "save": true
         },
         "index": {
             "qualname": {
                 "root": {
                     "docs": {
                         "parsetypes.TypeParser.__init__": {
                             "tf": 1
+                        },
+                        "parsetypes.Nullable.__init__": {
+                            "tf": 1
                         }
                     },
-                    "df": 1,
+                    "df": 2,
                     "t": {
                         "docs": {},
                         "df": 0,
                         "y": {
                             "docs": {},
                             "df": 0,
                             "p": {
@@ -1237,17 +1274,20 @@
                             "i": {
                                 "docs": {},
                                 "df": 0,
                                 "t": {
                                     "docs": {
                                         "parsetypes.TypeParser.__init__": {
                                             "tf": 1
+                                        },
+                                        "parsetypes.Nullable.__init__": {
+                                            "tf": 1
                                         }
                                     },
-                                    "df": 1
+                                    "df": 2
                                 }
                             },
                             "t": {
                                 "docs": {
                                     "parsetypes.TypeParser.is_int": {
                                         "tf": 1
                                     },
@@ -1346,14 +1386,49 @@
                                         "parsetypes.TypeParser.parse_none": {
                                             "tf": 1
                                         }
                                     },
                                     "df": 2
                                 }
                             }
+                        },
+                        "u": {
+                            "docs": {},
+                            "df": 0,
+                            "l": {
+                                "docs": {},
+                                "df": 0,
+                                "l": {
+                                    "docs": {},
+                                    "df": 0,
+                                    "a": {
+                                        "docs": {},
+                                        "df": 0,
+                                        "b": {
+                                            "docs": {},
+                                            "df": 0,
+                                            "l": {
+                                                "docs": {},
+                                                "df": 0,
+                                                "e": {
+                                                    "docs": {
+                                                        "parsetypes.Nullable": {
+                                                            "tf": 1
+                                                        },
+                                                        "parsetypes.Nullable.__init__": {
+                                                            "tf": 1
+                                                        }
+                                                    },
+                                                    "df": 2
+                                                }
+                                            }
+                                        }
+                                    }
+                                }
+                            }
                         }
                     },
                     "b": {
                         "docs": {},
                         "df": 0,
                         "o": {
                             "docs": {},
@@ -1576,17 +1651,20 @@
                 }
             },
             "fullname": {
                 "root": {
                     "docs": {
                         "parsetypes.TypeParser.__init__": {
                             "tf": 1
+                        },
+                        "parsetypes.Nullable.__init__": {
+                            "tf": 1
                         }
                     },
-                    "df": 1,
+                    "df": 2,
                     "p": {
                         "docs": {},
                         "df": 0,
                         "a": {
                             "docs": {},
                             "df": 0,
                             "r": {
@@ -1698,17 +1776,23 @@
                                                                     "tf": 1
                                                                 },
                                                                 "parsetypes.TypeParser.iterate_table": {
                                                                     "tf": 1
                                                                 },
                                                                 "parsetypes.reduce_types": {
                                                                     "tf": 1
+                                                                },
+                                                                "parsetypes.Nullable": {
+                                                                    "tf": 1
+                                                                },
+                                                                "parsetypes.Nullable.__init__": {
+                                                                    "tf": 1
                                                                 }
                                                             },
-                                                            "df": 22
+                                                            "df": 24
                                                         }
                                                     }
                                                 }
                                             }
                                         }
                                     }
                                 }
@@ -1859,17 +1943,20 @@
                             "i": {
                                 "docs": {},
                                 "df": 0,
                                 "t": {
                                     "docs": {
                                         "parsetypes.TypeParser.__init__": {
                                             "tf": 1
+                                        },
+                                        "parsetypes.Nullable.__init__": {
+                                            "tf": 1
                                         }
                                     },
-                                    "df": 1
+                                    "df": 2
                                 }
                             },
                             "t": {
                                 "docs": {
                                     "parsetypes.TypeParser.is_int": {
                                         "tf": 1
                                     },
@@ -1968,14 +2055,49 @@
                                         "parsetypes.TypeParser.parse_none": {
                                             "tf": 1
                                         }
                                     },
                                     "df": 2
                                 }
                             }
+                        },
+                        "u": {
+                            "docs": {},
+                            "df": 0,
+                            "l": {
+                                "docs": {},
+                                "df": 0,
+                                "l": {
+                                    "docs": {},
+                                    "df": 0,
+                                    "a": {
+                                        "docs": {},
+                                        "df": 0,
+                                        "b": {
+                                            "docs": {},
+                                            "df": 0,
+                                            "l": {
+                                                "docs": {},
+                                                "df": 0,
+                                                "e": {
+                                                    "docs": {
+                                                        "parsetypes.Nullable": {
+                                                            "tf": 1
+                                                        },
+                                                        "parsetypes.Nullable.__init__": {
+                                                            "tf": 1
+                                                        }
+                                                    },
+                                                    "df": 2
+                                                }
+                                            }
+                                        }
+                                    }
+                                }
+                            }
                         }
                     },
                     "b": {
                         "docs": {},
                         "df": 0,
                         "o": {
                             "docs": {},
@@ -2234,17 +2356,20 @@
                             "tf": 8.888194417315589
                         },
                         "parsetypes.TypeParser.iterate_table": {
                             "tf": 8.660254037844387
                         },
                         "parsetypes.reduce_types": {
                             "tf": 11.489125293076057
+                        },
+                        "parsetypes.Nullable.__init__": {
+                            "tf": 2
                         }
                     },
-                    "df": 20,
+                    "df": 21,
                     "t": {
                         "docs": {},
                         "df": 0,
                         "r": {
                             "docs": {},
                             "df": 0,
                             "i": {
@@ -3586,15 +3711,87 @@
                         }
                     }
                 }
             },
             "bases": {
                 "root": {
                     "docs": {},
-                    "df": 0
+                    "df": 0,
+                    "t": {
+                        "docs": {},
+                        "df": 0,
+                        "y": {
+                            "docs": {},
+                            "df": 0,
+                            "p": {
+                                "docs": {},
+                                "df": 0,
+                                "i": {
+                                    "docs": {},
+                                    "df": 0,
+                                    "n": {
+                                        "docs": {},
+                                        "df": 0,
+                                        "g": {
+                                            "docs": {
+                                                "parsetypes.Nullable": {
+                                                    "tf": 1
+                                                }
+                                            },
+                                            "df": 1
+                                        }
+                                    }
+                                }
+                            }
+                        }
+                    },
+                    "g": {
+                        "docs": {},
+                        "df": 0,
+                        "e": {
+                            "docs": {},
+                            "df": 0,
+                            "n": {
+                                "docs": {},
+                                "df": 0,
+                                "e": {
+                                    "docs": {},
+                                    "df": 0,
+                                    "r": {
+                                        "docs": {},
+                                        "df": 0,
+                                        "i": {
+                                            "docs": {},
+                                            "df": 0,
+                                            "c": {
+                                                "docs": {},
+                                                "df": 0,
+                                                "[": {
+                                                    "docs": {},
+                                                    "df": 0,
+                                                    "~": {
+                                                        "docs": {},
+                                                        "df": 0,
+                                                        "s": {
+                                                            "docs": {
+                                                                "parsetypes.Nullable": {
+                                                                    "tf": 1
+                                                                }
+                                                            },
+                                                            "df": 1
+                                                        }
+                                                    }
+                                                }
+                                            }
+                                        }
+                                    }
+                                }
+                            }
+                        }
+                    }
                 }
             },
             "doc": {
                 "root": {
                     "0": {
                         "1": {
                             "2": {
@@ -3970,17 +4167,23 @@
                             "tf": 16.06237840420901
                         },
                         "parsetypes.TypeParser.iterate_table": {
                             "tf": 15.524174696260024
                         },
                         "parsetypes.reduce_types": {
                             "tf": 9.433981132056603
+                        },
+                        "parsetypes.Nullable": {
+                            "tf": 4.242640687119285
+                        },
+                        "parsetypes.Nullable.__init__": {
+                            "tf": 1.7320508075688772
                         }
                     },
-                    "df": 22,
+                    "df": 24,
                     "t": {
                         "docs": {},
                         "df": 0,
                         "h": {
                             "docs": {},
                             "df": 0,
                             "i": {
@@ -4022,17 +4225,20 @@
                                             "tf": 1.4142135623730951
                                         },
                                         "parsetypes.TypeParser.iterate_table": {
                                             "tf": 1.4142135623730951
                                         },
                                         "parsetypes.reduce_types": {
                                             "tf": 1
+                                        },
+                                        "parsetypes.Nullable": {
+                                            "tf": 1
                                         }
                                     },
-                                    "df": 13
+                                    "df": 14
                                 }
                             },
                             "e": {
                                 "docs": {
                                     "parsetypes": {
                                         "tf": 1
                                     },
@@ -4091,17 +4297,20 @@
                                         "tf": 4.242640687119285
                                     },
                                     "parsetypes.TypeParser.iterate_table": {
                                         "tf": 3.4641016151377544
                                     },
                                     "parsetypes.reduce_types": {
                                         "tf": 2.23606797749979
+                                    },
+                                    "parsetypes.Nullable": {
+                                        "tf": 1.4142135623730951
                                     }
                                 },
-                                "df": 21,
+                                "df": 22,
                                 "i": {
                                     "docs": {},
                                     "df": 0,
                                     "r": {
                                         "docs": {
                                             "parsetypes": {
                                                 "tf": 1
@@ -4190,30 +4399,33 @@
                                             "tf": 2.449489742783178
                                         },
                                         "parsetypes.TypeParser.iterate_table": {
                                             "tf": 2
                                         },
                                         "parsetypes.reduce_types": {
                                             "tf": 1
+                                        },
+                                        "parsetypes.Nullable": {
+                                            "tf": 1.4142135623730951
                                         }
                                     },
-                                    "df": 17
+                                    "df": 18
                                 }
                             }
                         },
                         "o": {
                             "docs": {
                                 "parsetypes": {
                                     "tf": 1.4142135623730951
                                 },
                                 "parsetypes.TypeParser": {
                                     "tf": 1.4142135623730951
                                 },
                                 "parsetypes.TypeParser.__init__": {
-                                    "tf": 3.3166247903554
+                                    "tf": 3.4641016151377544
                                 },
                                 "parsetypes.TypeParser.is_none": {
                                     "tf": 1
                                 },
                                 "parsetypes.TypeParser.is_bool": {
                                     "tf": 1
                                 },
@@ -4254,17 +4466,20 @@
                                     "tf": 2.449489742783178
                                 },
                                 "parsetypes.TypeParser.iterate_table": {
                                     "tf": 1.7320508075688772
                                 },
                                 "parsetypes.reduce_types": {
                                     "tf": 1
+                                },
+                                "parsetypes.Nullable": {
+                                    "tf": 1
                                 }
                             },
-                            "df": 19,
+                            "df": 20,
                             "o": {
                                 "docs": {},
                                 "df": 0,
                                 "l": {
                                     "docs": {},
                                     "df": 0,
                                     "s": {
@@ -4314,17 +4529,20 @@
                                             "tf": 2.6457513110645907
                                         },
                                         "parsetypes.TypeParser.iterate_table": {
                                             "tf": 2.23606797749979
                                         },
                                         "parsetypes.reduce_types": {
                                             "tf": 2.23606797749979
+                                        },
+                                        "parsetypes.Nullable": {
+                                            "tf": 1.7320508075688772
                                         }
                                     },
-                                    "df": 11,
+                                    "df": 12,
                                     "s": {
                                         "docs": {
                                             "parsetypes": {
                                                 "tf": 1
                                             },
                                             "parsetypes.TypeParser": {
                                                 "tf": 1.4142135623730951
@@ -4345,17 +4563,20 @@
                                                 "tf": 1.4142135623730951
                                             },
                                             "parsetypes.TypeParser.iterate_table": {
                                                 "tf": 1.4142135623730951
                                             },
                                             "parsetypes.reduce_types": {
                                                 "tf": 3
+                                            },
+                                            "parsetypes.Nullable": {
+                                                "tf": 1
                                             }
                                         },
-                                        "df": 9
+                                        "df": 10
                                     },
                                     "p": {
                                         "docs": {},
                                         "df": 0,
                                         "a": {
                                             "docs": {},
                                             "df": 0,
@@ -4478,17 +4699,20 @@
                                         "e": {
                                             "docs": {},
                                             "df": 0,
                                             "d": {
                                                 "docs": {
                                                     "parsetypes.TypeParser.__init__": {
                                                         "tf": 1
+                                                    },
+                                                    "parsetypes.Nullable": {
+                                                        "tf": 1
                                                     }
                                                 },
-                                                "df": 1
+                                                "df": 2
                                             }
                                         }
                                     }
                                 }
                             },
                             "i": {
                                 "docs": {},
@@ -5451,16 +5675,20 @@
                                     },
                                     "df": 1
                                 }
                             }
                         }
                     },
                     "s": {
-                        "docs": {},
-                        "df": 0,
+                        "docs": {
+                            "parsetypes.Nullable": {
+                                "tf": 1.4142135623730951
+                            }
+                        },
+                        "df": 1,
                         "e": {
                             "docs": {},
                             "df": 0,
                             "r": {
                                 "docs": {},
                                 "df": 0,
                                 "i": {
@@ -5953,17 +6181,20 @@
                                                     "tf": 1
                                                 },
                                                 "parsetypes.TypeParser.parse_table": {
                                                     "tf": 1.4142135623730951
                                                 },
                                                 "parsetypes.reduce_types": {
                                                     "tf": 1
+                                                },
+                                                "parsetypes.Nullable": {
+                                                    "tf": 1
                                                 }
                                             },
-                                            "df": 7
+                                            "df": 8
                                         }
                                     }
                                 }
                             }
                         },
                         "p": {
                             "docs": {},
@@ -6053,14 +6284,34 @@
                                                         }
                                                     }
                                                 }
                                             }
                                         }
                                     }
                                 }
+                            },
+                            "a": {
+                                "docs": {},
+                                "df": 0,
+                                "l": {
+                                    "docs": {},
+                                    "df": 0,
+                                    "a": {
+                                        "docs": {},
+                                        "df": 0,
+                                        "r": {
+                                            "docs": {
+                                                "parsetypes.Nullable": {
+                                                    "tf": 1
+                                                }
+                                            },
+                                            "df": 1
+                                        }
+                                    }
+                                }
                             }
                         },
                         "i": {
                             "docs": {},
                             "df": 0,
                             "g": {
                                 "docs": {},
@@ -6553,14 +6804,30 @@
                                                     "tf": 1
                                                 }
                                             },
                                             "df": 1
                                         }
                                     }
                                 }
+                            },
+                            "m": {
+                                "docs": {},
+                                "df": 0,
+                                "m": {
+                                    "docs": {},
+                                    "df": 0,
+                                    "y": {
+                                        "docs": {
+                                            "parsetypes.Nullable": {
+                                                "tf": 1
+                                            }
+                                        },
+                                        "df": 1
+                                    }
+                                }
                             }
                         }
                     },
                     "r": {
                         "docs": {},
                         "df": 0,
                         "e": {
@@ -6633,17 +6900,20 @@
                                                                     "tf": 1
                                                                 },
                                                                 "parsetypes.TypeParser.parse_float": {
                                                                     "tf": 1.4142135623730951
                                                                 },
                                                                 "parsetypes.TypeParser.parse_decimal": {
                                                                     "tf": 1.4142135623730951
+                                                                },
+                                                                "parsetypes.Nullable": {
+                                                                    "tf": 1
                                                                 }
                                                             },
-                                                            "df": 7
+                                                            "df": 8
                                                         },
                                                         "a": {
                                                             "docs": {},
                                                             "df": 0,
                                                             "t": {
                                                                 "docs": {},
                                                                 "df": 0,
@@ -7040,17 +7310,20 @@
                                     "tf": 1
                                 },
                                 "parsetypes.TypeParser.convert": {
                                     "tf": 1
                                 },
                                 "parsetypes.reduce_types": {
                                     "tf": 1.4142135623730951
+                                },
+                                "parsetypes.Nullable": {
+                                    "tf": 1
                                 }
                             },
-                            "df": 7,
+                            "df": 8,
                             "i": {
                                 "docs": {},
                                 "df": 0,
                                 "g": {
                                     "docs": {},
                                     "df": 0,
                                     "i": {
@@ -7158,17 +7431,20 @@
                                     "tf": 2.8284271247461903
                                 },
                                 "parsetypes.TypeParser.iterate_table": {
                                     "tf": 2.449489742783178
                                 },
                                 "parsetypes.reduce_types": {
                                     "tf": 1
+                                },
+                                "parsetypes.Nullable": {
+                                    "tf": 1
                                 }
                             },
-                            "df": 20
+                            "df": 21
                         },
                         "p": {
                             "docs": {},
                             "df": 0,
                             "t": {
                                 "docs": {},
                                 "df": 0,
@@ -7384,14 +7660,38 @@
                                                         }
                                                     }
                                                 }
                                             }
                                         }
                                     }
                                 }
+                            },
+                            "i": {
+                                "docs": {},
+                                "df": 0,
+                                "o": {
+                                    "docs": {},
+                                    "df": 0,
+                                    "n": {
+                                        "docs": {},
+                                        "df": 0,
+                                        "[": {
+                                            "docs": {},
+                                            "df": 0,
+                                            "s": {
+                                                "docs": {
+                                                    "parsetypes.Nullable": {
+                                                        "tf": 1
+                                                    }
+                                                },
+                                                "df": 1
+                                            }
+                                        }
+                                    }
+                                }
                             }
                         },
                         "s": {
                             "docs": {},
                             "df": 0,
                             "e": {
                                 "docs": {
@@ -7472,17 +7772,20 @@
                                     "s": {
                                         "docs": {
                                             "parsetypes": {
                                                 "tf": 1
                                             },
                                             "parsetypes.TypeParser": {
                                                 "tf": 1
+                                            },
+                                            "parsetypes.Nullable": {
+                                                "tf": 1
                                             }
                                         },
-                                        "df": 2
+                                        "df": 3
                                     }
                                 }
                             }
                         },
                         "o": {
                             "docs": {},
                             "df": 0,
@@ -7668,14 +7971,42 @@
                                                             "df": 1
                                                         }
                                                     }
                                                 }
                                             }
                                         }
                                     }
+                                },
+                                "t": {
+                                    "docs": {},
+                                    "df": 0,
+                                    "a": {
+                                        "docs": {},
+                                        "df": 0,
+                                        "i": {
+                                            "docs": {},
+                                            "df": 0,
+                                            "n": {
+                                                "docs": {},
+                                                "df": 0,
+                                                "e": {
+                                                    "docs": {},
+                                                    "df": 0,
+                                                    "r": {
+                                                        "docs": {
+                                                            "parsetypes.Nullable": {
+                                                                "tf": 1
+                                                            }
+                                                        },
+                                                        "df": 1
+                                                    }
+                                                }
+                                            }
+                                        }
+                                    }
                                 }
                             },
                             "m": {
                                 "docs": {},
                                 "df": 0,
                                 "m": {
                                     "docs": {},
@@ -7779,17 +8110,20 @@
                                 "l": {
                                     "docs": {},
                                     "df": 0,
                                     "d": {
                                         "docs": {
                                             "parsetypes.reduce_types": {
                                                 "tf": 1
+                                            },
+                                            "parsetypes.Nullable": {
+                                                "tf": 1
                                             }
                                         },
-                                        "df": 1
+                                        "df": 2
                                     }
                                 }
                             }
                         },
                         "a": {
                             "docs": {},
                             "df": 0,
@@ -8390,14 +8724,42 @@
                                                             "parsetypes.TypeParser": {
                                                                 "tf": 1
                                                             }
                                                         },
                                                         "df": 1
                                                     }
                                                 }
+                                            },
+                                            "t": {
+                                                "docs": {},
+                                                "df": 0,
+                                                "i": {
+                                                    "docs": {},
+                                                    "df": 0,
+                                                    "a": {
+                                                        "docs": {},
+                                                        "df": 0,
+                                                        "t": {
+                                                            "docs": {},
+                                                            "df": 0,
+                                                            "e": {
+                                                                "docs": {},
+                                                                "df": 0,
+                                                                "d": {
+                                                                    "docs": {
+                                                                        "parsetypes.Nullable": {
+                                                                            "tf": 1
+                                                                        }
+                                                                    },
+                                                                    "df": 1
+                                                                }
+                                                            }
+                                                        }
+                                                    }
+                                                }
                                             }
                                         }
                                     }
                                 }
                             },
                             "l": {
                                 "docs": {},
@@ -8742,17 +9104,20 @@
                                     "tf": 2.23606797749979
                                 },
                                 "parsetypes.TypeParser.iterate_table": {
                                     "tf": 2
                                 },
                                 "parsetypes.reduce_types": {
                                     "tf": 1
+                                },
+                                "parsetypes.Nullable": {
+                                    "tf": 1
                                 }
                             },
-                            "df": 17
+                            "df": 18
                         },
                         "d": {
                             "docs": {},
                             "df": 0,
                             "e": {
                                 "docs": {},
                                 "df": 0,
@@ -9078,17 +9443,20 @@
                                 "tf": 2.449489742783178
                             },
                             "parsetypes.TypeParser.iterate_table": {
                                 "tf": 2.23606797749979
                             },
                             "parsetypes.reduce_types": {
                                 "tf": 2
+                            },
+                            "parsetypes.Nullable": {
+                                "tf": 1.4142135623730951
                             }
                         },
-                        "df": 21,
+                        "df": 22,
                         "n": {
                             "docs": {
                                 "parsetypes.TypeParser.is_none": {
                                     "tf": 1
                                 },
                                 "parsetypes.TypeParser.is_int": {
                                     "tf": 2
@@ -9221,26 +9589,62 @@
                                                         }
                                                     }
                                                 }
                                             }
                                         }
                                     }
                                 }
+                            },
+                            "n": {
+                                "docs": {},
+                                "df": 0,
+                                "o": {
+                                    "docs": {},
+                                    "df": 0,
+                                    "t": {
+                                        "docs": {},
+                                        "df": 0,
+                                        "a": {
+                                            "docs": {},
+                                            "df": 0,
+                                            "t": {
+                                                "docs": {},
+                                                "df": 0,
+                                                "i": {
+                                                    "docs": {},
+                                                    "df": 0,
+                                                    "o": {
+                                                        "docs": {},
+                                                        "df": 0,
+                                                        "n": {
+                                                            "docs": {
+                                                                "parsetypes.Nullable": {
+                                                                    "tf": 1
+                                                                }
+                                                            },
+                                                            "df": 1
+                                                        }
+                                                    }
+                                                }
+                                            }
+                                        }
+                                    }
+                                }
                             }
                         },
                         "s": {
                             "docs": {
                                 "parsetypes": {
                                     "tf": 1
                                 },
                                 "parsetypes.TypeParser": {
                                     "tf": 1
                                 },
                                 "parsetypes.TypeParser.__init__": {
-                                    "tf": 2
+                                    "tf": 1.7320508075688772
                                 },
                                 "parsetypes.TypeParser.is_none": {
                                     "tf": 1
                                 },
                                 "parsetypes.TypeParser.is_bool": {
                                     "tf": 1
                                 },
@@ -9272,17 +9676,20 @@
                                     "tf": 2
                                 },
                                 "parsetypes.TypeParser.iterate_table": {
                                     "tf": 1.4142135623730951
                                 },
                                 "parsetypes.reduce_types": {
                                     "tf": 1.4142135623730951
+                                },
+                                "parsetypes.Nullable": {
+                                    "tf": 1
                                 }
                             },
-                            "df": 16,
+                            "df": 17,
                             "s": {
                                 "docs": {},
                                 "df": 0,
                                 "e": {
                                     "docs": {},
                                     "df": 0,
                                     "r": {
@@ -9629,17 +10036,20 @@
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser.parse_decimal": {
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser.infer": {
                                             "tf": 1
+                                        },
+                                        "parsetypes.Nullable": {
+                                            "tf": 1
                                         }
                                     },
-                                    "df": 6
+                                    "df": 7
                                 }
                             },
                             "l": {
                                 "docs": {
                                     "parsetypes.TypeParser.__init__": {
                                         "tf": 1.4142135623730951
                                     },
@@ -9804,17 +10214,20 @@
                                                     "tf": 1
                                                 },
                                                 "parsetypes.TypeParser.parse_float": {
                                                     "tf": 1.7320508075688772
                                                 },
                                                 "parsetypes.TypeParser.parse_decimal": {
                                                     "tf": 1.7320508075688772
+                                                },
+                                                "parsetypes.Nullable": {
+                                                    "tf": 1
                                                 }
                                             },
-                                            "df": 5,
+                                            "df": 6,
                                             "e": {
                                                 "docs": {},
                                                 "df": 0,
                                                 "d": {
                                                     "docs": {
                                                         "parsetypes.TypeParser.is_none": {
                                                             "tf": 1
@@ -9898,15 +10311,15 @@
                                 "parsetypes": {
                                     "tf": 1
                                 },
                                 "parsetypes.TypeParser": {
                                     "tf": 1.4142135623730951
                                 },
                                 "parsetypes.TypeParser.__init__": {
-                                    "tf": 3
+                                    "tf": 3.1622776601683795
                                 },
                                 "parsetypes.TypeParser.is_none": {
                                     "tf": 1.4142135623730951
                                 },
                                 "parsetypes.TypeParser.is_bool": {
                                     "tf": 1.4142135623730951
                                 },
@@ -9953,17 +10366,20 @@
                                     "tf": 2.23606797749979
                                 },
                                 "parsetypes.TypeParser.iterate_table": {
                                     "tf": 1.7320508075688772
                                 },
                                 "parsetypes.reduce_types": {
                                     "tf": 1.7320508075688772
+                                },
+                                "parsetypes.Nullable": {
+                                    "tf": 1.4142135623730951
                                 }
                             },
-                            "df": 21,
+                            "df": 22,
                             "h": {
                                 "docs": {},
                                 "df": 0,
                                 "a": {
                                     "docs": {},
                                     "df": 0,
                                     "v": {
@@ -10195,17 +10611,20 @@
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser.iterate_table": {
                                             "tf": 1
                                         },
                                         "parsetypes.reduce_types": {
                                             "tf": 1.4142135623730951
+                                        },
+                                        "parsetypes.Nullable": {
+                                            "tf": 1
                                         }
                                     },
-                                    "df": 16
+                                    "df": 17
                                 }
                             }
                         },
                         "h": {
                             "docs": {},
                             "df": 0,
                             "e": {
@@ -10374,17 +10793,20 @@
                                                 "tf": 1
                                             },
                                             "parsetypes.TypeParser.parse_table": {
                                                 "tf": 1.4142135623730951
                                             },
                                             "parsetypes.TypeParser.iterate_table": {
                                                 "tf": 1
+                                            },
+                                            "parsetypes.Nullable": {
+                                                "tf": 1
                                             }
                                         },
-                                        "df": 14
+                                        "df": 15
                                     }
                                 }
                             }
                         },
                         "e": {
                             "docs": {},
                             "df": 0,
@@ -10724,17 +11146,20 @@
                                     "e": {
                                         "docs": {},
                                         "df": 0,
                                         "r": {
                                             "docs": {
                                                 "parsetypes": {
                                                     "tf": 1
+                                                },
+                                                "parsetypes.Nullable": {
+                                                    "tf": 1
                                                 }
                                             },
-                                            "df": 1
+                                            "df": 2
                                         }
                                     }
                                 }
                             }
                         },
                         "a": {
                             "docs": {},
@@ -10888,16 +11313,20 @@
                                                 "e": {
                                                     "docs": {},
                                                     "df": 0,
                                                     "n": {
                                                         "docs": {},
                                                         "df": 0,
                                                         "t": {
-                                                            "docs": {},
-                                                            "df": 0,
+                                                            "docs": {
+                                                                "parsetypes.Nullable": {
+                                                                    "tf": 1
+                                                                }
+                                                            },
+                                                            "df": 1,
                                                             "l": {
                                                                 "docs": {},
                                                                 "df": 0,
                                                                 "y": {
                                                                     "docs": {
                                                                         "parsetypes.TypeParser.is_float": {
                                                                             "tf": 1
@@ -11050,17 +11479,40 @@
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser.parse_series": {
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser.parse_table": {
                                             "tf": 1
+                                        },
+                                        "parsetypes.Nullable": {
+                                            "tf": 1.4142135623730951
                                         }
                                     },
-                                    "df": 6
+                                    "df": 7,
+                                    "t": {
+                                        "docs": {},
+                                        "df": 0,
+                                        "y": {
+                                            "docs": {},
+                                            "df": 0,
+                                            "p": {
+                                                "docs": {},
+                                                "df": 0,
+                                                "e": {
+                                                    "docs": {
+                                                        "parsetypes.Nullable": {
+                                                            "tf": 1
+                                                        }
+                                                    },
+                                                    "df": 1
+                                                }
+                                            }
+                                        }
+                                    }
                                 }
                             },
                             "t": {
                                 "docs": {
                                     "parsetypes.TypeParser.__init__": {
                                         "tf": 1.7320508075688772
                                     },
@@ -11092,17 +11544,20 @@
                                         "tf": 1
                                     },
                                     "parsetypes.TypeParser.iterate_table": {
                                         "tf": 1
                                     },
                                     "parsetypes.reduce_types": {
                                         "tf": 1
+                                    },
+                                    "parsetypes.Nullable": {
+                                        "tf": 1
                                     }
                                 },
-                                "df": 12,
+                                "df": 13,
                                 "e": {
                                     "docs": {
                                         "parsetypes.TypeParser.__init__": {
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser.is_int": {
                                             "tf": 1
@@ -11286,14 +11741,50 @@
                                                     "tf": 1
                                                 }
                                             },
                                             "df": 4
                                         }
                                     }
                                 }
+                            },
+                            "l": {
+                                "docs": {},
+                                "df": 0,
+                                "l": {
+                                    "docs": {},
+                                    "df": 0,
+                                    "a": {
+                                        "docs": {},
+                                        "df": 0,
+                                        "b": {
+                                            "docs": {},
+                                            "df": 0,
+                                            "l": {
+                                                "docs": {},
+                                                "df": 0,
+                                                "e": {
+                                                    "docs": {},
+                                                    "df": 0,
+                                                    "[": {
+                                                        "docs": {},
+                                                        "df": 0,
+                                                        "s": {
+                                                            "docs": {
+                                                                "parsetypes.Nullable": {
+                                                                    "tf": 1
+                                                                }
+                                                            },
+                                                            "df": 1
+                                                        }
+                                                    }
+                                                }
+                                            }
+                                        }
+                                    }
+                                }
                             }
                         },
                         "a": {
                             "docs": {},
                             "df": 0,
                             "n": {
                                 "docs": {
@@ -11485,17 +11976,20 @@
                                                 "tf": 1.4142135623730951
                                             },
                                             "parsetypes.TypeParser.parse_table": {
                                                 "tf": 1.4142135623730951
                                             },
                                             "parsetypes.TypeParser.iterate_table": {
                                                 "tf": 1.4142135623730951
+                                            },
+                                            "parsetypes.Nullable": {
+                                                "tf": 1.4142135623730951
                                             }
                                         },
-                                        "df": 16,
+                                        "df": 17,
                                         "s": {
                                             "docs": {
                                                 "parsetypes": {
                                                     "tf": 1
                                                 },
                                                 "parsetypes.TypeParser.__init__": {
                                                     "tf": 3.872983346207417
```

### Comparing `parsetypes-0.2.5/pyproject.toml` & `parsetypes-0.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `parsetypes-0.2.5/src/parsetypes/__init__.py` & `parsetypes-0.2.6/src/parsetypes/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 	The `TypeParser` class provides configurable type inference and parsing. This can be initialised with different settings to, for example:
 	- treat `inf` as either a float or a normal string
 	- give exact Decimal values instead of floats
 	- detect inline lists
 """
 
 
-__version__ = "0.2.5"
+__version__ = "0.2.6"
 
 from ._common import AnyScalar, AnyScalarType, AnyValue, AnyValueType, GenericValue, Nullable
 from ._parser import TypeParser
 from ._reduce_types import reduce_types
 
-__all__ = ('TypeParser', 'reduce_types')
+__all__ = ('TypeParser', 'reduce_types', 'Nullable')
```

### Comparing `parsetypes-0.2.5/src/parsetypes/_common.py` & `parsetypes-0.2.6/src/parsetypes/_common.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 
 
 class Nullable(Generic[S]):
 	"""
 		Dummy container type that represents a scalar (`S`) that could also be None
 
 		The type annotation `Nullable[S]` is treated as equivalent to `Union[S, types.NoneType]`, which will accept either a value of type `S` or the value `None`.
+
+		This class should not be instantiated.
 	"""
 	pass
 
 
 AnyContainerBase: TypeAlias = Union[Nullable, list]
 AnyContainerBaseType: TypeAlias = Type[AnyContainerBase]
```

### Comparing `parsetypes-0.2.5/src/parsetypes/_parser.py` & `parsetypes-0.2.6/src/parsetypes/_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
 			Parameters
 			----------
 			`trim`
 			: whether leading and trailing whitespace should be stripped from strings
 
 			`use_decimal`
-			: whether non-integer numeric values should be inferred as Decimal (exact values) instead of float (non-exact values). Note that this only applies to methods that attempt to infer type (`infer()` and `infer_*()`), and does not affect methods where the type is explicitly specified (`is_float()`, `is_decimal()`, `parse_float()`, `parse_decimal()`).
+			: whether non-integer numeric values should be inferred to be Decimal (exact values) instead of float (non-exact values). Note that this only applies to methods that attempt to infer type (`infer()` and `infer_*()`), and does not affect methods where the type is explicitly specified (`is_float()`, `is_decimal()`, `parse_float()`, `parse_decimal()`).
 
 			`list_delimiter`
 			: the delimiter used for identifying lists and for separating list items. If set to None, the parser will not attempt to identify lists when inferring types, which usually causes the value to be treated as a str instead.
 
 			`none_values`
 			: list of strings that represent the value None
 
@@ -876,15 +876,15 @@
 			return self.parse_float(value)
 		elif base == str:
 			return value
 		elif base == Nullable:
 			if self.is_none(value):
 				return None
 			else:
-				if type_args is not  None and len(type_args) == 1 and type_args[0] != str:
+				if type_args is not None and len(type_args) == 1 and type_args[0] != str:
 					inner_type = type_args[0]
 					return self.convert(value, inner_type)
 				else:
 					return value
 		elif base == list:
 			subvalues = value.split(self.list_delimiter)
 			if self.trim:
```

### Comparing `parsetypes-0.2.5/src/parsetypes/_reduce_types.py` & `parsetypes-0.2.6/src/parsetypes/_reduce_types.py`

 * *Files identical despite different names*

### Comparing `parsetypes-0.2.5/src/parsetypes.egg-info/PKG-INFO` & `parsetypes-0.2.6/src/parsetypes.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsetypes
-Version: 0.2.5
+Version: 0.2.6
 Summary: Parse serialised data to recover their original underlying types
 Author-email: Yu Shiyang <yu.shiyang@gnayihs.uy>
 License: MPL-2.0
 Project-URL: Homepage, https://github.com/yushiyangk/parsetypes
 Project-URL: Documentation, https://parsetypes.gnayihs.uy/
 Project-URL: Issues, https://github.com/yushiyangk/parsetypes/issues
 Keywords: python,str,string,types,conversion
@@ -158,14 +158,18 @@
 
 ## Changelog
 
 This project follows [PEP 440](https://peps.python.org/pep-0440/) and [Semantic Versioning (SemVer)](https://semver.org/spec/v2.0.0.html). In addition to the guarantees specified by SemVer, for versions before 1.0, this project guarantees backwards compatibility of the API for patch version updates (0.<var>y</var>.<b><var>z</var></b>).
 
 The recommended version specifier is <code>parsetypes ~= <var>x</var>.<var>y</var></code> for version 1.0 and later, and <code>parsetypes ~= <var>0</var>.<var>y</var>.<var>z</var></code> for versions prior to 1.0.
 
+### 0.2.6
+
+- Added `Nullable` to automatic imports via `from parsetypes import *` (previously only `TypeParser` and `reduce_types` were imported)
+
 ### 0.2.5
 
 - Fixed documentation
 
 ### 0.2.4
 
 - Added <code><var>parser</var>.convert()</code>
```

### Comparing `parsetypes-0.2.5/src/parsetypes.egg-info/SOURCES.txt` & `parsetypes-0.2.6/src/parsetypes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `parsetypes-0.2.5/tests/test_parser.py` & `parsetypes-0.2.6/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `parsetypes-0.2.5/tests/test_reduce_types.py` & `parsetypes-0.2.6/tests/test_reduce_types.py`

 * *Files identical despite different names*

