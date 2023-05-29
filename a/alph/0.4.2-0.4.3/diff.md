# Comparing `tmp/alph-0.4.2.tar.gz` & `tmp/alph-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alph-0.4.2.tar", last modified: Thu May 25 12:41:51 2023, max compression
+gzip compressed data, was "alph-0.4.3.tar", last modified: Mon May 29 08:15:46 2023, max compression
```

## Comparing `alph-0.4.2.tar` & `alph-0.4.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:41:51.334094 alph-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-25 12:39:46.000000 alph-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16163 2023-05-25 12:41:51.334094 alph-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14339 2023-05-25 12:39:46.000000 alph-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:41:51.330093 alph-0.4.2/alph/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-25 12:39:46.000000 alph-0.4.2/alph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-25 12:41:50.000000 alph-0.4.2/alph/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-05-25 12:39:46.000000 alph-0.4.2/alph/combo.py
--rw-r--r--   0 runner    (1001) docker     (123)     9769 2023-05-25 12:39:46.000000 alph-0.4.2/alph/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-05-25 12:39:46.000000 alph-0.4.2/alph/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-05-25 12:39:46.000000 alph-0.4.2/alph/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-25 12:39:46.000000 alph-0.4.2/alph/preproc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-05-25 12:39:46.000000 alph-0.4.2/alph/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:41:51.334094 alph-0.4.2/alph.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16163 2023-05-25 12:41:51.000000 alph-0.4.2/alph.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-25 12:41:51.000000 alph-0.4.2/alph.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 12:41:51.000000 alph-0.4.2/alph.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-25 12:41:51.000000 alph-0.4.2/alph.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-25 12:41:51.000000 alph-0.4.2/alph.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 12:41:51.334094 alph-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-25 12:39:46.000000 alph-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:15:46.537806 alph-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-29 08:12:37.000000 alph-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16650 2023-05-29 08:15:46.537806 alph-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14802 2023-05-29 08:12:37.000000 alph-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:15:46.533806 alph-0.4.3/alph/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-29 08:12:37.000000 alph-0.4.3/alph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-29 08:15:45.000000 alph-0.4.3/alph/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-05-29 08:12:37.000000 alph-0.4.3/alph/combo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9769 2023-05-29 08:12:37.000000 alph-0.4.3/alph/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-05-29 08:12:37.000000 alph-0.4.3/alph/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-05-29 08:12:37.000000 alph-0.4.3/alph/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-29 08:12:37.000000 alph-0.4.3/alph/preproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-05-29 08:12:37.000000 alph-0.4.3/alph/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:15:46.537806 alph-0.4.3/alph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16650 2023-05-29 08:15:46.000000 alph-0.4.3/alph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-29 08:15:46.000000 alph-0.4.3/alph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 08:15:46.000000 alph-0.4.3/alph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-29 08:15:46.000000 alph-0.4.3/alph.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-29 08:15:46.000000 alph-0.4.3/alph.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 08:15:46.537806 alph-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-29 08:12:37.000000 alph-0.4.3/setup.py
```

### Comparing `alph-0.4.2/LICENSE` & `alph-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alph-0.4.2/PKG-INFO` & `alph-0.4.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: alph
-Version: 0.4.2
+Version: 0.4.3
 Summary: alph
 Home-page: https://github.com/connectedcompany/alph
 Author: Uros Rapajic
 License: UNKNOWN
 Description: # **alph** - <b>al</b>tair for your gra<b>ph</b>
         
         A Python library using [Altair](https://altair-viz.github.io/) for declarative, data-driven network visualisation.
         
-        <p align="center"><img alt="Alph graph" src="examples/images/small_graph.png" width=60%/></p>
+        <p align="center"><img alt="Alph graph" src="https://github.com/connectedcompany/alph/raw/main/examples/images/small_graph.png" width=60%/></p>
         
         ## Why
         
         Tidy, legible graph visualisations can be elusive. Alph helps by bringing together effective styling, layout and pruning options from across the Python ecosystem.
         
         ## How it works
         
@@ -24,15 +24,15 @@
         
         Best bet is probably to dive straight into the [examples](./examples/), and come back to the API documentation below as needed.
         
         ## Features
         
         - plot any NetworkX Graph
         - support for any layout expressed as a NetworkX `pos` structure (a dict like `{node_id: (x,y), ...}`)
-        - several readily accessible and tunable layout functions (see [example](examples/3_layouts_gallery.ipynb))
+        - several readily accessible and tuneable layout functions (see [example](examples/3_layouts_gallery.ipynb))
         - Altair-style data driven node and edge styling - size, colour, stroke, opacity, scales, conditionals and more
         - convenience args for node labels, halos
         - experimental 1-level "combo" node support
         
         ## Installation
         
         ### Minimal
@@ -40,37 +40,37 @@
         ```
         pip install alph
         ```
         
         ### Recommended
         
         1. for graphviz layout support, install graphviz on your platform - e.g. `brew install graphviz` on Mac,
-           `sudo apt install graphviz` on Debian / Ubuntu etc - or [download the installer](https://graphviz.org/download/)
+           `sudo apt install libgraphviz-dev graphviz` on Colab, Debian, Ubuntu etc - or [download the installer](https://graphviz.org/download/)
         
         2. Install alph with graphviz support:
            ```
            pip install alph[graphviz]
            ```
         3. Install the ForceAtlas2 layout library from our fork, along with cython for speedup
            ```
-           pip install cython git+https://github.com/connectedcompany/forceatlas2.git
+           pip install cython "git+https://github.com/connectedcompany/forceatlas2.git"
            ```
         
         > #### Why is the ForceAtlas2 install separate?
         >
         > [ForceAtlas2](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0098679) is a classic,
         > user feedback led layout algorithm from the [Gephi](https://gephi.org/) team, and the [ForceAtlas2 library](https://github.com/bhargavchippada/forceatlas2)
         > implementation is an excellent, performant Python port. There are two things to be aware of:
         >
         > 1. **GPL licence** - the ForceAtlas2 library, and some of the works it is derived from, are GPL licensed -
         >    hence care is needed when distributing and linking to it. We thus intend to keep its install optional
         >    long term. Since alph uses a plugin design for layout providers, this is straightforward for us to
         >    accommodate, and maintain explicit separation for use cases where GPL is an issue.
         >
-        > 2. **Our fork** - recently, releases of the library have been sporradic - though there is stated intent for
+        > 2. **Our fork** - recently, releases of the library have been sporadic - though there is stated intent for
         >    regular maintenance to resume. In the meantime, we've created a temporary fork to be able to roll in
         >    changes. Currently, our fork incorporates a simple change that enables deterministic layouts.
         
         ## Usage
         
         Simply call the `alph` function with desired options.
         
@@ -81,27 +81,30 @@
         
         G = ...
         alph(G, weight_attr="weight")
         ```
         
         ## Examples
         
-        See [`examples`](./examples). Here's a taster:
+        See [`examples`](./examples). Here's an overview:
         
         - Some of the supported layouts (from the [layouts gallery example](examples/3_layouts_gallery.ipynb)):
-          ![Layouts gallery](examples/images/layouts.png)
+          ![Layouts gallery](https://github.com/connectedcompany/alph/raw/main/examples/images/layouts.png)
         
         - Use of geolocation coordinates for graph layout, (from the [flight routes example](examples/5_flight_routes.ipynb)):
-          ![Geo-location based layout](examples/images/flight_routes.png)
+          ![Geo-location based layout](https://github.com/connectedcompany/alph/raw/main/examples/images/flight_routes.png)
         
+        - Basic styling (from the [styling example](examples/2_styling.ipynb)):
+          ![Styling](https://github.com/uros-r/alph/blob/colab-friendly-examples/examples/images/styling.png?raw=true)
+          
         - A styled interaction network (from the [dolphins example](examples/4_dolphins.ipynb)):
-          ![Dolphins](examples/images/dolphins.png)
+          ![Dolphins](https://github.com/connectedcompany/alph/raw/main/examples/images/dolphins.png)
         
         - "Combo"-style layout (experimental) - category-driven node grouping with edge weight aggregation, from the [Les Mis example](examples/6_les_mis_experimental_combo.ipynb):
-          ![Combo layout](examples/images/combo.png)
+          ![Combo layout](https://github.com/connectedcompany/alph/raw/main/examples/images/combo.png)
         
         ---
         
         # API
         
         ### Supported layout functions
```

### Comparing `alph-0.4.2/README.md` & `alph-0.4.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # **alph** - <b>al</b>tair for your gra<b>ph</b>
 
 A Python library using [Altair](https://altair-viz.github.io/) for declarative, data-driven network visualisation.
 
-<p align="center"><img alt="Alph graph" src="examples/images/small_graph.png" width=60%/></p>
+<p align="center"><img alt="Alph graph" src="https://github.com/connectedcompany/alph/raw/main/examples/images/small_graph.png" width=60%/></p>
 
 ## Why
 
 Tidy, legible graph visualisations can be elusive. Alph helps by bringing together effective styling, layout and pruning options from across the Python ecosystem.
 
 ## How it works
 
@@ -17,15 +17,15 @@
 
 Best bet is probably to dive straight into the [examples](./examples/), and come back to the API documentation below as needed.
 
 ## Features
 
 - plot any NetworkX Graph
 - support for any layout expressed as a NetworkX `pos` structure (a dict like `{node_id: (x,y), ...}`)
-- several readily accessible and tunable layout functions (see [example](examples/3_layouts_gallery.ipynb))
+- several readily accessible and tuneable layout functions (see [example](examples/3_layouts_gallery.ipynb))
 - Altair-style data driven node and edge styling - size, colour, stroke, opacity, scales, conditionals and more
 - convenience args for node labels, halos
 - experimental 1-level "combo" node support
 
 ## Installation
 
 ### Minimal
@@ -33,37 +33,37 @@
 ```
 pip install alph
 ```
 
 ### Recommended
 
 1. for graphviz layout support, install graphviz on your platform - e.g. `brew install graphviz` on Mac,
-   `sudo apt install graphviz` on Debian / Ubuntu etc - or [download the installer](https://graphviz.org/download/)
+   `sudo apt install libgraphviz-dev graphviz` on Colab, Debian, Ubuntu etc - or [download the installer](https://graphviz.org/download/)
 
 2. Install alph with graphviz support:
    ```
    pip install alph[graphviz]
    ```
 3. Install the ForceAtlas2 layout library from our fork, along with cython for speedup
    ```
-   pip install cython git+https://github.com/connectedcompany/forceatlas2.git
+   pip install cython "git+https://github.com/connectedcompany/forceatlas2.git"
    ```
 
 > #### Why is the ForceAtlas2 install separate?
 >
 > [ForceAtlas2](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0098679) is a classic,
 > user feedback led layout algorithm from the [Gephi](https://gephi.org/) team, and the [ForceAtlas2 library](https://github.com/bhargavchippada/forceatlas2)
 > implementation is an excellent, performant Python port. There are two things to be aware of:
 >
 > 1. **GPL licence** - the ForceAtlas2 library, and some of the works it is derived from, are GPL licensed -
 >    hence care is needed when distributing and linking to it. We thus intend to keep its install optional
 >    long term. Since alph uses a plugin design for layout providers, this is straightforward for us to
 >    accommodate, and maintain explicit separation for use cases where GPL is an issue.
 >
-> 2. **Our fork** - recently, releases of the library have been sporradic - though there is stated intent for
+> 2. **Our fork** - recently, releases of the library have been sporadic - though there is stated intent for
 >    regular maintenance to resume. In the meantime, we've created a temporary fork to be able to roll in
 >    changes. Currently, our fork incorporates a simple change that enables deterministic layouts.
 
 ## Usage
 
 Simply call the `alph` function with desired options.
 
@@ -74,27 +74,30 @@
 
 G = ...
 alph(G, weight_attr="weight")
 ```
 
 ## Examples
 
-See [`examples`](./examples). Here's a taster:
+See [`examples`](./examples). Here's an overview:
 
 - Some of the supported layouts (from the [layouts gallery example](examples/3_layouts_gallery.ipynb)):
-  ![Layouts gallery](examples/images/layouts.png)
+  ![Layouts gallery](https://github.com/connectedcompany/alph/raw/main/examples/images/layouts.png)
 
 - Use of geolocation coordinates for graph layout, (from the [flight routes example](examples/5_flight_routes.ipynb)):
-  ![Geo-location based layout](examples/images/flight_routes.png)
+  ![Geo-location based layout](https://github.com/connectedcompany/alph/raw/main/examples/images/flight_routes.png)
 
+- Basic styling (from the [styling example](examples/2_styling.ipynb)):
+  ![Styling](https://github.com/uros-r/alph/blob/colab-friendly-examples/examples/images/styling.png?raw=true)
+  
 - A styled interaction network (from the [dolphins example](examples/4_dolphins.ipynb)):
-  ![Dolphins](examples/images/dolphins.png)
+  ![Dolphins](https://github.com/connectedcompany/alph/raw/main/examples/images/dolphins.png)
 
 - "Combo"-style layout (experimental) - category-driven node grouping with edge weight aggregation, from the [Les Mis example](examples/6_les_mis_experimental_combo.ipynb):
-  ![Combo layout](examples/images/combo.png)
+  ![Combo layout](https://github.com/connectedcompany/alph/raw/main/examples/images/combo.png)
 
 ---
 
 # API
 
 ### Supported layout functions
```

### Comparing `alph-0.4.2/alph/combo.py` & `alph-0.4.3/alph/combo.py`

 * *Files identical despite different names*

### Comparing `alph-0.4.2/alph/core.py` & `alph-0.4.3/alph/core.py`

 * *Files identical despite different names*

### Comparing `alph-0.4.2/alph/layers.py` & `alph-0.4.3/alph/layers.py`

 * *Files identical despite different names*

### Comparing `alph-0.4.2/alph/layout.py` & `alph-0.4.3/alph/layout.py`

 * *Files identical despite different names*

### Comparing `alph-0.4.2/alph/preproc.py` & `alph-0.4.3/alph/preproc.py`

 * *Files identical despite different names*

### Comparing `alph-0.4.2/alph/util.py` & `alph-0.4.3/alph/util.py`

 * *Files identical despite different names*

### Comparing `alph-0.4.2/alph.egg-info/PKG-INFO` & `alph-0.4.3/alph.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: alph
-Version: 0.4.2
+Version: 0.4.3
 Summary: alph
 Home-page: https://github.com/connectedcompany/alph
 Author: Uros Rapajic
 License: UNKNOWN
 Description: # **alph** - <b>al</b>tair for your gra<b>ph</b>
         
         A Python library using [Altair](https://altair-viz.github.io/) for declarative, data-driven network visualisation.
         
-        <p align="center"><img alt="Alph graph" src="examples/images/small_graph.png" width=60%/></p>
+        <p align="center"><img alt="Alph graph" src="https://github.com/connectedcompany/alph/raw/main/examples/images/small_graph.png" width=60%/></p>
         
         ## Why
         
         Tidy, legible graph visualisations can be elusive. Alph helps by bringing together effective styling, layout and pruning options from across the Python ecosystem.
         
         ## How it works
         
@@ -24,15 +24,15 @@
         
         Best bet is probably to dive straight into the [examples](./examples/), and come back to the API documentation below as needed.
         
         ## Features
         
         - plot any NetworkX Graph
         - support for any layout expressed as a NetworkX `pos` structure (a dict like `{node_id: (x,y), ...}`)
-        - several readily accessible and tunable layout functions (see [example](examples/3_layouts_gallery.ipynb))
+        - several readily accessible and tuneable layout functions (see [example](examples/3_layouts_gallery.ipynb))
         - Altair-style data driven node and edge styling - size, colour, stroke, opacity, scales, conditionals and more
         - convenience args for node labels, halos
         - experimental 1-level "combo" node support
         
         ## Installation
         
         ### Minimal
@@ -40,37 +40,37 @@
         ```
         pip install alph
         ```
         
         ### Recommended
         
         1. for graphviz layout support, install graphviz on your platform - e.g. `brew install graphviz` on Mac,
-           `sudo apt install graphviz` on Debian / Ubuntu etc - or [download the installer](https://graphviz.org/download/)
+           `sudo apt install libgraphviz-dev graphviz` on Colab, Debian, Ubuntu etc - or [download the installer](https://graphviz.org/download/)
         
         2. Install alph with graphviz support:
            ```
            pip install alph[graphviz]
            ```
         3. Install the ForceAtlas2 layout library from our fork, along with cython for speedup
            ```
-           pip install cython git+https://github.com/connectedcompany/forceatlas2.git
+           pip install cython "git+https://github.com/connectedcompany/forceatlas2.git"
            ```
         
         > #### Why is the ForceAtlas2 install separate?
         >
         > [ForceAtlas2](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0098679) is a classic,
         > user feedback led layout algorithm from the [Gephi](https://gephi.org/) team, and the [ForceAtlas2 library](https://github.com/bhargavchippada/forceatlas2)
         > implementation is an excellent, performant Python port. There are two things to be aware of:
         >
         > 1. **GPL licence** - the ForceAtlas2 library, and some of the works it is derived from, are GPL licensed -
         >    hence care is needed when distributing and linking to it. We thus intend to keep its install optional
         >    long term. Since alph uses a plugin design for layout providers, this is straightforward for us to
         >    accommodate, and maintain explicit separation for use cases where GPL is an issue.
         >
-        > 2. **Our fork** - recently, releases of the library have been sporradic - though there is stated intent for
+        > 2. **Our fork** - recently, releases of the library have been sporadic - though there is stated intent for
         >    regular maintenance to resume. In the meantime, we've created a temporary fork to be able to roll in
         >    changes. Currently, our fork incorporates a simple change that enables deterministic layouts.
         
         ## Usage
         
         Simply call the `alph` function with desired options.
         
@@ -81,27 +81,30 @@
         
         G = ...
         alph(G, weight_attr="weight")
         ```
         
         ## Examples
         
-        See [`examples`](./examples). Here's a taster:
+        See [`examples`](./examples). Here's an overview:
         
         - Some of the supported layouts (from the [layouts gallery example](examples/3_layouts_gallery.ipynb)):
-          ![Layouts gallery](examples/images/layouts.png)
+          ![Layouts gallery](https://github.com/connectedcompany/alph/raw/main/examples/images/layouts.png)
         
         - Use of geolocation coordinates for graph layout, (from the [flight routes example](examples/5_flight_routes.ipynb)):
-          ![Geo-location based layout](examples/images/flight_routes.png)
+          ![Geo-location based layout](https://github.com/connectedcompany/alph/raw/main/examples/images/flight_routes.png)
         
+        - Basic styling (from the [styling example](examples/2_styling.ipynb)):
+          ![Styling](https://github.com/uros-r/alph/blob/colab-friendly-examples/examples/images/styling.png?raw=true)
+          
         - A styled interaction network (from the [dolphins example](examples/4_dolphins.ipynb)):
-          ![Dolphins](examples/images/dolphins.png)
+          ![Dolphins](https://github.com/connectedcompany/alph/raw/main/examples/images/dolphins.png)
         
         - "Combo"-style layout (experimental) - category-driven node grouping with edge weight aggregation, from the [Les Mis example](examples/6_les_mis_experimental_combo.ipynb):
-          ![Combo layout](examples/images/combo.png)
+          ![Combo layout](https://github.com/connectedcompany/alph/raw/main/examples/images/combo.png)
         
         ---
         
         # API
         
         ### Supported layout functions
```

### Comparing `alph-0.4.2/setup.py` & `alph-0.4.3/setup.py`

 * *Files identical despite different names*

