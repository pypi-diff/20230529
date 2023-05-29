# Comparing `tmp/pandas-parallel-apply-2.1.tar.gz` & `tmp/pandas-parallel-apply-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas-parallel-apply-2.1.tar", last modified: Sun May  7 19:22:17 2023, max compression
+gzip compressed data, was "pandas-parallel-apply-2.2.tar", last modified: Mon May 29 20:52:12 2023, max compression
```

## Comparing `pandas-parallel-apply-2.1.tar` & `pandas-parallel-apply-2.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-05-07 19:22:17.121851 pandas-parallel-apply-2.1/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      483 2023-05-04 05:18:15.000000 pandas-parallel-apply-2.1/LICENSE
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3978 2023-05-07 19:22:17.121851 pandas-parallel-apply-2.1/PKG-INFO
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3700 2023-05-07 19:20:31.000000 pandas-parallel-apply-2.1/README.md
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-05-07 19:22:17.121851 pandas-parallel-apply-2.1/pandas_parallel_apply/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      157 2023-05-04 05:18:15.000000 pandas-parallel-apply-2.1/pandas_parallel_apply/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1788 2023-05-04 06:57:52.000000 pandas-parallel-apply-2.1/pandas_parallel_apply/data_frame_parallel.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3711 2023-05-04 06:57:52.000000 pandas-parallel-apply-2.1/pandas_parallel_apply/groupby_parallel.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3230 2023-05-04 06:57:31.000000 pandas-parallel-apply-2.1/pandas_parallel_apply/logger.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      974 2023-05-04 06:57:52.000000 pandas-parallel-apply-2.1/pandas_parallel_apply/series_parallel.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2139 2023-05-04 06:57:52.000000 pandas-parallel-apply-2.1/pandas_parallel_apply/utils.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-05-07 19:22:17.121851 pandas-parallel-apply-2.1/pandas_parallel_apply.egg-info/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3978 2023-05-07 19:22:17.000000 pandas-parallel-apply-2.1/pandas_parallel_apply.egg-info/PKG-INFO
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      572 2023-05-07 19:22:17.000000 pandas-parallel-apply-2.1/pandas_parallel_apply.egg-info/SOURCES.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        1 2023-05-07 19:22:17.000000 pandas-parallel-apply-2.1/pandas_parallel_apply.egg-info/dependency_links.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       71 2023-05-07 19:22:17.000000 pandas-parallel-apply-2.1/pandas_parallel_apply.egg-info/requires.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       22 2023-05-07 19:22:17.000000 pandas-parallel-apply-2.1/pandas_parallel_apply.egg-info/top_level.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       38 2023-05-07 19:22:17.121851 pandas-parallel-apply-2.1/setup.cfg
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1830 2023-05-07 19:21:47.000000 pandas-parallel-apply-2.1/setup.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-05-07 19:22:17.121851 pandas-parallel-apply-2.1/test/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      562 2023-05-04 06:58:51.000000 pandas-parallel-apply-2.1/test/test_apply_df.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      502 2023-05-04 06:57:31.000000 pandas-parallel-apply-2.1/test/test_apply_df_col.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2041 2023-05-04 06:57:31.000000 pandas-parallel-apply-2.1/test/test_apply_df_groupby.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      553 2023-05-04 06:57:31.000000 pandas-parallel-apply-2.1/test/test_utils.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-05-29 20:52:12.205342 pandas-parallel-apply-2.2/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      483 2023-05-04 05:18:15.000000 pandas-parallel-apply-2.2/LICENSE
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     4190 2023-05-29 20:52:12.205342 pandas-parallel-apply-2.2/PKG-INFO
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3912 2023-05-29 19:31:39.000000 pandas-parallel-apply-2.2/README.md
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-05-29 20:52:12.205342 pandas-parallel-apply-2.2/pandas_parallel_apply/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      157 2023-05-04 05:18:15.000000 pandas-parallel-apply-2.2/pandas_parallel_apply/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1596 2023-05-29 20:09:23.000000 pandas-parallel-apply-2.2/pandas_parallel_apply/data_frame_parallel.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3969 2023-05-29 19:24:32.000000 pandas-parallel-apply-2.2/pandas_parallel_apply/groupby_parallel.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3230 2023-05-04 06:57:31.000000 pandas-parallel-apply-2.2/pandas_parallel_apply/logger.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      770 2023-05-29 19:55:47.000000 pandas-parallel-apply-2.2/pandas_parallel_apply/series_parallel.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3145 2023-05-29 20:50:53.000000 pandas-parallel-apply-2.2/pandas_parallel_apply/utils.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-05-29 20:52:12.205342 pandas-parallel-apply-2.2/pandas_parallel_apply.egg-info/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     4190 2023-05-29 20:52:12.000000 pandas-parallel-apply-2.2/pandas_parallel_apply.egg-info/PKG-INFO
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      572 2023-05-29 20:52:12.000000 pandas-parallel-apply-2.2/pandas_parallel_apply.egg-info/SOURCES.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        1 2023-05-29 20:52:12.000000 pandas-parallel-apply-2.2/pandas_parallel_apply.egg-info/dependency_links.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       57 2023-05-29 20:52:12.000000 pandas-parallel-apply-2.2/pandas_parallel_apply.egg-info/requires.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       22 2023-05-29 20:52:12.000000 pandas-parallel-apply-2.2/pandas_parallel_apply.egg-info/top_level.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       38 2023-05-29 20:52:12.205342 pandas-parallel-apply-2.2/setup.cfg
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1830 2023-05-29 20:52:04.000000 pandas-parallel-apply-2.2/setup.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-05-29 20:52:12.205342 pandas-parallel-apply-2.2/test/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      562 2023-05-29 20:51:28.000000 pandas-parallel-apply-2.2/test/test_apply_df.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      502 2023-05-04 06:57:31.000000 pandas-parallel-apply-2.2/test/test_apply_df_col.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2537 2023-05-29 19:53:59.000000 pandas-parallel-apply-2.2/test/test_apply_df_groupby.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      553 2023-05-04 06:57:31.000000 pandas-parallel-apply-2.2/test/test_utils.py
```

### Comparing `pandas-parallel-apply-2.1/PKG-INFO` & `pandas-parallel-apply-2.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-parallel-apply
-Version: 2.1
+Version: 2.2
 Summary: Wrapper for df and df[col].apply parallelized
 Home-page: https://gitlab.com/meehai/pandas-parallel-apply
 License: WTFPL
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -66,33 +66,41 @@
 `df.apply(fn, axis=0)` is not because it may require rows that are on other workers.
 
 It is assumed that each row is processed in similar time, so the N/K chunks will finishe more or less at the same time.
 
 ### Future Improvement
 
 Not supported but may be interesting: define also a number of chunks (C>K), so the df is actually split in N/C chunks,
-and theses are passed using a round-robin approach to the K processes. Right now, C=K, so whenever one process finishes,
-it will not be assigned any more work.
+and theses are passed using a round-robin approach to the K processes. Right now, C=K, so whenever one process
+finishes, it will not be assigned any more work.
 
 ## n_cores semantics
 - `n_cores < -1` -> throws an error
 - `n_cores == -1` -> uses `cpu_count()` - 1 cores
 - `n_cores == 0` -> uses serial/standard pandas functions
 - `n_cores == 1` -> spawns a single process alongside the main one
 - `n_cores > 1` -> spanws N processes and chunks the df
 - `n_cores > cpu_cpunt()` -> throws an warning
 - `n_cores > len(df)` -> limits to `len(df)`
 
-On CPU-bound tasks (calculations), `n_cores = -1` is likely to be fastest. On network-bound operations (e.g., where threads may invoke network calls),
-using a very high `n_cores` value may be beneficial.
+On CPU-bound tasks (calculations), `n_cores = -1` is likely to be fastest. On network-bound operations (e.g., where
+threads may invoke network calls), using a very high `n_cores` value may be beneficial.
 
 ## Disclaimers
 
 - This is an experimental repository. It may lead to unexpected behaviour.
 
-- Not all the merging semantics of pandas are supported. Pandas has weird and complex methods of converting an apply return. For example, a series apply function may return a dataframe, a series, a dict, a list, etc. All of these are converted in some specific way. Some cases may not be supported.
+- Not all the merging semantics of pandas are supported. Pandas has weird and complex methods of converting an apply
+return. For example, a series apply function may return a dataframe, a series, a dict, a list, etc. All of these are
+converted in some specific way. Some cases may not be supported.
+
+- Groupby apply functions are **much** slower than their serial variant currently. Still experimenting with how to make
+it faster. It looks correct, just 10-100x slower for some small examples. May be better as dataframe get bigger.
+
+- Using `n_cores = 1` will create a multiprocessing pool of just 1 core, so the code is parallel (thus not running on
+the main process), but may not yield much speed improvement, except for not blocking the main process. May be useful
+in some GUI apps.
 
-- Groupby apply functions are **much** slower than their serial variant currently. Still experimenting with how to make it faster. It looks correct, just 10-100x slower for some small examples. May be better as dataframe get bigger.
-
-- Using `n_cores = 1` will create a multiprocessing pool of just 1 core, so the code is parallel (thus not running on the main process), but may not yield much speed improvement, except for not blocking the main process. May be useful in some GUI apps.
+- You can use `parallelism=multithread` of `parallelism=multiprocess` (2nd is default) for all constructors. Using
+multiprocess requires the functions to be picklable though (lambda for example, must be global)
 
 That's all.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pandas-parallel-apply Version: 2.1 Summary: Wrapper
+Metadata-Version: 2.1 Name: pandas-parallel-apply Version: 2.2 Summary: Wrapper
 for df and df[col].apply parallelized Home-page: https://gitlab.com/meehai/
 pandas-parallel-apply License: WTFPL Requires-Python: >=3.8 Description-
 Content-Type: text/markdown License-File: LICENSE # pandas-parallel-apply
                         [License] [PyPi_Latest_Release]
 Parallel wrappers for `df.apply(fn)`, `df[col].apply(fn)`, `series.apply(fn)`,
 and `df.groupby([cols]).apply(fn)`, with tqdm progress bars included. ##
 Installation `pip install pandas-parallel-apply` Import with: ```python from
@@ -41,8 +41,11 @@
 a list, etc. All of these are converted in some specific way. Some cases may
 not be supported. - Groupby apply functions are **much** slower than their
 serial variant currently. Still experimenting with how to make it faster. It
 looks correct, just 10-100x slower for some small examples. May be better as
 dataframe get bigger. - Using `n_cores = 1` will create a multiprocessing pool
 of just 1 core, so the code is parallel (thus not running on the main process),
 but may not yield much speed improvement, except for not blocking the main
-process. May be useful in some GUI apps. That's all.
+process. May be useful in some GUI apps. - You can use
+`parallelism=multithread` of `parallelism=multiprocess` (2nd is default) for
+all constructors. Using multiprocess requires the functions to be picklable
+though (lambda for example, must be global) That's all.
```

### Comparing `pandas-parallel-apply-2.1/README.md` & `pandas-parallel-apply-2.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -56,33 +56,41 @@
 `df.apply(fn, axis=0)` is not because it may require rows that are on other workers.
 
 It is assumed that each row is processed in similar time, so the N/K chunks will finishe more or less at the same time.
 
 ### Future Improvement
 
 Not supported but may be interesting: define also a number of chunks (C>K), so the df is actually split in N/C chunks,
-and theses are passed using a round-robin approach to the K processes. Right now, C=K, so whenever one process finishes,
-it will not be assigned any more work.
+and theses are passed using a round-robin approach to the K processes. Right now, C=K, so whenever one process
+finishes, it will not be assigned any more work.
 
 ## n_cores semantics
 - `n_cores < -1` -> throws an error
 - `n_cores == -1` -> uses `cpu_count()` - 1 cores
 - `n_cores == 0` -> uses serial/standard pandas functions
 - `n_cores == 1` -> spawns a single process alongside the main one
 - `n_cores > 1` -> spanws N processes and chunks the df
 - `n_cores > cpu_cpunt()` -> throws an warning
 - `n_cores > len(df)` -> limits to `len(df)`
 
-On CPU-bound tasks (calculations), `n_cores = -1` is likely to be fastest. On network-bound operations (e.g., where threads may invoke network calls),
-using a very high `n_cores` value may be beneficial.
+On CPU-bound tasks (calculations), `n_cores = -1` is likely to be fastest. On network-bound operations (e.g., where
+threads may invoke network calls), using a very high `n_cores` value may be beneficial.
 
 ## Disclaimers
 
 - This is an experimental repository. It may lead to unexpected behaviour.
 
-- Not all the merging semantics of pandas are supported. Pandas has weird and complex methods of converting an apply return. For example, a series apply function may return a dataframe, a series, a dict, a list, etc. All of these are converted in some specific way. Some cases may not be supported.
+- Not all the merging semantics of pandas are supported. Pandas has weird and complex methods of converting an apply
+return. For example, a series apply function may return a dataframe, a series, a dict, a list, etc. All of these are
+converted in some specific way. Some cases may not be supported.
+
+- Groupby apply functions are **much** slower than their serial variant currently. Still experimenting with how to make
+it faster. It looks correct, just 10-100x slower for some small examples. May be better as dataframe get bigger.
+
+- Using `n_cores = 1` will create a multiprocessing pool of just 1 core, so the code is parallel (thus not running on
+the main process), but may not yield much speed improvement, except for not blocking the main process. May be useful
+in some GUI apps.
 
-- Groupby apply functions are **much** slower than their serial variant currently. Still experimenting with how to make it faster. It looks correct, just 10-100x slower for some small examples. May be better as dataframe get bigger.
-
-- Using `n_cores = 1` will create a multiprocessing pool of just 1 core, so the code is parallel (thus not running on the main process), but may not yield much speed improvement, except for not blocking the main process. May be useful in some GUI apps.
+- You can use `parallelism=multithread` of `parallelism=multiprocess` (2nd is default) for all constructors. Using
+multiprocess requires the functions to be picklable though (lambda for example, must be global)
 
 That's all.
```

#### html2text {}

```diff
@@ -38,8 +38,11 @@
 a list, etc. All of these are converted in some specific way. Some cases may
 not be supported. - Groupby apply functions are **much** slower than their
 serial variant currently. Still experimenting with how to make it faster. It
 looks correct, just 10-100x slower for some small examples. May be better as
 dataframe get bigger. - Using `n_cores = 1` will create a multiprocessing pool
 of just 1 core, so the code is parallel (thus not running on the main process),
 but may not yield much speed improvement, except for not blocking the main
-process. May be useful in some GUI apps. That's all.
+process. May be useful in some GUI apps. - You can use
+`parallelism=multithread` of `parallelism=multiprocess` (2nd is default) for
+all constructors. Using multiprocess requires the functions to be picklable
+though (lambda for example, must be global) That's all.
```

### Comparing `pandas-parallel-apply-2.1/pandas_parallel_apply/data_frame_parallel.py` & `pandas-parallel-apply-2.2/pandas_parallel_apply/data_frame_parallel.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,45 +6,37 @@
     parallel => DataFrameParallel(df, n_cores)[col_name].apply(f)
 
 Apply on row
 Usage:
     standard => df.apply(f, axis=1)
     parallel => DataFrameParallel(df, n_cores).apply(f, axis=1)
 """
-from functools import partial
-from typing import Callable
 import pandas as pd
 
 from .series_parallel import SeriesParallel
 from .groupby_parallel import GroupByParallel
 from .utils import parallelize_dataframe
 
-
-def _apply_on_df(df: pd.DataFrame, f: Callable, pbar: bool = True) -> pd.Series:
-    """Apply a function on each row (all possible columns), returning a series"""
-    if pbar:
-        return df.progress_apply(f, axis=1)
-    return df.apply(f, axis=1)
-
 class DataFrameParallel:
     """DataFrameParallel implementation"""
-    def __init__(self, df: pd.DataFrame, n_cores: int, pbar: bool = True):
+    def __init__(self, df: pd.DataFrame, n_cores: int, pbar: bool = True, parallelism: str = "multiprocess"):
         self.df = df
         self.n_cores = n_cores
         self.pbar = pbar
+        self.parallelism = parallelism
 
     # pylint: disable=unused-argument
     def apply(self, func, axis, raw: bool = False, result_type = None, args=(), **kwargs):
         """Wrapper on top of regular df.apply(fn)"""
         assert axis == 1, "Only axis=1 is supported in parallel df apply"
-        return parallelize_dataframe(self.df, partial(_apply_on_df, f=func, pbar=self.pbar), self.n_cores)
+        return parallelize_dataframe(self.df, func, self.n_cores, self.pbar, self.parallelism, axis=axis, **kwargs)
 
     def groupby(self, *args, **kwargs):
         """Wrapper on top of regular df.groupby(col)"""
-        return GroupByParallel(self.df.groupby(*args, **kwargs), self.n_cores, self.pbar)
+        return GroupByParallel(self.df.groupby(*args, **kwargs), self.n_cores, self.pbar, self.parallelism)
 
     def __getitem__(self, x):
-        return SeriesParallel(self.df[x], self.n_cores, self.pbar)
+        return SeriesParallel(self.df[x], self.n_cores, self.pbar, self.parallelism)
 
     def __str__(self) -> str:
         f_str = f"[Parallel DataFrame - {self.n_cores} crores]\n" + self.df.__str__()
         return f_str
```

### Comparing `pandas-parallel-apply-2.1/pandas_parallel_apply/groupby_parallel.py` & `pandas-parallel-apply-2.2/pandas_parallel_apply/groupby_parallel.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 Usage:
     standard => df.groupby([cols]).apply(f)
     parallel => DataFrameParallel(df, n_cores).groupby([cols]).apply(f)
              => GroupByPrallel(df.groupby[cols], n_cores).apply(f)
 """
 from typing import Callable, List, Union
 from functools import partial
+from multiprocessing.pool import Pool, ThreadPool
 from pandas.core.groupby.generic import DataFrameGroupBy
 from pandas.core.indexes.multi import MultiIndex
 from tqdm import tqdm
 import pandas as pd
-from pathos.multiprocessing import ProcessingPool as Pool
 import numpy as np
 from .logger import logger
 from .utils import get_n_cores
 
 
 def _groupby_serial_func(data: List, func: Callable, pbar: bool = True) -> List:
     _range = tqdm(data) if pbar else data
@@ -45,25 +45,26 @@
             chunked_data.append(current_chunk)
             current_chunk = []
     if 0 < len(current_chunk) < chunk_size:
         chunked_data.append(current_chunk)
     assert n_cores == len(chunked_data)
     return key_data, chunked_data
 
-def _apply_on_groupby_parallel(df_grouped: DataFrameGroupBy, func: Callable, n_cores: int, pbar: bool = True,
-                              keep_original_indexes: bool = False) -> Union[pd.DataFrame, pd.Series]:
+def _apply_on_groupby_parallel(df_grouped: DataFrameGroupBy, func: Callable, n_cores: int, pbar: bool,
+                              keep_original_indexes: bool, parallelism: str) -> Union[pd.DataFrame, pd.Series]:
+    assert parallelism in ("multiprocess", "multithread"), parallelism
     n_cores = get_n_cores(n_cores, df_grouped)
     if n_cores == 0:
         logger.info("n_cores is set to 0, returning serial apply.")
         return df_grouped.apply(func)
 
     key_data, chunked_data = _chunk_df(df_grouped, n_cores)
 
     # Run the multi-process job
-    pool = Pool(n_cores)
+    pool = Pool(n_cores) if parallelism == "multiprocess" else ThreadPool(n_cores)
     pool_res = pool.map(partial(_groupby_serial_func, func=func, pbar=pbar), chunked_data)
 
     # Concatenate the result to preserve the original result of a regular groupby pandas code.
     concat_res = []
     for i in range(len(pool_res)):
         concat_res.extend(pool_res[i])
 
@@ -84,16 +85,18 @@
     res.index.name = df_grouped.keys
     return res
 
 
 class GroupByParallel:
     """GroupByParallel implementation"""
     def __init__(self, df_grouped: DataFrameGroupBy, n_cores: int, pbar: bool = True,
-                 keep_original_indexes: bool = False):
+                 keep_original_indexes: bool = False, parallelism: str = "multiprocess"):
         self.df_grouped = df_grouped
         self.n_cores = n_cores
         self.pbar = pbar
         self.keep_original_indexes = keep_original_indexes
+        self.parallelism = parallelism
 
     def apply(self, func: Callable):
         """Wrapper on top of regular df.groupby(col).apply(fn)"""
-        return _apply_on_groupby_parallel(self.df_grouped, func, self.n_cores, self.pbar, self.keep_original_indexes)
+        return _apply_on_groupby_parallel(self.df_grouped, func, self.n_cores, self.pbar,
+                                          self.keep_original_indexes, self.parallelism)
```

### Comparing `pandas-parallel-apply-2.1/pandas_parallel_apply/logger.py` & `pandas-parallel-apply-2.2/pandas_parallel_apply/logger.py`

 * *Files identical despite different names*

### Comparing `pandas-parallel-apply-2.1/pandas_parallel_apply/series_parallel.py` & `pandas-parallel-apply-2.2/pandas_parallel_apply/series_parallel.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,30 +2,22 @@
 Apply on series
 Usage:
     standard => series.apply(f)
     parallel => SeriesParallel(series, n_cores).apply(f)
              => SeriesParallel(df[col], n_cores).apply(f)
 """
 from typing import Callable
-from functools import partial
 import pandas as pd
 
 from .utils import parallelize_dataframe
 
-
-def _apply_on_series(series: pd.Series, f: Callable, pbar: bool = True) -> pd.Series:
-    """Returns progress_apply or simple apply based on pbar"""
-    if pbar:
-        return series.progress_apply(f)
-    return series.apply(f)
-
-
 class SeriesParallel:
     """SeriesParallel implementation"""
-    def __init__(self, series: pd.Series, n_cores: int, pbar: bool = True):
+    def __init__(self, series: pd.Series, n_cores: int, pbar: bool = True, parallelism: str = "multiprocess"):
         self.series = series
         self.n_cores = n_cores
         self.pbar = pbar
+        self.parallelism = parallelism
 
     def apply(self, func: Callable) -> pd.Series:
         """Wrapper on top of regular ser.apply(fn)"""
-        return parallelize_dataframe(self.series, partial(_apply_on_series, f=func, pbar=self.pbar), self.n_cores)
+        return parallelize_dataframe(self.series, func, self.n_cores, self.pbar, self.parallelism)
```

### Comparing `pandas-parallel-apply-2.1/pandas_parallel_apply/utils.py` & `pandas-parallel-apply-2.2/pandas_parallel_apply/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """General module for parallelizing a dataframe apply function on a column (series) or entire row"""
 
 from typing import Callable, Union
+from multiprocessing import cpu_count, current_process
+from multiprocessing.pool import Pool, ThreadPool
+from threading import current_thread
+from functools import partial
 import numpy as np
 import pandas as pd
 from tqdm import tqdm
-from pathos.multiprocessing import ProcessingPool as Pool, cpu_count
 
 from .logger import logger
 
-tqdm.pandas()
-
 def get_n_cores(n_cores: int, df: Union[pd.DataFrame, pd.Series]) -> int:
     """
     Returns the actual n_cores used for the parallel operation. cpu_count() represents the total amount of phyisical
     cores. Possible cases:
     - n_cores < -1: will throw an AssertionError
     - n_cores = -1: will return cpu_count() - 1
     - n_cores in [0, cpu_count()]: will return the number as is
@@ -26,25 +27,44 @@
     if n_cores > cpu_count():
         logger.warning(f"n_cores is greater than the number of physical cores: {n_cores} vs {cpu_count()}")
     if n_cores > len(df):
         logger.warning(f"n_cores is greater than the length of the df, return that: {n_cores} vs {len(df)}")
         n_cores = len(df)
     return n_cores
 
-def parallelize_dataframe(df: Union[pd.DataFrame, pd.Series], func: Callable, n_cores: int) -> pd.DataFrame:
+# pylint: disable=protected-access
+def _worker_fn(df: pd.DataFrame, fn: Callable, pbar: bool, kwargs: dict):
+    """worker_fn: calls df.progress_apply or df.apply. For pbar, will use position based on thread/process index"""
+    if not pbar:
+        return df.apply(fn, **kwargs)
+
+    if len(current_process()._identity) == 0:
+        position = int(current_thread().name.split(" ")[0].split("Thread-")[1])
+        desc = f"Thread-{position}"
+    else:
+        position = current_process()._identity[0] - 1
+        desc = f"Process-{position}"
+
+    tqdm.pandas(position=position, desc=desc)
+    return df.progress_apply(fn, **kwargs)
+
+def parallelize_dataframe(df: Union[pd.DataFrame, pd.Series], func: Callable, n_cores: int,
+                          pbar: bool, parallelism: str, **kwargs) -> pd.DataFrame:
     """Function used to split a dataframe in n sub dataframes, based on the number of cores we want to use."""
+    assert parallelism in ("multiprocess", "multithread"), parallelism
     n_cores = get_n_cores(n_cores, df)
     if n_cores == 0:
         logger.debug("n_cores is set to 0, returning serial function")
-        return func(df)
+        return df.apply(func, **kwargs)
     logger.debug(f"Parallelizing apply on df (rows: {len(df)}) with {n_cores} cores")
 
     df_split = np.array_split(df, n_cores)
-    pool = Pool(n_cores)
-    pool_res = pool.map(func, df_split)
+    pool_fn = partial(_worker_fn, fn=func, pbar=pbar, kwargs=kwargs)
+    pool = Pool(n_cores) if parallelism == "multiprocess" else ThreadPool(n_cores)
+    pool_res = pool.map(pool_fn, df_split)
 
     # This should use less memory than pd.concat(pool_res)
     final_df = pool_res[0]
     for res_df in pool_res[1: ]:
         final_df = pd.concat([final_df, res_df], copy=False)
         del res_df
     return final_df
```

### Comparing `pandas-parallel-apply-2.1/pandas_parallel_apply.egg-info/PKG-INFO` & `pandas-parallel-apply-2.2/pandas_parallel_apply.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-parallel-apply
-Version: 2.1
+Version: 2.2
 Summary: Wrapper for df and df[col].apply parallelized
 Home-page: https://gitlab.com/meehai/pandas-parallel-apply
 License: WTFPL
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -66,33 +66,41 @@
 `df.apply(fn, axis=0)` is not because it may require rows that are on other workers.
 
 It is assumed that each row is processed in similar time, so the N/K chunks will finishe more or less at the same time.
 
 ### Future Improvement
 
 Not supported but may be interesting: define also a number of chunks (C>K), so the df is actually split in N/C chunks,
-and theses are passed using a round-robin approach to the K processes. Right now, C=K, so whenever one process finishes,
-it will not be assigned any more work.
+and theses are passed using a round-robin approach to the K processes. Right now, C=K, so whenever one process
+finishes, it will not be assigned any more work.
 
 ## n_cores semantics
 - `n_cores < -1` -> throws an error
 - `n_cores == -1` -> uses `cpu_count()` - 1 cores
 - `n_cores == 0` -> uses serial/standard pandas functions
 - `n_cores == 1` -> spawns a single process alongside the main one
 - `n_cores > 1` -> spanws N processes and chunks the df
 - `n_cores > cpu_cpunt()` -> throws an warning
 - `n_cores > len(df)` -> limits to `len(df)`
 
-On CPU-bound tasks (calculations), `n_cores = -1` is likely to be fastest. On network-bound operations (e.g., where threads may invoke network calls),
-using a very high `n_cores` value may be beneficial.
+On CPU-bound tasks (calculations), `n_cores = -1` is likely to be fastest. On network-bound operations (e.g., where
+threads may invoke network calls), using a very high `n_cores` value may be beneficial.
 
 ## Disclaimers
 
 - This is an experimental repository. It may lead to unexpected behaviour.
 
-- Not all the merging semantics of pandas are supported. Pandas has weird and complex methods of converting an apply return. For example, a series apply function may return a dataframe, a series, a dict, a list, etc. All of these are converted in some specific way. Some cases may not be supported.
+- Not all the merging semantics of pandas are supported. Pandas has weird and complex methods of converting an apply
+return. For example, a series apply function may return a dataframe, a series, a dict, a list, etc. All of these are
+converted in some specific way. Some cases may not be supported.
+
+- Groupby apply functions are **much** slower than their serial variant currently. Still experimenting with how to make
+it faster. It looks correct, just 10-100x slower for some small examples. May be better as dataframe get bigger.
+
+- Using `n_cores = 1` will create a multiprocessing pool of just 1 core, so the code is parallel (thus not running on
+the main process), but may not yield much speed improvement, except for not blocking the main process. May be useful
+in some GUI apps.
 
-- Groupby apply functions are **much** slower than their serial variant currently. Still experimenting with how to make it faster. It looks correct, just 10-100x slower for some small examples. May be better as dataframe get bigger.
-
-- Using `n_cores = 1` will create a multiprocessing pool of just 1 core, so the code is parallel (thus not running on the main process), but may not yield much speed improvement, except for not blocking the main process. May be useful in some GUI apps.
+- You can use `parallelism=multithread` of `parallelism=multiprocess` (2nd is default) for all constructors. Using
+multiprocess requires the functions to be picklable though (lambda for example, must be global)
 
 That's all.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pandas-parallel-apply Version: 2.1 Summary: Wrapper
+Metadata-Version: 2.1 Name: pandas-parallel-apply Version: 2.2 Summary: Wrapper
 for df and df[col].apply parallelized Home-page: https://gitlab.com/meehai/
 pandas-parallel-apply License: WTFPL Requires-Python: >=3.8 Description-
 Content-Type: text/markdown License-File: LICENSE # pandas-parallel-apply
                         [License] [PyPi_Latest_Release]
 Parallel wrappers for `df.apply(fn)`, `df[col].apply(fn)`, `series.apply(fn)`,
 and `df.groupby([cols]).apply(fn)`, with tqdm progress bars included. ##
 Installation `pip install pandas-parallel-apply` Import with: ```python from
@@ -41,8 +41,11 @@
 a list, etc. All of these are converted in some specific way. Some cases may
 not be supported. - Groupby apply functions are **much** slower than their
 serial variant currently. Still experimenting with how to make it faster. It
 looks correct, just 10-100x slower for some small examples. May be better as
 dataframe get bigger. - Using `n_cores = 1` will create a multiprocessing pool
 of just 1 core, so the code is parallel (thus not running on the main process),
 but may not yield much speed improvement, except for not blocking the main
-process. May be useful in some GUI apps. That's all.
+process. May be useful in some GUI apps. - You can use
+`parallelism=multithread` of `parallelism=multiprocess` (2nd is default) for
+all constructors. Using multiprocess requires the functions to be picklable
+though (lambda for example, must be global) That's all.
```

### Comparing `pandas-parallel-apply-2.1/pandas_parallel_apply.egg-info/SOURCES.txt` & `pandas-parallel-apply-2.2/pandas_parallel_apply.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pandas-parallel-apply-2.1/setup.py` & `pandas-parallel-apply-2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
                 print("Dependency to a git repository should have the format:")
                 print("git+ssh://git@github.com/xxxxx/xxxxxx#egg=package_name")
         else:
             required.append(line)
     return required, dependency_links
 
 name = "pandas-parallel-apply"
-version = "2.1"
+version = "2.2"
 description = "Wrapper for df and df[col].apply parallelized"
 url = "https://gitlab.com/meehai/pandas-parallel-apply"
 
 loc = path.abspath(path.dirname(__file__))
 with open(f"{loc}/README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
```

### Comparing `pandas-parallel-apply-2.1/test/test_apply_df.py` & `pandas-parallel-apply-2.2/test/test_apply_df.py`

 * *Files identical despite different names*

### Comparing `pandas-parallel-apply-2.1/test/test_apply_df_groupby.py` & `pandas-parallel-apply-2.2/test/test_apply_df_groupby.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,32 +7,46 @@
 data_static = {
     "A": [1,1,2,3,5,3],
     "B": ["hello", "darkness", "hi", "dafuq", "who", "asdf"],
     1: [(1,2), (3,4), "yolo", 1, 2, 3]
 }
 
 N = 10000000
-data_random = {"A": np.random.randint(0, 10, size=(N, )), "B": np.arange(N),
-    "C": [chr(ord("A") + np.random.randint(0, 26)) for _ in range(N)] }
+data_random = {
+    "A": np.random.randint(0, 10, size=(N, )),
+    "B": np.arange(N),
+    "C": [chr(ord("A") + np.random.randint(0, 26)) for _ in range(N)]
+}
+
+# functions must be global, not lambdas
+def global_fn(df):
+    return df.iloc[0]
 
 def test_one_col_return_series():
     df = pd.DataFrame(data_random)
     Y = df.groupby("A").apply(len)
     K = GroupByParallel(df.groupby("A"), n_cores=4, pbar=False).apply(len)
     P = DataFrameParallel(df, n_cores=4, pbar=False).groupby("A").apply(len)
 
     assert np.allclose(Y.values, K.values)
     assert np.allclose(Y.values, P.values)
 
 def test_one_col_return_df():
     df = pd.DataFrame(data_random)
-    f = lambda df: df.iloc[0]
-    Y = df.groupby("A").apply(f)
-    K = GroupByParallel(df.groupby("A"), n_cores=4, pbar=False).apply(f)
-    P = DataFrameParallel(df, n_cores=4, pbar=False).groupby("A").apply(f)
+    Y = df.groupby("A").apply(global_fn)
+    K = GroupByParallel(df.groupby("A"), n_cores=4, pbar=False).apply(global_fn)
+    P = DataFrameParallel(df, n_cores=4, pbar=False).groupby("A").apply(global_fn)
+    assert (Y != K).sum().sum() == 0
+    assert (Y != P).sum().sum() == 0
+
+def test_one_col_return_df_multithread():
+    df = pd.DataFrame(data_random)
+    Y = df.groupby("A").apply(global_fn)
+    K = GroupByParallel(df.groupby("A"), n_cores=4, pbar=False, parallelism="multithread").apply(global_fn)
+    P = DataFrameParallel(df, n_cores=4, pbar=False, parallelism="multithread").groupby("A").apply(global_fn)
     assert (Y != K).sum().sum() == 0
     assert (Y != P).sum().sum() == 0
 
 def run_one_col_return_tricky_df_no_index(df):
     def f(df):
         np.random.seed(42)
         N = np.random.randint(1, len(df) + 1)
```

### Comparing `pandas-parallel-apply-2.1/test/test_utils.py` & `pandas-parallel-apply-2.2/test/test_utils.py`

 * *Files identical despite different names*

