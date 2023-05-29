# Comparing `tmp/pipd-0.0.3.tar.gz` & `tmp/pipd-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipd-0.0.3.tar", last modified: Mon May 29 11:20:38 2023, max compression
+gzip compressed data, was "pipd-0.0.4.tar", last modified: Mon May 29 13:19:32 2023, max compression
```

## Comparing `pipd-0.0.3.tar` & `pipd-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 11:20:38.991171 pipd-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-29 11:20:38.991171 pipd-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-29 11:20:25.000000 pipd-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 11:20:38.991171 pipd-0.0.3/pipd/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-29 11:20:25.000000 pipd-0.0.3/pipd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7501 2023-05-29 11:20:25.000000 pipd-0.0.3/pipd/pipd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 11:20:38.991171 pipd-0.0.3/pipd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-29 11:20:38.000000 pipd-0.0.3/pipd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-29 11:20:38.000000 pipd-0.0.3/pipd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 11:20:38.000000 pipd-0.0.3/pipd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-29 11:20:38.000000 pipd-0.0.3/pipd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 11:20:38.991171 pipd-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-29 11:20:25.000000 pipd-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:19:32.677392 pipd-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-29 13:19:32.677392 pipd-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-05-29 13:19:21.000000 pipd-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:19:32.677392 pipd-0.0.4/pipd/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-29 13:19:21.000000 pipd-0.0.4/pipd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-05-29 13:19:21.000000 pipd-0.0.4/pipd/pipd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:19:32.677392 pipd-0.0.4/pipd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-29 13:19:32.000000 pipd-0.0.4/pipd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-29 13:19:32.000000 pipd-0.0.4/pipd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 13:19:32.000000 pipd-0.0.4/pipd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-29 13:19:32.000000 pipd-0.0.4/pipd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 13:19:32.677392 pipd-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-29 13:19:21.000000 pipd-0.0.4/setup.py
```

### Comparing `pipd-0.0.3/pipd/pipd.py` & `pipd-0.0.4/pipd/pipd.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         def method(*args, **kwargs):
             return self.functions[name](*args, **kwargs)(self.items)
 
         return method
 
     def __call__(self):
         # Exhaust iterator
-        for _ in self.items:
+        for _ in self:
             pass
 
     @classmethod
     def add_function(cls, name: str, function: Callable):
         cls.functions[name] = function
 
 
@@ -61,63 +61,14 @@
         # If name is None we assume the function is named _name and remove the _
         name=fn.__name__[1:] if name is None else name,
         function=fn_curried,
     )
     return fn_curried
 
 
-def _batch(items: Iterable[T], size: int) -> Iterator[List[T]]:
-    batch = []
-    for item in items:
-        batch.append(item)
-        if len(batch) == size:
-            yield batch
-            batch = []
-    if batch:
-        yield batch
-
-
-batch = as_pipe(_batch)
-
-
-def _unbatch(items: Iterable[Sequence[T]]) -> Iterator[T]:
-    for b in items:
-        for item in b:
-            yield item
-
-
-unbatch = as_pipe(_unbatch)
-
-
-def pick(items: List[T], random: bool = False) -> T:
-    idx = randint(0, len(items) - 1) if random else 0
-    return items.pop(idx)
-
-
-def _buffer(
-    items: Iterator[T], size: int, start: int = 0, shuffle: bool = False
-) -> Iterator[T]:
-    buffer = []
-    for item in items:
-        buffer.append(item)
-        if len(buffer) < size:
-            try:
-                buffer.append(next(items))
-            except StopIteration:
-                pass
-        if len(buffer) >= start:
-            yield pick(buffer, random=shuffle)
-    # Empty buffer at the end
-    while len(buffer) > 0:
-        yield pick(buffer)
-
-
-buffer = as_pipe(_buffer)
-
-
 def _map(
     items: Iterable[T],
     fn: Callable[[T], U],
     num_workers: int = 0,
     buffer: Optional[int] = None,
     mode: str = "multithread",
     handler: Callable = log_and_continue,
@@ -155,54 +106,112 @@
             except Exception as e:
                 handler(e)
 
 
 map = as_pipe(_map)
 
 
-def _filter(items: Iterable[T], fn: Callable[[T], bool]) -> Iterator[T]:
-    for item in items:
-        if fn(item):
+def _filter(
+    items: Iterable[T], fn: Callable[[T], bool], *args, **kwargs
+) -> Iterator[T]:
+    for item, keep in _map(items, lambda x: (x, fn(x)), *args, **kwargs):
+        if keep:
             yield item
 
 
 filter = as_pipe(_filter)
 
 
-def _unpipe(
+def _side(
     items: Iterable[T],
     fn: Callable[[T], U],
-    num_workers: int = 1,
+    num_workers: int = 0,
     mode: str = "multithread",
+    handler: Callable = log_and_continue,
 ) -> Iterator[T]:
     assert mode in ["multithread", "multiprocess"]
+
+    if num_workers == 0:
+        for item in items:
+            try:
+                fn(item)
+            except Exception as e:
+                handler(e)
+            yield item
+        return
+
     executors = dict(multithread=ThreadPoolExecutor, multiprocess=ProcessPoolExecutor)
     with executors[mode](max_workers=num_workers) as executor:
         for item in items:
             executor.submit(fn, item)
             yield item
 
 
-unpipe = as_pipe(_unpipe)
+side = as_pipe(_side)
+
+
+def _batch(items: Iterable[T], size: int) -> Iterator[List[T]]:
+    batch = []
+    for item in items:
+        batch.append(item)
+        if len(batch) == size:
+            yield batch
+            batch = []
+    if batch:
+        yield batch
+
+
+batch = as_pipe(_batch)
+
+
+def _unbatch(items: Iterable[Sequence[T]]) -> Iterator[T]:
+    for b in items:
+        for item in b:
+            yield item
+
+
+unbatch = as_pipe(_unbatch)
+
+
+def pick(items: List[T], random: bool = False) -> T:
+    idx = randint(0, len(items) - 1) if random else 0
+    return items.pop(idx)
+
+
+def _shuffle(items: Iterator[T], size: int, start: Optional[int] = None) -> Iterator[T]:
+    start = start or size
+    buffer = []
+    for item in items:
+        buffer.append(item)
+        if len(buffer) < size:
+            try:
+                buffer.append(next(items))
+            except StopIteration:
+                pass
+        if len(buffer) >= start:
+            yield pick(buffer, random=True)
+    # Empty buffer at the end
+    while len(buffer) > 0:
+        yield pick(buffer)
+
+
+shuffle = as_pipe(_shuffle)
 
 
 def _limit(items: Iterable[T], limit: int = 10**100) -> Iterator[T]:
     for count, item in enumerate(items):
         if count < limit:
             yield item
 
 
 limit = as_pipe(_limit)
 
 
-def _log(items: Iterable[T], limit: int = 10**100) -> Iterator[T]:
-    for count, item in enumerate(items):
-        if count < limit:
-            print(item)
-        yield item
+def _log(items: Iterable[T], fn: Callable[[T], None] = print) -> Iterator[T]:
+    return _side(items, fn)
 
 
 log = as_pipe(_log)
 
 
 def _tqdm(items: Iterable[T], *args, **kwargs) -> Iterator[T]:
     try:
@@ -213,17 +222,15 @@
         yield item
 
 
 tqdm = as_pipe(_tqdm)
 
 
 def _sleep(items: Iterable[T], seconds: float) -> Iterator[T]:
-    for item in items:
-        time.sleep(seconds)
-        yield item
+    return _side(items, lambda _: time.sleep(seconds))
 
 
 sleep = as_pipe(_sleep)
 
 
 def watchdir(
     path: str, changes: Sequence[int] = [1]  # default to watchgod.Change.added == 1
```

