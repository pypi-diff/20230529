# Comparing `tmp/berens-neat-0.1.1.tar.gz` & `tmp/berens-neat-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "berens-neat-0.1.1.tar", last modified: Sun May 28 11:38:29 2023, max compression
+gzip compressed data, was "berens-neat-0.1.2.tar", last modified: Sun May 28 13:39:38 2023, max compression
```

## Comparing `berens-neat-0.1.1.tar` & `berens-neat-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 charlie   (1000) charlie   (1000)        0 2023-05-28 11:38:29.221498 berens-neat-0.1.1/
--rw-r--r--   0 charlie   (1000) charlie   (1000)     1058 2023-05-28 11:15:24.000000 berens-neat-0.1.1/LICENSE
--rw-r--r--   0 charlie   (1000) charlie   (1000)     1266 2023-05-28 11:38:29.221498 berens-neat-0.1.1/PKG-INFO
--rw-r--r--   0 charlie   (1000) charlie   (1000)      772 2023-05-27 21:27:50.000000 berens-neat-0.1.1/README.md
-drwxr-xr-x   0 charlie   (1000) charlie   (1000)        0 2023-05-28 11:38:29.221498 berens-neat-0.1.1/berens_neat.egg-info/
--rw-r--r--   0 charlie   (1000) charlie   (1000)     1266 2023-05-28 11:38:29.000000 berens-neat-0.1.1/berens_neat.egg-info/PKG-INFO
--rw-r--r--   0 charlie   (1000) charlie   (1000)      337 2023-05-28 11:38:29.000000 berens-neat-0.1.1/berens_neat.egg-info/SOURCES.txt
--rw-r--r--   0 charlie   (1000) charlie   (1000)        1 2023-05-28 11:38:29.000000 berens-neat-0.1.1/berens_neat.egg-info/dependency_links.txt
--rw-r--r--   0 charlie   (1000) charlie   (1000)       10 2023-05-28 11:38:29.000000 berens-neat-0.1.1/berens_neat.egg-info/top_level.txt
-drwxr-xr-x   0 charlie   (1000) charlie   (1000)        0 2023-05-28 11:38:29.221498 berens-neat-0.1.1/neat/
--rw-r--r--   0 charlie   (1000) charlie   (1000)     5184 2023-05-28 11:15:24.000000 berens-neat-0.1.1/neat/__init__.py
--rw-r--r--   0 charlie   (1000) charlie   (1000)      131 2023-05-28 11:15:24.000000 berens-neat-0.1.1/neat/activations.py
--rw-r--r--   0 charlie   (1000) charlie   (1000)     2915 2023-05-28 11:37:51.000000 berens-neat-0.1.1/neat/config.py
--rw-r--r--   0 charlie   (1000) charlie   (1000)    17561 2023-05-28 11:15:24.000000 berens-neat-0.1.1/neat/organism.py
--rw-r--r--   0 charlie   (1000) charlie   (1000)     2458 2023-05-28 11:15:24.000000 berens-neat-0.1.1/neat/population.py
--rw-r--r--   0 charlie   (1000) charlie   (1000)     4526 2023-05-28 11:15:24.000000 berens-neat-0.1.1/neat/reporter.py
--rw-r--r--   0 charlie   (1000) charlie   (1000)     7986 2023-05-28 11:15:24.000000 berens-neat-0.1.1/neat/reproduction.py
--rw-r--r--   0 charlie   (1000) charlie   (1000)     2156 2023-05-28 11:15:24.000000 berens-neat-0.1.1/neat/species.py
--rw-r--r--   0 charlie   (1000) charlie   (1000)      123 2023-05-28 11:15:24.000000 berens-neat-0.1.1/neat/utils.py
--rw-r--r--   0 charlie   (1000) charlie   (1000)      669 2023-05-28 11:38:11.000000 berens-neat-0.1.1/pyproject.toml
--rw-r--r--   0 charlie   (1000) charlie   (1000)       38 2023-05-28 11:38:29.221498 berens-neat-0.1.1/setup.cfg
--rw-r--r--   0 charlie   (1000) charlie   (1000)      136 2023-05-28 11:15:24.000000 berens-neat-0.1.1/setup.py
+drwxr-xr-x   0 charlie   (1000) charlie   (1000)        0 2023-05-28 13:39:38.681271 berens-neat-0.1.2/
+-rw-r--r--   0 charlie   (1000) charlie   (1000)     1058 2023-05-28 11:15:24.000000 berens-neat-0.1.2/LICENSE
+-rw-r--r--   0 charlie   (1000) charlie   (1000)     1316 2023-05-28 13:39:38.681271 berens-neat-0.1.2/PKG-INFO
+-rw-r--r--   0 charlie   (1000) charlie   (1000)      822 2023-05-28 11:39:18.000000 berens-neat-0.1.2/README.md
+drwxr-xr-x   0 charlie   (1000) charlie   (1000)        0 2023-05-28 13:39:38.661271 berens-neat-0.1.2/berens_neat.egg-info/
+-rw-r--r--   0 charlie   (1000) charlie   (1000)     1316 2023-05-28 13:39:38.000000 berens-neat-0.1.2/berens_neat.egg-info/PKG-INFO
+-rw-r--r--   0 charlie   (1000) charlie   (1000)      337 2023-05-28 13:39:38.000000 berens-neat-0.1.2/berens_neat.egg-info/SOURCES.txt
+-rw-r--r--   0 charlie   (1000) charlie   (1000)        1 2023-05-28 13:39:38.000000 berens-neat-0.1.2/berens_neat.egg-info/dependency_links.txt
+-rw-r--r--   0 charlie   (1000) charlie   (1000)       10 2023-05-28 13:39:38.000000 berens-neat-0.1.2/berens_neat.egg-info/top_level.txt
+drwxr-xr-x   0 charlie   (1000) charlie   (1000)        0 2023-05-28 13:39:38.681271 berens-neat-0.1.2/neat/
+-rw-r--r--   0 charlie   (1000) charlie   (1000)     5184 2023-05-28 11:15:24.000000 berens-neat-0.1.2/neat/__init__.py
+-rw-r--r--   0 charlie   (1000) charlie   (1000)      131 2023-05-28 11:15:24.000000 berens-neat-0.1.2/neat/activations.py
+-rw-r--r--   0 charlie   (1000) charlie   (1000)     2932 2023-05-28 11:42:05.000000 berens-neat-0.1.2/neat/config.py
+-rw-r--r--   0 charlie   (1000) charlie   (1000)    17583 2023-05-28 11:49:28.000000 berens-neat-0.1.2/neat/organism.py
+-rw-r--r--   0 charlie   (1000) charlie   (1000)     2458 2023-05-28 11:15:24.000000 berens-neat-0.1.2/neat/population.py
+-rw-r--r--   0 charlie   (1000) charlie   (1000)     4526 2023-05-28 11:15:24.000000 berens-neat-0.1.2/neat/reporter.py
+-rw-r--r--   0 charlie   (1000) charlie   (1000)     7986 2023-05-28 11:15:24.000000 berens-neat-0.1.2/neat/reproduction.py
+-rw-r--r--   0 charlie   (1000) charlie   (1000)     2156 2023-05-28 11:15:24.000000 berens-neat-0.1.2/neat/species.py
+-rw-r--r--   0 charlie   (1000) charlie   (1000)      123 2023-05-28 11:15:24.000000 berens-neat-0.1.2/neat/utils.py
+-rw-r--r--   0 charlie   (1000) charlie   (1000)      669 2023-05-28 13:39:11.000000 berens-neat-0.1.2/pyproject.toml
+-rw-r--r--   0 charlie   (1000) charlie   (1000)       38 2023-05-28 13:39:38.681271 berens-neat-0.1.2/setup.cfg
+-rw-r--r--   0 charlie   (1000) charlie   (1000)      136 2023-05-28 11:15:24.000000 berens-neat-0.1.2/setup.py
```

### Comparing `berens-neat-0.1.1/LICENSE` & `berens-neat-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `berens-neat-0.1.1/PKG-INFO` & `berens-neat-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: berens-neat
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple implementation of NEAT in Python
 Author-email: Charlie Berens <charliejb3@gmail.com>
 Project-URL: Homepage, https://github.com/charlieberens/neat
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,7 +15,13 @@
 # NEAT
 ## Algorithm
 This is a Python implementation of the **NeuroEvolution of Augmenting Topologies (NEAT)** algorithm described [here](https://nn.cs.utexas.edu/downloads/papers/stanley.ec02.pdf).
 
 **NEAT** is an evolutionary algorithm for reinforcement learning based on evolving neural networks. It provides a set of mutations that change connection weights and network topology, and preserves new mutations by dividing networks into species that are protected for a number of generations.
 
 I stay  mostly faithful to the original paper. The one major change that I made (that stuck) is how I implement biases. The authors of the originial paper simply added an input pin with a value of 1 to their networks. I, on the other hand, give each node its own bias value.   
+
+## Installation
+```
+pip install berens-neat
+```
+
```

### Comparing `berens-neat-0.1.1/README.md` & `berens-neat-0.1.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,13 @@
 # NEAT
 ## Algorithm
 This is a Python implementation of the **NeuroEvolution of Augmenting Topologies (NEAT)** algorithm described [here](https://nn.cs.utexas.edu/downloads/papers/stanley.ec02.pdf).
 
 **NEAT** is an evolutionary algorithm for reinforcement learning based on evolving neural networks. It provides a set of mutations that change connection weights and network topology, and preserves new mutations by dividing networks into species that are protected for a number of generations.
 
 I stay  mostly faithful to the original paper. The one major change that I made (that stuck) is how I implement biases. The authors of the originial paper simply added an input pin with a value of 1 to their networks. I, on the other hand, give each node its own bias value.   
+
+## Installation
+```
+pip install berens-neat
+```
+
```

### Comparing `berens-neat-0.1.1/berens_neat.egg-info/PKG-INFO` & `berens-neat-0.1.2/berens_neat.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: berens-neat
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple implementation of NEAT in Python
 Author-email: Charlie Berens <charliejb3@gmail.com>
 Project-URL: Homepage, https://github.com/charlieberens/neat
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,7 +15,13 @@
 # NEAT
 ## Algorithm
 This is a Python implementation of the **NeuroEvolution of Augmenting Topologies (NEAT)** algorithm described [here](https://nn.cs.utexas.edu/downloads/papers/stanley.ec02.pdf).
 
 **NEAT** is an evolutionary algorithm for reinforcement learning based on evolving neural networks. It provides a set of mutations that change connection weights and network topology, and preserves new mutations by dividing networks into species that are protected for a number of generations.
 
 I stay  mostly faithful to the original paper. The one major change that I made (that stuck) is how I implement biases. The authors of the originial paper simply added an input pin with a value of 1 to their networks. I, on the other hand, give each node its own bias value.   
+
+## Installation
+```
+pip install berens-neat
+```
+
```

### Comparing `berens-neat-0.1.1/neat/__init__.py` & `berens-neat-0.1.2/neat/__init__.py`

 * *Files identical despite different names*

### Comparing `berens-neat-0.1.1/neat/config.py` & `berens-neat-0.1.2/neat/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,8 +101,9 @@
     """
     Load a config from a file
     """
     file_config = {}
     if file:
         with open(file, "r") as f:
             file_config = json.load(f)
-    return config | file_config
+    config.update(file_config)
+    return config
```

### Comparing `berens-neat-0.1.1/neat/organism.py` & `berens-neat-0.1.2/neat/organism.py`

 * *Files 0% similar despite different names*

```diff
@@ -276,15 +276,15 @@
         """
         Takes inputs [-1, -2, -3, ... -n] and returns outputs [0, 1, 2, ... m-1]
         Where n is the number of input nodes and m is the number of output nodes
         """
         layers = self.calculate_layers()
 
         if len(inputs) != self.config["input_nodes"]:
-            raise ValueError(f"Expected {len(layers[0])} inputs, got {len(inputs)}")
+            raise ValueError("Expected {} inputs, got {}".format(self.config["input_nodes"], len(inputs)))
 
         for node in self.nodes:
             node.value = node.bias
 
         for i, input_node in enumerate(layers[0 : self.config["input_nodes"]]):
             input_node.value += inputs[i]
```

### Comparing `berens-neat-0.1.1/neat/population.py` & `berens-neat-0.1.2/neat/population.py`

 * *Files identical despite different names*

### Comparing `berens-neat-0.1.1/neat/reporter.py` & `berens-neat-0.1.2/neat/reporter.py`

 * *Files identical despite different names*

### Comparing `berens-neat-0.1.1/neat/reproduction.py` & `berens-neat-0.1.2/neat/reproduction.py`

 * *Files identical despite different names*

### Comparing `berens-neat-0.1.1/neat/species.py` & `berens-neat-0.1.2/neat/species.py`

 * *Files identical despite different names*

### Comparing `berens-neat-0.1.1/pyproject.toml` & `berens-neat-0.1.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "berens-neat"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Charlie Berens", email="charliejb3@gmail.com" },
 ]
 description = "A simple implementation of NEAT in Python"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

