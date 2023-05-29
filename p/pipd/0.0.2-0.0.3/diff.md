# Comparing `tmp/pipd-0.0.2.tar.gz` & `tmp/pipd-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipd-0.0.2.tar", last modified: Mon May 29 09:37:33 2023, max compression
+gzip compressed data, was "pipd-0.0.3.tar", last modified: Mon May 29 11:20:38 2023, max compression
```

## Comparing `pipd-0.0.2.tar` & `pipd-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:37:33.956477 pipd-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-29 09:37:33.956477 pipd-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-29 09:37:22.000000 pipd-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:37:33.952477 pipd-0.0.2/pipd/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-29 09:37:22.000000 pipd-0.0.2/pipd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-05-29 09:37:22.000000 pipd-0.0.2/pipd/pipd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:37:33.956477 pipd-0.0.2/pipd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-29 09:37:33.000000 pipd-0.0.2/pipd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-29 09:37:33.000000 pipd-0.0.2/pipd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 09:37:33.000000 pipd-0.0.2/pipd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-29 09:37:33.000000 pipd-0.0.2/pipd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 09:37:33.956477 pipd-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-29 09:37:22.000000 pipd-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 11:20:38.991171 pipd-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-29 11:20:38.991171 pipd-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-29 11:20:25.000000 pipd-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 11:20:38.991171 pipd-0.0.3/pipd/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-29 11:20:25.000000 pipd-0.0.3/pipd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7501 2023-05-29 11:20:25.000000 pipd-0.0.3/pipd/pipd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 11:20:38.991171 pipd-0.0.3/pipd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-29 11:20:38.000000 pipd-0.0.3/pipd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-29 11:20:38.000000 pipd-0.0.3/pipd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 11:20:38.000000 pipd-0.0.3/pipd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-29 11:20:38.000000 pipd-0.0.3/pipd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 11:20:38.991171 pipd-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-29 11:20:25.000000 pipd-0.0.3/setup.py
```

### Comparing `pipd-0.0.2/pipd/pipd.py` & `pipd-0.0.3/pipd/pipd.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,65 +6,90 @@
 from concurrent.futures import (
     FIRST_COMPLETED,
     ProcessPoolExecutor,
     ThreadPoolExecutor,
     wait,
 )
 from random import randint
-from typing import Callable, Iterable, Iterator, List, Optional, Sequence, TypeVar
+from typing import Callable, Dict, Iterable, Iterator, List, Optional, Sequence, TypeVar
 
 T = TypeVar("T")
 U = TypeVar("U")
 
 
 def log_and_continue(exception: Exception):
     print(repr(exception))
 
 
-def curry(fn: Callable) -> Callable:
-    # fn(a0, a1, a2) => curry(fn)(a1, a2)(a0)
-    def fn_curried(*args, **kwargs):
-        def _fn(arg0):
-            return fn(arg0, *args, **kwargs)
+class Pipe:
+    functions: Dict[str, Callable] = {}
 
-        return _fn
+    def __init__(self, *items):
+        if len(items) == 1 and isinstance(items[0], Iterable):
+            items = items[0]
+        self.items = iter(items)
 
-    return fn_curried
+    def __iter__(self):
+        return self
+
+    def __next__(self):
+        return next(self.items)
+
+    def __getattr__(self, name):
+        def method(*args, **kwargs):
+            return self.functions[name](*args, **kwargs)(self.items)
+
+        return method
 
+    def __call__(self):
+        # Exhaust iterator
+        for _ in self.items:
+            pass
 
-def _pipe(items: Iterable[T], *fns: Callable) -> Iterable[U]:
-    for fn in fns:
-        items = fn(items)
-    return items  # type: ignore
+    @classmethod
+    def add_function(cls, name: str, function: Callable):
+        cls.functions[name] = function
 
 
-pipe = curry(_pipe)
+def as_pipe(fn: Callable, name: Optional[str] = None) -> Callable:
+    def fn_curried(*args, **kwargs):
+        def _fn(items: Optional[Iterable[T]] = None):
+            return Pipe(fn(items, *args, **kwargs))
+
+        return _fn
+
+    Pipe.add_function(
+        # If name is None we assume the function is named _name and remove the _
+        name=fn.__name__[1:] if name is None else name,
+        function=fn_curried,
+    )
+    return fn_curried
 
 
 def _batch(items: Iterable[T], size: int) -> Iterator[List[T]]:
     batch = []
     for item in items:
         batch.append(item)
         if len(batch) == size:
             yield batch
             batch = []
     if batch:
         yield batch
 
 
-batch = curry(_batch)
+batch = as_pipe(_batch)
 
 
 def _unbatch(items: Iterable[Sequence[T]]) -> Iterator[T]:
     for b in items:
         for item in b:
             yield item
 
 
-unbatch = curry(_unbatch)
+unbatch = as_pipe(_unbatch)
 
 
 def pick(items: List[T], random: bool = False) -> T:
     idx = randint(0, len(items) - 1) if random else 0
     return items.pop(idx)
 
 
@@ -82,15 +107,15 @@
         if len(buffer) >= start:
             yield pick(buffer, random=shuffle)
     # Empty buffer at the end
     while len(buffer) > 0:
         yield pick(buffer)
 
 
-buffer = curry(_buffer)
+buffer = as_pipe(_buffer)
 
 
 def _map(
     items: Iterable[T],
     fn: Callable[[T], U],
     num_workers: int = 0,
     buffer: Optional[int] = None,
@@ -127,24 +152,24 @@
         for future in futures:
             try:
                 yield future.result()
             except Exception as e:
                 handler(e)
 
 
-map = curry(_map)
+map = as_pipe(_map)
 
 
 def _filter(items: Iterable[T], fn: Callable[[T], bool]) -> Iterator[T]:
     for item in items:
         if fn(item):
             yield item
 
 
-filter = curry(_filter)
+filter = as_pipe(_filter)
 
 
 def _unpipe(
     items: Iterable[T],
     fn: Callable[[T], U],
     num_workers: int = 1,
     mode: str = "multithread",
@@ -153,55 +178,55 @@
     executors = dict(multithread=ThreadPoolExecutor, multiprocess=ProcessPoolExecutor)
     with executors[mode](max_workers=num_workers) as executor:
         for item in items:
             executor.submit(fn, item)
             yield item
 
 
-unpipe = curry(_unpipe)
+unpipe = as_pipe(_unpipe)
 
 
 def _limit(items: Iterable[T], limit: int = 10**100) -> Iterator[T]:
     for count, item in enumerate(items):
         if count < limit:
             yield item
 
 
-limit = curry(_limit)
+limit = as_pipe(_limit)
 
 
 def _log(items: Iterable[T], limit: int = 10**100) -> Iterator[T]:
     for count, item in enumerate(items):
         if count < limit:
             print(item)
         yield item
 
 
-log = curry(_log)
+log = as_pipe(_log)
 
 
 def _tqdm(items: Iterable[T], *args, **kwargs) -> Iterator[T]:
     try:
         from tqdm import tqdm as progressbar
     except ImportError:
         raise ImportError("tqdm is required to use tqdm")
     for item in progressbar(items, *args, **kwargs):
         yield item
 
 
-tqdm = curry(_tqdm)
+tqdm = as_pipe(_tqdm)
 
 
 def _sleep(items: Iterable[T], seconds: float) -> Iterator[T]:
     for item in items:
         time.sleep(seconds)
         yield item
 
 
-sleep = curry(_sleep)
+sleep = as_pipe(_sleep)
 
 
 def watchdir(
     path: str, changes: Sequence[int] = [1]  # default to watchgod.Change.added == 1
 ) -> Iterator[str]:
     try:
         from watchgod import awatch
@@ -211,42 +236,58 @@
     async_generator = awatch(path)
     while True:
         for change, filepath in loop.run_until_complete(async_generator.__anext__()):
             if change in changes:
                 yield filepath
 
 
-def readf(filepath: str, watch: bool = False) -> Iterator[str]:
+def _readf(_, filepath: str, watch: bool = False) -> Iterator[str]:
     files = glob.glob(filepath)
     for file in files:
         yield file
     if watch:
         yield from watchdir(os.path.dirname(filepath))
 
 
-def readl(filepath: str, watch: bool = False) -> Iterator[str]:
+readf = as_pipe(_readf)
+
+
+class Readf(Pipe):
+    def __init__(self, *args, **kwargs):
+        super().__init__(readf(*args, **kwargs)())
+
+
+def _readl(_, filepath: str, watch: bool = False) -> Iterator[str]:
     with open(filepath, "r") as file:
         while True:
             line = file.readline()
             if line:
                 yield line.strip()
             elif watch:
                 select.select([file], [], [])  # Wait until there is more data to read
             else:
                 break
 
 
+readl = as_pipe(_readl)
+
+
+class Readl(Pipe):
+    def __init__(self, *args, **kwargs):
+        super().__init__(readl(*args, **kwargs)())
+
+
 def _writel(items: Iterable[str], filepath: str) -> Iterator[str]:
     with open(filepath, "w") as f:
         for item in items:
             f.write(item + "\n")
             yield item
 
 
-writel = curry(_writel)
+writel = as_pipe(_writel)
 
 
 def _filter_cached(
     items: Iterable[T],
     filepath: str,
     key: Optional[Callable] = None,
 ) -> Iterator[T]:
@@ -256,13 +297,8 @@
             value = key(item) if key is not None else item
             if value not in cache:
                 cache.add(value)
                 file.write(value + "\n")
                 yield item
 
 
-filter_cached = curry(_filter_cached)
-
-
-def run(items: Iterable[T]) -> None:
-    for item in items:
-        pass
+filter_cached = as_pipe(_filter_cached)
```

