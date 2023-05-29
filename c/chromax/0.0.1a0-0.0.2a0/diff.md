# Comparing `tmp/chromax-0.0.1a0.tar.gz` & `tmp/chromax-0.0.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromax-0.0.1a0.tar", last modified: Sun May 28 17:45:03 2023, max compression
+gzip compressed data, was "chromax-0.0.2a0.tar", last modified: Mon May 29 11:09:12 2023, max compression
```

## Comparing `chromax-0.0.1a0.tar` & `chromax-0.0.2a0.tar`

### file list

```diff
@@ -1,23 +1,27 @@
-drwxr-xr-x   0 omar       (501) staff       (20)        0 2023-05-28 17:45:03.337451 chromax-0.0.1a0/
--rw-r--r--   0 omar       (501) staff       (20)     1495 2023-05-26 18:49:32.000000 chromax-0.0.1a0/LICENSE
--rw-r--r--   0 omar       (501) staff       (20)      698 2023-05-28 17:45:03.337304 chromax-0.0.1a0/PKG-INFO
--rw-r--r--   0 omar       (501) staff       (20)      603 2023-04-20 13:14:48.000000 chromax-0.0.1a0/README.md
-drwxr-xr-x   0 omar       (501) staff       (20)        0 2023-05-28 17:45:03.335198 chromax-0.0.1a0/chromax/
--rw-r--r--   0 omar       (501) staff       (20)       57 2023-04-20 13:14:48.000000 chromax-0.0.1a0/chromax/__init__.py
--rw-r--r--   0 omar       (501) staff       (20)     5988 2023-05-25 09:57:10.000000 chromax-0.0.1a0/chromax/functional.py
--rw-r--r--   0 omar       (501) staff       (20)     4059 2023-05-14 19:13:35.000000 chromax-0.0.1a0/chromax/index_functions.py
-drwxr-xr-x   0 omar       (501) staff       (20)        0 2023-05-28 17:45:03.336077 chromax-0.0.1a0/chromax/sample_data/
--rw-r--r--   0 omar       (501) staff       (20)      144 2023-05-11 18:43:22.000000 chromax-0.0.1a0/chromax/sample_data/__init__.py
--rw-r--r--   0 omar       (501) staff       (20)    25140 2023-05-28 14:37:53.000000 chromax-0.0.1a0/chromax/simulator.py
--rw-r--r--   0 omar       (501) staff       (20)     1680 2023-05-11 18:43:22.000000 chromax-0.0.1a0/chromax/trait_model.py
--rw-r--r--   0 omar       (501) staff       (20)      478 2023-04-20 13:14:48.000000 chromax-0.0.1a0/chromax/typing.py
-drwxr-xr-x   0 omar       (501) staff       (20)        0 2023-05-28 17:45:03.335959 chromax-0.0.1a0/chromax.egg-info/
--rw-r--r--   0 omar       (501) staff       (20)      698 2023-05-28 17:45:03.000000 chromax-0.0.1a0/chromax.egg-info/PKG-INFO
--rw-r--r--   0 omar       (501) staff       (20)      367 2023-05-28 17:45:03.000000 chromax-0.0.1a0/chromax.egg-info/SOURCES.txt
--rw-r--r--   0 omar       (501) staff       (20)        1 2023-05-28 17:45:03.000000 chromax-0.0.1a0/chromax.egg-info/dependency_links.txt
--rw-r--r--   0 omar       (501) staff       (20)       34 2023-05-28 17:45:03.000000 chromax-0.0.1a0/chromax.egg-info/requires.txt
--rw-r--r--   0 omar       (501) staff       (20)        8 2023-05-28 17:45:03.000000 chromax-0.0.1a0/chromax.egg-info/top_level.txt
--rw-r--r--   0 omar       (501) staff       (20)       38 2023-05-28 17:45:03.337488 chromax-0.0.1a0/setup.cfg
--rw-r--r--   0 omar       (501) staff       (20)     1015 2023-05-28 17:35:21.000000 chromax-0.0.1a0/setup.py
-drwxr-xr-x   0 omar       (501) staff       (20)        0 2023-05-28 17:45:03.336799 chromax-0.0.1a0/tests/
--rw-r--r--   0 omar       (501) staff       (20)     7220 2023-05-14 18:59:46.000000 chromax-0.0.1a0/tests/test_simulator.py
+drwxr-xr-x   0 omar       (501) staff       (20)        0 2023-05-29 11:09:12.308405 chromax-0.0.2a0/
+-rw-r--r--   0 omar       (501) staff       (20)     1495 2023-05-26 18:49:32.000000 chromax-0.0.2a0/LICENSE
+-rw-r--r--   0 omar       (501) staff       (20)       83 2023-05-28 18:03:05.000000 chromax-0.0.2a0/MANIFEST.in
+-rw-r--r--   0 omar       (501) staff       (20)      698 2023-05-29 11:09:12.308258 chromax-0.0.2a0/PKG-INFO
+-rw-r--r--   0 omar       (501) staff       (20)      603 2023-04-20 13:14:48.000000 chromax-0.0.2a0/README.md
+drwxr-xr-x   0 omar       (501) staff       (20)        0 2023-05-29 11:09:12.296638 chromax-0.0.2a0/chromax/
+-rw-r--r--   0 omar       (501) staff       (20)       57 2023-04-20 13:14:48.000000 chromax-0.0.2a0/chromax/__init__.py
+-rw-r--r--   0 omar       (501) staff       (20)     6465 2023-05-29 09:18:24.000000 chromax-0.0.2a0/chromax/functional.py
+-rw-r--r--   0 omar       (501) staff       (20)     4059 2023-05-14 19:13:35.000000 chromax-0.0.2a0/chromax/index_functions.py
+drwxr-xr-x   0 omar       (501) staff       (20)        0 2023-05-29 11:09:12.299988 chromax-0.0.2a0/chromax/sample_data/
+-rw-r--r--   0 omar       (501) staff       (20)      144 2023-05-11 18:43:22.000000 chromax-0.0.2a0/chromax/sample_data/__init__.py
+-rw-r--r--   0 omar       (501) staff       (20)  1485917 2023-04-20 13:14:48.000000 chromax-0.0.2a0/chromax/sample_data/genetic_map.csv
+-rw-r--r--   0 omar       (501) staff       (20)  7300666 2023-05-11 18:43:22.000000 chromax-0.0.2a0/chromax/sample_data/genome.npy
+-rw-r--r--   0 omar       (501) staff       (20)    25107 2023-05-29 09:16:37.000000 chromax-0.0.2a0/chromax/simulator.py
+-rw-r--r--   0 omar       (501) staff       (20)     1680 2023-05-28 21:21:24.000000 chromax-0.0.2a0/chromax/trait_model.py
+-rw-r--r--   0 omar       (501) staff       (20)      477 2023-05-28 21:19:50.000000 chromax-0.0.2a0/chromax/typing.py
+drwxr-xr-x   0 omar       (501) staff       (20)        0 2023-05-29 11:09:12.297347 chromax-0.0.2a0/chromax.egg-info/
+-rw-r--r--   0 omar       (501) staff       (20)      698 2023-05-29 11:09:12.000000 chromax-0.0.2a0/chromax.egg-info/PKG-INFO
+-rw-r--r--   0 omar       (501) staff       (20)      471 2023-05-29 11:09:12.000000 chromax-0.0.2a0/chromax.egg-info/SOURCES.txt
+-rw-r--r--   0 omar       (501) staff       (20)        1 2023-05-29 11:09:12.000000 chromax-0.0.2a0/chromax.egg-info/dependency_links.txt
+-rw-r--r--   0 omar       (501) staff       (20)       34 2023-05-29 11:09:12.000000 chromax-0.0.2a0/chromax.egg-info/requires.txt
+-rw-r--r--   0 omar       (501) staff       (20)        8 2023-05-29 11:09:12.000000 chromax-0.0.2a0/chromax.egg-info/top_level.txt
+-rw-r--r--   0 omar       (501) staff       (20)       38 2023-05-29 11:09:12.308439 chromax-0.0.2a0/setup.cfg
+-rw-r--r--   0 omar       (501) staff       (20)     1011 2023-05-29 11:07:57.000000 chromax-0.0.2a0/setup.py
+drwxr-xr-x   0 omar       (501) staff       (20)        0 2023-05-29 11:09:12.307215 chromax-0.0.2a0/tests/
+-rw-r--r--   0 omar       (501) staff       (20)     1799 2023-05-29 11:01:53.000000 chromax-0.0.2a0/tests/test_functional.py
+-rw-r--r--   0 omar       (501) staff       (20)     8272 2023-05-29 10:30:14.000000 chromax-0.0.2a0/tests/test_simulator.py
```

### Comparing `chromax-0.0.1a0/LICENSE` & `chromax-0.0.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `chromax-0.0.1a0/PKG-INFO` & `chromax-0.0.2a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromax
-Version: 0.0.1a0
+Version: 0.0.2a0
 Summary: Breeding simulator based on JAX
 Home-page: https://github.com/younik/chromax
 Author: Omar Younis
 Author-email: omar.younis98@gmail.com
 License: bsd-3-clause
 Project-URL: Code, https://github.com/kora-labs/chromax
 Project-URL: Documentation, https://chromax.readthedocs.io/
```

### Comparing `chromax-0.0.1a0/README.md` & `chromax-0.0.2a0/README.md`

 * *Files identical despite different names*

### Comparing `chromax-0.0.1a0/chromax/functional.py` & `chromax-0.0.2a0/chromax/functional.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,46 +11,49 @@
     recombination_vec: Float[Array, N_MARKERS],
     random_key: jax.random.PRNGKeyArray,
 ) -> Population["n"]:
     """Main function that computes crosses from a list of parents.
 
     Args:
         - parents (array): parents to compute the cross. The shape of
-        the parents is (n, 2, m, 2), where n is the number of parents
-        and m is the number of markers.
+        the parents is (n, 2, m, d), where n is the number of parents, 
+        m is the number of markers, and d is the ploidy.
         - recombination_vec (array): array of m probabilities.
         The i-th value represent the probability to recombine before the marker i.
         - random_key (array): PRNGKey, for reproducibility purpose
 
     Returns:
-        - population (array): offspring population of shape (n, m, 2).
+        - population (array): offspring population of shape (n, m, d).
 
     Example:
     >>> from chromax import functional
     >>> import numpy as np
     >>> import jax
-    >>> n_chr, chr_len = 10, 100
+    >>> n_chr, chr_len, ploidy = 10, 100, 2
     >>> n_crosses = 50
-    >>> parents_shape = (n_crosses, 2, n_chr * chr_len, 2)
+    >>> parents_shape = (n_crosses, 2, n_chr * chr_len, ploidy)
     >>> parents = np.random.choice([False, True], size=parents_shape)
     >>> rec_vec = np.full((n_chr, chr_len), 1.5 / chr_len)
     >>> rec_vec[:, 0] = 0.5  # equal probability on starting haploid
     >>> rec_vec = rec_vec.flatten()
     >>> random_key = jax.random.PRNGKey(42)
     >>> f2 = functional.cross(parents, rec_vec, random_key)
     >>> f2.shape
     (50, 1000, 2)
     """
-    random_keys = jax.random.split(random_key, num=len(parents) * 2)
-    random_keys = random_keys.reshape(len(parents), 2, 2)
-    return _cross(parents, recombination_vec, random_keys)
+    parents = parents.reshape(*parents.shape[:3], -1, 2)
+    random_keys = jax.random.split(random_key, num=len(parents) * 2 * parents.shape[3])
+    random_keys = random_keys.reshape(len(parents), 2, parents.shape[3], 2)
+    offsprings = _cross(parents, recombination_vec, random_keys)
+    return offsprings.reshape(*offsprings.shape[:-2], -1)
+
 
 @jax.jit
 @partial(jax.vmap, in_axes=(0, None, 0))  # parallelize across individuals
-@partial(jax.vmap, in_axes=(0, None, 0), out_axes=1)  # parallelize parents
+@partial(jax.vmap, in_axes=(0, None, 0), out_axes=2)  # parallelize parents
 def _cross(
     parent: Individual,
     recombination_vec: Float[Array, N_MARKERS],
     random_key: jax.random.PRNGKeyArray
 ) -> Haploid:
     return _meiosis(
         parent,
@@ -64,45 +67,47 @@
     n_offspring: int,
     recombination_vec: Float[Array, N_MARKERS],
     random_key: jax.random.PRNGKeyArray
 ) -> Population["n n_offspring"]:
     """Computes the double haploid of the input population.
 
     Args:
-        - population (array): input population of shape (n, m, 2).
+        - population (array): input population of shape (n, m, d).
         - n_offspring (int): number of offspring per plant.
         - recombination_vec (array): array of m probabilities.
         The i-th value represent the probability to recombine before the marker i.
         - random_key (array): array of n PRNGKey, one for each individual.
 
     Returns:
-        - population (array): output population of shape (n, n_offspring, m, 2).
+        - population (array): output population of shape (n, n_offspring, m, d).
         This population will be homozygote.
     
     Example:
     >>> from chromax import functional
     >>> import numpy as np
     >>> import jax
-    >>> n_chr, chr_len = 10, 100
-    >>> pop_shape = (50, n_chr * chr_len, 2)
+    >>> n_chr, chr_len, ploidy = 10, 100, 2
+    >>> pop_shape = (50, n_chr * chr_len, ploidy)
     >>> f1 = np.random.choice([False, True], size=pop_shape)
     >>> rec_vec = np.full((n_chr, chr_len), 1.5 / chr_len)
     >>> rec_vec[:, 0] = 0.5  # equal probability on starting haploid
     >>> rec_vec = rec_vec.flatten()
     >>> random_key = jax.random.PRNGKey(42)
     >>> dh = functional.double_haploid(f1, 10, rec_vec, random_key)
     >>> dh.shape
     (50, 10, 1000, 2)
     """
+    population = population.reshape(*population.shape[:2], -1, 2)
     keys = jax.random.split(
         random_key, 
-        num=len(population) * n_offspring
-    ).reshape(len(population), n_offspring, 2)
-    haploid = _double_haploid(population, recombination_vec, keys)
-    return jnp.broadcast_to(haploid[..., None], shape=(*haploid.shape, 2))
+        num=len(population) * n_offspring * population.shape[2]
+    ).reshape(len(population), n_offspring, population.shape[2], 2)
+    haploids = _double_haploid(population, recombination_vec, keys)
+    dh_pop = jnp.broadcast_to(haploids[..., None], shape=(*haploids.shape, 2))
+    return dh_pop.reshape(*dh_pop.shape[:-2], -1)
 
 
 @jax.jit
 @partial(jax.vmap, in_axes=(0, None, 0))  # parallelize across individuals
 @partial(jax.vmap, in_axes=(None, None, 0))  # parallelize across offsprings
 def _double_haploid(
     individual: Individual,
@@ -113,14 +118,15 @@
         individual,
         recombination_vec,
         random_key
     )
 
 
 @jax.jit
+@partial(jax.vmap, in_axes=(1, None, 0), out_axes=1) # parallelize pair of chromosomes
 def _meiosis(
     individual: Individual,
     recombination_vec: Float[Array, N_MARKERS],
     random_key: jax.random.PRNGKeyArray
 ) -> Haploid:
     samples = jax.random.uniform(random_key, shape=recombination_vec.shape)
     rec_sites = samples < recombination_vec
@@ -140,30 +146,30 @@
     population: Population["n"],
     k: int,
     f_index: Callable[[Population["n"]], Float[Array, "n"]]
 ) -> Population["k"]:
     """Function to select individuals based on their score (index).
 
     Args:
-        - population (array): input grouped population of shape (n, m, 2)
+        - population (array): input grouped population of shape (n, m, d)
         - k (int): number of individual to select.
         - f_index (function): function that computes a score for each individual.
         The function accepts as input a population, i.e. and array of shape
         (n, m, 2) and returns an arrray of n float number.
 
     Returns:
-        - population (array): output population of (k, m, 2)
+        - population (array): output population of (k, m, d)
 
     Example:
     >>> from chromax import functional
     >>> from chromax.trait_model import TraitModel
     >>> from chromax.index_functions import conventional_index
     >>> import numpy as np
-    >>> n_chr, chr_len = 10, 100
-    >>> pop_shape = (50, n_chr * chr_len, 2)
+    >>> n_chr, chr_len, ploidy = 10, 100, 2
+    >>> pop_shape = (50, n_chr * chr_len, ploidy)
     >>> f1 = np.random.choice([False, True], size=pop_shape)
     >>> marker_effects = np.random.randn(n_chr * chr_len)
     >>> gebv_model = TraitModel(marker_effects[:, None])
     >>> f_index = conventional_index(gebv_model)
     >>> f2 = functional.select(f1, k=10, f_index=f_index)
     >>> f2.shape
     (10, 1000, 2)
```

### Comparing `chromax-0.0.1a0/chromax/index_functions.py` & `chromax-0.0.2a0/chromax/index_functions.py`

 * *Files identical despite different names*

### Comparing `chromax-0.0.1a0/chromax/simulator.py` & `chromax-0.0.2a0/chromax/simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,20 +200,20 @@
         """
         np.save(file_name, population, allow_pickle=False)
 
     def cross(self, parents: Parents["n"]) -> Population["n"]:
         """Main function that computes crosses from a list of parents.
 
         :param parents: parents to compute the cross. The shape of
-            the parents is (n, 2, m, 2), where n is the number of parents
-            and m is the number of markers.
+            the parents is (n, 2, m, d), where n is the number of parents, 
+            m is the number of markers, and d is the ploidy.
         :type parents: ndarray
 
         
-        :return: offspring population of shape (n, m, 2).
+        :return: offspring population of shape (n, m, d).
         :rtype: ndarray
         
         :Example:
             >>> from chromax import Simulator, sample_data
             >>> import numpy as np
             >>> simulator = Simulator(genetic_map=sample_data.genetic_map)
             >>> f1 = simulator.load_population(sample_data.genome)
@@ -233,29 +233,29 @@
     @property
     def differentiable_cross_func(self) -> Callable:
         """Experimental features that return a differentiable version
         of the cross function.
 
         The differentiable crossing function takes as input:
          - population (array): starting population from which performing the crosses.
-            The shape of the population is (n, m, 2).
-         - cross_weights (array): Array of shape (l, n, 2). It is used to compute
+            The shape of the population is (n, m, d).
+         - cross_weights (array): Array of shape (l, n, d). It is used to compute
             l crosses, starting from a weighted average of the n possible parents. 
             When the n-axis has all zeros except of a single element equals to one,
             this function is equivalent to the cross function.
          - random_key (JAX random key): random key used for recombination sampling.
 
-        And returns a population of shape (l, m, 2).
+        And returns a population of shape (l, m, d).
 
         :Example:
             >>> from chromax import Simulator, sample_data
             >>> import numpy as np
             >>> import jax
             >>> simulator = Simulator(genetic_map=sample_data.genetic_map)
-            >>> diff_cross = simulator.differentiable_cross_func()
+            >>> diff_cross = simulator.differentiable_cross_func
             >>> def mean_gebv(pop, weights, random_key):
                     new_pop = diff_cross(pop, weights, random_key)
                     return simulator.GEBV(new_pop, raw_array=True).mean()
             >>> grad_f = jax.grad(mean_gebv, argnums=1)
             >>> f1 = simulator.load_population(sample_data.genome)
             >>> weights = np.random.uniform(size=(10, len(f1), 2))
             >>> weights /= weights.sum(axis=1, keepdims=True)
@@ -275,18 +275,20 @@
 
         @jax.jit
         def diff_cross_f(
             population: Population["n"],
             cross_weights: Float[Array, "m n 2"],
             random_key: jax.random.PRNGKeyArray
         ) -> Population["m"]:
-            num_keys = len(cross_weights) * len(population) * 2
-            keys = jax.random.split(random_key, num=num_keys)
-            keys = keys.reshape(len(cross_weights), len(population), 2, 2)
+            population = population.reshape(*population.shape[:-1], -1, 2)
+            keys_shape = len(cross_weights), len(population), 2, population.shape[-2]
+            keys = jax.random.split(random_key, num=np.prod(keys_shape))
+            keys = keys.reshape(*keys_shape, 2)
             outer_res = cross_pop(population, self.recombination_vec, keys)
+            outer_res = outer_res.reshape(*outer_res.shape[:-2], -1)
             return (cross_weights[:, :, None, :] * outer_res).sum(axis=1)
 
         return diff_cross_f
 
     def double_haploid(
         self,
         population: Population["n"],
@@ -328,21 +330,21 @@
         self,
         population: Population["n"],
         n_offspring: int = 1
     ) -> Population["n*(n-1)/2 n_offspring"]:
         """Diallel crossing function, i.e. crossing between every possible
         couple, except self-crossing.
 
-        :param population: input population of shape (n, m, 2).
+        :param population: input population of shape (n, m, d).
         :type population: ndarray
         :param n_offspring: number of offspring per cross.
             The default value is 1.
         :type n_offspring: int
 
-        :return: output population of shape (l, n_offspring, m, 2),
+        :return: output population of shape (l, n_offspring, m, d),
             where l is the number of possible pair, i.e `n * (n-1) / 2`.
         :rtype: ndarray
 
         :Example:
             >>> from chromax import Simulator, sample_data
             >>> simulator = Simulator(genetic_map=sample_data.genetic_map)
             >>> f1 = simulator.load_population(sample_data.genome)[:10]
@@ -376,39 +378,33 @@
         self,
         population: Population["n"],
         n_crosses: int,
         n_offspring: int = 1
     ) -> Population["n_crosses n_offspring"]:
         """Computes random crosses on a population.
 
-        :param population: input population of shape (n, m, 2).
+        :param population: input population of shape (n, m, d).
         :type population: ndarray
         :param n_crosses: number of random crosses to perform.
         :type n_crosses: int
         :param n_offspring: number of offspring per cross. 
             The default value is 1.
         :type n_offspring: int
 
-        :return: output population of shape (n_crosses, n_offspring, m, 2).
+        :return: output population of shape (n_crosses, n_offspring, m, d).
         :rtype: ndarray
 
         :Example:
             >>> from chromax import Simulator, sample_data
             >>> simulator = Simulator(genetic_map=sample_data.genetic_map)
             >>> f1 = simulator.load_population(sample_data.genome)
             >>> f2 = simulator.random_crosses(f1, 100, n_offspring=10)
             >>> f2.shape
             (100, 10, 9839, 2)
         """
-
-        if n_crosses < 1:
-            raise ValueError("n_crosses must be higher or equal to 1")
-        if n_offspring < 1:
-            raise ValueError("n_offspring must be higher or equal to 1")
-
         all_indices = np.arange(len(population))
         diallel_indices = self._diallel_indices(all_indices)
         if n_crosses > len(diallel_indices):
             raise ValueError("n_crosses can be at most the diallel length")
 
         self.random_key, split_key = jax.random.split(self.random_key)
         random_select_idx = jax.random.choice(
@@ -430,26 +426,26 @@
         self,
         population: Population["_g n"],
         k: int,
         f_index: Optional[Callable[[Population["n"]], Float[Array, "n"]]] = None
     ) -> Population["_g k"]:
         """Function to select individuals based on their score (index).
 
-        :param population: input population of shape (n, m, 2), 
-            or shape (g, n, m, 2), to select k individual from each group population group g.
+        :param population: input population of shape (n, m, d), 
+            or shape (g, n, m, d), to select k individual from each group population group g.
         :type population: ndarray
         :param k: number of individual to select.
         :type k: int
         :param f_index: function that computes a score from each individual.
             The function accepts as input the population, i.e. and array of shape
-            (n, m, 2) and returns a n float numbers. The default f_index is the conventional index, 
+            (n, m, d) and returns a n float numbers. The default f_index is the conventional index, 
             i.e. the sum of the marker effects masked with the SNPs from the genetic_map.
         :type f_index: Callable
 
-        :return: output population of shape (k, m, 2) or (g, k, m, 2), 
+        :return: output population of shape (k, m, d) or (g, k, m, d), 
             depending on the input population.
         :rtype: ndarray
 
         :Example:
             >>> from chromax import Simulator, sample_data
             >>> simulator = Simulator(genetic_map=sample_data.genetic_map, trait_names=["Yield"])
             >>> f1 = simulator.load_population(sample_data.genome)
@@ -476,15 +472,15 @@
         population: Population["n"],
         *,
         raw_array: bool = False
     ) -> Union[pd.DataFrame, np.ndarray]:
         """Computes the Genomic Estimated Breeding Values using the
         marker effects from the genetic_map.
 
-        :param population: input population of shape (n, m, 2).
+        :param population: input population of shape (n, m, d).
         :type population: ndarray
         :param raw_array: whether to return a raw array or a DataFrame.
             Deafult value is False.
         :type raw_array: bool
 
         :return: a DataFrame (or array) with n rows and a column for each trait.
             It contains the GEBV of each trait for each individual.
@@ -537,15 +533,15 @@
         environments: Optional[np.ndarray] = None,
         raw_array: bool = False
     ) -> Union[pd.DataFrame, np.ndarray]:
         """Simulates the phenotype of a population.
         This uses the Genotype-by-Environment model described in the following:
         https://cran.r-project.org/web/packages/AlphaSimR/vignettes/traits.pdf
 
-        :param population: input population of shape (n, m, 2)
+        :param population: input population of shape (n, m, d)
         :type population: ndarray
         :param num_environments: number of environments to test the population.
             Default value is 1.
         :type num_environments: int
         :param environments: environments to test the population. Each environment
             must be represented by a floating number in the range (-1, 1).
             When drawing new environments use normal distribution to mantain
@@ -593,15 +589,15 @@
     def corrcoef(
         self,
         population: Population["n"]
     ) -> Float[Array, "n"]:
         """Computes the correlation coefficient of the population against its centroid.
         It can be used as an indicator of variance in the population.
 
-        :param population: input population of shape (n, m, 2)
+        :param population: input population of shape (n, m, d)
         :type population: ndarray
 
         :return: vector of length n, containing the correlation coefficient
             of each individual againts the average of the population.
         :rtype: ndarray
 
         :Example:
```

### Comparing `chromax-0.0.1a0/chromax/trait_model.py` & `chromax-0.0.2a0/chromax/trait_model.py`

 * *Files identical despite different names*

### Comparing `chromax-0.0.1a0/chromax.egg-info/PKG-INFO` & `chromax-0.0.2a0/chromax.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromax
-Version: 0.0.1a0
+Version: 0.0.2a0
 Summary: Breeding simulator based on JAX
 Home-page: https://github.com/younik/chromax
 Author: Omar Younis
 Author-email: omar.younis98@gmail.com
 License: bsd-3-clause
 Project-URL: Code, https://github.com/kora-labs/chromax
 Project-URL: Documentation, https://chromax.readthedocs.io/
```

### Comparing `chromax-0.0.1a0/setup.py` & `chromax-0.0.2a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,26 +7,26 @@
     'jaxlib',
     'jaxtyping'
 ]
 
 
 setuptools.setup(
     name='chromax',
-    version='0.0.1a',
+    version='0.0.2a',
     description='Breeding simulator based on JAX',
     url='https://github.com/younik/chromax',
     author='Omar Younis',
     author_email='omar.younis98@gmail.com',
     license='bsd-3-clause',
     keywords=['Breeding', 'simulator', 'JAX', 'chromosome', 'genetics', 'bioinformatics'],
     packages=setuptools.find_packages(),
     python_requires=">=3.8",
     include_package_data=True,
     install_requires=install_requires,
-        project_urls={
+    project_urls={
         "Code": "https://github.com/kora-labs/chromax",
         "Documentation": "https://chromax.readthedocs.io/",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

### Comparing `chromax-0.0.1a0/tests/test_simulator.py` & `chromax-0.0.2a0/tests/test_simulator.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,154 +1,166 @@
 from chromax import Simulator
 from chromax.sample_data import genetic_map, genome
 import jax
 from mock_simulator import MockSimulator
 import numpy as np
 import pytest
 import warnings
+import pandas as pd
 
 
 @pytest.mark.parametrize("idx", [0, 1])
 def test_cross_r(idx):
     n_markers = 1000
     recombination_vec = np.zeros(n_markers, dtype="bool")
     recombination_vec[0] = idx
     simulator = MockSimulator(recombination_vec=recombination_vec)
 
-    size = (1, 2, simulator.n_markers, 2)
+    ploidy = 4
+    size = (1, 2, simulator.n_markers, ploidy)
     parents = np.random.choice(a=[False, True], size=size, p=[0.5, 0.5])
 
     new_pop = simulator.cross(parents)
 
-    assert new_pop.shape == (1, simulator.n_markers, 2)
+    assert new_pop.shape == (1, simulator.n_markers, ploidy)
 
     ind = new_pop[0]
-    assert np.all(ind[:, 0] == parents[0, 0, :, idx])
-    assert np.all(ind[:, 1] == parents[0, 1, :, idx])
+    for i in range(ploidy):
+        pair_chr_idx = i % 2
+        assert np.all(ind[:, i] == parents[0, pair_chr_idx, :, i - pair_chr_idx + idx])
 
 
 def test_equal_parents():
     simulator = Simulator(genetic_map=genetic_map)
 
-    parents = np.zeros((1, 2, simulator.n_markers, 2), dtype="bool")
+    ploidy = 4
+    parents = np.zeros((1, 2, simulator.n_markers, ploidy), dtype="bool")
     child = simulator.cross(parents)
     assert np.all(child == 0)
 
-    parents = np.ones((1, 2, simulator.n_markers, 2), dtype="bool")
+    parents = np.ones((1, 2, simulator.n_markers, ploidy), dtype="bool")
     child = simulator.cross(parents)
     assert np.all(child == 1)
 
 
 def test_ad_hoc_cross():
     rec_vec = np.array(
         [0, 0, 0, 0, 1, 0, 0, 0, 1, 0, 1, 0, 0, 0, 1, 0, 0, 0, 0],
         dtype=np.int8
     )
 
     simulator = MockSimulator(recombination_vec=rec_vec)
-    population = simulator.load_population(2)
+    population = simulator.load_population(2, ploidy=4)
     parents = population[np.array([[0, 1]])]
     child = simulator.cross(parents)
 
     assert child.shape == (1, *population[0].shape)
 
     chr_idx = 0
     for mrk_idx, rec_prob in enumerate(rec_vec):
         if rec_prob == 1:
             chr_idx = 1 - chr_idx
         assert child[1, mrk_idx, 0] == population[0, mrk_idx, chr_idx]
         assert child[1, mrk_idx, 1] == population[1, mrk_idx, chr_idx]
+        assert child[1, mrk_idx, 2] == population[0, mrk_idx, 2 + chr_idx]
+        assert child[1, mrk_idx, 3] == population[1, mrk_idx, 2 + chr_idx]
 
 
 def test_cross_two_times():
     n_markers = 100_000
     n_ind = 2
     simulator = MockSimulator(n_markers=n_markers)
-    population = simulator.load_population(n_ind)
+    population = simulator.load_population(n_ind, ploidy=4)
 
     parents = population[np.array([[0, 1], [0, 1]])]
     children = simulator.cross(parents)
 
     assert np.any(children[0] != children[1])
 
 
 def test_double_haploid():
     n_markers = 1000
     n_ind = 100
     n_offspring = 10
+    ploidy = 4
 
     simulator = MockSimulator(n_markers=n_markers)
-    population = simulator.load_population(n_ind)
+    population = simulator.load_population(n_ind, ploidy=ploidy)
 
     new_pop = simulator.double_haploid(population, n_offspring=n_offspring)
     assert new_pop.shape == (len(population), n_offspring, *population.shape[1:])
     assert np.all(new_pop[..., 0] == new_pop[..., 1])
+    assert np.all(new_pop[..., 2] == new_pop[..., 3])
 
     new_pop = simulator.double_haploid(population)
     assert new_pop.shape == population.shape
     assert np.all(new_pop[..., 0] == new_pop[..., 1])
+    assert np.all(new_pop[..., 2] == new_pop[..., 3])
 
 
 
 def test_diallel():
     n_markers = 1000
     n_ind = 100
+    ploidy = 4
     simulator = MockSimulator(n_markers=n_markers)
-    population = simulator.load_population(n_ind)
+    population = simulator.load_population(n_ind, ploidy=ploidy)
 
     diallel_indices = simulator._diallel_indices(np.arange(10))
     assert len(np.unique(diallel_indices, axis=0)) == 45
 
     new_pop = simulator.diallel(population)
-    assert new_pop.shape == (n_ind * (n_ind - 1) // 2, n_markers, 2)
+    assert new_pop.shape == (n_ind * (n_ind - 1) // 2, n_markers, ploidy)
 
     new_pop = simulator.diallel(population, n_offspring=10)
-    assert new_pop.shape == (n_ind * (n_ind - 1) // 2, 10, n_markers, 2)
+    assert new_pop.shape == (n_ind * (n_ind - 1) // 2, 10, n_markers, ploidy)
 
 def test_select():
     n_markers = 1000
     n_ind = 100
+    ploidy = 4
     simulator = MockSimulator(n_markers=n_markers)
-    population = simulator.load_population(n_ind)
+    population = simulator.load_population(n_ind, ploidy=ploidy)
     pop_GEBV = simulator.GEBV(population)
 
     selected_pop = simulator.select(population, k=10)
     selected_GEBV = simulator.GEBV(selected_pop)
     assert np.all(selected_GEBV.mean() > pop_GEBV.mean())
     assert np.all(selected_GEBV.max() == pop_GEBV.max())
     assert np.all(selected_GEBV.min() > pop_GEBV.min())
 
     dh = simulator.double_haploid(population, n_offspring=100)
     selected_dh = simulator.select(dh, k=5)
-    assert selected_dh.shape == (n_ind, 5, n_markers, 2)
+    assert selected_dh.shape == (n_ind, 5, n_markers, ploidy)
     for i in range(n_ind):
         dh_GEBV = simulator.GEBV(dh[i])
         selected_GEBV = simulator.GEBV(selected_dh[i])
         assert np.all(selected_GEBV.mean() > dh_GEBV.mean())
         assert np.all(selected_GEBV.max() == dh_GEBV.max())
         assert np.all(selected_GEBV.min() > dh_GEBV.min())
 
 
 def test_random_crosses():
     n_markers = 1000
     n_ind = 100
+    ploidy = 4
     simulator = MockSimulator(n_markers=n_markers)
-    population = simulator.load_population(n_ind)
+    population = simulator.load_population(n_ind, ploidy=ploidy)
 
     n_crosses = 300
     new_pop = simulator.random_crosses(population, n_crosses=n_crosses)
-    assert new_pop.shape == (n_crosses, n_markers, 2)
+    assert new_pop.shape == (n_crosses, n_markers, ploidy)
 
     n_offspring = 10
     new_pop = simulator.random_crosses(
         population=population,
         n_crosses=n_crosses,
         n_offspring=n_offspring
     )
-    assert new_pop.shape == (n_crosses, n_offspring, n_markers, 2)
+    assert new_pop.shape == (n_crosses, n_offspring, n_markers, ploidy)
 
 
 def test_multi_trait():
     trait_names = [
         "Heading Date",
         "Protein Content",
         "Plant Height",
@@ -195,29 +207,46 @@
     ])
     new_pop = simulator.cross(dh_pop[cross_indices])
     assert new_pop.device_buffer.device() == device
 
 
 def test_seed_deterministic():
     n_ind = 100
+    ploidy = 4
     simulator1 = Simulator(genetic_map=genetic_map, seed=7)
     simulator2 = Simulator(genetic_map=genetic_map, seed=7)
     mock_simulator = MockSimulator(n_markers=simulator1.n_markers)
-    population = mock_simulator.load_population(n_ind)
+    population = mock_simulator.load_population(n_ind, ploidy=ploidy)
 
     new_pop1 = simulator1.random_crosses(population, n_crosses=10)
     new_pop2 = simulator2.random_crosses(population, n_crosses=10)
 
     assert np.all(new_pop1 == new_pop2)
 
 
+def test_gebv():
+    n_markers, n_ind = 100, 10
+    ploidy = 4
+    simulator = MockSimulator(n_markers=n_markers)
+    population = simulator.load_population(n_ind, ploidy=ploidy)
+
+    gebv_pandas = simulator.GEBV(population)
+    assert len(gebv_pandas) == n_ind
+    assert isinstance(gebv_pandas, pd.DataFrame)
+
+    gebv_array = simulator.GEBV(population, raw_array=True)
+    assert len(gebv_array) == n_ind
+    assert np.all(gebv_pandas.values == gebv_array)
+
+
 def test_phenotyping():
     n_markers, n_ind = 100, 10
+    ploidy = 4
     simulator = MockSimulator(n_markers=n_markers)
-    population = simulator.load_population(n_ind)
+    population = simulator.load_population(n_ind, ploidy=ploidy)
 
     phenotype = simulator.phenotype(population, num_environments=4)
     assert len(phenotype) == n_ind
 
     environments = np.random.uniform(-1, 1, size=(8,))
     _ = simulator.phenotype(population, environments=environments)
     assert len(phenotype) == n_ind
```

