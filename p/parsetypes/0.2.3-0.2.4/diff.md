# Comparing `tmp/parsetypes-0.2.3.tar.gz` & `tmp/parsetypes-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsetypes-0.2.3.tar", last modified: Sun May 28 05:49:15 2023, max compression
+gzip compressed data, was "parsetypes-0.2.4.tar", last modified: Sun May 28 23:01:21 2023, max compression
```

## Comparing `parsetypes-0.2.3.tar` & `parsetypes-0.2.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 05:49:15.966756 parsetypes-0.2.3/
--rw-rw-rw-   0        0        0      798 2023-05-28 05:48:36.000000 parsetypes-0.2.3/CHANGELOG.md
--rw-rw-rw-   0        0        0       22 2023-05-28 02:54:36.000000 parsetypes-0.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0     6617 2023-05-28 05:49:15.966756 parsetypes-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     4114 2023-05-28 05:48:36.000000 parsetypes-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 05:49:15.950755 parsetypes-0.2.3/docs/
-drwxrwxrwx   0        0        0        0 2023-05-28 05:49:15.957754 parsetypes-0.2.3/docs/html/
--rw-rw-rw-   0        0        0     1729 2023-05-28 05:49:06.000000 parsetypes-0.2.3/docs/html/favicon.png
--rw-rw-rw-   0        0        0      141 2023-05-28 05:49:06.000000 parsetypes-0.2.3/docs/html/index.html
--rw-rw-rw-   0        0        0   502932 2023-05-28 05:49:06.000000 parsetypes-0.2.3/docs/html/parsetypes.html
--rw-rw-rw-   0        0        0   208714 2023-05-28 05:49:06.000000 parsetypes-0.2.3/docs/html/search.js
--rw-rw-rw-   0        0        0     2297 2023-05-28 04:48:55.000000 parsetypes-0.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-28 05:49:15.966756 parsetypes-0.2.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-28 05:49:15.951756 parsetypes-0.2.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-28 05:49:15.961755 parsetypes-0.2.3/src/parsetypes/
--rw-rw-rw-   0        0        0      621 2023-05-28 05:43:14.000000 parsetypes-0.2.3/src/parsetypes/__init__.py
--rw-rw-rw-   0        0        0     1254 2023-05-28 05:37:03.000000 parsetypes-0.2.3/src/parsetypes/_common.py
--rw-rw-rw-   0        0        0      348 2023-05-28 04:48:55.000000 parsetypes-0.2.3/src/parsetypes/_compat.py
--rw-rw-rw-   0        0        0    34554 2023-05-28 05:32:22.000000 parsetypes-0.2.3/src/parsetypes/_parser.py
--rw-rw-rw-   0        0        0     5203 2023-05-28 05:32:22.000000 parsetypes-0.2.3/src/parsetypes/_reduce_types.py
-drwxrwxrwx   0        0        0        0 2023-05-28 05:49:15.964755 parsetypes-0.2.3/src/parsetypes.egg-info/
--rw-rw-rw-   0        0        0     6617 2023-05-28 05:49:15.000000 parsetypes-0.2.3/src/parsetypes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      512 2023-05-28 05:49:15.000000 parsetypes-0.2.3/src/parsetypes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 05:49:15.000000 parsetypes-0.2.3/src/parsetypes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      296 2023-05-28 05:49:15.000000 parsetypes-0.2.3/src/parsetypes.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-28 05:49:15.000000 parsetypes-0.2.3/src/parsetypes.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-28 05:49:15.965758 parsetypes-0.2.3/tests/
--rw-rw-rw-   0        0        0    60176 2023-05-28 04:48:55.000000 parsetypes-0.2.3/tests/test_parser.py
--rw-rw-rw-   0        0        0     8837 2023-05-28 04:48:55.000000 parsetypes-0.2.3/tests/test_reduce_types.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:01:21.080304 parsetypes-0.2.4/
+-rw-rw-rw-   0        0        0      863 2023-05-28 23:00:42.000000 parsetypes-0.2.4/CHANGELOG.md
+-rw-rw-rw-   0        0        0       22 2023-05-28 02:54:36.000000 parsetypes-0.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     6751 2023-05-28 23:01:21.080304 parsetypes-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4183 2023-05-28 23:00:42.000000 parsetypes-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 23:01:21.066302 parsetypes-0.2.4/docs/
+drwxrwxrwx   0        0        0        0 2023-05-28 23:01:21.072307 parsetypes-0.2.4/docs/html/
+-rw-rw-rw-   0        0        0     1729 2023-05-28 23:01:12.000000 parsetypes-0.2.4/docs/html/favicon.png
+-rw-rw-rw-   0        0        0      141 2023-05-28 23:01:11.000000 parsetypes-0.2.4/docs/html/index.html
+-rw-rw-rw-   0        0        0   529187 2023-05-28 23:01:11.000000 parsetypes-0.2.4/docs/html/parsetypes.html
+-rw-rw-rw-   0        0        0   217429 2023-05-28 23:01:12.000000 parsetypes-0.2.4/docs/html/search.js
+-rw-rw-rw-   0        0        0     2297 2023-05-28 04:48:55.000000 parsetypes-0.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-28 23:01:21.081303 parsetypes-0.2.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-28 23:01:21.067305 parsetypes-0.2.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-28 23:01:21.075305 parsetypes-0.2.4/src/parsetypes/
+-rw-rw-rw-   0        0        0      621 2023-05-28 23:00:42.000000 parsetypes-0.2.4/src/parsetypes/__init__.py
+-rw-rw-rw-   0        0        0     1254 2023-05-28 05:37:03.000000 parsetypes-0.2.4/src/parsetypes/_common.py
+-rw-rw-rw-   0        0        0      348 2023-05-28 04:48:55.000000 parsetypes-0.2.4/src/parsetypes/_compat.py
+-rw-rw-rw-   0        0        0    35474 2023-05-28 23:00:42.000000 parsetypes-0.2.4/src/parsetypes/_parser.py
+-rw-rw-rw-   0        0        0     5203 2023-05-28 05:32:22.000000 parsetypes-0.2.4/src/parsetypes/_reduce_types.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:01:21.078306 parsetypes-0.2.4/src/parsetypes.egg-info/
+-rw-rw-rw-   0        0        0     6751 2023-05-28 23:01:21.000000 parsetypes-0.2.4/src/parsetypes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2023-05-28 23:01:21.000000 parsetypes-0.2.4/src/parsetypes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 23:01:21.000000 parsetypes-0.2.4/src/parsetypes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      296 2023-05-28 23:01:21.000000 parsetypes-0.2.4/src/parsetypes.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-28 23:01:21.000000 parsetypes-0.2.4/src/parsetypes.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 23:01:21.079304 parsetypes-0.2.4/tests/
+-rw-rw-rw-   0        0        0    67890 2023-05-28 23:00:42.000000 parsetypes-0.2.4/tests/test_parser.py
+-rw-rw-rw-   0        0        0     8837 2023-05-28 04:48:55.000000 parsetypes-0.2.4/tests/test_reduce_types.py
```

### Comparing `parsetypes-0.2.3/CHANGELOG.md` & `parsetypes-0.2.4/CHANGELOG.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 ## Changelog
 
 This project follows [PEP 440](https://peps.python.org/pep-0440/) and [Semantic Versioning (SemVer)](https://semver.org/spec/v2.0.0.html). In addition to the guarantees specified by SemVer, for versions before 1.0, this project guarantees backwards compatibility of the API for patch version updates (0.<var>y</var>.<b><var>z</var></b>).
 
 The recommended version specifier is <code>parsetypes ~= <var>x</var>.<var>y</var></code> for version 1.0 and later, and <code>parsetypes ~= <var>0</var>.<var>y</var>.<var>z</var></code> for versions prior to 1.0.
 
+### 0.2.4
+
+- Added <code><var>parser</var>.convert()</code>
+
 ### 0.2.1, 0.2.2 and 0.2.3
 
 - Fixed documentation
 
 ### 0.2
 
 - Added support for Python version 3.9; previously only 3.10 and 3.11 were supported
```

### Comparing `parsetypes-0.2.3/PKG-INFO` & `parsetypes-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsetypes
-Version: 0.2.3
+Version: 0.2.4
 Summary: Parse serialised data to recover their original underlying types
 Author-email: Yu Shiyang <yu.shiyang@gnayihs.uy>
 License: MPL-2.0
 Project-URL: Homepage, https://github.com/yushiyangk/parsetypes
 Project-URL: Documentation, https://parsetypes.gnayihs.uy/
 Project-URL: Issues, https://github.com/yushiyangk/parsetypes/issues
 Keywords: python,str,string,types,conversion
@@ -42,15 +42,15 @@
 
 This Python package provides tools for parsing serialised data to recover their original underlying types.
 
 [![](https://img.shields.io/badge/PyPI--inactive?style=social&logo=pypi)](https://pypi.org/project/parsetypes/) [![](https://img.shields.io/badge/GitHub--inactive?style=social&logo=github)](https://github.com/yushiyangk/parsetypes) [![](https://img.shields.io/badge/Documentation--inactive?style=social&logo=readthedocs)](https://parsetypes.gnayihs.uy/)
 
 ## Overview
 
-The `TypeParser` class provides configurable type inference and parsing. This can be initialised with different settings to, for example:
+The `TypeParser` class provides configurable type inference and parsing. This can be [initialised with different settings](https://parsetypes.gnayihs.uy/parsetypes.html#TypeParser.__init__) to, for example:
 - treat `inf` as either a float or a normal string
 - give exact Decimal values instead of floats
 - detect inline lists
 
 ## Install
 
 ```
@@ -158,14 +158,18 @@
 
 ## Changelog
 
 This project follows [PEP 440](https://peps.python.org/pep-0440/) and [Semantic Versioning (SemVer)](https://semver.org/spec/v2.0.0.html). In addition to the guarantees specified by SemVer, for versions before 1.0, this project guarantees backwards compatibility of the API for patch version updates (0.<var>y</var>.<b><var>z</var></b>).
 
 The recommended version specifier is <code>parsetypes ~= <var>x</var>.<var>y</var></code> for version 1.0 and later, and <code>parsetypes ~= <var>0</var>.<var>y</var>.<var>z</var></code> for versions prior to 1.0.
 
+### 0.2.4
+
+- Added <code><var>parser</var>.convert()</code>
+
 ### 0.2.1, 0.2.2 and 0.2.3
 
 - Fixed documentation
 
 ### 0.2
 
 - Added support for Python version 3.9; previously only 3.10 and 3.11 were supported
```

### Comparing `parsetypes-0.2.3/README.md` & `parsetypes-0.2.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 This Python package provides tools for parsing serialised data to recover their original underlying types.
 
 [![](https://img.shields.io/badge/PyPI--inactive?style=social&logo=pypi)](https://pypi.org/project/parsetypes/) [![](https://img.shields.io/badge/GitHub--inactive?style=social&logo=github)](https://github.com/yushiyangk/parsetypes) [![](https://img.shields.io/badge/Documentation--inactive?style=social&logo=readthedocs)](https://parsetypes.gnayihs.uy/)
 
 ## Overview
 
-The `TypeParser` class provides configurable type inference and parsing. This can be initialised with different settings to, for example:
+The `TypeParser` class provides configurable type inference and parsing. This can be [initialised with different settings](https://parsetypes.gnayihs.uy/parsetypes.html#TypeParser.__init__) to, for example:
 - treat `inf` as either a float or a normal string
 - give exact Decimal values instead of floats
 - detect inline lists
 
 ## Install
 
 ```
```

### Comparing `parsetypes-0.2.3/docs/html/favicon.png` & `parsetypes-0.2.4/docs/html/favicon.png`

 * *Files identical despite different names*

### Comparing `parsetypes-0.2.3/docs/html/parsetypes.html` & `parsetypes-0.2.4/docs/html/parsetypes.html`

 * *Files 2% similar despite different names*

```diff
@@ -141,14 +141,17 @@
             			<li>
             						<a class="function" href="#TypeParser.infer_series">infer_series<span class="decorator">()</span></a>
             			</li>
             			<li>
             						<a class="function" href="#TypeParser.infer_table">infer_table<span class="decorator">()</span></a>
             			</li>
             			<li>
+            						<a class="function" href="#TypeParser.convert">convert<span class="decorator">()</span></a>
+            			</li>
+            			<li>
             						<a class="function" href="#TypeParser.parse">parse<span class="decorator">()</span></a>
             			</li>
             			<li>
             						<a class="function" href="#TypeParser.parse_series">parse_series<span class="decorator">()</span></a>
             			</li>
             			<li>
             						<a class="function" href="#TypeParser.parse_table">parse_table<span class="decorator">()</span></a>
@@ -201,15 +204,15 @@
 </span><span id="L-4"><a href="#L-4"><span class="linenos"> 4</span></a><span class="sd">	The `TypeParser` class provides configurable type inference and parsing. This can be initialised with different settings to, for example:</span>
 </span><span id="L-5"><a href="#L-5"><span class="linenos"> 5</span></a><span class="sd">	- treat `inf` as either a float or a normal string</span>
 </span><span id="L-6"><a href="#L-6"><span class="linenos"> 6</span></a><span class="sd">	- give exact Decimal values instead of floats</span>
 </span><span id="L-7"><a href="#L-7"><span class="linenos"> 7</span></a><span class="sd">	- detect inline lists</span>
 </span><span id="L-8"><a href="#L-8"><span class="linenos"> 8</span></a><span class="sd">&quot;&quot;&quot;</span>
 </span><span id="L-9"><a href="#L-9"><span class="linenos"> 9</span></a>
 </span><span id="L-10"><a href="#L-10"><span class="linenos">10</span></a>
-</span><span id="L-11"><a href="#L-11"><span class="linenos">11</span></a><span class="n">__version__</span> <span class="o">=</span> <span class="s2">&quot;0.2.3&quot;</span>
+</span><span id="L-11"><a href="#L-11"><span class="linenos">11</span></a><span class="n">__version__</span> <span class="o">=</span> <span class="s2">&quot;0.2.4&quot;</span>
 </span><span id="L-12"><a href="#L-12"><span class="linenos">12</span></a>
 </span><span id="L-13"><a href="#L-13"><span class="linenos">13</span></a><span class="kn">from</span> <span class="nn">._common</span> <span class="kn">import</span> <span class="n">AnyScalar</span><span class="p">,</span> <span class="n">AnyScalarType</span><span class="p">,</span> <span class="n">AnyValue</span><span class="p">,</span> <span class="n">AnyValueType</span><span class="p">,</span> <span class="n">GenericValue</span><span class="p">,</span> <span class="n">Nullable</span>
 </span><span id="L-14"><a href="#L-14"><span class="linenos">14</span></a><span class="kn">from</span> <span class="nn">._parser</span> <span class="kn">import</span> <span class="n">TypeParser</span>
 </span><span id="L-15"><a href="#L-15"><span class="linenos">15</span></a><span class="kn">from</span> <span class="nn">._reduce_types</span> <span class="kn">import</span> <span class="n">reduce_types</span>
 </span><span id="L-16"><a href="#L-16"><span class="linenos">16</span></a>
 </span><span id="L-17"><a href="#L-17"><span class="linenos">17</span></a><span class="n">__all__</span> <span class="o">=</span> <span class="p">(</span><span class="s1">&#39;TypeParser&#39;</span><span class="p">,</span> <span class="s1">&#39;reduce_types&#39;</span><span class="p">)</span>
 </span></pre></div>
@@ -224,952 +227,986 @@
     <span class="name">TypeParser</span>:
 
 
                 <label class="view-source-button" for="TypeParser-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#TypeParser"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser-60"><a href="#TypeParser-60"><span class="linenos"> 60</span></a><span class="k">class</span> <span class="nc">TypeParser</span><span class="p">:</span>
-</span><span id="TypeParser-61"><a href="#TypeParser-61"><span class="linenos"> 61</span></a><span class="w">	</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser-62"><a href="#TypeParser-62"><span class="linenos"> 62</span></a><span class="sd">		A parser that can be used to infer the underlying types of data serialised as strings, and to convert them into their original underlying types.</span>
-</span><span id="TypeParser-63"><a href="#TypeParser-63"><span class="linenos"> 63</span></a>
-</span><span id="TypeParser-64"><a href="#TypeParser-64"><span class="linenos"> 64</span></a><span class="sd">		Instances of this class can be configured with different settings for the parser and inferrer. See the constructor for more details about the available options.</span>
-</span><span id="TypeParser-65"><a href="#TypeParser-65"><span class="linenos"> 65</span></a><span class="sd">	&quot;&quot;&quot;</span>
-</span><span id="TypeParser-66"><a href="#TypeParser-66"><span class="linenos"> 66</span></a>
-</span><span id="TypeParser-67"><a href="#TypeParser-67"><span class="linenos"> 67</span></a>	<span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span>
-</span><span id="TypeParser-68"><a href="#TypeParser-68"><span class="linenos"> 68</span></a>	    <span class="o">*</span><span class="p">,</span>
-</span><span id="TypeParser-69"><a href="#TypeParser-69"><span class="linenos"> 69</span></a>		<span class="n">trim</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
-</span><span id="TypeParser-70"><a href="#TypeParser-70"><span class="linenos"> 70</span></a>		<span class="n">use_decimal</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">False</span><span class="p">,</span>
-</span><span id="TypeParser-71"><a href="#TypeParser-71"><span class="linenos"> 71</span></a>		<span class="n">list_delimiter</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
-</span><span id="TypeParser-72"><a href="#TypeParser-72"><span class="linenos"> 72</span></a>		<span class="n">none_values</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span><span class="o">=</span><span class="p">[</span><span class="s2">&quot;&quot;</span><span class="p">],</span>
-</span><span id="TypeParser-73"><a href="#TypeParser-73"><span class="linenos"> 73</span></a>		<span class="n">none_case_sensitive</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">False</span><span class="p">,</span>
-</span><span id="TypeParser-74"><a href="#TypeParser-74"><span class="linenos"> 74</span></a>		<span class="n">true_values</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span><span class="o">=</span><span class="p">[</span><span class="s2">&quot;true&quot;</span><span class="p">],</span>
-</span><span id="TypeParser-75"><a href="#TypeParser-75"><span class="linenos"> 75</span></a>		<span class="n">false_values</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span><span class="o">=</span><span class="p">[</span><span class="s2">&quot;false&quot;</span><span class="p">],</span>
-</span><span id="TypeParser-76"><a href="#TypeParser-76"><span class="linenos"> 76</span></a>		<span class="n">bool_case_sensitive</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">False</span><span class="p">,</span>
-</span><span id="TypeParser-77"><a href="#TypeParser-77"><span class="linenos"> 77</span></a>		<span class="n">int_case_sensitive</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">False</span><span class="p">,</span>
-</span><span id="TypeParser-78"><a href="#TypeParser-78"><span class="linenos"> 78</span></a>		<span class="n">inf_values</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span><span class="o">=</span><span class="p">[],</span>
-</span><span id="TypeParser-79"><a href="#TypeParser-79"><span class="linenos"> 79</span></a>		<span class="n">nan_values</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span><span class="o">=</span><span class="p">[],</span>
-</span><span id="TypeParser-80"><a href="#TypeParser-80"><span class="linenos"> 80</span></a>		<span class="n">float_case_sensitive</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">False</span><span class="p">,</span>
-</span><span id="TypeParser-81"><a href="#TypeParser-81"><span class="linenos"> 81</span></a>		<span class="n">case_sensitive</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">bool</span><span class="p">]</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
-</span><span id="TypeParser-82"><a href="#TypeParser-82"><span class="linenos"> 82</span></a>	<span class="p">):</span>
-</span><span id="TypeParser-83"><a href="#TypeParser-83"><span class="linenos"> 83</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser-84"><a href="#TypeParser-84"><span class="linenos"> 84</span></a><span class="sd">			Initialise a new parser</span>
-</span><span id="TypeParser-85"><a href="#TypeParser-85"><span class="linenos"> 85</span></a>
-</span><span id="TypeParser-86"><a href="#TypeParser-86"><span class="linenos"> 86</span></a><span class="sd">			Parameters</span>
-</span><span id="TypeParser-87"><a href="#TypeParser-87"><span class="linenos"> 87</span></a><span class="sd">			----------</span>
-</span><span id="TypeParser-88"><a href="#TypeParser-88"><span class="linenos"> 88</span></a><span class="sd">			`trim`</span>
-</span><span id="TypeParser-89"><a href="#TypeParser-89"><span class="linenos"> 89</span></a><span class="sd">			: whether leading and trailing whitespace should be stripped from strings</span>
-</span><span id="TypeParser-90"><a href="#TypeParser-90"><span class="linenos"> 90</span></a>
-</span><span id="TypeParser-91"><a href="#TypeParser-91"><span class="linenos"> 91</span></a><span class="sd">			`use_decimal`</span>
-</span><span id="TypeParser-92"><a href="#TypeParser-92"><span class="linenos"> 92</span></a><span class="sd">			: whether non-integer numeric values should be inferred as Decimal (exact values) instead of float (non-exact values). Note that this only applies to methods that attempt to infer type (`infer()` and `infer_*()`), and does not affect methods where the type is explicitly specified (`is_float()`, `is_decimal()`, `parse_float()`, `parse_decimal()`).</span>
-</span><span id="TypeParser-93"><a href="#TypeParser-93"><span class="linenos"> 93</span></a>
-</span><span id="TypeParser-94"><a href="#TypeParser-94"><span class="linenos"> 94</span></a><span class="sd">			`list_delimiter`</span>
-</span><span id="TypeParser-95"><a href="#TypeParser-95"><span class="linenos"> 95</span></a><span class="sd">			: the delimiter used for identifying lists and for separating list items. If set to None, the parser will not attempt to identify lists when inferring types, which usually causes the value to be treated as a str instead.</span>
-</span><span id="TypeParser-96"><a href="#TypeParser-96"><span class="linenos"> 96</span></a>
-</span><span id="TypeParser-97"><a href="#TypeParser-97"><span class="linenos"> 97</span></a><span class="sd">			`none_values`</span>
-</span><span id="TypeParser-98"><a href="#TypeParser-98"><span class="linenos"> 98</span></a><span class="sd">			: list of strings that represent the value None</span>
-</span><span id="TypeParser-99"><a href="#TypeParser-99"><span class="linenos"> 99</span></a>
-</span><span id="TypeParser-100"><a href="#TypeParser-100"><span class="linenos">100</span></a><span class="sd">			`none_case_sensitive`</span>
-</span><span id="TypeParser-101"><a href="#TypeParser-101"><span class="linenos">101</span></a><span class="sd">			: whether matches against `none_values` should be made in a case-sensitive manner</span>
-</span><span id="TypeParser-102"><a href="#TypeParser-102"><span class="linenos">102</span></a>
-</span><span id="TypeParser-103"><a href="#TypeParser-103"><span class="linenos">103</span></a><span class="sd">			`true_values`</span>
-</span><span id="TypeParser-104"><a href="#TypeParser-104"><span class="linenos">104</span></a><span class="sd">			: list of strings that represent the bool value True</span>
-</span><span id="TypeParser-105"><a href="#TypeParser-105"><span class="linenos">105</span></a>
-</span><span id="TypeParser-106"><a href="#TypeParser-106"><span class="linenos">106</span></a><span class="sd">			`false_values`</span>
-</span><span id="TypeParser-107"><a href="#TypeParser-107"><span class="linenos">107</span></a><span class="sd">			: list of strings that represent the bool value False</span>
-</span><span id="TypeParser-108"><a href="#TypeParser-108"><span class="linenos">108</span></a>
-</span><span id="TypeParser-109"><a href="#TypeParser-109"><span class="linenos">109</span></a><span class="sd">			`bool_case_sensitive`</span>
-</span><span id="TypeParser-110"><a href="#TypeParser-110"><span class="linenos">110</span></a><span class="sd">			: whether matches against `true_values` and `false_values` should be made in a case-sensitive manner</span>
-</span><span id="TypeParser-111"><a href="#TypeParser-111"><span class="linenos">111</span></a>
-</span><span id="TypeParser-112"><a href="#TypeParser-112"><span class="linenos">112</span></a><span class="sd">			`int_case_sensitive`</span>
-</span><span id="TypeParser-113"><a href="#TypeParser-113"><span class="linenos">113</span></a><span class="sd">			: whether checks for int should be done in a case-sensitive manner. This usually only applies to values given in scientific notation, where the mantissa and exponent usually are separated by `e`.</span>
-</span><span id="TypeParser-114"><a href="#TypeParser-114"><span class="linenos">114</span></a>
-</span><span id="TypeParser-115"><a href="#TypeParser-115"><span class="linenos">115</span></a><span class="sd">			`inf_values`</span>
-</span><span id="TypeParser-116"><a href="#TypeParser-116"><span class="linenos">116</span></a><span class="sd">			: list of strings that represent the float or Decimal value of infinity. Each of the strings can be prepended with a negative sign to represent negative infinity also.</span>
-</span><span id="TypeParser-117"><a href="#TypeParser-117"><span class="linenos">117</span></a>
-</span><span id="TypeParser-118"><a href="#TypeParser-118"><span class="linenos">118</span></a><span class="sd">			`nan_values`</span>
-</span><span id="TypeParser-119"><a href="#TypeParser-119"><span class="linenos">119</span></a><span class="sd">			: list of strings that represent a float or Decimal that is NaN (not a number)</span>
-</span><span id="TypeParser-120"><a href="#TypeParser-120"><span class="linenos">120</span></a>
-</span><span id="TypeParser-121"><a href="#TypeParser-121"><span class="linenos">121</span></a><span class="sd">			`float_case_sensitive`</span>
-</span><span id="TypeParser-122"><a href="#TypeParser-122"><span class="linenos">122</span></a><span class="sd">			: whether checks for float should be done in a case-sensitive manner. This applies to matches against `inf_values` and `nan_values`, as well as to values given in scientific notation, where the mantissa and exponent are usually separated by `e`.</span>
-</span><span id="TypeParser-123"><a href="#TypeParser-123"><span class="linenos">123</span></a>
-</span><span id="TypeParser-124"><a href="#TypeParser-124"><span class="linenos">124</span></a><span class="sd">			`case_sensitive`</span>
-</span><span id="TypeParser-125"><a href="#TypeParser-125"><span class="linenos">125</span></a><span class="sd">			: whether all matches should be made in a case-sensitive manner. Sets all of `none_case_sensitive`, `bool_case_sensitive`, `int_case_sensitive`, `float_case_sensitive` to the same value, ignoring any individual settings.</span>
-</span><span id="TypeParser-126"><a href="#TypeParser-126"><span class="linenos">126</span></a>
-</span><span id="TypeParser-127"><a href="#TypeParser-127"><span class="linenos">127</span></a><span class="sd">			Raises</span>
-</span><span id="TypeParser-128"><a href="#TypeParser-128"><span class="linenos">128</span></a><span class="sd">			------</span>
-</span><span id="TypeParser-129"><a href="#TypeParser-129"><span class="linenos">129</span></a><span class="sd">			`ValueError` if any of the options would lead to ambiguities during parsing</span>
-</span><span id="TypeParser-130"><a href="#TypeParser-130"><span class="linenos">130</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser-131"><a href="#TypeParser-131"><span class="linenos">131</span></a>
-</span><span id="TypeParser-132"><a href="#TypeParser-132"><span class="linenos">132</span></a>		<span class="k">if</span> <span class="n">case_sensitive</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="TypeParser-133"><a href="#TypeParser-133"><span class="linenos">133</span></a>			<span class="n">none_case_sensitive</span> <span class="o">=</span> <span class="n">case_sensitive</span>
-</span><span id="TypeParser-134"><a href="#TypeParser-134"><span class="linenos">134</span></a>			<span class="n">int_case_sensitive</span> <span class="o">=</span> <span class="n">case_sensitive</span>
-</span><span id="TypeParser-135"><a href="#TypeParser-135"><span class="linenos">135</span></a>			<span class="n">bool_case_sensitive</span> <span class="o">=</span> <span class="n">case_sensitive</span>
-</span><span id="TypeParser-136"><a href="#TypeParser-136"><span class="linenos">136</span></a>			<span class="n">float_case_sensitive</span> <span class="o">=</span> <span class="n">case_sensitive</span>
-</span><span id="TypeParser-137"><a href="#TypeParser-137"><span class="linenos">137</span></a>
-</span><span id="TypeParser-138"><a href="#TypeParser-138"><span class="linenos">138</span></a>		<span class="bp">self</span><span class="o">.</span><span class="n">trim</span> <span class="o">=</span> <span class="n">trim</span>
-</span><span id="TypeParser-139"><a href="#TypeParser-139"><span class="linenos">139</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">trim</span><span class="p">:</span>
-</span><span id="TypeParser-140"><a href="#TypeParser-140"><span class="linenos">140</span></a>			<span class="n">none_values</span> <span class="o">=</span> <span class="p">(</span><span class="n">value</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">none_values</span><span class="p">)</span>
-</span><span id="TypeParser-141"><a href="#TypeParser-141"><span class="linenos">141</span></a>			<span class="n">true_values</span> <span class="o">=</span> <span class="p">(</span><span class="n">value</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">true_values</span><span class="p">)</span>
-</span><span id="TypeParser-142"><a href="#TypeParser-142"><span class="linenos">142</span></a>			<span class="n">false_values</span> <span class="o">=</span> <span class="p">(</span><span class="n">value</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">false_values</span><span class="p">)</span>
-</span><span id="TypeParser-143"><a href="#TypeParser-143"><span class="linenos">143</span></a>			<span class="n">inf_values</span> <span class="o">=</span> <span class="p">(</span><span class="n">value</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">inf_values</span><span class="p">)</span>
-</span><span id="TypeParser-144"><a href="#TypeParser-144"><span class="linenos">144</span></a>			<span class="n">nan_values</span> <span class="o">=</span> <span class="p">(</span><span class="n">value</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">nan_values</span><span class="p">)</span>
-</span><span id="TypeParser-145"><a href="#TypeParser-145"><span class="linenos">145</span></a>
-</span><span id="TypeParser-146"><a href="#TypeParser-146"><span class="linenos">146</span></a>		<span class="bp">self</span><span class="o">.</span><span class="n">use_decimal</span> <span class="o">=</span> <span class="n">use_decimal</span>
-</span><span id="TypeParser-147"><a href="#TypeParser-147"><span class="linenos">147</span></a>		<span class="bp">self</span><span class="o">.</span><span class="n">list_delimiter</span> <span class="o">=</span> <span class="n">list_delimiter</span>
-</span><span id="TypeParser-148"><a href="#TypeParser-148"><span class="linenos">148</span></a>
-</span><span id="TypeParser-149"><a href="#TypeParser-149"><span class="linenos">149</span></a>		<span class="bp">self</span><span class="o">.</span><span class="n">none_case_sensitive</span> <span class="o">=</span> <span class="n">none_case_sensitive</span>
-</span><span id="TypeParser-150"><a href="#TypeParser-150"><span class="linenos">150</span></a>		<span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">none_case_sensitive</span><span class="p">:</span>
-</span><span id="TypeParser-151"><a href="#TypeParser-151"><span class="linenos">151</span></a>			<span class="n">none_values</span> <span class="o">=</span> <span class="p">(</span><span class="n">value</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">none_values</span><span class="p">)</span>
-</span><span id="TypeParser-152"><a href="#TypeParser-152"><span class="linenos">152</span></a>		<span class="bp">self</span><span class="o">.</span><span class="n">none_values</span> <span class="o">=</span> <span class="nb">set</span><span class="p">(</span><span class="n">none_values</span><span class="p">)</span>
-</span><span id="TypeParser-153"><a href="#TypeParser-153"><span class="linenos">153</span></a>
-</span><span id="TypeParser-154"><a href="#TypeParser-154"><span class="linenos">154</span></a>		<span class="bp">self</span><span class="o">.</span><span class="n">bool_case_sensitive</span> <span class="o">=</span> <span class="n">bool_case_sensitive</span>
-</span><span id="TypeParser-155"><a href="#TypeParser-155"><span class="linenos">155</span></a>		<span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">bool_case_sensitive</span><span class="p">:</span>
-</span><span id="TypeParser-156"><a href="#TypeParser-156"><span class="linenos">156</span></a>			<span class="n">true_values</span> <span class="o">=</span> <span class="p">(</span><span class="n">value</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">true_values</span><span class="p">)</span>
-</span><span id="TypeParser-157"><a href="#TypeParser-157"><span class="linenos">157</span></a>			<span class="n">false_values</span> <span class="o">=</span> <span class="p">(</span><span class="n">value</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">false_values</span><span class="p">)</span>
-</span><span id="TypeParser-158"><a href="#TypeParser-158"><span class="linenos">158</span></a>		<span class="bp">self</span><span class="o">.</span><span class="n">true_values</span> <span class="o">=</span> <span class="nb">set</span><span class="p">(</span><span class="n">true_values</span><span class="p">)</span>
-</span><span id="TypeParser-159"><a href="#TypeParser-159"><span class="linenos">159</span></a>		<span class="bp">self</span><span class="o">.</span><span class="n">false_values</span> <span class="o">=</span> <span class="nb">set</span><span class="p">(</span><span class="n">false_values</span><span class="p">)</span>
-</span><span id="TypeParser-160"><a href="#TypeParser-160"><span class="linenos">160</span></a>
-</span><span id="TypeParser-161"><a href="#TypeParser-161"><span class="linenos">161</span></a>		<span class="bp">self</span><span class="o">.</span><span class="n">int_case_sensitive</span> <span class="o">=</span> <span class="n">int_case_sensitive</span>
-</span><span id="TypeParser-162"><a href="#TypeParser-162"><span class="linenos">162</span></a>
-</span><span id="TypeParser-163"><a href="#TypeParser-163"><span class="linenos">163</span></a>		<span class="bp">self</span><span class="o">.</span><span class="n">float_case_sensitive</span> <span class="o">=</span> <span class="n">float_case_sensitive</span>
-</span><span id="TypeParser-164"><a href="#TypeParser-164"><span class="linenos">164</span></a>		<span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">float_case_sensitive</span><span class="p">:</span>
-</span><span id="TypeParser-165"><a href="#TypeParser-165"><span class="linenos">165</span></a>			<span class="n">inf_values</span> <span class="o">=</span> <span class="p">(</span><span class="n">value</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">inf_values</span><span class="p">)</span>
-</span><span id="TypeParser-166"><a href="#TypeParser-166"><span class="linenos">166</span></a>			<span class="n">nan_values</span> <span class="o">=</span> <span class="p">(</span><span class="n">value</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">nan_values</span><span class="p">)</span>
-</span><span id="TypeParser-167"><a href="#TypeParser-167"><span class="linenos">167</span></a>		<span class="bp">self</span><span class="o">.</span><span class="n">inf_values</span> <span class="o">=</span> <span class="nb">set</span><span class="p">(</span><span class="n">inf_values</span><span class="p">)</span>
-</span><span id="TypeParser-168"><a href="#TypeParser-168"><span class="linenos">168</span></a>		<span class="bp">self</span><span class="o">.</span><span class="n">nan_values</span> <span class="o">=</span> <span class="nb">set</span><span class="p">(</span><span class="n">nan_values</span><span class="p">)</span>
-</span><span id="TypeParser-169"><a href="#TypeParser-169"><span class="linenos">169</span></a>
-</span><span id="TypeParser-170"><a href="#TypeParser-170"><span class="linenos">170</span></a>		<span class="c1"># Unconfigurable default values</span>
-</span><span id="TypeParser-171"><a href="#TypeParser-171"><span class="linenos">171</span></a>		<span class="bp">self</span><span class="o">.</span><span class="n">_negative_char</span> <span class="o">=</span> <span class="s2">&quot;-&quot;</span>
-</span><span id="TypeParser-172"><a href="#TypeParser-172"><span class="linenos">172</span></a>		<span class="bp">self</span><span class="o">.</span><span class="n">_negative_chars</span> <span class="o">=</span> <span class="p">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_negative_char</span><span class="p">,</span> <span class="s2">&quot;−&quot;</span><span class="p">}</span>
-</span><span id="TypeParser-173"><a href="#TypeParser-173"><span class="linenos">173</span></a>		<span class="bp">self</span><span class="o">.</span><span class="n">_sign_chars</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_negative_chars</span> <span class="o">|</span> <span class="p">{</span><span class="s2">&quot;+&quot;</span><span class="p">}</span>
-</span><span id="TypeParser-174"><a href="#TypeParser-174"><span class="linenos">174</span></a>		<span class="bp">self</span><span class="o">.</span><span class="n">_digit_chars</span> <span class="o">=</span> <span class="p">{</span><span class="s2">&quot;0&quot;</span><span class="p">,</span> <span class="s2">&quot;1&quot;</span><span class="p">,</span> <span class="s2">&quot;2&quot;</span><span class="p">,</span> <span class="s2">&quot;3&quot;</span><span class="p">,</span> <span class="s2">&quot;4&quot;</span><span class="p">,</span> <span class="s2">&quot;5&quot;</span><span class="p">,</span> <span class="s2">&quot;6&quot;</span><span class="p">,</span> <span class="s2">&quot;7&quot;</span><span class="p">,</span> <span class="s2">&quot;8&quot;</span><span class="p">,</span> <span class="s2">&quot;9&quot;</span><span class="p">}</span>  <span class="c1"># Because isdigit(&quot;²&quot;) == True, but int(&quot;²&quot;) is invalid</span>
-</span><span id="TypeParser-175"><a href="#TypeParser-175"><span class="linenos">175</span></a>		<span class="bp">self</span><span class="o">.</span><span class="n">_digit_separators</span> <span class="o">=</span> <span class="p">{</span><span class="s2">&quot;_&quot;</span><span class="p">}</span>
-</span><span id="TypeParser-176"><a href="#TypeParser-176"><span class="linenos">176</span></a>		<span class="bp">self</span><span class="o">.</span><span class="n">_scientific_char</span> <span class="o">=</span> <span class="s2">&quot;e&quot;</span>
-</span><span id="TypeParser-177"><a href="#TypeParser-177"><span class="linenos">177</span></a>		<span class="bp">self</span><span class="o">.</span><span class="n">_float_separator</span> <span class="o">=</span> <span class="s2">&quot;.&quot;</span>
-</span><span id="TypeParser-178"><a href="#TypeParser-178"><span class="linenos">178</span></a>		<span class="bp">self</span><span class="o">.</span><span class="n">_reserved_chars</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_sign_chars</span> <span class="o">|</span> <span class="bp">self</span><span class="o">.</span><span class="n">_digit_chars</span> <span class="o">|</span> <span class="bp">self</span><span class="o">.</span><span class="n">_digit_separators</span> <span class="o">|</span> <span class="p">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_scientific_char</span><span class="p">}</span> <span class="o">|</span> <span class="p">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_float_separator</span><span class="p">}</span>
-</span><span id="TypeParser-179"><a href="#TypeParser-179"><span class="linenos">179</span></a>		<span class="c1"># special_chars = self._reserved_chars | self.list_delimiter</span>
-</span><span id="TypeParser-180"><a href="#TypeParser-180"><span class="linenos">180</span></a>
-</span><span id="TypeParser-181"><a href="#TypeParser-181"><span class="linenos">181</span></a>		<span class="c1"># Check if any special values conflict</span>
-</span><span id="TypeParser-182"><a href="#TypeParser-182"><span class="linenos">182</span></a>		<span class="k">for</span> <span class="n">name</span><span class="p">,</span> <span class="n">special_values</span> <span class="ow">in</span> <span class="p">[</span>
-</span><span id="TypeParser-183"><a href="#TypeParser-183"><span class="linenos">183</span></a>			<span class="p">(</span><span class="n">_SpecialValue</span><span class="o">.</span><span class="n">LIST</span><span class="p">,</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">list_delimiter</span><span class="p">]</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">list_delimiter</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span> <span class="k">else</span> <span class="p">[]),</span>
-</span><span id="TypeParser-184"><a href="#TypeParser-184"><span class="linenos">184</span></a>			<span class="p">(</span><span class="n">_SpecialValue</span><span class="o">.</span><span class="n">NONE</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">none_values</span><span class="p">),</span>
-</span><span id="TypeParser-185"><a href="#TypeParser-185"><span class="linenos">185</span></a>			<span class="p">(</span><span class="n">_SpecialValue</span><span class="o">.</span><span class="n">TRUE</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">true_values</span><span class="p">),</span>
-</span><span id="TypeParser-186"><a href="#TypeParser-186"><span class="linenos">186</span></a>			<span class="p">(</span><span class="n">_SpecialValue</span><span class="o">.</span><span class="n">FALSE</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">false_values</span><span class="p">),</span>
-</span><span id="TypeParser-187"><a href="#TypeParser-187"><span class="linenos">187</span></a>			<span class="p">(</span><span class="n">_SpecialValue</span><span class="o">.</span><span class="n">INF</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">inf_values</span><span class="p">),</span>
-</span><span id="TypeParser-188"><a href="#TypeParser-188"><span class="linenos">188</span></a>			<span class="p">(</span><span class="n">_SpecialValue</span><span class="o">.</span><span class="n">NAN</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">nan_values</span><span class="p">),</span>
-</span><span id="TypeParser-189"><a href="#TypeParser-189"><span class="linenos">189</span></a>		<span class="p">]:</span>
-</span><span id="TypeParser-190"><a href="#TypeParser-190"><span class="linenos">190</span></a>			<span class="k">for</span> <span class="n">special_value</span> <span class="ow">in</span> <span class="n">special_values</span><span class="p">:</span>
-</span><span id="TypeParser-191"><a href="#TypeParser-191"><span class="linenos">191</span></a>				<span class="k">if</span> <span class="n">special_value</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_reserved_chars</span><span class="p">:</span>
-</span><span id="TypeParser-192"><a href="#TypeParser-192"><span class="linenos">192</span></a>					<span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;cannot use reserved char as </span><span class="si">{</span><span class="n">name</span><span class="o">.</span><span class="n">value</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">special_value</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="TypeParser-193"><a href="#TypeParser-193"><span class="linenos">193</span></a>
-</span><span id="TypeParser-194"><a href="#TypeParser-194"><span class="linenos">194</span></a>				<span class="k">if</span> <span class="n">name</span> <span class="o">!=</span> <span class="n">_SpecialValue</span><span class="o">.</span><span class="n">NONE</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_none</span><span class="p">(</span><span class="n">special_value</span><span class="p">):</span>
-</span><span id="TypeParser-195"><a href="#TypeParser-195"><span class="linenos">195</span></a>					<span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;cannot use None value as </span><span class="si">{</span><span class="n">name</span><span class="o">.</span><span class="n">value</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">special_value</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="TypeParser-196"><a href="#TypeParser-196"><span class="linenos">196</span></a>
-</span><span id="TypeParser-197"><a href="#TypeParser-197"><span class="linenos">197</span></a>				<span class="k">if</span> <span class="p">(</span>
-</span><span id="TypeParser-198"><a href="#TypeParser-198"><span class="linenos">198</span></a>					<span class="p">(</span><span class="n">name</span> <span class="o">==</span> <span class="n">_SpecialValue</span><span class="o">.</span><span class="n">TRUE</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_bool</span><span class="p">(</span><span class="n">special_value</span><span class="p">)</span> <span class="o">!=</span> <span class="kc">True</span><span class="p">)</span> <span class="ow">or</span>
-</span><span id="TypeParser-199"><a href="#TypeParser-199"><span class="linenos">199</span></a>					<span class="p">(</span><span class="n">name</span> <span class="o">==</span> <span class="n">_SpecialValue</span><span class="o">.</span><span class="n">FALSE</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_bool</span><span class="p">(</span><span class="n">special_value</span><span class="p">)</span> <span class="o">!=</span> <span class="kc">False</span><span class="p">)</span> <span class="ow">or</span>
-</span><span id="TypeParser-200"><a href="#TypeParser-200"><span class="linenos">200</span></a>					<span class="p">(</span><span class="n">name</span> <span class="o">!=</span> <span class="n">_SpecialValue</span><span class="o">.</span><span class="n">TRUE</span> <span class="ow">and</span> <span class="n">name</span> <span class="o">!=</span> <span class="n">_SpecialValue</span><span class="o">.</span><span class="n">FALSE</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_bool</span><span class="p">(</span><span class="n">special_value</span><span class="p">))</span>
-</span><span id="TypeParser-201"><a href="#TypeParser-201"><span class="linenos">201</span></a>				<span class="p">):</span>
-</span><span id="TypeParser-202"><a href="#TypeParser-202"><span class="linenos">202</span></a>					<span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;cannot use bool value as </span><span class="si">{</span><span class="n">name</span><span class="o">.</span><span class="n">value</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">special_value</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="TypeParser-203"><a href="#TypeParser-203"><span class="linenos">203</span></a>
-</span><span id="TypeParser-204"><a href="#TypeParser-204"><span class="linenos">204</span></a>				<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_int</span><span class="p">(</span><span class="n">special_value</span><span class="p">):</span>
-</span><span id="TypeParser-205"><a href="#TypeParser-205"><span class="linenos">205</span></a>					<span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;cannot use int value as </span><span class="si">{</span><span class="n">name</span><span class="o">.</span><span class="n">value</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">special_value</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="TypeParser-206"><a href="#TypeParser-206"><span class="linenos">206</span></a>
-</span><span id="TypeParser-207"><a href="#TypeParser-207"><span class="linenos">207</span></a>				<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">use_decimal</span><span class="p">:</span>
-</span><span id="TypeParser-208"><a href="#TypeParser-208"><span class="linenos">208</span></a>					<span class="k">if</span> <span class="p">(</span>
-</span><span id="TypeParser-209"><a href="#TypeParser-209"><span class="linenos">209</span></a>						<span class="p">(</span><span class="n">name</span> <span class="o">==</span> <span class="n">_SpecialValue</span><span class="o">.</span><span class="n">INF</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_decimal</span><span class="p">(</span><span class="n">special_value</span><span class="p">)</span> <span class="o">!=</span> <span class="n">Decimal</span><span class="p">(</span><span class="n">math</span><span class="o">.</span><span class="n">inf</span><span class="p">))</span> <span class="ow">or</span>
-</span><span id="TypeParser-210"><a href="#TypeParser-210"><span class="linenos">210</span></a>						<span class="p">(</span><span class="n">name</span> <span class="o">==</span> <span class="n">_SpecialValue</span><span class="o">.</span><span class="n">NAN</span> <span class="ow">and</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_decimal</span><span class="p">(</span><span class="n">special_value</span><span class="p">)</span><span class="o">.</span><span class="n">is_nan</span><span class="p">())</span> <span class="ow">or</span>
-</span><span id="TypeParser-211"><a href="#TypeParser-211"><span class="linenos">211</span></a>						<span class="p">(</span><span class="n">name</span> <span class="o">!=</span> <span class="n">_SpecialValue</span><span class="o">.</span><span class="n">INF</span> <span class="ow">and</span> <span class="n">name</span> <span class="o">!=</span> <span class="n">_SpecialValue</span><span class="o">.</span><span class="n">NAN</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_float</span><span class="p">(</span><span class="n">special_value</span><span class="p">))</span>
-</span><span id="TypeParser-212"><a href="#TypeParser-212"><span class="linenos">212</span></a>					<span class="p">):</span>
-</span><span id="TypeParser-213"><a href="#TypeParser-213"><span class="linenos">213</span></a>						<span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;cannot use Decimal value as </span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">special_value</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="TypeParser-214"><a href="#TypeParser-214"><span class="linenos">214</span></a>				<span class="k">else</span><span class="p">:</span>
-</span><span id="TypeParser-215"><a href="#TypeParser-215"><span class="linenos">215</span></a>					<span class="k">if</span> <span class="p">(</span>
-</span><span id="TypeParser-216"><a href="#TypeParser-216"><span class="linenos">216</span></a>						<span class="p">(</span><span class="n">name</span> <span class="o">==</span> <span class="n">_SpecialValue</span><span class="o">.</span><span class="n">INF</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_float</span><span class="p">(</span><span class="n">special_value</span><span class="p">)</span> <span class="o">!=</span> <span class="n">math</span><span class="o">.</span><span class="n">inf</span><span class="p">)</span> <span class="ow">or</span>
-</span><span id="TypeParser-217"><a href="#TypeParser-217"><span class="linenos">217</span></a>						<span class="p">(</span><span class="n">name</span> <span class="o">==</span> <span class="n">_SpecialValue</span><span class="o">.</span><span class="n">NAN</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_float</span><span class="p">(</span><span class="n">special_value</span><span class="p">)</span> <span class="ow">is</span> <span class="ow">not</span> <span class="n">math</span><span class="o">.</span><span class="n">nan</span><span class="p">)</span> <span class="ow">or</span>
-</span><span id="TypeParser-218"><a href="#TypeParser-218"><span class="linenos">218</span></a>						<span class="p">(</span><span class="n">name</span> <span class="o">!=</span> <span class="n">_SpecialValue</span><span class="o">.</span><span class="n">INF</span> <span class="ow">and</span> <span class="n">name</span> <span class="o">!=</span> <span class="n">_SpecialValue</span><span class="o">.</span><span class="n">NAN</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_float</span><span class="p">(</span><span class="n">special_value</span><span class="p">))</span>
-</span><span id="TypeParser-219"><a href="#TypeParser-219"><span class="linenos">219</span></a>					<span class="p">):</span>
-</span><span id="TypeParser-220"><a href="#TypeParser-220"><span class="linenos">220</span></a>						<span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;cannot use float value as </span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">special_value</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="TypeParser-221"><a href="#TypeParser-221"><span class="linenos">221</span></a>
-</span><span id="TypeParser-222"><a href="#TypeParser-222"><span class="linenos">222</span></a>
-</span><span id="TypeParser-223"><a href="#TypeParser-223"><span class="linenos">223</span></a>	<span class="k">def</span> <span class="nf">is_none</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="TypeParser-224"><a href="#TypeParser-224"><span class="linenos">224</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser-225"><a href="#TypeParser-225"><span class="linenos">225</span></a><span class="sd">			Check if a string represents the value None</span>
-</span><span id="TypeParser-226"><a href="#TypeParser-226"><span class="linenos">226</span></a>
-</span><span id="TypeParser-227"><a href="#TypeParser-227"><span class="linenos">227</span></a><span class="sd">			Only strings that match the values in `self.none_values` will be interpreted as None. The default accepted values are `[&quot;&quot;]`, i.e. an empty string. The case sensitivity of this matching depends on `self.none_case_sensitive`, which is False by default.</span>
-</span><span id="TypeParser-228"><a href="#TypeParser-228"><span class="linenos">228</span></a>
-</span><span id="TypeParser-229"><a href="#TypeParser-229"><span class="linenos">229</span></a><span class="sd">			Parameters</span>
-</span><span id="TypeParser-230"><a href="#TypeParser-230"><span class="linenos">230</span></a><span class="sd">			----------</span>
-</span><span id="TypeParser-231"><a href="#TypeParser-231"><span class="linenos">231</span></a><span class="sd">			`value`</span>
-</span><span id="TypeParser-232"><a href="#TypeParser-232"><span class="linenos">232</span></a><span class="sd">			: string to be checked</span>
-</span><span id="TypeParser-233"><a href="#TypeParser-233"><span class="linenos">233</span></a>
-</span><span id="TypeParser-234"><a href="#TypeParser-234"><span class="linenos">234</span></a><span class="sd">			Returns</span>
-</span><span id="TypeParser-235"><a href="#TypeParser-235"><span class="linenos">235</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser-236"><a href="#TypeParser-236"><span class="linenos">236</span></a><span class="sd">			whether it is None</span>
-</span><span id="TypeParser-237"><a href="#TypeParser-237"><span class="linenos">237</span></a>
-</span><span id="TypeParser-238"><a href="#TypeParser-238"><span class="linenos">238</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser-239"><a href="#TypeParser-239"><span class="linenos">239</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser-240"><a href="#TypeParser-240"><span class="linenos">240</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser-241"><a href="#TypeParser-241"><span class="linenos">241</span></a><span class="sd">			parser = TypeParser()</span>
-</span><span id="TypeParser-242"><a href="#TypeParser-242"><span class="linenos">242</span></a><span class="sd">			parser.parse_bool(&quot;&quot;)     # True</span>
-</span><span id="TypeParser-243"><a href="#TypeParser-243"><span class="linenos">243</span></a><span class="sd">			parser.parse_bool(&quot;abc&quot;)  # False</span>
-</span><span id="TypeParser-244"><a href="#TypeParser-244"><span class="linenos">244</span></a><span class="sd">			```</span>
-</span><span id="TypeParser-245"><a href="#TypeParser-245"><span class="linenos">245</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser-246"><a href="#TypeParser-246"><span class="linenos">246</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">trim</span><span class="p">:</span>
-</span><span id="TypeParser-247"><a href="#TypeParser-247"><span class="linenos">247</span></a>			<span class="n">value</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
-</span><span id="TypeParser-248"><a href="#TypeParser-248"><span class="linenos">248</span></a>		<span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">bool_case_sensitive</span><span class="p">:</span>
-</span><span id="TypeParser-249"><a href="#TypeParser-249"><span class="linenos">249</span></a>			<span class="n">value</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span>
-</span><span id="TypeParser-250"><a href="#TypeParser-250"><span class="linenos">250</span></a>
-</span><span id="TypeParser-251"><a href="#TypeParser-251"><span class="linenos">251</span></a>		<span class="k">if</span> <span class="n">value</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">none_values</span><span class="p">:</span>
-</span><span id="TypeParser-252"><a href="#TypeParser-252"><span class="linenos">252</span></a>			<span class="k">return</span> <span class="kc">True</span>
-</span><span id="TypeParser-253"><a href="#TypeParser-253"><span class="linenos">253</span></a>		<span class="k">else</span><span class="p">:</span>
-</span><span id="TypeParser-254"><a href="#TypeParser-254"><span class="linenos">254</span></a>			<span class="k">return</span> <span class="kc">False</span>
-</span><span id="TypeParser-255"><a href="#TypeParser-255"><span class="linenos">255</span></a>
-</span><span id="TypeParser-256"><a href="#TypeParser-256"><span class="linenos">256</span></a>
-</span><span id="TypeParser-257"><a href="#TypeParser-257"><span class="linenos">257</span></a>	<span class="k">def</span> <span class="nf">is_bool</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="TypeParser-258"><a href="#TypeParser-258"><span class="linenos">258</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser-259"><a href="#TypeParser-259"><span class="linenos">259</span></a><span class="sd">			Check if a string represents a bool</span>
-</span><span id="TypeParser-260"><a href="#TypeParser-260"><span class="linenos">260</span></a>
-</span><span id="TypeParser-261"><a href="#TypeParser-261"><span class="linenos">261</span></a><span class="sd">			Only strings that match the values in `self.true_values` and `self.false_values` will be interpreted as booleans. The default accepted values are `[&quot;true&quot;]` and `[&quot;false&quot;]` respectively. The case sensitivity of this matching depends on `self.bool_case_sensitive`, which is False by default.</span>
-</span><span id="TypeParser-262"><a href="#TypeParser-262"><span class="linenos">262</span></a>
-</span><span id="TypeParser-263"><a href="#TypeParser-263"><span class="linenos">263</span></a><span class="sd">			Parameters</span>
-</span><span id="TypeParser-264"><a href="#TypeParser-264"><span class="linenos">264</span></a><span class="sd">			----------</span>
-</span><span id="TypeParser-265"><a href="#TypeParser-265"><span class="linenos">265</span></a><span class="sd">			`value`</span>
-</span><span id="TypeParser-266"><a href="#TypeParser-266"><span class="linenos">266</span></a><span class="sd">			: string to be checked</span>
-</span><span id="TypeParser-267"><a href="#TypeParser-267"><span class="linenos">267</span></a>
-</span><span id="TypeParser-268"><a href="#TypeParser-268"><span class="linenos">268</span></a><span class="sd">			Returns</span>
-</span><span id="TypeParser-269"><a href="#TypeParser-269"><span class="linenos">269</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser-270"><a href="#TypeParser-270"><span class="linenos">270</span></a><span class="sd">			whether it is a bool</span>
-</span><span id="TypeParser-271"><a href="#TypeParser-271"><span class="linenos">271</span></a>
-</span><span id="TypeParser-272"><a href="#TypeParser-272"><span class="linenos">272</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser-273"><a href="#TypeParser-273"><span class="linenos">273</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser-274"><a href="#TypeParser-274"><span class="linenos">274</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser-275"><a href="#TypeParser-275"><span class="linenos">275</span></a><span class="sd">			parser = TypeParser()</span>
-</span><span id="TypeParser-276"><a href="#TypeParser-276"><span class="linenos">276</span></a><span class="sd">			parser.is_bool(&quot;true&quot;)  # True</span>
-</span><span id="TypeParser-277"><a href="#TypeParser-277"><span class="linenos">277</span></a><span class="sd">			parser.is_bool(&quot;&quot;)      # True</span>
-</span><span id="TypeParser-278"><a href="#TypeParser-278"><span class="linenos">278</span></a><span class="sd">			parser.is_bool(&quot;abc&quot;)   # False</span>
-</span><span id="TypeParser-279"><a href="#TypeParser-279"><span class="linenos">279</span></a><span class="sd">			```</span>
-</span><span id="TypeParser-280"><a href="#TypeParser-280"><span class="linenos">280</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser-281"><a href="#TypeParser-281"><span class="linenos">281</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">trim</span><span class="p">:</span>
-</span><span id="TypeParser-282"><a href="#TypeParser-282"><span class="linenos">282</span></a>			<span class="n">value</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
-</span><span id="TypeParser-283"><a href="#TypeParser-283"><span class="linenos">283</span></a>
-</span><span id="TypeParser-284"><a href="#TypeParser-284"><span class="linenos">284</span></a>		<span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">bool_case_sensitive</span><span class="p">:</span>
-</span><span id="TypeParser-285"><a href="#TypeParser-285"><span class="linenos">285</span></a>			<span class="n">value</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span>
-</span><span id="TypeParser-286"><a href="#TypeParser-286"><span class="linenos">286</span></a>		<span class="k">if</span> <span class="n">value</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">true_values</span><span class="p">:</span>
-</span><span id="TypeParser-287"><a href="#TypeParser-287"><span class="linenos">287</span></a>			<span class="k">return</span> <span class="kc">True</span>
-</span><span id="TypeParser-288"><a href="#TypeParser-288"><span class="linenos">288</span></a>		<span class="k">if</span> <span class="n">value</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">false_values</span><span class="p">:</span>
-</span><span id="TypeParser-289"><a href="#TypeParser-289"><span class="linenos">289</span></a>			<span class="k">return</span> <span class="kc">True</span>
-</span><span id="TypeParser-290"><a href="#TypeParser-290"><span class="linenos">290</span></a>
-</span><span id="TypeParser-291"><a href="#TypeParser-291"><span class="linenos">291</span></a>		<span class="k">return</span> <span class="kc">False</span>
-</span><span id="TypeParser-292"><a href="#TypeParser-292"><span class="linenos">292</span></a>
-</span><span id="TypeParser-293"><a href="#TypeParser-293"><span class="linenos">293</span></a>
-</span><span id="TypeParser-294"><a href="#TypeParser-294"><span class="linenos">294</span></a>	<span class="k">def</span> <span class="nf">is_int</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="o">*</span><span class="p">,</span> <span class="n">allow_sign</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_negative</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="TypeParser-295"><a href="#TypeParser-295"><span class="linenos">295</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser-296"><a href="#TypeParser-296"><span class="linenos">296</span></a><span class="sd">			Check if a string represents an int</span>
-</span><span id="TypeParser-297"><a href="#TypeParser-297"><span class="linenos">297</span></a>
-</span><span id="TypeParser-298"><a href="#TypeParser-298"><span class="linenos">298</span></a><span class="sd">			Parameters</span>
-</span><span id="TypeParser-299"><a href="#TypeParser-299"><span class="linenos">299</span></a><span class="sd">			----------</span>
-</span><span id="TypeParser-300"><a href="#TypeParser-300"><span class="linenos">300</span></a><span class="sd">			`value`</span>
-</span><span id="TypeParser-301"><a href="#TypeParser-301"><span class="linenos">301</span></a><span class="sd">			: string to be checked</span>
-</span><span id="TypeParser-302"><a href="#TypeParser-302"><span class="linenos">302</span></a>
-</span><span id="TypeParser-303"><a href="#TypeParser-303"><span class="linenos">303</span></a><span class="sd">			`allow_negative`</span>
-</span><span id="TypeParser-304"><a href="#TypeParser-304"><span class="linenos">304</span></a><span class="sd">			: whether to accept negative values</span>
-</span><span id="TypeParser-305"><a href="#TypeParser-305"><span class="linenos">305</span></a>
-</span><span id="TypeParser-306"><a href="#TypeParser-306"><span class="linenos">306</span></a><span class="sd">			`allow_sign`</span>
-</span><span id="TypeParser-307"><a href="#TypeParser-307"><span class="linenos">307</span></a><span class="sd">			: whether to accept signed values. If False, it implies that `allow_negative` is False also.</span>
-</span><span id="TypeParser-308"><a href="#TypeParser-308"><span class="linenos">308</span></a>
-</span><span id="TypeParser-309"><a href="#TypeParser-309"><span class="linenos">309</span></a><span class="sd">			`allow_scientific`</span>
-</span><span id="TypeParser-310"><a href="#TypeParser-310"><span class="linenos">310</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form &lt;code&gt;&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;&lt;/code&gt; will be interpreted as the expression &lt;code&gt;&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)&lt;/code&gt;, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note &lt;var&gt;M&lt;/var&gt; *must* be an integer and &lt;var&gt;X&lt;/var&gt; *must* be a non-negative integer, even in cases where the above expression evaluates mathematically to an integer.</span>
-</span><span id="TypeParser-311"><a href="#TypeParser-311"><span class="linenos">311</span></a>
-</span><span id="TypeParser-312"><a href="#TypeParser-312"><span class="linenos">312</span></a><span class="sd">			Returns</span>
-</span><span id="TypeParser-313"><a href="#TypeParser-313"><span class="linenos">313</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser-314"><a href="#TypeParser-314"><span class="linenos">314</span></a><span class="sd">			whether it is an int</span>
-</span><span id="TypeParser-315"><a href="#TypeParser-315"><span class="linenos">315</span></a>
-</span><span id="TypeParser-316"><a href="#TypeParser-316"><span class="linenos">316</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser-317"><a href="#TypeParser-317"><span class="linenos">317</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser-318"><a href="#TypeParser-318"><span class="linenos">318</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser-319"><a href="#TypeParser-319"><span class="linenos">319</span></a><span class="sd">			parser = TypeParser()</span>
-</span><span id="TypeParser-320"><a href="#TypeParser-320"><span class="linenos">320</span></a><span class="sd">			parser.is_int(&quot;0&quot;)    # True</span>
-</span><span id="TypeParser-321"><a href="#TypeParser-321"><span class="linenos">321</span></a><span class="sd">			parser.is_int(&quot;-1&quot;)   # True</span>
-</span><span id="TypeParser-322"><a href="#TypeParser-322"><span class="linenos">322</span></a><span class="sd">			parser.is_int(&quot;abc&quot;)  # False</span>
-</span><span id="TypeParser-323"><a href="#TypeParser-323"><span class="linenos">323</span></a><span class="sd">			parser.is_int(&quot;&quot;)     # False</span>
-</span><span id="TypeParser-324"><a href="#TypeParser-324"><span class="linenos">324</span></a><span class="sd">			```</span>
-</span><span id="TypeParser-325"><a href="#TypeParser-325"><span class="linenos">325</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser-326"><a href="#TypeParser-326"><span class="linenos">326</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">trim</span><span class="p">:</span>
-</span><span id="TypeParser-327"><a href="#TypeParser-327"><span class="linenos">327</span></a>			<span class="n">value</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
-</span><span id="TypeParser-328"><a href="#TypeParser-328"><span class="linenos">328</span></a>
-</span><span id="TypeParser-329"><a href="#TypeParser-329"><span class="linenos">329</span></a>		<span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="TypeParser-330"><a href="#TypeParser-330"><span class="linenos">330</span></a>			<span class="k">return</span> <span class="kc">False</span>
-</span><span id="TypeParser-331"><a href="#TypeParser-331"><span class="linenos">331</span></a>
-</span><span id="TypeParser-332"><a href="#TypeParser-332"><span class="linenos">332</span></a>		<span class="k">if</span> <span class="n">allow_scientific</span><span class="p">:</span>
-</span><span id="TypeParser-333"><a href="#TypeParser-333"><span class="linenos">333</span></a>			<span class="n">value</span><span class="p">,</span> <span class="n">exp</span> <span class="o">=</span> <span class="n">_decompose_string_pair</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_scientific_char</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">int_case_sensitive</span><span class="p">)</span>
-</span><span id="TypeParser-334"><a href="#TypeParser-334"><span class="linenos">334</span></a>			<span class="k">if</span> <span class="n">exp</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="TypeParser-335"><a href="#TypeParser-335"><span class="linenos">335</span></a>				<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_int</span><span class="p">(</span>
-</span><span id="TypeParser-336"><a href="#TypeParser-336"><span class="linenos">336</span></a>					<span class="n">value</span><span class="p">,</span> <span class="n">allow_sign</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_negative</span><span class="o">=</span><span class="n">allow_negative</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="o">=</span><span class="kc">False</span>
-</span><span id="TypeParser-337"><a href="#TypeParser-337"><span class="linenos">337</span></a>				<span class="p">)</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_int</span><span class="p">(</span>
-</span><span id="TypeParser-338"><a href="#TypeParser-338"><span class="linenos">338</span></a>					<span class="n">exp</span><span class="p">,</span> <span class="n">allow_sign</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_negative</span><span class="o">=</span><span class="kc">False</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="o">=</span><span class="kc">False</span>
-</span><span id="TypeParser-339"><a href="#TypeParser-339"><span class="linenos">339</span></a>				<span class="p">)</span>
-</span><span id="TypeParser-340"><a href="#TypeParser-340"><span class="linenos">340</span></a>
-</span><span id="TypeParser-341"><a href="#TypeParser-341"><span class="linenos">341</span></a>		<span class="k">if</span> <span class="n">value</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_sign_chars</span><span class="p">:</span>
-</span><span id="TypeParser-342"><a href="#TypeParser-342"><span class="linenos">342</span></a>			<span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="TypeParser-343"><a href="#TypeParser-343"><span class="linenos">343</span></a>				<span class="k">return</span> <span class="kc">False</span>
-</span><span id="TypeParser-344"><a href="#TypeParser-344"><span class="linenos">344</span></a>			<span class="k">if</span> <span class="ow">not</span> <span class="n">allow_sign</span><span class="p">:</span>
-</span><span id="TypeParser-345"><a href="#TypeParser-345"><span class="linenos">345</span></a>				<span class="k">return</span> <span class="kc">False</span>
-</span><span id="TypeParser-346"><a href="#TypeParser-346"><span class="linenos">346</span></a>			<span class="k">if</span> <span class="ow">not</span> <span class="n">allow_negative</span> <span class="ow">and</span> <span class="n">value</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_negative_chars</span><span class="p">:</span>
-</span><span id="TypeParser-347"><a href="#TypeParser-347"><span class="linenos">347</span></a>				<span class="k">return</span> <span class="kc">False</span>
-</span><span id="TypeParser-348"><a href="#TypeParser-348"><span class="linenos">348</span></a>			<span class="n">value</span> <span class="o">=</span> <span class="n">value</span><span class="p">[</span><span class="mi">1</span><span class="p">:]</span>
-</span><span id="TypeParser-349"><a href="#TypeParser-349"><span class="linenos">349</span></a>		<span class="k">if</span> <span class="n">value</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_digit_separators</span> <span class="ow">or</span> <span class="n">value</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_digit_separators</span><span class="p">:</span>
-</span><span id="TypeParser-350"><a href="#TypeParser-350"><span class="linenos">350</span></a>			<span class="k">return</span> <span class="kc">False</span>
-</span><span id="TypeParser-351"><a href="#TypeParser-351"><span class="linenos">351</span></a>
-</span><span id="TypeParser-352"><a href="#TypeParser-352"><span class="linenos">352</span></a>		<span class="n">prev_separated</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="TypeParser-353"><a href="#TypeParser-353"><span class="linenos">353</span></a>		<span class="k">for</span> <span class="n">c</span> <span class="ow">in</span> <span class="n">value</span><span class="p">:</span>
-</span><span id="TypeParser-354"><a href="#TypeParser-354"><span class="linenos">354</span></a>			<span class="k">if</span> <span class="n">c</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_digit_separators</span><span class="p">:</span>
-</span><span id="TypeParser-355"><a href="#TypeParser-355"><span class="linenos">355</span></a>				<span class="k">if</span> <span class="n">prev_separated</span><span class="p">:</span>
-</span><span id="TypeParser-356"><a href="#TypeParser-356"><span class="linenos">356</span></a>					<span class="k">return</span> <span class="kc">False</span>
-</span><span id="TypeParser-357"><a href="#TypeParser-357"><span class="linenos">357</span></a>				<span class="n">prev_separated</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="TypeParser-358"><a href="#TypeParser-358"><span class="linenos">358</span></a>			<span class="k">else</span><span class="p">:</span>
-</span><span id="TypeParser-359"><a href="#TypeParser-359"><span class="linenos">359</span></a>				<span class="n">prev_separated</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="TypeParser-360"><a href="#TypeParser-360"><span class="linenos">360</span></a>				<span class="k">if</span> <span class="n">c</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_digit_chars</span><span class="p">:</span>
-</span><span id="TypeParser-361"><a href="#TypeParser-361"><span class="linenos">361</span></a>					<span class="k">return</span> <span class="kc">False</span>
-</span><span id="TypeParser-362"><a href="#TypeParser-362"><span class="linenos">362</span></a>		<span class="k">return</span> <span class="kc">True</span>
-</span><span id="TypeParser-363"><a href="#TypeParser-363"><span class="linenos">363</span></a>
-</span><span id="TypeParser-364"><a href="#TypeParser-364"><span class="linenos">364</span></a>
-</span><span id="TypeParser-365"><a href="#TypeParser-365"><span class="linenos">365</span></a>	<span class="k">def</span> <span class="nf">is_float</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="o">*</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_inf</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_nan</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="TypeParser-366"><a href="#TypeParser-366"><span class="linenos">366</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser-367"><a href="#TypeParser-367"><span class="linenos">367</span></a><span class="sd">			Check if a string represents a float (or equivalently, a Decimal)</span>
-</span><span id="TypeParser-368"><a href="#TypeParser-368"><span class="linenos">368</span></a>
-</span><span id="TypeParser-369"><a href="#TypeParser-369"><span class="linenos">369</span></a><span class="sd">			This function will also return True if the string represents an int.</span>
-</span><span id="TypeParser-370"><a href="#TypeParser-370"><span class="linenos">370</span></a>
-</span><span id="TypeParser-371"><a href="#TypeParser-371"><span class="linenos">371</span></a><span class="sd">			Alias: `is_decimal()`</span>
-</span><span id="TypeParser-372"><a href="#TypeParser-372"><span class="linenos">372</span></a>
-</span><span id="TypeParser-373"><a href="#TypeParser-373"><span class="linenos">373</span></a><span class="sd">			Parameters</span>
-</span><span id="TypeParser-374"><a href="#TypeParser-374"><span class="linenos">374</span></a><span class="sd">			----------</span>
-</span><span id="TypeParser-375"><a href="#TypeParser-375"><span class="linenos">375</span></a><span class="sd">			`value`</span>
-</span><span id="TypeParser-376"><a href="#TypeParser-376"><span class="linenos">376</span></a><span class="sd">			: string to be checked</span>
-</span><span id="TypeParser-377"><a href="#TypeParser-377"><span class="linenos">377</span></a>
-</span><span id="TypeParser-378"><a href="#TypeParser-378"><span class="linenos">378</span></a><span class="sd">			`allow_scientific`</span>
-</span><span id="TypeParser-379"><a href="#TypeParser-379"><span class="linenos">379</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form &lt;code&gt;&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;&lt;/code&gt; will be interpreted as the expression &lt;code&gt;&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)&lt;/code&gt;, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note that &lt;var&gt;X&lt;/var&gt; must be an integer, but can be negative.</span>
-</span><span id="TypeParser-380"><a href="#TypeParser-380"><span class="linenos">380</span></a>
-</span><span id="TypeParser-381"><a href="#TypeParser-381"><span class="linenos">381</span></a><span class="sd">			`allow_inf`</span>
-</span><span id="TypeParser-382"><a href="#TypeParser-382"><span class="linenos">382</span></a><span class="sd">			: whether to accept positive and negative infinity values. If True, strings that match the values in `self.inf_values` (empty by default) are interpreted as infinity, or as negative infinity if prepended by a negative sign. The case sensitivity of this matching depends on `self.float_case_sensitive`, which is False by default.</span>
-</span><span id="TypeParser-383"><a href="#TypeParser-383"><span class="linenos">383</span></a>
-</span><span id="TypeParser-384"><a href="#TypeParser-384"><span class="linenos">384</span></a><span class="sd">			`allow_nan`</span>
-</span><span id="TypeParser-385"><a href="#TypeParser-385"><span class="linenos">385</span></a><span class="sd">			: whether to accept NaN (not a number) representations. If True, strings that match the values in `self.nan_values` (empty by default) are interpeted as NaN. The case sensitivity of this matching depends on `self.float_case_sensitive`, which is False by default.</span>
-</span><span id="TypeParser-386"><a href="#TypeParser-386"><span class="linenos">386</span></a>
-</span><span id="TypeParser-387"><a href="#TypeParser-387"><span class="linenos">387</span></a><span class="sd">			Returns</span>
-</span><span id="TypeParser-388"><a href="#TypeParser-388"><span class="linenos">388</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser-389"><a href="#TypeParser-389"><span class="linenos">389</span></a><span class="sd">			whether it is a float or Decimal</span>
-</span><span id="TypeParser-390"><a href="#TypeParser-390"><span class="linenos">390</span></a>
-</span><span id="TypeParser-391"><a href="#TypeParser-391"><span class="linenos">391</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser-392"><a href="#TypeParser-392"><span class="linenos">392</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser-393"><a href="#TypeParser-393"><span class="linenos">393</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser-394"><a href="#TypeParser-394"><span class="linenos">394</span></a><span class="sd">			parser = TypeParser()</span>
-</span><span id="TypeParser-395"><a href="#TypeParser-395"><span class="linenos">395</span></a><span class="sd">			parser.is_float(&quot;1.&quot;)       # True</span>
-</span><span id="TypeParser-396"><a href="#TypeParser-396"><span class="linenos">396</span></a><span class="sd">			parser.is_float(&quot;12.3e-2&quot;)  # True</span>
-</span><span id="TypeParser-397"><a href="#TypeParser-397"><span class="linenos">397</span></a><span class="sd">			parser.is_float(&quot;abc&quot;)      # False</span>
-</span><span id="TypeParser-398"><a href="#TypeParser-398"><span class="linenos">398</span></a><span class="sd">			parser.is_float(&quot;&quot;)         # False</span>
-</span><span id="TypeParser-399"><a href="#TypeParser-399"><span class="linenos">399</span></a><span class="sd">			```</span>
-</span><span id="TypeParser-400"><a href="#TypeParser-400"><span class="linenos">400</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser-401"><a href="#TypeParser-401"><span class="linenos">401</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">trim</span><span class="p">:</span>
-</span><span id="TypeParser-402"><a href="#TypeParser-402"><span class="linenos">402</span></a>			<span class="n">value</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
-</span><span id="TypeParser-403"><a href="#TypeParser-403"><span class="linenos">403</span></a>
-</span><span id="TypeParser-404"><a href="#TypeParser-404"><span class="linenos">404</span></a>		<span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="o">&gt;</span> <span class="mi">0</span> <span class="ow">and</span> <span class="n">value</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_sign_chars</span><span class="p">:</span>
-</span><span id="TypeParser-405"><a href="#TypeParser-405"><span class="linenos">405</span></a>			<span class="n">value</span> <span class="o">=</span> <span class="n">value</span><span class="p">[</span><span class="mi">1</span><span class="p">:]</span>
-</span><span id="TypeParser-406"><a href="#TypeParser-406"><span class="linenos">406</span></a>
-</span><span id="TypeParser-407"><a href="#TypeParser-407"><span class="linenos">407</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">float_case_sensitive</span><span class="p">:</span>
-</span><span id="TypeParser-408"><a href="#TypeParser-408"><span class="linenos">408</span></a>			<span class="n">special_value</span> <span class="o">=</span> <span class="n">value</span>
-</span><span id="TypeParser-409"><a href="#TypeParser-409"><span class="linenos">409</span></a>		<span class="k">else</span><span class="p">:</span>
-</span><span id="TypeParser-410"><a href="#TypeParser-410"><span class="linenos">410</span></a>			<span class="n">special_value</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span>
-</span><span id="TypeParser-411"><a href="#TypeParser-411"><span class="linenos">411</span></a>		<span class="k">if</span> <span class="n">allow_inf</span> <span class="ow">and</span> <span class="n">special_value</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">inf_values</span><span class="p">:</span>
-</span><span id="TypeParser-412"><a href="#TypeParser-412"><span class="linenos">412</span></a>			<span class="k">return</span> <span class="kc">True</span>
-</span><span id="TypeParser-413"><a href="#TypeParser-413"><span class="linenos">413</span></a>		<span class="k">if</span> <span class="n">allow_nan</span> <span class="ow">and</span> <span class="n">special_value</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">nan_values</span><span class="p">:</span>
-</span><span id="TypeParser-414"><a href="#TypeParser-414"><span class="linenos">414</span></a>			<span class="k">return</span> <span class="kc">True</span>
-</span><span id="TypeParser-415"><a href="#TypeParser-415"><span class="linenos">415</span></a>
-</span><span id="TypeParser-416"><a href="#TypeParser-416"><span class="linenos">416</span></a>		<span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="TypeParser-417"><a href="#TypeParser-417"><span class="linenos">417</span></a>			<span class="k">return</span> <span class="kc">False</span>
-</span><span id="TypeParser-418"><a href="#TypeParser-418"><span class="linenos">418</span></a>
-</span><span id="TypeParser-419"><a href="#TypeParser-419"><span class="linenos">419</span></a>		<span class="k">if</span> <span class="n">allow_scientific</span><span class="p">:</span>
-</span><span id="TypeParser-420"><a href="#TypeParser-420"><span class="linenos">420</span></a>			<span class="n">value</span><span class="p">,</span> <span class="n">exp</span> <span class="o">=</span> <span class="n">_decompose_string_pair</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_scientific_char</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">float_case_sensitive</span><span class="p">)</span>
-</span><span id="TypeParser-421"><a href="#TypeParser-421"><span class="linenos">421</span></a>			<span class="k">if</span> <span class="n">exp</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="TypeParser-422"><a href="#TypeParser-422"><span class="linenos">422</span></a>				<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_float</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="o">=</span><span class="kc">False</span><span class="p">,</span> <span class="n">allow_inf</span><span class="o">=</span><span class="kc">False</span><span class="p">,</span> <span class="n">allow_nan</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_int</span><span class="p">(</span><span class="n">exp</span><span class="p">,</span> <span class="n">allow_sign</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_negative</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
-</span><span id="TypeParser-423"><a href="#TypeParser-423"><span class="linenos">423</span></a>
-</span><span id="TypeParser-424"><a href="#TypeParser-424"><span class="linenos">424</span></a>		<span class="n">value</span><span class="p">,</span> <span class="n">frac</span> <span class="o">=</span> <span class="n">_decompose_string_pair</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_float_separator</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">float_case_sensitive</span><span class="p">)</span>
-</span><span id="TypeParser-425"><a href="#TypeParser-425"><span class="linenos">425</span></a>		<span class="k">if</span> <span class="n">frac</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="TypeParser-426"><a href="#TypeParser-426"><span class="linenos">426</span></a>			<span class="k">if</span> <span class="n">value</span> <span class="o">==</span> <span class="s2">&quot;&quot;</span> <span class="ow">and</span> <span class="n">frac</span> <span class="o">==</span> <span class="s2">&quot;&quot;</span><span class="p">:</span>
-</span><span id="TypeParser-427"><a href="#TypeParser-427"><span class="linenos">427</span></a>				<span class="k">return</span> <span class="kc">False</span>
-</span><span id="TypeParser-428"><a href="#TypeParser-428"><span class="linenos">428</span></a>			<span class="k">return</span> <span class="p">(</span>
-</span><span id="TypeParser-429"><a href="#TypeParser-429"><span class="linenos">429</span></a>				<span class="bp">self</span><span class="o">.</span><span class="n">is_int</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">allow_sign</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_negative</span><span class="o">=</span><span class="kc">False</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span> <span class="ow">or</span> <span class="n">value</span> <span class="o">==</span> <span class="s2">&quot;&quot;</span>
-</span><span id="TypeParser-430"><a href="#TypeParser-430"><span class="linenos">430</span></a>			<span class="p">)</span> <span class="ow">and</span> <span class="p">(</span>
-</span><span id="TypeParser-431"><a href="#TypeParser-431"><span class="linenos">431</span></a>				<span class="bp">self</span><span class="o">.</span><span class="n">is_int</span><span class="p">(</span><span class="n">frac</span><span class="p">,</span> <span class="n">allow_sign</span><span class="o">=</span><span class="kc">False</span><span class="p">,</span> <span class="n">allow_negative</span><span class="o">=</span><span class="kc">False</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span> <span class="ow">or</span> <span class="n">frac</span> <span class="o">==</span> <span class="s2">&quot;&quot;</span>
-</span><span id="TypeParser-432"><a href="#TypeParser-432"><span class="linenos">432</span></a>			<span class="p">)</span>
-</span><span id="TypeParser-433"><a href="#TypeParser-433"><span class="linenos">433</span></a>
-</span><span id="TypeParser-434"><a href="#TypeParser-434"><span class="linenos">434</span></a>		<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_int</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">allow_sign</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_negative</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
-</span><span id="TypeParser-435"><a href="#TypeParser-435"><span class="linenos">435</span></a>
-</span><span id="TypeParser-436"><a href="#TypeParser-436"><span class="linenos">436</span></a>
-</span><span id="TypeParser-437"><a href="#TypeParser-437"><span class="linenos">437</span></a>	<span class="k">def</span> <span class="nf">is_decimal</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="o">*</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_inf</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_nan</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="TypeParser-438"><a href="#TypeParser-438"><span class="linenos">438</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser-439"><a href="#TypeParser-439"><span class="linenos">439</span></a><span class="sd">			Alias of `is_float()`</span>
-</span><span id="TypeParser-440"><a href="#TypeParser-440"><span class="linenos">440</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser-441"><a href="#TypeParser-441"><span class="linenos">441</span></a>		<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_float</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="o">=</span><span class="n">allow_scientific</span><span class="p">,</span> <span class="n">allow_inf</span><span class="o">=</span><span class="n">allow_inf</span><span class="p">,</span> <span class="n">allow_nan</span><span class="o">=</span><span class="n">allow_nan</span><span class="p">)</span>
-</span><span id="TypeParser-442"><a href="#TypeParser-442"><span class="linenos">442</span></a>
-</span><span id="TypeParser-443"><a href="#TypeParser-443"><span class="linenos">443</span></a>
-</span><span id="TypeParser-444"><a href="#TypeParser-444"><span class="linenos">444</span></a>	<span class="k">def</span> <span class="nf">parse_none</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="TypeParser-445"><a href="#TypeParser-445"><span class="linenos">445</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser-446"><a href="#TypeParser-446"><span class="linenos">446</span></a><span class="sd">			Parse a string and return it as the value None if possible</span>
-</span><span id="TypeParser-447"><a href="#TypeParser-447"><span class="linenos">447</span></a>
-</span><span id="TypeParser-448"><a href="#TypeParser-448"><span class="linenos">448</span></a><span class="sd">			Only strings that match the values in `self.none_values` will be interpreted as None. The default accepted values are `[&quot;&quot;]`, i.e. an empty string. The case sensitivity of this matching depends on `self.none_case_sensitive`, which is False by default.</span>
-</span><span id="TypeParser-449"><a href="#TypeParser-449"><span class="linenos">449</span></a>
-</span><span id="TypeParser-450"><a href="#TypeParser-450"><span class="linenos">450</span></a><span class="sd">			Parameters</span>
-</span><span id="TypeParser-451"><a href="#TypeParser-451"><span class="linenos">451</span></a><span class="sd">			----------</span>
-</span><span id="TypeParser-452"><a href="#TypeParser-452"><span class="linenos">452</span></a><span class="sd">			`value`</span>
-</span><span id="TypeParser-453"><a href="#TypeParser-453"><span class="linenos">453</span></a><span class="sd">			: string to be parsed</span>
-</span><span id="TypeParser-454"><a href="#TypeParser-454"><span class="linenos">454</span></a>
-</span><span id="TypeParser-455"><a href="#TypeParser-455"><span class="linenos">455</span></a><span class="sd">			Returns</span>
-</span><span id="TypeParser-456"><a href="#TypeParser-456"><span class="linenos">456</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser-457"><a href="#TypeParser-457"><span class="linenos">457</span></a><span class="sd">			parsed None value</span>
-</span><span id="TypeParser-458"><a href="#TypeParser-458"><span class="linenos">458</span></a>
-</span><span id="TypeParser-459"><a href="#TypeParser-459"><span class="linenos">459</span></a><span class="sd">			Raises</span>
-</span><span id="TypeParser-460"><a href="#TypeParser-460"><span class="linenos">460</span></a><span class="sd">			------</span>
-</span><span id="TypeParser-461"><a href="#TypeParser-461"><span class="linenos">461</span></a><span class="sd">			`ValueError` if `value` cannot be parsed</span>
-</span><span id="TypeParser-462"><a href="#TypeParser-462"><span class="linenos">462</span></a>
-</span><span id="TypeParser-463"><a href="#TypeParser-463"><span class="linenos">463</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser-464"><a href="#TypeParser-464"><span class="linenos">464</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser-465"><a href="#TypeParser-465"><span class="linenos">465</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser-466"><a href="#TypeParser-466"><span class="linenos">466</span></a><span class="sd">			parser = TypeParser()</span>
-</span><span id="TypeParser-467"><a href="#TypeParser-467"><span class="linenos">467</span></a><span class="sd">			parser.parse_bool(&quot;&quot;)     # None</span>
-</span><span id="TypeParser-468"><a href="#TypeParser-468"><span class="linenos">468</span></a><span class="sd">			parser.parse_bool(&quot;abc&quot;)  # raises ValueError</span>
-</span><span id="TypeParser-469"><a href="#TypeParser-469"><span class="linenos">469</span></a><span class="sd">			```</span>
-</span><span id="TypeParser-470"><a href="#TypeParser-470"><span class="linenos">470</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser-471"><a href="#TypeParser-471"><span class="linenos">471</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_none</span><span class="p">(</span><span class="n">value</span><span class="p">):</span>
-</span><span id="TypeParser-472"><a href="#TypeParser-472"><span class="linenos">472</span></a>			<span class="k">return</span> <span class="kc">None</span>
-</span><span id="TypeParser-473"><a href="#TypeParser-473"><span class="linenos">473</span></a>		<span class="k">else</span><span class="p">:</span>
-</span><span id="TypeParser-474"><a href="#TypeParser-474"><span class="linenos">474</span></a>			<span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;not a none value: </span><span class="si">{</span><span class="n">value</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="TypeParser-475"><a href="#TypeParser-475"><span class="linenos">475</span></a>
-</span><span id="TypeParser-476"><a href="#TypeParser-476"><span class="linenos">476</span></a>
-</span><span id="TypeParser-477"><a href="#TypeParser-477"><span class="linenos">477</span></a>	<span class="k">def</span> <span class="nf">parse_bool</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="TypeParser-478"><a href="#TypeParser-478"><span class="linenos">478</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser-479"><a href="#TypeParser-479"><span class="linenos">479</span></a><span class="sd">			Parse a string and return it as a bool if possible</span>
-</span><span id="TypeParser-480"><a href="#TypeParser-480"><span class="linenos">480</span></a>
-</span><span id="TypeParser-481"><a href="#TypeParser-481"><span class="linenos">481</span></a><span class="sd">			Only strings that match the values in `self.true_values` and `self.false_values` will be interpreted as booleans. The default accepted values are `[&quot;true&quot;]` and `[&quot;false&quot;]` respectively. The case sensitivity of this matching depends on `self.bool_case_sensitive`, which is False by default.</span>
-</span><span id="TypeParser-482"><a href="#TypeParser-482"><span class="linenos">482</span></a>
-</span><span id="TypeParser-483"><a href="#TypeParser-483"><span class="linenos">483</span></a><span class="sd">			Parameters</span>
-</span><span id="TypeParser-484"><a href="#TypeParser-484"><span class="linenos">484</span></a><span class="sd">			----------</span>
-</span><span id="TypeParser-485"><a href="#TypeParser-485"><span class="linenos">485</span></a><span class="sd">			`value`</span>
-</span><span id="TypeParser-486"><a href="#TypeParser-486"><span class="linenos">486</span></a><span class="sd">			: string to be parsed</span>
-</span><span id="TypeParser-487"><a href="#TypeParser-487"><span class="linenos">487</span></a>
-</span><span id="TypeParser-488"><a href="#TypeParser-488"><span class="linenos">488</span></a><span class="sd">			Returns</span>
-</span><span id="TypeParser-489"><a href="#TypeParser-489"><span class="linenos">489</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser-490"><a href="#TypeParser-490"><span class="linenos">490</span></a><span class="sd">			parsed bool value</span>
-</span><span id="TypeParser-491"><a href="#TypeParser-491"><span class="linenos">491</span></a>
-</span><span id="TypeParser-492"><a href="#TypeParser-492"><span class="linenos">492</span></a><span class="sd">			Raises</span>
-</span><span id="TypeParser-493"><a href="#TypeParser-493"><span class="linenos">493</span></a><span class="sd">			------</span>
-</span><span id="TypeParser-494"><a href="#TypeParser-494"><span class="linenos">494</span></a><span class="sd">			`ValueError` if `value` cannot be parsed</span>
-</span><span id="TypeParser-495"><a href="#TypeParser-495"><span class="linenos">495</span></a>
-</span><span id="TypeParser-496"><a href="#TypeParser-496"><span class="linenos">496</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser-497"><a href="#TypeParser-497"><span class="linenos">497</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser-498"><a href="#TypeParser-498"><span class="linenos">498</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser-499"><a href="#TypeParser-499"><span class="linenos">499</span></a><span class="sd">			parser = TypeParser()</span>
-</span><span id="TypeParser-500"><a href="#TypeParser-500"><span class="linenos">500</span></a><span class="sd">			parser.parse_bool(&quot;true&quot;)   # True</span>
-</span><span id="TypeParser-501"><a href="#TypeParser-501"><span class="linenos">501</span></a><span class="sd">			parser.parse_bool(&quot;FALSE&quot;)  # False</span>
-</span><span id="TypeParser-502"><a href="#TypeParser-502"><span class="linenos">502</span></a><span class="sd">			```</span>
-</span><span id="TypeParser-503"><a href="#TypeParser-503"><span class="linenos">503</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser-504"><a href="#TypeParser-504"><span class="linenos">504</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">trim</span><span class="p">:</span>
-</span><span id="TypeParser-505"><a href="#TypeParser-505"><span class="linenos">505</span></a>			<span class="n">value</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
-</span><span id="TypeParser-506"><a href="#TypeParser-506"><span class="linenos">506</span></a>
-</span><span id="TypeParser-507"><a href="#TypeParser-507"><span class="linenos">507</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">bool_case_sensitive</span><span class="p">:</span>
-</span><span id="TypeParser-508"><a href="#TypeParser-508"><span class="linenos">508</span></a>			<span class="n">special_value</span> <span class="o">=</span> <span class="n">value</span>
-</span><span id="TypeParser-509"><a href="#TypeParser-509"><span class="linenos">509</span></a>		<span class="k">else</span><span class="p">:</span>
-</span><span id="TypeParser-510"><a href="#TypeParser-510"><span class="linenos">510</span></a>			<span class="n">special_value</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span>
-</span><span id="TypeParser-511"><a href="#TypeParser-511"><span class="linenos">511</span></a>		<span class="k">if</span> <span class="n">special_value</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">true_values</span><span class="p">:</span>
-</span><span id="TypeParser-512"><a href="#TypeParser-512"><span class="linenos">512</span></a>			<span class="k">return</span> <span class="kc">True</span>
-</span><span id="TypeParser-513"><a href="#TypeParser-513"><span class="linenos">513</span></a>		<span class="k">if</span> <span class="n">special_value</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">false_values</span><span class="p">:</span>
-</span><span id="TypeParser-514"><a href="#TypeParser-514"><span class="linenos">514</span></a>			<span class="k">return</span> <span class="kc">False</span>
-</span><span id="TypeParser-515"><a href="#TypeParser-515"><span class="linenos">515</span></a>
-</span><span id="TypeParser-516"><a href="#TypeParser-516"><span class="linenos">516</span></a>		<span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;not a boolean: </span><span class="si">{</span><span class="n">value</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="TypeParser-517"><a href="#TypeParser-517"><span class="linenos">517</span></a>
-</span><span id="TypeParser-518"><a href="#TypeParser-518"><span class="linenos">518</span></a>
-</span><span id="TypeParser-519"><a href="#TypeParser-519"><span class="linenos">519</span></a>	<span class="k">def</span> <span class="nf">parse_int</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="o">*</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="TypeParser-520"><a href="#TypeParser-520"><span class="linenos">520</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser-521"><a href="#TypeParser-521"><span class="linenos">521</span></a><span class="sd">			Parse a string and return it as an int if possible</span>
-</span><span id="TypeParser-522"><a href="#TypeParser-522"><span class="linenos">522</span></a>
-</span><span id="TypeParser-523"><a href="#TypeParser-523"><span class="linenos">523</span></a><span class="sd">			If the string represents a bool, it will be converted to `1` for True and `0` for False.</span>
-</span><span id="TypeParser-524"><a href="#TypeParser-524"><span class="linenos">524</span></a>
-</span><span id="TypeParser-525"><a href="#TypeParser-525"><span class="linenos">525</span></a><span class="sd">			Parameters</span>
-</span><span id="TypeParser-526"><a href="#TypeParser-526"><span class="linenos">526</span></a><span class="sd">			----------</span>
-</span><span id="TypeParser-527"><a href="#TypeParser-527"><span class="linenos">527</span></a><span class="sd">			`value`</span>
-</span><span id="TypeParser-528"><a href="#TypeParser-528"><span class="linenos">528</span></a><span class="sd">			: string to be parsed</span>
-</span><span id="TypeParser-529"><a href="#TypeParser-529"><span class="linenos">529</span></a>
-</span><span id="TypeParser-530"><a href="#TypeParser-530"><span class="linenos">530</span></a><span class="sd">			`allow_scientific`</span>
-</span><span id="TypeParser-531"><a href="#TypeParser-531"><span class="linenos">531</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form &lt;code&gt;&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;&lt;/code&gt; will be interpreted as the expression &lt;code&gt;&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)&lt;/code&gt;, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note &lt;var&gt;M&lt;/var&gt; *must* be an integer and &lt;var&gt;X&lt;/var&gt; *must* be a non-negative integer, even in cases where the above expression evaluates mathematically to an integer.</span>
-</span><span id="TypeParser-532"><a href="#TypeParser-532"><span class="linenos">532</span></a>
-</span><span id="TypeParser-533"><a href="#TypeParser-533"><span class="linenos">533</span></a><span class="sd">			Returns</span>
-</span><span id="TypeParser-534"><a href="#TypeParser-534"><span class="linenos">534</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser-535"><a href="#TypeParser-535"><span class="linenos">535</span></a><span class="sd">			parsed int value</span>
-</span><span id="TypeParser-536"><a href="#TypeParser-536"><span class="linenos">536</span></a>
-</span><span id="TypeParser-537"><a href="#TypeParser-537"><span class="linenos">537</span></a><span class="sd">			Raises</span>
-</span><span id="TypeParser-538"><a href="#TypeParser-538"><span class="linenos">538</span></a><span class="sd">			------</span>
-</span><span id="TypeParser-539"><a href="#TypeParser-539"><span class="linenos">539</span></a><span class="sd">			`ValueError` if `value` cannot be parsed</span>
-</span><span id="TypeParser-540"><a href="#TypeParser-540"><span class="linenos">540</span></a>
-</span><span id="TypeParser-541"><a href="#TypeParser-541"><span class="linenos">541</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser-542"><a href="#TypeParser-542"><span class="linenos">542</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser-543"><a href="#TypeParser-543"><span class="linenos">543</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser-544"><a href="#TypeParser-544"><span class="linenos">544</span></a><span class="sd">			parser = TypeParser()</span>
-</span><span id="TypeParser-545"><a href="#TypeParser-545"><span class="linenos">545</span></a><span class="sd">			parser.parse_int(&quot;0&quot;)    # 0</span>
-</span><span id="TypeParser-546"><a href="#TypeParser-546"><span class="linenos">546</span></a><span class="sd">			parser.parse_int(&quot;-1&quot;)   # -1</span>
-</span><span id="TypeParser-547"><a href="#TypeParser-547"><span class="linenos">547</span></a><span class="sd">			parser.parse_int(&quot;2e3&quot;)  # 2000</span>
-</span><span id="TypeParser-548"><a href="#TypeParser-548"><span class="linenos">548</span></a><span class="sd">			```</span>
-</span><span id="TypeParser-549"><a href="#TypeParser-549"><span class="linenos">549</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser-550"><a href="#TypeParser-550"><span class="linenos">550</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">trim</span><span class="p">:</span>
-</span><span id="TypeParser-551"><a href="#TypeParser-551"><span class="linenos">551</span></a>			<span class="n">value</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
-</span><span id="TypeParser-552"><a href="#TypeParser-552"><span class="linenos">552</span></a>
-</span><span id="TypeParser-553"><a href="#TypeParser-553"><span class="linenos">553</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_int</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">allow_sign</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_negative</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="o">=</span><span class="n">allow_scientific</span><span class="p">):</span>
-</span><span id="TypeParser-554"><a href="#TypeParser-554"><span class="linenos">554</span></a>			<span class="k">if</span> <span class="n">allow_scientific</span><span class="p">:</span>
-</span><span id="TypeParser-555"><a href="#TypeParser-555"><span class="linenos">555</span></a>				<span class="n">value</span><span class="p">,</span> <span class="n">exp</span> <span class="o">=</span> <span class="n">_decompose_string_pair</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_scientific_char</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">int_case_sensitive</span><span class="p">)</span>
-</span><span id="TypeParser-556"><a href="#TypeParser-556"><span class="linenos">556</span></a>				<span class="k">if</span> <span class="n">exp</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="TypeParser-557"><a href="#TypeParser-557"><span class="linenos">557</span></a>					<span class="k">if</span> <span class="n">value</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="ow">in</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_negative_chars</span> <span class="o">-</span> <span class="p">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_negative_char</span><span class="p">}):</span>
-</span><span id="TypeParser-558"><a href="#TypeParser-558"><span class="linenos">558</span></a>						<span class="n">value</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_negative_char</span> <span class="o">+</span> <span class="n">value</span><span class="p">[</span><span class="mi">1</span><span class="p">:]</span>
-</span><span id="TypeParser-559"><a href="#TypeParser-559"><span class="linenos">559</span></a>					<span class="k">return</span> <span class="nb">int</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="o">*</span> <span class="p">(</span><span class="mi">10</span> <span class="o">**</span> <span class="nb">int</span><span class="p">(</span><span class="n">exp</span><span class="p">))</span>
-</span><span id="TypeParser-560"><a href="#TypeParser-560"><span class="linenos">560</span></a>
-</span><span id="TypeParser-561"><a href="#TypeParser-561"><span class="linenos">561</span></a>			<span class="k">if</span> <span class="n">value</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="ow">in</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_negative_chars</span> <span class="o">-</span> <span class="p">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_negative_char</span><span class="p">}):</span>
-</span><span id="TypeParser-562"><a href="#TypeParser-562"><span class="linenos">562</span></a>				<span class="n">value</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_negative_char</span> <span class="o">+</span> <span class="n">value</span><span class="p">[</span><span class="mi">1</span><span class="p">:]</span>
-</span><span id="TypeParser-563"><a href="#TypeParser-563"><span class="linenos">563</span></a>			<span class="k">return</span> <span class="nb">int</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
-</span><span id="TypeParser-564"><a href="#TypeParser-564"><span class="linenos">564</span></a>
-</span><span id="TypeParser-565"><a href="#TypeParser-565"><span class="linenos">565</span></a>		<span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_bool</span><span class="p">(</span><span class="n">value</span><span class="p">):</span>
-</span><span id="TypeParser-566"><a href="#TypeParser-566"><span class="linenos">566</span></a>			<span class="k">return</span> <span class="nb">int</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">parse_bool</span><span class="p">(</span><span class="n">value</span><span class="p">))</span>
-</span><span id="TypeParser-567"><a href="#TypeParser-567"><span class="linenos">567</span></a>		<span class="k">else</span><span class="p">:</span>
-</span><span id="TypeParser-568"><a href="#TypeParser-568"><span class="linenos">568</span></a>			<span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;not an integer: </span><span class="si">{</span><span class="n">value</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="TypeParser-569"><a href="#TypeParser-569"><span class="linenos">569</span></a>
-</span><span id="TypeParser-570"><a href="#TypeParser-570"><span class="linenos">570</span></a>
-</span><span id="TypeParser-571"><a href="#TypeParser-571"><span class="linenos">571</span></a>	<span class="k">def</span> <span class="nf">_parse_floatlike</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span>
-</span><span id="TypeParser-572"><a href="#TypeParser-572"><span class="linenos">572</span></a>		<span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
-</span><span id="TypeParser-573"><a href="#TypeParser-573"><span class="linenos">573</span></a>		<span class="n">converter</span><span class="p">:</span> <span class="n">Callable</span><span class="p">[[</span><span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">bool</span><span class="p">]],</span> <span class="n">_FloatLike</span><span class="p">],</span>
-</span><span id="TypeParser-574"><a href="#TypeParser-574"><span class="linenos">574</span></a>		<span class="n">inf_value</span><span class="p">:</span> <span class="n">_FloatLike</span><span class="p">,</span>
-</span><span id="TypeParser-575"><a href="#TypeParser-575"><span class="linenos">575</span></a>		<span class="n">nan_value</span><span class="p">:</span> <span class="n">_FloatLike</span><span class="p">,</span>
-</span><span id="TypeParser-576"><a href="#TypeParser-576"><span class="linenos">576</span></a>		<span class="o">*</span><span class="p">,</span>
-</span><span id="TypeParser-577"><a href="#TypeParser-577"><span class="linenos">577</span></a>		<span class="n">allow_scientific</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
-</span><span id="TypeParser-578"><a href="#TypeParser-578"><span class="linenos">578</span></a>		<span class="n">allow_inf</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
-</span><span id="TypeParser-579"><a href="#TypeParser-579"><span class="linenos">579</span></a>		<span class="n">allow_nan</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span>
-</span><span id="TypeParser-580"><a href="#TypeParser-580"><span class="linenos">580</span></a>	<span class="p">)</span> <span class="o">-&gt;</span> <span class="n">_FloatLike</span><span class="p">:</span>
-</span><span id="TypeParser-581"><a href="#TypeParser-581"><span class="linenos">581</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">trim</span><span class="p">:</span>
-</span><span id="TypeParser-582"><a href="#TypeParser-582"><span class="linenos">582</span></a>			<span class="n">value</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
-</span><span id="TypeParser-583"><a href="#TypeParser-583"><span class="linenos">583</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_float</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="o">=</span><span class="n">allow_scientific</span><span class="p">,</span> <span class="n">allow_inf</span><span class="o">=</span><span class="n">allow_inf</span><span class="p">,</span> <span class="n">allow_nan</span><span class="o">=</span><span class="n">allow_nan</span><span class="p">):</span>
-</span><span id="TypeParser-584"><a href="#TypeParser-584"><span class="linenos">584</span></a>			<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">float_case_sensitive</span><span class="p">:</span>
-</span><span id="TypeParser-585"><a href="#TypeParser-585"><span class="linenos">585</span></a>				<span class="n">special_value</span> <span class="o">=</span> <span class="n">value</span>
-</span><span id="TypeParser-586"><a href="#TypeParser-586"><span class="linenos">586</span></a>			<span class="k">else</span><span class="p">:</span>
-</span><span id="TypeParser-587"><a href="#TypeParser-587"><span class="linenos">587</span></a>				<span class="n">special_value</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span>
-</span><span id="TypeParser-588"><a href="#TypeParser-588"><span class="linenos">588</span></a>			<span class="k">if</span> <span class="n">allow_inf</span> <span class="ow">and</span> <span class="n">special_value</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">inf_values</span><span class="p">:</span>
-</span><span id="TypeParser-589"><a href="#TypeParser-589"><span class="linenos">589</span></a>				<span class="k">return</span> <span class="n">inf_value</span>
-</span><span id="TypeParser-590"><a href="#TypeParser-590"><span class="linenos">590</span></a>			<span class="k">if</span> <span class="n">allow_nan</span> <span class="ow">and</span> <span class="n">special_value</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">nan_values</span><span class="p">:</span>
-</span><span id="TypeParser-591"><a href="#TypeParser-591"><span class="linenos">591</span></a>				<span class="k">return</span> <span class="n">nan_value</span>
-</span><span id="TypeParser-592"><a href="#TypeParser-592"><span class="linenos">592</span></a>
-</span><span id="TypeParser-593"><a href="#TypeParser-593"><span class="linenos">593</span></a>			<span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="o">&gt;</span> <span class="mi">0</span> <span class="ow">and</span> <span class="n">value</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_sign_chars</span><span class="p">:</span>
-</span><span id="TypeParser-594"><a href="#TypeParser-594"><span class="linenos">594</span></a>				<span class="n">positive_part</span> <span class="o">=</span> <span class="n">value</span><span class="p">[</span><span class="mi">1</span><span class="p">:]</span>
-</span><span id="TypeParser-595"><a href="#TypeParser-595"><span class="linenos">595</span></a>				<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">float_case_sensitive</span><span class="p">:</span>
-</span><span id="TypeParser-596"><a href="#TypeParser-596"><span class="linenos">596</span></a>					<span class="n">special_value</span> <span class="o">=</span> <span class="n">positive_part</span>
-</span><span id="TypeParser-597"><a href="#TypeParser-597"><span class="linenos">597</span></a>				<span class="k">else</span><span class="p">:</span>
-</span><span id="TypeParser-598"><a href="#TypeParser-598"><span class="linenos">598</span></a>					<span class="n">special_value</span> <span class="o">=</span> <span class="n">positive_part</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span>
-</span><span id="TypeParser-599"><a href="#TypeParser-599"><span class="linenos">599</span></a>				<span class="k">if</span> <span class="n">allow_inf</span> <span class="ow">and</span> <span class="n">special_value</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">inf_values</span><span class="p">:</span>
-</span><span id="TypeParser-600"><a href="#TypeParser-600"><span class="linenos">600</span></a>					<span class="k">if</span> <span class="n">value</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_negative_chars</span><span class="p">:</span>
-</span><span id="TypeParser-601"><a href="#TypeParser-601"><span class="linenos">601</span></a>						<span class="k">return</span> <span class="o">-</span><span class="mi">1</span> <span class="o">*</span> <span class="n">inf_value</span>
-</span><span id="TypeParser-602"><a href="#TypeParser-602"><span class="linenos">602</span></a>					<span class="k">else</span><span class="p">:</span>
-</span><span id="TypeParser-603"><a href="#TypeParser-603"><span class="linenos">603</span></a>						<span class="k">return</span> <span class="n">inf_value</span>
-</span><span id="TypeParser-604"><a href="#TypeParser-604"><span class="linenos">604</span></a>				<span class="k">if</span> <span class="n">allow_nan</span> <span class="ow">and</span> <span class="n">special_value</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">nan_values</span><span class="p">:</span>
-</span><span id="TypeParser-605"><a href="#TypeParser-605"><span class="linenos">605</span></a>					<span class="k">return</span> <span class="n">nan_value</span>
-</span><span id="TypeParser-606"><a href="#TypeParser-606"><span class="linenos">606</span></a>
-</span><span id="TypeParser-607"><a href="#TypeParser-607"><span class="linenos">607</span></a>				<span class="k">if</span> <span class="n">value</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_negative_chars</span><span class="p">:</span>
-</span><span id="TypeParser-608"><a href="#TypeParser-608"><span class="linenos">608</span></a>					<span class="n">value</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_negative_char</span> <span class="o">+</span> <span class="n">positive_part</span>
-</span><span id="TypeParser-609"><a href="#TypeParser-609"><span class="linenos">609</span></a>			<span class="k">return</span> <span class="n">converter</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
-</span><span id="TypeParser-610"><a href="#TypeParser-610"><span class="linenos">610</span></a>		<span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_bool</span><span class="p">(</span><span class="n">value</span><span class="p">):</span>
-</span><span id="TypeParser-611"><a href="#TypeParser-611"><span class="linenos">611</span></a>			<span class="k">return</span> <span class="n">converter</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">parse_bool</span><span class="p">(</span><span class="n">value</span><span class="p">))</span>
-</span><span id="TypeParser-612"><a href="#TypeParser-612"><span class="linenos">612</span></a>		<span class="k">else</span><span class="p">:</span>
-</span><span id="TypeParser-613"><a href="#TypeParser-613"><span class="linenos">613</span></a>			<span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;not a </span><span class="si">{</span><span class="n">_FloatLike</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">value</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="TypeParser-614"><a href="#TypeParser-614"><span class="linenos">614</span></a>
-</span><span id="TypeParser-615"><a href="#TypeParser-615"><span class="linenos">615</span></a>
-</span><span id="TypeParser-616"><a href="#TypeParser-616"><span class="linenos">616</span></a>	<span class="k">def</span> <span class="nf">parse_float</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="o">*</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_inf</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_nan</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
-</span><span id="TypeParser-617"><a href="#TypeParser-617"><span class="linenos">617</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser-618"><a href="#TypeParser-618"><span class="linenos">618</span></a><span class="sd">			Parse a string and return it as a (non-exact) float if possible</span>
-</span><span id="TypeParser-619"><a href="#TypeParser-619"><span class="linenos">619</span></a>
-</span><span id="TypeParser-620"><a href="#TypeParser-620"><span class="linenos">620</span></a><span class="sd">			If the string represents a bool, it will be converted to `1.` for True and `0.` for False. If the string represents an int, it will be converted to a float also.</span>
-</span><span id="TypeParser-621"><a href="#TypeParser-621"><span class="linenos">621</span></a>
-</span><span id="TypeParser-622"><a href="#TypeParser-622"><span class="linenos">622</span></a><span class="sd">			Behaves analogously to `parse_decimal()`, except that that returns an exact Decimal instead.</span>
-</span><span id="TypeParser-623"><a href="#TypeParser-623"><span class="linenos">623</span></a>
-</span><span id="TypeParser-624"><a href="#TypeParser-624"><span class="linenos">624</span></a><span class="sd">			Parameters</span>
-</span><span id="TypeParser-625"><a href="#TypeParser-625"><span class="linenos">625</span></a><span class="sd">			----------</span>
-</span><span id="TypeParser-626"><a href="#TypeParser-626"><span class="linenos">626</span></a><span class="sd">			`value`</span>
-</span><span id="TypeParser-627"><a href="#TypeParser-627"><span class="linenos">627</span></a><span class="sd">			: string to be parsed</span>
-</span><span id="TypeParser-628"><a href="#TypeParser-628"><span class="linenos">628</span></a>
-</span><span id="TypeParser-629"><a href="#TypeParser-629"><span class="linenos">629</span></a><span class="sd">			`allow_scientific`</span>
-</span><span id="TypeParser-630"><a href="#TypeParser-630"><span class="linenos">630</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form &lt;code&gt;&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;&lt;/code&gt; will be interpreted as the expression &lt;code&gt;&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)&lt;/code&gt;, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note that &lt;var&gt;X&lt;/var&gt; must be an integer, but can be negative.</span>
-</span><span id="TypeParser-631"><a href="#TypeParser-631"><span class="linenos">631</span></a>
-</span><span id="TypeParser-632"><a href="#TypeParser-632"><span class="linenos">632</span></a><span class="sd">			`allow_inf`</span>
-</span><span id="TypeParser-633"><a href="#TypeParser-633"><span class="linenos">633</span></a><span class="sd">			: whether to accept positive and negative infinity values. If True, strings that match the values in `self.inf_values` (empty by default) are interpreted as infinity, or as negative infinity if prepended by a negative sign. The case sensitivity of this matching depends on `self.float_case_sensitive`, which is False by default.</span>
-</span><span id="TypeParser-634"><a href="#TypeParser-634"><span class="linenos">634</span></a>
-</span><span id="TypeParser-635"><a href="#TypeParser-635"><span class="linenos">635</span></a><span class="sd">			`allow_nan`</span>
-</span><span id="TypeParser-636"><a href="#TypeParser-636"><span class="linenos">636</span></a><span class="sd">			: whether to accept NaN (not a number) representations. If True, strings that match the values in `self.nan_values` (empty by default) are interpeted as NaN. The case sensitivity of this matching depends on `self.float_case_sensitive`, which is False by default.</span>
-</span><span id="TypeParser-637"><a href="#TypeParser-637"><span class="linenos">637</span></a>
-</span><span id="TypeParser-638"><a href="#TypeParser-638"><span class="linenos">638</span></a><span class="sd">			Returns</span>
-</span><span id="TypeParser-639"><a href="#TypeParser-639"><span class="linenos">639</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser-640"><a href="#TypeParser-640"><span class="linenos">640</span></a><span class="sd">			parsed float value</span>
-</span><span id="TypeParser-641"><a href="#TypeParser-641"><span class="linenos">641</span></a>
-</span><span id="TypeParser-642"><a href="#TypeParser-642"><span class="linenos">642</span></a><span class="sd">			Raises</span>
-</span><span id="TypeParser-643"><a href="#TypeParser-643"><span class="linenos">643</span></a><span class="sd">			------</span>
-</span><span id="TypeParser-644"><a href="#TypeParser-644"><span class="linenos">644</span></a><span class="sd">			`ValueError` if `value` cannot be parsed</span>
-</span><span id="TypeParser-645"><a href="#TypeParser-645"><span class="linenos">645</span></a>
-</span><span id="TypeParser-646"><a href="#TypeParser-646"><span class="linenos">646</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser-647"><a href="#TypeParser-647"><span class="linenos">647</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser-648"><a href="#TypeParser-648"><span class="linenos">648</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser-649"><a href="#TypeParser-649"><span class="linenos">649</span></a><span class="sd">			parser = TypeParser(inf_values=[&quot;inf&quot;], nan_values=[&quot;nan&quot;])</span>
-</span><span id="TypeParser-650"><a href="#TypeParser-650"><span class="linenos">650</span></a><span class="sd">			parser.parse_float(&quot;1.&quot;)       # 1.</span>
-</span><span id="TypeParser-651"><a href="#TypeParser-651"><span class="linenos">651</span></a><span class="sd">			parser.parse_float(&quot;1.23e2&quot;)   # 123.</span>
-</span><span id="TypeParser-652"><a href="#TypeParser-652"><span class="linenos">652</span></a><span class="sd">			parser.parse_float(&quot;1.23e-2&quot;)  # 0.0123</span>
-</span><span id="TypeParser-653"><a href="#TypeParser-653"><span class="linenos">653</span></a><span class="sd">			parser.parse_float(&quot;inf&quot;)      # math.inf</span>
-</span><span id="TypeParser-654"><a href="#TypeParser-654"><span class="linenos">654</span></a><span class="sd">			```</span>
-</span><span id="TypeParser-655"><a href="#TypeParser-655"><span class="linenos">655</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser-656"><a href="#TypeParser-656"><span class="linenos">656</span></a>		<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_parse_floatlike</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">math</span><span class="o">.</span><span class="n">inf</span><span class="p">,</span> <span class="n">math</span><span class="o">.</span><span class="n">nan</span><span class="p">,</span>
-</span><span id="TypeParser-657"><a href="#TypeParser-657"><span class="linenos">657</span></a>			<span class="n">allow_scientific</span><span class="o">=</span><span class="n">allow_scientific</span><span class="p">,</span>
-</span><span id="TypeParser-658"><a href="#TypeParser-658"><span class="linenos">658</span></a>			<span class="n">allow_inf</span><span class="o">=</span><span class="n">allow_inf</span><span class="p">,</span>
-</span><span id="TypeParser-659"><a href="#TypeParser-659"><span class="linenos">659</span></a>			<span class="n">allow_nan</span><span class="o">=</span><span class="n">allow_nan</span><span class="p">,</span>
-</span><span id="TypeParser-660"><a href="#TypeParser-660"><span class="linenos">660</span></a>		<span class="p">)</span>
-</span><span id="TypeParser-661"><a href="#TypeParser-661"><span class="linenos">661</span></a>
-</span><span id="TypeParser-662"><a href="#TypeParser-662"><span class="linenos">662</span></a>
-</span><span id="TypeParser-663"><a href="#TypeParser-663"><span class="linenos">663</span></a>	<span class="k">def</span> <span class="nf">parse_decimal</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="o">*</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_inf</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_nan</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Decimal</span><span class="p">:</span>
-</span><span id="TypeParser-664"><a href="#TypeParser-664"><span class="linenos">664</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser-665"><a href="#TypeParser-665"><span class="linenos">665</span></a><span class="sd">			Parse a string and return it as an exact Decimal if possible</span>
-</span><span id="TypeParser-666"><a href="#TypeParser-666"><span class="linenos">666</span></a>
-</span><span id="TypeParser-667"><a href="#TypeParser-667"><span class="linenos">667</span></a><span class="sd">			If the string represents a bool, it will be converted to `Decimal(1)` for True and `Decimal(0)` for False. If the string represents an int, it will be converted to a Decimal also.</span>
-</span><span id="TypeParser-668"><a href="#TypeParser-668"><span class="linenos">668</span></a>
-</span><span id="TypeParser-669"><a href="#TypeParser-669"><span class="linenos">669</span></a><span class="sd">			Behaves analogously to `parse_float()`, except that that returns a non-exact float instead.</span>
-</span><span id="TypeParser-670"><a href="#TypeParser-670"><span class="linenos">670</span></a>
-</span><span id="TypeParser-671"><a href="#TypeParser-671"><span class="linenos">671</span></a><span class="sd">			Parameters</span>
-</span><span id="TypeParser-672"><a href="#TypeParser-672"><span class="linenos">672</span></a><span class="sd">			----------</span>
-</span><span id="TypeParser-673"><a href="#TypeParser-673"><span class="linenos">673</span></a><span class="sd">			`value`</span>
-</span><span id="TypeParser-674"><a href="#TypeParser-674"><span class="linenos">674</span></a><span class="sd">			: string to be parsed</span>
-</span><span id="TypeParser-675"><a href="#TypeParser-675"><span class="linenos">675</span></a>
-</span><span id="TypeParser-676"><a href="#TypeParser-676"><span class="linenos">676</span></a><span class="sd">			`allow_scientific`</span>
-</span><span id="TypeParser-677"><a href="#TypeParser-677"><span class="linenos">677</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form &lt;code&gt;&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;&lt;/code&gt; will be interpreted as the expression &lt;code&gt;&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)&lt;/code&gt;, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note that &lt;var&gt;X&lt;/var&gt; must be an integer, but can be negative.</span>
-</span><span id="TypeParser-678"><a href="#TypeParser-678"><span class="linenos">678</span></a>
-</span><span id="TypeParser-679"><a href="#TypeParser-679"><span class="linenos">679</span></a><span class="sd">			`allow_inf`</span>
-</span><span id="TypeParser-680"><a href="#TypeParser-680"><span class="linenos">680</span></a><span class="sd">			: whether to accept positive and negative infinity values. If True, strings that match the values in `self.inf_values` (empty by default) are interpreted as infinity, or as negative infinity if prepended by a negative sign. The case sensitivity of this matching depends on `self.float_case_sensitive`, which is False by default.</span>
-</span><span id="TypeParser-681"><a href="#TypeParser-681"><span class="linenos">681</span></a>
-</span><span id="TypeParser-682"><a href="#TypeParser-682"><span class="linenos">682</span></a><span class="sd">			`allow_nan`</span>
-</span><span id="TypeParser-683"><a href="#TypeParser-683"><span class="linenos">683</span></a><span class="sd">			: whether to accept NaN (not a number) representations. If True, strings that match the values in `self.nan_values` (empty by default) are interpeted as NaN. The case sensitivity of this matching depends on `self.float_case_sensitive`, which is False by default.</span>
-</span><span id="TypeParser-684"><a href="#TypeParser-684"><span class="linenos">684</span></a>
-</span><span id="TypeParser-685"><a href="#TypeParser-685"><span class="linenos">685</span></a><span class="sd">			Returns</span>
-</span><span id="TypeParser-686"><a href="#TypeParser-686"><span class="linenos">686</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser-687"><a href="#TypeParser-687"><span class="linenos">687</span></a><span class="sd">			parsed Decimal value</span>
-</span><span id="TypeParser-688"><a href="#TypeParser-688"><span class="linenos">688</span></a>
-</span><span id="TypeParser-689"><a href="#TypeParser-689"><span class="linenos">689</span></a><span class="sd">			Raises</span>
-</span><span id="TypeParser-690"><a href="#TypeParser-690"><span class="linenos">690</span></a><span class="sd">			------</span>
-</span><span id="TypeParser-691"><a href="#TypeParser-691"><span class="linenos">691</span></a><span class="sd">			`ValueError` if `value` cannot be parsed</span>
-</span><span id="TypeParser-692"><a href="#TypeParser-692"><span class="linenos">692</span></a>
-</span><span id="TypeParser-693"><a href="#TypeParser-693"><span class="linenos">693</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser-694"><a href="#TypeParser-694"><span class="linenos">694</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser-695"><a href="#TypeParser-695"><span class="linenos">695</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser-696"><a href="#TypeParser-696"><span class="linenos">696</span></a><span class="sd">			parser = TypeParser(inf_values=[&quot;inf&quot;], nan_values=[&quot;nan&quot;])</span>
-</span><span id="TypeParser-697"><a href="#TypeParser-697"><span class="linenos">697</span></a><span class="sd">			parser.parse_decimal(&quot;1.&quot;)       # Decimal(1)</span>
-</span><span id="TypeParser-698"><a href="#TypeParser-698"><span class="linenos">698</span></a><span class="sd">			parser.parse_decimal(&quot;1.23e2&quot;)   # Decimal(123)</span>
-</span><span id="TypeParser-699"><a href="#TypeParser-699"><span class="linenos">699</span></a><span class="sd">			parser.parse_decimal(&quot;1.23e-2&quot;)  # Decimal(123) / Decimal(10000)</span>
-</span><span id="TypeParser-700"><a href="#TypeParser-700"><span class="linenos">700</span></a><span class="sd">			parser.parse_decimal(&quot;inf&quot;)      # Decimal(math.inf)</span>
-</span><span id="TypeParser-701"><a href="#TypeParser-701"><span class="linenos">701</span></a><span class="sd">			```</span>
-</span><span id="TypeParser-702"><a href="#TypeParser-702"><span class="linenos">702</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser-703"><a href="#TypeParser-703"><span class="linenos">703</span></a>		<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_parse_floatlike</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">Decimal</span><span class="p">,</span> <span class="n">Decimal</span><span class="p">(</span><span class="n">math</span><span class="o">.</span><span class="n">inf</span><span class="p">),</span> <span class="n">Decimal</span><span class="p">(</span><span class="n">math</span><span class="o">.</span><span class="n">nan</span><span class="p">),</span>
-</span><span id="TypeParser-704"><a href="#TypeParser-704"><span class="linenos">704</span></a>			<span class="n">allow_scientific</span><span class="o">=</span><span class="n">allow_scientific</span><span class="p">,</span>
-</span><span id="TypeParser-705"><a href="#TypeParser-705"><span class="linenos">705</span></a>			<span class="n">allow_inf</span><span class="o">=</span><span class="n">allow_inf</span><span class="p">,</span>
-</span><span id="TypeParser-706"><a href="#TypeParser-706"><span class="linenos">706</span></a>			<span class="n">allow_nan</span><span class="o">=</span><span class="n">allow_nan</span><span class="p">,</span>
-</span><span id="TypeParser-707"><a href="#TypeParser-707"><span class="linenos">707</span></a>		<span class="p">)</span>
-</span><span id="TypeParser-708"><a href="#TypeParser-708"><span class="linenos">708</span></a>
-</span><span id="TypeParser-709"><a href="#TypeParser-709"><span class="linenos">709</span></a>
-</span><span id="TypeParser-710"><a href="#TypeParser-710"><span class="linenos">710</span></a>	<span class="k">def</span> <span class="nf">infer</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">AnyValueType</span><span class="p">:</span>
-</span><span id="TypeParser-711"><a href="#TypeParser-711"><span class="linenos">711</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser-712"><a href="#TypeParser-712"><span class="linenos">712</span></a><span class="sd">			Infer the underlying type of a string</span>
-</span><span id="TypeParser-713"><a href="#TypeParser-713"><span class="linenos">713</span></a>
-</span><span id="TypeParser-714"><a href="#TypeParser-714"><span class="linenos">714</span></a><span class="sd">			Also check for inline lists if `self.list_delimiter` is not None.</span>
-</span><span id="TypeParser-715"><a href="#TypeParser-715"><span class="linenos">715</span></a>
-</span><span id="TypeParser-716"><a href="#TypeParser-716"><span class="linenos">716</span></a><span class="sd">			Parameters</span>
-</span><span id="TypeParser-717"><a href="#TypeParser-717"><span class="linenos">717</span></a><span class="sd">			----------</span>
-</span><span id="TypeParser-718"><a href="#TypeParser-718"><span class="linenos">718</span></a><span class="sd">			`value`</span>
-</span><span id="TypeParser-719"><a href="#TypeParser-719"><span class="linenos">719</span></a><span class="sd">			: the string for which the type should be inferred</span>
-</span><span id="TypeParser-720"><a href="#TypeParser-720"><span class="linenos">720</span></a>
-</span><span id="TypeParser-721"><a href="#TypeParser-721"><span class="linenos">721</span></a><span class="sd">			Returns</span>
-</span><span id="TypeParser-722"><a href="#TypeParser-722"><span class="linenos">722</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser-723"><a href="#TypeParser-723"><span class="linenos">723</span></a><span class="sd">			inferred type</span>
-</span><span id="TypeParser-724"><a href="#TypeParser-724"><span class="linenos">724</span></a>
-</span><span id="TypeParser-725"><a href="#TypeParser-725"><span class="linenos">725</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser-726"><a href="#TypeParser-726"><span class="linenos">726</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser-727"><a href="#TypeParser-727"><span class="linenos">727</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser-728"><a href="#TypeParser-728"><span class="linenos">728</span></a><span class="sd">			parser = TypeParser()</span>
-</span><span id="TypeParser-729"><a href="#TypeParser-729"><span class="linenos">729</span></a><span class="sd">			parser.infer(&quot;true&quot;)  # bool</span>
-</span><span id="TypeParser-730"><a href="#TypeParser-730"><span class="linenos">730</span></a><span class="sd">			parser.infer(&quot;2.0&quot;)   # float</span>
-</span><span id="TypeParser-731"><a href="#TypeParser-731"><span class="linenos">731</span></a><span class="sd">			parser.infer(&quot;abc&quot;)   # str</span>
-</span><span id="TypeParser-732"><a href="#TypeParser-732"><span class="linenos">732</span></a><span class="sd">			```</span>
-</span><span id="TypeParser-733"><a href="#TypeParser-733"><span class="linenos">733</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser-734"><a href="#TypeParser-734"><span class="linenos">734</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_none</span><span class="p">(</span><span class="n">value</span><span class="p">):</span>
-</span><span id="TypeParser-735"><a href="#TypeParser-735"><span class="linenos">735</span></a>			<span class="k">return</span> <span class="n">NoneType</span>
-</span><span id="TypeParser-736"><a href="#TypeParser-736"><span class="linenos">736</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_bool</span><span class="p">(</span><span class="n">value</span><span class="p">):</span>
-</span><span id="TypeParser-737"><a href="#TypeParser-737"><span class="linenos">737</span></a>			<span class="k">return</span> <span class="nb">bool</span>
-</span><span id="TypeParser-738"><a href="#TypeParser-738"><span class="linenos">738</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_int</span><span class="p">(</span><span class="n">value</span><span class="p">):</span>
-</span><span id="TypeParser-739"><a href="#TypeParser-739"><span class="linenos">739</span></a>			<span class="k">return</span> <span class="nb">int</span>
-</span><span id="TypeParser-740"><a href="#TypeParser-740"><span class="linenos">740</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_float</span><span class="p">(</span><span class="n">value</span><span class="p">):</span>
-</span><span id="TypeParser-741"><a href="#TypeParser-741"><span class="linenos">741</span></a>			<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">use_decimal</span><span class="p">:</span>
-</span><span id="TypeParser-742"><a href="#TypeParser-742"><span class="linenos">742</span></a>				<span class="k">return</span> <span class="n">Decimal</span>
-</span><span id="TypeParser-743"><a href="#TypeParser-743"><span class="linenos">743</span></a>			<span class="k">else</span><span class="p">:</span>
-</span><span id="TypeParser-744"><a href="#TypeParser-744"><span class="linenos">744</span></a>				<span class="k">return</span> <span class="nb">float</span>
-</span><span id="TypeParser-745"><a href="#TypeParser-745"><span class="linenos">745</span></a>
-</span><span id="TypeParser-746"><a href="#TypeParser-746"><span class="linenos">746</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">trim</span><span class="p">:</span>
-</span><span id="TypeParser-747"><a href="#TypeParser-747"><span class="linenos">747</span></a>			<span class="n">value</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
-</span><span id="TypeParser-748"><a href="#TypeParser-748"><span class="linenos">748</span></a>
-</span><span id="TypeParser-749"><a href="#TypeParser-749"><span class="linenos">749</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">list_delimiter</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">list_delimiter</span> <span class="ow">in</span> <span class="n">value</span><span class="p">:</span>
-</span><span id="TypeParser-750"><a href="#TypeParser-750"><span class="linenos">750</span></a>			<span class="n">subvalues</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">list_delimiter</span><span class="p">)</span>
-</span><span id="TypeParser-751"><a href="#TypeParser-751"><span class="linenos">751</span></a>			<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">trim</span><span class="p">:</span>
-</span><span id="TypeParser-752"><a href="#TypeParser-752"><span class="linenos">752</span></a>				<span class="n">subvalues</span> <span class="o">=</span> <span class="p">[</span><span class="n">subvalue</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="k">for</span> <span class="n">subvalue</span> <span class="ow">in</span> <span class="n">subvalues</span><span class="p">]</span>
-</span><span id="TypeParser-753"><a href="#TypeParser-753"><span class="linenos">753</span></a>			<span class="n">reduced_type</span> <span class="o">=</span> <span class="n">reduce_types</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">subvalue</span><span class="p">)</span> <span class="k">for</span> <span class="n">subvalue</span> <span class="ow">in</span> <span class="n">subvalues</span><span class="p">)</span>
-</span><span id="TypeParser-754"><a href="#TypeParser-754"><span class="linenos">754</span></a>			<span class="n">r</span> <span class="o">=</span> <span class="nb">list</span><span class="p">[</span><span class="n">reduced_type</span><span class="p">]</span>
-</span><span id="TypeParser-755"><a href="#TypeParser-755"><span class="linenos">755</span></a>			<span class="k">return</span> <span class="n">r</span>
-</span><span id="TypeParser-756"><a href="#TypeParser-756"><span class="linenos">756</span></a>
-</span><span id="TypeParser-757"><a href="#TypeParser-757"><span class="linenos">757</span></a>		<span class="k">return</span> <span class="n">GenericValue</span>
-</span><span id="TypeParser-758"><a href="#TypeParser-758"><span class="linenos">758</span></a>
-</span><span id="TypeParser-759"><a href="#TypeParser-759"><span class="linenos">759</span></a>
-</span><span id="TypeParser-760"><a href="#TypeParser-760"><span class="linenos">760</span></a>	<span class="k">def</span> <span class="nf">infer_series</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="n">AnyValueType</span><span class="p">:</span>
-</span><span id="TypeParser-761"><a href="#TypeParser-761"><span class="linenos">761</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser-762"><a href="#TypeParser-762"><span class="linenos">762</span></a><span class="sd">			Infer the underlying common type of a series of strings</span>
-</span><span id="TypeParser-763"><a href="#TypeParser-763"><span class="linenos">763</span></a>
-</span><span id="TypeParser-764"><a href="#TypeParser-764"><span class="linenos">764</span></a><span class="sd">			If the values in the series do not have the same apparent type, the resulting type will be narrowest possible type that will encompass all values in the series. See `parsetypes.reduce_types()` for more information.</span>
-</span><span id="TypeParser-765"><a href="#TypeParser-765"><span class="linenos">765</span></a>
-</span><span id="TypeParser-766"><a href="#TypeParser-766"><span class="linenos">766</span></a><span class="sd">			Parameters</span>
-</span><span id="TypeParser-767"><a href="#TypeParser-767"><span class="linenos">767</span></a><span class="sd">			----------</span>
-</span><span id="TypeParser-768"><a href="#TypeParser-768"><span class="linenos">768</span></a><span class="sd">			`values`</span>
-</span><span id="TypeParser-769"><a href="#TypeParser-769"><span class="linenos">769</span></a><span class="sd">			: series of strings for which the type should be inferred</span>
-</span><span id="TypeParser-770"><a href="#TypeParser-770"><span class="linenos">770</span></a>
-</span><span id="TypeParser-771"><a href="#TypeParser-771"><span class="linenos">771</span></a><span class="sd">			Returns</span>
-</span><span id="TypeParser-772"><a href="#TypeParser-772"><span class="linenos">772</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser-773"><a href="#TypeParser-773"><span class="linenos">773</span></a><span class="sd">			inferred type</span>
-</span><span id="TypeParser-774"><a href="#TypeParser-774"><span class="linenos">774</span></a>
-</span><span id="TypeParser-775"><a href="#TypeParser-775"><span class="linenos">775</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser-776"><a href="#TypeParser-776"><span class="linenos">776</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser-777"><a href="#TypeParser-777"><span class="linenos">777</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser-778"><a href="#TypeParser-778"><span class="linenos">778</span></a><span class="sd">			parser = TypeParser()</span>
-</span><span id="TypeParser-779"><a href="#TypeParser-779"><span class="linenos">779</span></a><span class="sd">			parser.infer_series([&quot;1&quot;, &quot;2&quot;, &quot;3.4&quot;])       # float</span>
-</span><span id="TypeParser-780"><a href="#TypeParser-780"><span class="linenos">780</span></a><span class="sd">			parser.infer_series([&quot;true&quot;, &quot;false&quot;, &quot;2&quot;])  # int</span>
-</span><span id="TypeParser-781"><a href="#TypeParser-781"><span class="linenos">781</span></a><span class="sd">			parser.infer_series([&quot;1&quot;, &quot;2.3&quot;, &quot;abc&quot;])     # str</span>
-</span><span id="TypeParser-782"><a href="#TypeParser-782"><span class="linenos">782</span></a><span class="sd">			```</span>
-</span><span id="TypeParser-783"><a href="#TypeParser-783"><span class="linenos">783</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser-784"><a href="#TypeParser-784"><span class="linenos">784</span></a>		<span class="k">return</span> <span class="n">reduce_types</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
-</span><span id="TypeParser-785"><a href="#TypeParser-785"><span class="linenos">785</span></a>
-</span><span id="TypeParser-786"><a href="#TypeParser-786"><span class="linenos">786</span></a>
-</span><span id="TypeParser-787"><a href="#TypeParser-787"><span class="linenos">787</span></a>	<span class="k">def</span> <span class="nf">infer_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">rows</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">AnyValueType</span><span class="p">]:</span>
-</span><span id="TypeParser-788"><a href="#TypeParser-788"><span class="linenos">788</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser-789"><a href="#TypeParser-789"><span class="linenos">789</span></a><span class="sd">			Infer the underlying common type for each column of a table of strings</span>
-</span><span id="TypeParser-790"><a href="#TypeParser-790"><span class="linenos">790</span></a>
-</span><span id="TypeParser-791"><a href="#TypeParser-791"><span class="linenos">791</span></a><span class="sd">			For each column, if the values do not have the same apparent type, the resulting type will be narrowest possible type that will encompass all values in the column. See `parsetypes.reduce_types()` for more information.</span>
-</span><span id="TypeParser-792"><a href="#TypeParser-792"><span class="linenos">792</span></a>
-</span><span id="TypeParser-793"><a href="#TypeParser-793"><span class="linenos">793</span></a><span class="sd">			Note that the individual inferred types of every value in the table must be able to fit into memory.</span>
-</span><span id="TypeParser-794"><a href="#TypeParser-794"><span class="linenos">794</span></a>
-</span><span id="TypeParser-795"><a href="#TypeParser-795"><span class="linenos">795</span></a><span class="sd">			Parameters</span>
-</span><span id="TypeParser-796"><a href="#TypeParser-796"><span class="linenos">796</span></a><span class="sd">			----------</span>
-</span><span id="TypeParser-797"><a href="#TypeParser-797"><span class="linenos">797</span></a><span class="sd">			`rows`</span>
-</span><span id="TypeParser-798"><a href="#TypeParser-798"><span class="linenos">798</span></a><span class="sd">			: table of strings for which the types should be inferred, in row-major order</span>
-</span><span id="TypeParser-799"><a href="#TypeParser-799"><span class="linenos">799</span></a>
-</span><span id="TypeParser-800"><a href="#TypeParser-800"><span class="linenos">800</span></a><span class="sd">			Returns</span>
-</span><span id="TypeParser-801"><a href="#TypeParser-801"><span class="linenos">801</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser-802"><a href="#TypeParser-802"><span class="linenos">802</span></a><span class="sd">			inferred types</span>
-</span><span id="TypeParser-803"><a href="#TypeParser-803"><span class="linenos">803</span></a>
-</span><span id="TypeParser-804"><a href="#TypeParser-804"><span class="linenos">804</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser-805"><a href="#TypeParser-805"><span class="linenos">805</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser-806"><a href="#TypeParser-806"><span class="linenos">806</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser-807"><a href="#TypeParser-807"><span class="linenos">807</span></a><span class="sd">			parser = TypeParser()</span>
-</span><span id="TypeParser-808"><a href="#TypeParser-808"><span class="linenos">808</span></a><span class="sd">			parser.infer_table([</span>
-</span><span id="TypeParser-809"><a href="#TypeParser-809"><span class="linenos">809</span></a><span class="sd">				[&quot;1&quot;,   &quot;true&quot;,  &quot;1&quot;],</span>
-</span><span id="TypeParser-810"><a href="#TypeParser-810"><span class="linenos">810</span></a><span class="sd">				[&quot;2&quot;,   &quot;false&quot;, &quot;2.3&quot;],</span>
-</span><span id="TypeParser-811"><a href="#TypeParser-811"><span class="linenos">811</span></a><span class="sd">				[&quot;3.4&quot;, &quot;2&quot;,     &quot;abc&quot;],</span>
-</span><span id="TypeParser-812"><a href="#TypeParser-812"><span class="linenos">812</span></a><span class="sd">			])</span>
-</span><span id="TypeParser-813"><a href="#TypeParser-813"><span class="linenos">813</span></a><span class="sd">			# [float, int, str]</span>
-</span><span id="TypeParser-814"><a href="#TypeParser-814"><span class="linenos">814</span></a><span class="sd">			```</span>
-</span><span id="TypeParser-815"><a href="#TypeParser-815"><span class="linenos">815</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser-816"><a href="#TypeParser-816"><span class="linenos">816</span></a>		<span class="n">rows_iter</span> <span class="o">=</span> <span class="nb">iter</span><span class="p">(</span><span class="n">rows</span><span class="p">)</span>
-</span><span id="TypeParser-817"><a href="#TypeParser-817"><span class="linenos">817</span></a>		<span class="n">first_row</span> <span class="o">=</span> <span class="nb">next</span><span class="p">(</span><span class="n">rows_iter</span><span class="p">,</span> <span class="kc">None</span><span class="p">)</span>
-</span><span id="TypeParser-818"><a href="#TypeParser-818"><span class="linenos">818</span></a>		<span class="k">if</span> <span class="n">first_row</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="TypeParser-819"><a href="#TypeParser-819"><span class="linenos">819</span></a>			<span class="k">return</span> <span class="p">[]</span>
-</span><span id="TypeParser-820"><a href="#TypeParser-820"><span class="linenos">820</span></a>
-</span><span id="TypeParser-821"><a href="#TypeParser-821"><span class="linenos">821</span></a>		<span class="n">num_cols</span> <span class="o">=</span> <span class="nb">len</span><span class="p">(</span><span class="n">first_row</span><span class="p">)</span>
-</span><span id="TypeParser-822"><a href="#TypeParser-822"><span class="linenos">822</span></a>		<span class="k">if</span> <span class="n">num_cols</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="TypeParser-823"><a href="#TypeParser-823"><span class="linenos">823</span></a>			<span class="k">return</span> <span class="p">[]</span>
-</span><span id="TypeParser-824"><a href="#TypeParser-824"><span class="linenos">824</span></a>
-</span><span id="TypeParser-825"><a href="#TypeParser-825"><span class="linenos">825</span></a>		<span class="n">table</span> <span class="o">=</span> <span class="n">_TypeTable</span><span class="p">([[</span><span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">value</span><span class="p">)]</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">first_row</span><span class="p">])</span>
-</span><span id="TypeParser-826"><a href="#TypeParser-826"><span class="linenos">826</span></a>		<span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">rows_iter</span><span class="p">:</span>
-</span><span id="TypeParser-827"><a href="#TypeParser-827"><span class="linenos">827</span></a>			<span class="n">table</span><span class="o">.</span><span class="n">add_row</span><span class="p">([</span><span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">row</span><span class="p">])</span>
-</span><span id="TypeParser-828"><a href="#TypeParser-828"><span class="linenos">828</span></a>
-</span><span id="TypeParser-829"><a href="#TypeParser-829"><span class="linenos">829</span></a>		<span class="k">return</span> <span class="p">[</span><span class="n">reduce_types</span><span class="p">(</span><span class="n">col</span><span class="p">)</span> <span class="k">for</span> <span class="n">col</span> <span class="ow">in</span> <span class="n">table</span><span class="o">.</span><span class="n">cols</span><span class="p">]</span>
-</span><span id="TypeParser-830"><a href="#TypeParser-830"><span class="linenos">830</span></a>
-</span><span id="TypeParser-831"><a href="#TypeParser-831"><span class="linenos">831</span></a>
-</span><span id="TypeParser-832"><a href="#TypeParser-832"><span class="linenos">832</span></a>	<span class="k">def</span> <span class="nf">_convert</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">t</span><span class="p">:</span> <span class="n">AnyValueType</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">AnyValue</span><span class="p">:</span>
-</span><span id="TypeParser-833"><a href="#TypeParser-833"><span class="linenos">833</span></a>		<span class="n">base</span><span class="p">,</span> <span class="n">type_args</span> <span class="o">=</span> <span class="n">_decompose_type</span><span class="p">(</span><span class="n">t</span><span class="p">)</span>
-</span><span id="TypeParser-834"><a href="#TypeParser-834"><span class="linenos">834</span></a>		<span class="k">if</span> <span class="n">base</span> <span class="o">==</span> <span class="n">NoneType</span><span class="p">:</span>
-</span><span id="TypeParser-835"><a href="#TypeParser-835"><span class="linenos">835</span></a>			<span class="k">return</span> <span class="kc">None</span>
-</span><span id="TypeParser-836"><a href="#TypeParser-836"><span class="linenos">836</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="TypeParser-837"><a href="#TypeParser-837"><span class="linenos">837</span></a>			<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_bool</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
-</span><span id="TypeParser-838"><a href="#TypeParser-838"><span class="linenos">838</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="TypeParser-839"><a href="#TypeParser-839"><span class="linenos">839</span></a>			<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_int</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
-</span><span id="TypeParser-840"><a href="#TypeParser-840"><span class="linenos">840</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="n">Decimal</span><span class="p">:</span>
-</span><span id="TypeParser-841"><a href="#TypeParser-841"><span class="linenos">841</span></a>			<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_decimal</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
-</span><span id="TypeParser-842"><a href="#TypeParser-842"><span class="linenos">842</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">float</span><span class="p">:</span>
-</span><span id="TypeParser-843"><a href="#TypeParser-843"><span class="linenos">843</span></a>			<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_float</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
-</span><span id="TypeParser-844"><a href="#TypeParser-844"><span class="linenos">844</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="TypeParser-845"><a href="#TypeParser-845"><span class="linenos">845</span></a>			<span class="k">return</span> <span class="n">value</span>
-</span><span id="TypeParser-846"><a href="#TypeParser-846"><span class="linenos">846</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="n">Nullable</span><span class="p">:</span>
-</span><span id="TypeParser-847"><a href="#TypeParser-847"><span class="linenos">847</span></a>			<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_none</span><span class="p">(</span><span class="n">value</span><span class="p">):</span>
-</span><span id="TypeParser-848"><a href="#TypeParser-848"><span class="linenos">848</span></a>				<span class="k">return</span> <span class="kc">None</span>
-</span><span id="TypeParser-849"><a href="#TypeParser-849"><span class="linenos">849</span></a>			<span class="k">else</span><span class="p">:</span>
-</span><span id="TypeParser-850"><a href="#TypeParser-850"><span class="linenos">850</span></a>				<span class="k">if</span> <span class="n">type_args</span> <span class="ow">is</span> <span class="ow">not</span>  <span class="kc">None</span> <span class="ow">and</span> <span class="nb">len</span><span class="p">(</span><span class="n">type_args</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span> <span class="ow">and</span> <span class="n">type_args</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">!=</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="TypeParser-851"><a href="#TypeParser-851"><span class="linenos">851</span></a>					<span class="n">inner_type</span> <span class="o">=</span> <span class="n">type_args</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="TypeParser-852"><a href="#TypeParser-852"><span class="linenos">852</span></a>					<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_convert</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">inner_type</span><span class="p">)</span>
-</span><span id="TypeParser-853"><a href="#TypeParser-853"><span class="linenos">853</span></a>				<span class="k">else</span><span class="p">:</span>
-</span><span id="TypeParser-854"><a href="#TypeParser-854"><span class="linenos">854</span></a>					<span class="k">return</span> <span class="n">value</span>
-</span><span id="TypeParser-855"><a href="#TypeParser-855"><span class="linenos">855</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">list</span><span class="p">:</span>
-</span><span id="TypeParser-856"><a href="#TypeParser-856"><span class="linenos">856</span></a>			<span class="n">subvalues</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">list_delimiter</span><span class="p">)</span>
-</span><span id="TypeParser-857"><a href="#TypeParser-857"><span class="linenos">857</span></a>			<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">trim</span><span class="p">:</span>
-</span><span id="TypeParser-858"><a href="#TypeParser-858"><span class="linenos">858</span></a>				<span class="n">subvalues</span> <span class="o">=</span> <span class="p">[</span><span class="n">subvalue</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="k">for</span> <span class="n">subvalue</span> <span class="ow">in</span> <span class="n">subvalues</span><span class="p">]</span>
-</span><span id="TypeParser-859"><a href="#TypeParser-859"><span class="linenos">859</span></a>			<span class="k">if</span> <span class="n">type_args</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span> <span class="ow">and</span> <span class="nb">len</span><span class="p">(</span><span class="n">type_args</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span> <span class="ow">and</span> <span class="n">type_args</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">!=</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="TypeParser-860"><a href="#TypeParser-860"><span class="linenos">860</span></a>				<span class="n">subtype</span> <span class="o">=</span> <span class="n">type_args</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="TypeParser-861"><a href="#TypeParser-861"><span class="linenos">861</span></a>				<span class="k">return</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">_convert</span><span class="p">(</span><span class="n">subvalue</span><span class="p">,</span> <span class="n">subtype</span><span class="p">)</span> <span class="k">for</span> <span class="n">subvalue</span> <span class="ow">in</span> <span class="n">subvalues</span><span class="p">]</span>
-</span><span id="TypeParser-862"><a href="#TypeParser-862"><span class="linenos">862</span></a>			<span class="k">else</span><span class="p">:</span>
-</span><span id="TypeParser-863"><a href="#TypeParser-863"><span class="linenos">863</span></a>				<span class="k">return</span> <span class="n">subvalues</span>
-</span><span id="TypeParser-864"><a href="#TypeParser-864"><span class="linenos">864</span></a>		<span class="k">else</span><span class="p">:</span>
-</span><span id="TypeParser-865"><a href="#TypeParser-865"><span class="linenos">865</span></a>			<span class="k">return</span> <span class="n">value</span>
-</span><span id="TypeParser-866"><a href="#TypeParser-866"><span class="linenos">866</span></a>
-</span><span id="TypeParser-867"><a href="#TypeParser-867"><span class="linenos">867</span></a>
-</span><span id="TypeParser-868"><a href="#TypeParser-868"><span class="linenos">868</span></a>	<span class="k">def</span> <span class="nf">parse</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">AnyValue</span><span class="p">:</span>
-</span><span id="TypeParser-869"><a href="#TypeParser-869"><span class="linenos">869</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser-870"><a href="#TypeParser-870"><span class="linenos">870</span></a><span class="sd">			Parse a string and convert it to its underlying type</span>
-</span><span id="TypeParser-871"><a href="#TypeParser-871"><span class="linenos">871</span></a>
-</span><span id="TypeParser-872"><a href="#TypeParser-872"><span class="linenos">872</span></a><span class="sd">			Parameters</span>
-</span><span id="TypeParser-873"><a href="#TypeParser-873"><span class="linenos">873</span></a><span class="sd">			----------</span>
-</span><span id="TypeParser-874"><a href="#TypeParser-874"><span class="linenos">874</span></a><span class="sd">			`value`</span>
-</span><span id="TypeParser-875"><a href="#TypeParser-875"><span class="linenos">875</span></a><span class="sd">			: the string to be parsed</span>
-</span><span id="TypeParser-876"><a href="#TypeParser-876"><span class="linenos">876</span></a>
-</span><span id="TypeParser-877"><a href="#TypeParser-877"><span class="linenos">877</span></a><span class="sd">			Returns</span>
-</span><span id="TypeParser-878"><a href="#TypeParser-878"><span class="linenos">878</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser-879"><a href="#TypeParser-879"><span class="linenos">879</span></a><span class="sd">			converted value</span>
-</span><span id="TypeParser-880"><a href="#TypeParser-880"><span class="linenos">880</span></a>
-</span><span id="TypeParser-881"><a href="#TypeParser-881"><span class="linenos">881</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser-882"><a href="#TypeParser-882"><span class="linenos">882</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser-883"><a href="#TypeParser-883"><span class="linenos">883</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser-884"><a href="#TypeParser-884"><span class="linenos">884</span></a><span class="sd">			parser = TypeParser()</span>
-</span><span id="TypeParser-885"><a href="#TypeParser-885"><span class="linenos">885</span></a><span class="sd">			parser.parse(&quot;true&quot;)  # True</span>
-</span><span id="TypeParser-886"><a href="#TypeParser-886"><span class="linenos">886</span></a><span class="sd">			parser.parse(&quot;2.0&quot;)   # 2.</span>
-</span><span id="TypeParser-887"><a href="#TypeParser-887"><span class="linenos">887</span></a><span class="sd">			parser.parse(&quot;abc&quot;)   # &quot;abc&quot;</span>
-</span><span id="TypeParser-888"><a href="#TypeParser-888"><span class="linenos">888</span></a><span class="sd">			```</span>
-</span><span id="TypeParser-889"><a href="#TypeParser-889"><span class="linenos">889</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser-890"><a href="#TypeParser-890"><span class="linenos">890</span></a>		<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_convert</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">value</span><span class="p">))</span>
-</span><span id="TypeParser-891"><a href="#TypeParser-891"><span class="linenos">891</span></a>
-</span><span id="TypeParser-892"><a href="#TypeParser-892"><span class="linenos">892</span></a>
-</span><span id="TypeParser-893"><a href="#TypeParser-893"><span class="linenos">893</span></a>	<span class="k">def</span> <span class="nf">parse_series</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">AnyValue</span><span class="p">]:</span>
-</span><span id="TypeParser-894"><a href="#TypeParser-894"><span class="linenos">894</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser-895"><a href="#TypeParser-895"><span class="linenos">895</span></a><span class="sd">			Parse a series of strings and convert them to their underlying common type</span>
-</span><span id="TypeParser-896"><a href="#TypeParser-896"><span class="linenos">896</span></a>
-</span><span id="TypeParser-897"><a href="#TypeParser-897"><span class="linenos">897</span></a><span class="sd">			If the values in the series do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the series. See `parsetypes.reduce_types()` for more information.</span>
-</span><span id="TypeParser-898"><a href="#TypeParser-898"><span class="linenos">898</span></a>
-</span><span id="TypeParser-899"><a href="#TypeParser-899"><span class="linenos">899</span></a><span class="sd">			Parameters</span>
-</span><span id="TypeParser-900"><a href="#TypeParser-900"><span class="linenos">900</span></a><span class="sd">			----------</span>
-</span><span id="TypeParser-901"><a href="#TypeParser-901"><span class="linenos">901</span></a><span class="sd">			`values`</span>
-</span><span id="TypeParser-902"><a href="#TypeParser-902"><span class="linenos">902</span></a><span class="sd">			: series of strings to be parsed</span>
-</span><span id="TypeParser-903"><a href="#TypeParser-903"><span class="linenos">903</span></a>
-</span><span id="TypeParser-904"><a href="#TypeParser-904"><span class="linenos">904</span></a><span class="sd">			Returns</span>
-</span><span id="TypeParser-905"><a href="#TypeParser-905"><span class="linenos">905</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser-906"><a href="#TypeParser-906"><span class="linenos">906</span></a><span class="sd">			converted values</span>
-</span><span id="TypeParser-907"><a href="#TypeParser-907"><span class="linenos">907</span></a>
-</span><span id="TypeParser-908"><a href="#TypeParser-908"><span class="linenos">908</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser-909"><a href="#TypeParser-909"><span class="linenos">909</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser-910"><a href="#TypeParser-910"><span class="linenos">910</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser-911"><a href="#TypeParser-911"><span class="linenos">911</span></a><span class="sd">			parser = TypeParser()</span>
-</span><span id="TypeParser-912"><a href="#TypeParser-912"><span class="linenos">912</span></a><span class="sd">			parser.parse_series([&quot;1&quot;, &quot;2&quot;, &quot;3&quot;])        # [1, 2, 3]</span>
-</span><span id="TypeParser-913"><a href="#TypeParser-913"><span class="linenos">913</span></a><span class="sd">			parser.parse_series([&quot;5&quot;, &quot;6.7&quot;, &quot;8.&quot;])     # [5., 6.7, 8.]</span>
-</span><span id="TypeParser-914"><a href="#TypeParser-914"><span class="linenos">914</span></a><span class="sd">			parser.parse_series([&quot;true&quot;, &quot;false&quot;, &quot;&quot;])  # [True, False, None]</span>
-</span><span id="TypeParser-915"><a href="#TypeParser-915"><span class="linenos">915</span></a><span class="sd">			parser.parse_series([&quot;1&quot;, &quot;2.3&quot;, &quot;abc&quot;])    # [&quot;1&quot;, &quot;2.3&quot;, &quot;abc&quot;]</span>
-</span><span id="TypeParser-916"><a href="#TypeParser-916"><span class="linenos">916</span></a><span class="sd">			```</span>
-</span><span id="TypeParser-917"><a href="#TypeParser-917"><span class="linenos">917</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser-918"><a href="#TypeParser-918"><span class="linenos">918</span></a>		<span class="n">inferred</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">infer_series</span><span class="p">(</span><span class="n">values</span><span class="p">)</span>
-</span><span id="TypeParser-919"><a href="#TypeParser-919"><span class="linenos">919</span></a>		<span class="k">return</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">_convert</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">inferred</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">values</span><span class="p">]</span>
-</span><span id="TypeParser-920"><a href="#TypeParser-920"><span class="linenos">920</span></a>
-</span><span id="TypeParser-921"><a href="#TypeParser-921"><span class="linenos">921</span></a>
-</span><span id="TypeParser-922"><a href="#TypeParser-922"><span class="linenos">922</span></a>	<span class="k">def</span> <span class="nf">parse_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">rows</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">AnyValue</span><span class="p">]]:</span>
-</span><span id="TypeParser-923"><a href="#TypeParser-923"><span class="linenos">923</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser-924"><a href="#TypeParser-924"><span class="linenos">924</span></a><span class="sd">			Parse a table of strings and convert them to the underlying common type of each column</span>
-</span><span id="TypeParser-925"><a href="#TypeParser-925"><span class="linenos">925</span></a>
-</span><span id="TypeParser-926"><a href="#TypeParser-926"><span class="linenos">926</span></a><span class="sd">			For each column, if the values do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the column. See `parsetypes.reduce_types()` for more information.</span>
-</span><span id="TypeParser-927"><a href="#TypeParser-927"><span class="linenos">927</span></a>
-</span><span id="TypeParser-928"><a href="#TypeParser-928"><span class="linenos">928</span></a><span class="sd">			Note that the type to which the values should be converted is determined by `infer_table()`, and so the individual inferred types of every value in the table must be able to fit into memory.</span>
-</span><span id="TypeParser-929"><a href="#TypeParser-929"><span class="linenos">929</span></a>
-</span><span id="TypeParser-930"><a href="#TypeParser-930"><span class="linenos">930</span></a><span class="sd">			This is a function that computes the entire table and returns it all at once. The generator `iterate_table()` behaves analogously, except that it computes and yields each row one at a time.</span>
-</span><span id="TypeParser-931"><a href="#TypeParser-931"><span class="linenos">931</span></a>
-</span><span id="TypeParser-932"><a href="#TypeParser-932"><span class="linenos">932</span></a><span class="sd">			Parameters</span>
-</span><span id="TypeParser-933"><a href="#TypeParser-933"><span class="linenos">933</span></a><span class="sd">			----------</span>
-</span><span id="TypeParser-934"><a href="#TypeParser-934"><span class="linenos">934</span></a><span class="sd">			`rows`</span>
-</span><span id="TypeParser-935"><a href="#TypeParser-935"><span class="linenos">935</span></a><span class="sd">			: table of strings to be parsed, in row-major order</span>
-</span><span id="TypeParser-936"><a href="#TypeParser-936"><span class="linenos">936</span></a>
-</span><span id="TypeParser-937"><a href="#TypeParser-937"><span class="linenos">937</span></a><span class="sd">			`iterator`</span>
-</span><span id="TypeParser-938"><a href="#TypeParser-938"><span class="linenos">938</span></a><span class="sd">			: whether the parsed values should be yielded as an iterator. If False, which is the default, the entire table is computed and returned as a list of lists. If True, this function behaves as a generator, and the rows of the table are computed and yielded one at a time. However, note that even when set to True, the type inference requires that inferred type of each individual value must all be able to fit into memory at once.</span>
-</span><span id="TypeParser-939"><a href="#TypeParser-939"><span class="linenos">939</span></a>
-</span><span id="TypeParser-940"><a href="#TypeParser-940"><span class="linenos">940</span></a><span class="sd">			Returns</span>
-</span><span id="TypeParser-941"><a href="#TypeParser-941"><span class="linenos">941</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser-942"><a href="#TypeParser-942"><span class="linenos">942</span></a><span class="sd">			converted table of values, in row-major order</span>
-</span><span id="TypeParser-943"><a href="#TypeParser-943"><span class="linenos">943</span></a>
-</span><span id="TypeParser-944"><a href="#TypeParser-944"><span class="linenos">944</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser-945"><a href="#TypeParser-945"><span class="linenos">945</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser-946"><a href="#TypeParser-946"><span class="linenos">946</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser-947"><a href="#TypeParser-947"><span class="linenos">947</span></a><span class="sd">			parser = TypeParser()</span>
-</span><span id="TypeParser-948"><a href="#TypeParser-948"><span class="linenos">948</span></a><span class="sd">			table = parser.parse_table([</span>
-</span><span id="TypeParser-949"><a href="#TypeParser-949"><span class="linenos">949</span></a><span class="sd">				[&quot;1&quot;, &quot;5&quot;,   &quot;true&quot;,  &quot;1&quot;],</span>
-</span><span id="TypeParser-950"><a href="#TypeParser-950"><span class="linenos">950</span></a><span class="sd">				[&quot;2&quot;, &quot;6.7&quot;, &quot;false&quot;, &quot;2.3&quot;],</span>
-</span><span id="TypeParser-951"><a href="#TypeParser-951"><span class="linenos">951</span></a><span class="sd">				[&quot;3&quot;, &quot;8.0&quot;, &quot;&quot;,      &quot;abc&quot;],</span>
-</span><span id="TypeParser-952"><a href="#TypeParser-952"><span class="linenos">952</span></a><span class="sd">			]):</span>
-</span><span id="TypeParser-953"><a href="#TypeParser-953"><span class="linenos">953</span></a><span class="sd">			assert table == [</span>
-</span><span id="TypeParser-954"><a href="#TypeParser-954"><span class="linenos">954</span></a><span class="sd">				[1, 5.,  True,  &quot;1&quot;],</span>
-</span><span id="TypeParser-955"><a href="#TypeParser-955"><span class="linenos">955</span></a><span class="sd">				[2, 6.7, False, &quot;2.3&quot;],</span>
-</span><span id="TypeParser-956"><a href="#TypeParser-956"><span class="linenos">956</span></a><span class="sd">				[3, 8.,  None,  &quot;abc&quot;],</span>
-</span><span id="TypeParser-957"><a href="#TypeParser-957"><span class="linenos">957</span></a><span class="sd">			]</span>
-</span><span id="TypeParser-958"><a href="#TypeParser-958"><span class="linenos">958</span></a><span class="sd">			```</span>
-</span><span id="TypeParser-959"><a href="#TypeParser-959"><span class="linenos">959</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser-960"><a href="#TypeParser-960"><span class="linenos">960</span></a>		<span class="k">return</span> <span class="p">[</span><span class="n">converted_row</span> <span class="k">for</span> <span class="n">converted_row</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">iterate_table</span><span class="p">(</span><span class="n">rows</span><span class="p">)]</span>
-</span><span id="TypeParser-961"><a href="#TypeParser-961"><span class="linenos">961</span></a>
-</span><span id="TypeParser-962"><a href="#TypeParser-962"><span class="linenos">962</span></a>
-</span><span id="TypeParser-963"><a href="#TypeParser-963"><span class="linenos">963</span></a>	<span class="k">def</span> <span class="nf">iterate_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">rows</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]])</span> <span class="o">-&gt;</span> <span class="n">Iterator</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">AnyValue</span><span class="p">]]:</span>
-</span><span id="TypeParser-964"><a href="#TypeParser-964"><span class="linenos">964</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser-965"><a href="#TypeParser-965"><span class="linenos">965</span></a><span class="sd">			Parse a table of strings for the underlying common type of each column, then convert and yield each row</span>
-</span><span id="TypeParser-966"><a href="#TypeParser-966"><span class="linenos">966</span></a>
-</span><span id="TypeParser-967"><a href="#TypeParser-967"><span class="linenos">967</span></a><span class="sd">			For each column, if the values do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the column. See `parsetypes.reduce_types()` for more information.</span>
-</span><span id="TypeParser-968"><a href="#TypeParser-968"><span class="linenos">968</span></a>
-</span><span id="TypeParser-969"><a href="#TypeParser-969"><span class="linenos">969</span></a><span class="sd">			This is a generator that computes and yields each row one at a time. The function `parse_table()` behaves analogously, except that it computes the entire table and returns it as a list of lists. However, note that although this is a generator, the type to which the value sshould be converted is still determined by `infer_table()`, and so the individual inferred types of every value in the table must be able to fit into memory.</span>
-</span><span id="TypeParser-970"><a href="#TypeParser-970"><span class="linenos">970</span></a>
-</span><span id="TypeParser-971"><a href="#TypeParser-971"><span class="linenos">971</span></a><span class="sd">			Parameters</span>
-</span><span id="TypeParser-972"><a href="#TypeParser-972"><span class="linenos">972</span></a><span class="sd">			----------</span>
-</span><span id="TypeParser-973"><a href="#TypeParser-973"><span class="linenos">973</span></a><span class="sd">			`rows`</span>
-</span><span id="TypeParser-974"><a href="#TypeParser-974"><span class="linenos">974</span></a><span class="sd">			: table of strings to be parsed, in row-major order</span>
-</span><span id="TypeParser-975"><a href="#TypeParser-975"><span class="linenos">975</span></a>
-</span><span id="TypeParser-976"><a href="#TypeParser-976"><span class="linenos">976</span></a><span class="sd">			Yields</span>
-</span><span id="TypeParser-977"><a href="#TypeParser-977"><span class="linenos">977</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser-978"><a href="#TypeParser-978"><span class="linenos">978</span></a><span class="sd">			each row of converted table values</span>
-</span><span id="TypeParser-979"><a href="#TypeParser-979"><span class="linenos">979</span></a>
-</span><span id="TypeParser-980"><a href="#TypeParser-980"><span class="linenos">980</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser-981"><a href="#TypeParser-981"><span class="linenos">981</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser-982"><a href="#TypeParser-982"><span class="linenos">982</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser-983"><a href="#TypeParser-983"><span class="linenos">983</span></a><span class="sd">			parser = TypeParser()</span>
-</span><span id="TypeParser-984"><a href="#TypeParser-984"><span class="linenos">984</span></a><span class="sd">			table = parser.iterate_table([</span>
-</span><span id="TypeParser-985"><a href="#TypeParser-985"><span class="linenos">985</span></a><span class="sd">				[&quot;1&quot;,   &quot;true&quot;,  &quot;1&quot;],</span>
-</span><span id="TypeParser-986"><a href="#TypeParser-986"><span class="linenos">986</span></a><span class="sd">				[&quot;2&quot;,   &quot;false&quot;, &quot;2.3&quot;],</span>
-</span><span id="TypeParser-987"><a href="#TypeParser-987"><span class="linenos">987</span></a><span class="sd">				[&quot;3.4&quot;, &quot;2&quot;,     &quot;abc&quot;],</span>
-</span><span id="TypeParser-988"><a href="#TypeParser-988"><span class="linenos">988</span></a><span class="sd">			]):</span>
-</span><span id="TypeParser-989"><a href="#TypeParser-989"><span class="linenos">989</span></a><span class="sd">			assert next(table) == [1.,  1, &quot;1&quot;]</span>
-</span><span id="TypeParser-990"><a href="#TypeParser-990"><span class="linenos">990</span></a><span class="sd">			assert next(table) == [2.,  0, &quot;2.3&quot;]</span>
-</span><span id="TypeParser-991"><a href="#TypeParser-991"><span class="linenos">991</span></a><span class="sd">			assert next(table) == [3.4, 2, &quot;abc&quot;]</span>
-</span><span id="TypeParser-992"><a href="#TypeParser-992"><span class="linenos">992</span></a><span class="sd">			```</span>
-</span><span id="TypeParser-993"><a href="#TypeParser-993"><span class="linenos">993</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser-994"><a href="#TypeParser-994"><span class="linenos">994</span></a>		<span class="n">inferred_types</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">infer_table</span><span class="p">(</span><span class="n">rows</span><span class="p">)</span>
-</span><span id="TypeParser-995"><a href="#TypeParser-995"><span class="linenos">995</span></a>
-</span><span id="TypeParser-996"><a href="#TypeParser-996"><span class="linenos">996</span></a>		<span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">rows</span><span class="p">:</span>
-</span><span id="TypeParser-997"><a href="#TypeParser-997"><span class="linenos">997</span></a>			<span class="k">yield</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">_convert</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">inferred</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span><span class="p">,</span> <span class="n">inferred</span> <span class="ow">in</span> <span class="nb">zip</span><span class="p">(</span><span class="n">row</span><span class="p">,</span> <span class="n">inferred_types</span><span class="p">)]</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser-60"><a href="#TypeParser-60"><span class="linenos">  60</span></a><span class="k">class</span> <span class="nc">TypeParser</span><span class="p">:</span>
+</span><span id="TypeParser-61"><a href="#TypeParser-61"><span class="linenos">  61</span></a><span class="w">	</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser-62"><a href="#TypeParser-62"><span class="linenos">  62</span></a><span class="sd">		A parser that can be used to infer the underlying types of data serialised as strings, and to convert them into their original underlying types.</span>
+</span><span id="TypeParser-63"><a href="#TypeParser-63"><span class="linenos">  63</span></a>
+</span><span id="TypeParser-64"><a href="#TypeParser-64"><span class="linenos">  64</span></a><span class="sd">		Instances of this class can be configured with different settings for the parser and inferrer. See the constructor for more details about the available options.</span>
+</span><span id="TypeParser-65"><a href="#TypeParser-65"><span class="linenos">  65</span></a><span class="sd">	&quot;&quot;&quot;</span>
+</span><span id="TypeParser-66"><a href="#TypeParser-66"><span class="linenos">  66</span></a>
+</span><span id="TypeParser-67"><a href="#TypeParser-67"><span class="linenos">  67</span></a>	<span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span>
+</span><span id="TypeParser-68"><a href="#TypeParser-68"><span class="linenos">  68</span></a>	    <span class="o">*</span><span class="p">,</span>
+</span><span id="TypeParser-69"><a href="#TypeParser-69"><span class="linenos">  69</span></a>		<span class="n">trim</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
+</span><span id="TypeParser-70"><a href="#TypeParser-70"><span class="linenos">  70</span></a>		<span class="n">use_decimal</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">False</span><span class="p">,</span>
+</span><span id="TypeParser-71"><a href="#TypeParser-71"><span class="linenos">  71</span></a>		<span class="n">list_delimiter</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="TypeParser-72"><a href="#TypeParser-72"><span class="linenos">  72</span></a>		<span class="n">none_values</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span><span class="o">=</span><span class="p">[</span><span class="s2">&quot;&quot;</span><span class="p">],</span>
+</span><span id="TypeParser-73"><a href="#TypeParser-73"><span class="linenos">  73</span></a>		<span class="n">none_case_sensitive</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">False</span><span class="p">,</span>
+</span><span id="TypeParser-74"><a href="#TypeParser-74"><span class="linenos">  74</span></a>		<span class="n">true_values</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span><span class="o">=</span><span class="p">[</span><span class="s2">&quot;true&quot;</span><span class="p">],</span>
+</span><span id="TypeParser-75"><a href="#TypeParser-75"><span class="linenos">  75</span></a>		<span class="n">false_values</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span><span class="o">=</span><span class="p">[</span><span class="s2">&quot;false&quot;</span><span class="p">],</span>
+</span><span id="TypeParser-76"><a href="#TypeParser-76"><span class="linenos">  76</span></a>		<span class="n">bool_case_sensitive</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">False</span><span class="p">,</span>
+</span><span id="TypeParser-77"><a href="#TypeParser-77"><span class="linenos">  77</span></a>		<span class="n">int_case_sensitive</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">False</span><span class="p">,</span>
+</span><span id="TypeParser-78"><a href="#TypeParser-78"><span class="linenos">  78</span></a>		<span class="n">inf_values</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span><span class="o">=</span><span class="p">[],</span>
+</span><span id="TypeParser-79"><a href="#TypeParser-79"><span class="linenos">  79</span></a>		<span class="n">nan_values</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span><span class="o">=</span><span class="p">[],</span>
+</span><span id="TypeParser-80"><a href="#TypeParser-80"><span class="linenos">  80</span></a>		<span class="n">float_case_sensitive</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">False</span><span class="p">,</span>
+</span><span id="TypeParser-81"><a href="#TypeParser-81"><span class="linenos">  81</span></a>		<span class="n">case_sensitive</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">bool</span><span class="p">]</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="TypeParser-82"><a href="#TypeParser-82"><span class="linenos">  82</span></a>	<span class="p">):</span>
+</span><span id="TypeParser-83"><a href="#TypeParser-83"><span class="linenos">  83</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser-84"><a href="#TypeParser-84"><span class="linenos">  84</span></a><span class="sd">			Initialise a new parser</span>
+</span><span id="TypeParser-85"><a href="#TypeParser-85"><span class="linenos">  85</span></a>
+</span><span id="TypeParser-86"><a href="#TypeParser-86"><span class="linenos">  86</span></a><span class="sd">			Parameters</span>
+</span><span id="TypeParser-87"><a href="#TypeParser-87"><span class="linenos">  87</span></a><span class="sd">			----------</span>
+</span><span id="TypeParser-88"><a href="#TypeParser-88"><span class="linenos">  88</span></a><span class="sd">			`trim`</span>
+</span><span id="TypeParser-89"><a href="#TypeParser-89"><span class="linenos">  89</span></a><span class="sd">			: whether leading and trailing whitespace should be stripped from strings</span>
+</span><span id="TypeParser-90"><a href="#TypeParser-90"><span class="linenos">  90</span></a>
+</span><span id="TypeParser-91"><a href="#TypeParser-91"><span class="linenos">  91</span></a><span class="sd">			`use_decimal`</span>
+</span><span id="TypeParser-92"><a href="#TypeParser-92"><span class="linenos">  92</span></a><span class="sd">			: whether non-integer numeric values should be inferred as Decimal (exact values) instead of float (non-exact values). Note that this only applies to methods that attempt to infer type (`infer()` and `infer_*()`), and does not affect methods where the type is explicitly specified (`is_float()`, `is_decimal()`, `parse_float()`, `parse_decimal()`).</span>
+</span><span id="TypeParser-93"><a href="#TypeParser-93"><span class="linenos">  93</span></a>
+</span><span id="TypeParser-94"><a href="#TypeParser-94"><span class="linenos">  94</span></a><span class="sd">			`list_delimiter`</span>
+</span><span id="TypeParser-95"><a href="#TypeParser-95"><span class="linenos">  95</span></a><span class="sd">			: the delimiter used for identifying lists and for separating list items. If set to None, the parser will not attempt to identify lists when inferring types, which usually causes the value to be treated as a str instead.</span>
+</span><span id="TypeParser-96"><a href="#TypeParser-96"><span class="linenos">  96</span></a>
+</span><span id="TypeParser-97"><a href="#TypeParser-97"><span class="linenos">  97</span></a><span class="sd">			`none_values`</span>
+</span><span id="TypeParser-98"><a href="#TypeParser-98"><span class="linenos">  98</span></a><span class="sd">			: list of strings that represent the value None</span>
+</span><span id="TypeParser-99"><a href="#TypeParser-99"><span class="linenos">  99</span></a>
+</span><span id="TypeParser-100"><a href="#TypeParser-100"><span class="linenos"> 100</span></a><span class="sd">			`none_case_sensitive`</span>
+</span><span id="TypeParser-101"><a href="#TypeParser-101"><span class="linenos"> 101</span></a><span class="sd">			: whether matches against `none_values` should be made in a case-sensitive manner</span>
+</span><span id="TypeParser-102"><a href="#TypeParser-102"><span class="linenos"> 102</span></a>
+</span><span id="TypeParser-103"><a href="#TypeParser-103"><span class="linenos"> 103</span></a><span class="sd">			`true_values`</span>
+</span><span id="TypeParser-104"><a href="#TypeParser-104"><span class="linenos"> 104</span></a><span class="sd">			: list of strings that represent the bool value True</span>
+</span><span id="TypeParser-105"><a href="#TypeParser-105"><span class="linenos"> 105</span></a>
+</span><span id="TypeParser-106"><a href="#TypeParser-106"><span class="linenos"> 106</span></a><span class="sd">			`false_values`</span>
+</span><span id="TypeParser-107"><a href="#TypeParser-107"><span class="linenos"> 107</span></a><span class="sd">			: list of strings that represent the bool value False</span>
+</span><span id="TypeParser-108"><a href="#TypeParser-108"><span class="linenos"> 108</span></a>
+</span><span id="TypeParser-109"><a href="#TypeParser-109"><span class="linenos"> 109</span></a><span class="sd">			`bool_case_sensitive`</span>
+</span><span id="TypeParser-110"><a href="#TypeParser-110"><span class="linenos"> 110</span></a><span class="sd">			: whether matches against `true_values` and `false_values` should be made in a case-sensitive manner</span>
+</span><span id="TypeParser-111"><a href="#TypeParser-111"><span class="linenos"> 111</span></a>
+</span><span id="TypeParser-112"><a href="#TypeParser-112"><span class="linenos"> 112</span></a><span class="sd">			`int_case_sensitive`</span>
+</span><span id="TypeParser-113"><a href="#TypeParser-113"><span class="linenos"> 113</span></a><span class="sd">			: whether checks for int should be done in a case-sensitive manner. This usually only applies to values given in scientific notation, where the mantissa and exponent usually are separated by `e`.</span>
+</span><span id="TypeParser-114"><a href="#TypeParser-114"><span class="linenos"> 114</span></a>
+</span><span id="TypeParser-115"><a href="#TypeParser-115"><span class="linenos"> 115</span></a><span class="sd">			`inf_values`</span>
+</span><span id="TypeParser-116"><a href="#TypeParser-116"><span class="linenos"> 116</span></a><span class="sd">			: list of strings that represent the float or Decimal value of infinity. Each of the strings can be prepended with a negative sign to represent negative infinity also.</span>
+</span><span id="TypeParser-117"><a href="#TypeParser-117"><span class="linenos"> 117</span></a>
+</span><span id="TypeParser-118"><a href="#TypeParser-118"><span class="linenos"> 118</span></a><span class="sd">			`nan_values`</span>
+</span><span id="TypeParser-119"><a href="#TypeParser-119"><span class="linenos"> 119</span></a><span class="sd">			: list of strings that represent a float or Decimal that is NaN (not a number)</span>
+</span><span id="TypeParser-120"><a href="#TypeParser-120"><span class="linenos"> 120</span></a>
+</span><span id="TypeParser-121"><a href="#TypeParser-121"><span class="linenos"> 121</span></a><span class="sd">			`float_case_sensitive`</span>
+</span><span id="TypeParser-122"><a href="#TypeParser-122"><span class="linenos"> 122</span></a><span class="sd">			: whether checks for float should be done in a case-sensitive manner. This applies to matches against `inf_values` and `nan_values`, as well as to values given in scientific notation, where the mantissa and exponent are usually separated by `e`.</span>
+</span><span id="TypeParser-123"><a href="#TypeParser-123"><span class="linenos"> 123</span></a>
+</span><span id="TypeParser-124"><a href="#TypeParser-124"><span class="linenos"> 124</span></a><span class="sd">			`case_sensitive`</span>
+</span><span id="TypeParser-125"><a href="#TypeParser-125"><span class="linenos"> 125</span></a><span class="sd">			: whether all matches should be made in a case-sensitive manner. Sets all of `none_case_sensitive`, `bool_case_sensitive`, `int_case_sensitive`, `float_case_sensitive` to the same value, ignoring any individual settings.</span>
+</span><span id="TypeParser-126"><a href="#TypeParser-126"><span class="linenos"> 126</span></a>
+</span><span id="TypeParser-127"><a href="#TypeParser-127"><span class="linenos"> 127</span></a><span class="sd">			Raises</span>
+</span><span id="TypeParser-128"><a href="#TypeParser-128"><span class="linenos"> 128</span></a><span class="sd">			------</span>
+</span><span id="TypeParser-129"><a href="#TypeParser-129"><span class="linenos"> 129</span></a><span class="sd">			`ValueError` if any of the options would lead to ambiguities during parsing</span>
+</span><span id="TypeParser-130"><a href="#TypeParser-130"><span class="linenos"> 130</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser-131"><a href="#TypeParser-131"><span class="linenos"> 131</span></a>
+</span><span id="TypeParser-132"><a href="#TypeParser-132"><span class="linenos"> 132</span></a>		<span class="k">if</span> <span class="n">case_sensitive</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="TypeParser-133"><a href="#TypeParser-133"><span class="linenos"> 133</span></a>			<span class="n">none_case_sensitive</span> <span class="o">=</span> <span class="n">case_sensitive</span>
+</span><span id="TypeParser-134"><a href="#TypeParser-134"><span class="linenos"> 134</span></a>			<span class="n">int_case_sensitive</span> <span class="o">=</span> <span class="n">case_sensitive</span>
+</span><span id="TypeParser-135"><a href="#TypeParser-135"><span class="linenos"> 135</span></a>			<span class="n">bool_case_sensitive</span> <span class="o">=</span> <span class="n">case_sensitive</span>
+</span><span id="TypeParser-136"><a href="#TypeParser-136"><span class="linenos"> 136</span></a>			<span class="n">float_case_sensitive</span> <span class="o">=</span> <span class="n">case_sensitive</span>
+</span><span id="TypeParser-137"><a href="#TypeParser-137"><span class="linenos"> 137</span></a>
+</span><span id="TypeParser-138"><a href="#TypeParser-138"><span class="linenos"> 138</span></a>		<span class="bp">self</span><span class="o">.</span><span class="n">trim</span> <span class="o">=</span> <span class="n">trim</span>
+</span><span id="TypeParser-139"><a href="#TypeParser-139"><span class="linenos"> 139</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">trim</span><span class="p">:</span>
+</span><span id="TypeParser-140"><a href="#TypeParser-140"><span class="linenos"> 140</span></a>			<span class="n">none_values</span> <span class="o">=</span> <span class="p">(</span><span class="n">value</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">none_values</span><span class="p">)</span>
+</span><span id="TypeParser-141"><a href="#TypeParser-141"><span class="linenos"> 141</span></a>			<span class="n">true_values</span> <span class="o">=</span> <span class="p">(</span><span class="n">value</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">true_values</span><span class="p">)</span>
+</span><span id="TypeParser-142"><a href="#TypeParser-142"><span class="linenos"> 142</span></a>			<span class="n">false_values</span> <span class="o">=</span> <span class="p">(</span><span class="n">value</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">false_values</span><span class="p">)</span>
+</span><span id="TypeParser-143"><a href="#TypeParser-143"><span class="linenos"> 143</span></a>			<span class="n">inf_values</span> <span class="o">=</span> <span class="p">(</span><span class="n">value</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">inf_values</span><span class="p">)</span>
+</span><span id="TypeParser-144"><a href="#TypeParser-144"><span class="linenos"> 144</span></a>			<span class="n">nan_values</span> <span class="o">=</span> <span class="p">(</span><span class="n">value</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">nan_values</span><span class="p">)</span>
+</span><span id="TypeParser-145"><a href="#TypeParser-145"><span class="linenos"> 145</span></a>
+</span><span id="TypeParser-146"><a href="#TypeParser-146"><span class="linenos"> 146</span></a>		<span class="bp">self</span><span class="o">.</span><span class="n">use_decimal</span> <span class="o">=</span> <span class="n">use_decimal</span>
+</span><span id="TypeParser-147"><a href="#TypeParser-147"><span class="linenos"> 147</span></a>		<span class="bp">self</span><span class="o">.</span><span class="n">list_delimiter</span> <span class="o">=</span> <span class="n">list_delimiter</span>
+</span><span id="TypeParser-148"><a href="#TypeParser-148"><span class="linenos"> 148</span></a>
+</span><span id="TypeParser-149"><a href="#TypeParser-149"><span class="linenos"> 149</span></a>		<span class="bp">self</span><span class="o">.</span><span class="n">none_case_sensitive</span> <span class="o">=</span> <span class="n">none_case_sensitive</span>
+</span><span id="TypeParser-150"><a href="#TypeParser-150"><span class="linenos"> 150</span></a>		<span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">none_case_sensitive</span><span class="p">:</span>
+</span><span id="TypeParser-151"><a href="#TypeParser-151"><span class="linenos"> 151</span></a>			<span class="n">none_values</span> <span class="o">=</span> <span class="p">(</span><span class="n">value</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">none_values</span><span class="p">)</span>
+</span><span id="TypeParser-152"><a href="#TypeParser-152"><span class="linenos"> 152</span></a>		<span class="bp">self</span><span class="o">.</span><span class="n">none_values</span> <span class="o">=</span> <span class="nb">set</span><span class="p">(</span><span class="n">none_values</span><span class="p">)</span>
+</span><span id="TypeParser-153"><a href="#TypeParser-153"><span class="linenos"> 153</span></a>
+</span><span id="TypeParser-154"><a href="#TypeParser-154"><span class="linenos"> 154</span></a>		<span class="bp">self</span><span class="o">.</span><span class="n">bool_case_sensitive</span> <span class="o">=</span> <span class="n">bool_case_sensitive</span>
+</span><span id="TypeParser-155"><a href="#TypeParser-155"><span class="linenos"> 155</span></a>		<span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">bool_case_sensitive</span><span class="p">:</span>
+</span><span id="TypeParser-156"><a href="#TypeParser-156"><span class="linenos"> 156</span></a>			<span class="n">true_values</span> <span class="o">=</span> <span class="p">(</span><span class="n">value</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">true_values</span><span class="p">)</span>
+</span><span id="TypeParser-157"><a href="#TypeParser-157"><span class="linenos"> 157</span></a>			<span class="n">false_values</span> <span class="o">=</span> <span class="p">(</span><span class="n">value</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">false_values</span><span class="p">)</span>
+</span><span id="TypeParser-158"><a href="#TypeParser-158"><span class="linenos"> 158</span></a>		<span class="bp">self</span><span class="o">.</span><span class="n">true_values</span> <span class="o">=</span> <span class="nb">set</span><span class="p">(</span><span class="n">true_values</span><span class="p">)</span>
+</span><span id="TypeParser-159"><a href="#TypeParser-159"><span class="linenos"> 159</span></a>		<span class="bp">self</span><span class="o">.</span><span class="n">false_values</span> <span class="o">=</span> <span class="nb">set</span><span class="p">(</span><span class="n">false_values</span><span class="p">)</span>
+</span><span id="TypeParser-160"><a href="#TypeParser-160"><span class="linenos"> 160</span></a>
+</span><span id="TypeParser-161"><a href="#TypeParser-161"><span class="linenos"> 161</span></a>		<span class="bp">self</span><span class="o">.</span><span class="n">int_case_sensitive</span> <span class="o">=</span> <span class="n">int_case_sensitive</span>
+</span><span id="TypeParser-162"><a href="#TypeParser-162"><span class="linenos"> 162</span></a>
+</span><span id="TypeParser-163"><a href="#TypeParser-163"><span class="linenos"> 163</span></a>		<span class="bp">self</span><span class="o">.</span><span class="n">float_case_sensitive</span> <span class="o">=</span> <span class="n">float_case_sensitive</span>
+</span><span id="TypeParser-164"><a href="#TypeParser-164"><span class="linenos"> 164</span></a>		<span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">float_case_sensitive</span><span class="p">:</span>
+</span><span id="TypeParser-165"><a href="#TypeParser-165"><span class="linenos"> 165</span></a>			<span class="n">inf_values</span> <span class="o">=</span> <span class="p">(</span><span class="n">value</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">inf_values</span><span class="p">)</span>
+</span><span id="TypeParser-166"><a href="#TypeParser-166"><span class="linenos"> 166</span></a>			<span class="n">nan_values</span> <span class="o">=</span> <span class="p">(</span><span class="n">value</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">nan_values</span><span class="p">)</span>
+</span><span id="TypeParser-167"><a href="#TypeParser-167"><span class="linenos"> 167</span></a>		<span class="bp">self</span><span class="o">.</span><span class="n">inf_values</span> <span class="o">=</span> <span class="nb">set</span><span class="p">(</span><span class="n">inf_values</span><span class="p">)</span>
+</span><span id="TypeParser-168"><a href="#TypeParser-168"><span class="linenos"> 168</span></a>		<span class="bp">self</span><span class="o">.</span><span class="n">nan_values</span> <span class="o">=</span> <span class="nb">set</span><span class="p">(</span><span class="n">nan_values</span><span class="p">)</span>
+</span><span id="TypeParser-169"><a href="#TypeParser-169"><span class="linenos"> 169</span></a>
+</span><span id="TypeParser-170"><a href="#TypeParser-170"><span class="linenos"> 170</span></a>		<span class="c1"># Unconfigurable default values</span>
+</span><span id="TypeParser-171"><a href="#TypeParser-171"><span class="linenos"> 171</span></a>		<span class="bp">self</span><span class="o">.</span><span class="n">_negative_char</span> <span class="o">=</span> <span class="s2">&quot;-&quot;</span>
+</span><span id="TypeParser-172"><a href="#TypeParser-172"><span class="linenos"> 172</span></a>		<span class="bp">self</span><span class="o">.</span><span class="n">_negative_chars</span> <span class="o">=</span> <span class="p">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_negative_char</span><span class="p">,</span> <span class="s2">&quot;−&quot;</span><span class="p">}</span>
+</span><span id="TypeParser-173"><a href="#TypeParser-173"><span class="linenos"> 173</span></a>		<span class="bp">self</span><span class="o">.</span><span class="n">_sign_chars</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_negative_chars</span> <span class="o">|</span> <span class="p">{</span><span class="s2">&quot;+&quot;</span><span class="p">}</span>
+</span><span id="TypeParser-174"><a href="#TypeParser-174"><span class="linenos"> 174</span></a>		<span class="bp">self</span><span class="o">.</span><span class="n">_digit_chars</span> <span class="o">=</span> <span class="p">{</span><span class="s2">&quot;0&quot;</span><span class="p">,</span> <span class="s2">&quot;1&quot;</span><span class="p">,</span> <span class="s2">&quot;2&quot;</span><span class="p">,</span> <span class="s2">&quot;3&quot;</span><span class="p">,</span> <span class="s2">&quot;4&quot;</span><span class="p">,</span> <span class="s2">&quot;5&quot;</span><span class="p">,</span> <span class="s2">&quot;6&quot;</span><span class="p">,</span> <span class="s2">&quot;7&quot;</span><span class="p">,</span> <span class="s2">&quot;8&quot;</span><span class="p">,</span> <span class="s2">&quot;9&quot;</span><span class="p">}</span>  <span class="c1"># Because isdigit(&quot;²&quot;) == True, but int(&quot;²&quot;) is invalid</span>
+</span><span id="TypeParser-175"><a href="#TypeParser-175"><span class="linenos"> 175</span></a>		<span class="bp">self</span><span class="o">.</span><span class="n">_digit_separators</span> <span class="o">=</span> <span class="p">{</span><span class="s2">&quot;_&quot;</span><span class="p">}</span>
+</span><span id="TypeParser-176"><a href="#TypeParser-176"><span class="linenos"> 176</span></a>		<span class="bp">self</span><span class="o">.</span><span class="n">_scientific_char</span> <span class="o">=</span> <span class="s2">&quot;e&quot;</span>
+</span><span id="TypeParser-177"><a href="#TypeParser-177"><span class="linenos"> 177</span></a>		<span class="bp">self</span><span class="o">.</span><span class="n">_float_separator</span> <span class="o">=</span> <span class="s2">&quot;.&quot;</span>
+</span><span id="TypeParser-178"><a href="#TypeParser-178"><span class="linenos"> 178</span></a>		<span class="bp">self</span><span class="o">.</span><span class="n">_reserved_chars</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_sign_chars</span> <span class="o">|</span> <span class="bp">self</span><span class="o">.</span><span class="n">_digit_chars</span> <span class="o">|</span> <span class="bp">self</span><span class="o">.</span><span class="n">_digit_separators</span> <span class="o">|</span> <span class="p">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_scientific_char</span><span class="p">}</span> <span class="o">|</span> <span class="p">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_float_separator</span><span class="p">}</span>
+</span><span id="TypeParser-179"><a href="#TypeParser-179"><span class="linenos"> 179</span></a>		<span class="c1"># special_chars = self._reserved_chars | self.list_delimiter</span>
+</span><span id="TypeParser-180"><a href="#TypeParser-180"><span class="linenos"> 180</span></a>
+</span><span id="TypeParser-181"><a href="#TypeParser-181"><span class="linenos"> 181</span></a>		<span class="c1"># Check if any special values conflict</span>
+</span><span id="TypeParser-182"><a href="#TypeParser-182"><span class="linenos"> 182</span></a>		<span class="k">for</span> <span class="n">name</span><span class="p">,</span> <span class="n">special_values</span> <span class="ow">in</span> <span class="p">[</span>
+</span><span id="TypeParser-183"><a href="#TypeParser-183"><span class="linenos"> 183</span></a>			<span class="p">(</span><span class="n">_SpecialValue</span><span class="o">.</span><span class="n">LIST</span><span class="p">,</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">list_delimiter</span><span class="p">]</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">list_delimiter</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span> <span class="k">else</span> <span class="p">[]),</span>
+</span><span id="TypeParser-184"><a href="#TypeParser-184"><span class="linenos"> 184</span></a>			<span class="p">(</span><span class="n">_SpecialValue</span><span class="o">.</span><span class="n">NONE</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">none_values</span><span class="p">),</span>
+</span><span id="TypeParser-185"><a href="#TypeParser-185"><span class="linenos"> 185</span></a>			<span class="p">(</span><span class="n">_SpecialValue</span><span class="o">.</span><span class="n">TRUE</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">true_values</span><span class="p">),</span>
+</span><span id="TypeParser-186"><a href="#TypeParser-186"><span class="linenos"> 186</span></a>			<span class="p">(</span><span class="n">_SpecialValue</span><span class="o">.</span><span class="n">FALSE</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">false_values</span><span class="p">),</span>
+</span><span id="TypeParser-187"><a href="#TypeParser-187"><span class="linenos"> 187</span></a>			<span class="p">(</span><span class="n">_SpecialValue</span><span class="o">.</span><span class="n">INF</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">inf_values</span><span class="p">),</span>
+</span><span id="TypeParser-188"><a href="#TypeParser-188"><span class="linenos"> 188</span></a>			<span class="p">(</span><span class="n">_SpecialValue</span><span class="o">.</span><span class="n">NAN</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">nan_values</span><span class="p">),</span>
+</span><span id="TypeParser-189"><a href="#TypeParser-189"><span class="linenos"> 189</span></a>		<span class="p">]:</span>
+</span><span id="TypeParser-190"><a href="#TypeParser-190"><span class="linenos"> 190</span></a>			<span class="k">for</span> <span class="n">special_value</span> <span class="ow">in</span> <span class="n">special_values</span><span class="p">:</span>
+</span><span id="TypeParser-191"><a href="#TypeParser-191"><span class="linenos"> 191</span></a>				<span class="k">if</span> <span class="n">special_value</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_reserved_chars</span><span class="p">:</span>
+</span><span id="TypeParser-192"><a href="#TypeParser-192"><span class="linenos"> 192</span></a>					<span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;cannot use reserved char as </span><span class="si">{</span><span class="n">name</span><span class="o">.</span><span class="n">value</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">special_value</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="TypeParser-193"><a href="#TypeParser-193"><span class="linenos"> 193</span></a>
+</span><span id="TypeParser-194"><a href="#TypeParser-194"><span class="linenos"> 194</span></a>				<span class="k">if</span> <span class="n">name</span> <span class="o">!=</span> <span class="n">_SpecialValue</span><span class="o">.</span><span class="n">NONE</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_none</span><span class="p">(</span><span class="n">special_value</span><span class="p">):</span>
+</span><span id="TypeParser-195"><a href="#TypeParser-195"><span class="linenos"> 195</span></a>					<span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;cannot use None value as </span><span class="si">{</span><span class="n">name</span><span class="o">.</span><span class="n">value</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">special_value</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="TypeParser-196"><a href="#TypeParser-196"><span class="linenos"> 196</span></a>
+</span><span id="TypeParser-197"><a href="#TypeParser-197"><span class="linenos"> 197</span></a>				<span class="k">if</span> <span class="p">(</span>
+</span><span id="TypeParser-198"><a href="#TypeParser-198"><span class="linenos"> 198</span></a>					<span class="p">(</span><span class="n">name</span> <span class="o">==</span> <span class="n">_SpecialValue</span><span class="o">.</span><span class="n">TRUE</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_bool</span><span class="p">(</span><span class="n">special_value</span><span class="p">)</span> <span class="o">!=</span> <span class="kc">True</span><span class="p">)</span> <span class="ow">or</span>
+</span><span id="TypeParser-199"><a href="#TypeParser-199"><span class="linenos"> 199</span></a>					<span class="p">(</span><span class="n">name</span> <span class="o">==</span> <span class="n">_SpecialValue</span><span class="o">.</span><span class="n">FALSE</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_bool</span><span class="p">(</span><span class="n">special_value</span><span class="p">)</span> <span class="o">!=</span> <span class="kc">False</span><span class="p">)</span> <span class="ow">or</span>
+</span><span id="TypeParser-200"><a href="#TypeParser-200"><span class="linenos"> 200</span></a>					<span class="p">(</span><span class="n">name</span> <span class="o">!=</span> <span class="n">_SpecialValue</span><span class="o">.</span><span class="n">TRUE</span> <span class="ow">and</span> <span class="n">name</span> <span class="o">!=</span> <span class="n">_SpecialValue</span><span class="o">.</span><span class="n">FALSE</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_bool</span><span class="p">(</span><span class="n">special_value</span><span class="p">))</span>
+</span><span id="TypeParser-201"><a href="#TypeParser-201"><span class="linenos"> 201</span></a>				<span class="p">):</span>
+</span><span id="TypeParser-202"><a href="#TypeParser-202"><span class="linenos"> 202</span></a>					<span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;cannot use bool value as </span><span class="si">{</span><span class="n">name</span><span class="o">.</span><span class="n">value</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">special_value</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="TypeParser-203"><a href="#TypeParser-203"><span class="linenos"> 203</span></a>
+</span><span id="TypeParser-204"><a href="#TypeParser-204"><span class="linenos"> 204</span></a>				<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_int</span><span class="p">(</span><span class="n">special_value</span><span class="p">):</span>
+</span><span id="TypeParser-205"><a href="#TypeParser-205"><span class="linenos"> 205</span></a>					<span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;cannot use int value as </span><span class="si">{</span><span class="n">name</span><span class="o">.</span><span class="n">value</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">special_value</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="TypeParser-206"><a href="#TypeParser-206"><span class="linenos"> 206</span></a>
+</span><span id="TypeParser-207"><a href="#TypeParser-207"><span class="linenos"> 207</span></a>				<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">use_decimal</span><span class="p">:</span>
+</span><span id="TypeParser-208"><a href="#TypeParser-208"><span class="linenos"> 208</span></a>					<span class="k">if</span> <span class="p">(</span>
+</span><span id="TypeParser-209"><a href="#TypeParser-209"><span class="linenos"> 209</span></a>						<span class="p">(</span><span class="n">name</span> <span class="o">==</span> <span class="n">_SpecialValue</span><span class="o">.</span><span class="n">INF</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_decimal</span><span class="p">(</span><span class="n">special_value</span><span class="p">)</span> <span class="o">!=</span> <span class="n">Decimal</span><span class="p">(</span><span class="n">math</span><span class="o">.</span><span class="n">inf</span><span class="p">))</span> <span class="ow">or</span>
+</span><span id="TypeParser-210"><a href="#TypeParser-210"><span class="linenos"> 210</span></a>						<span class="p">(</span><span class="n">name</span> <span class="o">==</span> <span class="n">_SpecialValue</span><span class="o">.</span><span class="n">NAN</span> <span class="ow">and</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_decimal</span><span class="p">(</span><span class="n">special_value</span><span class="p">)</span><span class="o">.</span><span class="n">is_nan</span><span class="p">())</span> <span class="ow">or</span>
+</span><span id="TypeParser-211"><a href="#TypeParser-211"><span class="linenos"> 211</span></a>						<span class="p">(</span><span class="n">name</span> <span class="o">!=</span> <span class="n">_SpecialValue</span><span class="o">.</span><span class="n">INF</span> <span class="ow">and</span> <span class="n">name</span> <span class="o">!=</span> <span class="n">_SpecialValue</span><span class="o">.</span><span class="n">NAN</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_float</span><span class="p">(</span><span class="n">special_value</span><span class="p">))</span>
+</span><span id="TypeParser-212"><a href="#TypeParser-212"><span class="linenos"> 212</span></a>					<span class="p">):</span>
+</span><span id="TypeParser-213"><a href="#TypeParser-213"><span class="linenos"> 213</span></a>						<span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;cannot use Decimal value as </span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">special_value</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="TypeParser-214"><a href="#TypeParser-214"><span class="linenos"> 214</span></a>				<span class="k">else</span><span class="p">:</span>
+</span><span id="TypeParser-215"><a href="#TypeParser-215"><span class="linenos"> 215</span></a>					<span class="k">if</span> <span class="p">(</span>
+</span><span id="TypeParser-216"><a href="#TypeParser-216"><span class="linenos"> 216</span></a>						<span class="p">(</span><span class="n">name</span> <span class="o">==</span> <span class="n">_SpecialValue</span><span class="o">.</span><span class="n">INF</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_float</span><span class="p">(</span><span class="n">special_value</span><span class="p">)</span> <span class="o">!=</span> <span class="n">math</span><span class="o">.</span><span class="n">inf</span><span class="p">)</span> <span class="ow">or</span>
+</span><span id="TypeParser-217"><a href="#TypeParser-217"><span class="linenos"> 217</span></a>						<span class="p">(</span><span class="n">name</span> <span class="o">==</span> <span class="n">_SpecialValue</span><span class="o">.</span><span class="n">NAN</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_float</span><span class="p">(</span><span class="n">special_value</span><span class="p">)</span> <span class="ow">is</span> <span class="ow">not</span> <span class="n">math</span><span class="o">.</span><span class="n">nan</span><span class="p">)</span> <span class="ow">or</span>
+</span><span id="TypeParser-218"><a href="#TypeParser-218"><span class="linenos"> 218</span></a>						<span class="p">(</span><span class="n">name</span> <span class="o">!=</span> <span class="n">_SpecialValue</span><span class="o">.</span><span class="n">INF</span> <span class="ow">and</span> <span class="n">name</span> <span class="o">!=</span> <span class="n">_SpecialValue</span><span class="o">.</span><span class="n">NAN</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_float</span><span class="p">(</span><span class="n">special_value</span><span class="p">))</span>
+</span><span id="TypeParser-219"><a href="#TypeParser-219"><span class="linenos"> 219</span></a>					<span class="p">):</span>
+</span><span id="TypeParser-220"><a href="#TypeParser-220"><span class="linenos"> 220</span></a>						<span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;cannot use float value as </span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">special_value</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="TypeParser-221"><a href="#TypeParser-221"><span class="linenos"> 221</span></a>
+</span><span id="TypeParser-222"><a href="#TypeParser-222"><span class="linenos"> 222</span></a>
+</span><span id="TypeParser-223"><a href="#TypeParser-223"><span class="linenos"> 223</span></a>	<span class="k">def</span> <span class="nf">is_none</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="TypeParser-224"><a href="#TypeParser-224"><span class="linenos"> 224</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser-225"><a href="#TypeParser-225"><span class="linenos"> 225</span></a><span class="sd">			Check if a string represents the value None</span>
+</span><span id="TypeParser-226"><a href="#TypeParser-226"><span class="linenos"> 226</span></a>
+</span><span id="TypeParser-227"><a href="#TypeParser-227"><span class="linenos"> 227</span></a><span class="sd">			Only strings that match the values in `self.none_values` will be interpreted as None. The default accepted values are `[&quot;&quot;]`, i.e. an empty string. The case sensitivity of this matching depends on `self.none_case_sensitive`, which is False by default.</span>
+</span><span id="TypeParser-228"><a href="#TypeParser-228"><span class="linenos"> 228</span></a>
+</span><span id="TypeParser-229"><a href="#TypeParser-229"><span class="linenos"> 229</span></a><span class="sd">			Parameters</span>
+</span><span id="TypeParser-230"><a href="#TypeParser-230"><span class="linenos"> 230</span></a><span class="sd">			----------</span>
+</span><span id="TypeParser-231"><a href="#TypeParser-231"><span class="linenos"> 231</span></a><span class="sd">			`value`</span>
+</span><span id="TypeParser-232"><a href="#TypeParser-232"><span class="linenos"> 232</span></a><span class="sd">			: string to be checked</span>
+</span><span id="TypeParser-233"><a href="#TypeParser-233"><span class="linenos"> 233</span></a>
+</span><span id="TypeParser-234"><a href="#TypeParser-234"><span class="linenos"> 234</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser-235"><a href="#TypeParser-235"><span class="linenos"> 235</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser-236"><a href="#TypeParser-236"><span class="linenos"> 236</span></a><span class="sd">			whether it is None</span>
+</span><span id="TypeParser-237"><a href="#TypeParser-237"><span class="linenos"> 237</span></a>
+</span><span id="TypeParser-238"><a href="#TypeParser-238"><span class="linenos"> 238</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser-239"><a href="#TypeParser-239"><span class="linenos"> 239</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser-240"><a href="#TypeParser-240"><span class="linenos"> 240</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser-241"><a href="#TypeParser-241"><span class="linenos"> 241</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser-242"><a href="#TypeParser-242"><span class="linenos"> 242</span></a><span class="sd">			parser.parse_bool(&quot;&quot;)     # True</span>
+</span><span id="TypeParser-243"><a href="#TypeParser-243"><span class="linenos"> 243</span></a><span class="sd">			parser.parse_bool(&quot;abc&quot;)  # False</span>
+</span><span id="TypeParser-244"><a href="#TypeParser-244"><span class="linenos"> 244</span></a><span class="sd">			```</span>
+</span><span id="TypeParser-245"><a href="#TypeParser-245"><span class="linenos"> 245</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser-246"><a href="#TypeParser-246"><span class="linenos"> 246</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">trim</span><span class="p">:</span>
+</span><span id="TypeParser-247"><a href="#TypeParser-247"><span class="linenos"> 247</span></a>			<span class="n">value</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
+</span><span id="TypeParser-248"><a href="#TypeParser-248"><span class="linenos"> 248</span></a>		<span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">bool_case_sensitive</span><span class="p">:</span>
+</span><span id="TypeParser-249"><a href="#TypeParser-249"><span class="linenos"> 249</span></a>			<span class="n">value</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span>
+</span><span id="TypeParser-250"><a href="#TypeParser-250"><span class="linenos"> 250</span></a>
+</span><span id="TypeParser-251"><a href="#TypeParser-251"><span class="linenos"> 251</span></a>		<span class="k">if</span> <span class="n">value</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">none_values</span><span class="p">:</span>
+</span><span id="TypeParser-252"><a href="#TypeParser-252"><span class="linenos"> 252</span></a>			<span class="k">return</span> <span class="kc">True</span>
+</span><span id="TypeParser-253"><a href="#TypeParser-253"><span class="linenos"> 253</span></a>		<span class="k">else</span><span class="p">:</span>
+</span><span id="TypeParser-254"><a href="#TypeParser-254"><span class="linenos"> 254</span></a>			<span class="k">return</span> <span class="kc">False</span>
+</span><span id="TypeParser-255"><a href="#TypeParser-255"><span class="linenos"> 255</span></a>
+</span><span id="TypeParser-256"><a href="#TypeParser-256"><span class="linenos"> 256</span></a>
+</span><span id="TypeParser-257"><a href="#TypeParser-257"><span class="linenos"> 257</span></a>	<span class="k">def</span> <span class="nf">is_bool</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="TypeParser-258"><a href="#TypeParser-258"><span class="linenos"> 258</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser-259"><a href="#TypeParser-259"><span class="linenos"> 259</span></a><span class="sd">			Check if a string represents a bool</span>
+</span><span id="TypeParser-260"><a href="#TypeParser-260"><span class="linenos"> 260</span></a>
+</span><span id="TypeParser-261"><a href="#TypeParser-261"><span class="linenos"> 261</span></a><span class="sd">			Only strings that match the values in `self.true_values` and `self.false_values` will be interpreted as booleans. The default accepted values are `[&quot;true&quot;]` and `[&quot;false&quot;]` respectively. The case sensitivity of this matching depends on `self.bool_case_sensitive`, which is False by default.</span>
+</span><span id="TypeParser-262"><a href="#TypeParser-262"><span class="linenos"> 262</span></a>
+</span><span id="TypeParser-263"><a href="#TypeParser-263"><span class="linenos"> 263</span></a><span class="sd">			Parameters</span>
+</span><span id="TypeParser-264"><a href="#TypeParser-264"><span class="linenos"> 264</span></a><span class="sd">			----------</span>
+</span><span id="TypeParser-265"><a href="#TypeParser-265"><span class="linenos"> 265</span></a><span class="sd">			`value`</span>
+</span><span id="TypeParser-266"><a href="#TypeParser-266"><span class="linenos"> 266</span></a><span class="sd">			: string to be checked</span>
+</span><span id="TypeParser-267"><a href="#TypeParser-267"><span class="linenos"> 267</span></a>
+</span><span id="TypeParser-268"><a href="#TypeParser-268"><span class="linenos"> 268</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser-269"><a href="#TypeParser-269"><span class="linenos"> 269</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser-270"><a href="#TypeParser-270"><span class="linenos"> 270</span></a><span class="sd">			whether it is a bool</span>
+</span><span id="TypeParser-271"><a href="#TypeParser-271"><span class="linenos"> 271</span></a>
+</span><span id="TypeParser-272"><a href="#TypeParser-272"><span class="linenos"> 272</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser-273"><a href="#TypeParser-273"><span class="linenos"> 273</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser-274"><a href="#TypeParser-274"><span class="linenos"> 274</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser-275"><a href="#TypeParser-275"><span class="linenos"> 275</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser-276"><a href="#TypeParser-276"><span class="linenos"> 276</span></a><span class="sd">			parser.is_bool(&quot;true&quot;)  # True</span>
+</span><span id="TypeParser-277"><a href="#TypeParser-277"><span class="linenos"> 277</span></a><span class="sd">			parser.is_bool(&quot;&quot;)      # True</span>
+</span><span id="TypeParser-278"><a href="#TypeParser-278"><span class="linenos"> 278</span></a><span class="sd">			parser.is_bool(&quot;abc&quot;)   # False</span>
+</span><span id="TypeParser-279"><a href="#TypeParser-279"><span class="linenos"> 279</span></a><span class="sd">			```</span>
+</span><span id="TypeParser-280"><a href="#TypeParser-280"><span class="linenos"> 280</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser-281"><a href="#TypeParser-281"><span class="linenos"> 281</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">trim</span><span class="p">:</span>
+</span><span id="TypeParser-282"><a href="#TypeParser-282"><span class="linenos"> 282</span></a>			<span class="n">value</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
+</span><span id="TypeParser-283"><a href="#TypeParser-283"><span class="linenos"> 283</span></a>
+</span><span id="TypeParser-284"><a href="#TypeParser-284"><span class="linenos"> 284</span></a>		<span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">bool_case_sensitive</span><span class="p">:</span>
+</span><span id="TypeParser-285"><a href="#TypeParser-285"><span class="linenos"> 285</span></a>			<span class="n">value</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span>
+</span><span id="TypeParser-286"><a href="#TypeParser-286"><span class="linenos"> 286</span></a>		<span class="k">if</span> <span class="n">value</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">true_values</span><span class="p">:</span>
+</span><span id="TypeParser-287"><a href="#TypeParser-287"><span class="linenos"> 287</span></a>			<span class="k">return</span> <span class="kc">True</span>
+</span><span id="TypeParser-288"><a href="#TypeParser-288"><span class="linenos"> 288</span></a>		<span class="k">if</span> <span class="n">value</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">false_values</span><span class="p">:</span>
+</span><span id="TypeParser-289"><a href="#TypeParser-289"><span class="linenos"> 289</span></a>			<span class="k">return</span> <span class="kc">True</span>
+</span><span id="TypeParser-290"><a href="#TypeParser-290"><span class="linenos"> 290</span></a>
+</span><span id="TypeParser-291"><a href="#TypeParser-291"><span class="linenos"> 291</span></a>		<span class="k">return</span> <span class="kc">False</span>
+</span><span id="TypeParser-292"><a href="#TypeParser-292"><span class="linenos"> 292</span></a>
+</span><span id="TypeParser-293"><a href="#TypeParser-293"><span class="linenos"> 293</span></a>
+</span><span id="TypeParser-294"><a href="#TypeParser-294"><span class="linenos"> 294</span></a>	<span class="k">def</span> <span class="nf">is_int</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="o">*</span><span class="p">,</span> <span class="n">allow_sign</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_negative</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="TypeParser-295"><a href="#TypeParser-295"><span class="linenos"> 295</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser-296"><a href="#TypeParser-296"><span class="linenos"> 296</span></a><span class="sd">			Check if a string represents an int</span>
+</span><span id="TypeParser-297"><a href="#TypeParser-297"><span class="linenos"> 297</span></a>
+</span><span id="TypeParser-298"><a href="#TypeParser-298"><span class="linenos"> 298</span></a><span class="sd">			Parameters</span>
+</span><span id="TypeParser-299"><a href="#TypeParser-299"><span class="linenos"> 299</span></a><span class="sd">			----------</span>
+</span><span id="TypeParser-300"><a href="#TypeParser-300"><span class="linenos"> 300</span></a><span class="sd">			`value`</span>
+</span><span id="TypeParser-301"><a href="#TypeParser-301"><span class="linenos"> 301</span></a><span class="sd">			: string to be checked</span>
+</span><span id="TypeParser-302"><a href="#TypeParser-302"><span class="linenos"> 302</span></a>
+</span><span id="TypeParser-303"><a href="#TypeParser-303"><span class="linenos"> 303</span></a><span class="sd">			`allow_negative`</span>
+</span><span id="TypeParser-304"><a href="#TypeParser-304"><span class="linenos"> 304</span></a><span class="sd">			: whether to accept negative values</span>
+</span><span id="TypeParser-305"><a href="#TypeParser-305"><span class="linenos"> 305</span></a>
+</span><span id="TypeParser-306"><a href="#TypeParser-306"><span class="linenos"> 306</span></a><span class="sd">			`allow_sign`</span>
+</span><span id="TypeParser-307"><a href="#TypeParser-307"><span class="linenos"> 307</span></a><span class="sd">			: whether to accept signed values. If False, it implies that `allow_negative` is False also.</span>
+</span><span id="TypeParser-308"><a href="#TypeParser-308"><span class="linenos"> 308</span></a>
+</span><span id="TypeParser-309"><a href="#TypeParser-309"><span class="linenos"> 309</span></a><span class="sd">			`allow_scientific`</span>
+</span><span id="TypeParser-310"><a href="#TypeParser-310"><span class="linenos"> 310</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form &lt;code&gt;&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;&lt;/code&gt; will be interpreted as the expression &lt;code&gt;&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)&lt;/code&gt;, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note &lt;var&gt;M&lt;/var&gt; *must* be an integer and &lt;var&gt;X&lt;/var&gt; *must* be a non-negative integer, even in cases where the above expression evaluates mathematically to an integer.</span>
+</span><span id="TypeParser-311"><a href="#TypeParser-311"><span class="linenos"> 311</span></a>
+</span><span id="TypeParser-312"><a href="#TypeParser-312"><span class="linenos"> 312</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser-313"><a href="#TypeParser-313"><span class="linenos"> 313</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser-314"><a href="#TypeParser-314"><span class="linenos"> 314</span></a><span class="sd">			whether it is an int</span>
+</span><span id="TypeParser-315"><a href="#TypeParser-315"><span class="linenos"> 315</span></a>
+</span><span id="TypeParser-316"><a href="#TypeParser-316"><span class="linenos"> 316</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser-317"><a href="#TypeParser-317"><span class="linenos"> 317</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser-318"><a href="#TypeParser-318"><span class="linenos"> 318</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser-319"><a href="#TypeParser-319"><span class="linenos"> 319</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser-320"><a href="#TypeParser-320"><span class="linenos"> 320</span></a><span class="sd">			parser.is_int(&quot;0&quot;)    # True</span>
+</span><span id="TypeParser-321"><a href="#TypeParser-321"><span class="linenos"> 321</span></a><span class="sd">			parser.is_int(&quot;-1&quot;)   # True</span>
+</span><span id="TypeParser-322"><a href="#TypeParser-322"><span class="linenos"> 322</span></a><span class="sd">			parser.is_int(&quot;abc&quot;)  # False</span>
+</span><span id="TypeParser-323"><a href="#TypeParser-323"><span class="linenos"> 323</span></a><span class="sd">			parser.is_int(&quot;&quot;)     # False</span>
+</span><span id="TypeParser-324"><a href="#TypeParser-324"><span class="linenos"> 324</span></a><span class="sd">			```</span>
+</span><span id="TypeParser-325"><a href="#TypeParser-325"><span class="linenos"> 325</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser-326"><a href="#TypeParser-326"><span class="linenos"> 326</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">trim</span><span class="p">:</span>
+</span><span id="TypeParser-327"><a href="#TypeParser-327"><span class="linenos"> 327</span></a>			<span class="n">value</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
+</span><span id="TypeParser-328"><a href="#TypeParser-328"><span class="linenos"> 328</span></a>
+</span><span id="TypeParser-329"><a href="#TypeParser-329"><span class="linenos"> 329</span></a>		<span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="TypeParser-330"><a href="#TypeParser-330"><span class="linenos"> 330</span></a>			<span class="k">return</span> <span class="kc">False</span>
+</span><span id="TypeParser-331"><a href="#TypeParser-331"><span class="linenos"> 331</span></a>
+</span><span id="TypeParser-332"><a href="#TypeParser-332"><span class="linenos"> 332</span></a>		<span class="k">if</span> <span class="n">allow_scientific</span><span class="p">:</span>
+</span><span id="TypeParser-333"><a href="#TypeParser-333"><span class="linenos"> 333</span></a>			<span class="n">value</span><span class="p">,</span> <span class="n">exp</span> <span class="o">=</span> <span class="n">_decompose_string_pair</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_scientific_char</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">int_case_sensitive</span><span class="p">)</span>
+</span><span id="TypeParser-334"><a href="#TypeParser-334"><span class="linenos"> 334</span></a>			<span class="k">if</span> <span class="n">exp</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="TypeParser-335"><a href="#TypeParser-335"><span class="linenos"> 335</span></a>				<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_int</span><span class="p">(</span>
+</span><span id="TypeParser-336"><a href="#TypeParser-336"><span class="linenos"> 336</span></a>					<span class="n">value</span><span class="p">,</span> <span class="n">allow_sign</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_negative</span><span class="o">=</span><span class="n">allow_negative</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="o">=</span><span class="kc">False</span>
+</span><span id="TypeParser-337"><a href="#TypeParser-337"><span class="linenos"> 337</span></a>				<span class="p">)</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_int</span><span class="p">(</span>
+</span><span id="TypeParser-338"><a href="#TypeParser-338"><span class="linenos"> 338</span></a>					<span class="n">exp</span><span class="p">,</span> <span class="n">allow_sign</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_negative</span><span class="o">=</span><span class="kc">False</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="o">=</span><span class="kc">False</span>
+</span><span id="TypeParser-339"><a href="#TypeParser-339"><span class="linenos"> 339</span></a>				<span class="p">)</span>
+</span><span id="TypeParser-340"><a href="#TypeParser-340"><span class="linenos"> 340</span></a>
+</span><span id="TypeParser-341"><a href="#TypeParser-341"><span class="linenos"> 341</span></a>		<span class="k">if</span> <span class="n">value</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_sign_chars</span><span class="p">:</span>
+</span><span id="TypeParser-342"><a href="#TypeParser-342"><span class="linenos"> 342</span></a>			<span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="TypeParser-343"><a href="#TypeParser-343"><span class="linenos"> 343</span></a>				<span class="k">return</span> <span class="kc">False</span>
+</span><span id="TypeParser-344"><a href="#TypeParser-344"><span class="linenos"> 344</span></a>			<span class="k">if</span> <span class="ow">not</span> <span class="n">allow_sign</span><span class="p">:</span>
+</span><span id="TypeParser-345"><a href="#TypeParser-345"><span class="linenos"> 345</span></a>				<span class="k">return</span> <span class="kc">False</span>
+</span><span id="TypeParser-346"><a href="#TypeParser-346"><span class="linenos"> 346</span></a>			<span class="k">if</span> <span class="ow">not</span> <span class="n">allow_negative</span> <span class="ow">and</span> <span class="n">value</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_negative_chars</span><span class="p">:</span>
+</span><span id="TypeParser-347"><a href="#TypeParser-347"><span class="linenos"> 347</span></a>				<span class="k">return</span> <span class="kc">False</span>
+</span><span id="TypeParser-348"><a href="#TypeParser-348"><span class="linenos"> 348</span></a>			<span class="n">value</span> <span class="o">=</span> <span class="n">value</span><span class="p">[</span><span class="mi">1</span><span class="p">:]</span>
+</span><span id="TypeParser-349"><a href="#TypeParser-349"><span class="linenos"> 349</span></a>		<span class="k">if</span> <span class="n">value</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_digit_separators</span> <span class="ow">or</span> <span class="n">value</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_digit_separators</span><span class="p">:</span>
+</span><span id="TypeParser-350"><a href="#TypeParser-350"><span class="linenos"> 350</span></a>			<span class="k">return</span> <span class="kc">False</span>
+</span><span id="TypeParser-351"><a href="#TypeParser-351"><span class="linenos"> 351</span></a>
+</span><span id="TypeParser-352"><a href="#TypeParser-352"><span class="linenos"> 352</span></a>		<span class="n">prev_separated</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="TypeParser-353"><a href="#TypeParser-353"><span class="linenos"> 353</span></a>		<span class="k">for</span> <span class="n">c</span> <span class="ow">in</span> <span class="n">value</span><span class="p">:</span>
+</span><span id="TypeParser-354"><a href="#TypeParser-354"><span class="linenos"> 354</span></a>			<span class="k">if</span> <span class="n">c</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_digit_separators</span><span class="p">:</span>
+</span><span id="TypeParser-355"><a href="#TypeParser-355"><span class="linenos"> 355</span></a>				<span class="k">if</span> <span class="n">prev_separated</span><span class="p">:</span>
+</span><span id="TypeParser-356"><a href="#TypeParser-356"><span class="linenos"> 356</span></a>					<span class="k">return</span> <span class="kc">False</span>
+</span><span id="TypeParser-357"><a href="#TypeParser-357"><span class="linenos"> 357</span></a>				<span class="n">prev_separated</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="TypeParser-358"><a href="#TypeParser-358"><span class="linenos"> 358</span></a>			<span class="k">else</span><span class="p">:</span>
+</span><span id="TypeParser-359"><a href="#TypeParser-359"><span class="linenos"> 359</span></a>				<span class="n">prev_separated</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="TypeParser-360"><a href="#TypeParser-360"><span class="linenos"> 360</span></a>				<span class="k">if</span> <span class="n">c</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_digit_chars</span><span class="p">:</span>
+</span><span id="TypeParser-361"><a href="#TypeParser-361"><span class="linenos"> 361</span></a>					<span class="k">return</span> <span class="kc">False</span>
+</span><span id="TypeParser-362"><a href="#TypeParser-362"><span class="linenos"> 362</span></a>		<span class="k">return</span> <span class="kc">True</span>
+</span><span id="TypeParser-363"><a href="#TypeParser-363"><span class="linenos"> 363</span></a>
+</span><span id="TypeParser-364"><a href="#TypeParser-364"><span class="linenos"> 364</span></a>
+</span><span id="TypeParser-365"><a href="#TypeParser-365"><span class="linenos"> 365</span></a>	<span class="k">def</span> <span class="nf">is_float</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="o">*</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_inf</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_nan</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="TypeParser-366"><a href="#TypeParser-366"><span class="linenos"> 366</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser-367"><a href="#TypeParser-367"><span class="linenos"> 367</span></a><span class="sd">			Check if a string represents a float (or equivalently, a Decimal)</span>
+</span><span id="TypeParser-368"><a href="#TypeParser-368"><span class="linenos"> 368</span></a>
+</span><span id="TypeParser-369"><a href="#TypeParser-369"><span class="linenos"> 369</span></a><span class="sd">			This function will also return True if the string represents an int.</span>
+</span><span id="TypeParser-370"><a href="#TypeParser-370"><span class="linenos"> 370</span></a>
+</span><span id="TypeParser-371"><a href="#TypeParser-371"><span class="linenos"> 371</span></a><span class="sd">			Alias: `is_decimal()`</span>
+</span><span id="TypeParser-372"><a href="#TypeParser-372"><span class="linenos"> 372</span></a>
+</span><span id="TypeParser-373"><a href="#TypeParser-373"><span class="linenos"> 373</span></a><span class="sd">			Parameters</span>
+</span><span id="TypeParser-374"><a href="#TypeParser-374"><span class="linenos"> 374</span></a><span class="sd">			----------</span>
+</span><span id="TypeParser-375"><a href="#TypeParser-375"><span class="linenos"> 375</span></a><span class="sd">			`value`</span>
+</span><span id="TypeParser-376"><a href="#TypeParser-376"><span class="linenos"> 376</span></a><span class="sd">			: string to be checked</span>
+</span><span id="TypeParser-377"><a href="#TypeParser-377"><span class="linenos"> 377</span></a>
+</span><span id="TypeParser-378"><a href="#TypeParser-378"><span class="linenos"> 378</span></a><span class="sd">			`allow_scientific`</span>
+</span><span id="TypeParser-379"><a href="#TypeParser-379"><span class="linenos"> 379</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form &lt;code&gt;&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;&lt;/code&gt; will be interpreted as the expression &lt;code&gt;&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)&lt;/code&gt;, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note that &lt;var&gt;X&lt;/var&gt; must be an integer, but can be negative.</span>
+</span><span id="TypeParser-380"><a href="#TypeParser-380"><span class="linenos"> 380</span></a>
+</span><span id="TypeParser-381"><a href="#TypeParser-381"><span class="linenos"> 381</span></a><span class="sd">			`allow_inf`</span>
+</span><span id="TypeParser-382"><a href="#TypeParser-382"><span class="linenos"> 382</span></a><span class="sd">			: whether to accept positive and negative infinity values. If True, strings that match the values in `self.inf_values` (empty by default) are interpreted as infinity, or as negative infinity if prepended by a negative sign. The case sensitivity of this matching depends on `self.float_case_sensitive`, which is False by default.</span>
+</span><span id="TypeParser-383"><a href="#TypeParser-383"><span class="linenos"> 383</span></a>
+</span><span id="TypeParser-384"><a href="#TypeParser-384"><span class="linenos"> 384</span></a><span class="sd">			`allow_nan`</span>
+</span><span id="TypeParser-385"><a href="#TypeParser-385"><span class="linenos"> 385</span></a><span class="sd">			: whether to accept NaN (not a number) representations. If True, strings that match the values in `self.nan_values` (empty by default) are interpeted as NaN. The case sensitivity of this matching depends on `self.float_case_sensitive`, which is False by default.</span>
+</span><span id="TypeParser-386"><a href="#TypeParser-386"><span class="linenos"> 386</span></a>
+</span><span id="TypeParser-387"><a href="#TypeParser-387"><span class="linenos"> 387</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser-388"><a href="#TypeParser-388"><span class="linenos"> 388</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser-389"><a href="#TypeParser-389"><span class="linenos"> 389</span></a><span class="sd">			whether it is a float or Decimal</span>
+</span><span id="TypeParser-390"><a href="#TypeParser-390"><span class="linenos"> 390</span></a>
+</span><span id="TypeParser-391"><a href="#TypeParser-391"><span class="linenos"> 391</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser-392"><a href="#TypeParser-392"><span class="linenos"> 392</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser-393"><a href="#TypeParser-393"><span class="linenos"> 393</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser-394"><a href="#TypeParser-394"><span class="linenos"> 394</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser-395"><a href="#TypeParser-395"><span class="linenos"> 395</span></a><span class="sd">			parser.is_float(&quot;1.&quot;)       # True</span>
+</span><span id="TypeParser-396"><a href="#TypeParser-396"><span class="linenos"> 396</span></a><span class="sd">			parser.is_float(&quot;12.3e-2&quot;)  # True</span>
+</span><span id="TypeParser-397"><a href="#TypeParser-397"><span class="linenos"> 397</span></a><span class="sd">			parser.is_float(&quot;abc&quot;)      # False</span>
+</span><span id="TypeParser-398"><a href="#TypeParser-398"><span class="linenos"> 398</span></a><span class="sd">			parser.is_float(&quot;&quot;)         # False</span>
+</span><span id="TypeParser-399"><a href="#TypeParser-399"><span class="linenos"> 399</span></a><span class="sd">			```</span>
+</span><span id="TypeParser-400"><a href="#TypeParser-400"><span class="linenos"> 400</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser-401"><a href="#TypeParser-401"><span class="linenos"> 401</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">trim</span><span class="p">:</span>
+</span><span id="TypeParser-402"><a href="#TypeParser-402"><span class="linenos"> 402</span></a>			<span class="n">value</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
+</span><span id="TypeParser-403"><a href="#TypeParser-403"><span class="linenos"> 403</span></a>
+</span><span id="TypeParser-404"><a href="#TypeParser-404"><span class="linenos"> 404</span></a>		<span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="o">&gt;</span> <span class="mi">0</span> <span class="ow">and</span> <span class="n">value</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_sign_chars</span><span class="p">:</span>
+</span><span id="TypeParser-405"><a href="#TypeParser-405"><span class="linenos"> 405</span></a>			<span class="n">value</span> <span class="o">=</span> <span class="n">value</span><span class="p">[</span><span class="mi">1</span><span class="p">:]</span>
+</span><span id="TypeParser-406"><a href="#TypeParser-406"><span class="linenos"> 406</span></a>
+</span><span id="TypeParser-407"><a href="#TypeParser-407"><span class="linenos"> 407</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">float_case_sensitive</span><span class="p">:</span>
+</span><span id="TypeParser-408"><a href="#TypeParser-408"><span class="linenos"> 408</span></a>			<span class="n">special_value</span> <span class="o">=</span> <span class="n">value</span>
+</span><span id="TypeParser-409"><a href="#TypeParser-409"><span class="linenos"> 409</span></a>		<span class="k">else</span><span class="p">:</span>
+</span><span id="TypeParser-410"><a href="#TypeParser-410"><span class="linenos"> 410</span></a>			<span class="n">special_value</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span>
+</span><span id="TypeParser-411"><a href="#TypeParser-411"><span class="linenos"> 411</span></a>		<span class="k">if</span> <span class="n">allow_inf</span> <span class="ow">and</span> <span class="n">special_value</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">inf_values</span><span class="p">:</span>
+</span><span id="TypeParser-412"><a href="#TypeParser-412"><span class="linenos"> 412</span></a>			<span class="k">return</span> <span class="kc">True</span>
+</span><span id="TypeParser-413"><a href="#TypeParser-413"><span class="linenos"> 413</span></a>		<span class="k">if</span> <span class="n">allow_nan</span> <span class="ow">and</span> <span class="n">special_value</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">nan_values</span><span class="p">:</span>
+</span><span id="TypeParser-414"><a href="#TypeParser-414"><span class="linenos"> 414</span></a>			<span class="k">return</span> <span class="kc">True</span>
+</span><span id="TypeParser-415"><a href="#TypeParser-415"><span class="linenos"> 415</span></a>
+</span><span id="TypeParser-416"><a href="#TypeParser-416"><span class="linenos"> 416</span></a>		<span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="TypeParser-417"><a href="#TypeParser-417"><span class="linenos"> 417</span></a>			<span class="k">return</span> <span class="kc">False</span>
+</span><span id="TypeParser-418"><a href="#TypeParser-418"><span class="linenos"> 418</span></a>
+</span><span id="TypeParser-419"><a href="#TypeParser-419"><span class="linenos"> 419</span></a>		<span class="k">if</span> <span class="n">allow_scientific</span><span class="p">:</span>
+</span><span id="TypeParser-420"><a href="#TypeParser-420"><span class="linenos"> 420</span></a>			<span class="n">value</span><span class="p">,</span> <span class="n">exp</span> <span class="o">=</span> <span class="n">_decompose_string_pair</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_scientific_char</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">float_case_sensitive</span><span class="p">)</span>
+</span><span id="TypeParser-421"><a href="#TypeParser-421"><span class="linenos"> 421</span></a>			<span class="k">if</span> <span class="n">exp</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="TypeParser-422"><a href="#TypeParser-422"><span class="linenos"> 422</span></a>				<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_float</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="o">=</span><span class="kc">False</span><span class="p">,</span> <span class="n">allow_inf</span><span class="o">=</span><span class="kc">False</span><span class="p">,</span> <span class="n">allow_nan</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_int</span><span class="p">(</span><span class="n">exp</span><span class="p">,</span> <span class="n">allow_sign</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_negative</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
+</span><span id="TypeParser-423"><a href="#TypeParser-423"><span class="linenos"> 423</span></a>
+</span><span id="TypeParser-424"><a href="#TypeParser-424"><span class="linenos"> 424</span></a>		<span class="n">value</span><span class="p">,</span> <span class="n">frac</span> <span class="o">=</span> <span class="n">_decompose_string_pair</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_float_separator</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">float_case_sensitive</span><span class="p">)</span>
+</span><span id="TypeParser-425"><a href="#TypeParser-425"><span class="linenos"> 425</span></a>		<span class="k">if</span> <span class="n">frac</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="TypeParser-426"><a href="#TypeParser-426"><span class="linenos"> 426</span></a>			<span class="k">if</span> <span class="n">value</span> <span class="o">==</span> <span class="s2">&quot;&quot;</span> <span class="ow">and</span> <span class="n">frac</span> <span class="o">==</span> <span class="s2">&quot;&quot;</span><span class="p">:</span>
+</span><span id="TypeParser-427"><a href="#TypeParser-427"><span class="linenos"> 427</span></a>				<span class="k">return</span> <span class="kc">False</span>
+</span><span id="TypeParser-428"><a href="#TypeParser-428"><span class="linenos"> 428</span></a>			<span class="k">return</span> <span class="p">(</span>
+</span><span id="TypeParser-429"><a href="#TypeParser-429"><span class="linenos"> 429</span></a>				<span class="bp">self</span><span class="o">.</span><span class="n">is_int</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">allow_sign</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_negative</span><span class="o">=</span><span class="kc">False</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span> <span class="ow">or</span> <span class="n">value</span> <span class="o">==</span> <span class="s2">&quot;&quot;</span>
+</span><span id="TypeParser-430"><a href="#TypeParser-430"><span class="linenos"> 430</span></a>			<span class="p">)</span> <span class="ow">and</span> <span class="p">(</span>
+</span><span id="TypeParser-431"><a href="#TypeParser-431"><span class="linenos"> 431</span></a>				<span class="bp">self</span><span class="o">.</span><span class="n">is_int</span><span class="p">(</span><span class="n">frac</span><span class="p">,</span> <span class="n">allow_sign</span><span class="o">=</span><span class="kc">False</span><span class="p">,</span> <span class="n">allow_negative</span><span class="o">=</span><span class="kc">False</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span> <span class="ow">or</span> <span class="n">frac</span> <span class="o">==</span> <span class="s2">&quot;&quot;</span>
+</span><span id="TypeParser-432"><a href="#TypeParser-432"><span class="linenos"> 432</span></a>			<span class="p">)</span>
+</span><span id="TypeParser-433"><a href="#TypeParser-433"><span class="linenos"> 433</span></a>
+</span><span id="TypeParser-434"><a href="#TypeParser-434"><span class="linenos"> 434</span></a>		<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_int</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">allow_sign</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_negative</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
+</span><span id="TypeParser-435"><a href="#TypeParser-435"><span class="linenos"> 435</span></a>
+</span><span id="TypeParser-436"><a href="#TypeParser-436"><span class="linenos"> 436</span></a>
+</span><span id="TypeParser-437"><a href="#TypeParser-437"><span class="linenos"> 437</span></a>	<span class="k">def</span> <span class="nf">is_decimal</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="o">*</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_inf</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_nan</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="TypeParser-438"><a href="#TypeParser-438"><span class="linenos"> 438</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser-439"><a href="#TypeParser-439"><span class="linenos"> 439</span></a><span class="sd">			Alias of `is_float()`</span>
+</span><span id="TypeParser-440"><a href="#TypeParser-440"><span class="linenos"> 440</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser-441"><a href="#TypeParser-441"><span class="linenos"> 441</span></a>		<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_float</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="o">=</span><span class="n">allow_scientific</span><span class="p">,</span> <span class="n">allow_inf</span><span class="o">=</span><span class="n">allow_inf</span><span class="p">,</span> <span class="n">allow_nan</span><span class="o">=</span><span class="n">allow_nan</span><span class="p">)</span>
+</span><span id="TypeParser-442"><a href="#TypeParser-442"><span class="linenos"> 442</span></a>
+</span><span id="TypeParser-443"><a href="#TypeParser-443"><span class="linenos"> 443</span></a>
+</span><span id="TypeParser-444"><a href="#TypeParser-444"><span class="linenos"> 444</span></a>	<span class="k">def</span> <span class="nf">parse_none</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="TypeParser-445"><a href="#TypeParser-445"><span class="linenos"> 445</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser-446"><a href="#TypeParser-446"><span class="linenos"> 446</span></a><span class="sd">			Parse a string and return it as the value None if possible</span>
+</span><span id="TypeParser-447"><a href="#TypeParser-447"><span class="linenos"> 447</span></a>
+</span><span id="TypeParser-448"><a href="#TypeParser-448"><span class="linenos"> 448</span></a><span class="sd">			Only strings that match the values in `self.none_values` will be interpreted as None. The default accepted values are `[&quot;&quot;]`, i.e. an empty string. The case sensitivity of this matching depends on `self.none_case_sensitive`, which is False by default.</span>
+</span><span id="TypeParser-449"><a href="#TypeParser-449"><span class="linenos"> 449</span></a>
+</span><span id="TypeParser-450"><a href="#TypeParser-450"><span class="linenos"> 450</span></a><span class="sd">			Parameters</span>
+</span><span id="TypeParser-451"><a href="#TypeParser-451"><span class="linenos"> 451</span></a><span class="sd">			----------</span>
+</span><span id="TypeParser-452"><a href="#TypeParser-452"><span class="linenos"> 452</span></a><span class="sd">			`value`</span>
+</span><span id="TypeParser-453"><a href="#TypeParser-453"><span class="linenos"> 453</span></a><span class="sd">			: string to be parsed</span>
+</span><span id="TypeParser-454"><a href="#TypeParser-454"><span class="linenos"> 454</span></a>
+</span><span id="TypeParser-455"><a href="#TypeParser-455"><span class="linenos"> 455</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser-456"><a href="#TypeParser-456"><span class="linenos"> 456</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser-457"><a href="#TypeParser-457"><span class="linenos"> 457</span></a><span class="sd">			parsed None value</span>
+</span><span id="TypeParser-458"><a href="#TypeParser-458"><span class="linenos"> 458</span></a>
+</span><span id="TypeParser-459"><a href="#TypeParser-459"><span class="linenos"> 459</span></a><span class="sd">			Raises</span>
+</span><span id="TypeParser-460"><a href="#TypeParser-460"><span class="linenos"> 460</span></a><span class="sd">			------</span>
+</span><span id="TypeParser-461"><a href="#TypeParser-461"><span class="linenos"> 461</span></a><span class="sd">			`ValueError` if `value` cannot be parsed</span>
+</span><span id="TypeParser-462"><a href="#TypeParser-462"><span class="linenos"> 462</span></a>
+</span><span id="TypeParser-463"><a href="#TypeParser-463"><span class="linenos"> 463</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser-464"><a href="#TypeParser-464"><span class="linenos"> 464</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser-465"><a href="#TypeParser-465"><span class="linenos"> 465</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser-466"><a href="#TypeParser-466"><span class="linenos"> 466</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser-467"><a href="#TypeParser-467"><span class="linenos"> 467</span></a><span class="sd">			parser.parse_bool(&quot;&quot;)     # None</span>
+</span><span id="TypeParser-468"><a href="#TypeParser-468"><span class="linenos"> 468</span></a><span class="sd">			parser.parse_bool(&quot;abc&quot;)  # raises ValueError</span>
+</span><span id="TypeParser-469"><a href="#TypeParser-469"><span class="linenos"> 469</span></a><span class="sd">			```</span>
+</span><span id="TypeParser-470"><a href="#TypeParser-470"><span class="linenos"> 470</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser-471"><a href="#TypeParser-471"><span class="linenos"> 471</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_none</span><span class="p">(</span><span class="n">value</span><span class="p">):</span>
+</span><span id="TypeParser-472"><a href="#TypeParser-472"><span class="linenos"> 472</span></a>			<span class="k">return</span> <span class="kc">None</span>
+</span><span id="TypeParser-473"><a href="#TypeParser-473"><span class="linenos"> 473</span></a>		<span class="k">else</span><span class="p">:</span>
+</span><span id="TypeParser-474"><a href="#TypeParser-474"><span class="linenos"> 474</span></a>			<span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;not a none value: </span><span class="si">{</span><span class="n">value</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="TypeParser-475"><a href="#TypeParser-475"><span class="linenos"> 475</span></a>
+</span><span id="TypeParser-476"><a href="#TypeParser-476"><span class="linenos"> 476</span></a>
+</span><span id="TypeParser-477"><a href="#TypeParser-477"><span class="linenos"> 477</span></a>	<span class="k">def</span> <span class="nf">parse_bool</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="TypeParser-478"><a href="#TypeParser-478"><span class="linenos"> 478</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser-479"><a href="#TypeParser-479"><span class="linenos"> 479</span></a><span class="sd">			Parse a string and return it as a bool if possible</span>
+</span><span id="TypeParser-480"><a href="#TypeParser-480"><span class="linenos"> 480</span></a>
+</span><span id="TypeParser-481"><a href="#TypeParser-481"><span class="linenos"> 481</span></a><span class="sd">			Only strings that match the values in `self.true_values` and `self.false_values` will be interpreted as booleans. The default accepted values are `[&quot;true&quot;]` and `[&quot;false&quot;]` respectively. The case sensitivity of this matching depends on `self.bool_case_sensitive`, which is False by default.</span>
+</span><span id="TypeParser-482"><a href="#TypeParser-482"><span class="linenos"> 482</span></a>
+</span><span id="TypeParser-483"><a href="#TypeParser-483"><span class="linenos"> 483</span></a><span class="sd">			Parameters</span>
+</span><span id="TypeParser-484"><a href="#TypeParser-484"><span class="linenos"> 484</span></a><span class="sd">			----------</span>
+</span><span id="TypeParser-485"><a href="#TypeParser-485"><span class="linenos"> 485</span></a><span class="sd">			`value`</span>
+</span><span id="TypeParser-486"><a href="#TypeParser-486"><span class="linenos"> 486</span></a><span class="sd">			: string to be parsed</span>
+</span><span id="TypeParser-487"><a href="#TypeParser-487"><span class="linenos"> 487</span></a>
+</span><span id="TypeParser-488"><a href="#TypeParser-488"><span class="linenos"> 488</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser-489"><a href="#TypeParser-489"><span class="linenos"> 489</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser-490"><a href="#TypeParser-490"><span class="linenos"> 490</span></a><span class="sd">			parsed bool value</span>
+</span><span id="TypeParser-491"><a href="#TypeParser-491"><span class="linenos"> 491</span></a>
+</span><span id="TypeParser-492"><a href="#TypeParser-492"><span class="linenos"> 492</span></a><span class="sd">			Raises</span>
+</span><span id="TypeParser-493"><a href="#TypeParser-493"><span class="linenos"> 493</span></a><span class="sd">			------</span>
+</span><span id="TypeParser-494"><a href="#TypeParser-494"><span class="linenos"> 494</span></a><span class="sd">			`ValueError` if `value` cannot be parsed</span>
+</span><span id="TypeParser-495"><a href="#TypeParser-495"><span class="linenos"> 495</span></a>
+</span><span id="TypeParser-496"><a href="#TypeParser-496"><span class="linenos"> 496</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser-497"><a href="#TypeParser-497"><span class="linenos"> 497</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser-498"><a href="#TypeParser-498"><span class="linenos"> 498</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser-499"><a href="#TypeParser-499"><span class="linenos"> 499</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser-500"><a href="#TypeParser-500"><span class="linenos"> 500</span></a><span class="sd">			parser.parse_bool(&quot;true&quot;)   # True</span>
+</span><span id="TypeParser-501"><a href="#TypeParser-501"><span class="linenos"> 501</span></a><span class="sd">			parser.parse_bool(&quot;FALSE&quot;)  # False</span>
+</span><span id="TypeParser-502"><a href="#TypeParser-502"><span class="linenos"> 502</span></a><span class="sd">			```</span>
+</span><span id="TypeParser-503"><a href="#TypeParser-503"><span class="linenos"> 503</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser-504"><a href="#TypeParser-504"><span class="linenos"> 504</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">trim</span><span class="p">:</span>
+</span><span id="TypeParser-505"><a href="#TypeParser-505"><span class="linenos"> 505</span></a>			<span class="n">value</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
+</span><span id="TypeParser-506"><a href="#TypeParser-506"><span class="linenos"> 506</span></a>
+</span><span id="TypeParser-507"><a href="#TypeParser-507"><span class="linenos"> 507</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">bool_case_sensitive</span><span class="p">:</span>
+</span><span id="TypeParser-508"><a href="#TypeParser-508"><span class="linenos"> 508</span></a>			<span class="n">special_value</span> <span class="o">=</span> <span class="n">value</span>
+</span><span id="TypeParser-509"><a href="#TypeParser-509"><span class="linenos"> 509</span></a>		<span class="k">else</span><span class="p">:</span>
+</span><span id="TypeParser-510"><a href="#TypeParser-510"><span class="linenos"> 510</span></a>			<span class="n">special_value</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span>
+</span><span id="TypeParser-511"><a href="#TypeParser-511"><span class="linenos"> 511</span></a>		<span class="k">if</span> <span class="n">special_value</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">true_values</span><span class="p">:</span>
+</span><span id="TypeParser-512"><a href="#TypeParser-512"><span class="linenos"> 512</span></a>			<span class="k">return</span> <span class="kc">True</span>
+</span><span id="TypeParser-513"><a href="#TypeParser-513"><span class="linenos"> 513</span></a>		<span class="k">if</span> <span class="n">special_value</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">false_values</span><span class="p">:</span>
+</span><span id="TypeParser-514"><a href="#TypeParser-514"><span class="linenos"> 514</span></a>			<span class="k">return</span> <span class="kc">False</span>
+</span><span id="TypeParser-515"><a href="#TypeParser-515"><span class="linenos"> 515</span></a>
+</span><span id="TypeParser-516"><a href="#TypeParser-516"><span class="linenos"> 516</span></a>		<span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;not a boolean: </span><span class="si">{</span><span class="n">value</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="TypeParser-517"><a href="#TypeParser-517"><span class="linenos"> 517</span></a>
+</span><span id="TypeParser-518"><a href="#TypeParser-518"><span class="linenos"> 518</span></a>
+</span><span id="TypeParser-519"><a href="#TypeParser-519"><span class="linenos"> 519</span></a>	<span class="k">def</span> <span class="nf">parse_int</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="o">*</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="TypeParser-520"><a href="#TypeParser-520"><span class="linenos"> 520</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser-521"><a href="#TypeParser-521"><span class="linenos"> 521</span></a><span class="sd">			Parse a string and return it as an int if possible</span>
+</span><span id="TypeParser-522"><a href="#TypeParser-522"><span class="linenos"> 522</span></a>
+</span><span id="TypeParser-523"><a href="#TypeParser-523"><span class="linenos"> 523</span></a><span class="sd">			If the string represents a bool, it will be converted to `1` for True and `0` for False.</span>
+</span><span id="TypeParser-524"><a href="#TypeParser-524"><span class="linenos"> 524</span></a>
+</span><span id="TypeParser-525"><a href="#TypeParser-525"><span class="linenos"> 525</span></a><span class="sd">			Parameters</span>
+</span><span id="TypeParser-526"><a href="#TypeParser-526"><span class="linenos"> 526</span></a><span class="sd">			----------</span>
+</span><span id="TypeParser-527"><a href="#TypeParser-527"><span class="linenos"> 527</span></a><span class="sd">			`value`</span>
+</span><span id="TypeParser-528"><a href="#TypeParser-528"><span class="linenos"> 528</span></a><span class="sd">			: string to be parsed</span>
+</span><span id="TypeParser-529"><a href="#TypeParser-529"><span class="linenos"> 529</span></a>
+</span><span id="TypeParser-530"><a href="#TypeParser-530"><span class="linenos"> 530</span></a><span class="sd">			`allow_scientific`</span>
+</span><span id="TypeParser-531"><a href="#TypeParser-531"><span class="linenos"> 531</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form &lt;code&gt;&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;&lt;/code&gt; will be interpreted as the expression &lt;code&gt;&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)&lt;/code&gt;, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note &lt;var&gt;M&lt;/var&gt; *must* be an integer and &lt;var&gt;X&lt;/var&gt; *must* be a non-negative integer, even in cases where the above expression evaluates mathematically to an integer.</span>
+</span><span id="TypeParser-532"><a href="#TypeParser-532"><span class="linenos"> 532</span></a>
+</span><span id="TypeParser-533"><a href="#TypeParser-533"><span class="linenos"> 533</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser-534"><a href="#TypeParser-534"><span class="linenos"> 534</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser-535"><a href="#TypeParser-535"><span class="linenos"> 535</span></a><span class="sd">			parsed int value</span>
+</span><span id="TypeParser-536"><a href="#TypeParser-536"><span class="linenos"> 536</span></a>
+</span><span id="TypeParser-537"><a href="#TypeParser-537"><span class="linenos"> 537</span></a><span class="sd">			Raises</span>
+</span><span id="TypeParser-538"><a href="#TypeParser-538"><span class="linenos"> 538</span></a><span class="sd">			------</span>
+</span><span id="TypeParser-539"><a href="#TypeParser-539"><span class="linenos"> 539</span></a><span class="sd">			`ValueError` if `value` cannot be parsed</span>
+</span><span id="TypeParser-540"><a href="#TypeParser-540"><span class="linenos"> 540</span></a>
+</span><span id="TypeParser-541"><a href="#TypeParser-541"><span class="linenos"> 541</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser-542"><a href="#TypeParser-542"><span class="linenos"> 542</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser-543"><a href="#TypeParser-543"><span class="linenos"> 543</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser-544"><a href="#TypeParser-544"><span class="linenos"> 544</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser-545"><a href="#TypeParser-545"><span class="linenos"> 545</span></a><span class="sd">			parser.parse_int(&quot;0&quot;)    # 0</span>
+</span><span id="TypeParser-546"><a href="#TypeParser-546"><span class="linenos"> 546</span></a><span class="sd">			parser.parse_int(&quot;-1&quot;)   # -1</span>
+</span><span id="TypeParser-547"><a href="#TypeParser-547"><span class="linenos"> 547</span></a><span class="sd">			parser.parse_int(&quot;2e3&quot;)  # 2000</span>
+</span><span id="TypeParser-548"><a href="#TypeParser-548"><span class="linenos"> 548</span></a><span class="sd">			```</span>
+</span><span id="TypeParser-549"><a href="#TypeParser-549"><span class="linenos"> 549</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser-550"><a href="#TypeParser-550"><span class="linenos"> 550</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">trim</span><span class="p">:</span>
+</span><span id="TypeParser-551"><a href="#TypeParser-551"><span class="linenos"> 551</span></a>			<span class="n">value</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
+</span><span id="TypeParser-552"><a href="#TypeParser-552"><span class="linenos"> 552</span></a>
+</span><span id="TypeParser-553"><a href="#TypeParser-553"><span class="linenos"> 553</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_int</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">allow_sign</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_negative</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="o">=</span><span class="n">allow_scientific</span><span class="p">):</span>
+</span><span id="TypeParser-554"><a href="#TypeParser-554"><span class="linenos"> 554</span></a>			<span class="k">if</span> <span class="n">allow_scientific</span><span class="p">:</span>
+</span><span id="TypeParser-555"><a href="#TypeParser-555"><span class="linenos"> 555</span></a>				<span class="n">value</span><span class="p">,</span> <span class="n">exp</span> <span class="o">=</span> <span class="n">_decompose_string_pair</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_scientific_char</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">int_case_sensitive</span><span class="p">)</span>
+</span><span id="TypeParser-556"><a href="#TypeParser-556"><span class="linenos"> 556</span></a>				<span class="k">if</span> <span class="n">exp</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="TypeParser-557"><a href="#TypeParser-557"><span class="linenos"> 557</span></a>					<span class="k">if</span> <span class="n">value</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="ow">in</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_negative_chars</span> <span class="o">-</span> <span class="p">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_negative_char</span><span class="p">}):</span>
+</span><span id="TypeParser-558"><a href="#TypeParser-558"><span class="linenos"> 558</span></a>						<span class="n">value</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_negative_char</span> <span class="o">+</span> <span class="n">value</span><span class="p">[</span><span class="mi">1</span><span class="p">:]</span>
+</span><span id="TypeParser-559"><a href="#TypeParser-559"><span class="linenos"> 559</span></a>					<span class="k">return</span> <span class="nb">int</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="o">*</span> <span class="p">(</span><span class="mi">10</span> <span class="o">**</span> <span class="nb">int</span><span class="p">(</span><span class="n">exp</span><span class="p">))</span>
+</span><span id="TypeParser-560"><a href="#TypeParser-560"><span class="linenos"> 560</span></a>
+</span><span id="TypeParser-561"><a href="#TypeParser-561"><span class="linenos"> 561</span></a>			<span class="k">if</span> <span class="n">value</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="ow">in</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_negative_chars</span> <span class="o">-</span> <span class="p">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_negative_char</span><span class="p">}):</span>
+</span><span id="TypeParser-562"><a href="#TypeParser-562"><span class="linenos"> 562</span></a>				<span class="n">value</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_negative_char</span> <span class="o">+</span> <span class="n">value</span><span class="p">[</span><span class="mi">1</span><span class="p">:]</span>
+</span><span id="TypeParser-563"><a href="#TypeParser-563"><span class="linenos"> 563</span></a>			<span class="k">return</span> <span class="nb">int</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
+</span><span id="TypeParser-564"><a href="#TypeParser-564"><span class="linenos"> 564</span></a>
+</span><span id="TypeParser-565"><a href="#TypeParser-565"><span class="linenos"> 565</span></a>		<span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_bool</span><span class="p">(</span><span class="n">value</span><span class="p">):</span>
+</span><span id="TypeParser-566"><a href="#TypeParser-566"><span class="linenos"> 566</span></a>			<span class="k">return</span> <span class="nb">int</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">parse_bool</span><span class="p">(</span><span class="n">value</span><span class="p">))</span>
+</span><span id="TypeParser-567"><a href="#TypeParser-567"><span class="linenos"> 567</span></a>		<span class="k">else</span><span class="p">:</span>
+</span><span id="TypeParser-568"><a href="#TypeParser-568"><span class="linenos"> 568</span></a>			<span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;not an integer: </span><span class="si">{</span><span class="n">value</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="TypeParser-569"><a href="#TypeParser-569"><span class="linenos"> 569</span></a>
+</span><span id="TypeParser-570"><a href="#TypeParser-570"><span class="linenos"> 570</span></a>
+</span><span id="TypeParser-571"><a href="#TypeParser-571"><span class="linenos"> 571</span></a>	<span class="k">def</span> <span class="nf">_parse_floatlike</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span>
+</span><span id="TypeParser-572"><a href="#TypeParser-572"><span class="linenos"> 572</span></a>		<span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
+</span><span id="TypeParser-573"><a href="#TypeParser-573"><span class="linenos"> 573</span></a>		<span class="n">converter</span><span class="p">:</span> <span class="n">Callable</span><span class="p">[[</span><span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">bool</span><span class="p">]],</span> <span class="n">_FloatLike</span><span class="p">],</span>
+</span><span id="TypeParser-574"><a href="#TypeParser-574"><span class="linenos"> 574</span></a>		<span class="n">inf_value</span><span class="p">:</span> <span class="n">_FloatLike</span><span class="p">,</span>
+</span><span id="TypeParser-575"><a href="#TypeParser-575"><span class="linenos"> 575</span></a>		<span class="n">nan_value</span><span class="p">:</span> <span class="n">_FloatLike</span><span class="p">,</span>
+</span><span id="TypeParser-576"><a href="#TypeParser-576"><span class="linenos"> 576</span></a>		<span class="o">*</span><span class="p">,</span>
+</span><span id="TypeParser-577"><a href="#TypeParser-577"><span class="linenos"> 577</span></a>		<span class="n">allow_scientific</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
+</span><span id="TypeParser-578"><a href="#TypeParser-578"><span class="linenos"> 578</span></a>		<span class="n">allow_inf</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
+</span><span id="TypeParser-579"><a href="#TypeParser-579"><span class="linenos"> 579</span></a>		<span class="n">allow_nan</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span>
+</span><span id="TypeParser-580"><a href="#TypeParser-580"><span class="linenos"> 580</span></a>	<span class="p">)</span> <span class="o">-&gt;</span> <span class="n">_FloatLike</span><span class="p">:</span>
+</span><span id="TypeParser-581"><a href="#TypeParser-581"><span class="linenos"> 581</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">trim</span><span class="p">:</span>
+</span><span id="TypeParser-582"><a href="#TypeParser-582"><span class="linenos"> 582</span></a>			<span class="n">value</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
+</span><span id="TypeParser-583"><a href="#TypeParser-583"><span class="linenos"> 583</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_float</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="o">=</span><span class="n">allow_scientific</span><span class="p">,</span> <span class="n">allow_inf</span><span class="o">=</span><span class="n">allow_inf</span><span class="p">,</span> <span class="n">allow_nan</span><span class="o">=</span><span class="n">allow_nan</span><span class="p">):</span>
+</span><span id="TypeParser-584"><a href="#TypeParser-584"><span class="linenos"> 584</span></a>			<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">float_case_sensitive</span><span class="p">:</span>
+</span><span id="TypeParser-585"><a href="#TypeParser-585"><span class="linenos"> 585</span></a>				<span class="n">special_value</span> <span class="o">=</span> <span class="n">value</span>
+</span><span id="TypeParser-586"><a href="#TypeParser-586"><span class="linenos"> 586</span></a>			<span class="k">else</span><span class="p">:</span>
+</span><span id="TypeParser-587"><a href="#TypeParser-587"><span class="linenos"> 587</span></a>				<span class="n">special_value</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span>
+</span><span id="TypeParser-588"><a href="#TypeParser-588"><span class="linenos"> 588</span></a>			<span class="k">if</span> <span class="n">allow_inf</span> <span class="ow">and</span> <span class="n">special_value</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">inf_values</span><span class="p">:</span>
+</span><span id="TypeParser-589"><a href="#TypeParser-589"><span class="linenos"> 589</span></a>				<span class="k">return</span> <span class="n">inf_value</span>
+</span><span id="TypeParser-590"><a href="#TypeParser-590"><span class="linenos"> 590</span></a>			<span class="k">if</span> <span class="n">allow_nan</span> <span class="ow">and</span> <span class="n">special_value</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">nan_values</span><span class="p">:</span>
+</span><span id="TypeParser-591"><a href="#TypeParser-591"><span class="linenos"> 591</span></a>				<span class="k">return</span> <span class="n">nan_value</span>
+</span><span id="TypeParser-592"><a href="#TypeParser-592"><span class="linenos"> 592</span></a>
+</span><span id="TypeParser-593"><a href="#TypeParser-593"><span class="linenos"> 593</span></a>			<span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="o">&gt;</span> <span class="mi">0</span> <span class="ow">and</span> <span class="n">value</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_sign_chars</span><span class="p">:</span>
+</span><span id="TypeParser-594"><a href="#TypeParser-594"><span class="linenos"> 594</span></a>				<span class="n">positive_part</span> <span class="o">=</span> <span class="n">value</span><span class="p">[</span><span class="mi">1</span><span class="p">:]</span>
+</span><span id="TypeParser-595"><a href="#TypeParser-595"><span class="linenos"> 595</span></a>				<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">float_case_sensitive</span><span class="p">:</span>
+</span><span id="TypeParser-596"><a href="#TypeParser-596"><span class="linenos"> 596</span></a>					<span class="n">special_value</span> <span class="o">=</span> <span class="n">positive_part</span>
+</span><span id="TypeParser-597"><a href="#TypeParser-597"><span class="linenos"> 597</span></a>				<span class="k">else</span><span class="p">:</span>
+</span><span id="TypeParser-598"><a href="#TypeParser-598"><span class="linenos"> 598</span></a>					<span class="n">special_value</span> <span class="o">=</span> <span class="n">positive_part</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span>
+</span><span id="TypeParser-599"><a href="#TypeParser-599"><span class="linenos"> 599</span></a>				<span class="k">if</span> <span class="n">allow_inf</span> <span class="ow">and</span> <span class="n">special_value</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">inf_values</span><span class="p">:</span>
+</span><span id="TypeParser-600"><a href="#TypeParser-600"><span class="linenos"> 600</span></a>					<span class="k">if</span> <span class="n">value</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_negative_chars</span><span class="p">:</span>
+</span><span id="TypeParser-601"><a href="#TypeParser-601"><span class="linenos"> 601</span></a>						<span class="k">return</span> <span class="o">-</span><span class="mi">1</span> <span class="o">*</span> <span class="n">inf_value</span>
+</span><span id="TypeParser-602"><a href="#TypeParser-602"><span class="linenos"> 602</span></a>					<span class="k">else</span><span class="p">:</span>
+</span><span id="TypeParser-603"><a href="#TypeParser-603"><span class="linenos"> 603</span></a>						<span class="k">return</span> <span class="n">inf_value</span>
+</span><span id="TypeParser-604"><a href="#TypeParser-604"><span class="linenos"> 604</span></a>				<span class="k">if</span> <span class="n">allow_nan</span> <span class="ow">and</span> <span class="n">special_value</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">nan_values</span><span class="p">:</span>
+</span><span id="TypeParser-605"><a href="#TypeParser-605"><span class="linenos"> 605</span></a>					<span class="k">return</span> <span class="n">nan_value</span>
+</span><span id="TypeParser-606"><a href="#TypeParser-606"><span class="linenos"> 606</span></a>
+</span><span id="TypeParser-607"><a href="#TypeParser-607"><span class="linenos"> 607</span></a>				<span class="k">if</span> <span class="n">value</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_negative_chars</span><span class="p">:</span>
+</span><span id="TypeParser-608"><a href="#TypeParser-608"><span class="linenos"> 608</span></a>					<span class="n">value</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_negative_char</span> <span class="o">+</span> <span class="n">positive_part</span>
+</span><span id="TypeParser-609"><a href="#TypeParser-609"><span class="linenos"> 609</span></a>			<span class="k">return</span> <span class="n">converter</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
+</span><span id="TypeParser-610"><a href="#TypeParser-610"><span class="linenos"> 610</span></a>		<span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_bool</span><span class="p">(</span><span class="n">value</span><span class="p">):</span>
+</span><span id="TypeParser-611"><a href="#TypeParser-611"><span class="linenos"> 611</span></a>			<span class="k">return</span> <span class="n">converter</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">parse_bool</span><span class="p">(</span><span class="n">value</span><span class="p">))</span>
+</span><span id="TypeParser-612"><a href="#TypeParser-612"><span class="linenos"> 612</span></a>		<span class="k">else</span><span class="p">:</span>
+</span><span id="TypeParser-613"><a href="#TypeParser-613"><span class="linenos"> 613</span></a>			<span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;not a </span><span class="si">{</span><span class="n">_FloatLike</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">value</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="TypeParser-614"><a href="#TypeParser-614"><span class="linenos"> 614</span></a>
+</span><span id="TypeParser-615"><a href="#TypeParser-615"><span class="linenos"> 615</span></a>
+</span><span id="TypeParser-616"><a href="#TypeParser-616"><span class="linenos"> 616</span></a>	<span class="k">def</span> <span class="nf">parse_float</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="o">*</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_inf</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_nan</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
+</span><span id="TypeParser-617"><a href="#TypeParser-617"><span class="linenos"> 617</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser-618"><a href="#TypeParser-618"><span class="linenos"> 618</span></a><span class="sd">			Parse a string and return it as a (non-exact) float if possible</span>
+</span><span id="TypeParser-619"><a href="#TypeParser-619"><span class="linenos"> 619</span></a>
+</span><span id="TypeParser-620"><a href="#TypeParser-620"><span class="linenos"> 620</span></a><span class="sd">			If the string represents a bool, it will be converted to `1.` for True and `0.` for False. If the string represents an int, it will be converted to a float also.</span>
+</span><span id="TypeParser-621"><a href="#TypeParser-621"><span class="linenos"> 621</span></a>
+</span><span id="TypeParser-622"><a href="#TypeParser-622"><span class="linenos"> 622</span></a><span class="sd">			Behaves analogously to `parse_decimal()`, except that that returns an exact Decimal instead.</span>
+</span><span id="TypeParser-623"><a href="#TypeParser-623"><span class="linenos"> 623</span></a>
+</span><span id="TypeParser-624"><a href="#TypeParser-624"><span class="linenos"> 624</span></a><span class="sd">			Parameters</span>
+</span><span id="TypeParser-625"><a href="#TypeParser-625"><span class="linenos"> 625</span></a><span class="sd">			----------</span>
+</span><span id="TypeParser-626"><a href="#TypeParser-626"><span class="linenos"> 626</span></a><span class="sd">			`value`</span>
+</span><span id="TypeParser-627"><a href="#TypeParser-627"><span class="linenos"> 627</span></a><span class="sd">			: string to be parsed</span>
+</span><span id="TypeParser-628"><a href="#TypeParser-628"><span class="linenos"> 628</span></a>
+</span><span id="TypeParser-629"><a href="#TypeParser-629"><span class="linenos"> 629</span></a><span class="sd">			`allow_scientific`</span>
+</span><span id="TypeParser-630"><a href="#TypeParser-630"><span class="linenos"> 630</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form &lt;code&gt;&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;&lt;/code&gt; will be interpreted as the expression &lt;code&gt;&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)&lt;/code&gt;, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note that &lt;var&gt;X&lt;/var&gt; must be an integer, but can be negative.</span>
+</span><span id="TypeParser-631"><a href="#TypeParser-631"><span class="linenos"> 631</span></a>
+</span><span id="TypeParser-632"><a href="#TypeParser-632"><span class="linenos"> 632</span></a><span class="sd">			`allow_inf`</span>
+</span><span id="TypeParser-633"><a href="#TypeParser-633"><span class="linenos"> 633</span></a><span class="sd">			: whether to accept positive and negative infinity values. If True, strings that match the values in `self.inf_values` (empty by default) are interpreted as infinity, or as negative infinity if prepended by a negative sign. The case sensitivity of this matching depends on `self.float_case_sensitive`, which is False by default.</span>
+</span><span id="TypeParser-634"><a href="#TypeParser-634"><span class="linenos"> 634</span></a>
+</span><span id="TypeParser-635"><a href="#TypeParser-635"><span class="linenos"> 635</span></a><span class="sd">			`allow_nan`</span>
+</span><span id="TypeParser-636"><a href="#TypeParser-636"><span class="linenos"> 636</span></a><span class="sd">			: whether to accept NaN (not a number) representations. If True, strings that match the values in `self.nan_values` (empty by default) are interpeted as NaN. The case sensitivity of this matching depends on `self.float_case_sensitive`, which is False by default.</span>
+</span><span id="TypeParser-637"><a href="#TypeParser-637"><span class="linenos"> 637</span></a>
+</span><span id="TypeParser-638"><a href="#TypeParser-638"><span class="linenos"> 638</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser-639"><a href="#TypeParser-639"><span class="linenos"> 639</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser-640"><a href="#TypeParser-640"><span class="linenos"> 640</span></a><span class="sd">			parsed float value</span>
+</span><span id="TypeParser-641"><a href="#TypeParser-641"><span class="linenos"> 641</span></a>
+</span><span id="TypeParser-642"><a href="#TypeParser-642"><span class="linenos"> 642</span></a><span class="sd">			Raises</span>
+</span><span id="TypeParser-643"><a href="#TypeParser-643"><span class="linenos"> 643</span></a><span class="sd">			------</span>
+</span><span id="TypeParser-644"><a href="#TypeParser-644"><span class="linenos"> 644</span></a><span class="sd">			`ValueError` if `value` cannot be parsed</span>
+</span><span id="TypeParser-645"><a href="#TypeParser-645"><span class="linenos"> 645</span></a>
+</span><span id="TypeParser-646"><a href="#TypeParser-646"><span class="linenos"> 646</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser-647"><a href="#TypeParser-647"><span class="linenos"> 647</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser-648"><a href="#TypeParser-648"><span class="linenos"> 648</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser-649"><a href="#TypeParser-649"><span class="linenos"> 649</span></a><span class="sd">			parser = TypeParser(inf_values=[&quot;inf&quot;], nan_values=[&quot;nan&quot;])</span>
+</span><span id="TypeParser-650"><a href="#TypeParser-650"><span class="linenos"> 650</span></a><span class="sd">			parser.parse_float(&quot;1.&quot;)       # 1.</span>
+</span><span id="TypeParser-651"><a href="#TypeParser-651"><span class="linenos"> 651</span></a><span class="sd">			parser.parse_float(&quot;1.23e2&quot;)   # 123.</span>
+</span><span id="TypeParser-652"><a href="#TypeParser-652"><span class="linenos"> 652</span></a><span class="sd">			parser.parse_float(&quot;1.23e-2&quot;)  # 0.0123</span>
+</span><span id="TypeParser-653"><a href="#TypeParser-653"><span class="linenos"> 653</span></a><span class="sd">			parser.parse_float(&quot;inf&quot;)      # math.inf</span>
+</span><span id="TypeParser-654"><a href="#TypeParser-654"><span class="linenos"> 654</span></a><span class="sd">			```</span>
+</span><span id="TypeParser-655"><a href="#TypeParser-655"><span class="linenos"> 655</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser-656"><a href="#TypeParser-656"><span class="linenos"> 656</span></a>		<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_parse_floatlike</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">math</span><span class="o">.</span><span class="n">inf</span><span class="p">,</span> <span class="n">math</span><span class="o">.</span><span class="n">nan</span><span class="p">,</span>
+</span><span id="TypeParser-657"><a href="#TypeParser-657"><span class="linenos"> 657</span></a>			<span class="n">allow_scientific</span><span class="o">=</span><span class="n">allow_scientific</span><span class="p">,</span>
+</span><span id="TypeParser-658"><a href="#TypeParser-658"><span class="linenos"> 658</span></a>			<span class="n">allow_inf</span><span class="o">=</span><span class="n">allow_inf</span><span class="p">,</span>
+</span><span id="TypeParser-659"><a href="#TypeParser-659"><span class="linenos"> 659</span></a>			<span class="n">allow_nan</span><span class="o">=</span><span class="n">allow_nan</span><span class="p">,</span>
+</span><span id="TypeParser-660"><a href="#TypeParser-660"><span class="linenos"> 660</span></a>		<span class="p">)</span>
+</span><span id="TypeParser-661"><a href="#TypeParser-661"><span class="linenos"> 661</span></a>
+</span><span id="TypeParser-662"><a href="#TypeParser-662"><span class="linenos"> 662</span></a>
+</span><span id="TypeParser-663"><a href="#TypeParser-663"><span class="linenos"> 663</span></a>	<span class="k">def</span> <span class="nf">parse_decimal</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="o">*</span><span class="p">,</span> <span class="n">allow_scientific</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_inf</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">allow_nan</span><span class="p">:</span> <span class="nb">bool</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Decimal</span><span class="p">:</span>
+</span><span id="TypeParser-664"><a href="#TypeParser-664"><span class="linenos"> 664</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser-665"><a href="#TypeParser-665"><span class="linenos"> 665</span></a><span class="sd">			Parse a string and return it as an exact Decimal if possible</span>
+</span><span id="TypeParser-666"><a href="#TypeParser-666"><span class="linenos"> 666</span></a>
+</span><span id="TypeParser-667"><a href="#TypeParser-667"><span class="linenos"> 667</span></a><span class="sd">			If the string represents a bool, it will be converted to `Decimal(1)` for True and `Decimal(0)` for False. If the string represents an int, it will be converted to a Decimal also.</span>
+</span><span id="TypeParser-668"><a href="#TypeParser-668"><span class="linenos"> 668</span></a>
+</span><span id="TypeParser-669"><a href="#TypeParser-669"><span class="linenos"> 669</span></a><span class="sd">			Behaves analogously to `parse_float()`, except that that returns a non-exact float instead.</span>
+</span><span id="TypeParser-670"><a href="#TypeParser-670"><span class="linenos"> 670</span></a>
+</span><span id="TypeParser-671"><a href="#TypeParser-671"><span class="linenos"> 671</span></a><span class="sd">			Parameters</span>
+</span><span id="TypeParser-672"><a href="#TypeParser-672"><span class="linenos"> 672</span></a><span class="sd">			----------</span>
+</span><span id="TypeParser-673"><a href="#TypeParser-673"><span class="linenos"> 673</span></a><span class="sd">			`value`</span>
+</span><span id="TypeParser-674"><a href="#TypeParser-674"><span class="linenos"> 674</span></a><span class="sd">			: string to be parsed</span>
+</span><span id="TypeParser-675"><a href="#TypeParser-675"><span class="linenos"> 675</span></a>
+</span><span id="TypeParser-676"><a href="#TypeParser-676"><span class="linenos"> 676</span></a><span class="sd">			`allow_scientific`</span>
+</span><span id="TypeParser-677"><a href="#TypeParser-677"><span class="linenos"> 677</span></a><span class="sd">			: whether to accept scientific notation. If True, strings of the form &lt;code&gt;&quot;&lt;var&gt;M&lt;/var&gt;e&lt;var&gt;X&lt;/var&gt;&quot;&lt;/code&gt; will be interpreted as the expression &lt;code&gt;&lt;var&gt;M&lt;/var&gt; * (10 ** &lt;var&gt;X&lt;/var&gt;)&lt;/code&gt;, where &lt;var&gt;M&lt;/var&gt; is the mantissa/significand and &lt;var&gt;X&lt;/var&gt; is the exponent. Note that &lt;var&gt;X&lt;/var&gt; must be an integer, but can be negative.</span>
+</span><span id="TypeParser-678"><a href="#TypeParser-678"><span class="linenos"> 678</span></a>
+</span><span id="TypeParser-679"><a href="#TypeParser-679"><span class="linenos"> 679</span></a><span class="sd">			`allow_inf`</span>
+</span><span id="TypeParser-680"><a href="#TypeParser-680"><span class="linenos"> 680</span></a><span class="sd">			: whether to accept positive and negative infinity values. If True, strings that match the values in `self.inf_values` (empty by default) are interpreted as infinity, or as negative infinity if prepended by a negative sign. The case sensitivity of this matching depends on `self.float_case_sensitive`, which is False by default.</span>
+</span><span id="TypeParser-681"><a href="#TypeParser-681"><span class="linenos"> 681</span></a>
+</span><span id="TypeParser-682"><a href="#TypeParser-682"><span class="linenos"> 682</span></a><span class="sd">			`allow_nan`</span>
+</span><span id="TypeParser-683"><a href="#TypeParser-683"><span class="linenos"> 683</span></a><span class="sd">			: whether to accept NaN (not a number) representations. If True, strings that match the values in `self.nan_values` (empty by default) are interpeted as NaN. The case sensitivity of this matching depends on `self.float_case_sensitive`, which is False by default.</span>
+</span><span id="TypeParser-684"><a href="#TypeParser-684"><span class="linenos"> 684</span></a>
+</span><span id="TypeParser-685"><a href="#TypeParser-685"><span class="linenos"> 685</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser-686"><a href="#TypeParser-686"><span class="linenos"> 686</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser-687"><a href="#TypeParser-687"><span class="linenos"> 687</span></a><span class="sd">			parsed Decimal value</span>
+</span><span id="TypeParser-688"><a href="#TypeParser-688"><span class="linenos"> 688</span></a>
+</span><span id="TypeParser-689"><a href="#TypeParser-689"><span class="linenos"> 689</span></a><span class="sd">			Raises</span>
+</span><span id="TypeParser-690"><a href="#TypeParser-690"><span class="linenos"> 690</span></a><span class="sd">			------</span>
+</span><span id="TypeParser-691"><a href="#TypeParser-691"><span class="linenos"> 691</span></a><span class="sd">			`ValueError` if `value` cannot be parsed</span>
+</span><span id="TypeParser-692"><a href="#TypeParser-692"><span class="linenos"> 692</span></a>
+</span><span id="TypeParser-693"><a href="#TypeParser-693"><span class="linenos"> 693</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser-694"><a href="#TypeParser-694"><span class="linenos"> 694</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser-695"><a href="#TypeParser-695"><span class="linenos"> 695</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser-696"><a href="#TypeParser-696"><span class="linenos"> 696</span></a><span class="sd">			parser = TypeParser(inf_values=[&quot;inf&quot;], nan_values=[&quot;nan&quot;])</span>
+</span><span id="TypeParser-697"><a href="#TypeParser-697"><span class="linenos"> 697</span></a><span class="sd">			parser.parse_decimal(&quot;1.&quot;)       # Decimal(1)</span>
+</span><span id="TypeParser-698"><a href="#TypeParser-698"><span class="linenos"> 698</span></a><span class="sd">			parser.parse_decimal(&quot;1.23e2&quot;)   # Decimal(123)</span>
+</span><span id="TypeParser-699"><a href="#TypeParser-699"><span class="linenos"> 699</span></a><span class="sd">			parser.parse_decimal(&quot;1.23e-2&quot;)  # Decimal(123) / Decimal(10000)</span>
+</span><span id="TypeParser-700"><a href="#TypeParser-700"><span class="linenos"> 700</span></a><span class="sd">			parser.parse_decimal(&quot;inf&quot;)      # Decimal(math.inf)</span>
+</span><span id="TypeParser-701"><a href="#TypeParser-701"><span class="linenos"> 701</span></a><span class="sd">			```</span>
+</span><span id="TypeParser-702"><a href="#TypeParser-702"><span class="linenos"> 702</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser-703"><a href="#TypeParser-703"><span class="linenos"> 703</span></a>		<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_parse_floatlike</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">Decimal</span><span class="p">,</span> <span class="n">Decimal</span><span class="p">(</span><span class="n">math</span><span class="o">.</span><span class="n">inf</span><span class="p">),</span> <span class="n">Decimal</span><span class="p">(</span><span class="n">math</span><span class="o">.</span><span class="n">nan</span><span class="p">),</span>
+</span><span id="TypeParser-704"><a href="#TypeParser-704"><span class="linenos"> 704</span></a>			<span class="n">allow_scientific</span><span class="o">=</span><span class="n">allow_scientific</span><span class="p">,</span>
+</span><span id="TypeParser-705"><a href="#TypeParser-705"><span class="linenos"> 705</span></a>			<span class="n">allow_inf</span><span class="o">=</span><span class="n">allow_inf</span><span class="p">,</span>
+</span><span id="TypeParser-706"><a href="#TypeParser-706"><span class="linenos"> 706</span></a>			<span class="n">allow_nan</span><span class="o">=</span><span class="n">allow_nan</span><span class="p">,</span>
+</span><span id="TypeParser-707"><a href="#TypeParser-707"><span class="linenos"> 707</span></a>		<span class="p">)</span>
+</span><span id="TypeParser-708"><a href="#TypeParser-708"><span class="linenos"> 708</span></a>
+</span><span id="TypeParser-709"><a href="#TypeParser-709"><span class="linenos"> 709</span></a>
+</span><span id="TypeParser-710"><a href="#TypeParser-710"><span class="linenos"> 710</span></a>	<span class="k">def</span> <span class="nf">infer</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">AnyValueType</span><span class="p">:</span>
+</span><span id="TypeParser-711"><a href="#TypeParser-711"><span class="linenos"> 711</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser-712"><a href="#TypeParser-712"><span class="linenos"> 712</span></a><span class="sd">			Infer the underlying type of a string</span>
+</span><span id="TypeParser-713"><a href="#TypeParser-713"><span class="linenos"> 713</span></a>
+</span><span id="TypeParser-714"><a href="#TypeParser-714"><span class="linenos"> 714</span></a><span class="sd">			Also check for inline lists if `self.list_delimiter` is not None.</span>
+</span><span id="TypeParser-715"><a href="#TypeParser-715"><span class="linenos"> 715</span></a>
+</span><span id="TypeParser-716"><a href="#TypeParser-716"><span class="linenos"> 716</span></a><span class="sd">			Parameters</span>
+</span><span id="TypeParser-717"><a href="#TypeParser-717"><span class="linenos"> 717</span></a><span class="sd">			----------</span>
+</span><span id="TypeParser-718"><a href="#TypeParser-718"><span class="linenos"> 718</span></a><span class="sd">			`value`</span>
+</span><span id="TypeParser-719"><a href="#TypeParser-719"><span class="linenos"> 719</span></a><span class="sd">			: the string for which the type should be inferred</span>
+</span><span id="TypeParser-720"><a href="#TypeParser-720"><span class="linenos"> 720</span></a>
+</span><span id="TypeParser-721"><a href="#TypeParser-721"><span class="linenos"> 721</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser-722"><a href="#TypeParser-722"><span class="linenos"> 722</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser-723"><a href="#TypeParser-723"><span class="linenos"> 723</span></a><span class="sd">			inferred type</span>
+</span><span id="TypeParser-724"><a href="#TypeParser-724"><span class="linenos"> 724</span></a>
+</span><span id="TypeParser-725"><a href="#TypeParser-725"><span class="linenos"> 725</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser-726"><a href="#TypeParser-726"><span class="linenos"> 726</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser-727"><a href="#TypeParser-727"><span class="linenos"> 727</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser-728"><a href="#TypeParser-728"><span class="linenos"> 728</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser-729"><a href="#TypeParser-729"><span class="linenos"> 729</span></a><span class="sd">			parser.infer(&quot;true&quot;)  # bool</span>
+</span><span id="TypeParser-730"><a href="#TypeParser-730"><span class="linenos"> 730</span></a><span class="sd">			parser.infer(&quot;2.0&quot;)   # float</span>
+</span><span id="TypeParser-731"><a href="#TypeParser-731"><span class="linenos"> 731</span></a><span class="sd">			parser.infer(&quot;abc&quot;)   # str</span>
+</span><span id="TypeParser-732"><a href="#TypeParser-732"><span class="linenos"> 732</span></a><span class="sd">			```</span>
+</span><span id="TypeParser-733"><a href="#TypeParser-733"><span class="linenos"> 733</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser-734"><a href="#TypeParser-734"><span class="linenos"> 734</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_none</span><span class="p">(</span><span class="n">value</span><span class="p">):</span>
+</span><span id="TypeParser-735"><a href="#TypeParser-735"><span class="linenos"> 735</span></a>			<span class="k">return</span> <span class="n">NoneType</span>
+</span><span id="TypeParser-736"><a href="#TypeParser-736"><span class="linenos"> 736</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_bool</span><span class="p">(</span><span class="n">value</span><span class="p">):</span>
+</span><span id="TypeParser-737"><a href="#TypeParser-737"><span class="linenos"> 737</span></a>			<span class="k">return</span> <span class="nb">bool</span>
+</span><span id="TypeParser-738"><a href="#TypeParser-738"><span class="linenos"> 738</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_int</span><span class="p">(</span><span class="n">value</span><span class="p">):</span>
+</span><span id="TypeParser-739"><a href="#TypeParser-739"><span class="linenos"> 739</span></a>			<span class="k">return</span> <span class="nb">int</span>
+</span><span id="TypeParser-740"><a href="#TypeParser-740"><span class="linenos"> 740</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_float</span><span class="p">(</span><span class="n">value</span><span class="p">):</span>
+</span><span id="TypeParser-741"><a href="#TypeParser-741"><span class="linenos"> 741</span></a>			<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">use_decimal</span><span class="p">:</span>
+</span><span id="TypeParser-742"><a href="#TypeParser-742"><span class="linenos"> 742</span></a>				<span class="k">return</span> <span class="n">Decimal</span>
+</span><span id="TypeParser-743"><a href="#TypeParser-743"><span class="linenos"> 743</span></a>			<span class="k">else</span><span class="p">:</span>
+</span><span id="TypeParser-744"><a href="#TypeParser-744"><span class="linenos"> 744</span></a>				<span class="k">return</span> <span class="nb">float</span>
+</span><span id="TypeParser-745"><a href="#TypeParser-745"><span class="linenos"> 745</span></a>
+</span><span id="TypeParser-746"><a href="#TypeParser-746"><span class="linenos"> 746</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">trim</span><span class="p">:</span>
+</span><span id="TypeParser-747"><a href="#TypeParser-747"><span class="linenos"> 747</span></a>			<span class="n">value</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
+</span><span id="TypeParser-748"><a href="#TypeParser-748"><span class="linenos"> 748</span></a>
+</span><span id="TypeParser-749"><a href="#TypeParser-749"><span class="linenos"> 749</span></a>		<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">list_delimiter</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">list_delimiter</span> <span class="ow">in</span> <span class="n">value</span><span class="p">:</span>
+</span><span id="TypeParser-750"><a href="#TypeParser-750"><span class="linenos"> 750</span></a>			<span class="n">subvalues</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">list_delimiter</span><span class="p">)</span>
+</span><span id="TypeParser-751"><a href="#TypeParser-751"><span class="linenos"> 751</span></a>			<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">trim</span><span class="p">:</span>
+</span><span id="TypeParser-752"><a href="#TypeParser-752"><span class="linenos"> 752</span></a>				<span class="n">subvalues</span> <span class="o">=</span> <span class="p">[</span><span class="n">subvalue</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="k">for</span> <span class="n">subvalue</span> <span class="ow">in</span> <span class="n">subvalues</span><span class="p">]</span>
+</span><span id="TypeParser-753"><a href="#TypeParser-753"><span class="linenos"> 753</span></a>			<span class="n">reduced_type</span> <span class="o">=</span> <span class="n">reduce_types</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">subvalue</span><span class="p">)</span> <span class="k">for</span> <span class="n">subvalue</span> <span class="ow">in</span> <span class="n">subvalues</span><span class="p">)</span>
+</span><span id="TypeParser-754"><a href="#TypeParser-754"><span class="linenos"> 754</span></a>			<span class="n">r</span> <span class="o">=</span> <span class="nb">list</span><span class="p">[</span><span class="n">reduced_type</span><span class="p">]</span>
+</span><span id="TypeParser-755"><a href="#TypeParser-755"><span class="linenos"> 755</span></a>			<span class="k">return</span> <span class="n">r</span>
+</span><span id="TypeParser-756"><a href="#TypeParser-756"><span class="linenos"> 756</span></a>
+</span><span id="TypeParser-757"><a href="#TypeParser-757"><span class="linenos"> 757</span></a>		<span class="k">return</span> <span class="n">GenericValue</span>
+</span><span id="TypeParser-758"><a href="#TypeParser-758"><span class="linenos"> 758</span></a>
+</span><span id="TypeParser-759"><a href="#TypeParser-759"><span class="linenos"> 759</span></a>
+</span><span id="TypeParser-760"><a href="#TypeParser-760"><span class="linenos"> 760</span></a>	<span class="k">def</span> <span class="nf">infer_series</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="n">AnyValueType</span><span class="p">:</span>
+</span><span id="TypeParser-761"><a href="#TypeParser-761"><span class="linenos"> 761</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser-762"><a href="#TypeParser-762"><span class="linenos"> 762</span></a><span class="sd">			Infer the underlying common type of a series of strings</span>
+</span><span id="TypeParser-763"><a href="#TypeParser-763"><span class="linenos"> 763</span></a>
+</span><span id="TypeParser-764"><a href="#TypeParser-764"><span class="linenos"> 764</span></a><span class="sd">			If the values in the series do not have the same apparent type, the resulting type will be narrowest possible type that will encompass all values in the series. See `parsetypes.reduce_types()` for more information.</span>
+</span><span id="TypeParser-765"><a href="#TypeParser-765"><span class="linenos"> 765</span></a>
+</span><span id="TypeParser-766"><a href="#TypeParser-766"><span class="linenos"> 766</span></a><span class="sd">			Parameters</span>
+</span><span id="TypeParser-767"><a href="#TypeParser-767"><span class="linenos"> 767</span></a><span class="sd">			----------</span>
+</span><span id="TypeParser-768"><a href="#TypeParser-768"><span class="linenos"> 768</span></a><span class="sd">			`values`</span>
+</span><span id="TypeParser-769"><a href="#TypeParser-769"><span class="linenos"> 769</span></a><span class="sd">			: series of strings for which the type should be inferred</span>
+</span><span id="TypeParser-770"><a href="#TypeParser-770"><span class="linenos"> 770</span></a>
+</span><span id="TypeParser-771"><a href="#TypeParser-771"><span class="linenos"> 771</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser-772"><a href="#TypeParser-772"><span class="linenos"> 772</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser-773"><a href="#TypeParser-773"><span class="linenos"> 773</span></a><span class="sd">			inferred type</span>
+</span><span id="TypeParser-774"><a href="#TypeParser-774"><span class="linenos"> 774</span></a>
+</span><span id="TypeParser-775"><a href="#TypeParser-775"><span class="linenos"> 775</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser-776"><a href="#TypeParser-776"><span class="linenos"> 776</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser-777"><a href="#TypeParser-777"><span class="linenos"> 777</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser-778"><a href="#TypeParser-778"><span class="linenos"> 778</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser-779"><a href="#TypeParser-779"><span class="linenos"> 779</span></a><span class="sd">			parser.infer_series([&quot;1&quot;, &quot;2&quot;, &quot;3.4&quot;])       # float</span>
+</span><span id="TypeParser-780"><a href="#TypeParser-780"><span class="linenos"> 780</span></a><span class="sd">			parser.infer_series([&quot;true&quot;, &quot;false&quot;, &quot;2&quot;])  # int</span>
+</span><span id="TypeParser-781"><a href="#TypeParser-781"><span class="linenos"> 781</span></a><span class="sd">			parser.infer_series([&quot;1&quot;, &quot;2.3&quot;, &quot;abc&quot;])     # str</span>
+</span><span id="TypeParser-782"><a href="#TypeParser-782"><span class="linenos"> 782</span></a><span class="sd">			```</span>
+</span><span id="TypeParser-783"><a href="#TypeParser-783"><span class="linenos"> 783</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser-784"><a href="#TypeParser-784"><span class="linenos"> 784</span></a>		<span class="k">return</span> <span class="n">reduce_types</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
+</span><span id="TypeParser-785"><a href="#TypeParser-785"><span class="linenos"> 785</span></a>
+</span><span id="TypeParser-786"><a href="#TypeParser-786"><span class="linenos"> 786</span></a>
+</span><span id="TypeParser-787"><a href="#TypeParser-787"><span class="linenos"> 787</span></a>	<span class="k">def</span> <span class="nf">infer_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">rows</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">AnyValueType</span><span class="p">]:</span>
+</span><span id="TypeParser-788"><a href="#TypeParser-788"><span class="linenos"> 788</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser-789"><a href="#TypeParser-789"><span class="linenos"> 789</span></a><span class="sd">			Infer the underlying common type for each column of a table of strings</span>
+</span><span id="TypeParser-790"><a href="#TypeParser-790"><span class="linenos"> 790</span></a>
+</span><span id="TypeParser-791"><a href="#TypeParser-791"><span class="linenos"> 791</span></a><span class="sd">			For each column, if the values do not have the same apparent type, the resulting type will be narrowest possible type that will encompass all values in the column. See `parsetypes.reduce_types()` for more information.</span>
+</span><span id="TypeParser-792"><a href="#TypeParser-792"><span class="linenos"> 792</span></a>
+</span><span id="TypeParser-793"><a href="#TypeParser-793"><span class="linenos"> 793</span></a><span class="sd">			Note that the individual inferred types of every value in the table must be able to fit into memory.</span>
+</span><span id="TypeParser-794"><a href="#TypeParser-794"><span class="linenos"> 794</span></a>
+</span><span id="TypeParser-795"><a href="#TypeParser-795"><span class="linenos"> 795</span></a><span class="sd">			Parameters</span>
+</span><span id="TypeParser-796"><a href="#TypeParser-796"><span class="linenos"> 796</span></a><span class="sd">			----------</span>
+</span><span id="TypeParser-797"><a href="#TypeParser-797"><span class="linenos"> 797</span></a><span class="sd">			`rows`</span>
+</span><span id="TypeParser-798"><a href="#TypeParser-798"><span class="linenos"> 798</span></a><span class="sd">			: table of strings for which the types should be inferred, in row-major order</span>
+</span><span id="TypeParser-799"><a href="#TypeParser-799"><span class="linenos"> 799</span></a>
+</span><span id="TypeParser-800"><a href="#TypeParser-800"><span class="linenos"> 800</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser-801"><a href="#TypeParser-801"><span class="linenos"> 801</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser-802"><a href="#TypeParser-802"><span class="linenos"> 802</span></a><span class="sd">			inferred types</span>
+</span><span id="TypeParser-803"><a href="#TypeParser-803"><span class="linenos"> 803</span></a>
+</span><span id="TypeParser-804"><a href="#TypeParser-804"><span class="linenos"> 804</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser-805"><a href="#TypeParser-805"><span class="linenos"> 805</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser-806"><a href="#TypeParser-806"><span class="linenos"> 806</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser-807"><a href="#TypeParser-807"><span class="linenos"> 807</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser-808"><a href="#TypeParser-808"><span class="linenos"> 808</span></a><span class="sd">			parser.infer_table([</span>
+</span><span id="TypeParser-809"><a href="#TypeParser-809"><span class="linenos"> 809</span></a><span class="sd">				[&quot;1&quot;,   &quot;true&quot;,  &quot;1&quot;],</span>
+</span><span id="TypeParser-810"><a href="#TypeParser-810"><span class="linenos"> 810</span></a><span class="sd">				[&quot;2&quot;,   &quot;false&quot;, &quot;2.3&quot;],</span>
+</span><span id="TypeParser-811"><a href="#TypeParser-811"><span class="linenos"> 811</span></a><span class="sd">				[&quot;3.4&quot;, &quot;2&quot;,     &quot;abc&quot;],</span>
+</span><span id="TypeParser-812"><a href="#TypeParser-812"><span class="linenos"> 812</span></a><span class="sd">			])</span>
+</span><span id="TypeParser-813"><a href="#TypeParser-813"><span class="linenos"> 813</span></a><span class="sd">			# [float, int, str]</span>
+</span><span id="TypeParser-814"><a href="#TypeParser-814"><span class="linenos"> 814</span></a><span class="sd">			```</span>
+</span><span id="TypeParser-815"><a href="#TypeParser-815"><span class="linenos"> 815</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser-816"><a href="#TypeParser-816"><span class="linenos"> 816</span></a>		<span class="n">rows_iter</span> <span class="o">=</span> <span class="nb">iter</span><span class="p">(</span><span class="n">rows</span><span class="p">)</span>
+</span><span id="TypeParser-817"><a href="#TypeParser-817"><span class="linenos"> 817</span></a>		<span class="n">first_row</span> <span class="o">=</span> <span class="nb">next</span><span class="p">(</span><span class="n">rows_iter</span><span class="p">,</span> <span class="kc">None</span><span class="p">)</span>
+</span><span id="TypeParser-818"><a href="#TypeParser-818"><span class="linenos"> 818</span></a>		<span class="k">if</span> <span class="n">first_row</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="TypeParser-819"><a href="#TypeParser-819"><span class="linenos"> 819</span></a>			<span class="k">return</span> <span class="p">[]</span>
+</span><span id="TypeParser-820"><a href="#TypeParser-820"><span class="linenos"> 820</span></a>
+</span><span id="TypeParser-821"><a href="#TypeParser-821"><span class="linenos"> 821</span></a>		<span class="n">num_cols</span> <span class="o">=</span> <span class="nb">len</span><span class="p">(</span><span class="n">first_row</span><span class="p">)</span>
+</span><span id="TypeParser-822"><a href="#TypeParser-822"><span class="linenos"> 822</span></a>		<span class="k">if</span> <span class="n">num_cols</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="TypeParser-823"><a href="#TypeParser-823"><span class="linenos"> 823</span></a>			<span class="k">return</span> <span class="p">[]</span>
+</span><span id="TypeParser-824"><a href="#TypeParser-824"><span class="linenos"> 824</span></a>
+</span><span id="TypeParser-825"><a href="#TypeParser-825"><span class="linenos"> 825</span></a>		<span class="n">table</span> <span class="o">=</span> <span class="n">_TypeTable</span><span class="p">([[</span><span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">value</span><span class="p">)]</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">first_row</span><span class="p">])</span>
+</span><span id="TypeParser-826"><a href="#TypeParser-826"><span class="linenos"> 826</span></a>		<span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">rows_iter</span><span class="p">:</span>
+</span><span id="TypeParser-827"><a href="#TypeParser-827"><span class="linenos"> 827</span></a>			<span class="n">table</span><span class="o">.</span><span class="n">add_row</span><span class="p">([</span><span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">row</span><span class="p">])</span>
+</span><span id="TypeParser-828"><a href="#TypeParser-828"><span class="linenos"> 828</span></a>
+</span><span id="TypeParser-829"><a href="#TypeParser-829"><span class="linenos"> 829</span></a>		<span class="k">return</span> <span class="p">[</span><span class="n">reduce_types</span><span class="p">(</span><span class="n">col</span><span class="p">)</span> <span class="k">for</span> <span class="n">col</span> <span class="ow">in</span> <span class="n">table</span><span class="o">.</span><span class="n">cols</span><span class="p">]</span>
+</span><span id="TypeParser-830"><a href="#TypeParser-830"><span class="linenos"> 830</span></a>
+</span><span id="TypeParser-831"><a href="#TypeParser-831"><span class="linenos"> 831</span></a>
+</span><span id="TypeParser-832"><a href="#TypeParser-832"><span class="linenos"> 832</span></a>	<span class="k">def</span> <span class="nf">convert</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">target_type</span><span class="p">:</span> <span class="n">AnyValueType</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">AnyValue</span><span class="p">:</span>
+</span><span id="TypeParser-833"><a href="#TypeParser-833"><span class="linenos"> 833</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser-834"><a href="#TypeParser-834"><span class="linenos"> 834</span></a><span class="sd">			Convert a string to the specified target type if possible</span>
+</span><span id="TypeParser-835"><a href="#TypeParser-835"><span class="linenos"> 835</span></a>
+</span><span id="TypeParser-836"><a href="#TypeParser-836"><span class="linenos"> 836</span></a><span class="sd">			Valid values for `target_type` include any return value from `infer()`, `infer_series()` and `infer_table()`. To infer and convert the string automatically, use `parse()`, `parse_series()` or `parse_table()` instead.</span>
+</span><span id="TypeParser-837"><a href="#TypeParser-837"><span class="linenos"> 837</span></a>
+</span><span id="TypeParser-838"><a href="#TypeParser-838"><span class="linenos"> 838</span></a><span class="sd">			Parameters</span>
+</span><span id="TypeParser-839"><a href="#TypeParser-839"><span class="linenos"> 839</span></a><span class="sd">			----------</span>
+</span><span id="TypeParser-840"><a href="#TypeParser-840"><span class="linenos"> 840</span></a><span class="sd">			`value`</span>
+</span><span id="TypeParser-841"><a href="#TypeParser-841"><span class="linenos"> 841</span></a><span class="sd">			: the string to be converted</span>
+</span><span id="TypeParser-842"><a href="#TypeParser-842"><span class="linenos"> 842</span></a>
+</span><span id="TypeParser-843"><a href="#TypeParser-843"><span class="linenos"> 843</span></a><span class="sd">			`target_type`</span>
+</span><span id="TypeParser-844"><a href="#TypeParser-844"><span class="linenos"> 844</span></a><span class="sd">			: type to which the value should be converted</span>
+</span><span id="TypeParser-845"><a href="#TypeParser-845"><span class="linenos"> 845</span></a>
+</span><span id="TypeParser-846"><a href="#TypeParser-846"><span class="linenos"> 846</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser-847"><a href="#TypeParser-847"><span class="linenos"> 847</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser-848"><a href="#TypeParser-848"><span class="linenos"> 848</span></a><span class="sd">			converted value</span>
+</span><span id="TypeParser-849"><a href="#TypeParser-849"><span class="linenos"> 849</span></a>
+</span><span id="TypeParser-850"><a href="#TypeParser-850"><span class="linenos"> 850</span></a><span class="sd">			Raises</span>
+</span><span id="TypeParser-851"><a href="#TypeParser-851"><span class="linenos"> 851</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser-852"><a href="#TypeParser-852"><span class="linenos"> 852</span></a><span class="sd">			`ValueError`</span>
+</span><span id="TypeParser-853"><a href="#TypeParser-853"><span class="linenos"> 853</span></a><span class="sd">			: if `value` cannot be converted to `target_type`</span>
+</span><span id="TypeParser-854"><a href="#TypeParser-854"><span class="linenos"> 854</span></a>
+</span><span id="TypeParser-855"><a href="#TypeParser-855"><span class="linenos"> 855</span></a><span class="sd">			`TypeError`</span>
+</span><span id="TypeParser-856"><a href="#TypeParser-856"><span class="linenos"> 856</span></a><span class="sd">			: if `target_type` is not a valid type</span>
+</span><span id="TypeParser-857"><a href="#TypeParser-857"><span class="linenos"> 857</span></a>
+</span><span id="TypeParser-858"><a href="#TypeParser-858"><span class="linenos"> 858</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser-859"><a href="#TypeParser-859"><span class="linenos"> 859</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser-860"><a href="#TypeParser-860"><span class="linenos"> 860</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser-861"><a href="#TypeParser-861"><span class="linenos"> 861</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser-862"><a href="#TypeParser-862"><span class="linenos"> 862</span></a><span class="sd">			parser.convert(&quot;true&quot;, bool)  # True</span>
+</span><span id="TypeParser-863"><a href="#TypeParser-863"><span class="linenos"> 863</span></a><span class="sd">			parser.convert(&quot;2&quot;, int)      # 2</span>
+</span><span id="TypeParser-864"><a href="#TypeParser-864"><span class="linenos"> 864</span></a><span class="sd">			parser.convert(&quot;2&quot;, float)    # 2.</span>
+</span><span id="TypeParser-865"><a href="#TypeParser-865"><span class="linenos"> 865</span></a><span class="sd">			```</span>
+</span><span id="TypeParser-866"><a href="#TypeParser-866"><span class="linenos"> 866</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser-867"><a href="#TypeParser-867"><span class="linenos"> 867</span></a>		<span class="n">base</span><span class="p">,</span> <span class="n">type_args</span> <span class="o">=</span> <span class="n">_decompose_type</span><span class="p">(</span><span class="n">target_type</span><span class="p">)</span>
+</span><span id="TypeParser-868"><a href="#TypeParser-868"><span class="linenos"> 868</span></a>		<span class="k">if</span> <span class="n">base</span> <span class="o">==</span> <span class="n">NoneType</span><span class="p">:</span>
+</span><span id="TypeParser-869"><a href="#TypeParser-869"><span class="linenos"> 869</span></a>			<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_none</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
+</span><span id="TypeParser-870"><a href="#TypeParser-870"><span class="linenos"> 870</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="TypeParser-871"><a href="#TypeParser-871"><span class="linenos"> 871</span></a>			<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_bool</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
+</span><span id="TypeParser-872"><a href="#TypeParser-872"><span class="linenos"> 872</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="TypeParser-873"><a href="#TypeParser-873"><span class="linenos"> 873</span></a>			<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_int</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
+</span><span id="TypeParser-874"><a href="#TypeParser-874"><span class="linenos"> 874</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="n">Decimal</span><span class="p">:</span>
+</span><span id="TypeParser-875"><a href="#TypeParser-875"><span class="linenos"> 875</span></a>			<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_decimal</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
+</span><span id="TypeParser-876"><a href="#TypeParser-876"><span class="linenos"> 876</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">float</span><span class="p">:</span>
+</span><span id="TypeParser-877"><a href="#TypeParser-877"><span class="linenos"> 877</span></a>			<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_float</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
+</span><span id="TypeParser-878"><a href="#TypeParser-878"><span class="linenos"> 878</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="TypeParser-879"><a href="#TypeParser-879"><span class="linenos"> 879</span></a>			<span class="k">return</span> <span class="n">value</span>
+</span><span id="TypeParser-880"><a href="#TypeParser-880"><span class="linenos"> 880</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="n">Nullable</span><span class="p">:</span>
+</span><span id="TypeParser-881"><a href="#TypeParser-881"><span class="linenos"> 881</span></a>			<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_none</span><span class="p">(</span><span class="n">value</span><span class="p">):</span>
+</span><span id="TypeParser-882"><a href="#TypeParser-882"><span class="linenos"> 882</span></a>				<span class="k">return</span> <span class="kc">None</span>
+</span><span id="TypeParser-883"><a href="#TypeParser-883"><span class="linenos"> 883</span></a>			<span class="k">else</span><span class="p">:</span>
+</span><span id="TypeParser-884"><a href="#TypeParser-884"><span class="linenos"> 884</span></a>				<span class="k">if</span> <span class="n">type_args</span> <span class="ow">is</span> <span class="ow">not</span>  <span class="kc">None</span> <span class="ow">and</span> <span class="nb">len</span><span class="p">(</span><span class="n">type_args</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span> <span class="ow">and</span> <span class="n">type_args</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">!=</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="TypeParser-885"><a href="#TypeParser-885"><span class="linenos"> 885</span></a>					<span class="n">inner_type</span> <span class="o">=</span> <span class="n">type_args</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="TypeParser-886"><a href="#TypeParser-886"><span class="linenos"> 886</span></a>					<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">convert</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">inner_type</span><span class="p">)</span>
+</span><span id="TypeParser-887"><a href="#TypeParser-887"><span class="linenos"> 887</span></a>				<span class="k">else</span><span class="p">:</span>
+</span><span id="TypeParser-888"><a href="#TypeParser-888"><span class="linenos"> 888</span></a>					<span class="k">return</span> <span class="n">value</span>
+</span><span id="TypeParser-889"><a href="#TypeParser-889"><span class="linenos"> 889</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">list</span><span class="p">:</span>
+</span><span id="TypeParser-890"><a href="#TypeParser-890"><span class="linenos"> 890</span></a>			<span class="n">subvalues</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">list_delimiter</span><span class="p">)</span>
+</span><span id="TypeParser-891"><a href="#TypeParser-891"><span class="linenos"> 891</span></a>			<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">trim</span><span class="p">:</span>
+</span><span id="TypeParser-892"><a href="#TypeParser-892"><span class="linenos"> 892</span></a>				<span class="n">subvalues</span> <span class="o">=</span> <span class="p">[</span><span class="n">subvalue</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="k">for</span> <span class="n">subvalue</span> <span class="ow">in</span> <span class="n">subvalues</span><span class="p">]</span>
+</span><span id="TypeParser-893"><a href="#TypeParser-893"><span class="linenos"> 893</span></a>			<span class="k">if</span> <span class="n">type_args</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span> <span class="ow">and</span> <span class="nb">len</span><span class="p">(</span><span class="n">type_args</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span> <span class="ow">and</span> <span class="n">type_args</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">!=</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="TypeParser-894"><a href="#TypeParser-894"><span class="linenos"> 894</span></a>				<span class="n">subtype</span> <span class="o">=</span> <span class="n">type_args</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="TypeParser-895"><a href="#TypeParser-895"><span class="linenos"> 895</span></a>				<span class="k">return</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">convert</span><span class="p">(</span><span class="n">subvalue</span><span class="p">,</span> <span class="n">subtype</span><span class="p">)</span> <span class="k">for</span> <span class="n">subvalue</span> <span class="ow">in</span> <span class="n">subvalues</span><span class="p">]</span>
+</span><span id="TypeParser-896"><a href="#TypeParser-896"><span class="linenos"> 896</span></a>			<span class="k">else</span><span class="p">:</span>
+</span><span id="TypeParser-897"><a href="#TypeParser-897"><span class="linenos"> 897</span></a>				<span class="k">return</span> <span class="n">subvalues</span>
+</span><span id="TypeParser-898"><a href="#TypeParser-898"><span class="linenos"> 898</span></a>		<span class="k">else</span><span class="p">:</span>
+</span><span id="TypeParser-899"><a href="#TypeParser-899"><span class="linenos"> 899</span></a>			<span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;cannot convert to type: </span><span class="si">{</span><span class="n">target_type</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="TypeParser-900"><a href="#TypeParser-900"><span class="linenos"> 900</span></a>
+</span><span id="TypeParser-901"><a href="#TypeParser-901"><span class="linenos"> 901</span></a>
+</span><span id="TypeParser-902"><a href="#TypeParser-902"><span class="linenos"> 902</span></a>	<span class="k">def</span> <span class="nf">parse</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">AnyValue</span><span class="p">:</span>
+</span><span id="TypeParser-903"><a href="#TypeParser-903"><span class="linenos"> 903</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser-904"><a href="#TypeParser-904"><span class="linenos"> 904</span></a><span class="sd">			Parse a string and convert it to its underlying type</span>
+</span><span id="TypeParser-905"><a href="#TypeParser-905"><span class="linenos"> 905</span></a>
+</span><span id="TypeParser-906"><a href="#TypeParser-906"><span class="linenos"> 906</span></a><span class="sd">			Parameters</span>
+</span><span id="TypeParser-907"><a href="#TypeParser-907"><span class="linenos"> 907</span></a><span class="sd">			----------</span>
+</span><span id="TypeParser-908"><a href="#TypeParser-908"><span class="linenos"> 908</span></a><span class="sd">			`value`</span>
+</span><span id="TypeParser-909"><a href="#TypeParser-909"><span class="linenos"> 909</span></a><span class="sd">			: the string to be parsed</span>
+</span><span id="TypeParser-910"><a href="#TypeParser-910"><span class="linenos"> 910</span></a>
+</span><span id="TypeParser-911"><a href="#TypeParser-911"><span class="linenos"> 911</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser-912"><a href="#TypeParser-912"><span class="linenos"> 912</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser-913"><a href="#TypeParser-913"><span class="linenos"> 913</span></a><span class="sd">			converted value</span>
+</span><span id="TypeParser-914"><a href="#TypeParser-914"><span class="linenos"> 914</span></a>
+</span><span id="TypeParser-915"><a href="#TypeParser-915"><span class="linenos"> 915</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser-916"><a href="#TypeParser-916"><span class="linenos"> 916</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser-917"><a href="#TypeParser-917"><span class="linenos"> 917</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser-918"><a href="#TypeParser-918"><span class="linenos"> 918</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser-919"><a href="#TypeParser-919"><span class="linenos"> 919</span></a><span class="sd">			parser.parse(&quot;true&quot;)  # True</span>
+</span><span id="TypeParser-920"><a href="#TypeParser-920"><span class="linenos"> 920</span></a><span class="sd">			parser.parse(&quot;2.0&quot;)   # 2.</span>
+</span><span id="TypeParser-921"><a href="#TypeParser-921"><span class="linenos"> 921</span></a><span class="sd">			parser.parse(&quot;abc&quot;)   # &quot;abc&quot;</span>
+</span><span id="TypeParser-922"><a href="#TypeParser-922"><span class="linenos"> 922</span></a><span class="sd">			```</span>
+</span><span id="TypeParser-923"><a href="#TypeParser-923"><span class="linenos"> 923</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser-924"><a href="#TypeParser-924"><span class="linenos"> 924</span></a>		<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">convert</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">value</span><span class="p">))</span>
+</span><span id="TypeParser-925"><a href="#TypeParser-925"><span class="linenos"> 925</span></a>
+</span><span id="TypeParser-926"><a href="#TypeParser-926"><span class="linenos"> 926</span></a>
+</span><span id="TypeParser-927"><a href="#TypeParser-927"><span class="linenos"> 927</span></a>	<span class="k">def</span> <span class="nf">parse_series</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">AnyValue</span><span class="p">]:</span>
+</span><span id="TypeParser-928"><a href="#TypeParser-928"><span class="linenos"> 928</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser-929"><a href="#TypeParser-929"><span class="linenos"> 929</span></a><span class="sd">			Parse a series of strings and convert them to their underlying common type</span>
+</span><span id="TypeParser-930"><a href="#TypeParser-930"><span class="linenos"> 930</span></a>
+</span><span id="TypeParser-931"><a href="#TypeParser-931"><span class="linenos"> 931</span></a><span class="sd">			If the values in the series do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the series. See `parsetypes.reduce_types()` for more information.</span>
+</span><span id="TypeParser-932"><a href="#TypeParser-932"><span class="linenos"> 932</span></a>
+</span><span id="TypeParser-933"><a href="#TypeParser-933"><span class="linenos"> 933</span></a><span class="sd">			Parameters</span>
+</span><span id="TypeParser-934"><a href="#TypeParser-934"><span class="linenos"> 934</span></a><span class="sd">			----------</span>
+</span><span id="TypeParser-935"><a href="#TypeParser-935"><span class="linenos"> 935</span></a><span class="sd">			`values`</span>
+</span><span id="TypeParser-936"><a href="#TypeParser-936"><span class="linenos"> 936</span></a><span class="sd">			: series of strings to be parsed</span>
+</span><span id="TypeParser-937"><a href="#TypeParser-937"><span class="linenos"> 937</span></a>
+</span><span id="TypeParser-938"><a href="#TypeParser-938"><span class="linenos"> 938</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser-939"><a href="#TypeParser-939"><span class="linenos"> 939</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser-940"><a href="#TypeParser-940"><span class="linenos"> 940</span></a><span class="sd">			converted values</span>
+</span><span id="TypeParser-941"><a href="#TypeParser-941"><span class="linenos"> 941</span></a>
+</span><span id="TypeParser-942"><a href="#TypeParser-942"><span class="linenos"> 942</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser-943"><a href="#TypeParser-943"><span class="linenos"> 943</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser-944"><a href="#TypeParser-944"><span class="linenos"> 944</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser-945"><a href="#TypeParser-945"><span class="linenos"> 945</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser-946"><a href="#TypeParser-946"><span class="linenos"> 946</span></a><span class="sd">			parser.parse_series([&quot;1&quot;, &quot;2&quot;, &quot;3&quot;])        # [1, 2, 3]</span>
+</span><span id="TypeParser-947"><a href="#TypeParser-947"><span class="linenos"> 947</span></a><span class="sd">			parser.parse_series([&quot;5&quot;, &quot;6.7&quot;, &quot;8.&quot;])     # [5., 6.7, 8.]</span>
+</span><span id="TypeParser-948"><a href="#TypeParser-948"><span class="linenos"> 948</span></a><span class="sd">			parser.parse_series([&quot;true&quot;, &quot;false&quot;, &quot;&quot;])  # [True, False, None]</span>
+</span><span id="TypeParser-949"><a href="#TypeParser-949"><span class="linenos"> 949</span></a><span class="sd">			parser.parse_series([&quot;1&quot;, &quot;2.3&quot;, &quot;abc&quot;])    # [&quot;1&quot;, &quot;2.3&quot;, &quot;abc&quot;]</span>
+</span><span id="TypeParser-950"><a href="#TypeParser-950"><span class="linenos"> 950</span></a><span class="sd">			```</span>
+</span><span id="TypeParser-951"><a href="#TypeParser-951"><span class="linenos"> 951</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser-952"><a href="#TypeParser-952"><span class="linenos"> 952</span></a>		<span class="n">inferred</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">infer_series</span><span class="p">(</span><span class="n">values</span><span class="p">)</span>
+</span><span id="TypeParser-953"><a href="#TypeParser-953"><span class="linenos"> 953</span></a>		<span class="k">return</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">convert</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">inferred</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">values</span><span class="p">]</span>
+</span><span id="TypeParser-954"><a href="#TypeParser-954"><span class="linenos"> 954</span></a>
+</span><span id="TypeParser-955"><a href="#TypeParser-955"><span class="linenos"> 955</span></a>
+</span><span id="TypeParser-956"><a href="#TypeParser-956"><span class="linenos"> 956</span></a>	<span class="k">def</span> <span class="nf">parse_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">rows</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">AnyValue</span><span class="p">]]:</span>
+</span><span id="TypeParser-957"><a href="#TypeParser-957"><span class="linenos"> 957</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser-958"><a href="#TypeParser-958"><span class="linenos"> 958</span></a><span class="sd">			Parse a table of strings and convert them to the underlying common type of each column</span>
+</span><span id="TypeParser-959"><a href="#TypeParser-959"><span class="linenos"> 959</span></a>
+</span><span id="TypeParser-960"><a href="#TypeParser-960"><span class="linenos"> 960</span></a><span class="sd">			For each column, if the values do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the column. See `parsetypes.reduce_types()` for more information.</span>
+</span><span id="TypeParser-961"><a href="#TypeParser-961"><span class="linenos"> 961</span></a>
+</span><span id="TypeParser-962"><a href="#TypeParser-962"><span class="linenos"> 962</span></a><span class="sd">			Note that the type to which the values should be converted is determined by `infer_table()`, and so the individual inferred types of every value in the table must be able to fit into memory.</span>
+</span><span id="TypeParser-963"><a href="#TypeParser-963"><span class="linenos"> 963</span></a>
+</span><span id="TypeParser-964"><a href="#TypeParser-964"><span class="linenos"> 964</span></a><span class="sd">			This is a function that computes the entire table and returns it all at once. The generator `iterate_table()` behaves analogously, except that it computes and yields each row one at a time.</span>
+</span><span id="TypeParser-965"><a href="#TypeParser-965"><span class="linenos"> 965</span></a>
+</span><span id="TypeParser-966"><a href="#TypeParser-966"><span class="linenos"> 966</span></a><span class="sd">			Parameters</span>
+</span><span id="TypeParser-967"><a href="#TypeParser-967"><span class="linenos"> 967</span></a><span class="sd">			----------</span>
+</span><span id="TypeParser-968"><a href="#TypeParser-968"><span class="linenos"> 968</span></a><span class="sd">			`rows`</span>
+</span><span id="TypeParser-969"><a href="#TypeParser-969"><span class="linenos"> 969</span></a><span class="sd">			: table of strings to be parsed, in row-major order</span>
+</span><span id="TypeParser-970"><a href="#TypeParser-970"><span class="linenos"> 970</span></a>
+</span><span id="TypeParser-971"><a href="#TypeParser-971"><span class="linenos"> 971</span></a><span class="sd">			`iterator`</span>
+</span><span id="TypeParser-972"><a href="#TypeParser-972"><span class="linenos"> 972</span></a><span class="sd">			: whether the parsed values should be yielded as an iterator. If False, which is the default, the entire table is computed and returned as a list of lists. If True, this function behaves as a generator, and the rows of the table are computed and yielded one at a time. However, note that even when set to True, the type inference requires that inferred type of each individual value must all be able to fit into memory at once.</span>
+</span><span id="TypeParser-973"><a href="#TypeParser-973"><span class="linenos"> 973</span></a>
+</span><span id="TypeParser-974"><a href="#TypeParser-974"><span class="linenos"> 974</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser-975"><a href="#TypeParser-975"><span class="linenos"> 975</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser-976"><a href="#TypeParser-976"><span class="linenos"> 976</span></a><span class="sd">			converted table of values, in row-major order</span>
+</span><span id="TypeParser-977"><a href="#TypeParser-977"><span class="linenos"> 977</span></a>
+</span><span id="TypeParser-978"><a href="#TypeParser-978"><span class="linenos"> 978</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser-979"><a href="#TypeParser-979"><span class="linenos"> 979</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser-980"><a href="#TypeParser-980"><span class="linenos"> 980</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser-981"><a href="#TypeParser-981"><span class="linenos"> 981</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser-982"><a href="#TypeParser-982"><span class="linenos"> 982</span></a><span class="sd">			table = parser.parse_table([</span>
+</span><span id="TypeParser-983"><a href="#TypeParser-983"><span class="linenos"> 983</span></a><span class="sd">				[&quot;1&quot;, &quot;5&quot;,   &quot;true&quot;,  &quot;1&quot;],</span>
+</span><span id="TypeParser-984"><a href="#TypeParser-984"><span class="linenos"> 984</span></a><span class="sd">				[&quot;2&quot;, &quot;6.7&quot;, &quot;false&quot;, &quot;2.3&quot;],</span>
+</span><span id="TypeParser-985"><a href="#TypeParser-985"><span class="linenos"> 985</span></a><span class="sd">				[&quot;3&quot;, &quot;8.0&quot;, &quot;&quot;,      &quot;abc&quot;],</span>
+</span><span id="TypeParser-986"><a href="#TypeParser-986"><span class="linenos"> 986</span></a><span class="sd">			]):</span>
+</span><span id="TypeParser-987"><a href="#TypeParser-987"><span class="linenos"> 987</span></a><span class="sd">			assert table == [</span>
+</span><span id="TypeParser-988"><a href="#TypeParser-988"><span class="linenos"> 988</span></a><span class="sd">				[1, 5.,  True,  &quot;1&quot;],</span>
+</span><span id="TypeParser-989"><a href="#TypeParser-989"><span class="linenos"> 989</span></a><span class="sd">				[2, 6.7, False, &quot;2.3&quot;],</span>
+</span><span id="TypeParser-990"><a href="#TypeParser-990"><span class="linenos"> 990</span></a><span class="sd">				[3, 8.,  None,  &quot;abc&quot;],</span>
+</span><span id="TypeParser-991"><a href="#TypeParser-991"><span class="linenos"> 991</span></a><span class="sd">			]</span>
+</span><span id="TypeParser-992"><a href="#TypeParser-992"><span class="linenos"> 992</span></a><span class="sd">			```</span>
+</span><span id="TypeParser-993"><a href="#TypeParser-993"><span class="linenos"> 993</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser-994"><a href="#TypeParser-994"><span class="linenos"> 994</span></a>		<span class="k">return</span> <span class="p">[</span><span class="n">converted_row</span> <span class="k">for</span> <span class="n">converted_row</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">iterate_table</span><span class="p">(</span><span class="n">rows</span><span class="p">)]</span>
+</span><span id="TypeParser-995"><a href="#TypeParser-995"><span class="linenos"> 995</span></a>
+</span><span id="TypeParser-996"><a href="#TypeParser-996"><span class="linenos"> 996</span></a>
+</span><span id="TypeParser-997"><a href="#TypeParser-997"><span class="linenos"> 997</span></a>	<span class="k">def</span> <span class="nf">iterate_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">rows</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]])</span> <span class="o">-&gt;</span> <span class="n">Iterator</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">AnyValue</span><span class="p">]]:</span>
+</span><span id="TypeParser-998"><a href="#TypeParser-998"><span class="linenos"> 998</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser-999"><a href="#TypeParser-999"><span class="linenos"> 999</span></a><span class="sd">			Parse a table of strings for the underlying common type of each column, then convert and yield each row</span>
+</span><span id="TypeParser-1000"><a href="#TypeParser-1000"><span class="linenos">1000</span></a>
+</span><span id="TypeParser-1001"><a href="#TypeParser-1001"><span class="linenos">1001</span></a><span class="sd">			For each column, if the values do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the column. See `parsetypes.reduce_types()` for more information.</span>
+</span><span id="TypeParser-1002"><a href="#TypeParser-1002"><span class="linenos">1002</span></a>
+</span><span id="TypeParser-1003"><a href="#TypeParser-1003"><span class="linenos">1003</span></a><span class="sd">			This is a generator that computes and yields each row one at a time. The function `parse_table()` behaves analogously, except that it computes the entire table and returns it as a list of lists. However, note that although this is a generator, the type to which the value sshould be converted is still determined by `infer_table()`, and so the individual inferred types of every value in the table must be able to fit into memory.</span>
+</span><span id="TypeParser-1004"><a href="#TypeParser-1004"><span class="linenos">1004</span></a>
+</span><span id="TypeParser-1005"><a href="#TypeParser-1005"><span class="linenos">1005</span></a><span class="sd">			Parameters</span>
+</span><span id="TypeParser-1006"><a href="#TypeParser-1006"><span class="linenos">1006</span></a><span class="sd">			----------</span>
+</span><span id="TypeParser-1007"><a href="#TypeParser-1007"><span class="linenos">1007</span></a><span class="sd">			`rows`</span>
+</span><span id="TypeParser-1008"><a href="#TypeParser-1008"><span class="linenos">1008</span></a><span class="sd">			: table of strings to be parsed, in row-major order</span>
+</span><span id="TypeParser-1009"><a href="#TypeParser-1009"><span class="linenos">1009</span></a>
+</span><span id="TypeParser-1010"><a href="#TypeParser-1010"><span class="linenos">1010</span></a><span class="sd">			Yields</span>
+</span><span id="TypeParser-1011"><a href="#TypeParser-1011"><span class="linenos">1011</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser-1012"><a href="#TypeParser-1012"><span class="linenos">1012</span></a><span class="sd">			each row of converted table values</span>
+</span><span id="TypeParser-1013"><a href="#TypeParser-1013"><span class="linenos">1013</span></a>
+</span><span id="TypeParser-1014"><a href="#TypeParser-1014"><span class="linenos">1014</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser-1015"><a href="#TypeParser-1015"><span class="linenos">1015</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser-1016"><a href="#TypeParser-1016"><span class="linenos">1016</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser-1017"><a href="#TypeParser-1017"><span class="linenos">1017</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser-1018"><a href="#TypeParser-1018"><span class="linenos">1018</span></a><span class="sd">			table = parser.iterate_table([</span>
+</span><span id="TypeParser-1019"><a href="#TypeParser-1019"><span class="linenos">1019</span></a><span class="sd">				[&quot;1&quot;,   &quot;true&quot;,  &quot;1&quot;],</span>
+</span><span id="TypeParser-1020"><a href="#TypeParser-1020"><span class="linenos">1020</span></a><span class="sd">				[&quot;2&quot;,   &quot;false&quot;, &quot;2.3&quot;],</span>
+</span><span id="TypeParser-1021"><a href="#TypeParser-1021"><span class="linenos">1021</span></a><span class="sd">				[&quot;3.4&quot;, &quot;2&quot;,     &quot;abc&quot;],</span>
+</span><span id="TypeParser-1022"><a href="#TypeParser-1022"><span class="linenos">1022</span></a><span class="sd">			]):</span>
+</span><span id="TypeParser-1023"><a href="#TypeParser-1023"><span class="linenos">1023</span></a><span class="sd">			assert next(table) == [1.,  1, &quot;1&quot;]</span>
+</span><span id="TypeParser-1024"><a href="#TypeParser-1024"><span class="linenos">1024</span></a><span class="sd">			assert next(table) == [2.,  0, &quot;2.3&quot;]</span>
+</span><span id="TypeParser-1025"><a href="#TypeParser-1025"><span class="linenos">1025</span></a><span class="sd">			assert next(table) == [3.4, 2, &quot;abc&quot;]</span>
+</span><span id="TypeParser-1026"><a href="#TypeParser-1026"><span class="linenos">1026</span></a><span class="sd">			```</span>
+</span><span id="TypeParser-1027"><a href="#TypeParser-1027"><span class="linenos">1027</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser-1028"><a href="#TypeParser-1028"><span class="linenos">1028</span></a>		<span class="n">inferred_types</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">infer_table</span><span class="p">(</span><span class="n">rows</span><span class="p">)</span>
+</span><span id="TypeParser-1029"><a href="#TypeParser-1029"><span class="linenos">1029</span></a>
+</span><span id="TypeParser-1030"><a href="#TypeParser-1030"><span class="linenos">1030</span></a>		<span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">rows</span><span class="p">:</span>
+</span><span id="TypeParser-1031"><a href="#TypeParser-1031"><span class="linenos">1031</span></a>			<span class="k">yield</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">convert</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">inferred</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span><span class="p">,</span> <span class="n">inferred</span> <span class="ow">in</span> <span class="nb">zip</span><span class="p">(</span><span class="n">row</span><span class="p">,</span> <span class="n">inferred_types</span><span class="p">)]</span>
 </span></pre></div>
 
 
     <div class="docstring">
 <p>A parser that can be used to infer the underlying types of data serialised as strings, and to convert them into their original underlying types.</p>
 
 <p>Instances of this class can be configured with different settings for the parser and inferrer. See the constructor for more details about the available options.</p></div>
@@ -2523,49 +2560,170 @@
 <span class="c1"># [float, int, str]</span>
 </code></pre>
 </div></div>
 
 
 
                             </div>
+                            <div id="TypeParser.convert" class="classattr">
+                                        <input id="TypeParser.convert-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+<div class="attr function">
+            
+        <span class="def">def</span>
+        <span class="name">convert</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">value</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">target_type</span><span class="p">:</span> <span class="n">Type</span><span class="p">[</span><span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">,</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">NoneType</span><span class="p">,</span> <span class="n">Nullable</span><span class="p">,</span> <span class="nb">list</span><span class="p">]]</span></span><span class="return-annotation">) -> <span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">,</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">NoneType</span><span class="p">,</span> <span class="nb">list</span><span class="p">]</span>:</span></span>
+
+
+                <label class="view-source-button" for="TypeParser.convert-view-source"><span>View Source</span></label>
+
+    </div>
+    <a class="headerlink" href="#TypeParser.convert"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.convert-832"><a href="#TypeParser.convert-832"><span class="linenos">832</span></a>	<span class="k">def</span> <span class="nf">convert</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">target_type</span><span class="p">:</span> <span class="n">AnyValueType</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">AnyValue</span><span class="p">:</span>
+</span><span id="TypeParser.convert-833"><a href="#TypeParser.convert-833"><span class="linenos">833</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser.convert-834"><a href="#TypeParser.convert-834"><span class="linenos">834</span></a><span class="sd">			Convert a string to the specified target type if possible</span>
+</span><span id="TypeParser.convert-835"><a href="#TypeParser.convert-835"><span class="linenos">835</span></a>
+</span><span id="TypeParser.convert-836"><a href="#TypeParser.convert-836"><span class="linenos">836</span></a><span class="sd">			Valid values for `target_type` include any return value from `infer()`, `infer_series()` and `infer_table()`. To infer and convert the string automatically, use `parse()`, `parse_series()` or `parse_table()` instead.</span>
+</span><span id="TypeParser.convert-837"><a href="#TypeParser.convert-837"><span class="linenos">837</span></a>
+</span><span id="TypeParser.convert-838"><a href="#TypeParser.convert-838"><span class="linenos">838</span></a><span class="sd">			Parameters</span>
+</span><span id="TypeParser.convert-839"><a href="#TypeParser.convert-839"><span class="linenos">839</span></a><span class="sd">			----------</span>
+</span><span id="TypeParser.convert-840"><a href="#TypeParser.convert-840"><span class="linenos">840</span></a><span class="sd">			`value`</span>
+</span><span id="TypeParser.convert-841"><a href="#TypeParser.convert-841"><span class="linenos">841</span></a><span class="sd">			: the string to be converted</span>
+</span><span id="TypeParser.convert-842"><a href="#TypeParser.convert-842"><span class="linenos">842</span></a>
+</span><span id="TypeParser.convert-843"><a href="#TypeParser.convert-843"><span class="linenos">843</span></a><span class="sd">			`target_type`</span>
+</span><span id="TypeParser.convert-844"><a href="#TypeParser.convert-844"><span class="linenos">844</span></a><span class="sd">			: type to which the value should be converted</span>
+</span><span id="TypeParser.convert-845"><a href="#TypeParser.convert-845"><span class="linenos">845</span></a>
+</span><span id="TypeParser.convert-846"><a href="#TypeParser.convert-846"><span class="linenos">846</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser.convert-847"><a href="#TypeParser.convert-847"><span class="linenos">847</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser.convert-848"><a href="#TypeParser.convert-848"><span class="linenos">848</span></a><span class="sd">			converted value</span>
+</span><span id="TypeParser.convert-849"><a href="#TypeParser.convert-849"><span class="linenos">849</span></a>
+</span><span id="TypeParser.convert-850"><a href="#TypeParser.convert-850"><span class="linenos">850</span></a><span class="sd">			Raises</span>
+</span><span id="TypeParser.convert-851"><a href="#TypeParser.convert-851"><span class="linenos">851</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser.convert-852"><a href="#TypeParser.convert-852"><span class="linenos">852</span></a><span class="sd">			`ValueError`</span>
+</span><span id="TypeParser.convert-853"><a href="#TypeParser.convert-853"><span class="linenos">853</span></a><span class="sd">			: if `value` cannot be converted to `target_type`</span>
+</span><span id="TypeParser.convert-854"><a href="#TypeParser.convert-854"><span class="linenos">854</span></a>
+</span><span id="TypeParser.convert-855"><a href="#TypeParser.convert-855"><span class="linenos">855</span></a><span class="sd">			`TypeError`</span>
+</span><span id="TypeParser.convert-856"><a href="#TypeParser.convert-856"><span class="linenos">856</span></a><span class="sd">			: if `target_type` is not a valid type</span>
+</span><span id="TypeParser.convert-857"><a href="#TypeParser.convert-857"><span class="linenos">857</span></a>
+</span><span id="TypeParser.convert-858"><a href="#TypeParser.convert-858"><span class="linenos">858</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser.convert-859"><a href="#TypeParser.convert-859"><span class="linenos">859</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser.convert-860"><a href="#TypeParser.convert-860"><span class="linenos">860</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser.convert-861"><a href="#TypeParser.convert-861"><span class="linenos">861</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser.convert-862"><a href="#TypeParser.convert-862"><span class="linenos">862</span></a><span class="sd">			parser.convert(&quot;true&quot;, bool)  # True</span>
+</span><span id="TypeParser.convert-863"><a href="#TypeParser.convert-863"><span class="linenos">863</span></a><span class="sd">			parser.convert(&quot;2&quot;, int)      # 2</span>
+</span><span id="TypeParser.convert-864"><a href="#TypeParser.convert-864"><span class="linenos">864</span></a><span class="sd">			parser.convert(&quot;2&quot;, float)    # 2.</span>
+</span><span id="TypeParser.convert-865"><a href="#TypeParser.convert-865"><span class="linenos">865</span></a><span class="sd">			```</span>
+</span><span id="TypeParser.convert-866"><a href="#TypeParser.convert-866"><span class="linenos">866</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser.convert-867"><a href="#TypeParser.convert-867"><span class="linenos">867</span></a>		<span class="n">base</span><span class="p">,</span> <span class="n">type_args</span> <span class="o">=</span> <span class="n">_decompose_type</span><span class="p">(</span><span class="n">target_type</span><span class="p">)</span>
+</span><span id="TypeParser.convert-868"><a href="#TypeParser.convert-868"><span class="linenos">868</span></a>		<span class="k">if</span> <span class="n">base</span> <span class="o">==</span> <span class="n">NoneType</span><span class="p">:</span>
+</span><span id="TypeParser.convert-869"><a href="#TypeParser.convert-869"><span class="linenos">869</span></a>			<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_none</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
+</span><span id="TypeParser.convert-870"><a href="#TypeParser.convert-870"><span class="linenos">870</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="TypeParser.convert-871"><a href="#TypeParser.convert-871"><span class="linenos">871</span></a>			<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_bool</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
+</span><span id="TypeParser.convert-872"><a href="#TypeParser.convert-872"><span class="linenos">872</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="TypeParser.convert-873"><a href="#TypeParser.convert-873"><span class="linenos">873</span></a>			<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_int</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
+</span><span id="TypeParser.convert-874"><a href="#TypeParser.convert-874"><span class="linenos">874</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="n">Decimal</span><span class="p">:</span>
+</span><span id="TypeParser.convert-875"><a href="#TypeParser.convert-875"><span class="linenos">875</span></a>			<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_decimal</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
+</span><span id="TypeParser.convert-876"><a href="#TypeParser.convert-876"><span class="linenos">876</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">float</span><span class="p">:</span>
+</span><span id="TypeParser.convert-877"><a href="#TypeParser.convert-877"><span class="linenos">877</span></a>			<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">parse_float</span><span class="p">(</span><span class="n">value</span><span class="p">)</span>
+</span><span id="TypeParser.convert-878"><a href="#TypeParser.convert-878"><span class="linenos">878</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="TypeParser.convert-879"><a href="#TypeParser.convert-879"><span class="linenos">879</span></a>			<span class="k">return</span> <span class="n">value</span>
+</span><span id="TypeParser.convert-880"><a href="#TypeParser.convert-880"><span class="linenos">880</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="n">Nullable</span><span class="p">:</span>
+</span><span id="TypeParser.convert-881"><a href="#TypeParser.convert-881"><span class="linenos">881</span></a>			<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_none</span><span class="p">(</span><span class="n">value</span><span class="p">):</span>
+</span><span id="TypeParser.convert-882"><a href="#TypeParser.convert-882"><span class="linenos">882</span></a>				<span class="k">return</span> <span class="kc">None</span>
+</span><span id="TypeParser.convert-883"><a href="#TypeParser.convert-883"><span class="linenos">883</span></a>			<span class="k">else</span><span class="p">:</span>
+</span><span id="TypeParser.convert-884"><a href="#TypeParser.convert-884"><span class="linenos">884</span></a>				<span class="k">if</span> <span class="n">type_args</span> <span class="ow">is</span> <span class="ow">not</span>  <span class="kc">None</span> <span class="ow">and</span> <span class="nb">len</span><span class="p">(</span><span class="n">type_args</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span> <span class="ow">and</span> <span class="n">type_args</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">!=</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="TypeParser.convert-885"><a href="#TypeParser.convert-885"><span class="linenos">885</span></a>					<span class="n">inner_type</span> <span class="o">=</span> <span class="n">type_args</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="TypeParser.convert-886"><a href="#TypeParser.convert-886"><span class="linenos">886</span></a>					<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">convert</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">inner_type</span><span class="p">)</span>
+</span><span id="TypeParser.convert-887"><a href="#TypeParser.convert-887"><span class="linenos">887</span></a>				<span class="k">else</span><span class="p">:</span>
+</span><span id="TypeParser.convert-888"><a href="#TypeParser.convert-888"><span class="linenos">888</span></a>					<span class="k">return</span> <span class="n">value</span>
+</span><span id="TypeParser.convert-889"><a href="#TypeParser.convert-889"><span class="linenos">889</span></a>		<span class="k">elif</span> <span class="n">base</span> <span class="o">==</span> <span class="nb">list</span><span class="p">:</span>
+</span><span id="TypeParser.convert-890"><a href="#TypeParser.convert-890"><span class="linenos">890</span></a>			<span class="n">subvalues</span> <span class="o">=</span> <span class="n">value</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">list_delimiter</span><span class="p">)</span>
+</span><span id="TypeParser.convert-891"><a href="#TypeParser.convert-891"><span class="linenos">891</span></a>			<span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">trim</span><span class="p">:</span>
+</span><span id="TypeParser.convert-892"><a href="#TypeParser.convert-892"><span class="linenos">892</span></a>				<span class="n">subvalues</span> <span class="o">=</span> <span class="p">[</span><span class="n">subvalue</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="k">for</span> <span class="n">subvalue</span> <span class="ow">in</span> <span class="n">subvalues</span><span class="p">]</span>
+</span><span id="TypeParser.convert-893"><a href="#TypeParser.convert-893"><span class="linenos">893</span></a>			<span class="k">if</span> <span class="n">type_args</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span> <span class="ow">and</span> <span class="nb">len</span><span class="p">(</span><span class="n">type_args</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span> <span class="ow">and</span> <span class="n">type_args</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">!=</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="TypeParser.convert-894"><a href="#TypeParser.convert-894"><span class="linenos">894</span></a>				<span class="n">subtype</span> <span class="o">=</span> <span class="n">type_args</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="TypeParser.convert-895"><a href="#TypeParser.convert-895"><span class="linenos">895</span></a>				<span class="k">return</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">convert</span><span class="p">(</span><span class="n">subvalue</span><span class="p">,</span> <span class="n">subtype</span><span class="p">)</span> <span class="k">for</span> <span class="n">subvalue</span> <span class="ow">in</span> <span class="n">subvalues</span><span class="p">]</span>
+</span><span id="TypeParser.convert-896"><a href="#TypeParser.convert-896"><span class="linenos">896</span></a>			<span class="k">else</span><span class="p">:</span>
+</span><span id="TypeParser.convert-897"><a href="#TypeParser.convert-897"><span class="linenos">897</span></a>				<span class="k">return</span> <span class="n">subvalues</span>
+</span><span id="TypeParser.convert-898"><a href="#TypeParser.convert-898"><span class="linenos">898</span></a>		<span class="k">else</span><span class="p">:</span>
+</span><span id="TypeParser.convert-899"><a href="#TypeParser.convert-899"><span class="linenos">899</span></a>			<span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;cannot convert to type: </span><span class="si">{</span><span class="n">target_type</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span></pre></div>
+
+
+    <div class="docstring">
+<p>Convert a string to the specified target type if possible</p>
+
+<p>Valid values for <code>target_type</code> include any return value from <code><a href="#TypeParser.infer">infer()</a></code>, <code><a href="#TypeParser.infer_series">infer_series()</a></code> and <code><a href="#TypeParser.infer_table">infer_table()</a></code>. To infer and convert the string automatically, use <code><a href="#TypeParser.parse">parse()</a></code>, <code><a href="#TypeParser.parse_series">parse_series()</a></code> or <code><a href="#TypeParser.parse_table">parse_table()</a></code> instead.</p>
+
+<h2 id="parameters">Parameters</h2>
+
+<p><code>value</code>
+: the string to be converted</p>
+
+<p><code>target_type</code>
+: type to which the value should be converted</p>
+
+<h2 id="returns">Returns</h2>
+
+<p>converted value</p>
+
+<h2 id="raises">Raises</h2>
+
+<p><code>ValueError</code>
+: if <code>value</code> cannot be converted to <code>target_type</code></p>
+
+<p><code>TypeError</code>
+: if <code>target_type</code> is not a valid type</p>
+
+<h2 id="examples">Examples</h2>
+
+<div class="pdoc-code codehilite">
+<pre><span></span><code><span class="n">parser</span> <span class="o">=</span> <span class="n">TypeParser</span><span class="p">()</span>
+<span class="n">parser</span><span class="o">.</span><span class="n">convert</span><span class="p">(</span><span class="s2">&quot;true&quot;</span><span class="p">,</span> <span class="nb">bool</span><span class="p">)</span>  <span class="c1"># True</span>
+<span class="n">parser</span><span class="o">.</span><span class="n">convert</span><span class="p">(</span><span class="s2">&quot;2&quot;</span><span class="p">,</span> <span class="nb">int</span><span class="p">)</span>      <span class="c1"># 2</span>
+<span class="n">parser</span><span class="o">.</span><span class="n">convert</span><span class="p">(</span><span class="s2">&quot;2&quot;</span><span class="p">,</span> <span class="nb">float</span><span class="p">)</span>    <span class="c1"># 2.</span>
+</code></pre>
+</div></div>
+
+
+
+                            </div>
                             <div id="TypeParser.parse" class="classattr">
                                         <input id="TypeParser.parse-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
         <span class="name">parse</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">value</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">,</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">NoneType</span><span class="p">,</span> <span class="nb">list</span><span class="p">]</span>:</span></span>
 
 
                 <label class="view-source-button" for="TypeParser.parse-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#TypeParser.parse"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.parse-868"><a href="#TypeParser.parse-868"><span class="linenos">868</span></a>	<span class="k">def</span> <span class="nf">parse</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">AnyValue</span><span class="p">:</span>
-</span><span id="TypeParser.parse-869"><a href="#TypeParser.parse-869"><span class="linenos">869</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser.parse-870"><a href="#TypeParser.parse-870"><span class="linenos">870</span></a><span class="sd">			Parse a string and convert it to its underlying type</span>
-</span><span id="TypeParser.parse-871"><a href="#TypeParser.parse-871"><span class="linenos">871</span></a>
-</span><span id="TypeParser.parse-872"><a href="#TypeParser.parse-872"><span class="linenos">872</span></a><span class="sd">			Parameters</span>
-</span><span id="TypeParser.parse-873"><a href="#TypeParser.parse-873"><span class="linenos">873</span></a><span class="sd">			----------</span>
-</span><span id="TypeParser.parse-874"><a href="#TypeParser.parse-874"><span class="linenos">874</span></a><span class="sd">			`value`</span>
-</span><span id="TypeParser.parse-875"><a href="#TypeParser.parse-875"><span class="linenos">875</span></a><span class="sd">			: the string to be parsed</span>
-</span><span id="TypeParser.parse-876"><a href="#TypeParser.parse-876"><span class="linenos">876</span></a>
-</span><span id="TypeParser.parse-877"><a href="#TypeParser.parse-877"><span class="linenos">877</span></a><span class="sd">			Returns</span>
-</span><span id="TypeParser.parse-878"><a href="#TypeParser.parse-878"><span class="linenos">878</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser.parse-879"><a href="#TypeParser.parse-879"><span class="linenos">879</span></a><span class="sd">			converted value</span>
-</span><span id="TypeParser.parse-880"><a href="#TypeParser.parse-880"><span class="linenos">880</span></a>
-</span><span id="TypeParser.parse-881"><a href="#TypeParser.parse-881"><span class="linenos">881</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser.parse-882"><a href="#TypeParser.parse-882"><span class="linenos">882</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser.parse-883"><a href="#TypeParser.parse-883"><span class="linenos">883</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser.parse-884"><a href="#TypeParser.parse-884"><span class="linenos">884</span></a><span class="sd">			parser = TypeParser()</span>
-</span><span id="TypeParser.parse-885"><a href="#TypeParser.parse-885"><span class="linenos">885</span></a><span class="sd">			parser.parse(&quot;true&quot;)  # True</span>
-</span><span id="TypeParser.parse-886"><a href="#TypeParser.parse-886"><span class="linenos">886</span></a><span class="sd">			parser.parse(&quot;2.0&quot;)   # 2.</span>
-</span><span id="TypeParser.parse-887"><a href="#TypeParser.parse-887"><span class="linenos">887</span></a><span class="sd">			parser.parse(&quot;abc&quot;)   # &quot;abc&quot;</span>
-</span><span id="TypeParser.parse-888"><a href="#TypeParser.parse-888"><span class="linenos">888</span></a><span class="sd">			```</span>
-</span><span id="TypeParser.parse-889"><a href="#TypeParser.parse-889"><span class="linenos">889</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser.parse-890"><a href="#TypeParser.parse-890"><span class="linenos">890</span></a>		<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_convert</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">value</span><span class="p">))</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.parse-902"><a href="#TypeParser.parse-902"><span class="linenos">902</span></a>	<span class="k">def</span> <span class="nf">parse</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">AnyValue</span><span class="p">:</span>
+</span><span id="TypeParser.parse-903"><a href="#TypeParser.parse-903"><span class="linenos">903</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser.parse-904"><a href="#TypeParser.parse-904"><span class="linenos">904</span></a><span class="sd">			Parse a string and convert it to its underlying type</span>
+</span><span id="TypeParser.parse-905"><a href="#TypeParser.parse-905"><span class="linenos">905</span></a>
+</span><span id="TypeParser.parse-906"><a href="#TypeParser.parse-906"><span class="linenos">906</span></a><span class="sd">			Parameters</span>
+</span><span id="TypeParser.parse-907"><a href="#TypeParser.parse-907"><span class="linenos">907</span></a><span class="sd">			----------</span>
+</span><span id="TypeParser.parse-908"><a href="#TypeParser.parse-908"><span class="linenos">908</span></a><span class="sd">			`value`</span>
+</span><span id="TypeParser.parse-909"><a href="#TypeParser.parse-909"><span class="linenos">909</span></a><span class="sd">			: the string to be parsed</span>
+</span><span id="TypeParser.parse-910"><a href="#TypeParser.parse-910"><span class="linenos">910</span></a>
+</span><span id="TypeParser.parse-911"><a href="#TypeParser.parse-911"><span class="linenos">911</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser.parse-912"><a href="#TypeParser.parse-912"><span class="linenos">912</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser.parse-913"><a href="#TypeParser.parse-913"><span class="linenos">913</span></a><span class="sd">			converted value</span>
+</span><span id="TypeParser.parse-914"><a href="#TypeParser.parse-914"><span class="linenos">914</span></a>
+</span><span id="TypeParser.parse-915"><a href="#TypeParser.parse-915"><span class="linenos">915</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser.parse-916"><a href="#TypeParser.parse-916"><span class="linenos">916</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser.parse-917"><a href="#TypeParser.parse-917"><span class="linenos">917</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser.parse-918"><a href="#TypeParser.parse-918"><span class="linenos">918</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser.parse-919"><a href="#TypeParser.parse-919"><span class="linenos">919</span></a><span class="sd">			parser.parse(&quot;true&quot;)  # True</span>
+</span><span id="TypeParser.parse-920"><a href="#TypeParser.parse-920"><span class="linenos">920</span></a><span class="sd">			parser.parse(&quot;2.0&quot;)   # 2.</span>
+</span><span id="TypeParser.parse-921"><a href="#TypeParser.parse-921"><span class="linenos">921</span></a><span class="sd">			parser.parse(&quot;abc&quot;)   # &quot;abc&quot;</span>
+</span><span id="TypeParser.parse-922"><a href="#TypeParser.parse-922"><span class="linenos">922</span></a><span class="sd">			```</span>
+</span><span id="TypeParser.parse-923"><a href="#TypeParser.parse-923"><span class="linenos">923</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser.parse-924"><a href="#TypeParser.parse-924"><span class="linenos">924</span></a>		<span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">convert</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">value</span><span class="p">))</span>
 </span></pre></div>
 
 
     <div class="docstring">
 <p>Parse a string and convert it to its underlying type</p>
 
 <h2 id="parameters">Parameters</h2>
@@ -2598,41 +2756,41 @@
         <span class="name">parse_series</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">values</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span></span><span class="return-annotation">) -> <span class="nb">list</span><span class="p">[</span><span class="n">typing</span><span class="o">.</span><span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">,</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">NoneType</span><span class="p">,</span> <span class="nb">list</span><span class="p">]]</span>:</span></span>
 
 
                 <label class="view-source-button" for="TypeParser.parse_series-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#TypeParser.parse_series"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.parse_series-893"><a href="#TypeParser.parse_series-893"><span class="linenos">893</span></a>	<span class="k">def</span> <span class="nf">parse_series</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">AnyValue</span><span class="p">]:</span>
-</span><span id="TypeParser.parse_series-894"><a href="#TypeParser.parse_series-894"><span class="linenos">894</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser.parse_series-895"><a href="#TypeParser.parse_series-895"><span class="linenos">895</span></a><span class="sd">			Parse a series of strings and convert them to their underlying common type</span>
-</span><span id="TypeParser.parse_series-896"><a href="#TypeParser.parse_series-896"><span class="linenos">896</span></a>
-</span><span id="TypeParser.parse_series-897"><a href="#TypeParser.parse_series-897"><span class="linenos">897</span></a><span class="sd">			If the values in the series do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the series. See `parsetypes.reduce_types()` for more information.</span>
-</span><span id="TypeParser.parse_series-898"><a href="#TypeParser.parse_series-898"><span class="linenos">898</span></a>
-</span><span id="TypeParser.parse_series-899"><a href="#TypeParser.parse_series-899"><span class="linenos">899</span></a><span class="sd">			Parameters</span>
-</span><span id="TypeParser.parse_series-900"><a href="#TypeParser.parse_series-900"><span class="linenos">900</span></a><span class="sd">			----------</span>
-</span><span id="TypeParser.parse_series-901"><a href="#TypeParser.parse_series-901"><span class="linenos">901</span></a><span class="sd">			`values`</span>
-</span><span id="TypeParser.parse_series-902"><a href="#TypeParser.parse_series-902"><span class="linenos">902</span></a><span class="sd">			: series of strings to be parsed</span>
-</span><span id="TypeParser.parse_series-903"><a href="#TypeParser.parse_series-903"><span class="linenos">903</span></a>
-</span><span id="TypeParser.parse_series-904"><a href="#TypeParser.parse_series-904"><span class="linenos">904</span></a><span class="sd">			Returns</span>
-</span><span id="TypeParser.parse_series-905"><a href="#TypeParser.parse_series-905"><span class="linenos">905</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser.parse_series-906"><a href="#TypeParser.parse_series-906"><span class="linenos">906</span></a><span class="sd">			converted values</span>
-</span><span id="TypeParser.parse_series-907"><a href="#TypeParser.parse_series-907"><span class="linenos">907</span></a>
-</span><span id="TypeParser.parse_series-908"><a href="#TypeParser.parse_series-908"><span class="linenos">908</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser.parse_series-909"><a href="#TypeParser.parse_series-909"><span class="linenos">909</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser.parse_series-910"><a href="#TypeParser.parse_series-910"><span class="linenos">910</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser.parse_series-911"><a href="#TypeParser.parse_series-911"><span class="linenos">911</span></a><span class="sd">			parser = TypeParser()</span>
-</span><span id="TypeParser.parse_series-912"><a href="#TypeParser.parse_series-912"><span class="linenos">912</span></a><span class="sd">			parser.parse_series([&quot;1&quot;, &quot;2&quot;, &quot;3&quot;])        # [1, 2, 3]</span>
-</span><span id="TypeParser.parse_series-913"><a href="#TypeParser.parse_series-913"><span class="linenos">913</span></a><span class="sd">			parser.parse_series([&quot;5&quot;, &quot;6.7&quot;, &quot;8.&quot;])     # [5., 6.7, 8.]</span>
-</span><span id="TypeParser.parse_series-914"><a href="#TypeParser.parse_series-914"><span class="linenos">914</span></a><span class="sd">			parser.parse_series([&quot;true&quot;, &quot;false&quot;, &quot;&quot;])  # [True, False, None]</span>
-</span><span id="TypeParser.parse_series-915"><a href="#TypeParser.parse_series-915"><span class="linenos">915</span></a><span class="sd">			parser.parse_series([&quot;1&quot;, &quot;2.3&quot;, &quot;abc&quot;])    # [&quot;1&quot;, &quot;2.3&quot;, &quot;abc&quot;]</span>
-</span><span id="TypeParser.parse_series-916"><a href="#TypeParser.parse_series-916"><span class="linenos">916</span></a><span class="sd">			```</span>
-</span><span id="TypeParser.parse_series-917"><a href="#TypeParser.parse_series-917"><span class="linenos">917</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser.parse_series-918"><a href="#TypeParser.parse_series-918"><span class="linenos">918</span></a>		<span class="n">inferred</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">infer_series</span><span class="p">(</span><span class="n">values</span><span class="p">)</span>
-</span><span id="TypeParser.parse_series-919"><a href="#TypeParser.parse_series-919"><span class="linenos">919</span></a>		<span class="k">return</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">_convert</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">inferred</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">values</span><span class="p">]</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.parse_series-927"><a href="#TypeParser.parse_series-927"><span class="linenos">927</span></a>	<span class="k">def</span> <span class="nf">parse_series</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">AnyValue</span><span class="p">]:</span>
+</span><span id="TypeParser.parse_series-928"><a href="#TypeParser.parse_series-928"><span class="linenos">928</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser.parse_series-929"><a href="#TypeParser.parse_series-929"><span class="linenos">929</span></a><span class="sd">			Parse a series of strings and convert them to their underlying common type</span>
+</span><span id="TypeParser.parse_series-930"><a href="#TypeParser.parse_series-930"><span class="linenos">930</span></a>
+</span><span id="TypeParser.parse_series-931"><a href="#TypeParser.parse_series-931"><span class="linenos">931</span></a><span class="sd">			If the values in the series do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the series. See `parsetypes.reduce_types()` for more information.</span>
+</span><span id="TypeParser.parse_series-932"><a href="#TypeParser.parse_series-932"><span class="linenos">932</span></a>
+</span><span id="TypeParser.parse_series-933"><a href="#TypeParser.parse_series-933"><span class="linenos">933</span></a><span class="sd">			Parameters</span>
+</span><span id="TypeParser.parse_series-934"><a href="#TypeParser.parse_series-934"><span class="linenos">934</span></a><span class="sd">			----------</span>
+</span><span id="TypeParser.parse_series-935"><a href="#TypeParser.parse_series-935"><span class="linenos">935</span></a><span class="sd">			`values`</span>
+</span><span id="TypeParser.parse_series-936"><a href="#TypeParser.parse_series-936"><span class="linenos">936</span></a><span class="sd">			: series of strings to be parsed</span>
+</span><span id="TypeParser.parse_series-937"><a href="#TypeParser.parse_series-937"><span class="linenos">937</span></a>
+</span><span id="TypeParser.parse_series-938"><a href="#TypeParser.parse_series-938"><span class="linenos">938</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser.parse_series-939"><a href="#TypeParser.parse_series-939"><span class="linenos">939</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser.parse_series-940"><a href="#TypeParser.parse_series-940"><span class="linenos">940</span></a><span class="sd">			converted values</span>
+</span><span id="TypeParser.parse_series-941"><a href="#TypeParser.parse_series-941"><span class="linenos">941</span></a>
+</span><span id="TypeParser.parse_series-942"><a href="#TypeParser.parse_series-942"><span class="linenos">942</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser.parse_series-943"><a href="#TypeParser.parse_series-943"><span class="linenos">943</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser.parse_series-944"><a href="#TypeParser.parse_series-944"><span class="linenos">944</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser.parse_series-945"><a href="#TypeParser.parse_series-945"><span class="linenos">945</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser.parse_series-946"><a href="#TypeParser.parse_series-946"><span class="linenos">946</span></a><span class="sd">			parser.parse_series([&quot;1&quot;, &quot;2&quot;, &quot;3&quot;])        # [1, 2, 3]</span>
+</span><span id="TypeParser.parse_series-947"><a href="#TypeParser.parse_series-947"><span class="linenos">947</span></a><span class="sd">			parser.parse_series([&quot;5&quot;, &quot;6.7&quot;, &quot;8.&quot;])     # [5., 6.7, 8.]</span>
+</span><span id="TypeParser.parse_series-948"><a href="#TypeParser.parse_series-948"><span class="linenos">948</span></a><span class="sd">			parser.parse_series([&quot;true&quot;, &quot;false&quot;, &quot;&quot;])  # [True, False, None]</span>
+</span><span id="TypeParser.parse_series-949"><a href="#TypeParser.parse_series-949"><span class="linenos">949</span></a><span class="sd">			parser.parse_series([&quot;1&quot;, &quot;2.3&quot;, &quot;abc&quot;])    # [&quot;1&quot;, &quot;2.3&quot;, &quot;abc&quot;]</span>
+</span><span id="TypeParser.parse_series-950"><a href="#TypeParser.parse_series-950"><span class="linenos">950</span></a><span class="sd">			```</span>
+</span><span id="TypeParser.parse_series-951"><a href="#TypeParser.parse_series-951"><span class="linenos">951</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser.parse_series-952"><a href="#TypeParser.parse_series-952"><span class="linenos">952</span></a>		<span class="n">inferred</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">infer_series</span><span class="p">(</span><span class="n">values</span><span class="p">)</span>
+</span><span id="TypeParser.parse_series-953"><a href="#TypeParser.parse_series-953"><span class="linenos">953</span></a>		<span class="k">return</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">convert</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">inferred</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">values</span><span class="p">]</span>
 </span></pre></div>
 
 
     <div class="docstring">
 <p>Parse a series of strings and convert them to their underlying common type</p>
 
 <p>If the values in the series do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the series. See <code><a href="#reduce_types">parsetypes.reduce_types()</a></code> for more information.</p>
@@ -2668,53 +2826,53 @@
         <span class="name">parse_table</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">rows</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]]</span></span><span class="return-annotation">) -> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">typing</span><span class="o">.</span><span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">,</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">NoneType</span><span class="p">,</span> <span class="nb">list</span><span class="p">]]]</span>:</span></span>
 
 
                 <label class="view-source-button" for="TypeParser.parse_table-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#TypeParser.parse_table"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.parse_table-922"><a href="#TypeParser.parse_table-922"><span class="linenos">922</span></a>	<span class="k">def</span> <span class="nf">parse_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">rows</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">AnyValue</span><span class="p">]]:</span>
-</span><span id="TypeParser.parse_table-923"><a href="#TypeParser.parse_table-923"><span class="linenos">923</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser.parse_table-924"><a href="#TypeParser.parse_table-924"><span class="linenos">924</span></a><span class="sd">			Parse a table of strings and convert them to the underlying common type of each column</span>
-</span><span id="TypeParser.parse_table-925"><a href="#TypeParser.parse_table-925"><span class="linenos">925</span></a>
-</span><span id="TypeParser.parse_table-926"><a href="#TypeParser.parse_table-926"><span class="linenos">926</span></a><span class="sd">			For each column, if the values do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the column. See `parsetypes.reduce_types()` for more information.</span>
-</span><span id="TypeParser.parse_table-927"><a href="#TypeParser.parse_table-927"><span class="linenos">927</span></a>
-</span><span id="TypeParser.parse_table-928"><a href="#TypeParser.parse_table-928"><span class="linenos">928</span></a><span class="sd">			Note that the type to which the values should be converted is determined by `infer_table()`, and so the individual inferred types of every value in the table must be able to fit into memory.</span>
-</span><span id="TypeParser.parse_table-929"><a href="#TypeParser.parse_table-929"><span class="linenos">929</span></a>
-</span><span id="TypeParser.parse_table-930"><a href="#TypeParser.parse_table-930"><span class="linenos">930</span></a><span class="sd">			This is a function that computes the entire table and returns it all at once. The generator `iterate_table()` behaves analogously, except that it computes and yields each row one at a time.</span>
-</span><span id="TypeParser.parse_table-931"><a href="#TypeParser.parse_table-931"><span class="linenos">931</span></a>
-</span><span id="TypeParser.parse_table-932"><a href="#TypeParser.parse_table-932"><span class="linenos">932</span></a><span class="sd">			Parameters</span>
-</span><span id="TypeParser.parse_table-933"><a href="#TypeParser.parse_table-933"><span class="linenos">933</span></a><span class="sd">			----------</span>
-</span><span id="TypeParser.parse_table-934"><a href="#TypeParser.parse_table-934"><span class="linenos">934</span></a><span class="sd">			`rows`</span>
-</span><span id="TypeParser.parse_table-935"><a href="#TypeParser.parse_table-935"><span class="linenos">935</span></a><span class="sd">			: table of strings to be parsed, in row-major order</span>
-</span><span id="TypeParser.parse_table-936"><a href="#TypeParser.parse_table-936"><span class="linenos">936</span></a>
-</span><span id="TypeParser.parse_table-937"><a href="#TypeParser.parse_table-937"><span class="linenos">937</span></a><span class="sd">			`iterator`</span>
-</span><span id="TypeParser.parse_table-938"><a href="#TypeParser.parse_table-938"><span class="linenos">938</span></a><span class="sd">			: whether the parsed values should be yielded as an iterator. If False, which is the default, the entire table is computed and returned as a list of lists. If True, this function behaves as a generator, and the rows of the table are computed and yielded one at a time. However, note that even when set to True, the type inference requires that inferred type of each individual value must all be able to fit into memory at once.</span>
-</span><span id="TypeParser.parse_table-939"><a href="#TypeParser.parse_table-939"><span class="linenos">939</span></a>
-</span><span id="TypeParser.parse_table-940"><a href="#TypeParser.parse_table-940"><span class="linenos">940</span></a><span class="sd">			Returns</span>
-</span><span id="TypeParser.parse_table-941"><a href="#TypeParser.parse_table-941"><span class="linenos">941</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser.parse_table-942"><a href="#TypeParser.parse_table-942"><span class="linenos">942</span></a><span class="sd">			converted table of values, in row-major order</span>
-</span><span id="TypeParser.parse_table-943"><a href="#TypeParser.parse_table-943"><span class="linenos">943</span></a>
-</span><span id="TypeParser.parse_table-944"><a href="#TypeParser.parse_table-944"><span class="linenos">944</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser.parse_table-945"><a href="#TypeParser.parse_table-945"><span class="linenos">945</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser.parse_table-946"><a href="#TypeParser.parse_table-946"><span class="linenos">946</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser.parse_table-947"><a href="#TypeParser.parse_table-947"><span class="linenos">947</span></a><span class="sd">			parser = TypeParser()</span>
-</span><span id="TypeParser.parse_table-948"><a href="#TypeParser.parse_table-948"><span class="linenos">948</span></a><span class="sd">			table = parser.parse_table([</span>
-</span><span id="TypeParser.parse_table-949"><a href="#TypeParser.parse_table-949"><span class="linenos">949</span></a><span class="sd">				[&quot;1&quot;, &quot;5&quot;,   &quot;true&quot;,  &quot;1&quot;],</span>
-</span><span id="TypeParser.parse_table-950"><a href="#TypeParser.parse_table-950"><span class="linenos">950</span></a><span class="sd">				[&quot;2&quot;, &quot;6.7&quot;, &quot;false&quot;, &quot;2.3&quot;],</span>
-</span><span id="TypeParser.parse_table-951"><a href="#TypeParser.parse_table-951"><span class="linenos">951</span></a><span class="sd">				[&quot;3&quot;, &quot;8.0&quot;, &quot;&quot;,      &quot;abc&quot;],</span>
-</span><span id="TypeParser.parse_table-952"><a href="#TypeParser.parse_table-952"><span class="linenos">952</span></a><span class="sd">			]):</span>
-</span><span id="TypeParser.parse_table-953"><a href="#TypeParser.parse_table-953"><span class="linenos">953</span></a><span class="sd">			assert table == [</span>
-</span><span id="TypeParser.parse_table-954"><a href="#TypeParser.parse_table-954"><span class="linenos">954</span></a><span class="sd">				[1, 5.,  True,  &quot;1&quot;],</span>
-</span><span id="TypeParser.parse_table-955"><a href="#TypeParser.parse_table-955"><span class="linenos">955</span></a><span class="sd">				[2, 6.7, False, &quot;2.3&quot;],</span>
-</span><span id="TypeParser.parse_table-956"><a href="#TypeParser.parse_table-956"><span class="linenos">956</span></a><span class="sd">				[3, 8.,  None,  &quot;abc&quot;],</span>
-</span><span id="TypeParser.parse_table-957"><a href="#TypeParser.parse_table-957"><span class="linenos">957</span></a><span class="sd">			]</span>
-</span><span id="TypeParser.parse_table-958"><a href="#TypeParser.parse_table-958"><span class="linenos">958</span></a><span class="sd">			```</span>
-</span><span id="TypeParser.parse_table-959"><a href="#TypeParser.parse_table-959"><span class="linenos">959</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser.parse_table-960"><a href="#TypeParser.parse_table-960"><span class="linenos">960</span></a>		<span class="k">return</span> <span class="p">[</span><span class="n">converted_row</span> <span class="k">for</span> <span class="n">converted_row</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">iterate_table</span><span class="p">(</span><span class="n">rows</span><span class="p">)]</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.parse_table-956"><a href="#TypeParser.parse_table-956"><span class="linenos">956</span></a>	<span class="k">def</span> <span class="nf">parse_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">rows</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">AnyValue</span><span class="p">]]:</span>
+</span><span id="TypeParser.parse_table-957"><a href="#TypeParser.parse_table-957"><span class="linenos">957</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser.parse_table-958"><a href="#TypeParser.parse_table-958"><span class="linenos">958</span></a><span class="sd">			Parse a table of strings and convert them to the underlying common type of each column</span>
+</span><span id="TypeParser.parse_table-959"><a href="#TypeParser.parse_table-959"><span class="linenos">959</span></a>
+</span><span id="TypeParser.parse_table-960"><a href="#TypeParser.parse_table-960"><span class="linenos">960</span></a><span class="sd">			For each column, if the values do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the column. See `parsetypes.reduce_types()` for more information.</span>
+</span><span id="TypeParser.parse_table-961"><a href="#TypeParser.parse_table-961"><span class="linenos">961</span></a>
+</span><span id="TypeParser.parse_table-962"><a href="#TypeParser.parse_table-962"><span class="linenos">962</span></a><span class="sd">			Note that the type to which the values should be converted is determined by `infer_table()`, and so the individual inferred types of every value in the table must be able to fit into memory.</span>
+</span><span id="TypeParser.parse_table-963"><a href="#TypeParser.parse_table-963"><span class="linenos">963</span></a>
+</span><span id="TypeParser.parse_table-964"><a href="#TypeParser.parse_table-964"><span class="linenos">964</span></a><span class="sd">			This is a function that computes the entire table and returns it all at once. The generator `iterate_table()` behaves analogously, except that it computes and yields each row one at a time.</span>
+</span><span id="TypeParser.parse_table-965"><a href="#TypeParser.parse_table-965"><span class="linenos">965</span></a>
+</span><span id="TypeParser.parse_table-966"><a href="#TypeParser.parse_table-966"><span class="linenos">966</span></a><span class="sd">			Parameters</span>
+</span><span id="TypeParser.parse_table-967"><a href="#TypeParser.parse_table-967"><span class="linenos">967</span></a><span class="sd">			----------</span>
+</span><span id="TypeParser.parse_table-968"><a href="#TypeParser.parse_table-968"><span class="linenos">968</span></a><span class="sd">			`rows`</span>
+</span><span id="TypeParser.parse_table-969"><a href="#TypeParser.parse_table-969"><span class="linenos">969</span></a><span class="sd">			: table of strings to be parsed, in row-major order</span>
+</span><span id="TypeParser.parse_table-970"><a href="#TypeParser.parse_table-970"><span class="linenos">970</span></a>
+</span><span id="TypeParser.parse_table-971"><a href="#TypeParser.parse_table-971"><span class="linenos">971</span></a><span class="sd">			`iterator`</span>
+</span><span id="TypeParser.parse_table-972"><a href="#TypeParser.parse_table-972"><span class="linenos">972</span></a><span class="sd">			: whether the parsed values should be yielded as an iterator. If False, which is the default, the entire table is computed and returned as a list of lists. If True, this function behaves as a generator, and the rows of the table are computed and yielded one at a time. However, note that even when set to True, the type inference requires that inferred type of each individual value must all be able to fit into memory at once.</span>
+</span><span id="TypeParser.parse_table-973"><a href="#TypeParser.parse_table-973"><span class="linenos">973</span></a>
+</span><span id="TypeParser.parse_table-974"><a href="#TypeParser.parse_table-974"><span class="linenos">974</span></a><span class="sd">			Returns</span>
+</span><span id="TypeParser.parse_table-975"><a href="#TypeParser.parse_table-975"><span class="linenos">975</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser.parse_table-976"><a href="#TypeParser.parse_table-976"><span class="linenos">976</span></a><span class="sd">			converted table of values, in row-major order</span>
+</span><span id="TypeParser.parse_table-977"><a href="#TypeParser.parse_table-977"><span class="linenos">977</span></a>
+</span><span id="TypeParser.parse_table-978"><a href="#TypeParser.parse_table-978"><span class="linenos">978</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser.parse_table-979"><a href="#TypeParser.parse_table-979"><span class="linenos">979</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser.parse_table-980"><a href="#TypeParser.parse_table-980"><span class="linenos">980</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser.parse_table-981"><a href="#TypeParser.parse_table-981"><span class="linenos">981</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser.parse_table-982"><a href="#TypeParser.parse_table-982"><span class="linenos">982</span></a><span class="sd">			table = parser.parse_table([</span>
+</span><span id="TypeParser.parse_table-983"><a href="#TypeParser.parse_table-983"><span class="linenos">983</span></a><span class="sd">				[&quot;1&quot;, &quot;5&quot;,   &quot;true&quot;,  &quot;1&quot;],</span>
+</span><span id="TypeParser.parse_table-984"><a href="#TypeParser.parse_table-984"><span class="linenos">984</span></a><span class="sd">				[&quot;2&quot;, &quot;6.7&quot;, &quot;false&quot;, &quot;2.3&quot;],</span>
+</span><span id="TypeParser.parse_table-985"><a href="#TypeParser.parse_table-985"><span class="linenos">985</span></a><span class="sd">				[&quot;3&quot;, &quot;8.0&quot;, &quot;&quot;,      &quot;abc&quot;],</span>
+</span><span id="TypeParser.parse_table-986"><a href="#TypeParser.parse_table-986"><span class="linenos">986</span></a><span class="sd">			]):</span>
+</span><span id="TypeParser.parse_table-987"><a href="#TypeParser.parse_table-987"><span class="linenos">987</span></a><span class="sd">			assert table == [</span>
+</span><span id="TypeParser.parse_table-988"><a href="#TypeParser.parse_table-988"><span class="linenos">988</span></a><span class="sd">				[1, 5.,  True,  &quot;1&quot;],</span>
+</span><span id="TypeParser.parse_table-989"><a href="#TypeParser.parse_table-989"><span class="linenos">989</span></a><span class="sd">				[2, 6.7, False, &quot;2.3&quot;],</span>
+</span><span id="TypeParser.parse_table-990"><a href="#TypeParser.parse_table-990"><span class="linenos">990</span></a><span class="sd">				[3, 8.,  None,  &quot;abc&quot;],</span>
+</span><span id="TypeParser.parse_table-991"><a href="#TypeParser.parse_table-991"><span class="linenos">991</span></a><span class="sd">			]</span>
+</span><span id="TypeParser.parse_table-992"><a href="#TypeParser.parse_table-992"><span class="linenos">992</span></a><span class="sd">			```</span>
+</span><span id="TypeParser.parse_table-993"><a href="#TypeParser.parse_table-993"><span class="linenos">993</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser.parse_table-994"><a href="#TypeParser.parse_table-994"><span class="linenos">994</span></a>		<span class="k">return</span> <span class="p">[</span><span class="n">converted_row</span> <span class="k">for</span> <span class="n">converted_row</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">iterate_table</span><span class="p">(</span><span class="n">rows</span><span class="p">)]</span>
 </span></pre></div>
 
 
     <div class="docstring">
 <p>Parse a table of strings and convert them to the underlying common type of each column</p>
 
 <p>For each column, if the values do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the column. See <code><a href="#reduce_types">parsetypes.reduce_types()</a></code> for more information.</p>
@@ -2763,49 +2921,49 @@
         <span class="name">iterate_table</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">rows</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]]</span></span><span class="return-annotation">) -> <span class="n">Iterator</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">,</span> <span class="nb">float</span><span class="p">,</span> <span class="n">decimal</span><span class="o">.</span><span class="n">Decimal</span><span class="p">,</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">NoneType</span><span class="p">,</span> <span class="nb">list</span><span class="p">]]]</span>:</span></span>
 
 
                 <label class="view-source-button" for="TypeParser.iterate_table-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#TypeParser.iterate_table"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.iterate_table-963"><a href="#TypeParser.iterate_table-963"><span class="linenos">963</span></a>	<span class="k">def</span> <span class="nf">iterate_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">rows</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]])</span> <span class="o">-&gt;</span> <span class="n">Iterator</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">AnyValue</span><span class="p">]]:</span>
-</span><span id="TypeParser.iterate_table-964"><a href="#TypeParser.iterate_table-964"><span class="linenos">964</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="TypeParser.iterate_table-965"><a href="#TypeParser.iterate_table-965"><span class="linenos">965</span></a><span class="sd">			Parse a table of strings for the underlying common type of each column, then convert and yield each row</span>
-</span><span id="TypeParser.iterate_table-966"><a href="#TypeParser.iterate_table-966"><span class="linenos">966</span></a>
-</span><span id="TypeParser.iterate_table-967"><a href="#TypeParser.iterate_table-967"><span class="linenos">967</span></a><span class="sd">			For each column, if the values do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the column. See `parsetypes.reduce_types()` for more information.</span>
-</span><span id="TypeParser.iterate_table-968"><a href="#TypeParser.iterate_table-968"><span class="linenos">968</span></a>
-</span><span id="TypeParser.iterate_table-969"><a href="#TypeParser.iterate_table-969"><span class="linenos">969</span></a><span class="sd">			This is a generator that computes and yields each row one at a time. The function `parse_table()` behaves analogously, except that it computes the entire table and returns it as a list of lists. However, note that although this is a generator, the type to which the value sshould be converted is still determined by `infer_table()`, and so the individual inferred types of every value in the table must be able to fit into memory.</span>
-</span><span id="TypeParser.iterate_table-970"><a href="#TypeParser.iterate_table-970"><span class="linenos">970</span></a>
-</span><span id="TypeParser.iterate_table-971"><a href="#TypeParser.iterate_table-971"><span class="linenos">971</span></a><span class="sd">			Parameters</span>
-</span><span id="TypeParser.iterate_table-972"><a href="#TypeParser.iterate_table-972"><span class="linenos">972</span></a><span class="sd">			----------</span>
-</span><span id="TypeParser.iterate_table-973"><a href="#TypeParser.iterate_table-973"><span class="linenos">973</span></a><span class="sd">			`rows`</span>
-</span><span id="TypeParser.iterate_table-974"><a href="#TypeParser.iterate_table-974"><span class="linenos">974</span></a><span class="sd">			: table of strings to be parsed, in row-major order</span>
-</span><span id="TypeParser.iterate_table-975"><a href="#TypeParser.iterate_table-975"><span class="linenos">975</span></a>
-</span><span id="TypeParser.iterate_table-976"><a href="#TypeParser.iterate_table-976"><span class="linenos">976</span></a><span class="sd">			Yields</span>
-</span><span id="TypeParser.iterate_table-977"><a href="#TypeParser.iterate_table-977"><span class="linenos">977</span></a><span class="sd">			-------</span>
-</span><span id="TypeParser.iterate_table-978"><a href="#TypeParser.iterate_table-978"><span class="linenos">978</span></a><span class="sd">			each row of converted table values</span>
-</span><span id="TypeParser.iterate_table-979"><a href="#TypeParser.iterate_table-979"><span class="linenos">979</span></a>
-</span><span id="TypeParser.iterate_table-980"><a href="#TypeParser.iterate_table-980"><span class="linenos">980</span></a><span class="sd">			Examples</span>
-</span><span id="TypeParser.iterate_table-981"><a href="#TypeParser.iterate_table-981"><span class="linenos">981</span></a><span class="sd">			--------</span>
-</span><span id="TypeParser.iterate_table-982"><a href="#TypeParser.iterate_table-982"><span class="linenos">982</span></a><span class="sd">			```python</span>
-</span><span id="TypeParser.iterate_table-983"><a href="#TypeParser.iterate_table-983"><span class="linenos">983</span></a><span class="sd">			parser = TypeParser()</span>
-</span><span id="TypeParser.iterate_table-984"><a href="#TypeParser.iterate_table-984"><span class="linenos">984</span></a><span class="sd">			table = parser.iterate_table([</span>
-</span><span id="TypeParser.iterate_table-985"><a href="#TypeParser.iterate_table-985"><span class="linenos">985</span></a><span class="sd">				[&quot;1&quot;,   &quot;true&quot;,  &quot;1&quot;],</span>
-</span><span id="TypeParser.iterate_table-986"><a href="#TypeParser.iterate_table-986"><span class="linenos">986</span></a><span class="sd">				[&quot;2&quot;,   &quot;false&quot;, &quot;2.3&quot;],</span>
-</span><span id="TypeParser.iterate_table-987"><a href="#TypeParser.iterate_table-987"><span class="linenos">987</span></a><span class="sd">				[&quot;3.4&quot;, &quot;2&quot;,     &quot;abc&quot;],</span>
-</span><span id="TypeParser.iterate_table-988"><a href="#TypeParser.iterate_table-988"><span class="linenos">988</span></a><span class="sd">			]):</span>
-</span><span id="TypeParser.iterate_table-989"><a href="#TypeParser.iterate_table-989"><span class="linenos">989</span></a><span class="sd">			assert next(table) == [1.,  1, &quot;1&quot;]</span>
-</span><span id="TypeParser.iterate_table-990"><a href="#TypeParser.iterate_table-990"><span class="linenos">990</span></a><span class="sd">			assert next(table) == [2.,  0, &quot;2.3&quot;]</span>
-</span><span id="TypeParser.iterate_table-991"><a href="#TypeParser.iterate_table-991"><span class="linenos">991</span></a><span class="sd">			assert next(table) == [3.4, 2, &quot;abc&quot;]</span>
-</span><span id="TypeParser.iterate_table-992"><a href="#TypeParser.iterate_table-992"><span class="linenos">992</span></a><span class="sd">			```</span>
-</span><span id="TypeParser.iterate_table-993"><a href="#TypeParser.iterate_table-993"><span class="linenos">993</span></a><span class="sd">		&quot;&quot;&quot;</span>
-</span><span id="TypeParser.iterate_table-994"><a href="#TypeParser.iterate_table-994"><span class="linenos">994</span></a>		<span class="n">inferred_types</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">infer_table</span><span class="p">(</span><span class="n">rows</span><span class="p">)</span>
-</span><span id="TypeParser.iterate_table-995"><a href="#TypeParser.iterate_table-995"><span class="linenos">995</span></a>
-</span><span id="TypeParser.iterate_table-996"><a href="#TypeParser.iterate_table-996"><span class="linenos">996</span></a>		<span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">rows</span><span class="p">:</span>
-</span><span id="TypeParser.iterate_table-997"><a href="#TypeParser.iterate_table-997"><span class="linenos">997</span></a>			<span class="k">yield</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">_convert</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">inferred</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span><span class="p">,</span> <span class="n">inferred</span> <span class="ow">in</span> <span class="nb">zip</span><span class="p">(</span><span class="n">row</span><span class="p">,</span> <span class="n">inferred_types</span><span class="p">)]</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="TypeParser.iterate_table-997"><a href="#TypeParser.iterate_table-997"><span class="linenos"> 997</span></a>	<span class="k">def</span> <span class="nf">iterate_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">rows</span><span class="p">:</span> <span class="n">Iterable</span><span class="p">[</span><span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]])</span> <span class="o">-&gt;</span> <span class="n">Iterator</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">AnyValue</span><span class="p">]]:</span>
+</span><span id="TypeParser.iterate_table-998"><a href="#TypeParser.iterate_table-998"><span class="linenos"> 998</span></a><span class="w">		</span><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="TypeParser.iterate_table-999"><a href="#TypeParser.iterate_table-999"><span class="linenos"> 999</span></a><span class="sd">			Parse a table of strings for the underlying common type of each column, then convert and yield each row</span>
+</span><span id="TypeParser.iterate_table-1000"><a href="#TypeParser.iterate_table-1000"><span class="linenos">1000</span></a>
+</span><span id="TypeParser.iterate_table-1001"><a href="#TypeParser.iterate_table-1001"><span class="linenos">1001</span></a><span class="sd">			For each column, if the values do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the column. See `parsetypes.reduce_types()` for more information.</span>
+</span><span id="TypeParser.iterate_table-1002"><a href="#TypeParser.iterate_table-1002"><span class="linenos">1002</span></a>
+</span><span id="TypeParser.iterate_table-1003"><a href="#TypeParser.iterate_table-1003"><span class="linenos">1003</span></a><span class="sd">			This is a generator that computes and yields each row one at a time. The function `parse_table()` behaves analogously, except that it computes the entire table and returns it as a list of lists. However, note that although this is a generator, the type to which the value sshould be converted is still determined by `infer_table()`, and so the individual inferred types of every value in the table must be able to fit into memory.</span>
+</span><span id="TypeParser.iterate_table-1004"><a href="#TypeParser.iterate_table-1004"><span class="linenos">1004</span></a>
+</span><span id="TypeParser.iterate_table-1005"><a href="#TypeParser.iterate_table-1005"><span class="linenos">1005</span></a><span class="sd">			Parameters</span>
+</span><span id="TypeParser.iterate_table-1006"><a href="#TypeParser.iterate_table-1006"><span class="linenos">1006</span></a><span class="sd">			----------</span>
+</span><span id="TypeParser.iterate_table-1007"><a href="#TypeParser.iterate_table-1007"><span class="linenos">1007</span></a><span class="sd">			`rows`</span>
+</span><span id="TypeParser.iterate_table-1008"><a href="#TypeParser.iterate_table-1008"><span class="linenos">1008</span></a><span class="sd">			: table of strings to be parsed, in row-major order</span>
+</span><span id="TypeParser.iterate_table-1009"><a href="#TypeParser.iterate_table-1009"><span class="linenos">1009</span></a>
+</span><span id="TypeParser.iterate_table-1010"><a href="#TypeParser.iterate_table-1010"><span class="linenos">1010</span></a><span class="sd">			Yields</span>
+</span><span id="TypeParser.iterate_table-1011"><a href="#TypeParser.iterate_table-1011"><span class="linenos">1011</span></a><span class="sd">			-------</span>
+</span><span id="TypeParser.iterate_table-1012"><a href="#TypeParser.iterate_table-1012"><span class="linenos">1012</span></a><span class="sd">			each row of converted table values</span>
+</span><span id="TypeParser.iterate_table-1013"><a href="#TypeParser.iterate_table-1013"><span class="linenos">1013</span></a>
+</span><span id="TypeParser.iterate_table-1014"><a href="#TypeParser.iterate_table-1014"><span class="linenos">1014</span></a><span class="sd">			Examples</span>
+</span><span id="TypeParser.iterate_table-1015"><a href="#TypeParser.iterate_table-1015"><span class="linenos">1015</span></a><span class="sd">			--------</span>
+</span><span id="TypeParser.iterate_table-1016"><a href="#TypeParser.iterate_table-1016"><span class="linenos">1016</span></a><span class="sd">			```python</span>
+</span><span id="TypeParser.iterate_table-1017"><a href="#TypeParser.iterate_table-1017"><span class="linenos">1017</span></a><span class="sd">			parser = TypeParser()</span>
+</span><span id="TypeParser.iterate_table-1018"><a href="#TypeParser.iterate_table-1018"><span class="linenos">1018</span></a><span class="sd">			table = parser.iterate_table([</span>
+</span><span id="TypeParser.iterate_table-1019"><a href="#TypeParser.iterate_table-1019"><span class="linenos">1019</span></a><span class="sd">				[&quot;1&quot;,   &quot;true&quot;,  &quot;1&quot;],</span>
+</span><span id="TypeParser.iterate_table-1020"><a href="#TypeParser.iterate_table-1020"><span class="linenos">1020</span></a><span class="sd">				[&quot;2&quot;,   &quot;false&quot;, &quot;2.3&quot;],</span>
+</span><span id="TypeParser.iterate_table-1021"><a href="#TypeParser.iterate_table-1021"><span class="linenos">1021</span></a><span class="sd">				[&quot;3.4&quot;, &quot;2&quot;,     &quot;abc&quot;],</span>
+</span><span id="TypeParser.iterate_table-1022"><a href="#TypeParser.iterate_table-1022"><span class="linenos">1022</span></a><span class="sd">			]):</span>
+</span><span id="TypeParser.iterate_table-1023"><a href="#TypeParser.iterate_table-1023"><span class="linenos">1023</span></a><span class="sd">			assert next(table) == [1.,  1, &quot;1&quot;]</span>
+</span><span id="TypeParser.iterate_table-1024"><a href="#TypeParser.iterate_table-1024"><span class="linenos">1024</span></a><span class="sd">			assert next(table) == [2.,  0, &quot;2.3&quot;]</span>
+</span><span id="TypeParser.iterate_table-1025"><a href="#TypeParser.iterate_table-1025"><span class="linenos">1025</span></a><span class="sd">			assert next(table) == [3.4, 2, &quot;abc&quot;]</span>
+</span><span id="TypeParser.iterate_table-1026"><a href="#TypeParser.iterate_table-1026"><span class="linenos">1026</span></a><span class="sd">			```</span>
+</span><span id="TypeParser.iterate_table-1027"><a href="#TypeParser.iterate_table-1027"><span class="linenos">1027</span></a><span class="sd">		&quot;&quot;&quot;</span>
+</span><span id="TypeParser.iterate_table-1028"><a href="#TypeParser.iterate_table-1028"><span class="linenos">1028</span></a>		<span class="n">inferred_types</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">infer_table</span><span class="p">(</span><span class="n">rows</span><span class="p">)</span>
+</span><span id="TypeParser.iterate_table-1029"><a href="#TypeParser.iterate_table-1029"><span class="linenos">1029</span></a>
+</span><span id="TypeParser.iterate_table-1030"><a href="#TypeParser.iterate_table-1030"><span class="linenos">1030</span></a>		<span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">rows</span><span class="p">:</span>
+</span><span id="TypeParser.iterate_table-1031"><a href="#TypeParser.iterate_table-1031"><span class="linenos">1031</span></a>			<span class="k">yield</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">convert</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">inferred</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span><span class="p">,</span> <span class="n">inferred</span> <span class="ow">in</span> <span class="nb">zip</span><span class="p">(</span><span class="n">row</span><span class="p">,</span> <span class="n">inferred_types</span><span class="p">)]</span>
 </span></pre></div>
 
 
     <div class="docstring">
 <p>Parse a table of strings for the underlying common type of each column, then convert and yield each row</p>
 
 <p>For each column, if the values do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the column. See <code><a href="#reduce_types">parsetypes.reduce_types()</a></code> for more information.</p>
```

#### html2text {}

```diff
@@ -13,14 +13,15 @@
           o parse_bool()
           o parse_int()
           o parse_float()
           o parse_decimal()
           o infer()
           o infer_series()
           o infer_table()
+          o convert()
           o parse()
           o parse_series()
           o parse_table()
           o iterate_table()
     * reduce_types()
 built_with_pdoc[pdoc_logo]
    Edit_on_GitHub
@@ -46,1855 +47,1918 @@
 _6
 - give exact Decimal values instead of floats
 _7
 - detect inline lists
 _8"""
 _9
 10
-11__version__ = "0.2.3"
+11__version__ = "0.2.4"
 12
 13from ._common import AnyScalar, AnyScalarType, AnyValue, AnyValueType,
 GenericValue, Nullable
 14from ._parser import TypeParser
 15from ._reduce_types import reduce_types
 16
 17__all__ = ('TypeParser', 'reduce_types')
   ⁰
 class TypeParser: View Source
-_60class TypeParser:
-_61
+__60class TypeParser:
+__61
 """
-_62
+__62
 A parser that can be used to infer the underlying types of data serialised as
 strings, and to convert them into their original underlying types.
-_63
-_64
+__63
+__64
 Instances of this class can be configured with different settings for the
 parser and inferrer. See the constructor for more details about the available
 options.
-_65
+__65
 """
-_66
-_67
+__66
+__67
 def __init__(self,
-_68
+__68
     *,
-_69
+__69
 trim: bool=True,
-_70
+__70
 use_decimal: bool=False,
-_71
+__71
 list_delimiter: Optional[str]=None,
-_72
+__72
 none_values: Iterable[str]=[""],
-_73
+__73
 none_case_sensitive: bool=False,
-_74
+__74
 true_values: Iterable[str]=["true"],
-_75
+__75
 false_values: Iterable[str]=["false"],
-_76
+__76
 bool_case_sensitive: bool=False,
-_77
+__77
 int_case_sensitive: bool=False,
-_78
+__78
 inf_values: Iterable[str]=[],
-_79
+__79
 nan_values: Iterable[str]=[],
-_80
+__80
 float_case_sensitive: bool=False,
-_81
+__81
 case_sensitive: Optional[bool]=None,
-_82
+__82
 ):
-_83
+__83
 """
-_84
+__84
 Initialise a new parser
-_85
-_86
+__85
+__86
 Parameters
-_87
+__87
 ----------
-_88
+__88
 `trim`
-_89
+__89
 : whether leading and trailing whitespace should be stripped from strings
-_90
-_91
+__90
+__91
 `use_decimal`
-_92
+__92
 : whether non-integer numeric values should be inferred as Decimal (exact
 values) instead of float (non-exact values). Note that this only applies to
 methods that attempt to infer type (`infer()` and `infer_*()`), and does not
 affect methods where the type is explicitly specified (`is_float()`,
 `is_decimal()`, `parse_float()`, `parse_decimal()`).
-_93
-_94
+__93
+__94
 `list_delimiter`
-_95
+__95
 : the delimiter used for identifying lists and for separating list items. If
 set to None, the parser will not attempt to identify lists when inferring
 types, which usually causes the value to be treated as a str instead.
-_96
-_97
+__96
+__97
 `none_values`
-_98
+__98
 : list of strings that represent the value None
-_99
-100
+__99
+_100
 `none_case_sensitive`
-101
+_101
 : whether matches against `none_values` should be made in a case-sensitive
 manner
-102
-103
+_102
+_103
 `true_values`
-104
+_104
 : list of strings that represent the bool value True
-105
-106
+_105
+_106
 `false_values`
-107
+_107
 : list of strings that represent the bool value False
-108
-109
+_108
+_109
 `bool_case_sensitive`
-110
+_110
 : whether matches against `true_values` and `false_values` should be made in a
 case-sensitive manner
-111
-112
+_111
+_112
 `int_case_sensitive`
-113
+_113
 : whether checks for int should be done in a case-sensitive manner. This
 usually only applies to values given in scientific notation, where the mantissa
 and exponent usually are separated by `e`.
-114
-115
+_114
+_115
 `inf_values`
-116
+_116
 : list of strings that represent the float or Decimal value of infinity. Each
 of the strings can be prepended with a negative sign to represent negative
 infinity also.
-117
-118
+_117
+_118
 `nan_values`
-119
+_119
 : list of strings that represent a float or Decimal that is NaN (not a number)
-120
-121
+_120
+_121
 `float_case_sensitive`
-122
+_122
 : whether checks for float should be done in a case-sensitive manner. This
 applies to matches against `inf_values` and `nan_values`, as well as to values
 given in scientific notation, where the mantissa and exponent are usually
 separated by `e`.
-123
-124
+_123
+_124
 `case_sensitive`
-125
+_125
 : whether all matches should be made in a case-sensitive manner. Sets all of
 `none_case_sensitive`, `bool_case_sensitive`, `int_case_sensitive`,
 `float_case_sensitive` to the same value, ignoring any individual settings.
-126
-127
+_126
+_127
 Raises
-128
+_128
 ------
-129
+_129
 `ValueError` if any of the options would lead to ambiguities during parsing
-130
+_130
 """
-131
-132
+_131
+_132
 if case_sensitive is not None:
-133
+_133
 none_case_sensitive = case_sensitive
-134
+_134
 int_case_sensitive = case_sensitive
-135
+_135
 bool_case_sensitive = case_sensitive
-136
+_136
 float_case_sensitive = case_sensitive
-137
-138
+_137
+_138
 self.trim = trim
-139
+_139
 if self.trim:
-140
+_140
 none_values = (value.strip() for value in none_values)
-141
+_141
 true_values = (value.strip() for value in true_values)
-142
+_142
 false_values = (value.strip() for value in false_values)
-143
+_143
 inf_values = (value.strip() for value in inf_values)
-144
+_144
 nan_values = (value.strip() for value in nan_values)
-145
-146
+_145
+_146
 self.use_decimal = use_decimal
-147
+_147
 self.list_delimiter = list_delimiter
-148
-149
+_148
+_149
 self.none_case_sensitive = none_case_sensitive
-150
+_150
 if not self.none_case_sensitive:
-151
+_151
 none_values = (value.lower() for value in none_values)
-152
+_152
 self.none_values = set(none_values)
-153
-154
+_153
+_154
 self.bool_case_sensitive = bool_case_sensitive
-155
+_155
 if not self.bool_case_sensitive:
-156
+_156
 true_values = (value.lower() for value in true_values)
-157
+_157
 false_values = (value.lower() for value in false_values)
-158
+_158
 self.true_values = set(true_values)
-159
+_159
 self.false_values = set(false_values)
-160
-161
+_160
+_161
 self.int_case_sensitive = int_case_sensitive
-162
-163
+_162
+_163
 self.float_case_sensitive = float_case_sensitive
-164
+_164
 if not self.float_case_sensitive:
-165
+_165
 inf_values = (value.lower() for value in inf_values)
-166
+_166
 nan_values = (value.lower() for value in nan_values)
-167
+_167
 self.inf_values = set(inf_values)
-168
+_168
 self.nan_values = set(nan_values)
-169
-170
+_169
+_170
 # Unconfigurable default values
-171
+_171
 self._negative_char = "-"
-172
+_172
 self._negative_chars = {self._negative_char, "â"}
-173
+_173
 self._sign_chars = self._negative_chars | {"+"}
-174
+_174
 self._digit_chars = {"0", "1", "2", "3", "4", "5", "6", "7", "8", "9"}  #
 Because isdigit("Â²") == True, but int("Â²") is invalid
-175
+_175
 self._digit_separators = {"_"}
-176
+_176
 self._scientific_char = "e"
-177
+_177
 self._float_separator = "."
-178
+_178
 self._reserved_chars = self._sign_chars | self._digit_chars |
 self._digit_separators | {self._scientific_char} | {self._float_separator}
-179
+_179
 # special_chars = self._reserved_chars | self.list_delimiter
-180
-181
+_180
+_181
 # Check if any special values conflict
-182
+_182
 for name, special_values in [
-183
+_183
 (_SpecialValue.LIST, [self.list_delimiter] if self.list_delimiter is not None
 else []),
-184
+_184
 (_SpecialValue.NONE, self.none_values),
-185
+_185
 (_SpecialValue.TRUE, self.true_values),
-186
+_186
 (_SpecialValue.FALSE, self.false_values),
-187
+_187
 (_SpecialValue.INF, self.inf_values),
-188
+_188
 (_SpecialValue.NAN, self.nan_values),
-189
+_189
 ]:
-190
+_190
 for special_value in special_values:
-191
+_191
 if special_value in self._reserved_chars:
-192
+_192
 raise ValueError(f"cannot use reserved char as {name.value}: {special_value}")
-193
-194
+_193
+_194
 if name != _SpecialValue.NONE and self.is_none(special_value):
-195
+_195
 raise ValueError(f"cannot use None value as {name.value}: {special_value}")
-196
-197
+_196
+_197
 if (
-198
+_198
 (name == _SpecialValue.TRUE and self.parse_bool(special_value) != True) or
-199
+_199
 (name == _SpecialValue.FALSE and self.parse_bool(special_value) != False) or
-200
+_200
 (name != _SpecialValue.TRUE and name != _SpecialValue.FALSE and self.is_bool
 (special_value))
-201
+_201
 ):
-202
+_202
 raise ValueError(f"cannot use bool value as {name.value}: {special_value}")
-203
-204
+_203
+_204
 if self.is_int(special_value):
-205
+_205
 raise ValueError(f"cannot use int value as {name.value}: {special_value}")
-206
-207
+_206
+_207
 if self.use_decimal:
-208
+_208
 if (
-209
+_209
 (name == _SpecialValue.INF and self.parse_decimal(special_value) != Decimal
 (math.inf)) or
-210
+_210
 (name == _SpecialValue.NAN and not self.parse_decimal(special_value).is_nan())
 or
-211
+_211
 (name != _SpecialValue.INF and name != _SpecialValue.NAN and self.is_float
 (special_value))
-212
+_212
 ):
-213
+_213
 raise ValueError(f"cannot use Decimal value as {name}: {special_value}")
-214
+_214
 else:
-215
+_215
 if (
-216
+_216
 (name == _SpecialValue.INF and self.parse_float(special_value) != math.inf) or
-217
+_217
 (name == _SpecialValue.NAN and self.parse_float(special_value) is not math.nan)
 or
-218
+_218
 (name != _SpecialValue.INF and name != _SpecialValue.NAN and self.is_float
 (special_value))
-219
+_219
 ):
-220
+_220
 raise ValueError(f"cannot use float value as {name}: {special_value}")
-221
-222
-223
+_221
+_222
+_223
 def is_none(self, value: str) -> bool:
-224
+_224
 """
-225
+_225
 Check if a string represents the value None
-226
-227
+_226
+_227
 Only strings that match the values in `self.none_values` will be interpreted as
 None. The default accepted values are `[""]`, i.e. an empty string. The case
 sensitivity of this matching depends on `self.none_case_sensitive`, which is
 False by default.
-228
-229
+_228
+_229
 Parameters
-230
+_230
 ----------
-231
+_231
 `value`
-232
+_232
 : string to be checked
-233
-234
+_233
+_234
 Returns
-235
+_235
 -------
-236
+_236
 whether it is None
-237
-238
+_237
+_238
 Examples
-239
+_239
 --------
-240
+_240
 ```python
-241
+_241
 parser = TypeParser()
-242
+_242
 parser.parse_bool("")     # True
-243
+_243
 parser.parse_bool("abc")  # False
-244
+_244
 ```
-245
+_245
 """
-246
+_246
 if self.trim:
-247
+_247
 value = value.strip()
-248
+_248
 if not self.bool_case_sensitive:
-249
+_249
 value = value.lower()
-250
-251
+_250
+_251
 if value in self.none_values:
-252
+_252
 return True
-253
+_253
 else:
-254
+_254
 return False
-255
-256
-257
+_255
+_256
+_257
 def is_bool(self, value: str) -> bool:
-258
+_258
 """
-259
+_259
 Check if a string represents a bool
-260
-261
+_260
+_261
 Only strings that match the values in `self.true_values` and
 `self.false_values` will be interpreted as booleans. The default accepted
 values are `["true"]` and `["false"]` respectively. The case sensitivity of
 this matching depends on `self.bool_case_sensitive`, which is False by default.
-262
-263
+_262
+_263
 Parameters
-264
+_264
 ----------
-265
+_265
 `value`
-266
+_266
 : string to be checked
-267
-268
+_267
+_268
 Returns
-269
+_269
 -------
-270
+_270
 whether it is a bool
-271
-272
+_271
+_272
 Examples
-273
+_273
 --------
-274
+_274
 ```python
-275
+_275
 parser = TypeParser()
-276
+_276
 parser.is_bool("true")  # True
-277
+_277
 parser.is_bool("")      # True
-278
+_278
 parser.is_bool("abc")   # False
-279
+_279
 ```
-280
+_280
 """
-281
+_281
 if self.trim:
-282
+_282
 value = value.strip()
-283
-284
+_283
+_284
 if not self.bool_case_sensitive:
-285
+_285
 value = value.lower()
-286
+_286
 if value in self.true_values:
-287
+_287
 return True
-288
+_288
 if value in self.false_values:
-289
+_289
 return True
-290
-291
+_290
+_291
 return False
-292
-293
-294
+_292
+_293
+_294
 def is_int(self, value: str, *, allow_sign: bool=True, allow_negative:
 bool=True, allow_scientific: bool=True) -> bool:
-295
+_295
 """
-296
+_296
 Check if a string represents an int
-297
-298
+_297
+_298
 Parameters
-299
+_299
 ----------
-300
+_300
 `value`
-301
+_301
 : string to be checked
-302
-303
+_302
+_303
 `allow_negative`
-304
+_304
 : whether to accept negative values
-305
-306
+_305
+_306
 `allow_sign`
-307
+_307
 : whether to accept signed values. If False, it implies that `allow_negative`
 is False also.
-308
-309
+_308
+_309
 `allow_scientific`
-310
+_310
 : whether to accept scientific notation. If True, strings of the form
 <code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression
 <code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the
 mantissa/significand and <var>X</var> is the exponent. Note <var>M</var> *must*
 be an integer and <var>X</var> *must* be a non-negative integer, even in cases
 where the above expression evaluates mathematically to an integer.
-311
-312
+_311
+_312
 Returns
-313
+_313
 -------
-314
+_314
 whether it is an int
-315
-316
+_315
+_316
 Examples
-317
+_317
 --------
-318
+_318
 ```python
-319
+_319
 parser = TypeParser()
-320
+_320
 parser.is_int("0")    # True
-321
+_321
 parser.is_int("-1")   # True
-322
+_322
 parser.is_int("abc")  # False
-323
+_323
 parser.is_int("")     # False
-324
+_324
 ```
-325
+_325
 """
-326
+_326
 if self.trim:
-327
+_327
 value = value.strip()
-328
-329
+_328
+_329
 if len(value) == 0:
-330
+_330
 return False
-331
-332
+_331
+_332
 if allow_scientific:
-333
+_333
 value, exp = _decompose_string_pair(value, self._scientific_char,
 self.int_case_sensitive)
-334
+_334
 if exp is not None:
-335
+_335
 return self.is_int(
-336
+_336
 value, allow_sign=True, allow_negative=allow_negative, allow_scientific=False
-337
+_337
 ) and self.is_int(
-338
+_338
 exp, allow_sign=True, allow_negative=False, allow_scientific=False
-339
+_339
 )
-340
-341
+_340
+_341
 if value[0] in self._sign_chars:
-342
+_342
 if len(value) == 1:
-343
+_343
 return False
-344
+_344
 if not allow_sign:
-345
+_345
 return False
-346
+_346
 if not allow_negative and value[0] in self._negative_chars:
-347
+_347
 return False
-348
+_348
 value = value[1:]
-349
+_349
 if value[0] in self._digit_separators or value[-1] in self._digit_separators:
-350
+_350
 return False
-351
-352
+_351
+_352
 prev_separated = False
-353
+_353
 for c in value:
-354
+_354
 if c in self._digit_separators:
-355
+_355
 if prev_separated:
-356
+_356
 return False
-357
+_357
 prev_separated = True
-358
+_358
 else:
-359
+_359
 prev_separated = False
-360
+_360
 if c not in self._digit_chars:
-361
+_361
 return False
-362
+_362
 return True
-363
-364
-365
+_363
+_364
+_365
 def is_float(self, value: str, *, allow_scientific: bool=True, allow_inf:
 bool=True, allow_nan: bool=True) -> bool:
-366
+_366
 """
-367
+_367
 Check if a string represents a float (or equivalently, a Decimal)
-368
-369
+_368
+_369
 This function will also return True if the string represents an int.
-370
-371
+_370
+_371
 Alias: `is_decimal()`
-372
-373
+_372
+_373
 Parameters
-374
+_374
 ----------
-375
+_375
 `value`
-376
+_376
 : string to be checked
-377
-378
+_377
+_378
 `allow_scientific`
-379
+_379
 : whether to accept scientific notation. If True, strings of the form
 <code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression
 <code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the
 mantissa/significand and <var>X</var> is the exponent. Note that <var>X</var>
 must be an integer, but can be negative.
-380
-381
+_380
+_381
 `allow_inf`
-382
+_382
 : whether to accept positive and negative infinity values. If True, strings
 that match the values in `self.inf_values` (empty by default) are interpreted
 as infinity, or as negative infinity if prepended by a negative sign. The case
 sensitivity of this matching depends on `self.float_case_sensitive`, which is
 False by default.
-383
-384
+_383
+_384
 `allow_nan`
-385
+_385
 : whether to accept NaN (not a number) representations. If True, strings that
 match the values in `self.nan_values` (empty by default) are interpeted as NaN.
 The case sensitivity of this matching depends on `self.float_case_sensitive`,
 which is False by default.
-386
-387
+_386
+_387
 Returns
-388
+_388
 -------
-389
+_389
 whether it is a float or Decimal
-390
-391
+_390
+_391
 Examples
-392
+_392
 --------
-393
+_393
 ```python
-394
+_394
 parser = TypeParser()
-395
+_395
 parser.is_float("1.")       # True
-396
+_396
 parser.is_float("12.3e-2")  # True
-397
+_397
 parser.is_float("abc")      # False
-398
+_398
 parser.is_float("")         # False
-399
+_399
 ```
-400
+_400
 """
-401
+_401
 if self.trim:
-402
+_402
 value = value.strip()
-403
-404
+_403
+_404
 if len(value) > 0 and value[0] in self._sign_chars:
-405
+_405
 value = value[1:]
-406
-407
+_406
+_407
 if self.float_case_sensitive:
-408
+_408
 special_value = value
-409
+_409
 else:
-410
+_410
 special_value = value.lower()
-411
+_411
 if allow_inf and special_value in self.inf_values:
-412
+_412
 return True
-413
+_413
 if allow_nan and special_value in self.nan_values:
-414
+_414
 return True
-415
-416
+_415
+_416
 if len(value) == 0:
-417
+_417
 return False
-418
-419
+_418
+_419
 if allow_scientific:
-420
+_420
 value, exp = _decompose_string_pair(value, self._scientific_char,
 self.float_case_sensitive)
-421
+_421
 if exp is not None:
-422
+_422
 return self.is_float(value, allow_scientific=False, allow_inf=False,
 allow_nan=False) and self.is_int(exp, allow_sign=True, allow_negative=True,
 allow_scientific=False)
-423
-424
+_423
+_424
 value, frac = _decompose_string_pair(value, self._float_separator,
 self.float_case_sensitive)
-425
+_425
 if frac is not None:
-426
+_426
 if value == "" and frac == "":
-427
+_427
 return False
-428
+_428
 return (
-429
+_429
 self.is_int(value, allow_sign=True, allow_negative=False,
 allow_scientific=False) or value == ""
-430
+_430
 ) and (
-431
+_431
 self.is_int(frac, allow_sign=False, allow_negative=False,
 allow_scientific=False) or frac == ""
-432
+_432
 )
-433
-434
+_433
+_434
 return self.is_int(value, allow_sign=True, allow_negative=True,
 allow_scientific=False)
-435
-436
-437
+_435
+_436
+_437
 def is_decimal(self, value: str, *, allow_scientific: bool=True, allow_inf:
 bool=True, allow_nan: bool=True) -> bool:
-438
+_438
 """
-439
+_439
 Alias of `is_float()`
-440
+_440
 """
-441
+_441
 return self.is_float(value, allow_scientific=allow_scientific,
 allow_inf=allow_inf, allow_nan=allow_nan)
-442
-443
-444
+_442
+_443
+_444
 def parse_none(self, value: str) -> None:
-445
+_445
 """
-446
+_446
 Parse a string and return it as the value None if possible
-447
-448
+_447
+_448
 Only strings that match the values in `self.none_values` will be interpreted as
 None. The default accepted values are `[""]`, i.e. an empty string. The case
 sensitivity of this matching depends on `self.none_case_sensitive`, which is
 False by default.
-449
-450
+_449
+_450
 Parameters
-451
+_451
 ----------
-452
+_452
 `value`
-453
+_453
 : string to be parsed
-454
-455
+_454
+_455
 Returns
-456
+_456
 -------
-457
+_457
 parsed None value
-458
-459
+_458
+_459
 Raises
-460
+_460
 ------
-461
+_461
 `ValueError` if `value` cannot be parsed
-462
-463
+_462
+_463
 Examples
-464
+_464
 --------
-465
+_465
 ```python
-466
+_466
 parser = TypeParser()
-467
+_467
 parser.parse_bool("")     # None
-468
+_468
 parser.parse_bool("abc")  # raises ValueError
-469
+_469
 ```
-470
+_470
 """
-471
+_471
 if self.is_none(value):
-472
+_472
 return None
-473
+_473
 else:
-474
+_474
 raise ValueError(f"not a none value: {value}")
-475
-476
-477
+_475
+_476
+_477
 def parse_bool(self, value: str) -> bool:
-478
+_478
 """
-479
+_479
 Parse a string and return it as a bool if possible
-480
-481
+_480
+_481
 Only strings that match the values in `self.true_values` and
 `self.false_values` will be interpreted as booleans. The default accepted
 values are `["true"]` and `["false"]` respectively. The case sensitivity of
 this matching depends on `self.bool_case_sensitive`, which is False by default.
-482
-483
+_482
+_483
 Parameters
-484
+_484
 ----------
-485
+_485
 `value`
-486
+_486
 : string to be parsed
-487
-488
+_487
+_488
 Returns
-489
+_489
 -------
-490
+_490
 parsed bool value
-491
-492
+_491
+_492
 Raises
-493
+_493
 ------
-494
+_494
 `ValueError` if `value` cannot be parsed
-495
-496
+_495
+_496
 Examples
-497
+_497
 --------
-498
+_498
 ```python
-499
+_499
 parser = TypeParser()
-500
+_500
 parser.parse_bool("true")   # True
-501
+_501
 parser.parse_bool("FALSE")  # False
-502
+_502
 ```
-503
+_503
 """
-504
+_504
 if self.trim:
-505
+_505
 value = value.strip()
-506
-507
+_506
+_507
 if self.bool_case_sensitive:
-508
+_508
 special_value = value
-509
+_509
 else:
-510
+_510
 special_value = value.lower()
-511
+_511
 if special_value in self.true_values:
-512
+_512
 return True
-513
+_513
 if special_value in self.false_values:
-514
+_514
 return False
-515
-516
+_515
+_516
 raise ValueError(f"not a boolean: {value}")
-517
-518
-519
+_517
+_518
+_519
 def parse_int(self, value: str, *, allow_scientific: bool=True) -> int:
-520
+_520
 """
-521
+_521
 Parse a string and return it as an int if possible
-522
-523
+_522
+_523
 If the string represents a bool, it will be converted to `1` for True and `0`
 for False.
-524
-525
+_524
+_525
 Parameters
-526
+_526
 ----------
-527
+_527
 `value`
-528
+_528
 : string to be parsed
-529
-530
+_529
+_530
 `allow_scientific`
-531
+_531
 : whether to accept scientific notation. If True, strings of the form
 <code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression
 <code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the
 mantissa/significand and <var>X</var> is the exponent. Note <var>M</var> *must*
 be an integer and <var>X</var> *must* be a non-negative integer, even in cases
 where the above expression evaluates mathematically to an integer.
-532
-533
+_532
+_533
 Returns
-534
+_534
 -------
-535
+_535
 parsed int value
-536
-537
+_536
+_537
 Raises
-538
+_538
 ------
-539
+_539
 `ValueError` if `value` cannot be parsed
-540
-541
+_540
+_541
 Examples
-542
+_542
 --------
-543
+_543
 ```python
-544
+_544
 parser = TypeParser()
-545
+_545
 parser.parse_int("0")    # 0
-546
+_546
 parser.parse_int("-1")   # -1
-547
+_547
 parser.parse_int("2e3")  # 2000
-548
+_548
 ```
-549
+_549
 """
-550
+_550
 if self.trim:
-551
+_551
 value = value.strip()
-552
-553
+_552
+_553
 if self.is_int(value, allow_sign=True, allow_negative=True,
 allow_scientific=allow_scientific):
-554
+_554
 if allow_scientific:
-555
+_555
 value, exp = _decompose_string_pair(value, self._scientific_char,
 self.int_case_sensitive)
-556
+_556
 if exp is not None:
-557
+_557
 if value[0] in (self._negative_chars - {self._negative_char}):
-558
+_558
 value = self._negative_char + value[1:]
-559
+_559
 return int(value) * (10 ** int(exp))
-560
-561
+_560
+_561
 if value[0] in (self._negative_chars - {self._negative_char}):
-562
+_562
 value = self._negative_char + value[1:]
-563
+_563
 return int(value)
-564
-565
+_564
+_565
 elif self.is_bool(value):
-566
+_566
 return int(self.parse_bool(value))
-567
+_567
 else:
-568
+_568
 raise ValueError(f"not an integer: {value}")
-569
-570
-571
+_569
+_570
+_571
 def _parse_floatlike(self,
-572
+_572
 value: str,
-573
+_573
 converter: Callable[[Union[str, bool]], _FloatLike],
-574
+_574
 inf_value: _FloatLike,
-575
+_575
 nan_value: _FloatLike,
-576
+_576
 *,
-577
+_577
 allow_scientific: bool=True,
-578
+_578
 allow_inf: bool=True,
-579
+_579
 allow_nan: bool=True
-580
+_580
 ) -> _FloatLike:
-581
+_581
 if self.trim:
-582
+_582
 value = value.strip()
-583
+_583
 if self.is_float(value, allow_scientific=allow_scientific, allow_inf=allow_inf,
 allow_nan=allow_nan):
-584
+_584
 if self.float_case_sensitive:
-585
+_585
 special_value = value
-586
+_586
 else:
-587
+_587
 special_value = value.lower()
-588
+_588
 if allow_inf and special_value in self.inf_values:
-589
+_589
 return inf_value
-590
+_590
 if allow_nan and special_value in self.nan_values:
-591
+_591
 return nan_value
-592
-593
+_592
+_593
 if len(value) > 0 and value[0] in self._sign_chars:
-594
+_594
 positive_part = value[1:]
-595
+_595
 if self.float_case_sensitive:
-596
+_596
 special_value = positive_part
-597
+_597
 else:
-598
+_598
 special_value = positive_part.lower()
-599
+_599
 if allow_inf and special_value in self.inf_values:
-600
+_600
 if value[0] in self._negative_chars:
-601
+_601
 return -1 * inf_value
-602
+_602
 else:
-603
+_603
 return inf_value
-604
+_604
 if allow_nan and special_value in self.nan_values:
-605
+_605
 return nan_value
-606
-607
+_606
+_607
 if value[0] in self._negative_chars:
-608
+_608
 value = self._negative_char + positive_part
-609
+_609
 return converter(value)
-610
+_610
 elif self.is_bool(value):
-611
+_611
 return converter(self.parse_bool(value))
-612
+_612
 else:
-613
+_613
 raise ValueError(f"not a {_FloatLike.__name__}: {value}")
-614
-615
-616
+_614
+_615
+_616
 def parse_float(self, value: str, *, allow_scientific: bool=True, allow_inf:
 bool=True, allow_nan: bool=True) -> float:
-617
+_617
 """
-618
+_618
 Parse a string and return it as a (non-exact) float if possible
-619
-620
+_619
+_620
 If the string represents a bool, it will be converted to `1.` for True and `0.`
 for False. If the string represents an int, it will be converted to a float
 also.
-621
-622
+_621
+_622
 Behaves analogously to `parse_decimal()`, except that that returns an exact
 Decimal instead.
-623
-624
+_623
+_624
 Parameters
-625
+_625
 ----------
-626
+_626
 `value`
-627
+_627
 : string to be parsed
-628
-629
+_628
+_629
 `allow_scientific`
-630
+_630
 : whether to accept scientific notation. If True, strings of the form
 <code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression
 <code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the
 mantissa/significand and <var>X</var> is the exponent. Note that <var>X</var>
 must be an integer, but can be negative.
-631
-632
+_631
+_632
 `allow_inf`
-633
+_633
 : whether to accept positive and negative infinity values. If True, strings
 that match the values in `self.inf_values` (empty by default) are interpreted
 as infinity, or as negative infinity if prepended by a negative sign. The case
 sensitivity of this matching depends on `self.float_case_sensitive`, which is
 False by default.
-634
-635
+_634
+_635
 `allow_nan`
-636
+_636
 : whether to accept NaN (not a number) representations. If True, strings that
 match the values in `self.nan_values` (empty by default) are interpeted as NaN.
 The case sensitivity of this matching depends on `self.float_case_sensitive`,
 which is False by default.
-637
-638
+_637
+_638
 Returns
-639
+_639
 -------
-640
+_640
 parsed float value
-641
-642
+_641
+_642
 Raises
-643
+_643
 ------
-644
+_644
 `ValueError` if `value` cannot be parsed
-645
-646
+_645
+_646
 Examples
-647
+_647
 --------
-648
+_648
 ```python
-649
+_649
 parser = TypeParser(inf_values=["inf"], nan_values=["nan"])
-650
+_650
 parser.parse_float("1.")       # 1.
-651
+_651
 parser.parse_float("1.23e2")   # 123.
-652
+_652
 parser.parse_float("1.23e-2")  # 0.0123
-653
+_653
 parser.parse_float("inf")      # math.inf
-654
+_654
 ```
-655
+_655
 """
-656
+_656
 return self._parse_floatlike(value, float, math.inf, math.nan,
-657
+_657
 allow_scientific=allow_scientific,
-658
+_658
 allow_inf=allow_inf,
-659
+_659
 allow_nan=allow_nan,
-660
+_660
 )
-661
-662
-663
+_661
+_662
+_663
 def parse_decimal(self, value: str, *, allow_scientific: bool=True, allow_inf:
 bool=True, allow_nan: bool=True) -> Decimal:
-664
+_664
 """
-665
+_665
 Parse a string and return it as an exact Decimal if possible
-666
-667
+_666
+_667
 If the string represents a bool, it will be converted to `Decimal(1)` for True
 and `Decimal(0)` for False. If the string represents an int, it will be
 converted to a Decimal also.
-668
-669
+_668
+_669
 Behaves analogously to `parse_float()`, except that that returns a non-exact
 float instead.
-670
-671
+_670
+_671
 Parameters
-672
+_672
 ----------
-673
+_673
 `value`
-674
+_674
 : string to be parsed
-675
-676
+_675
+_676
 `allow_scientific`
-677
+_677
 : whether to accept scientific notation. If True, strings of the form
 <code>"<var>M</var>e<var>X</var>"</code> will be interpreted as the expression
 <code><var>M</var> * (10 ** <var>X</var>)</code>, where <var>M</var> is the
 mantissa/significand and <var>X</var> is the exponent. Note that <var>X</var>
 must be an integer, but can be negative.
-678
-679
+_678
+_679
 `allow_inf`
-680
+_680
 : whether to accept positive and negative infinity values. If True, strings
 that match the values in `self.inf_values` (empty by default) are interpreted
 as infinity, or as negative infinity if prepended by a negative sign. The case
 sensitivity of this matching depends on `self.float_case_sensitive`, which is
 False by default.
-681
-682
+_681
+_682
 `allow_nan`
-683
+_683
 : whether to accept NaN (not a number) representations. If True, strings that
 match the values in `self.nan_values` (empty by default) are interpeted as NaN.
 The case sensitivity of this matching depends on `self.float_case_sensitive`,
 which is False by default.
-684
-685
+_684
+_685
 Returns
-686
+_686
 -------
-687
+_687
 parsed Decimal value
-688
-689
+_688
+_689
 Raises
-690
+_690
 ------
-691
+_691
 `ValueError` if `value` cannot be parsed
-692
-693
+_692
+_693
 Examples
-694
+_694
 --------
-695
+_695
 ```python
-696
+_696
 parser = TypeParser(inf_values=["inf"], nan_values=["nan"])
-697
+_697
 parser.parse_decimal("1.")       # Decimal(1)
-698
+_698
 parser.parse_decimal("1.23e2")   # Decimal(123)
-699
+_699
 parser.parse_decimal("1.23e-2")  # Decimal(123) / Decimal(10000)
-700
+_700
 parser.parse_decimal("inf")      # Decimal(math.inf)
-701
+_701
 ```
-702
+_702
 """
-703
+_703
 return self._parse_floatlike(value, Decimal, Decimal(math.inf), Decimal
 (math.nan),
-704
+_704
 allow_scientific=allow_scientific,
-705
+_705
 allow_inf=allow_inf,
-706
+_706
 allow_nan=allow_nan,
-707
+_707
 )
-708
-709
-710
+_708
+_709
+_710
 def infer(self, value: str) -> AnyValueType:
-711
+_711
 """
-712
+_712
 Infer the underlying type of a string
-713
-714
+_713
+_714
 Also check for inline lists if `self.list_delimiter` is not None.
-715
-716
+_715
+_716
 Parameters
-717
+_717
 ----------
-718
+_718
 `value`
-719
+_719
 : the string for which the type should be inferred
-720
-721
+_720
+_721
 Returns
-722
+_722
 -------
-723
+_723
 inferred type
-724
-725
+_724
+_725
 Examples
-726
+_726
 --------
-727
+_727
 ```python
-728
+_728
 parser = TypeParser()
-729
+_729
 parser.infer("true")  # bool
-730
+_730
 parser.infer("2.0")   # float
-731
+_731
 parser.infer("abc")   # str
-732
+_732
 ```
-733
+_733
 """
-734
+_734
 if self.is_none(value):
-735
+_735
 return NoneType
-736
+_736
 if self.is_bool(value):
-737
+_737
 return bool
-738
+_738
 if self.is_int(value):
-739
+_739
 return int
-740
+_740
 if self.is_float(value):
-741
+_741
 if self.use_decimal:
-742
+_742
 return Decimal
-743
+_743
 else:
-744
+_744
 return float
-745
-746
+_745
+_746
 if self.trim:
-747
+_747
 value = value.strip()
-748
-749
+_748
+_749
 if self.list_delimiter is not None and self.list_delimiter in value:
-750
+_750
 subvalues = value.split(self.list_delimiter)
-751
+_751
 if self.trim:
-752
+_752
 subvalues = [subvalue.strip() for subvalue in subvalues]
-753
+_753
 reduced_type = reduce_types(self.infer(subvalue) for subvalue in subvalues)
-754
+_754
 r = list[reduced_type]
-755
+_755
 return r
-756
-757
+_756
+_757
 return GenericValue
-758
-759
-760
+_758
+_759
+_760
 def infer_series(self, values: Iterable[str]) -> AnyValueType:
-761
+_761
 """
-762
+_762
 Infer the underlying common type of a series of strings
-763
-764
+_763
+_764
 If the values in the series do not have the same apparent type, the resulting
 type will be narrowest possible type that will encompass all values in the
 series. See `parsetypes.reduce_types()` for more information.
-765
-766
+_765
+_766
 Parameters
-767
+_767
 ----------
-768
+_768
 `values`
-769
+_769
 : series of strings for which the type should be inferred
-770
-771
+_770
+_771
 Returns
-772
+_772
 -------
-773
+_773
 inferred type
-774
-775
+_774
+_775
 Examples
-776
+_776
 --------
-777
+_777
 ```python
-778
+_778
 parser = TypeParser()
-779
+_779
 parser.infer_series(["1", "2", "3.4"])       # float
-780
+_780
 parser.infer_series(["true", "false", "2"])  # int
-781
+_781
 parser.infer_series(["1", "2.3", "abc"])     # str
-782
+_782
 ```
-783
+_783
 """
-784
+_784
 return reduce_types(self.infer(value) for value in values)
-785
-786
-787
+_785
+_786
+_787
 def infer_table(self, rows: Iterable[Sequence[str]]) -> list[AnyValueType]:
-788
+_788
 """
-789
+_789
 Infer the underlying common type for each column of a table of strings
-790
-791
+_790
+_791
 For each column, if the values do not have the same apparent type, the
 resulting type will be narrowest possible type that will encompass all values
 in the column. See `parsetypes.reduce_types()` for more information.
-792
-793
+_792
+_793
 Note that the individual inferred types of every value in the table must be
 able to fit into memory.
-794
-795
+_794
+_795
 Parameters
-796
+_796
 ----------
-797
+_797
 `rows`
-798
+_798
 : table of strings for which the types should be inferred, in row-major order
-799
-800
+_799
+_800
 Returns
-801
+_801
 -------
-802
+_802
 inferred types
-803
-804
+_803
+_804
 Examples
-805
+_805
 --------
-806
+_806
 ```python
-807
+_807
 parser = TypeParser()
-808
+_808
 parser.infer_table([
-809
+_809
 ["1",   "true",  "1"],
-810
+_810
 ["2",   "false", "2.3"],
-811
+_811
 ["3.4", "2",     "abc"],
-812
+_812
 ])
-813
+_813
 # [float, int, str]
-814
+_814
 ```
-815
+_815
 """
-816
+_816
 rows_iter = iter(rows)
-817
+_817
 first_row = next(rows_iter, None)
-818
+_818
 if first_row is None:
-819
+_819
 return []
-820
-821
+_820
+_821
 num_cols = len(first_row)
-822
+_822
 if num_cols == 0:
-823
+_823
 return []
-824
-825
+_824
+_825
 table = _TypeTable([[self.infer(value)] for value in first_row])
-826
+_826
 for row in rows_iter:
-827
+_827
 table.add_row([self.infer(value) for value in row])
-828
-829
+_828
+_829
 return [reduce_types(col) for col in table.cols]
-830
-831
-832
-def _convert(self, value: str, t: AnyValueType) -> AnyValue:
-833
-base, type_args = _decompose_type(t)
-834
+_830
+_831
+_832
+def convert(self, value: str, target_type: AnyValueType) -> AnyValue:
+_833
+"""
+_834
+Convert a string to the specified target type if possible
+_835
+_836
+Valid values for `target_type` include any return value from `infer()`,
+`infer_series()` and `infer_table()`. To infer and convert the string
+automatically, use `parse()`, `parse_series()` or `parse_table()` instead.
+_837
+_838
+Parameters
+_839
+----------
+_840
+`value`
+_841
+: the string to be converted
+_842
+_843
+`target_type`
+_844
+: type to which the value should be converted
+_845
+_846
+Returns
+_847
+-------
+_848
+converted value
+_849
+_850
+Raises
+_851
+-------
+_852
+`ValueError`
+_853
+: if `value` cannot be converted to `target_type`
+_854
+_855
+`TypeError`
+_856
+: if `target_type` is not a valid type
+_857
+_858
+Examples
+_859
+--------
+_860
+```python
+_861
+parser = TypeParser()
+_862
+parser.convert("true", bool)  # True
+_863
+parser.convert("2", int)      # 2
+_864
+parser.convert("2", float)    # 2.
+_865
+```
+_866
+"""
+_867
+base, type_args = _decompose_type(target_type)
+_868
 if base == NoneType:
-835
-return None
-836
+_869
+return self.parse_none(value)
+_870
 elif base == bool:
-837
+_871
 return self.parse_bool(value)
-838
+_872
 elif base == int:
-839
+_873
 return self.parse_int(value)
-840
+_874
 elif base == Decimal:
-841
+_875
 return self.parse_decimal(value)
-842
+_876
 elif base == float:
-843
+_877
 return self.parse_float(value)
-844
+_878
 elif base == str:
-845
+_879
 return value
-846
+_880
 elif base == Nullable:
-847
+_881
 if self.is_none(value):
-848
+_882
 return None
-849
+_883
 else:
-850
+_884
 if type_args is not  None and len(type_args) == 1 and type_args[0] != str:
-851
+_885
 inner_type = type_args[0]
-852
-return self._convert(value, inner_type)
-853
+_886
+return self.convert(value, inner_type)
+_887
 else:
-854
+_888
 return value
-855
+_889
 elif base == list:
-856
+_890
 subvalues = value.split(self.list_delimiter)
-857
+_891
 if self.trim:
-858
+_892
 subvalues = [subvalue.strip() for subvalue in subvalues]
-859
+_893
 if type_args is not None and len(type_args) == 1 and type_args[0] != str:
-860
+_894
 subtype = type_args[0]
-861
-return [self._convert(subvalue, subtype) for subvalue in subvalues]
-862
+_895
+return [self.convert(subvalue, subtype) for subvalue in subvalues]
+_896
 else:
-863
+_897
 return subvalues
-864
+_898
 else:
-865
-return value
-866
-867
-868
+_899
+raise TypeError(f"cannot convert to type: {target_type}")
+_900
+_901
+_902
 def parse(self, value: str) -> AnyValue:
-869
+_903
 """
-870
+_904
 Parse a string and convert it to its underlying type
-871
-872
+_905
+_906
 Parameters
-873
+_907
 ----------
-874
+_908
 `value`
-875
+_909
 : the string to be parsed
-876
-877
+_910
+_911
 Returns
-878
+_912
 -------
-879
+_913
 converted value
-880
-881
+_914
+_915
 Examples
-882
+_916
 --------
-883
+_917
 ```python
-884
+_918
 parser = TypeParser()
-885
+_919
 parser.parse("true")  # True
-886
+_920
 parser.parse("2.0")   # 2.
-887
+_921
 parser.parse("abc")   # "abc"
-888
+_922
 ```
-889
+_923
 """
-890
-return self._convert(value, self.infer(value))
-891
-892
-893
+_924
+return self.convert(value, self.infer(value))
+_925
+_926
+_927
 def parse_series(self, values: Iterable[str]) -> list[AnyValue]:
-894
+_928
 """
-895
+_929
 Parse a series of strings and convert them to their underlying common type
-896
-897
+_930
+_931
 If the values in the series do not have the same apparent type, the common type
 is taken as the narrowest possible type that will encompass all values in the
 series. See `parsetypes.reduce_types()` for more information.
-898
-899
+_932
+_933
 Parameters
-900
+_934
 ----------
-901
+_935
 `values`
-902
+_936
 : series of strings to be parsed
-903
-904
+_937
+_938
 Returns
-905
+_939
 -------
-906
+_940
 converted values
-907
-908
+_941
+_942
 Examples
-909
+_943
 --------
-910
+_944
 ```python
-911
+_945
 parser = TypeParser()
-912
+_946
 parser.parse_series(["1", "2", "3"])        # [1, 2, 3]
-913
+_947
 parser.parse_series(["5", "6.7", "8."])     # [5., 6.7, 8.]
-914
+_948
 parser.parse_series(["true", "false", ""])  # [True, False, None]
-915
+_949
 parser.parse_series(["1", "2.3", "abc"])    # ["1", "2.3", "abc"]
-916
+_950
 ```
-917
+_951
 """
-918
+_952
 inferred = self.infer_series(values)
-919
-return [self._convert(value, inferred) for value in values]
-920
-921
-922
+_953
+return [self.convert(value, inferred) for value in values]
+_954
+_955
+_956
 def parse_table(self, rows: Iterable[Sequence[str]]) -> list[list[AnyValue]]:
-923
+_957
 """
-924
+_958
 Parse a table of strings and convert them to the underlying common type of each
 column
-925
-926
+_959
+_960
 For each column, if the values do not have the same apparent type, the common
 type is taken as the narrowest possible type that will encompass all values in
 the column. See `parsetypes.reduce_types()` for more information.
-927
-928
+_961
+_962
 Note that the type to which the values should be converted is determined by
 `infer_table()`, and so the individual inferred types of every value in the
 table must be able to fit into memory.
-929
-930
+_963
+_964
 This is a function that computes the entire table and returns it all at once.
 The generator `iterate_table()` behaves analogously, except that it computes
 and yields each row one at a time.
-931
-932
+_965
+_966
 Parameters
-933
+_967
 ----------
-934
+_968
 `rows`
-935
+_969
 : table of strings to be parsed, in row-major order
-936
-937
+_970
+_971
 `iterator`
-938
+_972
 : whether the parsed values should be yielded as an iterator. If False, which
 is the default, the entire table is computed and returned as a list of lists.
 If True, this function behaves as a generator, and the rows of the table are
 computed and yielded one at a time. However, note that even when set to True,
 the type inference requires that inferred type of each individual value must
 all be able to fit into memory at once.
-939
-940
+_973
+_974
 Returns
-941
+_975
 -------
-942
+_976
 converted table of values, in row-major order
-943
-944
+_977
+_978
 Examples
-945
+_979
 --------
-946
+_980
 ```python
-947
+_981
 parser = TypeParser()
-948
+_982
 table = parser.parse_table([
-949
+_983
 ["1", "5",   "true",  "1"],
-950
+_984
 ["2", "6.7", "false", "2.3"],
-951
+_985
 ["3", "8.0", "",      "abc"],
-952
+_986
 ]):
-953
+_987
 assert table == [
-954
+_988
 [1, 5.,  True,  "1"],
-955
+_989
 [2, 6.7, False, "2.3"],
-956
+_990
 [3, 8.,  None,  "abc"],
-957
+_991
 ]
-958
+_992
 ```
-959
+_993
 """
-960
+_994
 return [converted_row for converted_row in self.iterate_table(rows)]
-961
-962
-963
+_995
+_996
+_997
 def iterate_table(self, rows: Iterable[Sequence[str]]) -> Iterator[list
 [AnyValue]]:
-964
+_998
 """
-965
+_999
 Parse a table of strings for the underlying common type of each column, then
 convert and yield each row
-966
-967
+1000
+1001
 For each column, if the values do not have the same apparent type, the common
 type is taken as the narrowest possible type that will encompass all values in
 the column. See `parsetypes.reduce_types()` for more information.
-968
-969
+1002
+1003
 This is a generator that computes and yields each row one at a time. The
 function `parse_table()` behaves analogously, except that it computes the
 entire table and returns it as a list of lists. However, note that although
 this is a generator, the type to which the value sshould be converted is still
 determined by `infer_table()`, and so the individual inferred types of every
 value in the table must be able to fit into memory.
-970
-971
+1004
+1005
 Parameters
-972
+1006
 ----------
-973
+1007
 `rows`
-974
+1008
 : table of strings to be parsed, in row-major order
-975
-976
+1009
+1010
 Yields
-977
+1011
 -------
-978
+1012
 each row of converted table values
-979
-980
+1013
+1014
 Examples
-981
+1015
 --------
-982
+1016
 ```python
-983
+1017
 parser = TypeParser()
-984
+1018
 table = parser.iterate_table([
-985
+1019
 ["1",   "true",  "1"],
-986
+1020
 ["2",   "false", "2.3"],
-987
+1021
 ["3.4", "2",     "abc"],
-988
+1022
 ]):
-989
+1023
 assert next(table) == [1.,  1, "1"]
-990
+1024
 assert next(table) == [2.,  0, "2.3"]
-991
+1025
 assert next(table) == [3.4, 2, "abc"]
-992
+1026
 ```
-993
+1027
 """
-994
+1028
 inferred_types = self.infer_table(rows)
-995
-996
+1029
+1030
 for row in rows:
-997
-yield [self._convert(value, inferred) for value, inferred in zip(row,
+1031
+yield [self.convert(value, inferred) for value, inferred in zip(row,
 inferred_types)]
 A parser that can be used to infer the underlying types of data serialised as
 strings, and to convert them into their original underlying types.
 Instances of this class can be configured with different settings for the
 parser and inferrer. See the constructor for more details about the available
 options.
 ⁰
@@ -3612,61 +3676,216 @@
 parser.infer_table([
 	["1",   "true",  "1"],
 	["2",   "false", "2.3"],
 	["3.4", "2",     "abc"],
 ])
 # [float, int, str]
 ⁰
-def parse(
+def convert(
 self,
-value: str) -> Union[str, int, float, decimal.Decimal, bool, NoneType, list]:
-View Source
+value: str,
+target_type: Type[Union[str, int, float, decimal.Decimal, bool, NoneType,
+Nullable, list]]) -> Union[str, int, float, decimal.Decimal, bool, NoneType,
+list]: View Source
+832
+def convert(self, value: str, target_type: AnyValueType) -> AnyValue:
+833
+"""
+834
+Convert a string to the specified target type if possible
+835
+836
+Valid values for `target_type` include any return value from `infer()`,
+`infer_series()` and `infer_table()`. To infer and convert the string
+automatically, use `parse()`, `parse_series()` or `parse_table()` instead.
+837
+838
+Parameters
+839
+----------
+840
+`value`
+841
+: the string to be converted
+842
+843
+`target_type`
+844
+: type to which the value should be converted
+845
+846
+Returns
+847
+-------
+848
+converted value
+849
+850
+Raises
+851
+-------
+852
+`ValueError`
+853
+: if `value` cannot be converted to `target_type`
+854
+855
+`TypeError`
+856
+: if `target_type` is not a valid type
+857
+858
+Examples
+859
+--------
+860
+```python
+861
+parser = TypeParser()
+862
+parser.convert("true", bool)  # True
+863
+parser.convert("2", int)      # 2
+864
+parser.convert("2", float)    # 2.
+865
+```
+866
+"""
+867
+base, type_args = _decompose_type(target_type)
 868
-def parse(self, value: str) -> AnyValue:
+if base == NoneType:
 869
-"""
+return self.parse_none(value)
 870
-Parse a string and convert it to its underlying type
+elif base == bool:
 871
+return self.parse_bool(value)
 872
-Parameters
+elif base == int:
 873
-----------
+return self.parse_int(value)
 874
-`value`
+elif base == Decimal:
 875
-: the string to be parsed
+return self.parse_decimal(value)
 876
+elif base == float:
 877
-Returns
+return self.parse_float(value)
 878
--------
+elif base == str:
 879
-converted value
+return value
 880
+elif base == Nullable:
 881
-Examples
+if self.is_none(value):
 882
---------
+return None
 883
-```python
+else:
 884
-parser = TypeParser()
+if type_args is not  None and len(type_args) == 1 and type_args[0] != str:
 885
-parser.parse("true")  # True
+inner_type = type_args[0]
 886
-parser.parse("2.0")   # 2.
+return self.convert(value, inner_type)
 887
-parser.parse("abc")   # "abc"
+else:
 888
-```
+return value
 889
-"""
+elif base == list:
 890
-return self._convert(value, self.infer(value))
+subvalues = value.split(self.list_delimiter)
+891
+if self.trim:
+892
+subvalues = [subvalue.strip() for subvalue in subvalues]
+893
+if type_args is not None and len(type_args) == 1 and type_args[0] != str:
+894
+subtype = type_args[0]
+895
+return [self.convert(subvalue, subtype) for subvalue in subvalues]
+896
+else:
+897
+return subvalues
+898
+else:
+899
+raise TypeError(f"cannot convert to type: {target_type}")
+Convert a string to the specified target type if possible
+Valid values for target_type include any return value from infer(),
+infer_series() and infer_table(). To infer and convert the string
+automatically, use parse(), parse_series() or parse_table() instead.
+***** Parameters *****
+value : the string to be converted
+target_type : type to which the value should be converted
+***** Returns *****
+converted value
+***** Raises *****
+ValueError : if value cannot be converted to target_type
+TypeError : if target_type is not a valid type
+***** Examples *****
+parser = TypeParser()
+parser.convert("true", bool)  # True
+parser.convert("2", int)      # 2
+parser.convert("2", float)    # 2.
+⁰
+def parse(
+self,
+value: str) -> Union[str, int, float, decimal.Decimal, bool, NoneType, list]:
+View Source
+902
+def parse(self, value: str) -> AnyValue:
+903
+"""
+904
+Parse a string and convert it to its underlying type
+905
+906
+Parameters
+907
+----------
+908
+`value`
+909
+: the string to be parsed
+910
+911
+Returns
+912
+-------
+913
+converted value
+914
+915
+Examples
+916
+--------
+917
+```python
+918
+parser = TypeParser()
+919
+parser.parse("true")  # True
+920
+parser.parse("2.0")   # 2.
+921
+parser.parse("abc")   # "abc"
+922
+```
+923
+"""
+924
+return self.convert(value, self.infer(value))
 Parse a string and convert it to its underlying type
 ***** Parameters *****
 value : the string to be parsed
 ***** Returns *****
 converted value
 ***** Examples *****
 parser = TypeParser()
@@ -3674,66 +3893,66 @@
 parser.parse("2.0")   # 2.
 parser.parse("abc")   # "abc"
 ⁰
 def parse_series(
 self,
 values: Iterable[str]) -> list[typing.Union[str, int, float, decimal.Decimal,
 bool, NoneType, list]]: View Source
-893
+927
 def parse_series(self, values: Iterable[str]) -> list[AnyValue]:
-894
+928
 """
-895
+929
 Parse a series of strings and convert them to their underlying common type
-896
-897
+930
+931
 If the values in the series do not have the same apparent type, the common type
 is taken as the narrowest possible type that will encompass all values in the
 series. See `parsetypes.reduce_types()` for more information.
-898
-899
+932
+933
 Parameters
-900
+934
 ----------
-901
+935
 `values`
-902
+936
 : series of strings to be parsed
-903
-904
+937
+938
 Returns
-905
+939
 -------
-906
+940
 converted values
-907
-908
+941
+942
 Examples
-909
+943
 --------
-910
+944
 ```python
-911
+945
 parser = TypeParser()
-912
+946
 parser.parse_series(["1", "2", "3"])        # [1, 2, 3]
-913
+947
 parser.parse_series(["5", "6.7", "8."])     # [5., 6.7, 8.]
-914
+948
 parser.parse_series(["true", "false", ""])  # [True, False, None]
-915
+949
 parser.parse_series(["1", "2.3", "abc"])    # ["1", "2.3", "abc"]
-916
+950
 ```
-917
+951
 """
-918
+952
 inferred = self.infer_series(values)
-919
-return [self._convert(value, inferred) for value in values]
+953
+return [self.convert(value, inferred) for value in values]
 Parse a series of strings and convert them to their underlying common type
 If the values in the series do not have the same apparent type, the common type
 is taken as the narrowest possible type that will encompass all values in the
 series. See parsetypes.reduce_types() for more information.
 ***** Parameters *****
 values : series of strings to be parsed
 ***** Returns *****
@@ -3745,96 +3964,96 @@
 parser.parse_series(["true", "false", ""])  # [True, False, None]
 parser.parse_series(["1", "2.3", "abc"])    # ["1", "2.3", "abc"]
 ⁰
 def parse_table(
 self,
 rows: Iterable[Sequence[str]]) -> list[list[typing.Union[str, int, float,
 decimal.Decimal, bool, NoneType, list]]]: View Source
-922
+956
 def parse_table(self, rows: Iterable[Sequence[str]]) -> list[list[AnyValue]]:
-923
+957
 """
-924
+958
 Parse a table of strings and convert them to the underlying common type of each
 column
-925
-926
+959
+960
 For each column, if the values do not have the same apparent type, the common
 type is taken as the narrowest possible type that will encompass all values in
 the column. See `parsetypes.reduce_types()` for more information.
-927
-928
+961
+962
 Note that the type to which the values should be converted is determined by
 `infer_table()`, and so the individual inferred types of every value in the
 table must be able to fit into memory.
-929
-930
+963
+964
 This is a function that computes the entire table and returns it all at once.
 The generator `iterate_table()` behaves analogously, except that it computes
 and yields each row one at a time.
-931
-932
+965
+966
 Parameters
-933
+967
 ----------
-934
+968
 `rows`
-935
+969
 : table of strings to be parsed, in row-major order
-936
-937
+970
+971
 `iterator`
-938
+972
 : whether the parsed values should be yielded as an iterator. If False, which
 is the default, the entire table is computed and returned as a list of lists.
 If True, this function behaves as a generator, and the rows of the table are
 computed and yielded one at a time. However, note that even when set to True,
 the type inference requires that inferred type of each individual value must
 all be able to fit into memory at once.
-939
-940
+973
+974
 Returns
-941
+975
 -------
-942
+976
 converted table of values, in row-major order
-943
-944
+977
+978
 Examples
-945
+979
 --------
-946
+980
 ```python
-947
+981
 parser = TypeParser()
-948
+982
 table = parser.parse_table([
-949
+983
 ["1", "5",   "true",  "1"],
-950
+984
 ["2", "6.7", "false", "2.3"],
-951
+985
 ["3", "8.0", "",      "abc"],
-952
+986
 ]):
-953
+987
 assert table == [
-954
+988
 [1, 5.,  True,  "1"],
-955
+989
 [2, 6.7, False, "2.3"],
-956
+990
 [3, 8.,  None,  "abc"],
-957
+991
 ]
-958
+992
 ```
-959
+993
 """
-960
+994
 return [converted_row for converted_row in self.iterate_table(rows)]
 Parse a table of strings and convert them to the underlying common type of each
 column
 For each column, if the values do not have the same apparent type, the common
 type is taken as the narrowest possible type that will encompass all values in
 the column. See parsetypes.reduce_types() for more information.
 Note that the type to which the values should be converted is determined by
@@ -3866,87 +4085,87 @@
 	[3, 8.,  None,  "abc"],
 ]
 ⁰
 def iterate_table(
 self,
 rows: Iterable[Sequence[str]]) -> Iterator[list[Union[str, int, float,
 decimal.Decimal, bool, NoneType, list]]]: View Source
-963
+_997
 def iterate_table(self, rows: Iterable[Sequence[str]]) -> Iterator[list
 [AnyValue]]:
-964
+_998
 """
-965
+_999
 Parse a table of strings for the underlying common type of each column, then
 convert and yield each row
-966
-967
+1000
+1001
 For each column, if the values do not have the same apparent type, the common
 type is taken as the narrowest possible type that will encompass all values in
 the column. See `parsetypes.reduce_types()` for more information.
-968
-969
+1002
+1003
 This is a generator that computes and yields each row one at a time. The
 function `parse_table()` behaves analogously, except that it computes the
 entire table and returns it as a list of lists. However, note that although
 this is a generator, the type to which the value sshould be converted is still
 determined by `infer_table()`, and so the individual inferred types of every
 value in the table must be able to fit into memory.
-970
-971
+1004
+1005
 Parameters
-972
+1006
 ----------
-973
+1007
 `rows`
-974
+1008
 : table of strings to be parsed, in row-major order
-975
-976
+1009
+1010
 Yields
-977
+1011
 -------
-978
+1012
 each row of converted table values
-979
-980
+1013
+1014
 Examples
-981
+1015
 --------
-982
+1016
 ```python
-983
+1017
 parser = TypeParser()
-984
+1018
 table = parser.iterate_table([
-985
+1019
 ["1",   "true",  "1"],
-986
+1020
 ["2",   "false", "2.3"],
-987
+1021
 ["3.4", "2",     "abc"],
-988
+1022
 ]):
-989
+1023
 assert next(table) == [1.,  1, "1"]
-990
+1024
 assert next(table) == [2.,  0, "2.3"]
-991
+1025
 assert next(table) == [3.4, 2, "abc"]
-992
+1026
 ```
-993
+1027
 """
-994
+1028
 inferred_types = self.infer_table(rows)
-995
-996
+1029
+1030
 for row in rows:
-997
-yield [self._convert(value, inferred) for value, inferred in zip(row,
+1031
+yield [self.convert(value, inferred) for value, inferred in zip(row,
 inferred_types)]
 Parse a table of strings for the underlying common type of each column, then
 convert and yield each row
 For each column, if the values do not have the same apparent type, the common
 type is taken as the narrowest possible type that will encompass all values in
 the column. See parsetypes.reduce_types() for more information.
 This is a generator that computes and yields each row one at a time. The
```

### Comparing `parsetypes-0.2.3/docs/html/search.js` & `parsetypes-0.2.4/docs/html/search.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -822,14 +822,23 @@
                     "modulename": "parsetypes",
                     "qualname": "TypeParser.infer_table",
                     "kind": "function",
                     "doc": "<p>Infer the underlying common type for each column of a table of strings</p>\n\n<p>For each column, if the values do not have the same apparent type, the resulting type will be narrowest possible type that will encompass all values in the column. See <code>parsetypes.reduce_types()</code> for more information.</p>\n\n<p>Note that the individual inferred types of every value in the table must be able to fit into memory.</p>\n\n<h2 id=\"parameters\">Parameters</h2>\n\n<p><code>rows</code>\n: table of strings for which the types should be inferred, in row-major order</p>\n\n<h2 id=\"returns\">Returns</h2>\n\n<p>inferred types</p>\n\n<h2 id=\"examples\">Examples</h2>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"n\">parser</span> <span class=\"o\">=</span> <span class=\"n\">TypeParser</span><span class=\"p\">()</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">infer_table</span><span class=\"p\">([</span>\n        <span class=\"p\">[</span><span class=\"s2\">&quot;1&quot;</span><span class=\"p\">,</span>   <span class=\"s2\">&quot;true&quot;</span><span class=\"p\">,</span>  <span class=\"s2\">&quot;1&quot;</span><span class=\"p\">],</span>\n        <span class=\"p\">[</span><span class=\"s2\">&quot;2&quot;</span><span class=\"p\">,</span>   <span class=\"s2\">&quot;false&quot;</span><span class=\"p\">,</span> <span class=\"s2\">&quot;2.3&quot;</span><span class=\"p\">],</span>\n        <span class=\"p\">[</span><span class=\"s2\">&quot;3.4&quot;</span><span class=\"p\">,</span> <span class=\"s2\">&quot;2&quot;</span><span class=\"p\">,</span>     <span class=\"s2\">&quot;abc&quot;</span><span class=\"p\">],</span>\n<span class=\"p\">])</span>\n<span class=\"c1\"># [float, int, str]</span>\n</code></pre>\n</div>\n",
                     "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"bp\">self</span>,</span><span class=\"param\">\t<span class=\"n\">rows</span><span class=\"p\">:</span> <span class=\"n\">Iterable</span><span class=\"p\">[</span><span class=\"n\">Sequence</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]]</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"n\">typing</span><span class=\"o\">.</span><span class=\"n\">Type</span><span class=\"p\">[</span><span class=\"n\">typing</span><span class=\"o\">.</span><span class=\"n\">Union</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">,</span> <span class=\"nb\">int</span><span class=\"p\">,</span> <span class=\"nb\">float</span><span class=\"p\">,</span> <span class=\"n\">decimal</span><span class=\"o\">.</span><span class=\"n\">Decimal</span><span class=\"p\">,</span> <span class=\"nb\">bool</span><span class=\"p\">,</span> <span class=\"n\">NoneType</span><span class=\"p\">,</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">,</span> <span class=\"nb\">list</span><span class=\"p\">]]]</span>:</span></span>",
                     "funcdef": "def"
                 },
+                "parsetypes.TypeParser.convert": {
+                    "fullname": "parsetypes.TypeParser.convert",
+                    "modulename": "parsetypes",
+                    "qualname": "TypeParser.convert",
+                    "kind": "function",
+                    "doc": "<p>Convert a string to the specified target type if possible</p>\n\n<p>Valid values for <code>target_type</code> include any return value from <code>infer()</code>, <code>infer_series()</code> and <code>infer_table()</code>. To infer and convert the string automatically, use <code>parse()</code>, <code>parse_series()</code> or <code>parse_table()</code> instead.</p>\n\n<h2 id=\"parameters\">Parameters</h2>\n\n<p><code>value</code>\n: the string to be converted</p>\n\n<p><code>target_type</code>\n: type to which the value should be converted</p>\n\n<h2 id=\"returns\">Returns</h2>\n\n<p>converted value</p>\n\n<h2 id=\"raises\">Raises</h2>\n\n<p><code>ValueError</code>\n: if <code>value</code> cannot be converted to <code>target_type</code></p>\n\n<p><code>TypeError</code>\n: if <code>target_type</code> is not a valid type</p>\n\n<h2 id=\"examples\">Examples</h2>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"n\">parser</span> <span class=\"o\">=</span> <span class=\"n\">TypeParser</span><span class=\"p\">()</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">convert</span><span class=\"p\">(</span><span class=\"s2\">&quot;true&quot;</span><span class=\"p\">,</span> <span class=\"nb\">bool</span><span class=\"p\">)</span>  <span class=\"c1\"># True</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">convert</span><span class=\"p\">(</span><span class=\"s2\">&quot;2&quot;</span><span class=\"p\">,</span> <span class=\"nb\">int</span><span class=\"p\">)</span>      <span class=\"c1\"># 2</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">convert</span><span class=\"p\">(</span><span class=\"s2\">&quot;2&quot;</span><span class=\"p\">,</span> <span class=\"nb\">float</span><span class=\"p\">)</span>    <span class=\"c1\"># 2.</span>\n</code></pre>\n</div>\n",
+                    "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"bp\">self</span>,</span><span class=\"param\">\t<span class=\"n\">value</span><span class=\"p\">:</span> <span class=\"nb\">str</span>,</span><span class=\"param\">\t<span class=\"n\">target_type</span><span class=\"p\">:</span> <span class=\"n\">Type</span><span class=\"p\">[</span><span class=\"n\">Union</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">,</span> <span class=\"nb\">int</span><span class=\"p\">,</span> <span class=\"nb\">float</span><span class=\"p\">,</span> <span class=\"n\">decimal</span><span class=\"o\">.</span><span class=\"n\">Decimal</span><span class=\"p\">,</span> <span class=\"nb\">bool</span><span class=\"p\">,</span> <span class=\"n\">NoneType</span><span class=\"p\">,</span> <span class=\"n\">parsetypes</span><span class=\"o\">.</span><span class=\"n\">_common</span><span class=\"o\">.</span><span class=\"n\">Nullable</span><span class=\"p\">,</span> <span class=\"nb\">list</span><span class=\"p\">]]</span></span><span class=\"return-annotation\">) -> <span class=\"n\">Union</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">,</span> <span class=\"nb\">int</span><span class=\"p\">,</span> <span class=\"nb\">float</span><span class=\"p\">,</span> <span class=\"n\">decimal</span><span class=\"o\">.</span><span class=\"n\">Decimal</span><span class=\"p\">,</span> <span class=\"nb\">bool</span><span class=\"p\">,</span> <span class=\"n\">NoneType</span><span class=\"p\">,</span> <span class=\"nb\">list</span><span class=\"p\">]</span>:</span></span>",
+                    "funcdef": "def"
+                },
                 "parsetypes.TypeParser.parse": {
                     "fullname": "parsetypes.TypeParser.parse",
                     "modulename": "parsetypes",
                     "qualname": "TypeParser.parse",
                     "kind": "function",
                     "doc": "<p>Parse a string and convert it to its underlying type</p>\n\n<h2 id=\"parameters\">Parameters</h2>\n\n<p><code>value</code>\n: the string to be parsed</p>\n\n<h2 id=\"returns\">Returns</h2>\n\n<p>converted value</p>\n\n<h2 id=\"examples\">Examples</h2>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"n\">parser</span> <span class=\"o\">=</span> <span class=\"n\">TypeParser</span><span class=\"p\">()</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">parse</span><span class=\"p\">(</span><span class=\"s2\">&quot;true&quot;</span><span class=\"p\">)</span>  <span class=\"c1\"># True</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">parse</span><span class=\"p\">(</span><span class=\"s2\">&quot;2.0&quot;</span><span class=\"p\">)</span>   <span class=\"c1\"># 2.</span>\n<span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">parse</span><span class=\"p\">(</span><span class=\"s2\">&quot;abc&quot;</span><span class=\"p\">)</span>   <span class=\"c1\"># &quot;abc&quot;</span>\n</code></pre>\n</div>\n",
                     "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"bp\">self</span>,</span><span class=\"param\">\t<span class=\"n\">value</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">) -> <span class=\"n\">Union</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">,</span> <span class=\"nb\">int</span><span class=\"p\">,</span> <span class=\"nb\">float</span><span class=\"p\">,</span> <span class=\"n\">decimal</span><span class=\"o\">.</span><span class=\"n\">Decimal</span><span class=\"p\">,</span> <span class=\"nb\">bool</span><span class=\"p\">,</span> <span class=\"n\">NoneType</span><span class=\"p\">,</span> <span class=\"nb\">list</span><span class=\"p\">]</span>:</span></span>",
@@ -1013,14 +1022,23 @@
                     "fullname": 4,
                     "annotation": 0,
                     "default_value": 0,
                     "signature": 118,
                     "bases": 0,
                     "doc": 256
                 },
+                "parsetypes.TypeParser.convert": {
+                    "qualname": 2,
+                    "fullname": 3,
+                    "annotation": 0,
+                    "default_value": 0,
+                    "signature": 153,
+                    "bases": 0,
+                    "doc": 257
+                },
                 "parsetypes.TypeParser.parse": {
                     "qualname": 2,
                     "fullname": 3,
                     "annotation": 0,
                     "default_value": 0,
                     "signature": 73,
                     "bases": 0,
@@ -1059,15 +1077,15 @@
                     "annotation": 0,
                     "default_value": 0,
                     "signature": 160,
                     "bases": 0,
                     "doc": 188
                 }
             },
-            "length": 21,
+            "length": 22,
             "save": true
         },
         "index": {
             "qualname": {
                 "root": {
                     "docs": {
                         "parsetypes.TypeParser.__init__": {
@@ -1145,28 +1163,31 @@
                                                                 },
                                                                 "parsetypes.TypeParser.infer_series": {
                                                                     "tf": 1
                                                                 },
                                                                 "parsetypes.TypeParser.infer_table": {
                                                                     "tf": 1
                                                                 },
+                                                                "parsetypes.TypeParser.convert": {
+                                                                    "tf": 1
+                                                                },
                                                                 "parsetypes.TypeParser.parse": {
                                                                     "tf": 1
                                                                 },
                                                                 "parsetypes.TypeParser.parse_series": {
                                                                     "tf": 1
                                                                 },
                                                                 "parsetypes.TypeParser.parse_table": {
                                                                     "tf": 1
                                                                 },
                                                                 "parsetypes.TypeParser.iterate_table": {
                                                                     "tf": 1
                                                                 }
                                                             },
-                                                            "df": 19
+                                                            "df": 20
                                                         }
                                                     }
                                                 }
                                             }
                                         }
                                     },
                                     "s": {
@@ -1488,14 +1509,46 @@
                                             "df": 2
                                         }
                                     }
                                 }
                             }
                         }
                     },
+                    "c": {
+                        "docs": {},
+                        "df": 0,
+                        "o": {
+                            "docs": {},
+                            "df": 0,
+                            "n": {
+                                "docs": {},
+                                "df": 0,
+                                "v": {
+                                    "docs": {},
+                                    "df": 0,
+                                    "e": {
+                                        "docs": {},
+                                        "df": 0,
+                                        "r": {
+                                            "docs": {},
+                                            "df": 0,
+                                            "t": {
+                                                "docs": {
+                                                    "parsetypes.TypeParser.convert": {
+                                                        "tf": 1
+                                                    }
+                                                },
+                                                "df": 1
+                                            }
+                                        }
+                                    }
+                                }
+                            }
+                        }
+                    },
                     "r": {
                         "docs": {},
                         "df": 0,
                         "e": {
                             "docs": {},
                             "df": 0,
                             "d": {
@@ -1628,14 +1681,17 @@
                                                                 },
                                                                 "parsetypes.TypeParser.infer_series": {
                                                                     "tf": 1
                                                                 },
                                                                 "parsetypes.TypeParser.infer_table": {
                                                                     "tf": 1
                                                                 },
+                                                                "parsetypes.TypeParser.convert": {
+                                                                    "tf": 1
+                                                                },
                                                                 "parsetypes.TypeParser.parse": {
                                                                     "tf": 1
                                                                 },
                                                                 "parsetypes.TypeParser.parse_series": {
                                                                     "tf": 1
                                                                 },
                                                                 "parsetypes.TypeParser.parse_table": {
@@ -1644,15 +1700,15 @@
                                                                 "parsetypes.TypeParser.iterate_table": {
                                                                     "tf": 1
                                                                 },
                                                                 "parsetypes.reduce_types": {
                                                                     "tf": 1
                                                                 }
                                                             },
-                                                            "df": 21
+                                                            "df": 22
                                                         }
                                                     }
                                                 }
                                             }
                                         }
                                     }
                                 }
@@ -1729,28 +1785,31 @@
                                                                 },
                                                                 "parsetypes.TypeParser.infer_series": {
                                                                     "tf": 1
                                                                 },
                                                                 "parsetypes.TypeParser.infer_table": {
                                                                     "tf": 1
                                                                 },
+                                                                "parsetypes.TypeParser.convert": {
+                                                                    "tf": 1
+                                                                },
                                                                 "parsetypes.TypeParser.parse": {
                                                                     "tf": 1
                                                                 },
                                                                 "parsetypes.TypeParser.parse_series": {
                                                                     "tf": 1
                                                                 },
                                                                 "parsetypes.TypeParser.parse_table": {
                                                                     "tf": 1
                                                                 },
                                                                 "parsetypes.TypeParser.iterate_table": {
                                                                     "tf": 1
                                                                 }
                                                             },
-                                                            "df": 19
+                                                            "df": 20
                                                         }
                                                     }
                                                 }
                                             }
                                         }
                                     },
                                     "s": {
@@ -2027,14 +2086,46 @@
                                             "df": 2
                                         }
                                     }
                                 }
                             }
                         }
                     },
+                    "c": {
+                        "docs": {},
+                        "df": 0,
+                        "o": {
+                            "docs": {},
+                            "df": 0,
+                            "n": {
+                                "docs": {},
+                                "df": 0,
+                                "v": {
+                                    "docs": {},
+                                    "df": 0,
+                                    "e": {
+                                        "docs": {},
+                                        "df": 0,
+                                        "r": {
+                                            "docs": {},
+                                            "df": 0,
+                                            "t": {
+                                                "docs": {
+                                                    "parsetypes.TypeParser.convert": {
+                                                        "tf": 1
+                                                    }
+                                                },
+                                                "df": 1
+                                            }
+                                        }
+                                    }
+                                }
+                            }
+                        }
+                    },
                     "r": {
                         "docs": {},
                         "df": 0,
                         "e": {
                             "docs": {},
                             "df": 0,
                             "d": {
@@ -2126,14 +2217,17 @@
                         },
                         "parsetypes.TypeParser.infer_series": {
                             "tf": 9.1104335791443
                         },
                         "parsetypes.TypeParser.infer_table": {
                             "tf": 9.848857801796104
                         },
+                        "parsetypes.TypeParser.convert": {
+                            "tf": 11.224972160321824
+                        },
                         "parsetypes.TypeParser.parse": {
                             "tf": 7.810249675906654
                         },
                         "parsetypes.TypeParser.parse_series": {
                             "tf": 8.54400374531753
                         },
                         "parsetypes.TypeParser.parse_table": {
@@ -2142,15 +2236,15 @@
                         "parsetypes.TypeParser.iterate_table": {
                             "tf": 8.660254037844387
                         },
                         "parsetypes.reduce_types": {
                             "tf": 11.489125293076057
                         }
                     },
-                    "df": 19,
+                    "df": 20,
                     "t": {
                         "docs": {},
                         "df": 0,
                         "r": {
                             "docs": {},
                             "df": 0,
                             "i": {
@@ -2209,19 +2303,22 @@
                                         },
                                         "parsetypes.TypeParser.infer_series": {
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser.infer_table": {
                                             "tf": 1
                                         },
+                                        "parsetypes.TypeParser.convert": {
+                                            "tf": 1.4142135623730951
+                                        },
                                         "parsetypes.reduce_types": {
                                             "tf": 1.4142135623730951
                                         }
                                     },
-                                    "df": 4,
+                                    "df": 5,
                                     "s": {
                                         "docs": {
                                             "parsetypes.reduce_types": {
                                                 "tf": 1
                                             }
                                         },
                                         "df": 1
@@ -2246,14 +2343,38 @@
                                                 }
                                             },
                                             "df": 3
                                         }
                                     }
                                 }
                             }
+                        },
+                        "a": {
+                            "docs": {},
+                            "df": 0,
+                            "r": {
+                                "docs": {},
+                                "df": 0,
+                                "g": {
+                                    "docs": {},
+                                    "df": 0,
+                                    "e": {
+                                        "docs": {},
+                                        "df": 0,
+                                        "t": {
+                                            "docs": {
+                                                "parsetypes.TypeParser.convert": {
+                                                    "tf": 1
+                                                }
+                                            },
+                                            "df": 1
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
@@ -2298,14 +2419,17 @@
                                         },
                                         "parsetypes.TypeParser.infer_series": {
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser.infer_table": {
                                             "tf": 1
                                         },
+                                        "parsetypes.TypeParser.convert": {
+                                            "tf": 1.4142135623730951
+                                        },
                                         "parsetypes.TypeParser.parse": {
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser.parse_series": {
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser.parse_table": {
@@ -2314,15 +2438,15 @@
                                         "parsetypes.TypeParser.iterate_table": {
                                             "tf": 1
                                         },
                                         "parsetypes.reduce_types": {
                                             "tf": 1.4142135623730951
                                         }
                                     },
-                                    "df": 18
+                                    "df": 19
                                 }
                             }
                         }
                     },
                     "u": {
                         "docs": {},
                         "df": 0,
@@ -2354,14 +2478,17 @@
                                             },
                                             "parsetypes.TypeParser.infer_series": {
                                                 "tf": 1
                                             },
                                             "parsetypes.TypeParser.infer_table": {
                                                 "tf": 1
                                             },
+                                            "parsetypes.TypeParser.convert": {
+                                                "tf": 1.4142135623730951
+                                            },
                                             "parsetypes.TypeParser.parse": {
                                                 "tf": 1
                                             },
                                             "parsetypes.TypeParser.parse_series": {
                                                 "tf": 1
                                             },
                                             "parsetypes.TypeParser.parse_table": {
@@ -2370,15 +2497,15 @@
                                             "parsetypes.TypeParser.iterate_table": {
                                                 "tf": 1
                                             },
                                             "parsetypes.reduce_types": {
                                                 "tf": 1.4142135623730951
                                             }
                                         },
-                                        "df": 8
+                                        "df": 9
                                     }
                                 }
                             }
                         }
                     },
                     "d": {
                         "docs": {},
@@ -2411,14 +2538,17 @@
                                                     },
                                                     "parsetypes.TypeParser.infer_series": {
                                                         "tf": 1.4142135623730951
                                                     },
                                                     "parsetypes.TypeParser.infer_table": {
                                                         "tf": 1.4142135623730951
                                                     },
+                                                    "parsetypes.TypeParser.convert": {
+                                                        "tf": 2
+                                                    },
                                                     "parsetypes.TypeParser.parse": {
                                                         "tf": 1.4142135623730951
                                                     },
                                                     "parsetypes.TypeParser.parse_series": {
                                                         "tf": 1.4142135623730951
                                                     },
                                                     "parsetypes.TypeParser.parse_table": {
@@ -2427,15 +2557,15 @@
                                                     "parsetypes.TypeParser.iterate_table": {
                                                         "tf": 1.4142135623730951
                                                     },
                                                     "parsetypes.reduce_types": {
                                                         "tf": 2
                                                     }
                                                 },
-                                                "df": 10
+                                                "df": 11
                                             }
                                         }
                                     }
                                 }
                             },
                             "l": {
                                 "docs": {},
@@ -2516,14 +2646,17 @@
                                             },
                                             "parsetypes.TypeParser.infer_series": {
                                                 "tf": 1
                                             },
                                             "parsetypes.TypeParser.infer_table": {
                                                 "tf": 1
                                             },
+                                            "parsetypes.TypeParser.convert": {
+                                                "tf": 1.4142135623730951
+                                            },
                                             "parsetypes.TypeParser.parse": {
                                                 "tf": 1
                                             },
                                             "parsetypes.TypeParser.parse_series": {
                                                 "tf": 1
                                             },
                                             "parsetypes.TypeParser.parse_table": {
@@ -2532,15 +2665,15 @@
                                             "parsetypes.TypeParser.iterate_table": {
                                                 "tf": 1
                                             },
                                             "parsetypes.reduce_types": {
                                                 "tf": 1.4142135623730951
                                             }
                                         },
-                                        "df": 10
+                                        "df": 11
                                     }
                                 }
                             }
                         }
                     },
                     "l": {
                         "docs": {},
@@ -2561,14 +2694,17 @@
                                         },
                                         "parsetypes.TypeParser.infer_series": {
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser.infer_table": {
                                             "tf": 1.4142135623730951
                                         },
+                                        "parsetypes.TypeParser.convert": {
+                                            "tf": 1.4142135623730951
+                                        },
                                         "parsetypes.TypeParser.parse": {
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser.parse_series": {
                                             "tf": 1.4142135623730951
                                         },
                                         "parsetypes.TypeParser.parse_table": {
@@ -2577,15 +2713,15 @@
                                         "parsetypes.TypeParser.iterate_table": {
                                             "tf": 1.4142135623730951
                                         },
                                         "parsetypes.reduce_types": {
                                             "tf": 1.4142135623730951
                                         }
                                     },
-                                    "df": 9
+                                    "df": 10
                                 }
                             }
                         }
                     },
                     "o": {
                         "docs": {},
                         "df": 0,
@@ -2668,14 +2804,17 @@
                                     },
                                     "parsetypes.TypeParser.infer_series": {
                                         "tf": 1.4142135623730951
                                     },
                                     "parsetypes.TypeParser.infer_table": {
                                         "tf": 1.4142135623730951
                                     },
+                                    "parsetypes.TypeParser.convert": {
+                                        "tf": 1.7320508075688772
+                                    },
                                     "parsetypes.TypeParser.parse": {
                                         "tf": 1.4142135623730951
                                     },
                                     "parsetypes.TypeParser.parse_series": {
                                         "tf": 1.4142135623730951
                                     },
                                     "parsetypes.TypeParser.parse_table": {
@@ -2684,15 +2823,15 @@
                                     "parsetypes.TypeParser.iterate_table": {
                                         "tf": 1.4142135623730951
                                     },
                                     "parsetypes.reduce_types": {
                                         "tf": 1.4142135623730951
                                     }
                                 },
-                                "df": 19
+                                "df": 20
                             }
                         },
                         "e": {
                             "docs": {},
                             "df": 0,
                             "n": {
                                 "docs": {},
@@ -2766,28 +2905,31 @@
                                         },
                                         "parsetypes.TypeParser.infer_series": {
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser.infer_table": {
                                             "tf": 1
                                         },
+                                        "parsetypes.TypeParser.convert": {
+                                            "tf": 1
+                                        },
                                         "parsetypes.TypeParser.parse": {
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser.parse_series": {
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser.parse_table": {
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser.iterate_table": {
                                             "tf": 1
                                         }
                                     },
-                                    "df": 17
+                                    "df": 18
                                 }
                             },
                             "q": {
                                 "docs": {},
                                 "df": 0,
                                 "u": {
                                     "docs": {},
@@ -2928,14 +3070,17 @@
                                                         },
                                                         "parsetypes.TypeParser.infer_series": {
                                                             "tf": 1
                                                         },
                                                         "parsetypes.TypeParser.infer_table": {
                                                             "tf": 1
                                                         },
+                                                        "parsetypes.TypeParser.convert": {
+                                                            "tf": 1.4142135623730951
+                                                        },
                                                         "parsetypes.TypeParser.parse": {
                                                             "tf": 1
                                                         },
                                                         "parsetypes.TypeParser.parse_series": {
                                                             "tf": 1
                                                         },
                                                         "parsetypes.TypeParser.parse_table": {
@@ -2944,15 +3089,15 @@
                                                         "parsetypes.TypeParser.iterate_table": {
                                                             "tf": 1
                                                         },
                                                         "parsetypes.reduce_types": {
                                                             "tf": 1.4142135623730951
                                                         }
                                                     },
-                                                    "df": 8
+                                                    "df": 9
                                                 }
                                             }
                                         }
                                     }
                                 }
                             }
                         },
@@ -3037,19 +3182,22 @@
                                                         },
                                                         "parsetypes.TypeParser.infer_series": {
                                                             "tf": 1
                                                         },
                                                         "parsetypes.TypeParser.infer_table": {
                                                             "tf": 1
                                                         },
+                                                        "parsetypes.TypeParser.convert": {
+                                                            "tf": 1
+                                                        },
                                                         "parsetypes.reduce_types": {
                                                             "tf": 1.4142135623730951
                                                         }
                                                     },
-                                                    "df": 4
+                                                    "df": 5
                                                 }
                                             }
                                         }
                                     }
                                 }
                             }
                         }
@@ -3097,19 +3245,22 @@
                                             },
                                             "parsetypes.TypeParser.parse_decimal": {
                                                 "tf": 1
                                             },
                                             "parsetypes.TypeParser.infer": {
                                                 "tf": 1
                                             },
+                                            "parsetypes.TypeParser.convert": {
+                                                "tf": 1
+                                            },
                                             "parsetypes.TypeParser.parse": {
                                                 "tf": 1
                                             }
                                         },
-                                        "df": 12,
+                                        "df": 13,
                                         "s": {
                                             "docs": {
                                                 "parsetypes.TypeParser.__init__": {
                                                     "tf": 2.23606797749979
                                                 },
                                                 "parsetypes.TypeParser.infer_series": {
                                                     "tf": 1
@@ -3210,14 +3361,17 @@
                                     },
                                     "parsetypes.TypeParser.infer_series": {
                                         "tf": 1
                                     },
                                     "parsetypes.TypeParser.infer_table": {
                                         "tf": 1
                                     },
+                                    "parsetypes.TypeParser.convert": {
+                                        "tf": 1.4142135623730951
+                                    },
                                     "parsetypes.TypeParser.parse": {
                                         "tf": 1
                                     },
                                     "parsetypes.TypeParser.parse_series": {
                                         "tf": 1
                                     },
                                     "parsetypes.TypeParser.parse_table": {
@@ -3226,15 +3380,15 @@
                                     "parsetypes.TypeParser.iterate_table": {
                                         "tf": 1
                                     },
                                     "parsetypes.reduce_types": {
                                         "tf": 1.4142135623730951
                                     }
                                 },
-                                "df": 10
+                                "df": 11
                             },
                             "f": {
                                 "docs": {
                                     "parsetypes.TypeParser.__init__": {
                                         "tf": 1
                                     },
                                     "parsetypes.TypeParser.is_float": {
@@ -3292,19 +3446,22 @@
                                                 },
                                                 "parsetypes.TypeParser.infer_series": {
                                                     "tf": 1
                                                 },
                                                 "parsetypes.TypeParser.infer_table": {
                                                     "tf": 1
                                                 },
+                                                "parsetypes.TypeParser.convert": {
+                                                    "tf": 1
+                                                },
                                                 "parsetypes.reduce_types": {
                                                     "tf": 1.4142135623730951
                                                 }
                                             },
-                                            "df": 4
+                                            "df": 5
                                         }
                                     }
                                 }
                             }
                         }
                     },
                     "a": {
@@ -3380,19 +3537,22 @@
                                                                 },
                                                                 "parsetypes.TypeParser.infer_series": {
                                                                     "tf": 1
                                                                 },
                                                                 "parsetypes.TypeParser.infer_table": {
                                                                     "tf": 1
                                                                 },
+                                                                "parsetypes.TypeParser.convert": {
+                                                                    "tf": 1
+                                                                },
                                                                 "parsetypes.reduce_types": {
                                                                     "tf": 1.4142135623730951
                                                                 }
                                                             },
-                                                            "df": 4
+                                                            "df": 5
                                                         }
                                                     }
                                                 }
                                             }
                                         }
                                     }
                                 }
@@ -3628,28 +3788,31 @@
                             },
                             "parsetypes.TypeParser.infer_series": {
                                 "tf": 1.7320508075688772
                             },
                             "parsetypes.TypeParser.infer_table": {
                                 "tf": 1.7320508075688772
                             },
+                            "parsetypes.TypeParser.convert": {
+                                "tf": 2
+                            },
                             "parsetypes.TypeParser.parse": {
                                 "tf": 1.4142135623730951
                             },
                             "parsetypes.TypeParser.parse_series": {
                                 "tf": 2
                             },
                             "parsetypes.TypeParser.parse_table": {
                                 "tf": 2
                             },
                             "parsetypes.TypeParser.iterate_table": {
                                 "tf": 2.449489742783178
                             }
                         },
-                        "df": 10,
+                        "df": 11,
                         "e": {
                             "3": {
                                 "docs": {
                                     "parsetypes.TypeParser.parse_int": {
                                         "tf": 1
                                     }
                                 },
@@ -3790,14 +3953,17 @@
                         },
                         "parsetypes.TypeParser.infer_series": {
                             "tf": 11.789826122551595
                         },
                         "parsetypes.TypeParser.infer_table": {
                             "tf": 11.445523142259598
                         },
+                        "parsetypes.TypeParser.convert": {
+                            "tf": 12.36931687685298
+                        },
                         "parsetypes.TypeParser.parse": {
                             "tf": 9.643650760992955
                         },
                         "parsetypes.TypeParser.parse_series": {
                             "tf": 13.19090595827292
                         },
                         "parsetypes.TypeParser.parse_table": {
@@ -3806,15 +3972,15 @@
                         "parsetypes.TypeParser.iterate_table": {
                             "tf": 15.524174696260024
                         },
                         "parsetypes.reduce_types": {
                             "tf": 9.433981132056603
                         }
                     },
-                    "df": 21,
+                    "df": 22,
                     "t": {
                         "docs": {},
                         "df": 0,
                         "h": {
                             "docs": {},
                             "df": 0,
                             "i": {
@@ -3908,14 +4074,17 @@
                                     },
                                     "parsetypes.TypeParser.infer_series": {
                                         "tf": 2.6457513110645907
                                     },
                                     "parsetypes.TypeParser.infer_table": {
                                         "tf": 2.8284271247461903
                                     },
+                                    "parsetypes.TypeParser.convert": {
+                                        "tf": 2
+                                    },
                                     "parsetypes.TypeParser.parse": {
                                         "tf": 1
                                     },
                                     "parsetypes.TypeParser.parse_series": {
                                         "tf": 2.449489742783178
                                     },
                                     "parsetypes.TypeParser.parse_table": {
@@ -3924,15 +4093,15 @@
                                     "parsetypes.TypeParser.iterate_table": {
                                         "tf": 3.4641016151377544
                                     },
                                     "parsetypes.reduce_types": {
                                         "tf": 2.23606797749979
                                     }
                                 },
-                                "df": 20,
+                                "df": 21,
                                 "i": {
                                     "docs": {},
                                     "df": 0,
                                     "r": {
                                         "docs": {
                                             "parsetypes": {
                                                 "tf": 1
@@ -4065,14 +4234,17 @@
                                 },
                                 "parsetypes.TypeParser.parse_decimal": {
                                     "tf": 2.6457513110645907
                                 },
                                 "parsetypes.TypeParser.infer_table": {
                                     "tf": 1
                                 },
+                                "parsetypes.TypeParser.convert": {
+                                    "tf": 2.23606797749979
+                                },
                                 "parsetypes.TypeParser.parse": {
                                     "tf": 1.4142135623730951
                                 },
                                 "parsetypes.TypeParser.parse_series": {
                                     "tf": 1.4142135623730951
                                 },
                                 "parsetypes.TypeParser.parse_table": {
@@ -4081,15 +4253,15 @@
                                 "parsetypes.TypeParser.iterate_table": {
                                     "tf": 1.7320508075688772
                                 },
                                 "parsetypes.reduce_types": {
                                     "tf": 1
                                 }
                             },
-                            "df": 18,
+                            "df": 19,
                             "o": {
                                 "docs": {},
                                 "df": 0,
                                 "l": {
                                     "docs": {},
                                     "df": 0,
                                     "s": {
@@ -4122,14 +4294,17 @@
                                         },
                                         "parsetypes.TypeParser.infer_series": {
                                             "tf": 2.449489742783178
                                         },
                                         "parsetypes.TypeParser.infer_table": {
                                             "tf": 2
                                         },
+                                        "parsetypes.TypeParser.convert": {
+                                            "tf": 2.6457513110645907
+                                        },
                                         "parsetypes.TypeParser.parse": {
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser.parse_series": {
                                             "tf": 2
                                         },
                                         "parsetypes.TypeParser.parse_table": {
@@ -4138,15 +4313,15 @@
                                         "parsetypes.TypeParser.iterate_table": {
                                             "tf": 2.23606797749979
                                         },
                                         "parsetypes.reduce_types": {
                                             "tf": 2.23606797749979
                                         }
                                     },
-                                    "df": 10,
+                                    "df": 11,
                                     "s": {
                                         "docs": {
                                             "parsetypes": {
                                                 "tf": 1
                                             },
                                             "parsetypes.TypeParser": {
                                                 "tf": 1.4142135623730951
@@ -4227,33 +4402,60 @@
                                                                 },
                                                                 "parsetypes.TypeParser.infer_series": {
                                                                     "tf": 1
                                                                 },
                                                                 "parsetypes.TypeParser.infer_table": {
                                                                     "tf": 1
                                                                 },
+                                                                "parsetypes.TypeParser.convert": {
+                                                                    "tf": 1
+                                                                },
                                                                 "parsetypes.TypeParser.parse": {
                                                                     "tf": 1
                                                                 },
                                                                 "parsetypes.TypeParser.parse_series": {
                                                                     "tf": 1
                                                                 },
                                                                 "parsetypes.TypeParser.parse_table": {
                                                                     "tf": 1
                                                                 },
                                                                 "parsetypes.TypeParser.iterate_table": {
                                                                     "tf": 1
                                                                 }
                                                             },
-                                                            "df": 17
+                                                            "df": 18
                                                         }
                                                     }
                                                 }
                                             }
                                         }
+                                    },
+                                    "e": {
+                                        "docs": {},
+                                        "df": 0,
+                                        "r": {
+                                            "docs": {},
+                                            "df": 0,
+                                            "r": {
+                                                "docs": {},
+                                                "df": 0,
+                                                "o": {
+                                                    "docs": {},
+                                                    "df": 0,
+                                                    "r": {
+                                                        "docs": {
+                                                            "parsetypes.TypeParser.convert": {
+                                                                "tf": 1
+                                                            }
+                                                        },
+                                                        "df": 1
+                                                    }
+                                                }
+                                            }
+                                        }
                                     }
                                 }
                             }
                         },
                         "r": {
                             "docs": {},
                             "df": 0,
@@ -4362,28 +4564,31 @@
                                         },
                                         "parsetypes.TypeParser.infer_series": {
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser.infer_table": {
                                             "tf": 1
                                         },
+                                        "parsetypes.TypeParser.convert": {
+                                            "tf": 1.4142135623730951
+                                        },
                                         "parsetypes.TypeParser.parse": {
                                             "tf": 1.4142135623730951
                                         },
                                         "parsetypes.TypeParser.parse_series": {
                                             "tf": 1.4142135623730951
                                         },
                                         "parsetypes.TypeParser.parse_table": {
                                             "tf": 2
                                         },
                                         "parsetypes.TypeParser.iterate_table": {
                                             "tf": 1
                                         }
                                     },
-                                    "df": 16
+                                    "df": 17
                                 }
                             }
                         },
                         "a": {
                             "docs": {},
                             "df": 0,
                             "b": {
@@ -4393,22 +4598,45 @@
                                     "docs": {},
                                     "df": 0,
                                     "e": {
                                         "docs": {
                                             "parsetypes.TypeParser.infer_table": {
                                                 "tf": 2
                                             },
+                                            "parsetypes.TypeParser.convert": {
+                                                "tf": 1.4142135623730951
+                                            },
                                             "parsetypes.TypeParser.parse_table": {
                                                 "tf": 3.4641016151377544
                                             },
                                             "parsetypes.TypeParser.iterate_table": {
                                                 "tf": 3.4641016151377544
                                             }
                                         },
-                                        "df": 3
+                                        "df": 4
+                                    }
+                                }
+                            },
+                            "r": {
+                                "docs": {},
+                                "df": 0,
+                                "g": {
+                                    "docs": {},
+                                    "df": 0,
+                                    "e": {
+                                        "docs": {},
+                                        "df": 0,
+                                        "t": {
+                                            "docs": {
+                                                "parsetypes.TypeParser.convert": {
+                                                    "tf": 2.23606797749979
+                                                }
+                                            },
+                                            "df": 1
+                                        }
                                     }
                                 }
                             },
                             "k": {
                                 "docs": {},
                                 "df": 0,
                                 "e": {
@@ -4528,28 +4756,31 @@
                                             },
                                             "parsetypes.TypeParser.parse_float": {
                                                 "tf": 2.449489742783178
                                             },
                                             "parsetypes.TypeParser.parse_decimal": {
                                                 "tf": 2.449489742783178
                                             },
+                                            "parsetypes.TypeParser.convert": {
+                                                "tf": 1.7320508075688772
+                                            },
                                             "parsetypes.TypeParser.parse": {
                                                 "tf": 2
                                             },
                                             "parsetypes.TypeParser.parse_series": {
                                                 "tf": 2.23606797749979
                                             },
                                             "parsetypes.TypeParser.parse_table": {
                                                 "tf": 1.4142135623730951
                                             },
                                             "parsetypes.TypeParser.iterate_table": {
                                                 "tf": 1.4142135623730951
                                             }
                                         },
-                                        "df": 11,
+                                        "df": 12,
                                         "r": {
                                             "docs": {
                                                 "parsetypes.TypeParser": {
                                                     "tf": 1.4142135623730951
                                                 },
                                                 "parsetypes.TypeParser.__init__": {
                                                     "tf": 1.4142135623730951
@@ -4586,28 +4817,31 @@
                                                 },
                                                 "parsetypes.TypeParser.infer_series": {
                                                     "tf": 2
                                                 },
                                                 "parsetypes.TypeParser.infer_table": {
                                                     "tf": 1.4142135623730951
                                                 },
+                                                "parsetypes.TypeParser.convert": {
+                                                    "tf": 2
+                                                },
                                                 "parsetypes.TypeParser.parse": {
                                                     "tf": 2
                                                 },
                                                 "parsetypes.TypeParser.parse_series": {
                                                     "tf": 2.23606797749979
                                                 },
                                                 "parsetypes.TypeParser.parse_table": {
                                                     "tf": 1.4142135623730951
                                                 },
                                                 "parsetypes.TypeParser.iterate_table": {
                                                     "tf": 1.4142135623730951
                                                 }
                                             },
-                                            "df": 18
+                                            "df": 19
                                         },
                                         "d": {
                                             "docs": {
                                                 "parsetypes.TypeParser.parse_none": {
                                                     "tf": 1.7320508075688772
                                                 },
                                                 "parsetypes.TypeParser.parse_bool": {
@@ -4730,14 +4964,17 @@
                                                                 },
                                                                 "parsetypes.TypeParser.infer_series": {
                                                                     "tf": 1
                                                                 },
                                                                 "parsetypes.TypeParser.infer_table": {
                                                                     "tf": 1
                                                                 },
+                                                                "parsetypes.TypeParser.convert": {
+                                                                    "tf": 1
+                                                                },
                                                                 "parsetypes.TypeParser.parse": {
                                                                     "tf": 1
                                                                 },
                                                                 "parsetypes.TypeParser.parse_series": {
                                                                     "tf": 1
                                                                 },
                                                                 "parsetypes.TypeParser.parse_table": {
@@ -4746,15 +4983,15 @@
                                                                 "parsetypes.TypeParser.iterate_table": {
                                                                     "tf": 1
                                                                 },
                                                                 "parsetypes.reduce_types": {
                                                                     "tf": 1
                                                                 }
                                                             },
-                                                            "df": 18
+                                                            "df": 19
                                                         }
                                                     }
                                                 }
                                             }
                                         }
                                     }
                                 }
@@ -4900,28 +5137,31 @@
                                                         },
                                                         "parsetypes.TypeParser.infer_series": {
                                                             "tf": 1
                                                         },
                                                         "parsetypes.TypeParser.infer_table": {
                                                             "tf": 1
                                                         },
+                                                        "parsetypes.TypeParser.convert": {
+                                                            "tf": 1
+                                                        },
                                                         "parsetypes.TypeParser.parse_series": {
                                                             "tf": 1
                                                         },
                                                         "parsetypes.TypeParser.parse_table": {
                                                             "tf": 1
                                                         },
                                                         "parsetypes.TypeParser.iterate_table": {
                                                             "tf": 1
                                                         },
                                                         "parsetypes.reduce_types": {
                                                             "tf": 1
                                                         }
                                                     },
-                                                    "df": 11
+                                                    "df": 12
                                                 }
                                             }
                                         }
                                     }
                                 }
                             }
                         }
@@ -4957,25 +5197,28 @@
                                     },
                                     "parsetypes.TypeParser.infer_series": {
                                         "tf": 1.4142135623730951
                                     },
                                     "parsetypes.TypeParser.infer_table": {
                                         "tf": 2
                                     },
+                                    "parsetypes.TypeParser.convert": {
+                                        "tf": 1
+                                    },
                                     "parsetypes.TypeParser.parse_series": {
                                         "tf": 1
                                     },
                                     "parsetypes.TypeParser.parse_table": {
                                         "tf": 1.4142135623730951
                                     },
                                     "parsetypes.TypeParser.iterate_table": {
                                         "tf": 1.7320508075688772
                                     }
                                 },
-                                "df": 12,
+                                "df": 13,
                                 "m": {
                                     "docs": {
                                         "parsetypes.TypeParser.is_int": {
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser.is_float": {
                                             "tf": 1
@@ -5028,19 +5271,22 @@
                                             },
                                             "parsetypes.TypeParser.infer_series": {
                                                 "tf": 1
                                             },
                                             "parsetypes.TypeParser.infer_table": {
                                                 "tf": 1
                                             },
+                                            "parsetypes.TypeParser.convert": {
+                                                "tf": 1
+                                            },
                                             "parsetypes.reduce_types": {
                                                 "tf": 1.7320508075688772
                                             }
                                         },
-                                        "df": 10,
+                                        "df": 11,
                                         "s": {
                                             "docs": {
                                                 "parsetypes": {
                                                     "tf": 1
                                                 },
                                                 "parsetypes.reduce_types": {
                                                     "tf": 1
@@ -5058,17 +5304,20 @@
                             "o": {
                                 "docs": {},
                                 "df": 0,
                                 "m": {
                                     "docs": {
                                         "parsetypes.TypeParser.__init__": {
                                             "tf": 1
+                                        },
+                                        "parsetypes.TypeParser.convert": {
+                                            "tf": 1
                                         }
                                     },
-                                    "df": 1
+                                    "df": 2
                                 }
                             }
                         },
                         "a": {
                             "docs": {},
                             "df": 0,
                             "l": {
@@ -5246,19 +5495,22 @@
                                         "docs": {},
                                         "df": 0,
                                         "s": {
                                             "docs": {
                                                 "parsetypes.TypeParser.infer_series": {
                                                     "tf": 2.6457513110645907
                                                 },
+                                                "parsetypes.TypeParser.convert": {
+                                                    "tf": 1.4142135623730951
+                                                },
                                                 "parsetypes.TypeParser.parse_series": {
                                                     "tf": 2.8284271247461903
                                                 }
                                             },
-                                            "df": 2
+                                            "df": 3
                                         }
                                     }
                                 }
                             },
                             "t": {
                                 "docs": {
                                     "parsetypes.TypeParser.__init__": {
@@ -5559,19 +5811,22 @@
                                                 },
                                                 "parsetypes.TypeParser.parse_decimal": {
                                                     "tf": 2
                                                 },
                                                 "parsetypes.TypeParser.infer": {
                                                     "tf": 1.4142135623730951
                                                 },
+                                                "parsetypes.TypeParser.convert": {
+                                                    "tf": 1.7320508075688772
+                                                },
                                                 "parsetypes.TypeParser.parse": {
                                                     "tf": 1.4142135623730951
                                                 }
                                             },
-                                            "df": 12,
+                                            "df": 13,
                                             "s": {
                                                 "docs": {
                                                     "parsetypes.TypeParser": {
                                                         "tf": 1
                                                     },
                                                     "parsetypes.TypeParser.__init__": {
                                                         "tf": 2.6457513110645907
@@ -5684,22 +5939,25 @@
                                                 },
                                                 "parsetypes.TypeParser.infer_series": {
                                                     "tf": 1
                                                 },
                                                 "parsetypes.TypeParser.infer_table": {
                                                     "tf": 1
                                                 },
+                                                "parsetypes.TypeParser.convert": {
+                                                    "tf": 1
+                                                },
                                                 "parsetypes.TypeParser.parse_table": {
                                                     "tf": 1.4142135623730951
                                                 },
                                                 "parsetypes.reduce_types": {
                                                     "tf": 1
                                                 }
                                             },
-                                            "df": 6
+                                            "df": 7
                                         }
                                     }
                                 }
                             }
                         },
                         "p": {
                             "docs": {},
@@ -5722,17 +5980,20 @@
                                                 "e": {
                                                     "docs": {},
                                                     "df": 0,
                                                     "d": {
                                                         "docs": {
                                                             "parsetypes.TypeParser.__init__": {
                                                                 "tf": 1
+                                                            },
+                                                            "parsetypes.TypeParser.convert": {
+                                                                "tf": 1
                                                             }
                                                         },
-                                                        "df": 1
+                                                        "df": 2
                                                     }
                                                 }
                                             }
                                         }
                                     }
                                 }
                             }
@@ -6451,17 +6712,20 @@
                                                     "tf": 1
                                                 },
                                                 "parsetypes.TypeParser.parse_float": {
                                                     "tf": 1
                                                 },
                                                 "parsetypes.TypeParser.parse_decimal": {
                                                     "tf": 1
+                                                },
+                                                "parsetypes.TypeParser.convert": {
+                                                    "tf": 1
                                                 }
                                             },
-                                            "df": 6,
+                                            "df": 7,
                                             "s": {
                                                 "docs": {
                                                     "parsetypes.TypeParser.is_none": {
                                                         "tf": 1
                                                     },
                                                     "parsetypes.TypeParser.is_bool": {
                                                         "tf": 1
@@ -6492,14 +6756,17 @@
                                                     },
                                                     "parsetypes.TypeParser.infer_series": {
                                                         "tf": 1
                                                     },
                                                     "parsetypes.TypeParser.infer_table": {
                                                         "tf": 1
                                                     },
+                                                    "parsetypes.TypeParser.convert": {
+                                                        "tf": 1
+                                                    },
                                                     "parsetypes.TypeParser.parse": {
                                                         "tf": 1
                                                     },
                                                     "parsetypes.TypeParser.parse_series": {
                                                         "tf": 1
                                                     },
                                                     "parsetypes.TypeParser.parse_table": {
@@ -6508,15 +6775,15 @@
                                                     "parsetypes.TypeParser.iterate_table": {
                                                         "tf": 1
                                                     },
                                                     "parsetypes.reduce_types": {
                                                         "tf": 1
                                                     }
                                                 },
-                                                "df": 17
+                                                "df": 18
                                             },
                                             "e": {
                                                 "docs": {},
                                                 "df": 0,
                                                 "d": {
                                                     "docs": {
                                                         "parsetypes.TypeParser.parse_table": {
@@ -6710,17 +6977,20 @@
                                                     "tf": 1
                                                 },
                                                 "parsetypes.TypeParser.parse_float": {
                                                     "tf": 1
                                                 },
                                                 "parsetypes.TypeParser.parse_decimal": {
                                                     "tf": 1
+                                                },
+                                                "parsetypes.TypeParser.convert": {
+                                                    "tf": 1
                                                 }
                                             },
-                                            "df": 6
+                                            "df": 7
                                         }
                                     }
                                 }
                             }
                         },
                         "o": {
                             "docs": {},
@@ -6771,19 +7041,22 @@
                                 },
                                 "parsetypes.TypeParser.parse_float": {
                                     "tf": 1
                                 },
                                 "parsetypes.TypeParser.parse_decimal": {
                                     "tf": 1
                                 },
+                                "parsetypes.TypeParser.convert": {
+                                    "tf": 1
+                                },
                                 "parsetypes.reduce_types": {
                                     "tf": 1.4142135623730951
                                 }
                             },
-                            "df": 6,
+                            "df": 7,
                             "i": {
                                 "docs": {},
                                 "df": 0,
                                 "g": {
                                     "docs": {},
                                     "df": 0,
                                     "i": {
@@ -7126,17 +7399,20 @@
                         "s": {
                             "docs": {},
                             "df": 0,
                             "e": {
                                 "docs": {
                                     "parsetypes.TypeParser.__init__": {
                                         "tf": 1
+                                    },
+                                    "parsetypes.TypeParser.convert": {
+                                        "tf": 1
                                     }
                                 },
-                                "df": 1,
+                                "df": 2,
                                 "d": {
                                     "docs": {
                                         "parsetypes.TypeParser": {
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser.__init__": {
                                             "tf": 1
@@ -7281,56 +7557,62 @@
                                             "docs": {},
                                             "df": 0,
                                             "t": {
                                                 "docs": {
                                                     "parsetypes.TypeParser": {
                                                         "tf": 1
                                                     },
+                                                    "parsetypes.TypeParser.convert": {
+                                                        "tf": 2.23606797749979
+                                                    },
                                                     "parsetypes.TypeParser.parse": {
                                                         "tf": 1
                                                     },
                                                     "parsetypes.TypeParser.parse_series": {
                                                         "tf": 1
                                                     },
                                                     "parsetypes.TypeParser.parse_table": {
                                                         "tf": 1
                                                     },
                                                     "parsetypes.TypeParser.iterate_table": {
                                                         "tf": 1
                                                     }
                                                 },
-                                                "df": 5,
+                                                "df": 6,
                                                 "e": {
                                                     "docs": {},
                                                     "df": 0,
                                                     "d": {
                                                         "docs": {
                                                             "parsetypes.TypeParser.parse_int": {
                                                                 "tf": 1
                                                             },
                                                             "parsetypes.TypeParser.parse_float": {
                                                                 "tf": 1.4142135623730951
                                                             },
                                                             "parsetypes.TypeParser.parse_decimal": {
                                                                 "tf": 1.4142135623730951
                                                             },
+                                                            "parsetypes.TypeParser.convert": {
+                                                                "tf": 2
+                                                            },
                                                             "parsetypes.TypeParser.parse": {
                                                                 "tf": 1
                                                             },
                                                             "parsetypes.TypeParser.parse_series": {
                                                                 "tf": 1
                                                             },
                                                             "parsetypes.TypeParser.parse_table": {
                                                                 "tf": 1.4142135623730951
                                                             },
                                                             "parsetypes.TypeParser.iterate_table": {
                                                                 "tf": 1.4142135623730951
                                                             }
                                                         },
-                                                        "df": 7
+                                                        "df": 8
                                                     }
                                                 }
                                             }
                                         }
                                     }
                                 },
                                 "s": {
@@ -7557,17 +7839,20 @@
                                                     "tf": 1
                                                 },
                                                 "parsetypes.TypeParser.parse_float": {
                                                     "tf": 1
                                                 },
                                                 "parsetypes.TypeParser.parse_decimal": {
                                                     "tf": 1
+                                                },
+                                                "parsetypes.TypeParser.convert": {
+                                                    "tf": 1
                                                 }
                                             },
-                                            "df": 5
+                                            "df": 6
                                         }
                                     }
                                 }
                             },
                             "u": {
                                 "docs": {},
                                 "df": 0,
@@ -7807,22 +8092,25 @@
                                             },
                                             "parsetypes.TypeParser.infer_series": {
                                                 "tf": 2
                                             },
                                             "parsetypes.TypeParser.infer_table": {
                                                 "tf": 1.4142135623730951
                                             },
+                                            "parsetypes.TypeParser.convert": {
+                                                "tf": 2
+                                            },
                                             "parsetypes.TypeParser.parse_table": {
                                                 "tf": 1
                                             },
                                             "parsetypes.TypeParser.iterate_table": {
                                                 "tf": 1
                                             }
                                         },
-                                        "df": 7,
+                                        "df": 8,
                                         "e": {
                                             "docs": {},
                                             "df": 0,
                                             "n": {
                                                 "docs": {},
                                                 "df": 0,
                                                 "c": {
@@ -8046,17 +8334,20 @@
                                                         "tf": 1.4142135623730951
                                                     },
                                                     "parsetypes.TypeParser.parse_float": {
                                                         "tf": 1
                                                     },
                                                     "parsetypes.TypeParser.parse_decimal": {
                                                         "tf": 1
+                                                    },
+                                                    "parsetypes.TypeParser.convert": {
+                                                        "tf": 1
                                                     }
                                                 },
-                                                "df": 4
+                                                "df": 5
                                             }
                                         }
                                     },
                                     "a": {
                                         "docs": {},
                                         "df": 0,
                                         "n": {
@@ -8127,19 +8418,22 @@
                                     },
                                     "parsetypes.TypeParser.infer_series": {
                                         "tf": 1
                                     },
                                     "parsetypes.TypeParser.infer_table": {
                                         "tf": 1
                                     },
+                                    "parsetypes.TypeParser.convert": {
+                                        "tf": 1
+                                    },
                                     "parsetypes.reduce_types": {
                                         "tf": 2
                                     }
                                 },
-                                "df": 9,
+                                "df": 10,
                                 "o": {
                                     "docs": {
                                         "parsetypes.TypeParser": {
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser.infer_table": {
                                             "tf": 1
@@ -8329,14 +8623,38 @@
                                                     }
                                                 }
                                             }
                                         }
                                     }
                                 }
                             },
+                            "c": {
+                                "docs": {},
+                                "df": 0,
+                                "l": {
+                                    "docs": {},
+                                    "df": 0,
+                                    "u": {
+                                        "docs": {},
+                                        "df": 0,
+                                        "d": {
+                                            "docs": {},
+                                            "df": 0,
+                                            "e": {
+                                                "docs": {
+                                                    "parsetypes.TypeParser.convert": {
+                                                        "tf": 1
+                                                    }
+                                                },
+                                                "df": 1
+                                            }
+                                        }
+                                    }
+                                }
+                            },
                             "p": {
                                 "docs": {},
                                 "df": 0,
                                 "u": {
                                     "docs": {},
                                     "df": 0,
                                     "t": {
@@ -8384,28 +8702,31 @@
                                 },
                                 "parsetypes.TypeParser.parse_decimal": {
                                     "tf": 2
                                 },
                                 "parsetypes.TypeParser.infer": {
                                     "tf": 1
                                 },
+                                "parsetypes.TypeParser.convert": {
+                                    "tf": 1
+                                },
                                 "parsetypes.TypeParser.parse_series": {
                                     "tf": 1
                                 },
                                 "parsetypes.TypeParser.parse_table": {
                                     "tf": 2.23606797749979
                                 },
                                 "parsetypes.TypeParser.iterate_table": {
                                     "tf": 2
                                 },
                                 "parsetypes.reduce_types": {
                                     "tf": 1
                                 }
                             },
-                            "df": 16
+                            "df": 17
                         },
                         "d": {
                             "docs": {},
                             "df": 0,
                             "e": {
                                 "docs": {},
                                 "df": 0,
@@ -8588,28 +8909,31 @@
                                 },
                                 "parsetypes.TypeParser.infer_series": {
                                     "tf": 1
                                 },
                                 "parsetypes.TypeParser.infer_table": {
                                     "tf": 1
                                 },
+                                "parsetypes.TypeParser.convert": {
+                                    "tf": 1.7320508075688772
+                                },
                                 "parsetypes.TypeParser.parse_series": {
                                     "tf": 1
                                 },
                                 "parsetypes.TypeParser.parse_table": {
                                     "tf": 1.7320508075688772
                                 },
                                 "parsetypes.TypeParser.iterate_table": {
                                     "tf": 1
                                 },
                                 "parsetypes.reduce_types": {
                                     "tf": 1
                                 }
                             },
-                            "df": 17
+                            "df": 18
                         },
                         "g": {
                             "docs": {},
                             "df": 0,
                             "n": {
                                 "docs": {},
                                 "df": 0,
@@ -8711,14 +9035,17 @@
                             },
                             "parsetypes.TypeParser.infer_series": {
                                 "tf": 1
                             },
                             "parsetypes.TypeParser.infer_table": {
                                 "tf": 1
                             },
+                            "parsetypes.TypeParser.convert": {
+                                "tf": 1.4142135623730951
+                            },
                             "parsetypes.TypeParser.parse": {
                                 "tf": 1
                             },
                             "parsetypes.TypeParser.parse_series": {
                                 "tf": 1
                             },
                             "parsetypes.TypeParser.parse_table": {
@@ -8727,15 +9054,15 @@
                             "parsetypes.TypeParser.iterate_table": {
                                 "tf": 2.23606797749979
                             },
                             "parsetypes.reduce_types": {
                                 "tf": 2
                             }
                         },
-                        "df": 20,
+                        "df": 21,
                         "n": {
                             "docs": {
                                 "parsetypes.TypeParser.is_none": {
                                     "tf": 1
                                 },
                                 "parsetypes.TypeParser.is_int": {
                                     "tf": 2
@@ -8791,36 +9118,42 @@
                                     },
                                     "parsetypes.TypeParser.parse_float": {
                                         "tf": 2
                                     },
                                     "parsetypes.TypeParser.parse_decimal": {
                                         "tf": 2
                                     },
+                                    "parsetypes.TypeParser.convert": {
+                                        "tf": 1.4142135623730951
+                                    },
                                     "parsetypes.TypeParser.parse": {
                                         "tf": 1
                                     },
                                     "parsetypes.TypeParser.parse_series": {
                                         "tf": 1
                                     },
                                     "parsetypes.TypeParser.parse_table": {
                                         "tf": 2.6457513110645907
                                     },
                                     "parsetypes.TypeParser.iterate_table": {
                                         "tf": 2
                                     }
                                 },
-                                "df": 15
+                                "df": 16
                             },
                             "y": {
                                 "docs": {
                                     "parsetypes.TypeParser.__init__": {
                                         "tf": 1.4142135623730951
+                                    },
+                                    "parsetypes.TypeParser.convert": {
+                                        "tf": 1
                                     }
                                 },
-                                "df": 1
+                                "df": 2
                             },
                             "a": {
                                 "docs": {},
                                 "df": 0,
                                 "l": {
                                     "docs": {},
                                     "df": 0,
@@ -9488,14 +9821,66 @@
                                                     "df": 4
                                                 }
                                             }
                                         }
                                     }
                                 }
                             }
+                        },
+                        "u": {
+                            "docs": {},
+                            "df": 0,
+                            "t": {
+                                "docs": {},
+                                "df": 0,
+                                "o": {
+                                    "docs": {},
+                                    "df": 0,
+                                    "m": {
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
+                                                    "c": {
+                                                        "docs": {},
+                                                        "df": 0,
+                                                        "a": {
+                                                            "docs": {},
+                                                            "df": 0,
+                                                            "l": {
+                                                                "docs": {},
+                                                                "df": 0,
+                                                                "l": {
+                                                                    "docs": {},
+                                                                    "df": 0,
+                                                                    "y": {
+                                                                        "docs": {
+                                                                            "parsetypes.TypeParser.convert": {
+                                                                                "tf": 1
+                                                                            }
+                                                                        },
+                                                                        "df": 1
+                                                                    }
+                                                                }
+                                                            }
+                                                        }
+                                                    }
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
                         "e": {
                             "docs": {
@@ -9540,14 +9925,17 @@
                                 },
                                 "parsetypes.TypeParser.infer_series": {
                                     "tf": 1.4142135623730951
                                 },
                                 "parsetypes.TypeParser.infer_table": {
                                     "tf": 1.7320508075688772
                                 },
+                                "parsetypes.TypeParser.convert": {
+                                    "tf": 1.7320508075688772
+                                },
                                 "parsetypes.TypeParser.parse": {
                                     "tf": 1
                                 },
                                 "parsetypes.TypeParser.parse_series": {
                                     "tf": 1
                                 },
                                 "parsetypes.TypeParser.parse_table": {
@@ -9556,15 +9944,15 @@
                                 "parsetypes.TypeParser.iterate_table": {
                                     "tf": 1.7320508075688772
                                 },
                                 "parsetypes.reduce_types": {
                                     "tf": 1.7320508075688772
                                 }
                             },
-                            "df": 20,
+                            "df": 21,
                             "h": {
                                 "docs": {},
                                 "df": 0,
                                 "a": {
                                     "docs": {},
                                     "df": 0,
                                     "v": {
@@ -9626,19 +10014,22 @@
                                         },
                                         "parsetypes.TypeParser.parse_decimal": {
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser.infer": {
                                             "tf": 1
                                         },
+                                        "parsetypes.TypeParser.convert": {
+                                            "tf": 1
+                                        },
                                         "parsetypes.reduce_types": {
                                             "tf": 1
                                         }
                                     },
-                                    "df": 10,
+                                    "df": 11,
                                     "e": {
                                         "docs": {},
                                         "df": 0,
                                         "a": {
                                             "docs": {},
                                             "df": 0,
                                             "n": {
@@ -9961,22 +10352,25 @@
                                             },
                                             "parsetypes.TypeParser.infer_series": {
                                                 "tf": 1
                                             },
                                             "parsetypes.TypeParser.infer_table": {
                                                 "tf": 1
                                             },
+                                            "parsetypes.TypeParser.convert": {
+                                                "tf": 1
+                                            },
                                             "parsetypes.TypeParser.parse_table": {
                                                 "tf": 1.4142135623730951
                                             },
                                             "parsetypes.TypeParser.iterate_table": {
                                                 "tf": 1
                                             }
                                         },
-                                        "df": 13
+                                        "df": 14
                                     }
                                 }
                             }
                         },
                         "e": {
                             "docs": {},
                             "df": 0,
@@ -10098,14 +10492,17 @@
                                                         },
                                                         "parsetypes.TypeParser.infer_series": {
                                                             "tf": 1
                                                         },
                                                         "parsetypes.TypeParser.infer_table": {
                                                             "tf": 1
                                                         },
+                                                        "parsetypes.TypeParser.convert": {
+                                                            "tf": 1
+                                                        },
                                                         "parsetypes.TypeParser.parse": {
                                                             "tf": 1
                                                         },
                                                         "parsetypes.TypeParser.parse_series": {
                                                             "tf": 1
                                                         },
                                                         "parsetypes.TypeParser.parse_table": {
@@ -10114,15 +10511,15 @@
                                                         "parsetypes.TypeParser.iterate_table": {
                                                             "tf": 1
                                                         },
                                                         "parsetypes.reduce_types": {
                                                             "tf": 1
                                                         }
                                                     },
-                                                    "df": 17
+                                                    "df": 18
                                                 }
                                             }
                                         }
                                     }
                                 },
                                 "c": {
                                     "docs": {},
@@ -10665,28 +11062,31 @@
                                     },
                                     "parsetypes.TypeParser.infer_series": {
                                         "tf": 1
                                     },
                                     "parsetypes.TypeParser.infer_table": {
                                         "tf": 1
                                     },
+                                    "parsetypes.TypeParser.convert": {
+                                        "tf": 1
+                                    },
                                     "parsetypes.TypeParser.parse_series": {
                                         "tf": 1
                                     },
                                     "parsetypes.TypeParser.parse_table": {
                                         "tf": 1
                                     },
                                     "parsetypes.TypeParser.iterate_table": {
                                         "tf": 1
                                     },
                                     "parsetypes.reduce_types": {
                                         "tf": 1
                                     }
                                 },
-                                "df": 11,
+                                "df": 12,
                                 "e": {
                                     "docs": {
                                         "parsetypes.TypeParser.__init__": {
                                             "tf": 1
                                         },
                                         "parsetypes.TypeParser.is_int": {
                                             "tf": 1
@@ -11058,25 +11458,28 @@
                                             },
                                             "parsetypes.TypeParser.infer": {
                                                 "tf": 1
                                             },
                                             "parsetypes.TypeParser.infer_table": {
                                                 "tf": 1
                                             },
+                                            "parsetypes.TypeParser.convert": {
+                                                "tf": 2.23606797749979
+                                            },
                                             "parsetypes.TypeParser.parse": {
                                                 "tf": 1.4142135623730951
                                             },
                                             "parsetypes.TypeParser.parse_table": {
                                                 "tf": 1.4142135623730951
                                             },
                                             "parsetypes.TypeParser.iterate_table": {
                                                 "tf": 1.4142135623730951
                                             }
                                         },
-                                        "df": 15,
+                                        "df": 16,
                                         "s": {
                                             "docs": {
                                                 "parsetypes": {
                                                     "tf": 1
                                                 },
                                                 "parsetypes.TypeParser.__init__": {
                                                     "tf": 3.872983346207417
@@ -11107,28 +11510,31 @@
                                                 },
                                                 "parsetypes.TypeParser.infer_series": {
                                                     "tf": 1.7320508075688772
                                                 },
                                                 "parsetypes.TypeParser.infer_table": {
                                                     "tf": 1.4142135623730951
                                                 },
+                                                "parsetypes.TypeParser.convert": {
+                                                    "tf": 1
+                                                },
                                                 "parsetypes.TypeParser.parse_series": {
                                                     "tf": 2
                                                 },
                                                 "parsetypes.TypeParser.parse_table": {
                                                     "tf": 2.23606797749979
                                                 },
                                                 "parsetypes.TypeParser.iterate_table": {
                                                     "tf": 1.7320508075688772
                                                 },
                                                 "parsetypes.reduce_types": {
                                                     "tf": 1
                                                 }
                                             },
-                                            "df": 16
+                                            "df": 17
                                         },
                                         "e": {
                                             "docs": {},
                                             "df": 0,
                                             "r": {
                                                 "docs": {},
                                                 "df": 0,
@@ -11153,23 +11559,38 @@
                                                                     "tf": 1
                                                                 },
                                                                 "parsetypes.TypeParser.parse_float": {
                                                                     "tf": 1
                                                                 },
                                                                 "parsetypes.TypeParser.parse_decimal": {
                                                                     "tf": 1
+                                                                },
+                                                                "parsetypes.TypeParser.convert": {
+                                                                    "tf": 1
                                                                 }
                                                             },
-                                                            "df": 6
+                                                            "df": 7
                                                         }
                                                     }
                                                 }
                                             }
                                         }
                                     }
+                                },
+                                "i": {
+                                    "docs": {},
+                                    "df": 0,
+                                    "d": {
+                                        "docs": {
+                                            "parsetypes.TypeParser.convert": {
+                                                "tf": 1.4142135623730951
+                                            }
+                                        },
+                                        "df": 1
+                                    }
                                 }
                             },
                             "r": {
                                 "docs": {},
                                 "df": 0,
                                 "i": {
                                     "docs": {},
@@ -11780,28 +12201,31 @@
                                         },
                                         "parsetypes.TypeParser.infer_series": {
                                             "tf": 4.242640687119285
                                         },
                                         "parsetypes.TypeParser.infer_table": {
                                             "tf": 4.242640687119285
                                         },
+                                        "parsetypes.TypeParser.convert": {
+                                            "tf": 2.449489742783178
+                                        },
                                         "parsetypes.TypeParser.parse": {
                                             "tf": 2.8284271247461903
                                         },
                                         "parsetypes.TypeParser.parse_series": {
                                             "tf": 5.477225575051661
                                         },
                                         "parsetypes.TypeParser.parse_table": {
                                             "tf": 5.477225575051661
                                         },
                                         "parsetypes.TypeParser.iterate_table": {
                                             "tf": 4.898979485566356
                                         }
                                     },
-                                    "df": 16
+                                    "df": 17
                                 }
                             }
                         }
                     },
                     "x": {
                         "docs": {
                             "parsetypes.TypeParser.is_int": {
```

### Comparing `parsetypes-0.2.3/pyproject.toml` & `parsetypes-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `parsetypes-0.2.3/src/parsetypes/__init__.py` & `parsetypes-0.2.4/src/parsetypes/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 	The `TypeParser` class provides configurable type inference and parsing. This can be initialised with different settings to, for example:
 	- treat `inf` as either a float or a normal string
 	- give exact Decimal values instead of floats
 	- detect inline lists
 """
 
 
-__version__ = "0.2.3"
+__version__ = "0.2.4"
 
 from ._common import AnyScalar, AnyScalarType, AnyValue, AnyValueType, GenericValue, Nullable
 from ._parser import TypeParser
 from ._reduce_types import reduce_types
 
 __all__ = ('TypeParser', 'reduce_types')
```

### Comparing `parsetypes-0.2.3/src/parsetypes/_common.py` & `parsetypes-0.2.4/src/parsetypes/_common.py`

 * *Files identical despite different names*

### Comparing `parsetypes-0.2.3/src/parsetypes/_parser.py` & `parsetypes-0.2.4/src/parsetypes/_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -824,18 +824,52 @@
 		table = _TypeTable([[self.infer(value)] for value in first_row])
 		for row in rows_iter:
 			table.add_row([self.infer(value) for value in row])
 
 		return [reduce_types(col) for col in table.cols]
 
 
-	def _convert(self, value: str, t: AnyValueType) -> AnyValue:
-		base, type_args = _decompose_type(t)
+	def convert(self, value: str, target_type: AnyValueType) -> AnyValue:
+		"""
+			Convert a string to the specified target type if possible
+
+			Valid values for `target_type` include any return value from `infer()`, `infer_series()` and `infer_table()`. To infer and convert the string automatically, use `parse()`, `parse_series()` or `parse_table()` instead.
+
+			Parameters
+			----------
+			`value`
+			: the string to be converted
+
+			`target_type`
+			: type to which the value should be converted
+
+			Returns
+			-------
+			converted value
+
+			Raises
+			-------
+			`ValueError`
+			: if `value` cannot be converted to `target_type`
+
+			`TypeError`
+			: if `target_type` is not a valid type
+
+			Examples
+			--------
+			```python
+			parser = TypeParser()
+			parser.convert("true", bool)  # True
+			parser.convert("2", int)      # 2
+			parser.convert("2", float)    # 2.
+			```
+		"""
+		base, type_args = _decompose_type(target_type)
 		if base == NoneType:
-			return None
+			return self.parse_none(value)
 		elif base == bool:
 			return self.parse_bool(value)
 		elif base == int:
 			return self.parse_int(value)
 		elif base == Decimal:
 			return self.parse_decimal(value)
 		elif base == float:
@@ -844,28 +878,28 @@
 			return value
 		elif base == Nullable:
 			if self.is_none(value):
 				return None
 			else:
 				if type_args is not  None and len(type_args) == 1 and type_args[0] != str:
 					inner_type = type_args[0]
-					return self._convert(value, inner_type)
+					return self.convert(value, inner_type)
 				else:
 					return value
 		elif base == list:
 			subvalues = value.split(self.list_delimiter)
 			if self.trim:
 				subvalues = [subvalue.strip() for subvalue in subvalues]
 			if type_args is not None and len(type_args) == 1 and type_args[0] != str:
 				subtype = type_args[0]
-				return [self._convert(subvalue, subtype) for subvalue in subvalues]
+				return [self.convert(subvalue, subtype) for subvalue in subvalues]
 			else:
 				return subvalues
 		else:
-			return value
+			raise TypeError(f"cannot convert to type: {target_type}")
 
 
 	def parse(self, value: str) -> AnyValue:
 		"""
 			Parse a string and convert it to its underlying type
 
 			Parameters
@@ -882,15 +916,15 @@
 			```python
 			parser = TypeParser()
 			parser.parse("true")  # True
 			parser.parse("2.0")   # 2.
 			parser.parse("abc")   # "abc"
 			```
 		"""
-		return self._convert(value, self.infer(value))
+		return self.convert(value, self.infer(value))
 
 
 	def parse_series(self, values: Iterable[str]) -> list[AnyValue]:
 		"""
 			Parse a series of strings and convert them to their underlying common type
 
 			If the values in the series do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the series. See `parsetypes.reduce_types()` for more information.
@@ -911,15 +945,15 @@
 			parser.parse_series(["1", "2", "3"])        # [1, 2, 3]
 			parser.parse_series(["5", "6.7", "8."])     # [5., 6.7, 8.]
 			parser.parse_series(["true", "false", ""])  # [True, False, None]
 			parser.parse_series(["1", "2.3", "abc"])    # ["1", "2.3", "abc"]
 			```
 		"""
 		inferred = self.infer_series(values)
-		return [self._convert(value, inferred) for value in values]
+		return [self.convert(value, inferred) for value in values]
 
 
 	def parse_table(self, rows: Iterable[Sequence[str]]) -> list[list[AnyValue]]:
 		"""
 			Parse a table of strings and convert them to the underlying common type of each column
 
 			For each column, if the values do not have the same apparent type, the common type is taken as the narrowest possible type that will encompass all values in the column. See `parsetypes.reduce_types()` for more information.
@@ -989,8 +1023,8 @@
 			assert next(table) == [2.,  0, "2.3"]
 			assert next(table) == [3.4, 2, "abc"]
 			```
 		"""
 		inferred_types = self.infer_table(rows)
 
 		for row in rows:
-			yield [self._convert(value, inferred) for value, inferred in zip(row, inferred_types)]
+			yield [self.convert(value, inferred) for value, inferred in zip(row, inferred_types)]
```

### Comparing `parsetypes-0.2.3/src/parsetypes/_reduce_types.py` & `parsetypes-0.2.4/src/parsetypes/_reduce_types.py`

 * *Files identical despite different names*

### Comparing `parsetypes-0.2.3/src/parsetypes.egg-info/PKG-INFO` & `parsetypes-0.2.4/src/parsetypes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsetypes
-Version: 0.2.3
+Version: 0.2.4
 Summary: Parse serialised data to recover their original underlying types
 Author-email: Yu Shiyang <yu.shiyang@gnayihs.uy>
 License: MPL-2.0
 Project-URL: Homepage, https://github.com/yushiyangk/parsetypes
 Project-URL: Documentation, https://parsetypes.gnayihs.uy/
 Project-URL: Issues, https://github.com/yushiyangk/parsetypes/issues
 Keywords: python,str,string,types,conversion
@@ -42,15 +42,15 @@
 
 This Python package provides tools for parsing serialised data to recover their original underlying types.
 
 [![](https://img.shields.io/badge/PyPI--inactive?style=social&logo=pypi)](https://pypi.org/project/parsetypes/) [![](https://img.shields.io/badge/GitHub--inactive?style=social&logo=github)](https://github.com/yushiyangk/parsetypes) [![](https://img.shields.io/badge/Documentation--inactive?style=social&logo=readthedocs)](https://parsetypes.gnayihs.uy/)
 
 ## Overview
 
-The `TypeParser` class provides configurable type inference and parsing. This can be initialised with different settings to, for example:
+The `TypeParser` class provides configurable type inference and parsing. This can be [initialised with different settings](https://parsetypes.gnayihs.uy/parsetypes.html#TypeParser.__init__) to, for example:
 - treat `inf` as either a float or a normal string
 - give exact Decimal values instead of floats
 - detect inline lists
 
 ## Install
 
 ```
@@ -158,14 +158,18 @@
 
 ## Changelog
 
 This project follows [PEP 440](https://peps.python.org/pep-0440/) and [Semantic Versioning (SemVer)](https://semver.org/spec/v2.0.0.html). In addition to the guarantees specified by SemVer, for versions before 1.0, this project guarantees backwards compatibility of the API for patch version updates (0.<var>y</var>.<b><var>z</var></b>).
 
 The recommended version specifier is <code>parsetypes ~= <var>x</var>.<var>y</var></code> for version 1.0 and later, and <code>parsetypes ~= <var>0</var>.<var>y</var>.<var>z</var></code> for versions prior to 1.0.
 
+### 0.2.4
+
+- Added <code><var>parser</var>.convert()</code>
+
 ### 0.2.1, 0.2.2 and 0.2.3
 
 - Fixed documentation
 
 ### 0.2
 
 - Added support for Python version 3.9; previously only 3.10 and 3.11 were supported
```

### Comparing `parsetypes-0.2.3/src/parsetypes.egg-info/SOURCES.txt` & `parsetypes-0.2.4/src/parsetypes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `parsetypes-0.2.3/tests/test_parser.py` & `parsetypes-0.2.4/tests/test_parser.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from decimal import Decimal
 from unittest.mock import call, patch
 
 import pytest
 
 import parsetypes
 from parsetypes import AnyScalar, AnyScalarType, AnyValue, AnyValueType, Nullable, TypeParser
+from parsetypes._reduce_types import _decompose_type
 
 from parsetypes._compat import NoneType, Union
 
 
 @pytest.fixture
 def default_parser():
 	return TypeParser()
@@ -1261,14 +1262,264 @@
 					)
 			mocked_infer.assert_has_calls(expected_calls, any_order=True)
 
 			mocked_reduce_types.assert_has_calls([call(expected_call) for expected_call in type_rows])
 			assert result == expected
 
 
+class TestConvert():
+	@staticmethod
+	@pytest.mark.parametrize(
+		('value', 'target_type', 'expected'),
+		[
+			("true", bool, True),
+			("false", bool, False),
+			("TRUE", bool, True),
+			("FALSE", bool, False),
+			("true", int, 1),
+			("false", int, 0),
+			("TRUE", int, 1),
+			("FALSE", int, 0),
+			("true", Decimal, Decimal(1)),
+			("false", Decimal, Decimal(0)),
+			("TRUE", Decimal, Decimal(1)),
+			("FALSE", Decimal, Decimal(0)),
+			("true", float, 1.),
+			("false", float, 0.),
+			("TRUE", float, 1.),
+			("FALSE", float, 0.),
+
+			("0", int, 0),
+			("+0", int, 0),
+			("-0", int, 0),
+			("1", int, 1),
+			("+1", int, 1),
+			("-1", int, -1),
+			("20", int, 20),
+			("1e6", int, 1000000),
+			("0", Decimal, Decimal(0)),
+			("+0", Decimal, Decimal(0)),
+			("-0", Decimal, Decimal(0)),
+			("1", Decimal, Decimal(1)),
+			("+1", Decimal, Decimal(1)),
+			("-1", Decimal, Decimal(-1)),
+			("20", Decimal, Decimal(20)),
+			("1e6", Decimal, Decimal(1000000)),
+			("0", float, 0.),
+			("+0", float, 0.),
+			("-0", float, 0.),
+			("1", float, 1.),
+			("+1", float, 1.),
+			("-1", float, -1.),
+			("20", float, 20.),
+
+			("1e6", float, 1000000.),
+			("0.0", float, 0.),
+			("+0.0", float, 0.),
+			("-0.0", float, 0.),
+			("0.", float, 0.),
+			("+0.", float, 0.),
+			("-0.", float, 0.),
+			(".0", float, 0.),
+			("+.0", float, 0.),
+			("-.0", float, 0.),
+			("1.0", float, 1.),
+			("+1.0", float, 1.),
+			("-1.0", float, -1.),
+			("1.", float, 1.),
+			(".1", float, .1),
+			("1.1", float, 1.1),
+			("1.23e0", float, 1.23),
+			("1.23e-0", float, 1.23),
+			("1.23e+0", float, 1.23),
+			("1.23e1", float, 12.3),
+			("1.23e-1", float, 0.123),
+			("1.23e+1", float, 12.3),
+			("1.23e6", float, 1230000.),
+			("1e6", Decimal, Decimal(1000000.)),
+			("0.0", Decimal, Decimal(0.)),
+			("+0.0", Decimal, Decimal(0.)),
+			("-0.0", Decimal, Decimal(0.)),
+			("0.", Decimal, Decimal(0.)),
+			("+0.", Decimal, Decimal(0.)),
+			("-0.", Decimal, Decimal(0.)),
+			(".0", Decimal, Decimal(0.)),
+			("+.0", Decimal, Decimal(0.)),
+			("-.0", Decimal, Decimal(0.)),
+			("1.0", Decimal, Decimal(1.)),
+			("+1.0", Decimal, Decimal(1.)),
+			("-1.0", Decimal, Decimal(-1.)),
+			("1.", Decimal, Decimal(1.)),
+			(".1", Decimal, Decimal(1) / Decimal(10)),
+			("1.1", Decimal, Decimal(11) / Decimal(10)),
+			("1.23e0", Decimal, Decimal(123) / Decimal(100)),
+			("1.23e+0", Decimal, Decimal(123) / Decimal(100)),
+			("1.23e-0", Decimal, Decimal(123) / Decimal(100)),
+			("1.23e1", Decimal, Decimal(123) / Decimal(10)),
+			("1.23e-1", Decimal, Decimal(123) / Decimal(1000)),
+			("1.23e+1", Decimal, Decimal(123) / Decimal(10)),
+			("1.23e6", Decimal, Decimal(1230000)),
+
+			("a", str, "a"),
+			("a1", str, "a1"),
+			("1a", str, "1a"),
+			("1a1", str, "1a1"),
+			("a1a", str, "a1a"),
+			("1.0.0", str, "1.0.0"),
+			("0+1", str, "0+1"),
+			("1-1", str, "1-1"),
+			("1e2.", str, "1e2."),
+			("1e2e3", str, "1e2e3"),
+			("a,", str, "a,"),
+			("a,b,c", str, "a,b,c"),
+			("1,", str, "1,"),
+			("1,2,3", str, "1,2,3"),
+			("a\n", str, "a\n"),
+			("a\nb\nc\n", str, "a\nb\nc\n"),
+			("", NoneType, None),
+
+			("inf", str, "inf"),
+			("nan", str, "nan"),
+		]
+	)
+	def test_scalars_and_nullables(default_parser: TypeParser, value: str, target_type: AnyScalarType, expected: AnyScalar):
+		result = default_parser.convert(value, target_type)
+		assert type(result) == type(expected)
+		assert result == expected
+
+		result = default_parser.convert(value, Nullable[target_type])
+		assert type(result) == type(expected)
+		assert result == expected
+
+
+	@staticmethod
+	@pytest.mark.parametrize('target_type', [int, float, Decimal, bool, str, None])
+	def test_none_nullables(default_parser: TypeParser, target_type: AnyScalarType):
+		result = default_parser.convert("", Nullable[target_type])
+		assert type(result) == NoneType
+		assert result == None
+
+
+	@staticmethod
+	@pytest.mark.parametrize(
+		('value', 'list_parser', 'target_inner_type', 'expected'),
+		[
+			("a,a", ",", str, ["a", "a"]),
+			("a,b,c", ",", str, ["a", "b", "c"]),
+			("a", ",", str, ["a"]),
+
+			("true,false,true", ",", bool, [True, False, True]),
+			("true:false:true", ":", bool, [True, False, True]),
+			("truepfalseptrue", "p", bool, [True, False, True]),
+			("true", ",", bool, [True]),
+
+			("0,1,2", ",", int, [0, 1, 2]),
+			("0,01,-2,+3,4e5,-60,7_0", ",", int, [0, 1, -2, 3, 400000, -60, 70]),
+
+			("0.1,0.2,0.3", ",", float, [0.1, 0.2, 0.3]),
+			(
+				"0.,.0,0.0,01.00,-0.2,+3.0,4.e+5,6e-7,-80.08,9_0e1_0",
+				",",
+				float,
+				[0., 0., 0., 1., -0.2, 3., 400000., 0.0000006, -80.08, 9.e11],
+			),
+			("0.1", ",", float, [0.1]),
+
+			("false,1", ",", int, [0, 1]),
+			("false,1.", ",", float, [0., 1.]),
+			("1,2.", ",", float, [1., 2.]),
+			("1,2.,a", ",", str, ["1", "2.", "a"]),
+
+			(",,,", ",", NoneType, [None, None, None, None]),
+			("", ",", NoneType, [None]),
+		],
+		indirect=['list_parser']
+	)
+	def test_lists(
+		value: str,
+		list_parser: TypeParser,
+		target_inner_type: AnyValueType,
+		expected: AnyValue,
+	):
+		result = list_parser.convert(value, list[target_inner_type])
+		assert type(result) == list
+		for result_value in result:
+			assert type(result_value) == target_inner_type
+		assert result == expected
+
+
+	@staticmethod
+	@pytest.mark.parametrize(
+		('value', 'list_parser', 'target_inner_type', 'expected'),
+		[
+			(",,a", ",", str, [None, None, "a"]),
+			(",,true", ",", bool, [None, None, True]),
+			("true,false,true", "t", str, [None, "rue,false,", "rue"]),
+			(",,0.4", ",", float, [None, None, 0.4]),
+			("false,,1.", ",", float, [0., None, 1.]),
+			("1,2.,,a", ",", str, ["1", "2.", None, "a"]),
+		],
+		indirect=['list_parser']
+	)
+	def test_list_nullables(
+		value: str,
+		list_parser: TypeParser,
+		target_inner_type: AnyScalarType,
+		expected: AnyValue,
+	):
+		result = list_parser.convert(value, list[Nullable[target_inner_type]])
+		assert type(result) == list
+		for result_value in result:
+			assert (type(result_value) == target_inner_type) or (result_value == None)
+		assert result == expected
+
+
+	@staticmethod
+	@pytest.mark.parametrize('value', ["1", "true", "a"])
+	@pytest.mark.parametrize('target_type', [dict, set, tuple])
+	def test_invalid_types(default_parser: TypeParser, value: str, target_type: type):
+		with pytest.raises(TypeError):
+			default_parser.convert(value, target_type)
+
+
+	@staticmethod
+	@pytest.mark.parametrize(
+		('value', 'target_type'),
+		[
+			("0", bool),
+			("1", bool),
+			("2", bool),
+			("0.", bool),
+			("1.2", bool),
+			("inf", bool),
+			("a", bool),
+			("", bool),
+
+			("0.", int),
+			("1.2", int),
+			("a", int),
+			("", int),
+
+			("a", float),
+			("", float),
+			("a", Decimal),
+			("", Decimal),
+
+			("true", NoneType),
+			("0", NoneType),
+			("0.", NoneType),
+			("a", NoneType),
+		]
+	)
+	def test_invalid_values(default_parser: TypeParser, value: str, target_type: type):
+		with pytest.raises(ValueError):
+			default_parser.convert(value, target_type)
+
+
+
 class TestParse():
 	@staticmethod
 	@pytest.mark.parametrize(
 		('value', 'expected_type', 'expected'),
 		[
 			("true", bool, True),
 			("false", bool, False),
@@ -1323,22 +1574,25 @@
 			("", NoneType, None),
 
 			("inf", str, "inf"),
 			("nan", str, "nan"),
 		]
 	)
 	def test_scalars_and_nullables(default_parser: TypeParser, value: str, expected_type: AnyScalarType, expected: AnyScalar):
-		with patch.object(default_parser, 'infer', return_value=expected_type) as mocked_infer:
+		with patch.object(default_parser, 'infer', return_value=expected_type) as mocked_infer, patch.object(default_parser, 'convert', return_value=expected) as mocked_convert:
 			result = default_parser.parse(value)
 			mocked_infer.assert_called_once_with(value)
+			mocked_convert.assert_called_once_with(value, expected_type)
 			assert result == expected
 
-		with patch.object(default_parser, 'infer', return_value=Nullable[expected_type]) as mocked_infer:
+		# infer should not actually return Nullable in these cases, but we mock it to test the behaviour of parse anyway
+		with patch.object(default_parser, 'infer', return_value=Nullable[expected_type]) as mocked_infer, patch.object(default_parser, 'convert', return_value=expected) as mocked_convert:
 			result = default_parser.parse(value)
 			mocked_infer.assert_called_once_with(value)
+			mocked_convert.assert_called_once_with(value, Nullable[expected_type])
 			assert result == expected
 
 
 	@staticmethod
 	@pytest.mark.parametrize(
 		('value', 'list_parser', 'expected_type', 'expected'),
 		[
@@ -1377,17 +1631,18 @@
 	)
 	def test_lists(
 		value: str,
 		list_parser: TypeParser,
 		expected_type: AnyValueType,
 		expected: AnyValue,
 	):
-		with patch.object(list_parser, 'infer', return_value=expected_type) as mocked_infer:
+		with patch.object(list_parser, 'infer', return_value=expected_type) as mocked_infer, patch.object(list_parser, 'convert', return_value=expected) as mocked_convert:
 			result = list_parser.parse(value)
 			mocked_infer.assert_called_once_with(value)
+			mocked_convert.assert_called_once_with(value, expected_type)
 			assert result == expected
 
 
 class TestParseSeries:
 	@staticmethod
 	@pytest.mark.parametrize(
 		('values', 'type', 'expected'),
```

### Comparing `parsetypes-0.2.3/tests/test_reduce_types.py` & `parsetypes-0.2.4/tests/test_reduce_types.py`

 * *Files identical despite different names*

