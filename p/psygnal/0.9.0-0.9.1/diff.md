# Comparing `tmp/psygnal-0.9.0.tar.gz` & `tmp/psygnal-0.9.1.tar.gz`

## Comparing `psygnal-0.9.0.tar` & `psygnal-0.9.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0    22798 2020-02-02 00:00:00.000000 psygnal-0.9.0/CHANGELOG.md
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 psygnal-0.9.0/src/psygnal/__init__.py
--rw-r--r--   0        0        0     5164 2020-02-02 00:00:00.000000 psygnal-0.9.0/src/psygnal/_dataclass_utils.py
--rw-r--r--   0        0        0     4212 2020-02-02 00:00:00.000000 psygnal-0.9.0/src/psygnal/_evented_decorator.py
--rw-r--r--   0        0        0    18334 2020-02-02 00:00:00.000000 psygnal-0.9.0/src/psygnal/_evented_model.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 psygnal-0.9.0/src/psygnal/_exceptions.py
--rw-r--r--   0        0        0     9106 2020-02-02 00:00:00.000000 psygnal-0.9.0/src/psygnal/_group.py
--rw-r--r--   0        0        0    16214 2020-02-02 00:00:00.000000 psygnal-0.9.0/src/psygnal/_group_descriptor.py
--rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 psygnal-0.9.0/src/psygnal/_queue.py
--rw-r--r--   0        0        0    50080 2020-02-02 00:00:00.000000 psygnal-0.9.0/src/psygnal/_signal.py
--rw-r--r--   0        0        0     7341 2020-02-02 00:00:00.000000 psygnal-0.9.0/src/psygnal/_throttler.py
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 psygnal-0.9.0/src/psygnal/_throttler.pyi
--rw-r--r--   0        0        0    16226 2020-02-02 00:00:00.000000 psygnal-0.9.0/src/psygnal/_weak_callback.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psygnal-0.9.0/src/psygnal/py.typed
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 psygnal-0.9.0/src/psygnal/qt.py
--rw-r--r--   0        0        0     4396 2020-02-02 00:00:00.000000 psygnal-0.9.0/src/psygnal/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psygnal-0.9.0/src/psygnal/_pyinstaller_util/__init__.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 psygnal-0.9.0/src/psygnal/_pyinstaller_util/_pyinstaller_hook.py
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 psygnal-0.9.0/src/psygnal/_pyinstaller_util/hook-psygnal.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 psygnal-0.9.0/src/psygnal/containers/__init__.py
--rw-r--r--   0        0        0     5746 2020-02-02 00:00:00.000000 psygnal-0.9.0/src/psygnal/containers/_evented_dict.py
--rw-r--r--   0        0        0    15427 2020-02-02 00:00:00.000000 psygnal-0.9.0/src/psygnal/containers/_evented_list.py
--rw-r--r--   0        0        0     7182 2020-02-02 00:00:00.000000 psygnal-0.9.0/src/psygnal/containers/_evented_proxy.py
--rw-r--r--   0        0        0     9967 2020-02-02 00:00:00.000000 psygnal-0.9.0/src/psygnal/containers/_evented_set.py
--rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 psygnal-0.9.0/src/psygnal/containers/_selectable_evented_list.py
--rw-r--r--   0        0        0     6513 2020-02-02 00:00:00.000000 psygnal-0.9.0/src/psygnal/containers/_selection.py
--rw-r--r--   0        0        0     6012 2020-02-02 00:00:00.000000 psygnal-0.9.0/tests/test_bench.py
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 psygnal-0.9.0/tests/test_dataclass_utils.py
--rw-r--r--   0        0        0     5296 2020-02-02 00:00:00.000000 psygnal-0.9.0/tests/test_evented_decorator.py
--rw-r--r--   0        0        0    13116 2020-02-02 00:00:00.000000 psygnal-0.9.0/tests/test_evented_model.py
--rw-r--r--   0        0        0     4934 2020-02-02 00:00:00.000000 psygnal-0.9.0/tests/test_group.py
--rw-r--r--   0        0        0     5078 2020-02-02 00:00:00.000000 psygnal-0.9.0/tests/test_group_descriptor.py
--rw-r--r--   0        0        0    24859 2020-02-02 00:00:00.000000 psygnal-0.9.0/tests/test_psygnal.py
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 psygnal-0.9.0/tests/test_pyinstaller_hook.py
--rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 psygnal-0.9.0/tests/test_qt_compat.py
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 psygnal-0.9.0/tests/test_throttler.py
--rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 psygnal-0.9.0/tests/test_utils.py
--rw-r--r--   0        0        0     4427 2020-02-02 00:00:00.000000 psygnal-0.9.0/tests/test_weak_callable.py
--rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 psygnal-0.9.0/tests/containers/test_evented_dict.py
--rw-r--r--   0        0        0    11859 2020-02-02 00:00:00.000000 psygnal-0.9.0/tests/containers/test_evented_list.py
--rw-r--r--   0        0        0     5085 2020-02-02 00:00:00.000000 psygnal-0.9.0/tests/containers/test_evented_proxy.py
--rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 psygnal-0.9.0/tests/containers/test_evented_set.py
--rw-r--r--   0        0        0     4453 2020-02-02 00:00:00.000000 psygnal-0.9.0/tests/containers/test_selectable_evented_list.py
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 psygnal-0.9.0/tests/containers/test_selection.py
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 psygnal-0.9.0/.gitignore
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 psygnal-0.9.0/LICENSE
--rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 psygnal-0.9.0/README.md
--rw-r--r--   0        0        0     5646 2020-02-02 00:00:00.000000 psygnal-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     6641 2020-02-02 00:00:00.000000 psygnal-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0    23937 2020-02-02 00:00:00.000000 psygnal-0.9.1/CHANGELOG.md
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 psygnal-0.9.1/src/psygnal/__init__.py
+-rw-r--r--   0        0        0     5164 2020-02-02 00:00:00.000000 psygnal-0.9.1/src/psygnal/_dataclass_utils.py
+-rw-r--r--   0        0        0     4212 2020-02-02 00:00:00.000000 psygnal-0.9.1/src/psygnal/_evented_decorator.py
+-rw-r--r--   0        0        0    18334 2020-02-02 00:00:00.000000 psygnal-0.9.1/src/psygnal/_evented_model.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 psygnal-0.9.1/src/psygnal/_exceptions.py
+-rw-r--r--   0        0        0     9106 2020-02-02 00:00:00.000000 psygnal-0.9.1/src/psygnal/_group.py
+-rw-r--r--   0        0        0    16214 2020-02-02 00:00:00.000000 psygnal-0.9.1/src/psygnal/_group_descriptor.py
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 psygnal-0.9.1/src/psygnal/_queue.py
+-rw-r--r--   0        0        0    50396 2020-02-02 00:00:00.000000 psygnal-0.9.1/src/psygnal/_signal.py
+-rw-r--r--   0        0        0     7341 2020-02-02 00:00:00.000000 psygnal-0.9.1/src/psygnal/_throttler.py
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 psygnal-0.9.1/src/psygnal/_throttler.pyi
+-rw-r--r--   0        0        0    16999 2020-02-02 00:00:00.000000 psygnal-0.9.1/src/psygnal/_weak_callback.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psygnal-0.9.1/src/psygnal/py.typed
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 psygnal-0.9.1/src/psygnal/qt.py
+-rw-r--r--   0        0        0     4396 2020-02-02 00:00:00.000000 psygnal-0.9.1/src/psygnal/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psygnal-0.9.1/src/psygnal/_pyinstaller_util/__init__.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 psygnal-0.9.1/src/psygnal/_pyinstaller_util/_pyinstaller_hook.py
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 psygnal-0.9.1/src/psygnal/_pyinstaller_util/hook-psygnal.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 psygnal-0.9.1/src/psygnal/containers/__init__.py
+-rw-r--r--   0        0        0     5746 2020-02-02 00:00:00.000000 psygnal-0.9.1/src/psygnal/containers/_evented_dict.py
+-rw-r--r--   0        0        0    15427 2020-02-02 00:00:00.000000 psygnal-0.9.1/src/psygnal/containers/_evented_list.py
+-rw-r--r--   0        0        0     7182 2020-02-02 00:00:00.000000 psygnal-0.9.1/src/psygnal/containers/_evented_proxy.py
+-rw-r--r--   0        0        0     9967 2020-02-02 00:00:00.000000 psygnal-0.9.1/src/psygnal/containers/_evented_set.py
+-rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 psygnal-0.9.1/src/psygnal/containers/_selectable_evented_list.py
+-rw-r--r--   0        0        0     6513 2020-02-02 00:00:00.000000 psygnal-0.9.1/src/psygnal/containers/_selection.py
+-rw-r--r--   0        0        0     6012 2020-02-02 00:00:00.000000 psygnal-0.9.1/tests/test_bench.py
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 psygnal-0.9.1/tests/test_dataclass_utils.py
+-rw-r--r--   0        0        0     5296 2020-02-02 00:00:00.000000 psygnal-0.9.1/tests/test_evented_decorator.py
+-rw-r--r--   0        0        0    13116 2020-02-02 00:00:00.000000 psygnal-0.9.1/tests/test_evented_model.py
+-rw-r--r--   0        0        0     4934 2020-02-02 00:00:00.000000 psygnal-0.9.1/tests/test_group.py
+-rw-r--r--   0        0        0     5078 2020-02-02 00:00:00.000000 psygnal-0.9.1/tests/test_group_descriptor.py
+-rw-r--r--   0        0        0    25800 2020-02-02 00:00:00.000000 psygnal-0.9.1/tests/test_psygnal.py
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 psygnal-0.9.1/tests/test_pyinstaller_hook.py
+-rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 psygnal-0.9.1/tests/test_qt_compat.py
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 psygnal-0.9.1/tests/test_throttler.py
+-rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 psygnal-0.9.1/tests/test_utils.py
+-rw-r--r--   0        0        0     4827 2020-02-02 00:00:00.000000 psygnal-0.9.1/tests/test_weak_callable.py
+-rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 psygnal-0.9.1/tests/containers/test_evented_dict.py
+-rw-r--r--   0        0        0    11859 2020-02-02 00:00:00.000000 psygnal-0.9.1/tests/containers/test_evented_list.py
+-rw-r--r--   0        0        0     5085 2020-02-02 00:00:00.000000 psygnal-0.9.1/tests/containers/test_evented_proxy.py
+-rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 psygnal-0.9.1/tests/containers/test_evented_set.py
+-rw-r--r--   0        0        0     4453 2020-02-02 00:00:00.000000 psygnal-0.9.1/tests/containers/test_selectable_evented_list.py
+-rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 psygnal-0.9.1/tests/containers/test_selection.py
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 psygnal-0.9.1/.gitignore
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 psygnal-0.9.1/LICENSE
+-rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 psygnal-0.9.1/README.md
+-rw-r--r--   0        0        0     5741 2020-02-02 00:00:00.000000 psygnal-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     6717 2020-02-02 00:00:00.000000 psygnal-0.9.1/PKG-INFO
```

### Comparing `psygnal-0.9.0/CHANGELOG.md` & `psygnal-0.9.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,46 @@
 # Changelog
 
-## [0.9.0](https://github.com/pyapp-kit/psygnal/tree/0.9.0) (2023-04-07)
+## [0.9.1](https://github.com/pyapp-kit/psygnal/tree/0.9.1) (2023-05-29)
 
-[Full Changelog](https://github.com/pyapp-kit/psygnal/compare/v0.8.1...0.9.0)
+[Full Changelog](https://github.com/pyapp-kit/psygnal/compare/v0.9.0...0.9.1)
 
 **Implemented enhancements:**
 
-- feat: add thread parameter to connection method, allowed "queued connections" [\#200](https://github.com/pyapp-kit/psygnal/pull/200) ([tlambert03](https://github.com/tlambert03))
+- feat: Support toolz [\#210](https://github.com/pyapp-kit/psygnal/pull/210) ([tlambert03](https://github.com/tlambert03))
+
+**Fixed bugs:**
+
+- fix: better error message with keyword only partials [\#209](https://github.com/pyapp-kit/psygnal/pull/209) ([tlambert03](https://github.com/tlambert03))
 
 **Tests & CI:**
 
-- ci\(dependabot\): bump pypa/cibuildwheel from 2.12.0 to 2.12.1 [\#197](https://github.com/pyapp-kit/psygnal/pull/197) ([dependabot[bot]](https://github.com/apps/dependabot))
-- ci\(dependabot\): bump actions/setup-python from 3 to 4 [\#193](https://github.com/pyapp-kit/psygnal/pull/193) ([dependabot[bot]](https://github.com/apps/dependabot))
+- build: add test dep [\#206](https://github.com/pyapp-kit/psygnal/pull/206) ([tlambert03](https://github.com/tlambert03))
+
+**Merged pull requests:**
+
+- ci\(dependabot\): bump pypa/cibuildwheel from 2.12.3 to 2.13.0 [\#207](https://github.com/pyapp-kit/psygnal/pull/207) ([dependabot[bot]](https://github.com/apps/dependabot))
+- ci\(pre-commit.ci\): autoupdate [\#205](https://github.com/pyapp-kit/psygnal/pull/205) ([pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci))
+- ci\(dependabot\): bump pypa/cibuildwheel from 2.12.1 to 2.12.3 [\#204](https://github.com/pyapp-kit/psygnal/pull/204) ([dependabot[bot]](https://github.com/apps/dependabot))
+
+## [v0.9.0](https://github.com/pyapp-kit/psygnal/tree/v0.9.0) (2023-04-07)
+
+[Full Changelog](https://github.com/pyapp-kit/psygnal/compare/v0.8.1...v0.9.0)
+
+**Implemented enhancements:**
+
+- feat: add thread parameter to connection method, allowed "queued connections" [\#200](https://github.com/pyapp-kit/psygnal/pull/200) ([tlambert03](https://github.com/tlambert03))
+- build: add pyinstaller hook to simplify frozing apps using pyinstaller  [\#194](https://github.com/pyapp-kit/psygnal/pull/194) ([Czaki](https://github.com/Czaki))
 
 **Merged pull requests:**
 
 - docs: add docs on connecting across thread [\#203](https://github.com/pyapp-kit/psygnal/pull/203) ([tlambert03](https://github.com/tlambert03))
 - chore: deprecate async keyword in emit method [\#201](https://github.com/pyapp-kit/psygnal/pull/201) ([tlambert03](https://github.com/tlambert03))
-- build: add pyinstaller hook to simplify frozing apps using pyinstaller  [\#194](https://github.com/pyapp-kit/psygnal/pull/194) ([Czaki](https://github.com/Czaki))
+- ci\(dependabot\): bump pypa/cibuildwheel from 2.12.0 to 2.12.1 [\#197](https://github.com/pyapp-kit/psygnal/pull/197) ([dependabot[bot]](https://github.com/apps/dependabot))
+- ci\(dependabot\): bump actions/setup-python from 3 to 4 [\#193](https://github.com/pyapp-kit/psygnal/pull/193) ([dependabot[bot]](https://github.com/apps/dependabot))
 
 ## [v0.8.1](https://github.com/pyapp-kit/psygnal/tree/v0.8.1) (2023-02-23)
 
 [Full Changelog](https://github.com/pyapp-kit/psygnal/compare/v0.8.0...v0.8.1)
 
 **Fixed bugs:**
```

### Comparing `psygnal-0.9.0/src/psygnal/__init__.py` & `psygnal-0.9.1/src/psygnal/__init__.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.0/src/psygnal/_dataclass_utils.py` & `psygnal-0.9.1/src/psygnal/_dataclass_utils.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.0/src/psygnal/_evented_decorator.py` & `psygnal-0.9.1/src/psygnal/_evented_decorator.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.0/src/psygnal/_evented_model.py` & `psygnal-0.9.1/src/psygnal/_evented_model.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.0/src/psygnal/_group.py` & `psygnal-0.9.1/src/psygnal/_group.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.0/src/psygnal/_group_descriptor.py` & `psygnal-0.9.1/src/psygnal/_group_descriptor.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.0/src/psygnal/_queue.py` & `psygnal-0.9.1/src/psygnal/_queue.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.0/src/psygnal/_signal.py` & `psygnal-0.9.1/src/psygnal/_signal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import inspect
 import threading
 import warnings
 import weakref
 from contextlib import contextmanager, suppress
-from functools import lru_cache, reduce
+from functools import lru_cache, partial, reduce
 from inspect import Parameter, Signature, isclass
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     ClassVar,
     ContextManager,
@@ -751,15 +751,23 @@
             slot_sig = _get_signature_possibly_qt(slot)
         except ValueError as e:
             warnings.warn(
                 f"{e}. To silence this warning, connect with " "`check_nargs=False`",
                 stacklevel=2,
             )
             return None, None, False
-        minargs, maxargs = _acceptable_posarg_range(slot_sig)
+        try:
+            minargs, maxargs = _acceptable_posarg_range(slot_sig)
+        except ValueError as e:
+            if isinstance(slot, partial):
+                raise ValueError(
+                    f"{e}. (Note: prefer using positional args with "
+                    "functools.partials when possible)."
+                ) from e
+            raise
 
         n_spec_params = len(spec.parameters)
         # if `slot` requires more arguments than we will provide, raise.
         if minargs > n_spec_params:
             extra = (
                 f"- Slot requires at least {minargs} positional "
                 f"arguments, but spec only provides {n_spec_params}"
@@ -1286,15 +1294,15 @@
         elif param.kind is Parameter.VAR_POSITIONAL:
             posargs_unlimited = True
         elif (
             param.kind is Parameter.KEYWORD_ONLY
             and param.default is Parameter.empty
             and forbid_required_kwarg
         ):
-            raise ValueError("Required KEYWORD_ONLY parameters not allowed")
+            raise ValueError(f"Unsupported KEYWORD_ONLY parameters in signature: {sig}")
     return (required, None if posargs_unlimited else required + optional)
 
 
 def _parameter_types_match(
     function: Callable, spec: Signature, func_sig: Signature | None = None
 ) -> bool:
     """Return True if types in `function` signature match those in `spec`.
```

### Comparing `psygnal-0.9.0/src/psygnal/_throttler.py` & `psygnal-0.9.1/src/psygnal/_throttler.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.0/src/psygnal/_throttler.pyi` & `psygnal-0.9.1/src/psygnal/_throttler.pyi`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.0/src/psygnal/_weak_callback.py` & `psygnal-0.9.1/src/psygnal/_weak_callback.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 from __future__ import annotations
 
+import sys
 import weakref
 from functools import partial
 from types import BuiltinMethodType, FunctionType, MethodType, MethodWrapperType
 from typing import TYPE_CHECKING, Any, Callable, Generic, TypeVar, cast
 from warnings import warn
 
 from typing_extensions import Protocol
 
 if TYPE_CHECKING:
-    from typing_extensions import Literal, TypeAlias
+    import toolz
+    from typing_extensions import Literal, TypeAlias, TypeGuard
 
     RefErrorChoice: TypeAlias = Literal["raise", "warn", "ignore"]
 
 __all__ = ["weak_callback", "WeakCallback"]
 _T = TypeVar("_T")
 _R = TypeVar("_R")  # return type of cb
 
 
+def _is_toolz_curry(obj: Any) -> TypeGuard[toolz.curry]:
+    """Return True if obj is a toolz.curry object."""
+    tz = sys.modules.get("toolz")
+    return False if tz is None else isinstance(obj, tz.curry)
+
+
 def weak_callback(
     cb: Callable[..., _R] | WeakCallback[_R],
     *args: Any,
     max_args: int | None = None,
     finalize: Callable[[WeakCallback], Any] | None = None,
     strong_func: bool = True,
     on_ref_error: RefErrorChoice = "warn",
@@ -132,14 +140,29 @@
             except IndexError as e:  # pragma: no cover
                 raise TypeError(
                     "setattr requires two arguments, an object and an attribute name."
                 ) from e
             return _WeakSetattr(obj, attr, max_args, finalize, on_ref_error)
         return _WeakBuiltin(cb, max_args, args, finalize, on_ref_error)
 
+    if _is_toolz_curry(cb):
+        cb_partial = getattr(cb, "_partial", None)
+        if cb_partial is None:  # pragma: no cover
+            raise TypeError(
+                "toolz.curry object found without a '_partial' attribute. This "
+                "version of toolz is not supported. Please open an issue at psygnal."
+            )
+        return weak_callback(
+            cb_partial,
+            *args,
+            max_args=max_args,
+            finalize=finalize,
+            on_ref_error=on_ref_error,
+        )
+
     if callable(cb):
         return _WeakFunction(cb, max_args, args, kwargs, finalize, on_ref_error)
 
     raise TypeError(f"unsupported type {type(cb)}")  # pragma: no cover
 
 
 class WeakCallback(Generic[_R]):
```

### Comparing `psygnal-0.9.0/src/psygnal/qt.py` & `psygnal-0.9.1/src/psygnal/qt.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.0/src/psygnal/utils.py` & `psygnal-0.9.1/src/psygnal/utils.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.0/src/psygnal/_pyinstaller_util/hook-psygnal.py` & `psygnal-0.9.1/src/psygnal/_pyinstaller_util/hook-psygnal.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.0/src/psygnal/containers/__init__.py` & `psygnal-0.9.1/src/psygnal/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.0/src/psygnal/containers/_evented_dict.py` & `psygnal-0.9.1/src/psygnal/containers/_evented_dict.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.0/src/psygnal/containers/_evented_list.py` & `psygnal-0.9.1/src/psygnal/containers/_evented_list.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.0/src/psygnal/containers/_evented_proxy.py` & `psygnal-0.9.1/src/psygnal/containers/_evented_proxy.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.0/src/psygnal/containers/_evented_set.py` & `psygnal-0.9.1/src/psygnal/containers/_evented_set.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.0/src/psygnal/containers/_selectable_evented_list.py` & `psygnal-0.9.1/src/psygnal/containers/_selectable_evented_list.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.0/src/psygnal/containers/_selection.py` & `psygnal-0.9.1/src/psygnal/containers/_selection.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.0/tests/test_bench.py` & `psygnal-0.9.1/tests/test_bench.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.0/tests/test_dataclass_utils.py` & `psygnal-0.9.1/tests/test_dataclass_utils.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.0/tests/test_evented_decorator.py` & `psygnal-0.9.1/tests/test_evented_decorator.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.0/tests/test_evented_model.py` & `psygnal-0.9.1/tests/test_evented_model.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.0/tests/test_group.py` & `psygnal-0.9.1/tests/test_group.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.0/tests/test_group_descriptor.py` & `psygnal-0.9.1/tests/test_group_descriptor.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.0/tests/test_psygnal.py` & `psygnal-0.9.1/tests/test_psygnal.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from contextlib import suppress
 from functools import partial, wraps
 from inspect import Signature
 from typing import Optional
 from unittest.mock import MagicMock, Mock, call
 
 import pytest
+import toolz
 from typing_extensions import Literal
 
 from psygnal import EmitLoopError, Signal, SignalInstance, _compiled
 from psygnal._weak_callback import WeakCallback
 
 
 def stupid_decorator(fun):
@@ -230,34 +231,57 @@
     emitter.one_int.disconnect(mock)
     emitter.one_int.emit(1)
     mock.assert_not_called()
     assert len(emitter.one_int) == 0
 
 
 @pytest.mark.parametrize(
-    "type_", ["function", "lambda", "method", "partial_method", "setattr", "setitem"]
+    "type_",
+    [
+        "function",
+        "lambda",
+        "method",
+        "partial_method",
+        "toolz_function",
+        "toolz_method",
+        "partial_method_kwarg",
+        "partial_method_kwarg_bad",
+        "setattr",
+        "setitem",
+    ],
 )
 def test_slot_types(type_: str) -> None:
     emitter = Emitter()
     signal = emitter.one_int
     assert len(signal) == 0
     obj = MyObj()
 
     if type_ == "setattr":
         signal.connect_setattr(obj, "x")
     elif type_ == "setitem":
         signal.connect_setitem(obj, "x")
     elif type_ == "function":
         signal.connect(f_int)
+
     elif type_ == "lambda":
         signal.connect(lambda x: None)
     elif type_ == "method":
         signal.connect(obj.f_int)
     elif type_ == "partial_method":
         signal.connect(partial(obj.f_int_int, 2))
+    elif type_ == "toolz_function":
+        signal.connect(toolz.curry(f_int_int, 2))
+    elif type_ == "toolz_method":
+        signal.connect(toolz.curry(obj.f_int_int, 2))
+    elif type_ == "partial_method_kwarg":
+        signal.connect(partial(obj.f_int_int, b=2))
+    elif type_ == "partial_method_kwarg_bad":
+        with pytest.raises(ValueError, match=".*prefer using positional args"):
+            signal.connect(partial(obj.f_int_int, a=2))
+        return
 
     assert len(signal) == 1
 
     stored_slot = signal._slots[-1]
     assert isinstance(stored_slot, WeakCallback)
     assert stored_slot == stored_slot
 
@@ -323,25 +347,29 @@
     "slot",
     [
         "f_no_arg",
         "f_int_decorated_stupid",
         "f_int_decorated_good",
         "f_any_assigned",
         "partial",
+        "toolz_curry",
     ],
 )
 def test_weakref(slot):
     """Test that a connected method doesn't hold strong ref."""
     emitter = Emitter()
     obj = MyObj()
 
     assert len(emitter.one_int) == 0
-    emitter.one_int.connect(
-        partial(obj.f_int_int, 1) if slot == "partial" else getattr(obj, slot)
-    )
+    if slot == "partial":
+        emitter.one_int.connect(partial(obj.f_int_int, 1))
+    elif slot == "toolz_curry":
+        emitter.one_int.connect(toolz.curry(obj.f_int_int, 1))
+    else:
+        emitter.one_int.connect(getattr(obj, slot))
     assert len(emitter.one_int) == 1
     emitter.one_int.emit(1)
     assert len(emitter.one_int) == 1
     del obj
     gc.collect()
     emitter.one_int.emit(1)  # this should trigger deletion
     assert len(emitter.one_int) == 0
@@ -534,15 +562,15 @@
     e = Emitter()
 
     def f(a: int, *, b: int):
         ...
 
     with pytest.raises(ValueError) as er:
         e.two_int.connect(f)
-    assert "Required KEYWORD_ONLY parameters not allowed" in str(er)
+    assert "Unsupported KEYWORD_ONLY parameters in signature" in str(er)
 
 
 def test_unique_connections():
     e = Emitter()
     assert len(e.one_int._slots) == 0
 
     e.one_int.connect(f_no_arg, unique=True)
@@ -814,14 +842,15 @@
     "slot",
     [
         "f_no_arg",
         "f_int_decorated_stupid",
         "f_int_decorated_good",
         "f_any_assigned",
         "partial",
+        "partial_kwargs",
         pytest.param(
             "partial",
             marks=pytest.mark.xfail(
                 sys.version_info < (3, 8), reason="no idea why this fails on 3.7"
             ),
         ),
     ],
@@ -829,15 +858,20 @@
 def test_weakref_disconnect(slot):
     """Test that a connected method doesn't hold strong ref."""
 
     emitter = Emitter()
     obj = MyObj()
 
     assert len(emitter.one_int) == 0
-    cb = partial(obj.f_int_int, 1) if slot == "partial" else getattr(obj, slot)
+    if slot == "partial":
+        cb = partial(obj.f_int_int, 1)
+    elif slot == "partial_kwargs":
+        cb = partial(obj.f_int_int, b=1)
+    else:
+        cb = getattr(obj, slot)
     emitter.one_int.connect(cb)
     assert len(emitter.one_int) == 1
     emitter.one_int.emit(1)
     assert len(emitter.one_int) == 1
     emitter.one_int.disconnect(cb)
     assert len(emitter.one_int) == 0
```

### Comparing `psygnal-0.9.0/tests/test_pyinstaller_hook.py` & `psygnal-0.9.1/tests/test_pyinstaller_hook.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.0/tests/test_qt_compat.py` & `psygnal-0.9.1/tests/test_qt_compat.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.0/tests/test_throttler.py` & `psygnal-0.9.1/tests/test_throttler.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.0/tests/test_utils.py` & `psygnal-0.9.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.0/tests/test_weak_callable.py` & `psygnal-0.9.1/tests/test_weak_callable.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import gc
 from functools import partial
 from unittest.mock import Mock
 from weakref import ref
 
 import pytest
+import toolz
 
 from psygnal._weak_callback import WeakCallback, weak_callback
 
 
 @pytest.mark.parametrize(
     "type_",
     [
         "function",
+        "toolz_function",
         "weak_func",
         "lambda",
         "method",
         "partial_method",
+        "toolz_method",
         "setattr",
         "setitem",
         "mock",
         "weak_cb",
         "print",
     ],
 )
@@ -50,20 +53,30 @@
     elif type_ in {"function", "weak_func"}:
 
         def obj(x: int) -> None:
             mock(x)
             return x
 
         cb = weak_callback(obj, strong_func=(type_ == "function"), finalize=final_mock)
+    elif type_ == "toolz_function":
+
+        @toolz.curry
+        def obj(z: int, x: int) -> None:
+            mock(x)
+            return x
+
+        cb = weak_callback(obj(5), finalize=final_mock)
     elif type_ == "lambda":
         cb = weak_callback(lambda x: mock(x) and x, finalize=final_mock)
     elif type_ == "method":
         cb = weak_callback(obj.method, finalize=final_mock)
     elif type_ == "partial_method":
         cb = weak_callback(partial(obj.method, 2), max_args=0, finalize=final_mock)
+    elif type_ == "toolz_method":
+        cb = weak_callback(toolz.curry(obj.method, 2), max_args=0, finalize=final_mock)
     elif type_ == "mock":
         cb = weak_callback(mock, finalize=final_mock)
     elif type_ == "weak_cb":
         cb = weak_callback(obj.method, finalize=final_mock)
         cb = weak_callback(cb, finalize=final_mock)
     elif type_ == "print":
         cb = weak_callback(print, finalize=final_mock)
@@ -80,15 +93,15 @@
     result = cb(2)
     if type_ not in ("setattr", "mock"):
         assert result == 2
     mock.assert_called_once_with(2)
 
     del obj
 
-    if type_ not in ("function", "lambda", "mock"):
+    if type_ not in ("function", "toolz_function", "lambda", "mock"):
         final_mock.assert_called_once_with(cb)
         assert cb.dereference() is None
         with pytest.raises(ReferenceError):
             cb.cb((2,))
         with pytest.raises(ReferenceError):
             cb(2)
     else:
```

### Comparing `psygnal-0.9.0/tests/containers/test_evented_dict.py` & `psygnal-0.9.1/tests/containers/test_evented_dict.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.0/tests/containers/test_evented_list.py` & `psygnal-0.9.1/tests/containers/test_evented_list.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.0/tests/containers/test_evented_proxy.py` & `psygnal-0.9.1/tests/containers/test_evented_proxy.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.0/tests/containers/test_evented_set.py` & `psygnal-0.9.1/tests/containers/test_evented_set.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.0/tests/containers/test_selectable_evented_list.py` & `psygnal-0.9.1/tests/containers/test_selectable_evented_list.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.0/tests/containers/test_selection.py` & `psygnal-0.9.1/tests/containers/test_selection.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.0/.gitignore` & `psygnal-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.0/LICENSE` & `psygnal-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.0/README.md` & `psygnal-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.0/pyproject.toml` & `psygnal-0.9.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -60,22 +60,24 @@
     "mkdocstrings==0.20.0",
     "mkdocs-spellcheck[all]",
 ]
 proxy = ["wrapt"]
 pydantic = ["pydantic"]
 test = [
     "dask",
+    "attrs",
     "numpy",
     "pydantic",
     "pyinstaller>=4.0",
     "pytest>=6.0",
     "pytest-codspeed",
     "pytest-cov",
     "wrapt",
     "msgspec ; python_version >= '3.8'",
+    "toolz",
 ]
 testqt = ["pytest-qt", "qtpy"]
 
 [project.urls]
 homepage = "https://github.com/pyapp-kit/psygnal"
 repository = "https://github.com/pyapp-kit/psygnal"
 documentation = "https://psygnal.readthedocs.io"
@@ -125,37 +127,38 @@
 
 
 # https://github.com/charliermarsh/ruff
 [tool.ruff]
 line-length = 88
 target-version = "py37"
 src = ["src", "tests"]
-extend-select = [
+select = [
     "E",  # style errors
     "F",  # flakes
     "D",  # pydocstyle
     "I",  # isort
     "UP", # pyupgrade
     # "N",  # pep8-naming
     "S",    # bandit
     "C4",   # flake8-comprehensions
     "B",    # flake8-bugbear
     "A001", # flake8-builtins
     "TID",  # flake8-tidy-imports
     "RUF",  # ruff-specific rules
 ]
-extend-ignore = [
-    "D100", # Missing docstring in public module
-    "D107", # Missing docstring in __init__
-    "D203", # 1 blank line required before class docstring
-    "D212", # Multi-line docstring summary should start at the first line
-    "D213", # Multi-line docstring summary should start at the second line
-    "D401", # First line should be in imperative mood
-    "D413", # Missing blank line after last section
-    "D416", # Section name should end with a colon
+ignore = [
+    "D100",   # Missing docstring in public module
+    "D107",   # Missing docstring in __init__
+    "D203",   # 1 blank line required before class docstring
+    "D212",   # Multi-line docstring summary should start at the first line
+    "D213",   # Multi-line docstring summary should start at the second line
+    "D401",   # First line should be in imperative mood
+    "D413",   # Missing blank line after last section
+    "D416",   # Section name should end with a colon
+    "RUF009", # Do not perform function call in dataclass defaults
 ]
 
 [tool.ruff.per-file-ignores]
 "tests/*.py" = ["D", "S"]
 "benchmarks/*.py" = ["D"]
 "setup.py" = ["D"]
```

### Comparing `psygnal-0.9.0/PKG-INFO` & `psygnal-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psygnal
-Version: 0.9.0
+Version: 0.9.1
 Summary: Fast python callback/event system modeled after Qt Signals
 Project-URL: homepage, https://github.com/pyapp-kit/psygnal
 Project-URL: repository, https://github.com/pyapp-kit/psygnal
 Project-URL: documentation, https://psygnal.readthedocs.io
 Author-email: Talley Lambert <talley.lambert@gmail.com>
 License: BSD 3-Clause License
 License-File: LICENSE
@@ -48,22 +48,24 @@
 Requires-Dist: mkdocstrings-python==0.8.3; extra == 'docs'
 Requires-Dist: mkdocstrings==0.20.0; extra == 'docs'
 Provides-Extra: proxy
 Requires-Dist: wrapt; extra == 'proxy'
 Provides-Extra: pydantic
 Requires-Dist: pydantic; extra == 'pydantic'
 Provides-Extra: test
+Requires-Dist: attrs; extra == 'test'
 Requires-Dist: dask; extra == 'test'
 Requires-Dist: msgspec; python_version >= '3.8' and extra == 'test'
 Requires-Dist: numpy; extra == 'test'
 Requires-Dist: pydantic; extra == 'test'
 Requires-Dist: pyinstaller>=4.0; extra == 'test'
 Requires-Dist: pytest-codspeed; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: pytest>=6.0; extra == 'test'
+Requires-Dist: toolz; extra == 'test'
 Requires-Dist: wrapt; extra == 'test'
 Provides-Extra: testqt
 Requires-Dist: pytest-qt; extra == 'testqt'
 Requires-Dist: qtpy; extra == 'testqt'
 Description-Content-Type: text/markdown
 
 # psygnal
```

