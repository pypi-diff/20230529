# Comparing `tmp/baboo_game-2.0.6.tar.gz` & `tmp/baboo_game-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baboo_game-2.0.6.tar", last modified: Mon May 29 19:52:05 2023, max compression
+gzip compressed data, was "baboo_game-2.1.0.tar", last modified: Mon May 29 20:15:30 2023, max compression
```

## Comparing `baboo_game-2.0.6.tar` & `baboo_game-2.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:52:05.922050 baboo_game-2.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-29 19:51:54.000000 baboo_game-2.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-05-29 19:52:05.922050 baboo_game-2.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-05-29 19:51:54.000000 baboo_game-2.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-29 19:51:54.000000 baboo_game-2.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 19:52:05.922050 baboo_game-2.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:52:05.918050 baboo_game-2.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:52:05.918050 baboo_game-2.0.6/src/baboo_game/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 19:51:54.000000 baboo_game-2.0.6/src/baboo_game/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:52:05.922050 baboo_game-2.0.6/src/baboo_game/game/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 19:51:54.000000 baboo_game-2.0.6/src/baboo_game/game/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-29 19:51:54.000000 baboo_game-2.0.6/src/baboo_game/game/baboo_game.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:52:05.922050 baboo_game-2.0.6/src/baboo_game/game/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 19:51:54.000000 baboo_game-2.0.6/src/baboo_game/game/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-29 19:51:54.000000 baboo_game-2.0.6/src/baboo_game/game/config/color_config.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-29 19:51:54.000000 baboo_game-2.0.6/src/baboo_game/game/config/game_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    15031 2023-05-29 19:51:54.000000 baboo_game-2.0.6/src/baboo_game/game/config/text_constant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:52:05.922050 baboo_game-2.0.6/src/baboo_game/game/library/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 19:51:54.000000 baboo_game-2.0.6/src/baboo_game/game/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-05-29 19:51:54.000000 baboo_game-2.0.6/src/baboo_game/game/library/abstract_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-05-29 19:51:54.000000 baboo_game-2.0.6/src/baboo_game/game/render_game.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-29 19:51:54.000000 baboo_game-2.0.6/src/baboo_game/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:52:05.922050 baboo_game-2.0.6/src/baboo_game.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-05-29 19:52:05.000000 baboo_game-2.0.6/src/baboo_game.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-29 19:52:05.000000 baboo_game-2.0.6/src/baboo_game.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 19:52:05.000000 baboo_game-2.0.6/src/baboo_game.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-29 19:52:05.000000 baboo_game-2.0.6/src/baboo_game.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-29 19:52:05.000000 baboo_game-2.0.6/src/baboo_game.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:15:30.949332 baboo_game-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-29 20:15:18.000000 baboo_game-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-05-29 20:15:30.949332 baboo_game-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-05-29 20:15:18.000000 baboo_game-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-29 20:15:18.000000 baboo_game-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 20:15:30.949332 baboo_game-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:15:30.945332 baboo_game-2.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:15:30.945332 baboo_game-2.1.0/src/baboo_game/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 20:15:18.000000 baboo_game-2.1.0/src/baboo_game/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:15:30.945332 baboo_game-2.1.0/src/baboo_game/game/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 20:15:18.000000 baboo_game-2.1.0/src/baboo_game/game/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-29 20:15:18.000000 baboo_game-2.1.0/src/baboo_game/game/baboo_game.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:15:30.949332 baboo_game-2.1.0/src/baboo_game/game/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 20:15:18.000000 baboo_game-2.1.0/src/baboo_game/game/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-29 20:15:18.000000 baboo_game-2.1.0/src/baboo_game/game/config/color_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-29 20:15:18.000000 baboo_game-2.1.0/src/baboo_game/game/config/game_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15031 2023-05-29 20:15:18.000000 baboo_game-2.1.0/src/baboo_game/game/config/text_constant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:15:30.949332 baboo_game-2.1.0/src/baboo_game/game/library/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 20:15:18.000000 baboo_game-2.1.0/src/baboo_game/game/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-05-29 20:15:18.000000 baboo_game-2.1.0/src/baboo_game/game/library/abstract_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-05-29 20:15:18.000000 baboo_game-2.1.0/src/baboo_game/game/render_game.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-29 20:15:18.000000 baboo_game-2.1.0/src/baboo_game/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:15:30.945332 baboo_game-2.1.0/src/baboo_game.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-05-29 20:15:30.000000 baboo_game-2.1.0/src/baboo_game.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-29 20:15:30.000000 baboo_game-2.1.0/src/baboo_game.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 20:15:30.000000 baboo_game-2.1.0/src/baboo_game.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-29 20:15:30.000000 baboo_game-2.1.0/src/baboo_game.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-29 20:15:30.000000 baboo_game-2.1.0/src/baboo_game.egg-info/top_level.txt
```

### Comparing `baboo_game-2.0.6/LICENSE` & `baboo_game-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `baboo_game-2.0.6/PKG-INFO` & `baboo_game-2.1.0/src/baboo_game.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: baboo_game
-Version: 2.0.6
+Name: baboo-game
+Version: 2.1.0
 Summary: A dice game prototype
 Author-email: Vitalii Sili <vitaliisili@yahoo.com>
 License: MIT License
         
         Copyright (c) 2023 Vitalii Sili
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -45,14 +45,21 @@
 ![PyPI version](https://img.shields.io/pypi/v/baboo-game)
 ![Watchers](https://img.shields.io/github/watchers/vitaliisili/dice_game_python?style=social)
 
 #### *Welcome to Baboo Dice Game, an exciting and addictive dice game that will test your luck and strategy!* 
 
 ![baboo](https://lh3.googleusercontent.com/pw/AJFCJaWOlNjWnEZ6Lcp7Z8AE3YGCv1CaVTXDX-9VXJxfnNVw_Qljmyfhx-khr0Shs1wI2oESp3tbQ8dmKpcmOHViL-OoKLZE10lQ1qUbnz7cikdgstf7bFq7fds7V1WK7DTMOjJejmubcV0MMieJMfxASOtl=w577-h433-s-no)
 
+*Gather your friends, set up the scoreboards, 
+and prepare to dive into the thrilling world 
+of Baboo Dice Game. Roll the dice, make strategic 
+choices, and aim for the highest score to emerge 
+as the ultimate dice champion! It's time to test
+your luck, strategy, and decision-making skills 
+in this addictive and enjoyable dice game.*
 
 ## How to run
 ### ***Method 1***:  *Download or Clone source file:*
 - Step 1: Clone repository to your local machine and open the folder
 ```bash
 git clone https://github.com/vitaliisili/dice_game_python
 ```
@@ -83,8 +90,8 @@
 
 - Step 3: Run game
 ```python
 main.start()
 ```
 ***If you need `Virtual Environment` in Python look [here](https://www.freecodecamp.org/news/how-to-setup-virtual-environments-in-python/)***
 
-![baboo](https://lh3.googleusercontent.com/X7hyBNThwuGC8wtWoppQGLgBvrI_AU0f3iQVFhDCQKEEQkgu6mBQBWk-nhkMr3B93irG-irKeCyI0nGTB45Om9y0-ggG9OfUK8J09wThBaywgFzrAJjIJuz2BCQZMJwM6XWMDoT0RCB_c2V5GOHh86io2UkA_uHQotaJjaBTnHCcLFmlNaqc4_pZeWLPqfjHgqPMIbbaU3tRMqdY1p4eWipxRz-AoditSV3NQ3vuBCL0-PwZNP0_M5oXjfYNqmcrcomtjcJUtelpHVCuxdhDymyxL_FnW_P-OrbrM56r7dOsXlwxX2JIQbov0dhODjoA4wh6LSZATjlWlTOS_7Qp6RqKdZ3fPSOITFjShcxLNHA0P3vCN0j61FAVqyQ6tr9qDO5H7Y67kpMuyE0MJ281F79XIi43uohz_gk_7aXEP8WcoyfLKF2gTAJsRypIU7UUNdfHnnYzpEVcSsxXN81N2gPzA2wIJE6NEX91CxrAT7ZqcDelUuOSBJoK8fOOYaAcOZq4LK8gSyW7sCwqfyk677_FIBkh-uW84Z_7F2WMQSqzzZ4ieFLKoLo-C8V41-f9_hElxfzfw5nGWTkAZ4qtpchPjnLESt6uj_ZShAZqtLXRONi1zNoosj8nA1qxbaIBpPSjtFpapKhdf1q6PX91GT1dh0FffrBarX0pvUo3HCZNlTQCE15sD6i1egS-FGfTrRHYorx-R5rqa_TFLMZ6WynRyEC3zkjkdt39HsQL0Ved4SNQ9Chyd1mfRF9Dc9c887OAMULniI3Q2mBCOHKt0lKr0-qGbvIFFAwo7zklNrZxAOVoVR4i64Uzqd13e8abWbuPA_Tx1xRUiyRXP3zz1XAHM9r3VrwWEruJFxtS6qMXZsCXrEBSgDdBcQ780TaDdDTOuiCln_P2-hoSRAzpaOppcMVMjP_OPfs5bm0ZVWs0JbZAYAPIpHn4xPTnPlvy5o_JIX25unGeWSGnBweU=w800-h600-s-no?authuser=0)
+![baboo](https://lh3.googleusercontent.com/bX55HaA98EqlNIre9gkICrZ7Cndd0qMowjG5TkgpkNK3IE2YRF2UA94Rj6-ucKaySz9E3Yx60VR2dfNkCCZAowZbNwmeQTWM0dJZQoANHFXohCvnBbI9gpMQa9YLXjoT9lGmEnJAZRDSpm9Vb9Ix6-MAMJ-LLp2zd3zaBJbRsphWTv_tVzmJDFM7_-xTeu0fShmpW7Yrka9sx7ISIm67-Lr_Y3vzieRllStQ5cZyCUp0Lc_eg6nig5PNIPE-bpUbYelskEiOEVKovq9l9_ggt4VXuk7mLlpmfMOtLpL7m8qpG2KK2pEljOeHcfUkcahfNgEPOsCKroy3GwGT4xKwD7SguwW7kzvFUlFUaGJlAd-mSFa7O4jY5GRMDw4Y0MLBdoRPAHcKBKYf36GrssVRUYp3TcDLtW2cDkHi6Hdzmvupek1xJ22AxLKCy7wJTMSMLEVyEuBbS0wt-xS5zfoUWH5GepUgNSoOUvWCQm86TZ6c1G4oahIPqNwMo5ALTalyb0SmshQKy0NZCxNJihXROTxA5Mgl1D85dnKIrbdYG29Vy6hGhAloNnSoq9287jfm5__om5y6Xbm7auum8MimVt9eZ4akGsI-_LaVB1LNMSM_KFHFt_Uvgxf_5RvWomuPti_vKlZ21Eg8NsKbIi5LXTnOqIfbn-dGqlrfvjHE1siM2D2l7hsWwb_SC3FEyunAErNmg_CFi8-GpahlRL3OSUIhbpFbKWctV04Z1_yQ3vfDnhnmb_2qrxIr5-3nJhxvp6IwrmxtIYp266qwSem28QIysbV-ubUADQuQ92h8LnZpN8Lp-BzGHz3-sfeHKRAICQmpCTSFCA9rEIjslCTpard1pxp56az3apgz2aERIUEhefvdV4pcmB-9zc-vpiW2Yxs_nFRB1PteTPiNGnwpOB0qN89mOilrQ97eaB2L4eKAXDT6SOJpiYAvimtI4PbBYswKuN_ZTlanj5FdULpV=w800-h600-s-no?authuser=0)
```

### Comparing `baboo_game-2.0.6/README.md` & `baboo_game-2.1.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -5,14 +5,21 @@
 ![PyPI version](https://img.shields.io/pypi/v/baboo-game)
 ![Watchers](https://img.shields.io/github/watchers/vitaliisili/dice_game_python?style=social)
 
 #### *Welcome to Baboo Dice Game, an exciting and addictive dice game that will test your luck and strategy!* 
 
 ![baboo](https://lh3.googleusercontent.com/pw/AJFCJaWOlNjWnEZ6Lcp7Z8AE3YGCv1CaVTXDX-9VXJxfnNVw_Qljmyfhx-khr0Shs1wI2oESp3tbQ8dmKpcmOHViL-OoKLZE10lQ1qUbnz7cikdgstf7bFq7fds7V1WK7DTMOjJejmubcV0MMieJMfxASOtl=w577-h433-s-no)
 
+*Gather your friends, set up the scoreboards, 
+and prepare to dive into the thrilling world 
+of Baboo Dice Game. Roll the dice, make strategic 
+choices, and aim for the highest score to emerge 
+as the ultimate dice champion! It's time to test
+your luck, strategy, and decision-making skills 
+in this addictive and enjoyable dice game.*
 
 ## How to run
 ### ***Method 1***:  *Download or Clone source file:*
 - Step 1: Clone repository to your local machine and open the folder
 ```bash
 git clone https://github.com/vitaliisili/dice_game_python
 ```
@@ -43,8 +50,8 @@
 
 - Step 3: Run game
 ```python
 main.start()
 ```
 ***If you need `Virtual Environment` in Python look [here](https://www.freecodecamp.org/news/how-to-setup-virtual-environments-in-python/)***
 
-![baboo](https://lh3.googleusercontent.com/X7hyBNThwuGC8wtWoppQGLgBvrI_AU0f3iQVFhDCQKEEQkgu6mBQBWk-nhkMr3B93irG-irKeCyI0nGTB45Om9y0-ggG9OfUK8J09wThBaywgFzrAJjIJuz2BCQZMJwM6XWMDoT0RCB_c2V5GOHh86io2UkA_uHQotaJjaBTnHCcLFmlNaqc4_pZeWLPqfjHgqPMIbbaU3tRMqdY1p4eWipxRz-AoditSV3NQ3vuBCL0-PwZNP0_M5oXjfYNqmcrcomtjcJUtelpHVCuxdhDymyxL_FnW_P-OrbrM56r7dOsXlwxX2JIQbov0dhODjoA4wh6LSZATjlWlTOS_7Qp6RqKdZ3fPSOITFjShcxLNHA0P3vCN0j61FAVqyQ6tr9qDO5H7Y67kpMuyE0MJ281F79XIi43uohz_gk_7aXEP8WcoyfLKF2gTAJsRypIU7UUNdfHnnYzpEVcSsxXN81N2gPzA2wIJE6NEX91CxrAT7ZqcDelUuOSBJoK8fOOYaAcOZq4LK8gSyW7sCwqfyk677_FIBkh-uW84Z_7F2WMQSqzzZ4ieFLKoLo-C8V41-f9_hElxfzfw5nGWTkAZ4qtpchPjnLESt6uj_ZShAZqtLXRONi1zNoosj8nA1qxbaIBpPSjtFpapKhdf1q6PX91GT1dh0FffrBarX0pvUo3HCZNlTQCE15sD6i1egS-FGfTrRHYorx-R5rqa_TFLMZ6WynRyEC3zkjkdt39HsQL0Ved4SNQ9Chyd1mfRF9Dc9c887OAMULniI3Q2mBCOHKt0lKr0-qGbvIFFAwo7zklNrZxAOVoVR4i64Uzqd13e8abWbuPA_Tx1xRUiyRXP3zz1XAHM9r3VrwWEruJFxtS6qMXZsCXrEBSgDdBcQ780TaDdDTOuiCln_P2-hoSRAzpaOppcMVMjP_OPfs5bm0ZVWs0JbZAYAPIpHn4xPTnPlvy5o_JIX25unGeWSGnBweU=w800-h600-s-no?authuser=0)
+![baboo](https://lh3.googleusercontent.com/bX55HaA98EqlNIre9gkICrZ7Cndd0qMowjG5TkgpkNK3IE2YRF2UA94Rj6-ucKaySz9E3Yx60VR2dfNkCCZAowZbNwmeQTWM0dJZQoANHFXohCvnBbI9gpMQa9YLXjoT9lGmEnJAZRDSpm9Vb9Ix6-MAMJ-LLp2zd3zaBJbRsphWTv_tVzmJDFM7_-xTeu0fShmpW7Yrka9sx7ISIm67-Lr_Y3vzieRllStQ5cZyCUp0Lc_eg6nig5PNIPE-bpUbYelskEiOEVKovq9l9_ggt4VXuk7mLlpmfMOtLpL7m8qpG2KK2pEljOeHcfUkcahfNgEPOsCKroy3GwGT4xKwD7SguwW7kzvFUlFUaGJlAd-mSFa7O4jY5GRMDw4Y0MLBdoRPAHcKBKYf36GrssVRUYp3TcDLtW2cDkHi6Hdzmvupek1xJ22AxLKCy7wJTMSMLEVyEuBbS0wt-xS5zfoUWH5GepUgNSoOUvWCQm86TZ6c1G4oahIPqNwMo5ALTalyb0SmshQKy0NZCxNJihXROTxA5Mgl1D85dnKIrbdYG29Vy6hGhAloNnSoq9287jfm5__om5y6Xbm7auum8MimVt9eZ4akGsI-_LaVB1LNMSM_KFHFt_Uvgxf_5RvWomuPti_vKlZ21Eg8NsKbIi5LXTnOqIfbn-dGqlrfvjHE1siM2D2l7hsWwb_SC3FEyunAErNmg_CFi8-GpahlRL3OSUIhbpFbKWctV04Z1_yQ3vfDnhnmb_2qrxIr5-3nJhxvp6IwrmxtIYp266qwSem28QIysbV-ubUADQuQ92h8LnZpN8Lp-BzGHz3-sfeHKRAICQmpCTSFCA9rEIjslCTpard1pxp56az3apgz2aERIUEhefvdV4pcmB-9zc-vpiW2Yxs_nFRB1PteTPiNGnwpOB0qN89mOilrQ97eaB2L4eKAXDT6SOJpiYAvimtI4PbBYswKuN_ZTlanj5FdULpV=w800-h600-s-no?authuser=0)
```

### Comparing `baboo_game-2.0.6/pyproject.toml` & `baboo_game-2.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "baboo_game"
-version = "2.0.6" # Insert manual version
+version = "2.1.0" # Insert manual version
 authors = [
    { name="Vitalii Sili", email="vitaliisili@yahoo.com" },
 ]
 license = {file = "LICENSE"}
 description = "A dice game prototype"
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `baboo_game-2.0.6/src/baboo_game/game/baboo_game.py` & `baboo_game-2.1.0/src/baboo_game/game/baboo_game.py`

 * *Files identical despite different names*

### Comparing `baboo_game-2.0.6/src/baboo_game/game/config/text_constant.py` & `baboo_game-2.1.0/src/baboo_game/game/config/text_constant.py`

 * *Files identical despite different names*

### Comparing `baboo_game-2.0.6/src/baboo_game/game/library/abstract_dice.py` & `baboo_game-2.1.0/src/baboo_game/game/library/abstract_dice.py`

 * *Files identical despite different names*

### Comparing `baboo_game-2.0.6/src/baboo_game/game/render_game.py` & `baboo_game-2.1.0/src/baboo_game/game/render_game.py`

 * *Files identical despite different names*

### Comparing `baboo_game-2.0.6/src/baboo_game.egg-info/PKG-INFO` & `baboo_game-2.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: baboo-game
-Version: 2.0.6
+Name: baboo_game
+Version: 2.1.0
 Summary: A dice game prototype
 Author-email: Vitalii Sili <vitaliisili@yahoo.com>
 License: MIT License
         
         Copyright (c) 2023 Vitalii Sili
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -45,14 +45,21 @@
 ![PyPI version](https://img.shields.io/pypi/v/baboo-game)
 ![Watchers](https://img.shields.io/github/watchers/vitaliisili/dice_game_python?style=social)
 
 #### *Welcome to Baboo Dice Game, an exciting and addictive dice game that will test your luck and strategy!* 
 
 ![baboo](https://lh3.googleusercontent.com/pw/AJFCJaWOlNjWnEZ6Lcp7Z8AE3YGCv1CaVTXDX-9VXJxfnNVw_Qljmyfhx-khr0Shs1wI2oESp3tbQ8dmKpcmOHViL-OoKLZE10lQ1qUbnz7cikdgstf7bFq7fds7V1WK7DTMOjJejmubcV0MMieJMfxASOtl=w577-h433-s-no)
 
+*Gather your friends, set up the scoreboards, 
+and prepare to dive into the thrilling world 
+of Baboo Dice Game. Roll the dice, make strategic 
+choices, and aim for the highest score to emerge 
+as the ultimate dice champion! It's time to test
+your luck, strategy, and decision-making skills 
+in this addictive and enjoyable dice game.*
 
 ## How to run
 ### ***Method 1***:  *Download or Clone source file:*
 - Step 1: Clone repository to your local machine and open the folder
 ```bash
 git clone https://github.com/vitaliisili/dice_game_python
 ```
@@ -83,8 +90,8 @@
 
 - Step 3: Run game
 ```python
 main.start()
 ```
 ***If you need `Virtual Environment` in Python look [here](https://www.freecodecamp.org/news/how-to-setup-virtual-environments-in-python/)***
 
-![baboo](https://lh3.googleusercontent.com/X7hyBNThwuGC8wtWoppQGLgBvrI_AU0f3iQVFhDCQKEEQkgu6mBQBWk-nhkMr3B93irG-irKeCyI0nGTB45Om9y0-ggG9OfUK8J09wThBaywgFzrAJjIJuz2BCQZMJwM6XWMDoT0RCB_c2V5GOHh86io2UkA_uHQotaJjaBTnHCcLFmlNaqc4_pZeWLPqfjHgqPMIbbaU3tRMqdY1p4eWipxRz-AoditSV3NQ3vuBCL0-PwZNP0_M5oXjfYNqmcrcomtjcJUtelpHVCuxdhDymyxL_FnW_P-OrbrM56r7dOsXlwxX2JIQbov0dhODjoA4wh6LSZATjlWlTOS_7Qp6RqKdZ3fPSOITFjShcxLNHA0P3vCN0j61FAVqyQ6tr9qDO5H7Y67kpMuyE0MJ281F79XIi43uohz_gk_7aXEP8WcoyfLKF2gTAJsRypIU7UUNdfHnnYzpEVcSsxXN81N2gPzA2wIJE6NEX91CxrAT7ZqcDelUuOSBJoK8fOOYaAcOZq4LK8gSyW7sCwqfyk677_FIBkh-uW84Z_7F2WMQSqzzZ4ieFLKoLo-C8V41-f9_hElxfzfw5nGWTkAZ4qtpchPjnLESt6uj_ZShAZqtLXRONi1zNoosj8nA1qxbaIBpPSjtFpapKhdf1q6PX91GT1dh0FffrBarX0pvUo3HCZNlTQCE15sD6i1egS-FGfTrRHYorx-R5rqa_TFLMZ6WynRyEC3zkjkdt39HsQL0Ved4SNQ9Chyd1mfRF9Dc9c887OAMULniI3Q2mBCOHKt0lKr0-qGbvIFFAwo7zklNrZxAOVoVR4i64Uzqd13e8abWbuPA_Tx1xRUiyRXP3zz1XAHM9r3VrwWEruJFxtS6qMXZsCXrEBSgDdBcQ780TaDdDTOuiCln_P2-hoSRAzpaOppcMVMjP_OPfs5bm0ZVWs0JbZAYAPIpHn4xPTnPlvy5o_JIX25unGeWSGnBweU=w800-h600-s-no?authuser=0)
+![baboo](https://lh3.googleusercontent.com/bX55HaA98EqlNIre9gkICrZ7Cndd0qMowjG5TkgpkNK3IE2YRF2UA94Rj6-ucKaySz9E3Yx60VR2dfNkCCZAowZbNwmeQTWM0dJZQoANHFXohCvnBbI9gpMQa9YLXjoT9lGmEnJAZRDSpm9Vb9Ix6-MAMJ-LLp2zd3zaBJbRsphWTv_tVzmJDFM7_-xTeu0fShmpW7Yrka9sx7ISIm67-Lr_Y3vzieRllStQ5cZyCUp0Lc_eg6nig5PNIPE-bpUbYelskEiOEVKovq9l9_ggt4VXuk7mLlpmfMOtLpL7m8qpG2KK2pEljOeHcfUkcahfNgEPOsCKroy3GwGT4xKwD7SguwW7kzvFUlFUaGJlAd-mSFa7O4jY5GRMDw4Y0MLBdoRPAHcKBKYf36GrssVRUYp3TcDLtW2cDkHi6Hdzmvupek1xJ22AxLKCy7wJTMSMLEVyEuBbS0wt-xS5zfoUWH5GepUgNSoOUvWCQm86TZ6c1G4oahIPqNwMo5ALTalyb0SmshQKy0NZCxNJihXROTxA5Mgl1D85dnKIrbdYG29Vy6hGhAloNnSoq9287jfm5__om5y6Xbm7auum8MimVt9eZ4akGsI-_LaVB1LNMSM_KFHFt_Uvgxf_5RvWomuPti_vKlZ21Eg8NsKbIi5LXTnOqIfbn-dGqlrfvjHE1siM2D2l7hsWwb_SC3FEyunAErNmg_CFi8-GpahlRL3OSUIhbpFbKWctV04Z1_yQ3vfDnhnmb_2qrxIr5-3nJhxvp6IwrmxtIYp266qwSem28QIysbV-ubUADQuQ92h8LnZpN8Lp-BzGHz3-sfeHKRAICQmpCTSFCA9rEIjslCTpard1pxp56az3apgz2aERIUEhefvdV4pcmB-9zc-vpiW2Yxs_nFRB1PteTPiNGnwpOB0qN89mOilrQ97eaB2L4eKAXDT6SOJpiYAvimtI4PbBYswKuN_ZTlanj5FdULpV=w800-h600-s-no?authuser=0)
```

### Comparing `baboo_game-2.0.6/src/baboo_game.egg-info/SOURCES.txt` & `baboo_game-2.1.0/src/baboo_game.egg-info/SOURCES.txt`

 * *Files identical despite different names*

