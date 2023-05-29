# Comparing `tmp/scikit_rough-0.0.1a2.tar.gz` & `tmp/scikit_rough-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit_rough-0.0.1a2.tar", max compression
+gzip compressed data, was "scikit_rough-0.1.0.tar", max compression
```

## Comparing `scikit_rough-0.0.1a2.tar` & `scikit_rough-0.1.0.tar`

### file list

```diff
@@ -1,58 +1,73 @@
--rw-r--r--   0        0        0     1062 2021-12-29 15:40:09.403124 scikit_rough-0.0.1a2/LICENSE
--rw-r--r--   0        0        0     2326 2022-12-10 13:48:31.376536 scikit_rough-0.0.1a2/README.md
--rw-r--r--   0        0        0     2736 2023-02-04 15:30:41.663208 scikit_rough-0.0.1a2/pyproject.toml
--rw-r--r--   0        0        0      641 2022-10-03 16:58:08.197786 scikit_rough-0.0.1a2/src/skrough/__init__.py
--rw-r--r--   0        0        0        0 2022-07-21 22:41:43.827993 scikit_rough-0.0.1a2/src/skrough/algorithms/__init__.py
--rw-r--r--   0        0        0     1158 2022-09-11 17:21:42.171638 scikit_rough-0.0.1a2/src/skrough/algorithms/bireduct_ordering.py
--rw-r--r--   0        0        0      355 2022-10-03 16:58:08.197786 scikit_rough-0.0.1a2/src/skrough/algorithms/exceptions.py
--rw-r--r--   0        0        0      532 2022-08-01 17:51:34.166308 scikit_rough-0.0.1a2/src/skrough/algorithms/hooks/__init__.py
--rw-r--r--   0        0        0     4438 2022-11-12 13:41:10.366208 scikit_rough-0.0.1a2/src/skrough/algorithms/hooks/common/process_elements.py
--rw-r--r--   0        0        0     1995 2022-12-02 22:57:30.555588 scikit_rough-0.0.1a2/src/skrough/algorithms/hooks/filter_hooks.py
--rw-r--r--   0        0        0      792 2022-11-20 23:49:48.941955 scikit_rough-0.0.1a2/src/skrough/algorithms/hooks/finalize_hooks.py
--rw-r--r--   0        0        0     5145 2023-01-15 23:28:34.034062 scikit_rough-0.0.1a2/src/skrough/algorithms/hooks/init_hooks.py
--rw-r--r--   0        0        0      640 2022-11-20 23:49:48.941955 scikit_rough-0.0.1a2/src/skrough/algorithms/hooks/inner_init_hooks.py
--rw-r--r--   0        0        0      907 2022-11-20 23:49:48.941955 scikit_rough-0.0.1a2/src/skrough/algorithms/hooks/inner_process_hooks.py
--rw-r--r--   0        0        0      358 2022-09-14 22:29:15.424012 scikit_rough-0.0.1a2/src/skrough/algorithms/hooks/inner_stop_hooks.py
--rw-r--r--   0        0        0      680 2022-11-20 23:49:48.941955 scikit_rough-0.0.1a2/src/skrough/algorithms/hooks/pre_candidates_hooks.py
--rw-r--r--   0        0        0      801 2022-11-20 23:49:48.941955 scikit_rough-0.0.1a2/src/skrough/algorithms/hooks/prepare_result_hooks.py
--rw-r--r--   0        0        0     1371 2022-11-20 23:49:48.941955 scikit_rough-0.0.1a2/src/skrough/algorithms/hooks/select_hooks.py
--rw-r--r--   0        0        0     5239 2022-12-03 00:58:36.523489 scikit_rough-0.0.1a2/src/skrough/algorithms/hooks/stop_hooks.py
--rw-r--r--   0        0        0     2700 2022-12-03 00:52:25.598479 scikit_rough-0.0.1a2/src/skrough/algorithms/key_names.py
--rw-r--r--   0        0        0        0 2022-07-21 22:41:43.831993 scikit_rough-0.0.1a2/src/skrough/algorithms/meta/__init__.py
--rw-r--r--   0        0        0     5900 2023-01-15 18:46:36.524766 scikit_rough-0.0.1a2/src/skrough/algorithms/meta/aggregates.py
--rw-r--r--   0        0        0     8719 2023-01-15 18:45:38.309293 scikit_rough-0.0.1a2/src/skrough/algorithms/meta/describe.py
--rw-r--r--   0        0        0     1875 2022-10-03 16:58:08.197786 scikit_rough-0.0.1a2/src/skrough/algorithms/meta/helpers.py
--rw-r--r--   0        0        0     5116 2023-01-15 18:46:40.560730 scikit_rough-0.0.1a2/src/skrough/algorithms/meta/processing.py
--rw-r--r--   0        0        0     8658 2023-01-15 18:46:36.524766 scikit_rough-0.0.1a2/src/skrough/algorithms/meta/stage.py
--rw-r--r--   0        0        0     2304 2022-11-20 23:49:48.945955 scikit_rough-0.0.1a2/src/skrough/algorithms/meta/visual_block.py
--rw-r--r--   0        0        0      677 2022-09-11 17:21:42.171638 scikit_rough-0.0.1a2/src/skrough/algorithms/reduct_ordering.py
--rw-r--r--   0        0        0     1669 2022-08-24 18:51:55.252722 scikit_rough-0.0.1a2/src/skrough/attrs_checks.py
--rw-r--r--   0        0        0      142 2022-10-03 16:58:08.197786 scikit_rough-0.0.1a2/src/skrough/chaos_measures/__init__.py
--rw-r--r--   0        0        0     3530 2022-11-15 22:54:03.636482 scikit_rough-0.0.1a2/src/skrough/chaos_measures/chaos_measures.py
--rw-r--r--   0        0        0     1282 2022-07-21 22:41:43.831993 scikit_rough-0.0.1a2/src/skrough/chaos_measures/gini_impurity_cython.pyx
--rw-r--r--   0        0        0     9652 2022-11-12 11:59:31.521830 scikit_rough-0.0.1a2/src/skrough/chaos_score.py
--rw-r--r--   0        0        0     7995 2022-12-14 23:01:17.732422 scikit_rough-0.0.1a2/src/skrough/checks.py
--rw-r--r--   0        0        0     5342 2022-12-14 23:01:25.912353 scikit_rough-0.0.1a2/src/skrough/dataprep.py
--rw-r--r--   0        0        0        0 2022-07-21 22:41:43.831993 scikit_rough-0.0.1a2/src/skrough/estimators/__init__.py
--rw-r--r--   0        0        0     1434 2022-07-21 22:41:43.831993 scikit_rough-0.0.1a2/src/skrough/estimators/base.py
--rw-r--r--   0        0        0     3550 2022-10-03 16:58:08.201786 scikit_rough-0.0.1a2/src/skrough/feature_importance.py
--rw-r--r--   0        0        0    15165 2022-11-12 11:59:31.521830 scikit_rough-0.0.1a2/src/skrough/homogeneity.py
--rw-r--r--   0        0        0     6414 2022-10-08 17:21:02.795399 scikit_rough-0.0.1a2/src/skrough/instances.py
--rw-r--r--   0        0        0     1396 2022-10-03 16:58:08.201786 scikit_rough-0.0.1a2/src/skrough/logs.py
--rw-r--r--   0        0        0     6302 2022-10-03 16:58:08.201786 scikit_rough-0.0.1a2/src/skrough/permutations.py
--rw-r--r--   0        0        0     3637 2022-09-27 20:04:11.457692 scikit_rough-0.0.1a2/src/skrough/predict.py
--rw-r--r--   0        0        0     2672 2022-12-14 23:01:34.440281 scikit_rough-0.0.1a2/src/skrough/rough.py
--rw-r--r--   0        0        0       26 2022-10-03 16:58:08.201786 scikit_rough-0.0.1a2/src/skrough/structs/__init__.py
--rw-r--r--   0        0        0     1115 2022-10-03 16:58:08.201786 scikit_rough-0.0.1a2/src/skrough/structs/attrs_subset.py
--rw-r--r--   0        0        0     1213 2022-10-03 16:58:08.201786 scikit_rough-0.0.1a2/src/skrough/structs/chaos_score_stats.py
--rw-r--r--   0        0        0     2314 2022-11-20 23:49:48.945955 scikit_rough-0.0.1a2/src/skrough/structs/description_node.py
--rw-r--r--   0        0        0     5697 2022-11-22 23:33:28.074692 scikit_rough-0.0.1a2/src/skrough/structs/group_index.py
--rw-r--r--   0        0        0     1360 2022-10-03 16:58:08.205786 scikit_rough-0.0.1a2/src/skrough/structs/objs_attrs_subset.py
--rw-r--r--   0        0        0     1825 2022-11-22 23:49:05.234388 scikit_rough-0.0.1a2/src/skrough/structs/state.py
--rw-r--r--   0        0        0     3847 2023-01-15 18:46:36.524766 scikit_rough-0.0.1a2/src/skrough/typing.py
--rw-r--r--   0        0        0      820 2023-01-15 21:23:48.857033 scikit_rough-0.0.1a2/src/skrough/unify.py
--rw-r--r--   0        0        0     4298 2022-10-03 16:58:08.205786 scikit_rough-0.0.1a2/src/skrough/unique.py
--rw-r--r--   0        0        0     2367 2022-10-03 16:58:08.205786 scikit_rough-0.0.1a2/src/skrough/utils.py
--rw-r--r--   0        0        0     5892 2022-10-03 16:58:08.205786 scikit_rough-0.0.1a2/src/skrough/weights.py
--rw-r--r--   0        0        0     3402 1970-01-01 00:00:00.000000 scikit_rough-0.0.1a2/setup.py
--rw-r--r--   0        0        0     3184 1970-01-01 00:00:00.000000 scikit_rough-0.0.1a2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2021-12-29 15:40:09.403124 scikit_rough-0.1.0/LICENSE
+-rw-r--r--   0        0        0     2326 2023-03-24 17:28:51.767768 scikit_rough-0.1.0/README.md
+-rw-r--r--   0        0        0     2633 2023-05-29 06:52:48.963212 scikit_rough-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      613 2023-04-06 22:35:02.629566 scikit_rough-0.1.0/src/skrough/__init__.py
+-rw-r--r--   0        0        0        0 2022-07-21 22:41:43.827993 scikit_rough-0.1.0/src/skrough/algorithms/__init__.py
+-rw-r--r--   0        0        0     1158 2023-03-24 17:34:53.713358 scikit_rough-0.1.0/src/skrough/algorithms/bireduct_ordering.py
+-rw-r--r--   0        0        0     4513 2023-04-04 20:57:31.277105 scikit_rough-0.1.0/src/skrough/algorithms/bireducts.py
+-rw-r--r--   0        0        0       27 2023-04-02 21:56:08.828673 scikit_rough-0.1.0/src/skrough/algorithms/constants.py
+-rw-r--r--   0        0        0      355 2022-10-03 16:58:08.197786 scikit_rough-0.1.0/src/skrough/algorithms/exceptions.py
+-rw-r--r--   0        0        0      532 2022-08-01 17:51:34.166308 scikit_rough-0.1.0/src/skrough/algorithms/hooks/__init__.py
+-rw-r--r--   0        0        0     4441 2023-04-01 08:11:26.460438 scikit_rough-0.1.0/src/skrough/algorithms/hooks/common/process_elements.py
+-rw-r--r--   0        0        0     1998 2023-04-04 06:18:31.195599 scikit_rough-0.1.0/src/skrough/algorithms/hooks/filter_hooks.py
+-rw-r--r--   0        0        0      794 2023-04-01 23:15:42.415609 scikit_rough-0.1.0/src/skrough/algorithms/hooks/finalize_hooks.py
+-rw-r--r--   0        0        0     1029 2023-04-01 08:51:01.439278 scikit_rough-0.1.0/src/skrough/algorithms/hooks/helpers.py
+-rw-r--r--   0        0        0     6170 2023-04-04 20:35:32.043838 scikit_rough-0.1.0/src/skrough/algorithms/hooks/init_hooks.py
+-rw-r--r--   0        0        0      640 2022-11-20 23:49:48.941955 scikit_rough-0.1.0/src/skrough/algorithms/hooks/inner_init_hooks.py
+-rw-r--r--   0        0        0     1585 2023-04-04 06:18:37.707561 scikit_rough-0.1.0/src/skrough/algorithms/hooks/inner_process_hooks.py
+-rw-r--r--   0        0        0      646 2023-04-01 08:28:07.386135 scikit_rough-0.1.0/src/skrough/algorithms/hooks/inner_stop_hooks.py
+-rw-r--r--   0        0        0      836 2023-04-01 08:41:25.586112 scikit_rough-0.1.0/src/skrough/algorithms/hooks/pre_candidates_hooks.py
+-rw-r--r--   0        0        0      801 2022-11-20 23:49:48.941955 scikit_rough-0.1.0/src/skrough/algorithms/hooks/prepare_result_hooks.py
+-rw-r--r--   0        0        0     1371 2023-04-04 06:20:15.082969 scikit_rough-0.1.0/src/skrough/algorithms/hooks/select_hooks.py
+-rw-r--r--   0        0        0     5092 2023-04-03 12:53:25.690892 scikit_rough-0.1.0/src/skrough/algorithms/hooks/stop_hooks.py
+-rw-r--r--   0        0        0     3238 2023-04-03 11:31:36.008592 scikit_rough-0.1.0/src/skrough/algorithms/key_names.py
+-rw-r--r--   0        0        0        0 2022-07-21 22:41:43.831993 scikit_rough-0.1.0/src/skrough/algorithms/meta/__init__.py
+-rw-r--r--   0        0        0     5900 2023-01-15 18:46:36.524766 scikit_rough-0.1.0/src/skrough/algorithms/meta/aggregates.py
+-rw-r--r--   0        0        0     8712 2023-04-06 21:25:33.260645 scikit_rough-0.1.0/src/skrough/algorithms/meta/describe.py
+-rw-r--r--   0        0        0     1875 2022-10-03 16:58:08.197786 scikit_rough-0.1.0/src/skrough/algorithms/meta/helpers.py
+-rw-r--r--   0        0        0     5874 2023-04-02 22:53:41.286673 scikit_rough-0.1.0/src/skrough/algorithms/meta/processing.py
+-rw-r--r--   0        0        0     8658 2023-01-15 18:46:36.524766 scikit_rough-0.1.0/src/skrough/algorithms/meta/stage.py
+-rw-r--r--   0        0        0     2304 2022-11-20 23:49:48.945955 scikit_rough-0.1.0/src/skrough/algorithms/meta/visual_block.py
+-rw-r--r--   0        0        0      677 2022-09-11 17:21:42.171638 scikit_rough-0.1.0/src/skrough/algorithms/reduct_ordering.py
+-rw-r--r--   0        0        0     4127 2023-04-03 21:26:51.573057 scikit_rough-0.1.0/src/skrough/algorithms/reducts.py
+-rw-r--r--   0        0        0        0 2023-03-30 07:15:57.177405 scikit_rough-0.1.0/src/skrough/algorithms/reusables/__init__.py
+-rw-r--r--   0        0        0     1198 2023-04-06 18:35:16.293477 scikit_rough-0.1.0/src/skrough/algorithms/reusables/attrs_daab.py
+-rw-r--r--   0        0        0     1097 2023-04-06 18:35:27.545626 scikit_rough-0.1.0/src/skrough/algorithms/reusables/attrs_daar.py
+-rw-r--r--   0        0        0      971 2023-04-06 18:36:02.786112 scikit_rough-0.1.0/src/skrough/algorithms/reusables/attrs_greedy.py
+-rw-r--r--   0        0        0      831 2023-04-03 11:36:29.970571 scikit_rough-0.1.0/src/skrough/algorithms/reusables/attrs_reduction.py
+-rw-r--r--   0        0        0     1671 2023-04-03 07:56:35.990697 scikit_rough-0.1.0/src/skrough/attrs_checks.py
+-rw-r--r--   0        0        0      142 2022-10-03 16:58:08.197786 scikit_rough-0.1.0/src/skrough/chaos_measures/__init__.py
+-rw-r--r--   0        0        0     3530 2022-11-15 22:54:03.636482 scikit_rough-0.1.0/src/skrough/chaos_measures/chaos_measures.py
+-rw-r--r--   0        0        0     1282 2022-07-21 22:41:43.831993 scikit_rough-0.1.0/src/skrough/chaos_measures/gini_impurity_cython.pyx
+-rw-r--r--   0        0        0     9720 2023-03-29 13:53:00.396859 scikit_rough-0.1.0/src/skrough/chaos_score.py
+-rw-r--r--   0        0        0     7995 2022-12-14 23:01:17.732422 scikit_rough-0.1.0/src/skrough/checks.py
+-rw-r--r--   0        0        0     5634 2023-04-17 10:21:42.576840 scikit_rough-0.1.0/src/skrough/dataprep.py
+-rw-r--r--   0        0        0        0 2022-07-21 22:41:43.831993 scikit_rough-0.1.0/src/skrough/estimators/__init__.py
+-rw-r--r--   0        0        0     1434 2022-07-21 22:41:43.831993 scikit_rough-0.1.0/src/skrough/estimators/base.py
+-rw-r--r--   0        0        0     9937 2023-04-03 21:20:27.987988 scikit_rough-0.1.0/src/skrough/feature_importance.py
+-rw-r--r--   0        0        0    15165 2022-11-12 11:59:31.521830 scikit_rough-0.1.0/src/skrough/homogeneity.py
+-rw-r--r--   0        0        0     6414 2022-10-08 17:21:02.795399 scikit_rough-0.1.0/src/skrough/instances.py
+-rw-r--r--   0        0        0     1396 2022-10-03 16:58:08.201786 scikit_rough-0.1.0/src/skrough/logs.py
+-rw-r--r--   0        0        0     6302 2022-10-03 16:58:08.201786 scikit_rough-0.1.0/src/skrough/permutations.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:36:28.084330 scikit_rough-0.1.0/src/skrough/predict/__init__.py
+-rw-r--r--   0        0        0      810 2023-04-06 20:10:29.718991 scikit_rough-0.1.0/src/skrough/predict/aggregate.py
+-rw-r--r--   0        0        0     7835 2023-04-07 15:22:13.919380 scikit_rough-0.1.0/src/skrough/predict/helpers.py
+-rw-r--r--   0        0        0     1357 2023-04-07 15:14:38.311191 scikit_rough-0.1.0/src/skrough/predict/predict_attrs.py
+-rw-r--r--   0        0        0     1233 2023-04-07 15:17:58.561532 scikit_rough-0.1.0/src/skrough/predict/predict_attrs_ensemble.py
+-rw-r--r--   0        0        0     1418 2023-04-07 15:17:09.665940 scikit_rough-0.1.0/src/skrough/predict/predict_objs_attrs.py
+-rw-r--r--   0        0        0     1266 2023-04-07 15:17:54.885563 scikit_rough-0.1.0/src/skrough/predict/predict_objs_attrs_ensemble.py
+-rw-r--r--   0        0        0     2580 2023-04-21 19:53:36.531956 scikit_rough-0.1.0/src/skrough/ranks.py
+-rw-r--r--   0        0        0     2672 2022-12-14 23:01:34.440281 scikit_rough-0.1.0/src/skrough/rough.py
+-rw-r--r--   0        0        0       26 2022-10-03 16:58:08.201786 scikit_rough-0.1.0/src/skrough/structs/__init__.py
+-rw-r--r--   0        0        0     1115 2022-10-03 16:58:08.201786 scikit_rough-0.1.0/src/skrough/structs/attrs_subset.py
+-rw-r--r--   0        0        0     1213 2022-10-03 16:58:08.201786 scikit_rough-0.1.0/src/skrough/structs/chaos_score_stats.py
+-rw-r--r--   0        0        0     2314 2022-11-20 23:49:48.945955 scikit_rough-0.1.0/src/skrough/structs/description_node.py
+-rw-r--r--   0        0        0     5714 2023-03-29 13:46:51.929882 scikit_rough-0.1.0/src/skrough/structs/group_index.py
+-rw-r--r--   0        0        0     1360 2022-10-03 16:58:08.205786 scikit_rough-0.1.0/src/skrough/structs/objs_attrs_subset.py
+-rw-r--r--   0        0        0     1825 2022-11-22 23:49:05.234388 scikit_rough-0.1.0/src/skrough/structs/state.py
+-rw-r--r--   0        0        0     4517 2023-04-07 15:12:22.108298 scikit_rough-0.1.0/src/skrough/typing.py
+-rw-r--r--   0        0        0      820 2023-01-15 21:23:48.857033 scikit_rough-0.1.0/src/skrough/unify.py
+-rw-r--r--   0        0        0     4298 2022-10-03 16:58:08.205786 scikit_rough-0.1.0/src/skrough/unique.py
+-rw-r--r--   0        0        0     2367 2022-10-03 16:58:08.205786 scikit_rough-0.1.0/src/skrough/utils.py
+-rw-r--r--   0        0        0     5892 2022-10-03 16:58:08.205786 scikit_rough-0.1.0/src/skrough/weights.py
+-rw-r--r--   0        0        0     3181 1970-01-01 00:00:00.000000 scikit_rough-0.1.0/PKG-INFO
```

### Comparing `scikit_rough-0.0.1a2/LICENSE` & `scikit_rough-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_rough-0.0.1a2/README.md` & `scikit_rough-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `scikit_rough-0.0.1a2/pyproject.toml` & `scikit_rough-0.1.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "scikit-rough"
-version = "0.0.1-alpha.2"
+version = "0.1.0"
 description = ""
 authors = ["sebov <12091011+sebov@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "skrough", from = "src" }]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.12"
-attrs = "^22.0.1"
+python = "^3.8"
+attrs = "^23.1.0"
 docstring-parser = "^0.15"
 joblib = "^1.1.0"
 more-itertools = "^8.14.0"
 numba = "^0.56.0"
 numpy = "^1.22.4"
-pandas = "^1.4.2"
+pandas = "^2.0.0"
 scikit-learn = "^1.1.1"
 
 [tool.poetry.group.dev.dependencies]
 nbconvert = "^7.2.3"
 nb-pdf-template = "^4.0.0"
 jupytext = "^1.14.1"
 poethepoet = "^0.14.0"
@@ -75,43 +75,35 @@
 
 [tool.bandit]
 exclude_dirs = ["tests/"]
 
 [tool.pyright]
 
 [tool.poe.tasks.test]
-shell = "poetry run pytest ${opts} ${tests}"
-[[tool.poe.tasks.test.args]]
-name = "opts"
-positional = false
-multiple = false
-default = ""
+shell = "poetry run pytest ${tests}"
 [[tool.poe.tasks.test.args]]
 name = "tests"
 positional = true
 multiple = true
 default = "tests"
 
 [tool.poe.tasks.testcov]
 shell = """
         NUMBA_DISABLE_JIT=1 poetry run pytest \
-        --cov-report=term --cov-report=xml --cov=src/skrough ${opts} ${tests}
+        --cov-report=term --cov-report=xml --cov=src/skrough ${tests}
         """
 [[tool.poe.tasks.testcov.args]]
-name = "opts"
-positional = false
-multiple = false
-default = ""
-[[tool.poe.tasks.testcov.args]]
 name = "tests"
 positional = true
 multiple = true
 default = "tests"
 
 [tool.poe.tasks.docs]
 shell = """
         cd docs && make html
         """
 
 [tool.poe.tasks]
 isort = "isort src/ tests/"
 format = "black src/ tests/"
+lint = "pylint --rcfile .pylintrc src/ tests/ dev/"
+lint-examples = "pylint --rcfile .pylintrc_examples examples/"
```

### Comparing `scikit_rough-0.0.1a2/src/skrough/__init__.py` & `scikit_rough-0.1.0/src/skrough/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     chaos_score,
     checks,
     dataprep,
     feature_importance,
     homogeneity,
     instances,
     permutations,
-    predict,
     rough,
     structs,
     unify,
     unique,
     weights,
 )
 
@@ -26,15 +25,14 @@
     "chaos_score",
     "checks",
     "dataprep",
     "feature_importance",
     "homogeneity",
     "instances",
     "permutations",
-    "predict",
     "rough",
     "structs",
     "unify",
     "unique",
     "weights",
 ]
 __version__ = "0.1.0"
```

### Comparing `scikit_rough-0.0.1a2/src/skrough/algorithms/bireduct_ordering.py` & `scikit_rough-0.1.0/src/skrough/algorithms/bireduct_ordering.py`

 * *Files identical despite different names*

### Comparing `scikit_rough-0.0.1a2/src/skrough/algorithms/hooks/__init__.py` & `scikit_rough-0.1.0/src/skrough/algorithms/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit_rough-0.0.1a2/src/skrough/algorithms/hooks/common/process_elements.py` & `scikit_rough-0.1.0/src/skrough/algorithms/hooks/common/process_elements.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,16 +44,16 @@
     ) -> rght.Elements:
         """Process elements hook returning a random sample from the input ``elements``.
 
         Process elements hook returning a random sample from the input ``elements``. The
         number of elements that should be drawn randomly is stored in
         :code:`state.config` under the ``candidates_count_config_key`` key. If the given
         key is not available in :code:`state.config` or is `None` then the number of
-        elements to be draw will fallback to the total number of elements. The value of
-        the ``elements_count_config_key`` come from the enclosing scope. The hook
+        elements to be drawn will fall back to the total number of elements. The value
+        of the ``elements_count_config_key`` comes from the enclosing scope. The hook
         function uses :obj:`state.rng` random generator to perform the random choice
         operation. If the number of elements to be drawn from the config is larger than
         the actual size of the input elements then the sample size is decreased to the
         size of the input.
 
         Args:
             state: An object representing processing state.
```

### Comparing `scikit_rough-0.0.1a2/src/skrough/algorithms/hooks/filter_hooks.py` & `scikit_rough-0.1.0/src/skrough/algorithms/hooks/filter_hooks.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import numpy as np
 
 import skrough.typing as rght
 from skrough.algorithms.key_names import (
     CONFIG_CHAOS_FUN,
     CONFIG_DAAR_ALLOWED_RANDOMNESS,
-    CONFIG_DAAR_N_OF_PROBES,
+    CONFIG_DAAR_PROBES_COUNT,
     VALUES_GROUP_INDEX,
     VALUES_X,
     VALUES_X_COUNTS,
     VALUES_Y,
     VALUES_Y_COUNT,
 )
 from skrough.attrs_checks import check_if_attr_better_than_shuffled
@@ -24,16 +24,16 @@
 
 
 @log_start_end(logger)
 def filter_hook_attrs_first_daar(
     state: ProcessingState,
     elements: rght.Elements,
 ) -> rght.Elements:
-    daar_n_of_probes = state.config[CONFIG_DAAR_N_OF_PROBES]
-    logger.debug("Param daar_n_of_probes == %d", daar_n_of_probes)
+    daar_probes_count = state.config[CONFIG_DAAR_PROBES_COUNT]
+    logger.debug("Param daar_probes_count == %d", daar_probes_count)
     daar_allowed_randomness = state.config[CONFIG_DAAR_ALLOWED_RANDOMNESS]
     logger.debug("Param daar_allowed_randomness == %f", daar_allowed_randomness)
     chaos_fun = state.config[CONFIG_CHAOS_FUN]
 
     group_index = state.values[VALUES_GROUP_INDEX]
     x = state.values[VALUES_X]
     x_counts = state.values[VALUES_X_COUNTS]
@@ -44,19 +44,19 @@
         logger.debug("Check if attr <%d> is better than shuffled", attr)
         if check_if_attr_better_than_shuffled(
             group_index=group_index,
             attr_values=x[:, attr],
             attr_values_count=x_counts[attr],
             values=y,
             values_count=y_count,
-            n_of_probes=daar_n_of_probes,
+            probes_count=daar_probes_count,
             allowed_randomness=daar_allowed_randomness,
             chaos_fun=chaos_fun,
             rng=state.rng,
         ):
             logger.debug(
                 "Attr <%d> is better than shuffled with respect to allowed_randomness",
                 attr,
             )
             result.append(attr)
-            break  # for current version we finish whenever the first one is found
+            break  # in this version we finish whenever the first one is found
     return np.asarray(result)
```

### Comparing `scikit_rough-0.0.1a2/src/skrough/algorithms/hooks/finalize_hooks.py` & `scikit_rough-0.1.0/src/skrough/algorithms/hooks/finalize_hooks.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from skrough.logs import log_start_end
 from skrough.structs.state import ProcessingState
 
 logger = logging.getLogger(__name__)
 
 
 @log_start_end(logger)
-def finalize_hook_choose_objs_random(
+def finalize_hook_choose_objs_randomly(
     state: ProcessingState,
 ) -> None:
     group_index = state.values[VALUES_GROUP_INDEX]
     y = state.values[VALUES_Y]
     y_count = state.values[VALUES_Y_COUNT]
     result_objs = choose_objects(
         group_index=group_index,
```

### Comparing `scikit_rough-0.0.1a2/src/skrough/algorithms/hooks/init_hooks.py` & `scikit_rough-0.1.0/src/skrough/algorithms/hooks/init_hooks.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """Init hook functions."""
 
 import logging
 
 from skrough.algorithms.key_names import (
     CONFIG_CHAOS_FUN,
     CONFIG_EPSILON,
+    CONFIG_SET_APPROX_THRESHOLD_TO_CURRENT,
     INPUT_DATA_X,
+    INPUT_DATA_X_COUNTS,
     INPUT_DATA_Y,
+    INPUT_DATA_Y_COUNT,
     VALUES_CHAOS_SCORE_APPROX_THRESHOLD,
     VALUES_CHAOS_SCORE_BASE,
     VALUES_CHAOS_SCORE_TOTAL,
     VALUES_GROUP_INDEX,
     VALUES_RESULT_ATTRS,
     VALUES_RESULT_OBJS,
     VALUES_X,
@@ -56,14 +59,25 @@
     y, y_count = prepare_factorized_vector(state.input_data[INPUT_DATA_Y])
     state.values[VALUES_X] = x
     state.values[VALUES_X_COUNTS] = x_counts
     state.values[VALUES_Y] = y
     state.values[VALUES_Y_COUNT] = y_count
 
 
+# TODO: add docstring
+@log_start_end(logger)
+def init_hook_pass_data(
+    state: ProcessingState,
+) -> None:
+    state.values[VALUES_X] = state.input_data[INPUT_DATA_X]
+    state.values[VALUES_X_COUNTS] = state.input_data[INPUT_DATA_X_COUNTS]
+    state.values[VALUES_Y] = state.input_data[INPUT_DATA_Y]
+    state.values[VALUES_Y_COUNT] = state.input_data[INPUT_DATA_Y_COUNT]
+
+
 # TODO: update docstring
 @log_start_end(logger)
 def init_hook_single_group_index(
     state: ProcessingState,
 ) -> None:
     """Init hook function to initialize a uniform group index structure.
 
@@ -120,15 +134,15 @@
     Args:
         state: An object representing the processing state.
     """
     state.values[VALUES_RESULT_ATTRS] = []
 
 
 @log_start_end(logger)
-def init_hook_approx_threshold(
+def init_hook_epsilon_approx_threshold(
     state: ProcessingState,
 ) -> None:
     chaos_stats = get_chaos_score_stats(
         x=state.values[VALUES_X],
         x_counts=state.values[VALUES_X_COUNTS],
         y=state.values[VALUES_Y],
         y_count=state.values[VALUES_Y_COUNT],
@@ -138,7 +152,21 @@
     state.values.update(
         {
             VALUES_CHAOS_SCORE_BASE: chaos_stats.base,
             VALUES_CHAOS_SCORE_TOTAL: chaos_stats.total,
             VALUES_CHAOS_SCORE_APPROX_THRESHOLD: chaos_stats.approx_threshold,
         }
     )
+
+
+@log_start_end(logger)
+def init_hook_current_approx_threshold(
+    state: ProcessingState,
+) -> None:
+    if state.config.get(CONFIG_SET_APPROX_THRESHOLD_TO_CURRENT) is True:
+        group_index: GroupIndex = state.values[VALUES_GROUP_INDEX]
+        approx_threshold = group_index.get_chaos_score(
+            values=state.values[VALUES_Y],
+            values_count=state.values[VALUES_Y_COUNT],
+            chaos_fun=state.config[CONFIG_CHAOS_FUN],
+        )
+        state.values.update({VALUES_CHAOS_SCORE_APPROX_THRESHOLD: approx_threshold})
```

### Comparing `scikit_rough-0.0.1a2/src/skrough/algorithms/hooks/inner_init_hooks.py` & `scikit_rough-0.1.0/src/skrough/algorithms/hooks/inner_init_hooks.py`

 * *Files identical despite different names*

### Comparing `scikit_rough-0.0.1a2/src/skrough/algorithms/hooks/inner_process_hooks.py` & `scikit_rough-0.1.0/src/skrough/algorithms/hooks/inner_process_hooks.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 
 import skrough.typing as rght
+from skrough.algorithms.hooks.helpers import check_if_below_approx_value_threshold
 from skrough.algorithms.key_names import (
     VALUES_GROUP_INDEX,
     VALUES_RESULT_ATTRS,
     VALUES_X,
     VALUES_X_COUNTS,
 )
 from skrough.logs import log_start_end
@@ -23,9 +24,27 @@
         attr = elements[0]
         elements = elements[1:]
         state.values[VALUES_RESULT_ATTRS].append(attr)
         group_index: GroupIndex = state.values[VALUES_GROUP_INDEX]
         state.values[VALUES_GROUP_INDEX] = group_index.split(
             values=state.values[VALUES_X][:, attr],
             values_count=state.values[VALUES_X_COUNTS][attr],
+            compress=True,
         )
     return elements
+
+
+def inner_process_hook_discard_first_attr_approx_threshold(
+    state: ProcessingState,
+    elements: rght.Elements,
+) -> rght.Elements:
+    attr = elements[0]
+    elements = elements[1:]
+    attrs_to_try = [a for a in state.values[VALUES_RESULT_ATTRS] if a != attr]
+    group_index = GroupIndex.from_data(
+        x=state.values[VALUES_X],
+        x_counts=state.values[VALUES_X_COUNTS],
+        attrs=attrs_to_try,
+    )
+    if check_if_below_approx_value_threshold(state, group_index):
+        state.values[VALUES_RESULT_ATTRS] = attrs_to_try
+    return elements
```

### Comparing `scikit_rough-0.0.1a2/src/skrough/algorithms/hooks/pre_candidates_hooks.py` & `scikit_rough-0.1.0/src/skrough/algorithms/hooks/pre_candidates_hooks.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,7 +18,14 @@
     pre_candidates: np.ndarray = np.delete(
         np.arange(state.values[VALUES_X].shape[1]),
         state.values[VALUES_RESULT_ATTRS],
     )
     if len(pre_candidates) == 0:
         raise LoopBreak("No remaining attrs")
     return pre_candidates
+
+
+@log_start_end(logger)
+def pre_candidates_hook_result_attrs(
+    state: ProcessingState,
+) -> rght.Elements:
+    return state.values[VALUES_RESULT_ATTRS]
```

### Comparing `scikit_rough-0.0.1a2/src/skrough/algorithms/hooks/prepare_result_hooks.py` & `scikit_rough-0.1.0/src/skrough/algorithms/hooks/prepare_result_hooks.py`

 * *Files identical despite different names*

### Comparing `scikit_rough-0.0.1a2/src/skrough/algorithms/hooks/select_hooks.py` & `scikit_rough-0.1.0/src/skrough/algorithms/hooks/select_hooks.py`

 * *Files identical despite different names*

### Comparing `scikit_rough-0.0.1a2/src/skrough/algorithms/hooks/stop_hooks.py` & `scikit_rough-0.1.0/src/skrough/algorithms/hooks/stop_hooks.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 import logging
 
+from skrough.algorithms.hooks.helpers import check_if_below_approx_value_threshold
 from skrough.algorithms.key_names import (
-    CONFIG_CHAOS_FUN,
     CONFIG_CONSECUTIVE_EMPTY_ITERATIONS_MAX_COUNT,
     CONFIG_RESULT_ATTRS_MAX_COUNT,
-    VALUES_CHAOS_SCORE_APPROX_THRESHOLD,
     VALUES_CONSECUTIVE_EMPTY_ITERATIONS_COUNT,
     VALUES_GROUP_INDEX,
     VALUES_RESULT_ATTRS,
-    VALUES_Y,
-    VALUES_Y_COUNT,
 )
 from skrough.logs import log_start_end
 from skrough.structs.group_index import GroupIndex
 from skrough.structs.state import ProcessingState
 
 logger = logging.getLogger(__name__)
 
@@ -57,29 +54,18 @@
         state: State object that holds the computation's state.
 
     Returns:
         Indication whether the chaos score computed for the current group index falls
         below the defined chaos score approximation threshold.
     """
     group_index: GroupIndex = state.values[VALUES_GROUP_INDEX]
-    current_chaos_score = group_index.get_chaos_score(
-        values=state.values[VALUES_Y],
-        values_count=state.values[VALUES_Y_COUNT],
-        chaos_fun=state.config[CONFIG_CHAOS_FUN],
-    )
-    approx_chaos_score_value_threshold = state.values[
-        VALUES_CHAOS_SCORE_APPROX_THRESHOLD
-    ]
-    logger.debug("current_chaos_score = %f", current_chaos_score)
-    logger.debug(
-        "approx_chaos_score_value_threshold = %f", approx_chaos_score_value_threshold
-    )
-    return bool(current_chaos_score <= approx_chaos_score_value_threshold)
+    return check_if_below_approx_value_threshold(state, group_index)
 
 
+# TODO: add description for max_count == None ~ no limit
 @log_start_end(logger)
 def stop_hook_attrs_count(
     state: ProcessingState,
 ) -> bool:
     """Stop check based on a number of result attrs.
 
     Stop check based on a number of result attrs. The function implements a simple check
@@ -91,18 +77,22 @@
 
     Args:
         state: State object that holds a computation's state.
 
     Returns:
         Indication whether the computation should stop.
     """
-    return bool(
-        len(state.values[VALUES_RESULT_ATTRS])
-        >= state.config[CONFIG_RESULT_ATTRS_MAX_COUNT]
-    )
+    result = False
+    attrs_max_count = state.config.get(CONFIG_RESULT_ATTRS_MAX_COUNT)
+    if attrs_max_count is not None:
+        result = bool(
+            len(state.values[VALUES_RESULT_ATTRS])
+            >= state.config[CONFIG_RESULT_ATTRS_MAX_COUNT]
+        )
+    return result
 
 
 @log_start_end(logger)
 def stop_hook_empty_iterations(
     state: ProcessingState,
 ) -> bool:
     """Stop check based on a number of empty iterations.
@@ -125,7 +115,14 @@
     Returns:
         Indication whether the computation should stop.
     """
     return bool(
         state.values.get(VALUES_CONSECUTIVE_EMPTY_ITERATIONS_COUNT, 0)
         >= state.config[CONFIG_CONSECUTIVE_EMPTY_ITERATIONS_MAX_COUNT]
     )
+
+
+@log_start_end(logger)
+def stop_hook_never(
+    state: ProcessingState,  # pylint: disable=unused-argument
+) -> bool:
+    return False
```

### Comparing `scikit_rough-0.0.1a2/src/skrough/algorithms/key_names.py` & `scikit_rough-0.1.0/src/skrough/algorithms/key_names.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,37 +10,49 @@
 VALUES_KEYS_DOCSTRING_REGEX = "VALUES_\\w*"
 
 
 INPUT_DATA_X = "input_data_x"
 """A key used to reference the input data table representing conditional
 features/attributes in ProcessingState.input_data."""
 
+INPUT_DATA_X_COUNTS = "input_data_x_counts"
+"""A key used to reference the input data table domain sizes in
+ProcessingState.input_data."""
+
 INPUT_DATA_Y = "input_data_y"
-"""A key used to reference the decision values in ProcessingState.input_data."""
+"""A key used to reference the input decision values in ProcessingState.input_data."""
+
+INPUT_DATA_Y_COUNT = "input_data_y_count"
+"""A key used to reference the input decision values domain size in
+ProcessingState.input_data."""
 
-CONFIG_CANDIDATES_MAX_COUNT = "config_candidates_max_count"
 CONFIG_CHAOS_FUN = "config_chaos_fun"
 """A key used to reference the chaos measure function to be used."""
 
 CONFIG_CONSECUTIVE_EMPTY_ITERATIONS_MAX_COUNT = (
     "config_consecutive_empty_iterations_max_count"
 )
 CONFIG_DAAR_ALLOWED_RANDOMNESS = "config_daar_allowed_randomness"
-CONFIG_DAAR_N_OF_PROBES = "config_daar_n_of_probes"
+CONFIG_DAAR_PROBES_COUNT = "config_daar_probes_count"
 CONFIG_EPSILON = "config_epsilon"
 CONFIG_SELECT_ATTRS_CHAOS_SCORE_BASED_MAX_COUNT = (
     "config_select_attrs_chaos_score_based_max_count"
 )
-CONFIG_SELECT_RANDOM_MAX_COUNT = "config_select_attrs_random_max_count"
+CONFIG_CANDIDATES_SELECT_RANDOM_MAX_COUNT = "config_candidates_select_random_max_count"
 """A key used to reference the max number of randomly selected candidate elements."""
 
 CONFIG_RESULT_ATTRS_MAX_COUNT = "config_result_attrs_max_count"
 """A key used to reference the max number of attrs in the results."""
 
-VALUES_CHAOS_SCORE_APPROX_THRESHOLD = "values_chaos_score_approx_value_threshold"
+CONFIG_SET_APPROX_THRESHOLD_TO_CURRENT = "config_set_approx_threshold_to_current"
+"""A key used to control the hook that sets approx threshold available under
+ProcessingState.values['VALUES_CHAOS_SCORE_APPROX_THRESHOLD'] to the value resulting
+from the current group index and decision values."""
+
+VALUES_CHAOS_SCORE_APPROX_THRESHOLD = "values_chaos_score_approx_threshold"
 """A key used to reference the chaos score approximation threshold."""
 
 VALUES_CHAOS_SCORE_BASE = "values_chaos_score_base"
 """A key used to reference the chaos score base value."""
 
 VALUES_CHAOS_SCORE_TOTAL = "values_chaos_score_total"
 """A key used to reference the chaos score total value."""
```

### Comparing `scikit_rough-0.0.1a2/src/skrough/algorithms/meta/aggregates.py` & `scikit_rough-0.1.0/src/skrough/algorithms/meta/aggregates.py`

 * *Files identical despite different names*

### Comparing `scikit_rough-0.0.1a2/src/skrough/algorithms/meta/describe.py` & `scikit_rough-0.1.0/src/skrough/algorithms/meta/describe.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,17 +169,15 @@
         # in case of the docstring parsing - we also need to decode key names used
         # commonly in docstring descriptions, i.e., constant names from
         # skrough.algorithms.key_names, to actual keys
         result = list(filter(None, [getattr(key_names, name, None) for name in result]))
     return result
 
 
-def inspect_config_keys(
-    processing_element,
-) -> List[str]:
+def inspect_config_keys(processing_element) -> List[str]:
     return _inspect_keys(
         processing_element,
         key_method_name=rght.Describable.get_config_keys.__name__,
         regex_pattern=CONFIG_KEYS_DOCSTRING_REGEX,
     )
```

### Comparing `scikit_rough-0.0.1a2/src/skrough/algorithms/meta/helpers.py` & `scikit_rough-0.1.0/src/skrough/algorithms/meta/helpers.py`

 * *Files identical despite different names*

### Comparing `scikit_rough-0.0.1a2/src/skrough/algorithms/meta/processing.py` & `scikit_rough-0.1.0/src/skrough/algorithms/meta/processing.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 # pylint: disable=duplicate-code
 
+from __future__ import annotations
+
 import logging
-from typing import Any, List, Optional, Sequence
+from typing import Any, Sequence, cast
 
+import joblib
 import numpy as np
 from attrs import define
 from sklearn.base import BaseEstimator
 
 import skrough.typing as rght
+from skrough.algorithms.constants import RNG_INTEGERS_PARAM
 from skrough.algorithms.meta.aggregates import UpdateStateHooksAggregate
 from skrough.algorithms.meta.describe import (
     autogenerate_description_node,
     describe,
     inspect_config_keys,
     inspect_input_data_keys,
     inspect_values_keys,
@@ -39,37 +43,36 @@
     _sk_visual_block_ = sk_visual_block
 
     @classmethod
     @log_start_end(logger)
     def from_hooks(
         cls,
         prepare_result_fun: rght.PrepareResultFunction,
-        init_multi_stage_hooks: Optional[
-            rght.OneOrSequence[rght.UpdateStateHook]
-        ] = None,
-        init_hooks: Optional[rght.OneOrSequence[rght.UpdateStateHook]] = None,
-        stages: Optional[rght.OneOrSequence[Stage]] = None,
-        finalize_hooks: Optional[rght.OneOrSequence[rght.UpdateStateHook]] = None,
+        init_multi_stage_hooks: None
+        | (rght.OneOrSequence[rght.UpdateStateHook]) = None,
+        init_hooks: rght.OneOrSequence[rght.UpdateStateHook] | None = None,
+        stages: rght.OneOrSequence[Stage] | None = None,
+        finalize_hooks: rght.OneOrSequence[rght.UpdateStateHook] | None = None,
     ):
         return cls(
             init_multi_stage_agg=UpdateStateHooksAggregate.from_hooks(
                 init_multi_stage_hooks
             ),
             init_agg=UpdateStateHooksAggregate.from_hooks(init_hooks),
             stages=normalize_sequence(stages, optional=True),
             finalize_agg=UpdateStateHooksAggregate.from_hooks(finalize_hooks),
             prepare_result_fun=prepare_result_fun,
         )
 
     @log_start_end(logger)
     def __call__(
         self,
-        state: Optional[ProcessingState] = None,
-        input_data: Optional[StateInputData] = None,
-        config: Optional[StateConfig] = None,
+        state: ProcessingState | None = None,
+        input_data: StateInputData | None = None,
+        config: StateConfig | None = None,
         seed: rght.Seed = None,
     ) -> Any:
         logger.debug("Create state object")
         if state is None:
             logger.debug("No state passed, create new one from config, input and seed")
             state = ProcessingState.from_optional(
                 rng=np.random.default_rng(seed),
@@ -91,14 +94,36 @@
         logger.debug("Run finalize hooks")
         self.finalize_agg(state)
 
         logger.debug("Prepare result function")
         result = self.prepare_result_fun(state)
         return result
 
+    @log_start_end(logger)
+    def call_parallel(
+        self,
+        n_times: int,
+        state: ProcessingState | None = None,
+        input_data: StateInputData | None = None,
+        config: StateConfig | None = None,
+        seed: rght.Seed = None,
+        n_jobs: int | None = None,
+    ) -> list[Any]:
+        rng = np.random.default_rng(seed)
+        result = joblib.Parallel(n_jobs=n_jobs)(
+            joblib.delayed(self)(
+                state=state,
+                input_data=input_data,
+                config=config,
+                seed=rng.integers(RNG_INTEGERS_PARAM),
+            )
+            for _ in range(n_times)
+        )
+        return cast(list[Any], result)
+
     def get_description_graph(self):
         result = autogenerate_description_node(
             processing_element=self, process_docstring=True
         )
         result.children = [
             describe(
                 self.init_multi_stage_agg,
@@ -129,24 +154,24 @@
             self.init_multi_stage_agg,
             self.init_agg,
             *self.stages,
             self.finalize_agg,
             self.prepare_result_fun,
         ]
 
-    def get_config_keys(self) -> List[str]:
+    def get_config_keys(self) -> list[str]:
         return self._get_keys_from_elements(
             children=self._get_children_processing_elements(),
             inspect_keys_function=inspect_config_keys,
         )
 
-    def get_input_data_keys(self) -> List[str]:
+    def get_input_data_keys(self) -> list[str]:
         return self._get_keys_from_elements(
             children=self._get_children_processing_elements(),
             inspect_keys_function=inspect_input_data_keys,
         )
 
-    def get_values_keys(self) -> List[str]:
+    def get_values_keys(self) -> list[str]:
         return self._get_keys_from_elements(
             children=self._get_children_processing_elements(),
             inspect_keys_function=inspect_values_keys,
         )
```

### Comparing `scikit_rough-0.0.1a2/src/skrough/algorithms/meta/stage.py` & `scikit_rough-0.1.0/src/skrough/algorithms/meta/stage.py`

 * *Files identical despite different names*

### Comparing `scikit_rough-0.0.1a2/src/skrough/algorithms/meta/visual_block.py` & `scikit_rough-0.1.0/src/skrough/algorithms/meta/visual_block.py`

 * *Files identical despite different names*

### Comparing `scikit_rough-0.0.1a2/src/skrough/algorithms/reduct_ordering.py` & `scikit_rough-0.1.0/src/skrough/algorithms/reduct_ordering.py`

 * *Files identical despite different names*

### Comparing `scikit_rough-0.0.1a2/src/skrough/attrs_checks.py` & `scikit_rough-0.1.0/src/skrough/attrs_checks.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,41 +15,41 @@
 @log_start_end(logger)
 def check_if_attr_better_than_shuffled(
     group_index: GroupIndex,
     attr_values: np.ndarray,
     attr_values_count: int,
     values: np.ndarray,
     values_count: int,
-    n_of_probes: int,
+    probes_count: int,
     allowed_randomness: float,
     chaos_fun: rght.ChaosMeasure,
     rng: np.random.Generator,
     smoothing_parameter: float = DEFAULT_SMOOTHING_PARAMETER,
 ) -> bool:
     attr_chaos_score = group_index.get_chaos_score_after_split(
         attr_values,
         attr_values_count,
         values,
         values_count,
         chaos_fun,
     )
     attr_is_better_count = 0
-    for _ in range(n_of_probes):
+    for _ in range(probes_count):
         attr_values_shuffled = rng.permutation(attr_values)
         shuffled_chaos_score = group_index.get_chaos_score_after_split(
             attr_values_shuffled,
             attr_values_count,
             values,
             values_count,
             chaos_fun,
         )
-        attr_is_better_count += int(attr_chaos_score <= shuffled_chaos_score)
+        attr_is_better_count += int(attr_chaos_score < shuffled_chaos_score)
 
     smoothing_dims = 2  # binomial distribution, i.e., better/worse
     attr_probe_score = (attr_is_better_count + smoothing_parameter) / (
-        n_of_probes + smoothing_parameter * smoothing_dims
+        probes_count + smoothing_parameter * smoothing_dims
     )
     logger.debug("attr_probe_score == %f", attr_probe_score)
     logger.debug("allowed_randomness == %f", allowed_randomness)
     logger.debug("attr_probe_threshold == %f", (1 - allowed_randomness))
 
     return attr_probe_score >= (1 - allowed_randomness)
```

### Comparing `scikit_rough-0.0.1a2/src/skrough/chaos_measures/chaos_measures.py` & `scikit_rough-0.1.0/src/skrough/chaos_measures/chaos_measures.py`

 * *Files identical despite different names*

### Comparing `scikit_rough-0.0.1a2/src/skrough/chaos_measures/gini_impurity_cython.pyx` & `scikit_rough-0.1.0/src/skrough/chaos_measures/gini_impurity_cython.pyx`

 * *Files identical despite different names*

### Comparing `scikit_rough-0.0.1a2/src/skrough/chaos_score.py` & `scikit_rough-0.1.0/src/skrough/chaos_score.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,23 +166,25 @@
     increment_attrs_chaos_score = None
     attrs_added: Set[int] = set()
     if increment_attrs is not None:
         increment_attrs_chaos_score = []
         for attrs in increment_attrs:
             attrs_to_add = set(attrs) - attrs_added
             for attr in attrs_to_add:
-                group_index = group_index.split(x[:, attr], x_counts[attr])
+                group_index = group_index.split(
+                    x[:, attr], x_counts[attr], compress=True
+                )
             attrs_added = attrs_added.union(attrs_to_add)
             chaos_score = group_index.get_chaos_score(y, y_count, chaos_fun)
             increment_attrs_chaos_score.append(chaos_score)
 
     # add remaining attrs
     attrs_other = set(range(x.shape[1])) - attrs_added
     for attr in attrs_other:
-        group_index = group_index.split(x[:, attr], x_counts[attr])
+        group_index = group_index.split(x[:, attr], x_counts[attr], compress=True)
 
     # compute total chaos score
     total_chaos_score = group_index.get_chaos_score(y, y_count, chaos_fun)
 
     approx_threshold = None
     if epsilon is not None:
         delta_dependency = base_chaos_score - total_chaos_score
```

### Comparing `scikit_rough-0.0.1a2/src/skrough/checks.py` & `scikit_rough-0.1.0/src/skrough/checks.py`

 * *Files identical despite different names*

### Comparing `scikit_rough-0.0.1a2/src/skrough/dataprep.py` & `scikit_rough-0.1.0/src/skrough/dataprep.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,17 +9,21 @@
 
 import numpy as np
 import pandas as pd
 
 import skrough.typing as rght
 from skrough.logs import log_start_end
 
+DEFAULT_SHUFFLED_PREFIX = "shuffled_"
+
+
 logger = logging.getLogger(__name__)
 
 
+# TODO: add handling also for pd.Series
 @log_start_end(logger)
 def prepare_factorized_vector(values: np.ndarray) -> Tuple[np.ndarray, int]:
     """Factorize values.
 
     Prepare enumerated values along with a number of distinct values.
 
     Args:
@@ -37,14 +41,15 @@
         (array([0, 1, 0, 0, 2]), 3)
     """
     factorized_values, uniques = pd.factorize(values, use_na_sentinel=False)
     count_distinct = len(uniques)
     return factorized_values, count_distinct
 
 
+# TODO: add handling also for pd.DataFrame
 @log_start_end(logger)
 def prepare_factorized_array(
     data_x: np.ndarray,
 ) -> Tuple[np.ndarray, np.ndarray]:
     """Factorize data table.
 
     Factorize data table and return statistics of feature domain sizes.
@@ -118,50 +123,52 @@
     data_y = df[target_attr]
     data_x = df.drop(columns=target_attr)
     x, x_counts = prepare_factorized_array(data_x.to_numpy())
     y, y_count = prepare_factorized_vector(data_y.to_numpy())
     return x, x_counts, y, y_count
 
 
+# TODO: make target_attr optional - so one can shuffle just conditional attrs without
+# the need the target attr to be present
 @log_start_end(logger)
-def add_shadow_attrs(
+def add_shuffled_attrs(
     df: pd.DataFrame,
     target_attr: Union[str, int],
-    shadow_attrs_prefix: str = "shadow_",
+    shuffled_attrs_prefix: str = DEFAULT_SHUFFLED_PREFIX,
     seed: rght.Seed = None,
 ) -> pd.DataFrame:
-    """Add shadow attrs.
+    """Add shuffled attrs.
 
-    Add shadow counterpart attribute for each conditional attribute (for all but one
-    distinguished target attribute) of the input dataset. A shadow (reordered) attribute
-    for a given original attribute consists of the same values but shuffled in random
-    order. In other words, a shadow attribute is an attribute of the same empirical
-    distribution as the original one but (possibly) uncorrelated with the target
-    attribute.
+    Add shuffled counterpart attribute for each conditional attribute (for all but one
+    distinguished target attribute) of the input dataset. A shuffled (reordered)
+    attribute for a given original attribute consists of the same values but permuted in
+    random order. In other words, a shuffled attribute is an attribute of the same
+    empirical distribution as the original one but (possibly) uncorrelated with the
+    target attribute.
 
     Args:
         df: Input dataset.
         target_attr: Identifier of the target column in the input dataset.
-        shadow_attrs_prefix: A prefix for shadow attribute names.
+        shuffled_attrs_prefix: A prefix for shuffled attribute names.
         seed: Random seed. Defaults to :obj:`None`.
 
     Returns:
-        A dataset with shadow counterpart attributes added.
+        A dataset with shuffled counterpart attributes added.
 
     Examples:
         >>> df = pd.DataFrame([[5, 3, 3],
         ...                    [9, 3, 1],
-        ...                    [5, 2, 3]], columns=["a", "b", "dec"])
-        >>> add_shadow_attrs(df, target_attr="dec", shadow_attrs_prefix="s_", seed=0)
+        ...                    [5, 2, 3]], columns=["a", "b", "d"])
+        >>> add_shuffled_attrs(df, target_attr="d", shuffled_attrs_prefix="s_", seed=0)
            a  b  s_a  s_b  dec
         0  5  3    5    2    3
         1  9  3    5    3    1
         2  5  2    9    3    3
     """
     rng = np.random.default_rng(seed)
     data_y = df[target_attr]
     data_x = df.drop(columns=target_attr)
-    data_x_shadow = data_x.apply(rng.permutation)
-    col_names = list(shadow_attrs_prefix + data_x_shadow.columns.astype(str))
-    data_x_shadow.columns = col_names
-    result = pd.concat([data_x, data_x_shadow, data_y], axis=1)
+    data_x_shuffled = data_x.apply(rng.permutation)
+    col_names = list(shuffled_attrs_prefix + data_x_shuffled.columns.astype(str))
+    data_x_shuffled.columns = col_names
+    result = pd.concat([data_x, data_x_shuffled, data_y], axis=1)
     return result
```

### Comparing `scikit_rough-0.0.1a2/src/skrough/estimators/base.py` & `scikit_rough-0.1.0/src/skrough/estimators/base.py`

 * *Files identical despite different names*

### Comparing `scikit_rough-0.0.1a2/src/skrough/homogeneity.py` & `scikit_rough-0.1.0/src/skrough/homogeneity.py`

 * *Files identical despite different names*

### Comparing `scikit_rough-0.0.1a2/src/skrough/instances.py` & `scikit_rough-0.1.0/src/skrough/instances.py`

 * *Files identical despite different names*

### Comparing `scikit_rough-0.0.1a2/src/skrough/logs.py` & `scikit_rough-0.1.0/src/skrough/logs.py`

 * *Files identical despite different names*

### Comparing `scikit_rough-0.0.1a2/src/skrough/permutations.py` & `scikit_rough-0.1.0/src/skrough/permutations.py`

 * *Files identical despite different names*

### Comparing `scikit_rough-0.0.1a2/src/skrough/rough.py` & `scikit_rough-0.1.0/src/skrough/rough.py`

 * *Files identical despite different names*

### Comparing `scikit_rough-0.0.1a2/src/skrough/structs/attrs_subset.py` & `scikit_rough-0.1.0/src/skrough/structs/attrs_subset.py`

 * *Files identical despite different names*

### Comparing `scikit_rough-0.0.1a2/src/skrough/structs/chaos_score_stats.py` & `scikit_rough-0.1.0/src/skrough/structs/chaos_score_stats.py`

 * *Files identical despite different names*

### Comparing `scikit_rough-0.0.1a2/src/skrough/structs/description_node.py` & `scikit_rough-0.1.0/src/skrough/structs/description_node.py`

 * *Files identical despite different names*

### Comparing `scikit_rough-0.0.1a2/src/skrough/structs/group_index.py` & `scikit_rough-0.1.0/src/skrough/structs/group_index.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
         if len(values) != self.n_objs:
             raise ValueError("Values vector length does not match the group index")
 
     def split(
         self,
         values: npt.NDArray[np.int64],
         values_count: int,
-        compress: bool = True,
+        compress: bool = False,
     ) -> "GroupIndex":
         """
         Split groups of objects into finer groups according to values on
         a single splitting attribute
 
         It is up to the user to ensure that ``values_count`` correctly represents
         ``values``. Otherwise, the behavior is unspecified.
@@ -189,9 +189,9 @@
         self,
         split_values: npt.NDArray[np.int64],
         split_values_count: int,
         values: npt.NDArray[np.int64],
         values_count: int,
         chaos_fun: rght.ChaosMeasure,
     ):
-        split_group_index = self.split(split_values, split_values_count)
+        split_group_index = self.split(split_values, split_values_count, compress=False)
         return split_group_index.get_chaos_score(values, values_count, chaos_fun)
```

### Comparing `scikit_rough-0.0.1a2/src/skrough/structs/objs_attrs_subset.py` & `scikit_rough-0.1.0/src/skrough/structs/objs_attrs_subset.py`

 * *Files identical despite different names*

### Comparing `scikit_rough-0.0.1a2/src/skrough/structs/state.py` & `scikit_rough-0.1.0/src/skrough/structs/state.py`

 * *Files identical despite different names*

### Comparing `scikit_rough-0.0.1a2/src/skrough/typing.py` & `scikit_rough-0.1.0/src/skrough/typing.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,87 +32,106 @@
     T,
     Sequence[T],
 ]
 
 
 # Predict strategy
 class PredictStrategyFunction(Protocol):
-    @staticmethod
+    @abc.abstractmethod
     def __call__(
+        self,
         reference_ids: np.ndarray,
-        reference_y: np.ndarray,
+        reference_data_y: np.ndarray,
         predict_ids: np.ndarray,
-        seed: Seed,
+        seed: Seed = None,
+    ) -> Any:
+        raise NotImplementedError
+
+
+# no-answer strategy - what should be the answer when a classifier "do not know"
+class NoAnswerStrategyFunction(Protocol):
+    @abc.abstractmethod
+    def __call__(
+        self,
+        reference_data_y: np.ndarray,
+        seed: Seed = None,
     ) -> Any:
-        ...
+        raise NotImplementedError
 
 
 # Permutation strategy
 class ObjsAttrsPermutationStrategyFunction(Protocol):
     @staticmethod
+    @abc.abstractmethod
     def __call__(
         n_objs: int,
         n_attrs: int,
         objs_weights: Optional[Union[int, float, np.ndarray]] = None,
         attrs_weights: Optional[Union[int, float, np.ndarray]] = None,
         rng: Seed = None,
     ) -> Any:
-        ...
+        raise NotImplementedError
 
 
 # Processing/stage functions
 class PrepareResultFunction(Protocol):
     @staticmethod
+    @abc.abstractmethod
     def __call__(
         state: ProcessingState,
     ) -> Any:
-        ...
+        raise NotImplementedError
 
 
 # Hook functions - to be composed/aggregated into processing/stage functions
 class StopHook(Protocol):
     @staticmethod
+    @abc.abstractmethod
     def __call__(
         state: ProcessingState,
     ) -> bool:
-        ...
+        raise NotImplementedError
 
 
 class InnerStopHook(Protocol):
     @staticmethod
+    @abc.abstractmethod
     def __call__(
         state: ProcessingState,
         elements: Elements,
     ) -> bool:
-        ...
+        raise NotImplementedError
 
 
 class UpdateStateHook(Protocol):
     @staticmethod
+    @abc.abstractmethod
     def __call__(
         state: ProcessingState,
     ) -> None:
-        ...
+        raise NotImplementedError
 
 
 class ProduceElementsHook(Protocol):
     @staticmethod
+    @abc.abstractmethod
     def __call__(
         state: ProcessingState,
     ) -> Elements:
-        ...
+        raise NotImplementedError
 
 
 class ProcessElementsHook(Protocol):
     @staticmethod
+    @abc.abstractmethod
     def __call__(
         state: ProcessingState,
         elements: Elements,
     ) -> Elements:
-        ...
+        raise NotImplementedError
 
 
 # Describable
 class Describable(abc.ABC):
     @abc.abstractmethod
     def get_description_graph(self) -> DescriptionNode:
         """Get a description graph.
```

### Comparing `scikit_rough-0.0.1a2/src/skrough/unify.py` & `scikit_rough-0.1.0/src/skrough/unify.py`

 * *Files identical despite different names*

### Comparing `scikit_rough-0.0.1a2/src/skrough/unique.py` & `scikit_rough-0.1.0/src/skrough/unique.py`

 * *Files identical despite different names*

### Comparing `scikit_rough-0.0.1a2/src/skrough/utils.py` & `scikit_rough-0.1.0/src/skrough/utils.py`

 * *Files identical despite different names*

### Comparing `scikit_rough-0.0.1a2/src/skrough/weights.py` & `scikit_rough-0.1.0/src/skrough/weights.py`

 * *Files identical despite different names*

### Comparing `scikit_rough-0.0.1a2/setup.py` & `scikit_rough-0.1.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,48 +1,46 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: scikit-rough
+Version: 0.1.0
+Summary: 
+License: MIT
+Author: sebov
+Author-email: 12091011+sebov@users.noreply.github.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: attrs (>=23.1.0,<24.0.0)
+Requires-Dist: docstring-parser (>=0.15,<0.16)
+Requires-Dist: joblib (>=1.1.0,<2.0.0)
+Requires-Dist: more-itertools (>=8.14.0,<9.0.0)
+Requires-Dist: numba (>=0.56.0,<0.57.0)
+Requires-Dist: numpy (>=1.22.4,<2.0.0)
+Requires-Dist: pandas (>=2.0.0,<3.0.0)
+Requires-Dist: scikit-learn (>=1.1.1,<2.0.0)
+Description-Content-Type: text/markdown
+
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Documentation Status](https://readthedocs.org/projects/scikit-rough/badge/?version=latest)](https://scikit-rough.readthedocs.io/en/latest/)
+
+
+[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=sebov_scikit-rough&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=sebov_scikit-rough)
+[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=sebov_scikit-rough&metric=coverage)](https://sonarcloud.io/summary/new_code?id=sebov_scikit-rough)
+[![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=sebov_scikit-rough&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=sebov_scikit-rough)
+[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=sebov_scikit-rough&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=sebov_scikit-rough)
+[![Total alerts](https://img.shields.io/lgtm/alerts/g/sebov/scikit-rough.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/sebov/scikit-rough/alerts/)
+[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/sebov/scikit-rough.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/sebov/scikit-rough/context:python)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/a1e1457efb4b4b5da569b9c9881f1ca9)](https://www.codacy.com/gh/sebov/scikit-rough/dashboard?utm_source=github.com&utm_medium=referral&utm_content=sebov/scikit-rough&utm_campaign=Badge_Grade)
+[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/a1e1457efb4b4b5da569b9c9881f1ca9)](https://www.codacy.com/gh/sebov/scikit-rough/dashboard?utm_source=github.com&utm_medium=referral&utm_content=sebov/scikit-rough&utm_campaign=Badge_Coverage)
 
-package_dir = \
-{'': 'src'}
+# scikit-rough
 
-packages = \
-['skrough',
- 'skrough.algorithms',
- 'skrough.algorithms.hooks',
- 'skrough.algorithms.hooks.common',
- 'skrough.algorithms.meta',
- 'skrough.chaos_measures',
- 'skrough.estimators',
- 'skrough.structs']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['attrs>=22.0.1,<23.0.0',
- 'docstring-parser>=0.15,<0.16',
- 'joblib>=1.1.0,<2.0.0',
- 'more-itertools>=8.14.0,<9.0.0',
- 'numba>=0.56.0,<0.57.0',
- 'numpy>=1.22.4,<2.0.0',
- 'pandas>=1.4.2,<2.0.0',
- 'scikit-learn>=1.1.1,<2.0.0']
-
-setup_kwargs = {
-    'name': 'scikit-rough',
-    'version': '0.0.1a2',
-    'description': '',
-    'long_description': '[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)\n[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Documentation Status](https://readthedocs.org/projects/scikit-rough/badge/?version=latest)](https://scikit-rough.readthedocs.io/en/latest/)\n\n\n[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=sebov_scikit-rough&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=sebov_scikit-rough)\n[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=sebov_scikit-rough&metric=coverage)](https://sonarcloud.io/summary/new_code?id=sebov_scikit-rough)\n[![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=sebov_scikit-rough&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=sebov_scikit-rough)\n[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=sebov_scikit-rough&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=sebov_scikit-rough)\n[![Total alerts](https://img.shields.io/lgtm/alerts/g/sebov/scikit-rough.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/sebov/scikit-rough/alerts/)\n[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/sebov/scikit-rough.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/sebov/scikit-rough/context:python)\n[![Codacy Badge](https://app.codacy.com/project/badge/Grade/a1e1457efb4b4b5da569b9c9881f1ca9)](https://www.codacy.com/gh/sebov/scikit-rough/dashboard?utm_source=github.com&utm_medium=referral&utm_content=sebov/scikit-rough&utm_campaign=Badge_Grade)\n[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/a1e1457efb4b4b5da569b9c9881f1ca9)](https://www.codacy.com/gh/sebov/scikit-rough/dashboard?utm_source=github.com&utm_medium=referral&utm_content=sebov/scikit-rough&utm_campaign=Badge_Coverage)\n\n# scikit-rough\n\n**scikit-rough** is a Python package/toolbox of algorithms and functions for data analysis\nbased on the rough set theory\n\nRead [scikit-rough documentation](https://scikit-rough.readthedocs.io/).\n',
-    'author': 'sebov',
-    'author_email': '12091011+sebov@users.noreply.github.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.12',
-}
+**scikit-rough** is a Python package/toolbox of algorithms and functions for data analysis
+based on the rough set theory
 
+Read [scikit-rough documentation](https://scikit-rough.readthedocs.io/).
 
-setup(**setup_kwargs)
```

