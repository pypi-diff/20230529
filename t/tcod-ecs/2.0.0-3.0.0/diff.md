# Comparing `tmp/tcod_ecs-2.0.0.tar.gz` & `tmp/tcod_ecs-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcod_ecs-2.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "tcod_ecs-3.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `tcod_ecs-2.0.0.tar` & `tcod_ecs-3.0.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1079 2023-05-26 10:42:53.718165 tcod_ecs-2.0.0/LICENSE
--rw-r--r--   0        0        0     8626 2023-05-26 10:42:53.718165 tcod_ecs-2.0.0/README.md
--rw-r--r--   0        0        0     3688 2023-05-26 10:42:53.722166 tcod_ecs-2.0.0/pyproject.toml
--rw-r--r--   0        0        0    35712 2023-05-26 10:42:53.722166 tcod_ecs-2.0.0/tcod/ecs/__init__.py
--rw-r--r--   0        0        0      160 2023-05-26 10:43:03.010447 tcod_ecs-2.0.0/tcod/ecs/_version.py
--rw-r--r--   0        0        0        0 2023-05-26 10:42:53.722166 tcod_ecs-2.0.0/tcod/ecs/py.typed
--rw-r--r--   0        0        0     9821 1970-01-01 00:00:00.000000 tcod_ecs-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-05-29 16:49:45.307406 tcod_ecs-3.0.0/LICENSE
+-rw-r--r--   0        0        0     8627 2023-05-29 16:49:45.307406 tcod_ecs-3.0.0/README.md
+-rw-r--r--   0        0        0     3688 2023-05-29 16:49:45.307406 tcod_ecs-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0    35405 2023-05-29 16:49:45.307406 tcod_ecs-3.0.0/tcod/ecs/__init__.py
+-rw-r--r--   0        0        0      160 2023-05-29 16:49:53.175620 tcod_ecs-3.0.0/tcod/ecs/_version.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:49:45.307406 tcod_ecs-3.0.0/tcod/ecs/py.typed
+-rw-r--r--   0        0        0     9822 1970-01-01 00:00:00.000000 tcod_ecs-3.0.0/PKG-INFO
```

### Comparing `tcod_ecs-2.0.0/LICENSE` & `tcod_ecs-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tcod_ecs-2.0.0/README.md` & `tcod_ecs-3.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # About
 
-[![PyPI](https://img.shields.io/pypi/v/tcod-ec)](https://pypi.org/project/tcod-ecs/)
+[![PyPI](https://img.shields.io/pypi/v/tcod-ecs)](https://pypi.org/project/tcod-ecs/)
 [![PyPI - License](https://img.shields.io/pypi/l/tcod-ecs)](https://github.com/HexDecimal/python-tcod-ecs/blob/main/LICENSE)
 [![Documentation Status](https://readthedocs.org/projects/python-tcod-ecs/badge/?version=latest)](https://python-tcod-ecs.readthedocs.io)
 [![codecov](https://codecov.io/gh/HexDecimal/python-tcod-ecs/branch/main/graph/badge.svg?token=4Ak5QpTLZB)](https://codecov.io/gh/HexDecimal/python-tcod-ecs)
 
 This is an [Entity-component-system](https://en.wikipedia.org/wiki/Entity_component_system) implemented in Python.
 See the [ECS FAQ](https://github.com/SanderMertens/ecs-faq) for more info.
```

### Comparing `tcod_ecs-2.0.0/pyproject.toml` & `tcod_ecs-3.0.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 [tool.pytest.ini_options]
 minversion = "6.0"
 required_plugins = ["pytest-cov>=4.0.0", "pytest-benchmark>=4.0.0"]
 addopts = "--doctest-modules --cov=tcod --cov-report=term-missing --doctest-glob=*.md"
 testpaths = ["."]
 
 [tool.coverage.report] # https://coverage.readthedocs.io/en/latest/config.html
-exclude_lines = ['$\s*\.\.\.', "if TYPE_CHECKING:"]
+exclude_lines = ['^\s*\.\.\.', "if TYPE_CHECKING:"]
 
 [tool.ruff]
 # https://beta.ruff.rs/docs/rules/
 select = [
     "C90", # mccabe
     "E",   # pycodestyle
     "W",   # pycodestyle
```

### Comparing `tcod_ecs-2.0.0/tcod/ecs/__init__.py` & `tcod_ecs-3.0.0/tcod/ecs/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -234,15 +234,14 @@
         return f"<{' '.join(items)}>"
 
     def __reduce__(self) -> tuple[type[Entity], tuple[World, object]]:
         """Pickle this Entity.
 
         Note that any pickled entity will include the world it belongs to and all the entities of that world.
         """
-        # Note: This was added after version 1.0.0, objects pickled in <=1.0.0 will call __setstate__.
         return self.__class__, (self.world, self.uid)
 
     def _force_remap(self, new_uid: object) -> None:
         """Remap this Entity to a new uid, both and old and new uid's will use this entity."""
         _entity_table[self.world][new_uid] = self
         self.uid = new_uid  # type: ignore[misc]
 
@@ -310,14 +309,34 @@
         return len(self.entity.world._components_by_entity.get(self.entity, ()))
 
     def update_values(self, values: Iterable[object]) -> None:
         """Add or overwrite multiple components inplace, deriving the keys from the values."""
         for value in values:
             self.set(value)
 
+    def by_name_type(self, name_type: type[_T1], component_type: type[_T2]) -> Iterator[tuple[_T1, type[_T2]]]:
+        """Iterate over all of an entities component keys with a specific (name_type, component_type) combination.
+
+        .. versionadded:: 3.0.0
+
+        Example::
+
+            >>> entity.components["A", int] = 1
+            >>> entity.components["B", int] = 2
+            >>> sorted(entity.components.by_name_type(str, int))
+            [('A', <class 'int'>), ('B', <class 'int'>)]
+        """
+        # Naive implementation until I feel like optimizing it.
+        for key in self:
+            if not isinstance(key, tuple):
+                continue
+            key_name, key_component = key
+            if key_component is component_type and isinstance(key_name, name_type):
+                yield key_name, key_component
+
     if TYPE_CHECKING:  # Type-hinted overrides
 
         @overload
         def get(self, __key: _ComponentKey[T]) -> T | None:
             ...
 
         @overload
@@ -700,35 +719,21 @@
             >>> world[None].components[("turn", int)]  # Alternative syntax
             0
         """
         return Entity(self, None)
 
     def __setstate__(self, state: dict[str, Any]) -> None:
         """Unpickle this object and handle state migration."""
-        # Migrate from version <=1.0.0.
-        if "_relation_components" in state:
-            _relation_components: dict[_ComponentKey[object], dict[Entity, dict[Entity, Any]]] = state.pop(
-                "_relation_components"
-            )
-            self._relation_components_by_entity = defaultdict(partial(defaultdict, dict))  # type: ignore[arg-type]
-            for component_key, component_key_relations in _relation_components.items():
-                for entity, entities_component_table in component_key_relations.items():
-                    for target_entity, target_component in entities_component_table.items():
-                        self._relation_components_by_entity[entity][component_key][target_entity] = target_component
-
-            _relations_by_key: dict[object, dict[Entity, set[Entity]]] = state.pop("_relations_by_key")
-            self._relation_tags_by_entity = defaultdict(partial(defaultdict, set))  # type: ignore[arg-type]
-            for tag, tag_relations in _relations_by_key.items():
-                for entity, targets in tag_relations.items():
-                    self._relation_tags_by_entity[entity][tag] = targets
-
         state.pop("global_", None)  # Migrate from version <=1.2.0.
 
         self.__dict__.update(state)
 
+        if self.global_.uid is not None:  # Migrate from version <=1.2.0.
+            self.global_._force_remap(None)
+
     def __getitem__(self, uid: object) -> Entity:
         """Return an entity associated with a unique id.
 
         Example::
 
             >>> world = World()
             >>> foo = world["foo"]  # Referencing a new entity returns a new empty entity
```

### Comparing `tcod_ecs-2.0.0/PKG-INFO` & `tcod_ecs-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcod-ecs
-Version: 2.0.0
+Version: 3.0.0
 Summary: A type-hinted Entity Component System based on Python dictionaries and sets.
 Author-email: Kyle Benesch <4b796c65+github@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -22,15 +22,15 @@
 Project-URL: Documentation, https://python-tcod-ecs.readthedocs.io
 Project-URL: Home, https://github.com/HexDecimal
 Project-URL: Source, https://github.com/HexDecimal/python-tcod-ecs
 Provides-Extra: test
 
 # About
 
-[![PyPI](https://img.shields.io/pypi/v/tcod-ec)](https://pypi.org/project/tcod-ecs/)
+[![PyPI](https://img.shields.io/pypi/v/tcod-ecs)](https://pypi.org/project/tcod-ecs/)
 [![PyPI - License](https://img.shields.io/pypi/l/tcod-ecs)](https://github.com/HexDecimal/python-tcod-ecs/blob/main/LICENSE)
 [![Documentation Status](https://readthedocs.org/projects/python-tcod-ecs/badge/?version=latest)](https://python-tcod-ecs.readthedocs.io)
 [![codecov](https://codecov.io/gh/HexDecimal/python-tcod-ecs/branch/main/graph/badge.svg?token=4Ak5QpTLZB)](https://codecov.io/gh/HexDecimal/python-tcod-ecs)
 
 This is an [Entity-component-system](https://en.wikipedia.org/wiki/Entity_component_system) implemented in Python.
 See the [ECS FAQ](https://github.com/SanderMertens/ecs-faq) for more info.
```

