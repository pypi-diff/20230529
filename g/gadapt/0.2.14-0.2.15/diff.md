# Comparing `tmp/gadapt-0.2.14.tar.gz` & `tmp/gadapt-0.2.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gadapt-0.2.14.tar", last modified: Sun May 28 17:26:21 2023, max compression
+gzip compressed data, was "dist\gadapt-0.2.15.tar", last modified: Mon May 29 08:33:50 2023, max compression
```

## Comparing `gadapt-0.2.14.tar` & `gadapt-0.2.15.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.202414 gadapt-0.2.14/
--rw-rw-rw-   0        0        0      320 2023-05-28 17:26:21.202914 gadapt-0.2.14/PKG-INFO
--rw-rw-rw-   0        0        0    19350 2023-05-28 15:29:08.000000 gadapt-0.2.14/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.018915 gadapt-0.2.14/gadapt/
--rw-rw-rw-   0        0        0        2 2023-05-24 06:11:19.000000 gadapt-0.2.14/gadapt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.045914 gadapt-0.2.14/gadapt/cost_finding/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:14:46.000000 gadapt-0.2.14/gadapt/cost_finding/__init__.py
--rw-rw-rw-   0        0        0      728 2023-05-24 06:38:53.000000 gadapt-0.2.14/gadapt/cost_finding/base_cost_finder.py
--rw-rw-rw-   0        0        0     2112 2023-05-24 06:54:25.000000 gadapt-0.2.14/gadapt/cost_finding/common_cost_finder.py
-drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.050913 gadapt-0.2.14/gadapt/crossover/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:14:39.000000 gadapt-0.2.14/gadapt/crossover/__init__.py
--rw-rw-rw-   0        0        0     7034 2023-05-28 13:24:31.000000 gadapt-0.2.14/gadapt/crossover/base_crossover.py
--rw-rw-rw-   0        0        0     1257 2023-05-23 23:45:14.000000 gadapt-0.2.14/gadapt/crossover/uniform_crossover.py
-drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.052914 gadapt-0.2.14/gadapt/execution/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:14:34.000000 gadapt-0.2.14/gadapt/execution/__init__.py
--rw-rw-rw-   0        0        0     3233 2023-05-27 11:13:47.000000 gadapt-0.2.14/gadapt/execution/ga_executor.py
-drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.059915 gadapt-0.2.14/gadapt/exit_check/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:14:29.000000 gadapt-0.2.14/gadapt/exit_check/__init__.py
--rw-rw-rw-   0        0        0      315 2023-05-23 23:28:45.000000 gadapt-0.2.14/gadapt/exit_check/avg_cost_exit_checker.py
--rw-rw-rw-   0        0        0     1060 2023-05-24 06:38:53.000000 gadapt-0.2.14/gadapt/exit_check/base_exit_checker.py
--rw-rw-rw-   0        0        0      305 2023-05-23 23:28:54.000000 gadapt-0.2.14/gadapt/exit_check/min_cost_exit_checker.py
--rw-rw-rw-   0        0        0      387 2023-05-23 23:29:00.000000 gadapt-0.2.14/gadapt/exit_check/requested_cost_exit_checker.py
-drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.061914 gadapt-0.2.14/gadapt/factory/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:14:24.000000 gadapt-0.2.14/gadapt/factory/__init__.py
--rw-rw-rw-   0        0        0     9949 2023-05-28 13:25:45.000000 gadapt-0.2.14/gadapt/factory/ga_factory.py
--rw-rw-rw-   0        0        0     8920 2023-05-28 13:38:36.000000 gadapt-0.2.14/gadapt/ga.py
-drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.072413 gadapt-0.2.14/gadapt/ga_logging/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:14:17.000000 gadapt-0.2.14/gadapt/ga_logging/__init__.py
--rw-rw-rw-   0        0        0     2123 2023-05-24 07:42:21.000000 gadapt-0.2.14/gadapt/ga_logging/logging_settings.py
-drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.085914 gadapt-0.2.14/gadapt/ga_model/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:14:07.000000 gadapt-0.2.14/gadapt/ga_model/__init__.py
--rw-rw-rw-   0        0        0     6671 2023-05-28 13:24:31.000000 gadapt-0.2.14/gadapt/ga_model/chromosome.py
--rw-rw-rw-   0        0        0      680 2023-05-28 13:25:45.000000 gadapt-0.2.14/gadapt/ga_model/definitions.py
--rw-rw-rw-   0        0        0     5248 2023-05-25 16:08:26.000000 gadapt-0.2.14/gadapt/ga_model/ga_options.py
--rw-rw-rw-   0        0        0     1398 2023-05-24 16:01:11.000000 gadapt-0.2.14/gadapt/ga_model/ga_results.py
--rw-rw-rw-   0        0        0     1339 2023-05-24 06:38:53.000000 gadapt-0.2.14/gadapt/ga_model/gene.py
--rw-rw-rw-   0        0        0     2546 2023-05-24 06:38:53.000000 gadapt-0.2.14/gadapt/ga_model/genetic_variable.py
--rw-rw-rw-   0        0        0       53 2023-05-17 16:44:58.000000 gadapt-0.2.14/gadapt/ga_model/message_levels.py
--rw-rw-rw-   0        0        0    10169 2023-05-24 16:00:25.000000 gadapt-0.2.14/gadapt/ga_model/population.py
--rw-rw-rw-   0        0        0      785 2023-05-24 06:38:53.000000 gadapt-0.2.14/gadapt/ga_model/ranking_model.py
-drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.089414 gadapt-0.2.14/gadapt/gene_combination/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:14:01.000000 gadapt-0.2.14/gadapt/gene_combination/__init__.py
--rw-rw-rw-   0        0        0      308 2023-05-24 06:38:53.000000 gadapt-0.2.14/gadapt/gene_combination/base_gene_combination.py
--rw-rw-rw-   0        0        0      837 2023-05-23 23:22:44.000000 gadapt-0.2.14/gadapt/gene_combination/blending_gene_combination.py
-drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.097914 gadapt-0.2.14/gadapt/immigration/
--rw-rw-rw-   0        0        0        0 2023-05-24 00:04:24.000000 gadapt-0.2.14/gadapt/immigration/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.103914 gadapt-0.2.14/gadapt/immigration/chromosome_immigration/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:13:55.000000 gadapt-0.2.14/gadapt/immigration/chromosome_immigration/__init__.py
--rw-rw-rw-   0        0        0      611 2023-05-24 06:38:53.000000 gadapt-0.2.14/gadapt/immigration/chromosome_immigration/base_chromosome_immigrator.py
--rw-rw-rw-   0        0        0      336 2023-05-23 23:22:33.000000 gadapt-0.2.14/gadapt/immigration/chromosome_immigration/random_chromosome_immigrator.py
-drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.108415 gadapt-0.2.14/gadapt/immigration/population_immigration/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:13:43.000000 gadapt-0.2.14/gadapt/immigration/population_immigration/__init__.py
--rw-rw-rw-   0        0        0      174 2023-05-24 06:38:53.000000 gadapt-0.2.14/gadapt/immigration/population_immigration/base_population_immigrator.py
--rw-rw-rw-   0        0        0      831 2023-05-23 23:22:20.000000 gadapt-0.2.14/gadapt/immigration/population_immigration/common_population_immigrator.py
-drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.113415 gadapt-0.2.14/gadapt/mutation/
--rw-rw-rw-   0        0        0        0 2023-05-24 00:04:04.000000 gadapt-0.2.14/gadapt/mutation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.122414 gadapt-0.2.14/gadapt/mutation/chromosome_mutation/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:13:32.000000 gadapt-0.2.14/gadapt/mutation/chromosome_mutation/__init__.py
--rw-rw-rw-   0        0        0      841 2023-05-24 06:38:53.000000 gadapt-0.2.14/gadapt/mutation/chromosome_mutation/base_chromosome_mutator.py
--rw-rw-rw-   0        0        0     2938 2023-05-24 06:54:25.000000 gadapt-0.2.14/gadapt/mutation/chromosome_mutation/cross_diversity_chromosome_mutator.py
--rw-rw-rw-   0        0        0      936 2023-05-23 23:45:26.000000 gadapt-0.2.14/gadapt/mutation/chromosome_mutation/random_chromosome_mutator.py
-drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.152413 gadapt-0.2.14/gadapt/mutation/population_mutation/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:13:12.000000 gadapt-0.2.14/gadapt/mutation/population_mutation/__init__.py
--rw-rw-rw-   0        0        0     1402 2023-05-24 06:38:53.000000 gadapt-0.2.14/gadapt/mutation/population_mutation/base_population_mutator.py
--rw-rw-rw-   0        0        0     1269 2023-05-23 23:43:50.000000 gadapt-0.2.14/gadapt/mutation/population_mutation/composed_population_mutator.py
-drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.154915 gadapt-0.2.14/gadapt/mutation/population_mutation/cost_diversity/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:13:26.000000 gadapt-0.2.14/gadapt/mutation/population_mutation/cost_diversity/__init__.py
--rw-rw-rw-   0        0        0     2899 2023-05-24 06:54:25.000000 gadapt-0.2.14/gadapt/mutation/population_mutation/cost_diversity/cost_diversity_population_mutator.py
--rw-rw-rw-   0        0        0     1976 2023-05-28 15:09:04.000000 gadapt-0.2.14/gadapt/mutation/population_mutation/parent_diversity_population_mutator.py
-drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.158914 gadapt-0.2.14/gadapt/mutation/population_mutation/previous_cost_diversity/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:13:19.000000 gadapt-0.2.14/gadapt/mutation/population_mutation/previous_cost_diversity/__init__.py
--rw-rw-rw-   0        0        0     3769 2023-05-24 06:54:24.000000 gadapt-0.2.14/gadapt/mutation/population_mutation/previous_cost_diversity/previous_cost_diversity_population_mutator.py
--rw-rw-rw-   0        0        0      469 2023-05-24 06:38:53.000000 gadapt-0.2.14/gadapt/mutation/population_mutation/previous_cost_diversity/previous_cost_diversity_property_taker.py
--rw-rw-rw-   0        0        0     1069 2023-05-23 23:46:12.000000 gadapt-0.2.14/gadapt/mutation/population_mutation/random_population_mutator.py
-drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.162414 gadapt-0.2.14/gadapt/parent_selection/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:12:56.000000 gadapt-0.2.14/gadapt/parent_selection/__init__.py
--rw-rw-rw-   0        0        0      299 2023-05-24 06:38:53.000000 gadapt-0.2.14/gadapt/parent_selection/base_parent_selector.py
--rw-rw-rw-   0        0        0      883 2023-05-23 23:20:13.000000 gadapt-0.2.14/gadapt/parent_selection/sampling_parent_selector.py
-drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.185414 gadapt-0.2.14/gadapt/sampling/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:12:48.000000 gadapt-0.2.14/gadapt/sampling/__init__.py
--rw-rw-rw-   0        0        0      707 2023-05-24 06:38:53.000000 gadapt-0.2.14/gadapt/sampling/base_sampling.py
--rw-rw-rw-   0        0        0      433 2023-05-23 23:19:58.000000 gadapt-0.2.14/gadapt/sampling/from_top_to_bottom_sampling.py
--rw-rw-rw-   0        0        0      425 2023-05-23 23:46:22.000000 gadapt-0.2.14/gadapt/sampling/random_sampling.py
--rw-rw-rw-   0        0        0     1812 2023-05-23 23:46:32.000000 gadapt-0.2.14/gadapt/sampling/roulette_wheel_sampling.py
--rw-rw-rw-   0        0        0     2622 2023-05-23 23:46:42.000000 gadapt-0.2.14/gadapt/sampling/tournament_sampling.py
-drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.187914 gadapt-0.2.14/gadapt/string_operation/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:11:28.000000 gadapt-0.2.14/gadapt/string_operation/__init__.py
--rw-rw-rw-   0        0        0     3219 2023-05-24 06:41:20.000000 gadapt-0.2.14/gadapt/string_operation/ga_strings.py
-drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.192916 gadapt-0.2.14/gadapt/utils/
--rw-rw-rw-   0        0        0      229 2023-05-04 17:34:59.000000 gadapt-0.2.14/gadapt/utils/TimeStampFormatter.py
--rw-rw-rw-   0        0        0        0 2023-05-24 06:12:32.000000 gadapt-0.2.14/gadapt/utils/__init__.py
--rw-rw-rw-   0        0        0     1272 2023-05-25 15:37:31.000000 gadapt-0.2.14/gadapt/utils/ga_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.197914 gadapt-0.2.14/gadapt/validation/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:12:26.000000 gadapt-0.2.14/gadapt/validation/__init__.py
--rw-rw-rw-   0        0        0      787 2023-05-24 06:45:03.000000 gadapt-0.2.14/gadapt/validation/base_options_validator.py
--rw-rw-rw-   0        0        0    17413 2023-05-28 13:25:45.000000 gadapt-0.2.14/gadapt/validation/common_options_validator.py
-drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.201415 gadapt-0.2.14/gadapt/variable_update/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:12:11.000000 gadapt-0.2.14/gadapt/variable_update/__init__.py
--rw-rw-rw-   0        0        0      176 2023-05-24 06:38:52.000000 gadapt-0.2.14/gadapt/variable_update/base_variable_updater.py
--rw-rw-rw-   0        0        0     2001 2023-05-24 06:54:25.000000 gadapt-0.2.14/gadapt/variable_update/common_variable_updater.py
-drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.039413 gadapt-0.2.14/gadapt.egg-info/
--rw-rw-rw-   0        0        0      320 2023-05-28 17:26:20.000000 gadapt-0.2.14/gadapt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3460 2023-05-28 17:26:20.000000 gadapt-0.2.14/gadapt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 17:26:20.000000 gadapt-0.2.14/gadapt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-28 17:26:20.000000 gadapt-0.2.14/gadapt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      111 2023-05-28 17:26:21.208913 gadapt-0.2.14/setup.cfg
--rw-rw-rw-   0        0        0      389 2023-05-28 17:26:01.000000 gadapt-0.2.14/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 08:33:50.797439 gadapt-0.2.15/
+-rw-rw-rw-   0        0        0    21680 2023-05-29 08:33:50.797939 gadapt-0.2.15/PKG-INFO
+-rw-rw-rw-   0        0        0    19350 2023-05-28 15:29:08.000000 gadapt-0.2.15/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 08:33:50.667438 gadapt-0.2.15/gadapt/
+-rw-rw-rw-   0        0        0        2 2023-05-24 06:11:19.000000 gadapt-0.2.15/gadapt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 08:33:50.691939 gadapt-0.2.15/gadapt/cost_finding/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:14:46.000000 gadapt-0.2.15/gadapt/cost_finding/__init__.py
+-rw-rw-rw-   0        0        0      728 2023-05-24 06:38:53.000000 gadapt-0.2.15/gadapt/cost_finding/base_cost_finder.py
+-rw-rw-rw-   0        0        0     2112 2023-05-24 06:54:25.000000 gadapt-0.2.15/gadapt/cost_finding/common_cost_finder.py
+drwxrwxrwx   0        0        0        0 2023-05-29 08:33:50.695937 gadapt-0.2.15/gadapt/crossover/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:14:39.000000 gadapt-0.2.15/gadapt/crossover/__init__.py
+-rw-rw-rw-   0        0        0     7034 2023-05-28 13:24:31.000000 gadapt-0.2.15/gadapt/crossover/base_crossover.py
+-rw-rw-rw-   0        0        0     1257 2023-05-23 23:45:14.000000 gadapt-0.2.15/gadapt/crossover/uniform_crossover.py
+drwxrwxrwx   0        0        0        0 2023-05-29 08:33:50.699939 gadapt-0.2.15/gadapt/execution/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:14:34.000000 gadapt-0.2.15/gadapt/execution/__init__.py
+-rw-rw-rw-   0        0        0     3233 2023-05-27 11:13:47.000000 gadapt-0.2.15/gadapt/execution/ga_executor.py
+drwxrwxrwx   0        0        0        0 2023-05-29 08:33:50.710438 gadapt-0.2.15/gadapt/exit_check/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:14:29.000000 gadapt-0.2.15/gadapt/exit_check/__init__.py
+-rw-rw-rw-   0        0        0      315 2023-05-23 23:28:45.000000 gadapt-0.2.15/gadapt/exit_check/avg_cost_exit_checker.py
+-rw-rw-rw-   0        0        0     1060 2023-05-24 06:38:53.000000 gadapt-0.2.15/gadapt/exit_check/base_exit_checker.py
+-rw-rw-rw-   0        0        0      305 2023-05-23 23:28:54.000000 gadapt-0.2.15/gadapt/exit_check/min_cost_exit_checker.py
+-rw-rw-rw-   0        0        0      387 2023-05-23 23:29:00.000000 gadapt-0.2.15/gadapt/exit_check/requested_cost_exit_checker.py
+drwxrwxrwx   0        0        0        0 2023-05-29 08:33:50.712440 gadapt-0.2.15/gadapt/factory/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:14:24.000000 gadapt-0.2.15/gadapt/factory/__init__.py
+-rw-rw-rw-   0        0        0     9949 2023-05-28 13:25:45.000000 gadapt-0.2.15/gadapt/factory/ga_factory.py
+-rw-rw-rw-   0        0        0     8920 2023-05-28 13:38:36.000000 gadapt-0.2.15/gadapt/ga.py
+drwxrwxrwx   0        0        0        0 2023-05-29 08:33:50.714940 gadapt-0.2.15/gadapt/ga_logging/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:14:17.000000 gadapt-0.2.15/gadapt/ga_logging/__init__.py
+-rw-rw-rw-   0        0        0     2123 2023-05-24 07:42:21.000000 gadapt-0.2.15/gadapt/ga_logging/logging_settings.py
+drwxrwxrwx   0        0        0        0 2023-05-29 08:33:50.727939 gadapt-0.2.15/gadapt/ga_model/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:14:07.000000 gadapt-0.2.15/gadapt/ga_model/__init__.py
+-rw-rw-rw-   0        0        0     6671 2023-05-28 13:24:31.000000 gadapt-0.2.15/gadapt/ga_model/chromosome.py
+-rw-rw-rw-   0        0        0      680 2023-05-28 13:25:45.000000 gadapt-0.2.15/gadapt/ga_model/definitions.py
+-rw-rw-rw-   0        0        0     5248 2023-05-25 16:08:26.000000 gadapt-0.2.15/gadapt/ga_model/ga_options.py
+-rw-rw-rw-   0        0        0     1398 2023-05-24 16:01:11.000000 gadapt-0.2.15/gadapt/ga_model/ga_results.py
+-rw-rw-rw-   0        0        0     1339 2023-05-24 06:38:53.000000 gadapt-0.2.15/gadapt/ga_model/gene.py
+-rw-rw-rw-   0        0        0     2546 2023-05-24 06:38:53.000000 gadapt-0.2.15/gadapt/ga_model/genetic_variable.py
+-rw-rw-rw-   0        0        0       53 2023-05-17 16:44:58.000000 gadapt-0.2.15/gadapt/ga_model/message_levels.py
+-rw-rw-rw-   0        0        0    10169 2023-05-24 16:00:25.000000 gadapt-0.2.15/gadapt/ga_model/population.py
+-rw-rw-rw-   0        0        0      785 2023-05-24 06:38:53.000000 gadapt-0.2.15/gadapt/ga_model/ranking_model.py
+drwxrwxrwx   0        0        0        0 2023-05-29 08:33:50.731439 gadapt-0.2.15/gadapt/gene_combination/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:14:01.000000 gadapt-0.2.15/gadapt/gene_combination/__init__.py
+-rw-rw-rw-   0        0        0      308 2023-05-24 06:38:53.000000 gadapt-0.2.15/gadapt/gene_combination/base_gene_combination.py
+-rw-rw-rw-   0        0        0      837 2023-05-23 23:22:44.000000 gadapt-0.2.15/gadapt/gene_combination/blending_gene_combination.py
+drwxrwxrwx   0        0        0        0 2023-05-29 08:33:50.732440 gadapt-0.2.15/gadapt/immigration/
+-rw-rw-rw-   0        0        0        0 2023-05-24 00:04:24.000000 gadapt-0.2.15/gadapt/immigration/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 08:33:50.735438 gadapt-0.2.15/gadapt/immigration/chromosome_immigration/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:13:55.000000 gadapt-0.2.15/gadapt/immigration/chromosome_immigration/__init__.py
+-rw-rw-rw-   0        0        0      611 2023-05-24 06:38:53.000000 gadapt-0.2.15/gadapt/immigration/chromosome_immigration/base_chromosome_immigrator.py
+-rw-rw-rw-   0        0        0      336 2023-05-23 23:22:33.000000 gadapt-0.2.15/gadapt/immigration/chromosome_immigration/random_chromosome_immigrator.py
+drwxrwxrwx   0        0        0        0 2023-05-29 08:33:50.738438 gadapt-0.2.15/gadapt/immigration/population_immigration/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:13:43.000000 gadapt-0.2.15/gadapt/immigration/population_immigration/__init__.py
+-rw-rw-rw-   0        0        0      174 2023-05-24 06:38:53.000000 gadapt-0.2.15/gadapt/immigration/population_immigration/base_population_immigrator.py
+-rw-rw-rw-   0        0        0      831 2023-05-23 23:22:20.000000 gadapt-0.2.15/gadapt/immigration/population_immigration/common_population_immigrator.py
+drwxrwxrwx   0        0        0        0 2023-05-29 08:33:50.739939 gadapt-0.2.15/gadapt/mutation/
+-rw-rw-rw-   0        0        0        0 2023-05-24 00:04:04.000000 gadapt-0.2.15/gadapt/mutation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 08:33:50.755939 gadapt-0.2.15/gadapt/mutation/chromosome_mutation/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:13:32.000000 gadapt-0.2.15/gadapt/mutation/chromosome_mutation/__init__.py
+-rw-rw-rw-   0        0        0      841 2023-05-24 06:38:53.000000 gadapt-0.2.15/gadapt/mutation/chromosome_mutation/base_chromosome_mutator.py
+-rw-rw-rw-   0        0        0     2938 2023-05-24 06:54:25.000000 gadapt-0.2.15/gadapt/mutation/chromosome_mutation/cross_diversity_chromosome_mutator.py
+-rw-rw-rw-   0        0        0      936 2023-05-23 23:45:26.000000 gadapt-0.2.15/gadapt/mutation/chromosome_mutation/random_chromosome_mutator.py
+drwxrwxrwx   0        0        0        0 2023-05-29 08:33:50.762438 gadapt-0.2.15/gadapt/mutation/population_mutation/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:13:12.000000 gadapt-0.2.15/gadapt/mutation/population_mutation/__init__.py
+-rw-rw-rw-   0        0        0     1402 2023-05-24 06:38:53.000000 gadapt-0.2.15/gadapt/mutation/population_mutation/base_population_mutator.py
+-rw-rw-rw-   0        0        0     1269 2023-05-23 23:43:50.000000 gadapt-0.2.15/gadapt/mutation/population_mutation/composed_population_mutator.py
+drwxrwxrwx   0        0        0        0 2023-05-29 08:33:50.764938 gadapt-0.2.15/gadapt/mutation/population_mutation/cost_diversity/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:13:26.000000 gadapt-0.2.15/gadapt/mutation/population_mutation/cost_diversity/__init__.py
+-rw-rw-rw-   0        0        0     2899 2023-05-24 06:54:25.000000 gadapt-0.2.15/gadapt/mutation/population_mutation/cost_diversity/cost_diversity_population_mutator.py
+-rw-rw-rw-   0        0        0     1976 2023-05-28 15:09:04.000000 gadapt-0.2.15/gadapt/mutation/population_mutation/parent_diversity_population_mutator.py
+drwxrwxrwx   0        0        0        0 2023-05-29 08:33:50.767939 gadapt-0.2.15/gadapt/mutation/population_mutation/previous_cost_diversity/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:13:19.000000 gadapt-0.2.15/gadapt/mutation/population_mutation/previous_cost_diversity/__init__.py
+-rw-rw-rw-   0        0        0     3769 2023-05-24 06:54:24.000000 gadapt-0.2.15/gadapt/mutation/population_mutation/previous_cost_diversity/previous_cost_diversity_population_mutator.py
+-rw-rw-rw-   0        0        0      469 2023-05-24 06:38:53.000000 gadapt-0.2.15/gadapt/mutation/population_mutation/previous_cost_diversity/previous_cost_diversity_property_taker.py
+-rw-rw-rw-   0        0        0     1069 2023-05-23 23:46:12.000000 gadapt-0.2.15/gadapt/mutation/population_mutation/random_population_mutator.py
+drwxrwxrwx   0        0        0        0 2023-05-29 08:33:50.771438 gadapt-0.2.15/gadapt/parent_selection/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:12:56.000000 gadapt-0.2.15/gadapt/parent_selection/__init__.py
+-rw-rw-rw-   0        0        0      299 2023-05-24 06:38:53.000000 gadapt-0.2.15/gadapt/parent_selection/base_parent_selector.py
+-rw-rw-rw-   0        0        0      883 2023-05-23 23:20:13.000000 gadapt-0.2.15/gadapt/parent_selection/sampling_parent_selector.py
+drwxrwxrwx   0        0        0        0 2023-05-29 08:33:50.778938 gadapt-0.2.15/gadapt/sampling/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:12:48.000000 gadapt-0.2.15/gadapt/sampling/__init__.py
+-rw-rw-rw-   0        0        0      707 2023-05-24 06:38:53.000000 gadapt-0.2.15/gadapt/sampling/base_sampling.py
+-rw-rw-rw-   0        0        0      433 2023-05-23 23:19:58.000000 gadapt-0.2.15/gadapt/sampling/from_top_to_bottom_sampling.py
+-rw-rw-rw-   0        0        0      425 2023-05-23 23:46:22.000000 gadapt-0.2.15/gadapt/sampling/random_sampling.py
+-rw-rw-rw-   0        0        0     1812 2023-05-23 23:46:32.000000 gadapt-0.2.15/gadapt/sampling/roulette_wheel_sampling.py
+-rw-rw-rw-   0        0        0     2622 2023-05-23 23:46:42.000000 gadapt-0.2.15/gadapt/sampling/tournament_sampling.py
+drwxrwxrwx   0        0        0        0 2023-05-29 08:33:50.780938 gadapt-0.2.15/gadapt/string_operation/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:11:28.000000 gadapt-0.2.15/gadapt/string_operation/__init__.py
+-rw-rw-rw-   0        0        0     3219 2023-05-24 06:41:20.000000 gadapt-0.2.15/gadapt/string_operation/ga_strings.py
+drwxrwxrwx   0        0        0        0 2023-05-29 08:33:50.784439 gadapt-0.2.15/gadapt/utils/
+-rw-rw-rw-   0        0        0      229 2023-05-04 17:34:59.000000 gadapt-0.2.15/gadapt/utils/TimeStampFormatter.py
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:12:32.000000 gadapt-0.2.15/gadapt/utils/__init__.py
+-rw-rw-rw-   0        0        0     1272 2023-05-25 15:37:31.000000 gadapt-0.2.15/gadapt/utils/ga_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-29 08:33:50.787938 gadapt-0.2.15/gadapt/validation/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:12:26.000000 gadapt-0.2.15/gadapt/validation/__init__.py
+-rw-rw-rw-   0        0        0      787 2023-05-24 06:45:03.000000 gadapt-0.2.15/gadapt/validation/base_options_validator.py
+-rw-rw-rw-   0        0        0    17413 2023-05-28 13:25:45.000000 gadapt-0.2.15/gadapt/validation/common_options_validator.py
+drwxrwxrwx   0        0        0        0 2023-05-29 08:33:50.795938 gadapt-0.2.15/gadapt/variable_update/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:12:11.000000 gadapt-0.2.15/gadapt/variable_update/__init__.py
+-rw-rw-rw-   0        0        0      176 2023-05-24 06:38:52.000000 gadapt-0.2.15/gadapt/variable_update/base_variable_updater.py
+-rw-rw-rw-   0        0        0     2001 2023-05-24 06:54:25.000000 gadapt-0.2.15/gadapt/variable_update/common_variable_updater.py
+drwxrwxrwx   0        0        0        0 2023-05-29 08:33:50.687440 gadapt-0.2.15/gadapt.egg-info/
+-rw-rw-rw-   0        0        0    21680 2023-05-29 08:33:50.000000 gadapt-0.2.15/gadapt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3460 2023-05-29 08:33:50.000000 gadapt-0.2.15/gadapt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 08:33:50.000000 gadapt-0.2.15/gadapt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-29 08:33:50.000000 gadapt-0.2.15/gadapt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      111 2023-05-29 08:33:50.805437 gadapt-0.2.15/setup.cfg
+-rw-rw-rw-   0        0        0      465 2023-05-29 08:33:40.000000 gadapt-0.2.15/setup.py
```

### Comparing `gadapt-0.2.14/README.md` & `gadapt-0.2.15/README.md`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.14/gadapt/cost_finding/base_cost_finder.py` & `gadapt-0.2.15/gadapt/cost_finding/base_cost_finder.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.14/gadapt/cost_finding/common_cost_finder.py` & `gadapt-0.2.15/gadapt/cost_finding/common_cost_finder.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.14/gadapt/crossover/base_crossover.py` & `gadapt-0.2.15/gadapt/crossover/base_crossover.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.14/gadapt/crossover/uniform_crossover.py` & `gadapt-0.2.15/gadapt/crossover/uniform_crossover.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.14/gadapt/execution/ga_executor.py` & `gadapt-0.2.15/gadapt/execution/ga_executor.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.14/gadapt/exit_check/base_exit_checker.py` & `gadapt-0.2.15/gadapt/exit_check/base_exit_checker.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.14/gadapt/factory/ga_factory.py` & `gadapt-0.2.15/gadapt/factory/ga_factory.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.14/gadapt/ga.py` & `gadapt-0.2.15/gadapt/ga.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.14/gadapt/ga_logging/logging_settings.py` & `gadapt-0.2.15/gadapt/ga_logging/logging_settings.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.14/gadapt/ga_model/chromosome.py` & `gadapt-0.2.15/gadapt/ga_model/chromosome.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.14/gadapt/ga_model/definitions.py` & `gadapt-0.2.15/gadapt/ga_model/definitions.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.14/gadapt/ga_model/ga_options.py` & `gadapt-0.2.15/gadapt/ga_model/ga_options.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.14/gadapt/ga_model/ga_results.py` & `gadapt-0.2.15/gadapt/ga_model/ga_results.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.14/gadapt/ga_model/gene.py` & `gadapt-0.2.15/gadapt/ga_model/gene.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.14/gadapt/ga_model/genetic_variable.py` & `gadapt-0.2.15/gadapt/ga_model/genetic_variable.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.14/gadapt/ga_model/population.py` & `gadapt-0.2.15/gadapt/ga_model/population.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.14/gadapt/ga_model/ranking_model.py` & `gadapt-0.2.15/gadapt/ga_model/ranking_model.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.14/gadapt/gene_combination/blending_gene_combination.py` & `gadapt-0.2.15/gadapt/gene_combination/blending_gene_combination.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.14/gadapt/immigration/chromosome_immigration/base_chromosome_immigrator.py` & `gadapt-0.2.15/gadapt/immigration/chromosome_immigration/base_chromosome_immigrator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.14/gadapt/immigration/population_immigration/common_population_immigrator.py` & `gadapt-0.2.15/gadapt/immigration/population_immigration/common_population_immigrator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.14/gadapt/mutation/chromosome_mutation/base_chromosome_mutator.py` & `gadapt-0.2.15/gadapt/mutation/chromosome_mutation/base_chromosome_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.14/gadapt/mutation/chromosome_mutation/cross_diversity_chromosome_mutator.py` & `gadapt-0.2.15/gadapt/mutation/chromosome_mutation/cross_diversity_chromosome_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.14/gadapt/mutation/chromosome_mutation/random_chromosome_mutator.py` & `gadapt-0.2.15/gadapt/mutation/chromosome_mutation/random_chromosome_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.14/gadapt/mutation/population_mutation/base_population_mutator.py` & `gadapt-0.2.15/gadapt/mutation/population_mutation/base_population_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.14/gadapt/mutation/population_mutation/composed_population_mutator.py` & `gadapt-0.2.15/gadapt/mutation/population_mutation/composed_population_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.14/gadapt/mutation/population_mutation/cost_diversity/cost_diversity_population_mutator.py` & `gadapt-0.2.15/gadapt/mutation/population_mutation/cost_diversity/cost_diversity_population_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.14/gadapt/mutation/population_mutation/parent_diversity_population_mutator.py` & `gadapt-0.2.15/gadapt/mutation/population_mutation/parent_diversity_population_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.14/gadapt/mutation/population_mutation/previous_cost_diversity/previous_cost_diversity_population_mutator.py` & `gadapt-0.2.15/gadapt/mutation/population_mutation/previous_cost_diversity/previous_cost_diversity_population_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.14/gadapt/mutation/population_mutation/random_population_mutator.py` & `gadapt-0.2.15/gadapt/mutation/population_mutation/random_population_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.14/gadapt/parent_selection/sampling_parent_selector.py` & `gadapt-0.2.15/gadapt/parent_selection/sampling_parent_selector.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.14/gadapt/sampling/base_sampling.py` & `gadapt-0.2.15/gadapt/sampling/base_sampling.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.14/gadapt/sampling/roulette_wheel_sampling.py` & `gadapt-0.2.15/gadapt/sampling/roulette_wheel_sampling.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.14/gadapt/sampling/tournament_sampling.py` & `gadapt-0.2.15/gadapt/sampling/tournament_sampling.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.14/gadapt/string_operation/ga_strings.py` & `gadapt-0.2.15/gadapt/string_operation/ga_strings.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.14/gadapt/utils/ga_utils.py` & `gadapt-0.2.15/gadapt/utils/ga_utils.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.14/gadapt/validation/base_options_validator.py` & `gadapt-0.2.15/gadapt/validation/base_options_validator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.14/gadapt/validation/common_options_validator.py` & `gadapt-0.2.15/gadapt/validation/common_options_validator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.14/gadapt/variable_update/common_variable_updater.py` & `gadapt-0.2.15/gadapt/variable_update/common_variable_updater.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.14/gadapt.egg-info/SOURCES.txt` & `gadapt-0.2.15/gadapt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

