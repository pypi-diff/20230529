# Comparing `tmp/ma_gym-0.0.8.tar.gz` & `tmp/ma_gym-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ma_gym-0.0.8.tar", last modified: Wed Nov 10 04:16:59 2021, max compression
+gzip compressed data, was "ma_gym-0.0.9.tar", last modified: Sat Jul  9 22:00:57 2022, max compression
```

## Comparing `ma_gym-0.0.8.tar` & `ma_gym-0.0.9.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 04:16:59.853522 ma_gym-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)    11340 2021-11-10 04:16:31.000000 ma_gym-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4393 2021-11-10 04:16:59.853522 ma_gym-0.0.8/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (121)     3827 2021-11-10 04:16:31.000000 ma_gym-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 04:16:59.849522 ma_gym-0.0.8/ma_gym/
--rwxr-xr-x   0 runner    (1001) docker     (121)     3490 2021-11-10 04:16:31.000000 ma_gym-0.0.8/ma_gym/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 04:16:59.849522 ma_gym-0.0.8/ma_gym/envs/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 04:16:31.000000 ma_gym-0.0.8/ma_gym/envs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 04:16:59.849522 ma_gym-0.0.8/ma_gym/envs/checkers/
--rw-r--r--   0 runner    (1001) docker     (121)       30 2021-11-10 04:16:31.000000 ma_gym-0.0.8/ma_gym/envs/checkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12044 2021-11-10 04:16:31.000000 ma_gym-0.0.8/ma_gym/envs/checkers/checkers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 04:16:59.849522 ma_gym-0.0.8/ma_gym/envs/combat/
--rw-r--r--   0 runner    (1001) docker     (121)       27 2021-11-10 04:16:31.000000 ma_gym-0.0.8/ma_gym/envs/combat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    24464 2021-11-10 04:16:31.000000 ma_gym-0.0.8/ma_gym/envs/combat/combat.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 04:16:59.849522 ma_gym-0.0.8/ma_gym/envs/lumberjacks/
--rw-r--r--   0 runner    (1001) docker     (121)       37 2021-11-10 04:16:31.000000 ma_gym-0.0.8/ma_gym/envs/lumberjacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16116 2021-11-10 04:16:31.000000 ma_gym-0.0.8/ma_gym/envs/lumberjacks/lumberjacks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 04:16:59.849522 ma_gym-0.0.8/ma_gym/envs/openai/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1709 2021-11-10 04:16:31.000000 ma_gym-0.0.8/ma_gym/envs/openai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 04:16:59.849522 ma_gym-0.0.8/ma_gym/envs/pong_duel/
--rwxr-xr-x   0 runner    (1001) docker     (121)       31 2021-11-10 04:16:31.000000 ma_gym-0.0.8/ma_gym/envs/pong_duel/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    11627 2021-11-10 04:16:31.000000 ma_gym-0.0.8/ma_gym/envs/pong_duel/pong_duel.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 04:16:59.849522 ma_gym-0.0.8/ma_gym/envs/predator_prey/
--rwxr-xr-x   0 runner    (1001) docker     (121)       40 2021-11-10 04:16:31.000000 ma_gym-0.0.8/ma_gym/envs/predator_prey/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    15287 2021-11-10 04:16:31.000000 ma_gym-0.0.8/ma_gym/envs/predator_prey/predator_prey.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 04:16:59.849522 ma_gym-0.0.8/ma_gym/envs/switch/
--rw-r--r--   0 runner    (1001) docker     (121)       39 2021-11-10 04:16:31.000000 ma_gym-0.0.8/ma_gym/envs/switch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8075 2021-11-10 04:16:31.000000 ma_gym-0.0.8/ma_gym/envs/switch/switch_one_corridor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 04:16:59.849522 ma_gym-0.0.8/ma_gym/envs/traffic_junction/
--rw-r--r--   0 runner    (1001) docker     (121)       46 2021-11-10 04:16:31.000000 ma_gym-0.0.8/ma_gym/envs/traffic_junction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22982 2021-11-10 04:16:31.000000 ma_gym-0.0.8/ma_gym/envs/traffic_junction/traffic_junction.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 04:16:59.853522 ma_gym-0.0.8/ma_gym/envs/utils/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 04:16:31.000000 ma_gym-0.0.8/ma_gym/envs/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      509 2021-11-10 04:16:31.000000 ma_gym-0.0.8/ma_gym/envs/utils/action_space.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4296 2021-11-10 04:16:31.000000 ma_gym-0.0.8/ma_gym/envs/utils/draw.py
--rw-r--r--   0 runner    (1001) docker     (121)      773 2021-11-10 04:16:31.000000 ma_gym-0.0.8/ma_gym/envs/utils/observation_space.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 04:16:59.853522 ma_gym-0.0.8/ma_gym/wrappers/
--rw-r--r--   0 runner    (1001) docker     (121)       43 2021-11-10 04:16:31.000000 ma_gym-0.0.8/ma_gym/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5093 2021-11-10 04:16:31.000000 ma_gym-0.0.8/ma_gym/wrappers/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 04:16:59.853522 ma_gym-0.0.8/ma_gym/wrappers/monitoring/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-10 04:16:31.000000 ma_gym-0.0.8/ma_gym/wrappers/monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      311 2021-11-10 04:16:31.000000 ma_gym-0.0.8/ma_gym/wrappers/monitoring/stats_recorder.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 04:16:59.849522 ma_gym-0.0.8/ma_gym.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4393 2021-11-10 04:16:59.000000 ma_gym-0.0.8/ma_gym.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1353 2021-11-10 04:16:59.000000 ma_gym-0.0.8/ma_gym.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-10 04:16:59.000000 ma_gym-0.0.8/ma_gym.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      195 2021-11-10 04:16:59.000000 ma_gym-0.0.8/ma_gym.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-11-10 04:16:59.000000 ma_gym-0.0.8/ma_gym.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-10 04:16:59.853522 ma_gym-0.0.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1260 2021-11-10 04:16:31.000000 ma_gym-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 04:16:59.853522 ma_gym-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-10 04:16:31.000000 ma_gym-0.0.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 04:16:59.853522 ma_gym-0.0.8/tests/envs/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-10 04:16:31.000000 ma_gym-0.0.8/tests/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5815 2021-11-10 04:16:31.000000 ma_gym-0.0.8/tests/envs/test_checkers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1390 2021-11-10 04:16:31.000000 ma_gym-0.0.8/tests/envs/test_combat.py
--rw-r--r--   0 runner    (1001) docker     (121)     3279 2021-11-10 04:16:31.000000 ma_gym-0.0.8/tests/envs/test_lumberjacks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2021-11-10 04:16:31.000000 ma_gym-0.0.8/tests/envs/test_openai_cartpole.py
--rw-r--r--   0 runner    (1001) docker     (121)     1236 2021-11-10 04:16:31.000000 ma_gym-0.0.8/tests/envs/test_pong_duel.py
--rw-r--r--   0 runner    (1001) docker     (121)     1979 2021-11-10 04:16:31.000000 ma_gym-0.0.8/tests/envs/test_predatorprey5x5.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1623 2021-11-10 04:16:31.000000 ma_gym-0.0.8/tests/envs/test_predatorprey7x7.py
--rw-r--r--   0 runner    (1001) docker     (121)     5049 2021-11-10 04:16:31.000000 ma_gym-0.0.8/tests/envs/test_switch2.py
--rw-r--r--   0 runner    (1001) docker     (121)     8620 2021-11-10 04:16:31.000000 ma_gym-0.0.8/tests/envs/test_trafficjunction.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-09 22:00:57.569025 ma_gym-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11340 2022-07-09 22:00:49.000000 ma_gym-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     4643 2022-07-09 22:00:57.569025 ma_gym-0.0.9/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4077 2022-07-09 22:00:49.000000 ma_gym-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-09 22:00:57.565025 ma_gym-0.0.9/ma_gym/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3490 2022-07-09 22:00:49.000000 ma_gym-0.0.9/ma_gym/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-09 22:00:57.565025 ma_gym-0.0.9/ma_gym/envs/
+-rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-09 22:00:49.000000 ma_gym-0.0.9/ma_gym/envs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-09 22:00:57.565025 ma_gym-0.0.9/ma_gym/envs/checkers/
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2022-07-09 22:00:49.000000 ma_gym-0.0.9/ma_gym/envs/checkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12248 2022-07-09 22:00:49.000000 ma_gym-0.0.9/ma_gym/envs/checkers/checkers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-09 22:00:57.565025 ma_gym-0.0.9/ma_gym/envs/combat/
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2022-07-09 22:00:49.000000 ma_gym-0.0.9/ma_gym/envs/combat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25370 2022-07-09 22:00:49.000000 ma_gym-0.0.9/ma_gym/envs/combat/combat.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-09 22:00:57.565025 ma_gym-0.0.9/ma_gym/envs/lumberjacks/
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-07-09 22:00:49.000000 ma_gym-0.0.9/ma_gym/envs/lumberjacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17107 2022-07-09 22:00:49.000000 ma_gym-0.0.9/ma_gym/envs/lumberjacks/lumberjacks.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-09 22:00:57.565025 ma_gym-0.0.9/ma_gym/envs/openai/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1781 2022-07-09 22:00:49.000000 ma_gym-0.0.9/ma_gym/envs/openai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-09 22:00:57.569025 ma_gym-0.0.9/ma_gym/envs/pong_duel/
+-rwxr-xr-x   0 runner    (1001) docker     (121)       31 2022-07-09 22:00:49.000000 ma_gym-0.0.9/ma_gym/envs/pong_duel/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    12582 2022-07-09 22:00:49.000000 ma_gym-0.0.9/ma_gym/envs/pong_duel/pong_duel.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-09 22:00:57.569025 ma_gym-0.0.9/ma_gym/envs/predator_prey/
+-rwxr-xr-x   0 runner    (1001) docker     (121)       40 2022-07-09 22:00:49.000000 ma_gym-0.0.9/ma_gym/envs/predator_prey/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    16966 2022-07-09 22:00:49.000000 ma_gym-0.0.9/ma_gym/envs/predator_prey/predator_prey.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-09 22:00:57.569025 ma_gym-0.0.9/ma_gym/envs/switch/
+-rw-r--r--   0 runner    (1001) docker     (121)       39 2022-07-09 22:00:49.000000 ma_gym-0.0.9/ma_gym/envs/switch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8279 2022-07-09 22:00:49.000000 ma_gym-0.0.9/ma_gym/envs/switch/switch_one_corridor.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-09 22:00:57.569025 ma_gym-0.0.9/ma_gym/envs/traffic_junction/
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2022-07-09 22:00:49.000000 ma_gym-0.0.9/ma_gym/envs/traffic_junction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22985 2022-07-09 22:00:49.000000 ma_gym-0.0.9/ma_gym/envs/traffic_junction/traffic_junction.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-09 22:00:57.569025 ma_gym-0.0.9/ma_gym/envs/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-09 22:00:49.000000 ma_gym-0.0.9/ma_gym/envs/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      509 2022-07-09 22:00:49.000000 ma_gym-0.0.9/ma_gym/envs/utils/action_space.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4296 2022-07-09 22:00:49.000000 ma_gym-0.0.9/ma_gym/envs/utils/draw.py
+-rw-r--r--   0 runner    (1001) docker     (121)      773 2022-07-09 22:00:49.000000 ma_gym-0.0.9/ma_gym/envs/utils/observation_space.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-09 22:00:57.569025 ma_gym-0.0.9/ma_gym/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2022-07-09 22:00:49.000000 ma_gym-0.0.9/ma_gym/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5093 2022-07-09 22:00:49.000000 ma_gym-0.0.9/ma_gym/wrappers/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-09 22:00:57.569025 ma_gym-0.0.9/ma_gym/wrappers/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-09 22:00:49.000000 ma_gym-0.0.9/ma_gym/wrappers/monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      311 2022-07-09 22:00:49.000000 ma_gym-0.0.9/ma_gym/wrappers/monitoring/stats_recorder.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-09 22:00:57.565025 ma_gym-0.0.9/ma_gym.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4643 2022-07-09 22:00:57.000000 ma_gym-0.0.9/ma_gym.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1353 2022-07-09 22:00:57.000000 ma_gym-0.0.9/ma_gym.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-09 22:00:57.000000 ma_gym-0.0.9/ma_gym.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      195 2022-07-09 22:00:57.000000 ma_gym-0.0.9/ma_gym.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-07-09 22:00:57.000000 ma_gym-0.0.9/ma_gym.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-09 22:00:57.569025 ma_gym-0.0.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1260 2022-07-09 22:00:49.000000 ma_gym-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-09 22:00:57.569025 ma_gym-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-09 22:00:49.000000 ma_gym-0.0.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-09 22:00:57.569025 ma_gym-0.0.9/tests/envs/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-09 22:00:49.000000 ma_gym-0.0.9/tests/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5815 2022-07-09 22:00:49.000000 ma_gym-0.0.9/tests/envs/test_checkers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1390 2022-07-09 22:00:49.000000 ma_gym-0.0.9/tests/envs/test_combat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3279 2022-07-09 22:00:49.000000 ma_gym-0.0.9/tests/envs/test_lumberjacks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-07-09 22:00:49.000000 ma_gym-0.0.9/tests/envs/test_openai_cartpole.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1236 2022-07-09 22:00:49.000000 ma_gym-0.0.9/tests/envs/test_pong_duel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1979 2022-07-09 22:00:49.000000 ma_gym-0.0.9/tests/envs/test_predatorprey5x5.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1623 2022-07-09 22:00:49.000000 ma_gym-0.0.9/tests/envs/test_predatorprey7x7.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5049 2022-07-09 22:00:49.000000 ma_gym-0.0.9/tests/envs/test_switch2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8620 2022-07-09 22:00:49.000000 ma_gym-0.0.9/tests/envs/test_trafficjunction.py
```

### Comparing `ma_gym-0.0.8/LICENSE` & `ma_gym-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ma_gym-0.0.8/PKG-INFO` & `ma_gym-0.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ma_gym
-Version: 0.0.8
+Version: 0.0.9
 Summary: A collection of multi agent environments based on OpenAI gym.
 Home-page: https://github.com/koulanurag/ma-gym
 Author: Anurag Koul
 Author-email: koulanurag@gmail.com
 License: MIT License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
@@ -19,23 +19,23 @@
 
 # ma-gym
 It's a collection of multi agent environments based on OpenAI gym. Also, you can use [**minimal-marl**](https://github.com/koulanurag/minimal-marl) to warm-start training of agents.
 
 ![Python package](https://github.com/koulanurag/ma-gym/workflows/Python%20package/badge.svg) 
 ![Upload Python Package](https://github.com/koulanurag/ma-gym/workflows/Upload%20Python%20Package/badge.svg)
 [![Wiki Docs](https://img.shields.io/badge/-Wiki%20Docs-informational?style=flat)](https://github.com/koulanurag/ma-gym/wiki)
-
+[![Papers using ma-gym](https://img.shields.io/badge/-Papers%20using%20ma--gym-9cf?style=flat&logo=googlescholar)](https://scholar.google.com/scholar?hl=en&as_sdt=5,38&cites=14123576959169220642,12284637994392993807&scipsc=&q=&scisbd=1)
 
 ## Installation
 Using PyPI:
 ```bash
 pip install ma-gym
 ```
 
-Directly from source:
+Directly from source (recommended):
 ```bash
 git clone https://github.com/koulanurag/ma-gym.git
 cd ma-gym
 pip install -e .
 ```
 ## Reference:
 Please use this bibtex if you would like to cite it:
```

### Comparing `ma_gym-0.0.8/README.md` & `ma_gym-0.0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # ma-gym
 It's a collection of multi agent environments based on OpenAI gym. Also, you can use [**minimal-marl**](https://github.com/koulanurag/minimal-marl) to warm-start training of agents.
 
 ![Python package](https://github.com/koulanurag/ma-gym/workflows/Python%20package/badge.svg) 
 ![Upload Python Package](https://github.com/koulanurag/ma-gym/workflows/Upload%20Python%20Package/badge.svg)
 [![Wiki Docs](https://img.shields.io/badge/-Wiki%20Docs-informational?style=flat)](https://github.com/koulanurag/ma-gym/wiki)
-
+[![Papers using ma-gym](https://img.shields.io/badge/-Papers%20using%20ma--gym-9cf?style=flat&logo=googlescholar)](https://scholar.google.com/scholar?hl=en&as_sdt=5,38&cites=14123576959169220642,12284637994392993807&scipsc=&q=&scisbd=1)
 
 ## Installation
 Using PyPI:
 ```bash
 pip install ma-gym
 ```
 
-Directly from source:
+Directly from source (recommended):
 ```bash
 git clone https://github.com/koulanurag/ma-gym.git
 cd ma-gym
 pip install -e .
 ```
 ## Reference:
 Please use this bibtex if you would like to cite it:
```

### Comparing `ma_gym-0.0.8/ma_gym/__init__.py` & `ma_gym-0.0.9/ma_gym/__init__.py`

 * *Files identical despite different names*

### Comparing `ma_gym-0.0.8/ma_gym/envs/checkers/checkers.py` & `ma_gym-0.0.9/ma_gym/envs/checkers/checkers.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,14 +172,17 @@
             self.agent_pos[agent_i] = next_pos
 
     def __update_agent_view(self, agent_i):
         self._full_obs[self.agent_prev_pos[agent_i][0]][self.agent_prev_pos[agent_i][1]] = PRE_IDS['empty']
         self._full_obs[self.agent_pos[agent_i][0]][self.agent_pos[agent_i][1]] = PRE_IDS['agent'] + str(agent_i + 1)
 
     def step(self, agents_action):
+        assert (self._step_count is not None), \
+            "Call reset before using step method."
+
         assert len(agents_action) == self.n_agents
 
         self._step_count += 1
         rewards = [self._step_cost for _ in range(self.n_agents)]
 
         for agent_i, action in enumerate(agents_action):
 
@@ -213,14 +216,17 @@
                     " steps are undefined behavior.")
             self.steps_beyond_done += 1
             rewards = [0 for _ in range(self.n_agents)]
 
         return self.get_agent_obs(), rewards, self._agent_dones, {'food_count': self._food_count}
 
     def render(self, mode='human'):
+        assert (self._step_count is not None), \
+            "Call reset before using render method."
+
         for agent_i in range(self.n_agents):
             fill_cell(self._base_img, self.agent_pos[agent_i], cell_size=CELL_SIZE, fill='white', margin=0.05)
             fill_cell(self._base_img, self.agent_prev_pos[agent_i], cell_size=CELL_SIZE, fill='white', margin=0.05)
             draw_circle(self._base_img, self.agent_pos[agent_i], cell_size=CELL_SIZE, fill=AGENT_COLORS[agent_i])
             write_cell_text(self._base_img, text=str(agent_i + 1), pos=self.agent_pos[agent_i], cell_size=CELL_SIZE,
                             fill='white', margin=0.4)
```

### Comparing `ma_gym-0.0.8/ma_gym/envs/combat/combat.py` & `ma_gym-0.0.9/ma_gym/envs/combat/combat.py`

 * *Files 3% similar despite different names*

```diff
@@ -225,14 +225,15 @@
                     self.__update_opp_view(opp_i)
                     break
 
         self.__draw_base_img()
 
     def reset(self):
         self._step_count = 0
+        self._steps_beyond_done = None
         self._total_episode_reward = [0 for _ in range(self.n_agents)]
         self.agent_health = {_: self._init_health for _ in range(self.n_agents)}
         self.opp_health = {_: self._init_health for _ in range(self._n_opponents)}
         self._agent_cool = {_: True for _ in range(self.n_agents)}
         self._agent_cool_step = {_: 0 for _ in range(self.n_agents)}
         self._opp_cool = {_: True for _ in range(self._n_opponents)}
         self._opp_cool_step = {_: 0 for _ in range(self._n_opponents)}
@@ -243,14 +244,17 @@
         # For debug only
         self._agents_trace = {_: [self.agent_pos[_]] for _ in range(self.n_agents)}
         self._opponents_trace = {_: [self.opp_pos[_]] for _ in range(self._n_opponents)}
 
         return self.get_agent_obs()
 
     def render(self, mode='human'):
+        assert (self._step_count is not None), \
+            "Call reset before using render method."
+
         img = copy.copy(self._base_img)
 
         # draw agents
         for agent_i in range(self.n_agents):
             if self.agent_health[agent_i] > 0:
                 fill_cell(img, self.agent_pos[agent_i], cell_size=CELL_SIZE, fill=AGENT_COLOR)
                 write_cell_text(img, text=str(agent_i + 1), pos=self.agent_pos[agent_i], cell_size=CELL_SIZE,
@@ -416,14 +420,17 @@
                     action = self.np_random.choice(range(5))
                 else:
                     action = 4  # dead opponent could only execute 'no-op' action.
             opp_action_n.append(action)
         return opp_action_n
 
     def step(self, agents_action):
+        assert (self._step_count is not None), \
+            "Call reset before using step method."
+
         assert len(agents_action) == self.n_agents
 
         self._step_count += 1
         rewards = [self._step_cost for _ in range(self.n_agents)]
 
         # What's the confusion?
         # What if agents attack each other at the same time? Should both of them be effected?
@@ -499,14 +506,29 @@
                 or (sum([v for k, v in self.opp_health.items()]) == 0) \
                 or (sum([v for k, v in self.agent_health.items()]) == 0):
             self._agent_dones = [True for _ in range(self.n_agents)]
 
         for i in range(self.n_agents):
             self._total_episode_reward[i] += rewards[i]
 
+        # Check for episode overflow
+        if all(self._agent_dones):
+            if self._steps_beyond_done is None:
+                self._steps_beyond_done = 0
+            else:
+                if self._steps_beyond_done == 0:
+                    logger.warn(
+                        "You are calling 'step()' even though this "
+                        "environment has already returned done = True. You "
+                        "should always call 'reset()' once you receive "
+                        "'done = True' -- any further steps are undefined "
+                        "behavior."
+                    )
+                self._steps_beyond_done += 1
+
         return self.get_agent_obs(), rewards, self._agent_dones, {'health': self.agent_health}
 
     def seed(self, n=None):
         self.np_random, seed = seeding.np_random(n)
         return [seed]
 
     def close(self):
```

### Comparing `ma_gym-0.0.8/ma_gym/envs/lumberjacks/lumberjacks.py` & `ma_gym-0.0.9/ma_gym/envs/lumberjacks/lumberjacks.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,24 +79,26 @@
 
         self._grid_shape = grid_shape
         self.n_agents = n_agents
         self._n_trees = n_trees
         self._agent_view = agent_view
         self.full_observable = full_observable
         self._step_cost = step_cost
+        self._step_count = None
         self._tree_cutdown_reward = tree_cutdown_reward
         self._max_steps = max_steps
         self.steps_beyond_done = 0
         self.seed()
 
         self._agents = []  # List[Agent]
         # In order to speed up the environment we used the advantage of vector operations.
         # Therefor we need to pad the grid size by the maximum agent_view size.
         # Relative coordinates refer to the coordinates in non pad grid. These are the only
         # coordinates visible to user. Extended coordinates refer to the coordinates in pad grid.
+        self.__init_pos = None
         self._agent_map = None
         self._tree_map = None
         self._total_episode_reward = None
         self._agent_dones = None
 
         mask_size = np.prod(tuple(2 * v + 1 for v in self._agent_view))
         # Agent ID (1) + Pos (2) + Step (1) + Neighborhood (2 * mask_size)
@@ -165,27 +167,45 @@
         return relative_coordinates[0] + self._agent_view[0], relative_coordinates[1] + self._agent_view[1]
 
     def _to_relative_coordinates(self, extended_coordinates):
         """Translate extended coordinates in to the relative coordinates."""
         return extended_coordinates[0] - self._agent_view[0], extended_coordinates[1] - self._agent_view[1]
 
     def _generate_init_pos(self) -> np.ndarray:
-        """Returns randomly selected initial positions for agents and trees in relative coordinates.
+        """Returns randomly selected initial positions for agents and trees
+        in relative coordinates.
 
         No agent or trees share the same cell in initial positions.
         """
         init_pos = np.array(
             [PRE_IDS['agent']] * self.n_agents +
             [PRE_IDS['tree']] * self._n_trees +
             [PRE_IDS['empty']] * (np.prod(self._grid_shape) - self.n_agents - self._n_trees)
         )
-        self.np_random.shuffle(init_pos)
+
+        # We ensure initial grid position is not same as last episode's
+        # initial position. Though, just shuffling the array is sufficient,
+        # we do validate and iterate to ensure change in position. If it still
+        # remains same, we issue a warning and continue with the configuration.
+        if self.__init_pos is not None:
+            _shuffle_counter = 0
+            self.np_random.shuffle(init_pos)
+            while not all(self.__init_pos == init_pos):
+                self.np_random.shuffle(init_pos)
+                _shuffle_counter += 1
+                if _shuffle_counter > 10:
+                    logger.warning("Grid configuration same as last episode")
+                    break
+        self.__init_pos = init_pos
         return np.reshape(init_pos, self._grid_shape)
 
     def render(self, mode='human'):
+        assert (self._step_count is not None), \
+            "Call reset before using render method."
+
         img = copy.copy(self._base_img)
 
         mask = (
             slice(self._agent_view[0], self._agent_view[0] + self._grid_shape[0]),
             slice(self._agent_view[1], self._agent_view[1] + self._grid_shape[1]),
         )
 
@@ -216,15 +236,16 @@
             from gym.envs.classic_control import rendering
             if self._viewer is None:
                 self._viewer = rendering.SimpleImageViewer()
             self._viewer.imshow(img)
             return self._viewer.isopen
 
     def _view_generator(self, mask: Tuple[slice, slice]) -> Tuple[Coordinates, int, int]:
-        """Yields position, number of agent and tree strength for all cells defined by `mask`.
+        """Yields position, number of agent and tree strength for all cells
+        defined by `mask`.
 
         Args:
             mask: tuple of slices in extended coordinates.
         """
         agent_iter = np.ndenumerate(np.sum(self._agent_map[mask], axis=2))
         tree_iter = np.nditer(self._tree_map[mask])
         for (pos, n_a), n_t in zip(agent_iter, tree_iter):
@@ -265,14 +286,16 @@
         mask = (
             slice(pos[0] - view_range[0], pos[0] + view_range[0] + 1),
             slice(pos[1] - view_range[1], pos[1] + view_range[1] + 1),
         )
         yield from self._view_generator(mask)
 
     def step(self, agents_action: List[int]):
+        assert (self._step_count is not None), \
+            "Call reset before using step method."
         # Assert would slow down the environment which is undesirable. We rather expect the check on the user side.
         # assert len(agents_action) == self.n_agents
 
         # Following snippet of code was refereed from:
         # https://github.com/openai/gym/blob/master/gym/envs/classic_control/cartpole.py#L124
         if all(self._agent_dones):
             if self.steps_beyond_done == 0:
```

### Comparing `ma_gym-0.0.8/ma_gym/envs/openai/__init__.py` & `ma_gym-0.0.9/ma_gym/envs/openai/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,17 +12,19 @@
         self.n_agents = 1
         self._step_count = None
         self._total_episode_reward = None
         self._agent_dones = [None for _ in range(self.n_agents)]
 
         self.action_space = MultiAgentActionSpace([self.env.action_space])
         self.observation_space = MultiAgentObservationSpace([self.env.observation_space])
-        self._step_count = 0
 
     def step(self, action_n):
+        assert (self._step_count is not None), \
+            "Call reset before using step method."
+
         self._step_count += 1
         assert len(action_n) == self.n_agents
 
         action = action_n[0]
         obs, reward, done, info = self.env.step(action)
 
         # Following is a hack:
```

### Comparing `ma_gym-0.0.8/ma_gym/envs/pong_duel/pong_duel.py` & `ma_gym-0.0.9/ma_gym/envs/pong_duel/pong_duel.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,15 @@
         self._grid_shape = (40, 30)
         self.n_agents = 2
         self.reward = reward
         self._max_rounds = max_rounds
         self.action_space = MultiAgentActionSpace([spaces.Discrete(3) for _ in range(self.n_agents)])
 
         self._step_count = None
+        self._steps_beyond_done = None
         self._step_cost = step_cost
         self._total_episode_reward = None
         self.agent_pos = {_: None for _ in range(self.n_agents)}
         self._agent_dones = None
         self.ball_pos = None
         self.__rounds = None
 
@@ -110,14 +111,15 @@
         self.agent_pos[1] = (self.np_random.randint(PADDLE_SIZE, self._grid_shape[0] - PADDLE_SIZE - 1),
                              self._grid_shape[1] - 2)
         self.agent_prev_pos = {_: self.agent_pos[_] for _ in range(self.n_agents)}
         self.__init_ball_pos()
         self._agent_dones = [False, False]
         self.__init_full_obs()
         self._step_count = 0
+        self._steps_beyond_done = None
         self._total_episode_reward = [0 for _ in range(self.n_agents)]
 
         return self.get_agent_obs()
 
     @property
     def __ball_cells(self):
         if self.curr_ball_dir == 'E':
@@ -134,14 +136,17 @@
             return [self.ball_pos, [self.ball_pos[0] - 1, self.ball_pos[1] - 1],
                     [self.ball_pos[0] - 2, self.ball_pos[1] - 2]]
         if self.curr_ball_dir == 'SW':
             return [self.ball_pos, [self.ball_pos[0] - 1, self.ball_pos[1] + 1],
                     [self.ball_pos[0] - 2, self.ball_pos[1] + 2]]
 
     def render(self, mode='human'):
+        assert (self._step_count is not None), \
+            "Call reset before using render method."
+
         img = copy.copy(self._base_img)
         for agent_i in range(self.n_agents):
             for row in range(self.agent_pos[agent_i][0] - 2, self.agent_pos[agent_i][0] + 3):
                 fill_cell(img, (row, self.agent_pos[agent_i][1]), cell_size=CELL_SIZE, fill=AGENT_COLORS[agent_i])
 
         ball_cells = self.__ball_cells
         fill_cell(img, ball_cells[0], cell_size=CELL_SIZE, fill=BALL_HEAD_COLOR)
@@ -227,14 +232,17 @@
         self.ball_pos = new_ball_pos
 
     def seed(self, n=None):
         self.np_random, seed = seeding.np_random(n)
         return [seed]
 
     def step(self, action_n):
+        assert (self._step_count is not None), \
+            "Call reset before using step method."
+
         assert len(action_n) == self.n_agents
         self._step_count += 1
         rewards = [self._step_cost for _ in range(self.n_agents)]
 
         # if ball is beyond paddle, initiate a new round
         if self.ball_pos[1] < 1:
             rewards = [0, self.reward]
@@ -253,14 +261,29 @@
                 self.__init_ball_pos()
             else:
                 self.__update_ball_pos()
 
         for i in range(self.n_agents):
             self._total_episode_reward[i] += rewards[i]
 
+        # Check for episode overflow
+        if all(self._agent_dones):
+            if self._steps_beyond_done is None:
+                self._steps_beyond_done = 0
+            else:
+                if self._steps_beyond_done == 0:
+                    logger.warn(
+                        "You are calling 'step()' even though this "
+                        "environment has already returned all(done) = True. You "
+                        "should always call 'reset()' once you receive "
+                        "'all(done) = True' -- any further steps are undefined "
+                        "behavior."
+                    )
+                self._steps_beyond_done += 1
+
         return self.get_agent_obs(), rewards, self._agent_dones, {'rounds': self.__rounds}
 
 
 CELL_SIZE = 5
 
 ACTION_MEANING = {
     0: "NOOP",
```

### Comparing `ma_gym-0.0.8/ma_gym/envs/predator_prey/predator_prey.py` & `ma_gym-0.0.9/ma_gym/envs/predator_prey/predator_prey.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,24 +34,33 @@
     The terminating condition of this task is when all preys are caught by more than one predator.
     For every new episodes , preys are initialized into random locations. Also, preys never move by themself into
     predator's neighbourhood
     """
     metadata = {'render.modes': ['human', 'rgb_array']}
 
     def __init__(self, grid_shape=(5, 5), n_agents=2, n_preys=1, prey_move_probs=(0.175, 0.175, 0.175, 0.175, 0.3),
-                 full_observable=False, penalty=-0.5, step_cost=-0.01, prey_capture_reward=5, max_steps=100):
+                 full_observable=False, penalty=-0.5, step_cost=-0.01, prey_capture_reward=5, max_steps=100,
+                 agent_view_mask=(5, 5)):
+        assert len(grid_shape) == 2, 'expected a tuple of size 2 for grid_shape, but found {}'.format(grid_shape)
+        assert len(agent_view_mask) == 2, 'expected a tuple of size 2 for agent view mask,' \
+                                          ' but found {}'.format(agent_view_mask)
+        assert grid_shape[0] > 0 and grid_shape[1] > 0, 'grid shape should be > 0'
+        assert 0 < agent_view_mask[0] <= grid_shape[0], 'agent view mask has to be within (0,{}]'.format(grid_shape[0])
+        assert 0 < agent_view_mask[1] <= grid_shape[1], 'agent view mask has to be within (0,{}]'.format(grid_shape[1])
+
         self._grid_shape = grid_shape
         self.n_agents = n_agents
         self.n_preys = n_preys
         self._max_steps = max_steps
         self._step_count = None
+        self._steps_beyond_done = None
         self._penalty = penalty
         self._step_cost = step_cost
         self._prey_capture_reward = prey_capture_reward
-        self._agent_view_mask = (5, 5)
+        self._agent_view_mask = agent_view_mask
 
         self.action_space = MultiAgentActionSpace([spaces.Discrete(5) for _ in range(self.n_agents)])
         self.agent_pos = {_: None for _ in range(self.n_agents)}
         self.prey_pos = {_: None for _ in range(self.n_preys)}
         self._prey_alive = None
 
         self._base_grid = self.__create_grid()  # with no agents
@@ -64,15 +73,16 @@
         # agent pos (2), prey (25), step (1)
         mask_size = np.prod(self._agent_view_mask)
         self._obs_high = np.array([1., 1.] + [1.] * mask_size + [1.0], dtype=np.float32)
         self._obs_low = np.array([0., 0.] + [0.] * mask_size + [0.0], dtype=np.float32)
         if self.full_observable:
             self._obs_high = np.tile(self._obs_high, self.n_agents)
             self._obs_low = np.tile(self._obs_low, self.n_agents)
-        self.observation_space = MultiAgentObservationSpace([spaces.Box(self._obs_low, self._obs_high) for _ in range(self.n_agents)])
+        self.observation_space = MultiAgentObservationSpace(
+            [spaces.Box(self._obs_low, self._obs_high) for _ in range(self.n_agents)])
 
         self._total_episode_reward = None
         self.seed()
 
     def get_action_meanings(self, agent_i=None):
         if agent_i is not None:
             assert agent_i <= self.n_agents
@@ -91,35 +101,37 @@
         return _grid
 
     def __init_full_obs(self):
         self._full_obs = self.__create_grid()
 
         for agent_i in range(self.n_agents):
             while True:
-                pos = [self.np_random.randint(0, self._grid_shape[0] - 1), self.np_random.randint(0, self._grid_shape[1] - 1)]
+                pos = [self.np_random.randint(0, self._grid_shape[0] - 1),
+                       self.np_random.randint(0, self._grid_shape[1] - 1)]
                 if self._is_cell_vacant(pos):
                     self.agent_pos[agent_i] = pos
                     break
             self.__update_agent_view(agent_i)
 
         for prey_i in range(self.n_preys):
             while True:
-                pos = [self.np_random.randint(0, self._grid_shape[0] - 1), self.np_random.randint(0, self._grid_shape[1] - 1)]
+                pos = [self.np_random.randint(0, self._grid_shape[0] - 1),
+                       self.np_random.randint(0, self._grid_shape[1] - 1)]
                 if self._is_cell_vacant(pos) and (self._neighbour_agents(pos)[0] == 0):
                     self.prey_pos[prey_i] = pos
                     break
             self.__update_prey_view(prey_i)
 
         self.__draw_base_img()
 
     def get_agent_obs(self):
         _obs = []
         for agent_i in range(self.n_agents):
             pos = self.agent_pos[agent_i]
-            _agent_i_obs = [pos[0] / (self._grid_shape[0] - 1), pos[1] / (self._grid_shape[1] - 1)] # coordinates
+            _agent_i_obs = [pos[0] / (self._grid_shape[0] - 1), pos[1] / (self._grid_shape[1] - 1)]  # coordinates
 
             # check if prey is in the view area
             _prey_pos = np.zeros(self._agent_view_mask)  # prey location in neighbour
             for row in range(max(0, pos[0] - 2), min(pos[0] + 2 + 1, self._grid_shape[0])):
                 for col in range(max(0, pos[1] - 2), min(pos[1] + 2 + 1, self._grid_shape[1])):
                     if PRE_IDS['prey'] in self._full_obs[row][col]:
                         _prey_pos[row - (pos[0] - 2), col - (pos[1] - 2)] = 1  # get relative position for the prey loc.
@@ -136,14 +148,15 @@
     def reset(self):
         self._total_episode_reward = [0 for _ in range(self.n_agents)]
         self.agent_pos = {}
         self.prey_pos = {}
 
         self.__init_full_obs()
         self._step_count = 0
+        self._steps_beyond_done = None
         self._agent_dones = [False for _ in range(self.n_agents)]
         self._prey_alive = [True for _ in range(self.n_preys)]
 
         return self.get_agent_obs()
 
     def __wall_exists(self, pos):
         row, col = pos
@@ -242,14 +255,17 @@
 
         agent_id = []
         for x, y in neighbours_xy:
             agent_id.append(int(self._full_obs[x][y].split(PRE_IDS['agent'])[1]) - 1)
         return _count, agent_id
 
     def step(self, agents_action):
+        assert (self._step_count is not None), \
+            "Call reset before using step method."
+
         self._step_count += 1
         rewards = [self._step_cost for _ in range(self.n_agents)]
 
         for agent_i, action in enumerate(agents_action):
             if not (self._agent_dones[agent_i]):
                 self.__update_agent_pos(agent_i, action)
 
@@ -279,14 +295,29 @@
         if (self._step_count >= self._max_steps) or (True not in self._prey_alive):
             for i in range(self.n_agents):
                 self._agent_dones[i] = True
 
         for i in range(self.n_agents):
             self._total_episode_reward[i] += rewards[i]
 
+        # Check for episode overflow
+        if all(self._agent_dones):
+            if self._steps_beyond_done is None:
+                self._steps_beyond_done = 0
+            else:
+                if self._steps_beyond_done == 0:
+                    logger.warn(
+                        "You are calling 'step()' even though this "
+                        "environment has already returned all(done) = True. You "
+                        "should always call 'reset()' once you receive "
+                        "'all(done) = True' -- any further steps are undefined "
+                        "behavior."
+                    )
+                self._steps_beyond_done += 1
+
         return self.get_agent_obs(), rewards, self._agent_dones, {'prey_alive': self._prey_alive}
 
     def __get_neighbour_coordinates(self, pos):
         neighbours = []
         if self.is_valid([pos[0] + 1, pos[1]]):
             neighbours.append([pos[0] + 1, pos[1]])
         if self.is_valid([pos[0] - 1, pos[1]]):
@@ -294,14 +325,17 @@
         if self.is_valid([pos[0], pos[1] + 1]):
             neighbours.append([pos[0], pos[1] + 1])
         if self.is_valid([pos[0], pos[1] - 1]):
             neighbours.append([pos[0], pos[1] - 1])
         return neighbours
 
     def render(self, mode='human'):
+        assert (self._step_count is not None), \
+            "Call reset before using render method."
+
         img = copy.copy(self._base_img)
         for agent_i in range(self.n_agents):
             for neighbour in self.__get_neighbour_coordinates(self.agent_pos[agent_i]):
                 fill_cell(img, neighbour, cell_size=CELL_SIZE, fill=AGENT_NEIGHBORHOOD_COLOR, margin=0.1)
             fill_cell(img, self.agent_pos[agent_i], cell_size=CELL_SIZE, fill=AGENT_NEIGHBORHOOD_COLOR, margin=0.1)
 
         for agent_i in range(self.n_agents):
```

### Comparing `ma_gym-0.0.8/ma_gym/envs/switch/switch_one_corridor.py` & `ma_gym-0.0.9/ma_gym/envs/switch/switch_one_corridor.py`

 * *Files 3% similar despite different names*

```diff
@@ -144,14 +144,17 @@
     def __update_agent_view(self, agent_i):
         self._full_obs[self.agent_pos[agent_i][0], self.agent_pos[agent_i][1]] = agent_i + 1
 
     def __is_agent_done(self, agent_i):
         return self.agent_pos[agent_i] == self.final_agent_pos[agent_i]
 
     def step(self, agents_action):
+        assert (self._step_count is not None), \
+            "Call reset before using step method."
+
         self._step_count += 1
         rewards = [self._step_cost for _ in range(self.n_agents)]
         for agent_i, action in enumerate(agents_action):
             if not (self._agent_dones[agent_i]):
                 self.__update_agent_pos(agent_i, action)
 
                 self._agent_dones[agent_i] = self.__is_agent_done(agent_i)
@@ -166,14 +169,17 @@
 
         for i in range(self.n_agents):
             self._total_episode_reward[i] += rewards[i]
 
         return self.get_agent_obs(), rewards, self._agent_dones, {}
 
     def render(self, mode='human'):
+        assert (self._step_count is not None), \
+            "Call reset before using render method."
+
         img = copy.copy(self._base_img)
         for agent_i in range(self.n_agents):
             draw_circle(img, self.agent_pos[agent_i], cell_size=CELL_SIZE, fill=AGENT_COLORS[agent_i], radius=0.3)
             write_cell_text(img, text=str(agent_i + 1), pos=self.agent_pos[agent_i], cell_size=CELL_SIZE,
                             fill='white', margin=0.4)
         img = np.asarray(img)
```

### Comparing `ma_gym-0.0.8/ma_gym/envs/traffic_junction/traffic_junction.py` & `ma_gym-0.0.9/ma_gym/envs/traffic_junction/traffic_junction.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         assert 0 <= arrive_prob <= 1, "arrive probability should be in range [0,1]"
         assert len(grid_shape) == 2, 'only 2-d grids are acceptable'
         assert 1 <= max_steps, "max_steps should be more than 1"
 
         self._grid_shape = grid_shape
         self.n_agents = n_max
         self._max_steps = max_steps
-        self._step_count = 0  # environment step counter
+        self._step_count = None  # environment step counter
         self._collision_reward = collision_reward
         self._total_episode_reward = None
         self._arrive_prob = arrive_prob
         self._n_max = n_max
         self._step_cost = step_cost
         self.curr_cars_count = 0
         self._n_routes = 3
```

### Comparing `ma_gym-0.0.8/ma_gym/envs/utils/draw.py` & `ma_gym-0.0.9/ma_gym/envs/utils/draw.py`

 * *Files identical despite different names*

### Comparing `ma_gym-0.0.8/ma_gym/envs/utils/observation_space.py` & `ma_gym-0.0.9/ma_gym/envs/utils/observation_space.py`

 * *Files identical despite different names*

### Comparing `ma_gym-0.0.8/ma_gym/wrappers/monitor.py` & `ma_gym-0.0.9/ma_gym/wrappers/monitor.py`

 * *Files identical despite different names*

### Comparing `ma_gym-0.0.8/ma_gym.egg-info/PKG-INFO` & `ma_gym-0.0.9/ma_gym.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ma-gym
-Version: 0.0.8
+Version: 0.0.9
 Summary: A collection of multi agent environments based on OpenAI gym.
 Home-page: https://github.com/koulanurag/ma-gym
 Author: Anurag Koul
 Author-email: koulanurag@gmail.com
 License: MIT License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
@@ -19,23 +19,23 @@
 
 # ma-gym
 It's a collection of multi agent environments based on OpenAI gym. Also, you can use [**minimal-marl**](https://github.com/koulanurag/minimal-marl) to warm-start training of agents.
 
 ![Python package](https://github.com/koulanurag/ma-gym/workflows/Python%20package/badge.svg) 
 ![Upload Python Package](https://github.com/koulanurag/ma-gym/workflows/Upload%20Python%20Package/badge.svg)
 [![Wiki Docs](https://img.shields.io/badge/-Wiki%20Docs-informational?style=flat)](https://github.com/koulanurag/ma-gym/wiki)
-
+[![Papers using ma-gym](https://img.shields.io/badge/-Papers%20using%20ma--gym-9cf?style=flat&logo=googlescholar)](https://scholar.google.com/scholar?hl=en&as_sdt=5,38&cites=14123576959169220642,12284637994392993807&scipsc=&q=&scisbd=1)
 
 ## Installation
 Using PyPI:
 ```bash
 pip install ma-gym
 ```
 
-Directly from source:
+Directly from source (recommended):
 ```bash
 git clone https://github.com/koulanurag/ma-gym.git
 cd ma-gym
 pip install -e .
 ```
 ## Reference:
 Please use this bibtex if you would like to cite it:
```

### Comparing `ma_gym-0.0.8/ma_gym.egg-info/SOURCES.txt` & `ma_gym-0.0.9/ma_gym.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ma_gym-0.0.8/setup.py` & `ma_gym-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     'develop': ['imageio'],
 }
 
 # Meta dependency groups.
 extras['all'] = [item for group in extras.values() for item in group]
 
 setup(name='ma_gym',
-      version='0.0.8',
+      version='0.0.9',
       description='A collection of multi agent environments based on OpenAI gym.',
       long_description_content_type='text/markdown',
       long_description=open(path.join(path.abspath(path.dirname(__file__)), 'README.md'), encoding='utf-8').read(),
       url='https://github.com/koulanurag/ma-gym',
       author='Anurag Koul',
       author_email='koulanurag@gmail.com',
       license='MIT License',
```

### Comparing `ma_gym-0.0.8/tests/envs/test_checkers.py` & `ma_gym-0.0.9/tests/envs/test_checkers.py`

 * *Files identical despite different names*

### Comparing `ma_gym-0.0.8/tests/envs/test_combat.py` & `ma_gym-0.0.9/tests/envs/test_combat.py`

 * *Files identical despite different names*

### Comparing `ma_gym-0.0.8/tests/envs/test_lumberjacks.py` & `ma_gym-0.0.9/tests/envs/test_lumberjacks.py`

 * *Files identical despite different names*

### Comparing `ma_gym-0.0.8/tests/envs/test_openai_cartpole.py` & `ma_gym-0.0.9/tests/envs/test_openai_cartpole.py`

 * *Files identical despite different names*

### Comparing `ma_gym-0.0.8/tests/envs/test_pong_duel.py` & `ma_gym-0.0.9/tests/envs/test_pong_duel.py`

 * *Files identical despite different names*

### Comparing `ma_gym-0.0.8/tests/envs/test_predatorprey5x5.py` & `ma_gym-0.0.9/tests/envs/test_predatorprey5x5.py`

 * *Files identical despite different names*

### Comparing `ma_gym-0.0.8/tests/envs/test_predatorprey7x7.py` & `ma_gym-0.0.9/tests/envs/test_predatorprey7x7.py`

 * *Files identical despite different names*

### Comparing `ma_gym-0.0.8/tests/envs/test_switch2.py` & `ma_gym-0.0.9/tests/envs/test_switch2.py`

 * *Files identical despite different names*

### Comparing `ma_gym-0.0.8/tests/envs/test_trafficjunction.py` & `ma_gym-0.0.9/tests/envs/test_trafficjunction.py`

 * *Files identical despite different names*

