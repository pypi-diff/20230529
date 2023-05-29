# Comparing `tmp/ikabot-6.6.1.tar.gz` & `tmp/ikabot-6.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ikabot-6.6.1.tar", last modified: Mon May 15 14:22:15 2023, max compression
+gzip compressed data, was "ikabot-6.6.2.tar", last modified: Mon May 29 18:09:18 2023, max compression
```

## Comparing `ikabot-6.6.1.tar` & `ikabot-6.6.2.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-15 14:22:15.977108 ikabot-6.6.1/
--rw-r--r--   0 user      (1000) user      (1000)     1064 2023-05-15 14:21:42.000000 ikabot-6.6.1/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)       56 2023-05-15 14:21:42.000000 ikabot-6.6.1/MANIFEST.in
--rw-r--r--   0 user      (1000) user      (1000)      318 2023-05-15 14:22:15.977108 ikabot-6.6.1/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)    11217 2023-05-15 14:21:42.000000 ikabot-6.6.1/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-15 14:22:15.967108 ikabot-6.6.1/ikabot/
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)       44 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/__main__.py
--rwxr-xr-x   0 user      (1000) user      (1000)     7575 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/command_line.py
--rw-r--r--   0 user      (1000) user      (1000)     2058 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/config.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-15 14:22:15.970441 ikabot-6.6.1/ikabot/function/
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/function/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)    10994 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/function/activateMiracle.py
--rw-r--r--   0 user      (1000) user      (1000)     5770 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/function/alertAttacks.py
--rw-r--r--   0 user      (1000) user      (1000)     3959 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/function/alertLowWine.py
--rw-r--r--   0 user      (1000) user      (1000)    20485 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/function/attackBarbarians.py
--rw-r--r--   0 user      (1000) user      (1000)    10947 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/function/autoPirate.py
--rw-r--r--   0 user      (1000) user      (1000)    11003 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/function/buyResources.py
--rw-r--r--   0 user      (1000) user      (1000)      674 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/function/checkForUpdate.py
--rw-r--r--   0 user      (1000) user      (1000)     4148 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/function/constructBuilding.py
--rw-r--r--   0 user      (1000) user      (1000)    20942 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/function/constructionList.py
--rw-r--r--   0 user      (1000) user      (1000)    51779 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/function/decaptchaConf.py
--rw-r--r--   0 user      (1000) user      (1000)    11987 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/function/distributeResources.py
--rw-r--r--   0 user      (1000) user      (1000)     5996 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/function/donate.py
--rw-r--r--   0 user      (1000) user      (1000)     5182 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/function/donationBot.py
--rw-r--r--   0 user      (1000) user      (1000)    19423 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/function/dumpWorld.py
--rw-r--r--   0 user      (1000) user      (1000)     6301 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/function/getStatus.py
--rw-r--r--   0 user      (1000) user      (1000)     3285 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/function/importExportCookie.py
--rw-r--r--   0 user      (1000) user      (1000)     6332 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/function/investigate.py
--rw-r--r--   0 user      (1000) user      (1000)     2004 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/function/killTasks.py
--rw-r--r--   0 user      (1000) user      (1000)     2271 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/function/loginDaily.py
--rw-r--r--   0 user      (1000) user      (1000)     3954 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/function/proxyConf.py
--rw-r--r--   0 user      (1000) user      (1000)     6754 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/function/searchForIslandSpaces.py
--rw-r--r--   0 user      (1000) user      (1000)    13699 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/function/sellResources.py
--rw-r--r--   0 user      (1000) user      (1000)     4717 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/function/sendResources.py
--rw-r--r--   0 user      (1000) user      (1000)     4325 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/function/shipMovements.py
--rw-r--r--   0 user      (1000) user      (1000)    11734 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/function/trainArmy.py
--rw-r--r--   0 user      (1000) user      (1000)      886 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/function/update.py
--rw-r--r--   0 user      (1000) user      (1000)     1538 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/function/vacationMode.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-15 14:22:15.973775 ikabot-6.6.1/ikabot/helpers/
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/helpers/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     5116 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/helpers/aesCipher.py
--rw-r--r--   0 user      (1000) user      (1000)    10072 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/helpers/botComm.py
--rw-r--r--   0 user      (1000) user      (1000)     5028 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/helpers/getJson.py
--rw-r--r--   0 user      (1000) user      (1000)     1684 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/helpers/gui.py
--rw-r--r--   0 user      (1000) user      (1000)     2493 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/helpers/market.py
--rw-r--r--   0 user      (1000) user      (1000)      868 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/helpers/naval.py
--rw-r--r--   0 user      (1000) user      (1000)     9333 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/helpers/pedirInfo.py
--rw-r--r--   0 user      (1000) user      (1000)     7340 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/helpers/planRoutes.py
--rw-r--r--   0 user      (1000) user      (1000)     2296 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/helpers/process.py
--rw-r--r--   0 user      (1000) user      (1000)     1977 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/helpers/resources.py
--rw-r--r--   0 user      (1000) user      (1000)     1150 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/helpers/signals.py
--rw-r--r--   0 user      (1000) user      (1000)     2298 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/helpers/varios.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-15 14:22:15.963775 ikabot-6.6.1/ikabot/locale/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-15 14:22:15.963775 ikabot-6.6.1/ikabot/locale/es/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-15 14:22:15.977108 ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/
--rw-r--r--   0 user      (1000) user      (1000)     2828 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/activateMiracle.po
--rw-r--r--   0 user      (1000) user      (1000)      719 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/aesCipher.po
--rw-r--r--   0 user      (1000) user      (1000)     1995 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/alertAttacks.po
--rw-r--r--   0 user      (1000) user      (1000)     1481 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/alertLowWine.po
--rw-r--r--   0 user      (1000) user      (1000)     2219 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/botComm.po
--rw-r--r--   0 user      (1000) user      (1000)     2417 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/buyResources.po
--rw-r--r--   0 user      (1000) user      (1000)      575 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/checkForUpdate.po
--rw-r--r--   0 user      (1000) user      (1000)     2432 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/command_line.po
--rw-r--r--   0 user      (1000) user      (1000)      755 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/config.po
--rw-r--r--   0 user      (1000) user      (1000)     1001 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/constructBuilding.po
--rw-r--r--   0 user      (1000) user      (1000)     4367 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/constructionList.po
--rw-r--r--   0 user      (1000) user      (1000)     1547 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/distributeResources.po
--rw-r--r--   0 user      (1000) user      (1000)     1416 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/donate.po
--rw-r--r--   0 user      (1000) user      (1000)     1628 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/donationBot.po
--rw-r--r--   0 user      (1000) user      (1000)     1673 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/getStatus.po
--rw-r--r--   0 user      (1000) user      (1000)      376 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/gui.mo
--rw-r--r--   0 user      (1000) user      (1000)      553 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/gui.po
--rw-r--r--   0 user      (1000) user      (1000)      841 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/loginDaily.po
--rw-r--r--   0 user      (1000) user      (1000)      837 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/pedirInfo.mo
--rw-r--r--   0 user      (1000) user      (1000)     1255 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/pedirInfo.po
--rw-r--r--   0 user      (1000) user      (1000)     1235 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/searchForIslandSpaces.po
--rw-r--r--   0 user      (1000) user      (1000)     2792 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/sellResources.po
--rw-r--r--   0 user      (1000) user      (1000)     3510 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/sendResources.po
--rw-r--r--   0 user      (1000) user      (1000)     1253 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/session.mo
--rw-r--r--   0 user      (1000) user      (1000)     1828 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/session.po
--rw-r--r--   0 user      (1000) user      (1000)     1350 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/shipMovements.po
--rw-r--r--   0 user      (1000) user      (1000)      497 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/signals.mo
--rw-r--r--   0 user      (1000) user      (1000)      715 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/signals.po
--rw-r--r--   0 user      (1000) user      (1000)     2464 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/trainArmy.pot
--rw-r--r--   0 user      (1000) user      (1000)     3175 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/trainFleets.po
--rw-r--r--   0 user      (1000) user      (1000)     3169 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/trainTroops.po
--rw-r--r--   0 user      (1000) user      (1000)      579 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/update.po
--rw-r--r--   0 user      (1000) user      (1000)      717 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/vacationMode.po
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-15 14:22:15.977108 ikabot-6.6.1/ikabot/web/
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/web/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)    43966 2023-05-15 14:21:42.000000 ikabot-6.6.1/ikabot/web/session.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-15 14:22:15.967108 ikabot-6.6.1/ikabot.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)      318 2023-05-15 14:22:15.000000 ikabot-6.6.1/ikabot.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     3024 2023-05-15 14:22:15.000000 ikabot-6.6.1/ikabot.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-15 14:22:15.000000 ikabot-6.6.1/ikabot.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       52 2023-05-15 14:22:15.000000 ikabot-6.6.1/ikabot.egg-info/entry_points.txt
--rw-r--r--   0 user      (1000) user      (1000)       45 2023-05-15 14:22:15.000000 ikabot-6.6.1/ikabot.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)        7 2023-05-15 14:22:15.000000 ikabot-6.6.1/ikabot.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-05-15 14:22:15.977108 ikabot-6.6.1/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)      655 2023-05-15 14:21:42.000000 ikabot-6.6.1/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-29 18:09:18.209533 ikabot-6.6.2/
+-rw-r--r--   0 user      (1000) user      (1000)     1064 2023-05-29 18:08:27.000000 ikabot-6.6.2/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)       56 2023-05-29 18:08:27.000000 ikabot-6.6.2/MANIFEST.in
+-rw-r--r--   0 user      (1000) user      (1000)      318 2023-05-29 18:09:18.209533 ikabot-6.6.2/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)    11289 2023-05-29 18:08:27.000000 ikabot-6.6.2/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-29 18:09:18.199533 ikabot-6.6.2/ikabot/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)       44 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/__main__.py
+-rwxr-xr-x   0 user      (1000) user      (1000)     8466 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/command_line.py
+-rw-r--r--   0 user      (1000) user      (1000)     2058 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/config.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-29 18:09:18.206200 ikabot-6.6.2/ikabot/function/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/function/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)    11102 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/function/activateMiracle.py
+-rw-r--r--   0 user      (1000) user      (1000)     5770 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/function/alertAttacks.py
+-rw-r--r--   0 user      (1000) user      (1000)     3959 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/function/alertLowWine.py
+-rw-r--r--   0 user      (1000) user      (1000)    20485 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/function/attackBarbarians.py
+-rw-r--r--   0 user      (1000) user      (1000)    14049 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/function/autoPirate.py
+-rw-r--r--   0 user      (1000) user      (1000)    11133 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/function/buyResources.py
+-rw-r--r--   0 user      (1000) user      (1000)      674 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/function/checkForUpdate.py
+-rw-r--r--   0 user      (1000) user      (1000)     4148 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/function/constructBuilding.py
+-rw-r--r--   0 user      (1000) user      (1000)    20942 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/function/constructionList.py
+-rw-r--r--   0 user      (1000) user      (1000)    51779 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/function/decaptchaConf.py
+-rw-r--r--   0 user      (1000) user      (1000)    11987 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/function/distributeResources.py
+-rw-r--r--   0 user      (1000) user      (1000)     5996 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/function/donate.py
+-rw-r--r--   0 user      (1000) user      (1000)     5182 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/function/donationBot.py
+-rw-r--r--   0 user      (1000) user      (1000)    19423 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/function/dumpWorld.py
+-rw-r--r--   0 user      (1000) user      (1000)     6671 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/function/getStatus.py
+-rw-r--r--   0 user      (1000) user      (1000)     3285 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/function/importExportCookie.py
+-rw-r--r--   0 user      (1000) user      (1000)     6332 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/function/investigate.py
+-rw-r--r--   0 user      (1000) user      (1000)     2004 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/function/killTasks.py
+-rw-r--r--   0 user      (1000) user      (1000)     2271 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/function/loginDaily.py
+-rw-r--r--   0 user      (1000) user      (1000)     3954 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/function/proxyConf.py
+-rw-r--r--   0 user      (1000) user      (1000)     6754 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/function/searchForIslandSpaces.py
+-rw-r--r--   0 user      (1000) user      (1000)    13699 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/function/sellResources.py
+-rw-r--r--   0 user      (1000) user      (1000)     4717 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/function/sendResources.py
+-rw-r--r--   0 user      (1000) user      (1000)     4325 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/function/shipMovements.py
+-rw-r--r--   0 user      (1000) user      (1000)    11734 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/function/trainArmy.py
+-rw-r--r--   0 user      (1000) user      (1000)      886 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/function/update.py
+-rw-r--r--   0 user      (1000) user      (1000)     1538 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/function/vacationMode.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-29 18:09:18.206200 ikabot-6.6.2/ikabot/helpers/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/helpers/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     5392 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/helpers/aesCipher.py
+-rw-r--r--   0 user      (1000) user      (1000)    10072 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/helpers/botComm.py
+-rw-r--r--   0 user      (1000) user      (1000)     5028 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/helpers/getJson.py
+-rw-r--r--   0 user      (1000) user      (1000)     1684 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/helpers/gui.py
+-rw-r--r--   0 user      (1000) user      (1000)     2493 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/helpers/market.py
+-rw-r--r--   0 user      (1000) user      (1000)      868 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/helpers/naval.py
+-rw-r--r--   0 user      (1000) user      (1000)     9333 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/helpers/pedirInfo.py
+-rw-r--r--   0 user      (1000) user      (1000)     7340 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/helpers/planRoutes.py
+-rw-r--r--   0 user      (1000) user      (1000)     2296 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/helpers/process.py
+-rw-r--r--   0 user      (1000) user      (1000)     1977 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/helpers/resources.py
+-rw-r--r--   0 user      (1000) user      (1000)     1150 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/helpers/signals.py
+-rw-r--r--   0 user      (1000) user      (1000)     2298 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/helpers/varios.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-29 18:09:18.199533 ikabot-6.6.2/ikabot/locale/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-29 18:09:18.199533 ikabot-6.6.2/ikabot/locale/es/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-29 18:09:18.209533 ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/
+-rw-r--r--   0 user      (1000) user      (1000)     2828 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/activateMiracle.po
+-rw-r--r--   0 user      (1000) user      (1000)      719 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/aesCipher.po
+-rw-r--r--   0 user      (1000) user      (1000)     1995 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/alertAttacks.po
+-rw-r--r--   0 user      (1000) user      (1000)     1481 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/alertLowWine.po
+-rw-r--r--   0 user      (1000) user      (1000)     2219 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/botComm.po
+-rw-r--r--   0 user      (1000) user      (1000)     2417 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/buyResources.po
+-rw-r--r--   0 user      (1000) user      (1000)      575 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/checkForUpdate.po
+-rw-r--r--   0 user      (1000) user      (1000)     2432 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/command_line.po
+-rw-r--r--   0 user      (1000) user      (1000)      755 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/config.po
+-rw-r--r--   0 user      (1000) user      (1000)     1001 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/constructBuilding.po
+-rw-r--r--   0 user      (1000) user      (1000)     4367 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/constructionList.po
+-rw-r--r--   0 user      (1000) user      (1000)     1547 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/distributeResources.po
+-rw-r--r--   0 user      (1000) user      (1000)     1416 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/donate.po
+-rw-r--r--   0 user      (1000) user      (1000)     1628 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/donationBot.po
+-rw-r--r--   0 user      (1000) user      (1000)     1673 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/getStatus.po
+-rw-r--r--   0 user      (1000) user      (1000)      376 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/gui.mo
+-rw-r--r--   0 user      (1000) user      (1000)      553 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/gui.po
+-rw-r--r--   0 user      (1000) user      (1000)      841 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/loginDaily.po
+-rw-r--r--   0 user      (1000) user      (1000)      837 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/pedirInfo.mo
+-rw-r--r--   0 user      (1000) user      (1000)     1255 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/pedirInfo.po
+-rw-r--r--   0 user      (1000) user      (1000)     1235 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/searchForIslandSpaces.po
+-rw-r--r--   0 user      (1000) user      (1000)     2792 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/sellResources.po
+-rw-r--r--   0 user      (1000) user      (1000)     3510 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/sendResources.po
+-rw-r--r--   0 user      (1000) user      (1000)     1253 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/session.mo
+-rw-r--r--   0 user      (1000) user      (1000)     1828 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/session.po
+-rw-r--r--   0 user      (1000) user      (1000)     1350 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/shipMovements.po
+-rw-r--r--   0 user      (1000) user      (1000)      497 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/signals.mo
+-rw-r--r--   0 user      (1000) user      (1000)      715 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/signals.po
+-rw-r--r--   0 user      (1000) user      (1000)     2464 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/trainArmy.pot
+-rw-r--r--   0 user      (1000) user      (1000)     3175 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/trainFleets.po
+-rw-r--r--   0 user      (1000) user      (1000)     3169 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/trainTroops.po
+-rw-r--r--   0 user      (1000) user      (1000)      579 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/update.po
+-rw-r--r--   0 user      (1000) user      (1000)      717 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/vacationMode.po
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-29 18:09:18.209533 ikabot-6.6.2/ikabot/web/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/web/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)    43966 2023-05-29 18:08:27.000000 ikabot-6.6.2/ikabot/web/session.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-29 18:09:18.202866 ikabot-6.6.2/ikabot.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)      318 2023-05-29 18:09:18.000000 ikabot-6.6.2/ikabot.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     3024 2023-05-29 18:09:18.000000 ikabot-6.6.2/ikabot.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-29 18:09:18.000000 ikabot-6.6.2/ikabot.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       52 2023-05-29 18:09:18.000000 ikabot-6.6.2/ikabot.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1000) user      (1000)       45 2023-05-29 18:09:18.000000 ikabot-6.6.2/ikabot.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)        7 2023-05-29 18:09:18.000000 ikabot-6.6.2/ikabot.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)       38 2023-05-29 18:09:18.209533 ikabot-6.6.2/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)      655 2023-05-29 18:08:27.000000 ikabot-6.6.2/setup.py
```

### Comparing `ikabot-6.6.1/LICENSE` & `ikabot-6.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/README.md` & `ikabot-6.6.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,37 +13,34 @@
 | # | Feature | Description |
 |--|--|--|
 | 0 | Exit | Closes the main menu, returning to the normal console. You can also use `ctrl-c`. When closing _ikabot_, all the actions that you configured will continue running in the background. If you want to see which actions are running, simply run _ikabot_ and log into the account from which you initiated those actions. You will be able to see their PIDs and will be able to kill them using `kill -9 [pid]` on Unix or using Task Manager on Windows |
 | 1 | Construction list | The user selects a building, the number of levels to upload, _ikabot_ calculates if it has enough resources and uploads the selected number of levels. If you don't have enough resources, it can send them automatically from the cities that you specify. |
 | 2 | Send resources |  It sends unlimited amount of resources from one city to another. It doesn't matter how many boats you have, _ikabot_ will send all the trips that were necessary. The destination city can be own by the user or by other. |
 | 3 | Distribute resources | It lets you distribute the type of resource in two possible ways: from the cities that produce it to cities that do not (very useful to send wine) and to distribute it evenly among all cities. |
 | 4 | Account status | It shows information such as levels of the buildings, time until the wine runs out, resources among other things from all the cities. |
-| 5 | Donate | It allows you to donate (WOW!). |
-| 6 | Search for new spaces | This functionality alerts by telegram, if a city disappears or if someone founds in any of the islands where the user has at least one city or any user defined island or set of islands. |
-| 7 | Login Daily | For those who do not want to spend a day without their account login. This feature also collects the ambrosia fountain if it is available. |
-| 8 | Alert attacks | It alerts by Telegram if you are going to be attacked. You can configure how often _ikabot_ checks for incoming attacks. |
-| 9 | Donate automatically | _Ikabot_ enters once a day and donates a percentage of the available wood from the selected cities to the luxury good or the forest. |
-| 10 | Alert wine running out | It warns you by Telegram when less than N hours are needed for a city to run out of wine. The number of hours is specified by the user. |
-| 11 | Buy resources | It allows you to choose what type of resource to buy and how much. It automatically purchases the different offers from the cheapest to the most expensive. |
-| 12 | Sell resources | It allows you to choose what type of resource to sell and how much. It does not matter how much storage you have, it automatically updates the offers as pĺayers buy from you. When it sells all the resources, it lets you know via Telegram. |
-| 13 | Activate Vacation Mode | Sets the account in vacation mode and closes _ikabot_. |
-| 14 | Activate miracle | It allows you to activate any miracle you have available as many times in a row as you want. |
-| 15 | Train army | It allows you to easily create large amounts of troops or fleets in one city. If there are not enough resources to train all of them, it will train all the units it can and when it finishes it will try to train the rest. It also allows you to build your army in multiple small steps so that you can use it as fast as possible. |
-| 16 | See movements | Let's you see movements coming to/from your cities. This includes attacks, transports, etc. |
-| 17 | Construct building | It allows you to contruct a building (WOW!, again). |
-| 18 | Update Ikabot | It tells you how to update _ikabot_ |
-| 19 | Import / Export cookie | You can use this feature to insert your _ikabot_ cookie into your browser or other _ikabot_ instances running on a different machine. This will result in _ikabot_ not logging you out of your browser Ikariam session. Keep in mind that logging into Ikariam from another browser will invalidate all previous cookies, and you will need to do this again if that happens. |
-| 20 | Auto-Pirate | This feature will run any available piracy mission as many times as you need it to. It will also attempt to automatically solve the captcha should it be presented with one. |
-| 21 | Investigate | It allows you to investigate an available research. |
-| 22 | Attack barbarians | Now you can attack the barbarians in an automated way. You can send your troops in many rounds and it will automatically collect the resources. |
-| 23 | Dump / View world | Create a dump file containing all data about the world you are playing on. You can also search this dump later for a specific player's cities or islands with specific miracles and forest / luxury resource levels. |
-| 25 | Configure Proxy | It lets you configure a proxy that will be used to all request except those sent to the lobby (during login). The proxy affects immediately all processes associated with the current ikariam username. |
-| 26 | Update the Telegram data | It allows you to set or change the Telegram data. |
-| 27 | Kill tasks | It allows you to end a currently-running ikabot task |
-| 28 | Configure captcha resolver | It allows you to configure your desired captcha resolver for the Auto-Pirate task. The options you have to choose from are: <ol><li>Default </li><li>Custom</li><li>9kw.eu</li><li>Telegram</li></ol> |
+| 5 | Monitor islands | This functionality alerts by telegram, if a city disappears or if someone creates a city in any of the islands where the user has at least one city or any user defined island or set of islands. |
+| 6 | Login Daily | For those who do not want to spend a day without their account login. This feature also collects the ambrosia fountain if it is available. |
+| 7 | Alerts / Notifications | **- Alert attacks**, it alerts by Telegram if you are going to be attacked. You can configure how often _ikabot_ checks for incoming attacks. <br /> **- Alert wine running out**, it warns you by Telegram when less than N hours are needed for a city to run out of wine. The number of hours is specified by the user.|
+| 8 | Marketplace | **- Buy resources**, it allows you to choose what type of resource to buy and how much. It automatically purchases the different offers from the cheapest to the most expensive. <br /> **- Sell resources**, it allows you to choose what type of resource to sell and how much. It does not matter how much storage you have, it automatically updates the offers as players buy from you. When it sells all the resources, it lets you know via Telegram. |
+| 9 | Donate | **- Donate**, it allows you to donate (WOW!). <br /> **- Donate automatically**, _Ikabot_ enters once a day and donates a percentage of the available wood from the selected cities to the luxury good or the forest. |
+| 10 | Activate Vacation Mode | Sets the account in vacation mode and closes _ikabot_. |
+| 11 | Activate miracle | It allows you to activate any miracle you have available as many times in a row as you want. |
+| 12 | Train army | It allows you to easily create large amounts of troops or fleets in one city. If there are not enough resources to train all of them, it will train all the units it can and when it finishes it will try to train the rest. It also allows you to build your army in multiple small steps so that you can use it as fast as possible. |
+| 13 | See movements | Let's you see movements coming to/from your cities. This includes attacks, transports, etc. |
+| 14 | Construct building | It allows you to contruct a building (WOW!, again). |
+| 15 | Update Ikabot | It tells you how to update _ikabot_ |
+| 16 | Import / Export cookie | You can use this feature to insert your _ikabot_ cookie into your browser or other _ikabot_ instances running on a different machine. This will result in _ikabot_ not logging you out of your browser Ikariam session. Keep in mind that logging into Ikariam from another browser will invalidate all previous cookies, and you will need to do this again if that happens. |
+| 17 | Auto-Pirate | This feature will run any available piracy mission as many times as you need it to. It will also attempt to automatically solve the captcha should it be presented with one. |
+| 18 | Investigate | It allows you to investigate an available research. |
+| 19 | Attack barbarians | Now you can attack the barbarians in an automated way. You can send your troops in many rounds and it will automatically collect the resources. |
+| 20 | Dump / View world | Create a dump file containing all data about the world you are playing on. You can also search this dump later for a specific player's cities or islands with specific miracles and forest / luxury resource levels. |
+| 22 | Configure Proxy | It lets you configure a proxy that will be used to all request except those sent to the lobby (during login). The proxy affects immediately all processes associated with the current ikariam username. |
+| 23 | Update the Telegram data | It allows you to set or change the Telegram data. |
+| 24 | Kill tasks | It allows you to end a currently-running ikabot task |
+| 25 | Configure captcha resolver | It allows you to configure your desired captcha resolver for the Auto-Pirate task. The options you have to choose from are: <ol><li>Default </li><li>Custom</li><li>9kw.eu</li><li>Telegram</li></ol> |
 
 # <img src="https://user-images.githubusercontent.com/54487782/236309220-b257d870-6846-4740-a855-dba89deeacaf.png" width="30" height="30"> Install
 
 ## Pre-built Windows binary
 
 You can use the pre-built _ikabot_ binary for Windows in the ikabot.zip file for a certain version [here](https://github.com/physics-sp/ikabot/releases)!
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -23,64 +23,66 @@
 doesn't matter how many boats you have, _ikabot_ will send all the trips that
 were necessary. The destination city can be own by the user or by other. | | 3
 | Distribute resources | It lets you distribute the type of resource in two
 possible ways: from the cities that produce it to cities that do not (very
 useful to send wine) and to distribute it evenly among all cities. | | 4 |
 Account status | It shows information such as levels of the buildings, time
 until the wine runs out, resources among other things from all the cities. | |
-5 | Donate | It allows you to donate (WOW!). | | 6 | Search for new spaces |
-This functionality alerts by telegram, if a city disappears or if someone
-founds in any of the islands where the user has at least one city or any user
-defined island or set of islands. | | 7 | Login Daily | For those who do not
-want to spend a day without their account login. This feature also collects the
-ambrosia fountain if it is available. | | 8 | Alert attacks | It alerts by
-Telegram if you are going to be attacked. You can configure how often _ikabot_
-checks for incoming attacks. | | 9 | Donate automatically | _Ikabot_ enters
-once a day and donates a percentage of the available wood from the selected
-cities to the luxury good or the forest. | | 10 | Alert wine running out | It
-warns you by Telegram when less than N hours are needed for a city to run out
-of wine. The number of hours is specified by the user. | | 11 | Buy resources |
-It allows you to choose what type of resource to buy and how much. It
-automatically purchases the different offers from the cheapest to the most
-expensive. | | 12 | Sell resources | It allows you to choose what type of
-resource to sell and how much. It does not matter how much storage you have, it
-automatically updates the offers as pÄºayers buy from you. When it sells all
-the resources, it lets you know via Telegram. | | 13 | Activate Vacation Mode |
-Sets the account in vacation mode and closes _ikabot_. | | 14 | Activate
-miracle | It allows you to activate any miracle you have available as many
-times in a row as you want. | | 15 | Train army | It allows you to easily
-create large amounts of troops or fleets in one city. If there are not enough
-resources to train all of them, it will train all the units it can and when it
-finishes it will try to train the rest. It also allows you to build your army
-in multiple small steps so that you can use it as fast as possible. | | 16 |
-See movements | Let's you see movements coming to/from your cities. This
-includes attacks, transports, etc. | | 17 | Construct building | It allows you
-to contruct a building (WOW!, again). | | 18 | Update Ikabot | It tells you how
-to update _ikabot_ | | 19 | Import / Export cookie | You can use this feature
-to insert your _ikabot_ cookie into your browser or other _ikabot_ instances
-running on a different machine. This will result in _ikabot_ not logging you
-out of your browser Ikariam session. Keep in mind that logging into Ikariam
-from another browser will invalidate all previous cookies, and you will need to
-do this again if that happens. | | 20 | Auto-Pirate | This feature will run any
-available piracy mission as many times as you need it to. It will also attempt
-to automatically solve the captcha should it be presented with one. | | 21 |
-Investigate | It allows you to investigate an available research. | | 22 |
-Attack barbarians | Now you can attack the barbarians in an automated way. You
-can send your troops in many rounds and it will automatically collect the
-resources. | | 23 | Dump / View world | Create a dump file containing all data
-about the world you are playing on. You can also search this dump later for a
-specific player's cities or islands with specific miracles and forest / luxury
-resource levels. | | 25 | Configure Proxy | It lets you configure a proxy that
-will be used to all request except those sent to the lobby (during login). The
-proxy affects immediately all processes associated with the current ikariam
-username. | | 26 | Update the Telegram data | It allows you to set or change
-the Telegram data. | | 27 | Kill tasks | It allows you to end a currently-
-running ikabot task | | 28 | Configure captcha resolver | It allows you to
-configure your desired captcha resolver for the Auto-Pirate task. The options
-you have to choose from are:
+5 | Monitor islands | This functionality alerts by telegram, if a city
+disappears or if someone creates a city in any of the islands where the user
+has at least one city or any user defined island or set of islands. | | 6 |
+Login Daily | For those who do not want to spend a day without their account
+login. This feature also collects the ambrosia fountain if it is available. | |
+7 | Alerts / Notifications | **- Alert attacks**, it alerts by Telegram if you
+are going to be attacked. You can configure how often _ikabot_ checks for
+incoming attacks.
+**- Alert wine running out**, it warns you by Telegram when less than N hours
+are needed for a city to run out of wine. The number of hours is specified by
+the user.| | 8 | Marketplace | **- Buy resources**, it allows you to choose
+what type of resource to buy and how much. It automatically purchases the
+different offers from the cheapest to the most expensive.
+**- Sell resources**, it allows you to choose what type of resource to sell and
+how much. It does not matter how much storage you have, it automatically
+updates the offers as players buy from you. When it sells all the resources, it
+lets you know via Telegram. | | 9 | Donate | **- Donate**, it allows you to
+donate (WOW!).
+**- Donate automatically**, _Ikabot_ enters once a day and donates a percentage
+of the available wood from the selected cities to the luxury good or the
+forest. | | 10 | Activate Vacation Mode | Sets the account in vacation mode and
+closes _ikabot_. | | 11 | Activate miracle | It allows you to activate any
+miracle you have available as many times in a row as you want. | | 12 | Train
+army | It allows you to easily create large amounts of troops or fleets in one
+city. If there are not enough resources to train all of them, it will train all
+the units it can and when it finishes it will try to train the rest. It also
+allows you to build your army in multiple small steps so that you can use it as
+fast as possible. | | 13 | See movements | Let's you see movements coming to/
+from your cities. This includes attacks, transports, etc. | | 14 | Construct
+building | It allows you to contruct a building (WOW!, again). | | 15 | Update
+Ikabot | It tells you how to update _ikabot_ | | 16 | Import / Export cookie |
+You can use this feature to insert your _ikabot_ cookie into your browser or
+other _ikabot_ instances running on a different machine. This will result in
+_ikabot_ not logging you out of your browser Ikariam session. Keep in mind that
+logging into Ikariam from another browser will invalidate all previous cookies,
+and you will need to do this again if that happens. | | 17 | Auto-Pirate | This
+feature will run any available piracy mission as many times as you need it to.
+It will also attempt to automatically solve the captcha should it be presented
+with one. | | 18 | Investigate | It allows you to investigate an available
+research. | | 19 | Attack barbarians | Now you can attack the barbarians in an
+automated way. You can send your troops in many rounds and it will
+automatically collect the resources. | | 20 | Dump / View world | Create a dump
+file containing all data about the world you are playing on. You can also
+search this dump later for a specific player's cities or islands with specific
+miracles and forest / luxury resource levels. | | 22 | Configure Proxy | It
+lets you configure a proxy that will be used to all request except those sent
+to the lobby (during login). The proxy affects immediately all processes
+associated with the current ikariam username. | | 23 | Update the Telegram data
+| It allows you to set or change the Telegram data. | | 24 | Kill tasks | It
+allows you to end a currently-running ikabot task | | 25 | Configure captcha
+resolver | It allows you to configure your desired captcha resolver for the
+Auto-Pirate task. The options you have to choose from are:
    1. Default
    2. Custom
    3. 9kw.eu
    4. Telegram
 | # [https://user-images.githubusercontent.com/54487782/236309220-b257d870-
 6846-4740-a855-dba89deeacaf.png] Install ## Pre-built Windows binary You can
 use the pre-built _ikabot_ binary for Windows in the ikabot.zip file for a
```

### Comparing `ikabot-6.6.1/ikabot/command_line.py` & `ikabot-6.6.2/ikabot/command_line.py`

 * *Files 12% similar despite different names*

```diff
@@ -72,68 +72,104 @@
         print('')
 
     menu_actions = {
         1:            constructionList,
         2:            sendResources,
         3:            distributeResources,
         4:            getStatus,
-        5:            donate,
-        6:            searchForIslandSpaces,
-        7:            loginDaily,
-        8:            alertAttacks,
-        9:            donationBot,
-        10:            alertLowWine,
-        11:            buyResources,
-        12:            sellResources,
-        13:            vacationMode,
-        14:            activateMiracle,
-        15:            trainArmy,
-        16:            shipMovements,
-        17:            constructBuilding,
-        18:            update,
-        19:            importExportCookie,
-        20:            autoPirate,
-        21:            investigate,
-        22:            attackBarbarians,
-        23:            dumpWorld,
-        25:            proxyConf,
-        26:            updateTelegramData,
-        27:            killTasks,
-        28:            decaptchaConf,
+        5:            searchForIslandSpaces,
+        6:            loginDaily,
+        101:            alertAttacks,
+        102:            alertLowWine,
+        111:            buyResources,
+        112:            sellResources,
+        121:            donate,
+        122:            donationBot,
+        10:            vacationMode,
+        11:            activateMiracle,
+        12:            trainArmy,
+        13:            shipMovements,
+        14:            constructBuilding,
+        15:            update,
+        16:            importExportCookie,
+        17:            autoPirate,
+        18:            investigate,
+        19:            attackBarbarians,
+        20:            dumpWorld,
+        22:            proxyConf,
+        23:            updateTelegramData,
+        24:            killTasks,
+        25:            decaptchaConf,
                     }
 
     print(_('(0)  Exit'))
     print(_('(1)  Construction list'))
     print(_('(2)  Send resources'))
     print(_('(3)  Distribute resources'))
     print(_('(4)  Account status'))
-    print(_('(5)  Donate'))
-    print(_('(6)  Search for new spaces'))
-    print(_('(7)  Login daily'))
-    print(_('(8)  Alert attacks'))
-    print(_('(9)  Donate automatically'))
-    print(_('(10) Alert wine running out'))
-    print(_('(11) Buy resources'))
-    print(_('(12) Sell resources'))
-    print(_('(13) Activate vacation mode'))
-    print(_('(14) Activate miracle'))
-    print(_('(15) Train army'))
-    print(_('(16) See movements'))
-    print(_('(17) Construct building'))
-    print(_('(18) Update Ikabot'))
-    print(_('(19) Import / Export cookie'))
-    print(_('(20) Auto-Pirate'))
-    print(_('(21) Investigate'))
-    print(_('(22) Attack barbarians'))
-    print(_('(23) Dump / View world'))
-    print(_('(24) Options / Settings'))
+    print(_('(5)  Monitor islands'))
+    print(_('(6)  Login daily'))
+    print(_('(7)  Alerts / Notifications'))
+    print(_('(8)  Marketplace'))
+    print(_('(9)  Donate'))
+    print(_('(10) Activate vacation mode'))
+    print(_('(11) Activate miracle'))
+    print(_('(12) Train army'))
+    print(_('(13) See movements'))
+    print(_('(14) Construct building'))
+    print(_('(15) Update Ikabot'))
+    print(_('(16) Import / Export cookie'))
+    print(_('(17) Auto-Pirate'))
+    print(_('(18) Investigate'))
+    print(_('(19) Attack barbarians'))
+    print(_('(20) Dump / View world'))
+    print(_('(21) Options / Settings'))
     total_options = len(menu_actions) + 1
     selected = read(min=0, max=total_options, digit=True)
+    
+    if selected == 7:
+        banner()
+        print(_('(0) Back'))
+        print(_('(1) Alert attacks'))
+        print(_('(2) Alert wine running out'))
+
+        selected = read(min=0, max=2, digit=True)
+        if selected == 0:
+            menu(session)
+            return
+        if selected > 0:
+            selected += 100
+            
+    if selected == 8:
+        banner()
+        print(_('(0) Back'))
+        print(_('(1) Buy resources'))
+        print(_('(2) Sell resources'))
+
+        selected = read(min=0, max=2, digit=True)
+        if selected == 0:
+            menu(session)
+            return
+        if selected > 0:
+            selected += 110
+            
+    if selected == 9:
+        banner()
+        print(_('(0) Back'))
+        print(_('(1) Donate once'))
+        print(_('(2) Donate automatically'))
+
+        selected = read(min=0, max=2, digit=True)
+        if selected == 0:
+            menu(session)
+            return
+        if selected > 0:
+            selected += 120
 
-    if selected == 24:
+    if selected == 21:
         banner()
         print(_('(0) Back'))
         print(_('(1) Configure Proxy'))
         if telegramDataIsValid(session):
             print(_('(2) Change the Telegram data'))
         else:
             print(_('(2) Enter the Telegram data'))
@@ -141,15 +177,15 @@
         print(_('(4) Configure captcha resolver'))
 
         selected = read(min=0, max=4, digit=True)
         if selected == 0:
             menu(session)
             return
         if selected > 0:
-            selected += 24
+            selected += 21
 
     if selected != 0:
         try:
             event = multiprocessing.Event()  # creates a new event
             process = multiprocessing.Process(target=menu_actions[selected], args=(session, event, sys.stdin.fileno(), config.predetermined_input), name=menu_actions[selected].__name__)
             process.start()
             process_list.append({'pid': process.pid, 'action': menu_actions[selected].__name__, 'date': time.time()})
```

### Comparing `ikabot-6.6.1/ikabot/config.py` & `ikabot-6.6.2/ikabot/config.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/function/activateMiracle.py` & `ikabot-6.6.2/ikabot/function/activateMiracle.py`

 * *Files 3% similar despite different names*

```diff
@@ -105,30 +105,31 @@
     islands : list[dict]
 
     Returns
     -------
     island : dict
     """
     print(_('Which miracle do you want to activate?'))
+    # Sort islands by name
+    sorted_islands = sorted(islands, key=lambda x: x['wonderName'])
     i = 0
     print(_('(0) Exit'))
-    for island in islands:
+    for island in sorted_islands:
         i += 1
         if island['available']:
             print('({:d}) {}'.format(i, island['wonderName']))
         else:
             print(_('({:d}) {} (available in: {})').format(i, island['wonderName'], daysHoursMinutes(island['available_in'])))
 
     index = read(min=0, max=i)
     if index == 0:
         return None
-    island = islands[index - 1]
+    island = sorted_islands[index - 1]
     return island
 
-
 def activateMiracle(session, event, stdin_fd, predetermined_input):
     """
     Parameters
     ----------
     session : ikabot.web.session.Session
     event : multiprocessing.Event
     stdin_fd: int
```

### Comparing `ikabot-6.6.1/ikabot/function/alertAttacks.py` & `ikabot-6.6.2/ikabot/function/alertAttacks.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/function/alertLowWine.py` & `ikabot-6.6.2/ikabot/function/alertLowWine.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/function/attackBarbarians.py` & `ikabot-6.6.2/ikabot/function/attackBarbarians.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/function/autoPirate.py` & `ikabot-6.6.2/ikabot/function/autoPirate.py`

 * *Files 24% similar despite different names*

```diff
@@ -41,26 +41,96 @@
                 enter()
                 event.set()
                 return
 
         print('{}⚠️ USING THIS FEATURE WILL EXPOSE YOUR IP ADDRESS TO A THIRD PARTY FOR CAPTCHA SOLVING ⚠️{}\n\n'.format(bcolors.WARNING, bcolors.ENDC))
         print('How many pirate missions should I do? (min = 1)')
         pirateCount = read(min=1, digit=True)
-        print("""Which pirate mission should I do?
-    (1) 2m 30s
-    (2) 7m 30s
-    (3) 15m
-    (4) 30m
-    (5) 1h
-    (6) 2h
-    (7) 4h
-    (8) 8h
-    (9) 16h
-    """)
-        pirateMissionChoice = read(min=1, max=9, digit=True)
+        print('Should I schedule pirate missions by the time of day? (y/N)')
+        scheduleInput = read(values=['y', 'Y', 'n', 'N', ''])
+        if scheduleInput.lower() == 'y':
+            pirateSchedule = True
+            print("""Which pirate mission should I do at daytime? (Default mission)
+        (1) 2m 30s
+        (2) 7m 30s
+        (3) 15m
+        (4) 30m
+        (5) 1h
+        (6) 2h
+        (7) 4h
+        (8) 8h
+        (9) 16h
+        """)
+            pirateMissionDayChoice = read(min=1, max=9, digit=True)
+            print("""At which hours should I operate at daytime? (Default: 9 hours from 10 till 18)
+            """)
+            print("From: ")
+            dayStart = read()
+            if dayStart == '':
+                dayStart = 10
+            else:
+                dayStart = int(dayStart)
+
+            print("Till: ")
+            dayEnd = read()
+            if dayEnd == '':
+                dayEnd = 18
+            else:
+                dayEnd = int(dayEnd)
+
+            print("""Which pirate mission should I do at night time?
+            (1) 2m 30s
+            (2) 7m 30s
+            (3) 15m
+            (4) 30m
+            (5) 1h
+            (6) 2h
+            (7) 4h
+            (8) 8h
+            (9) 16h
+            """)
+            pirateMissionNightChoice = read(min=1, max=9, digit=True)
+
+            print("""At which hours should I operate at night time? (Default: 15 hours from 19 till 9): 
+            """)
+            print("From: ")
+            nightStart = read()
+            if nightStart == '':
+                nightStart = 19
+            else:
+                nightStart = int(nightStart)
+
+            print("Till: ")
+            nightEnd = read()
+            if nightEnd == '':
+                nightEnd = 9
+            else:
+                nightEnd = int(nightEnd)
+        else:
+            pirateSchedule = False
+            print("""Which pirate mission should I do?
+        (1) 2m 30s
+        (2) 7m 30s
+        (3) 15m
+        (4) 30m
+        (5) 1h
+        (6) 2h
+        (7) 4h
+        (8) 8h
+        (9) 16h
+        """)
+            pirateMissionChoice = read(min=1, max=9, digit=True)
+        if pirateSchedule == True:
+            current_hour = int(time.strftime("%H"))
+            if current_hour >= dayStart and current_hour <= dayEnd:
+                pirateMissionChoice = pirateMissionDayChoice
+            elif current_hour >= nightStart or current_hour <= nightEnd:
+                pirateMissionChoice = pirateMissionNightChoice
+            else:
+                pirateMissionChoice = pirateMissionDayChoice
         print('Do you want me to automatically convert capture points to crew strength? (Y|N)')
         autoConvert = read(values=['y', 'Y', 'n', 'N'])
         if autoConvert.lower() == 'y':
             print('How many points should I convert every time I do a mission? (Type "all" to convert all points at once)')
             convertPerMission = read(min=0, additionalValues=['all'], digit=True)
         print('Enter a maximum additional random waiting time between missions in seconds. (min = 0)')
         maxRandomWaitingTime = read(min=0, digit=True)
@@ -75,14 +145,22 @@
         enter()
     except KeyboardInterrupt:
         event.set()
         return
     event.set()
     try:
         while (pirateCount > 0):
+            if pirateSchedule == True:
+                current_hour = int(time.strftime("%H"))
+                if current_hour >= dayStart and current_hour <= dayEnd:
+                    pirateMissionChoice = pirateMissionDayChoice
+                elif current_hour >= nightStart or current_hour <= nightEnd:
+                    pirateMissionChoice = pirateMissionNightChoice
+                else:
+                    pirateMissionChoice = pirateMissionDayChoice
             pirateCount -= 1
             piracyCities = getPiracyCities(session, pirateMissionChoice)  # this is done again inside the loop in case the user destroys / creates another pirate fortress while this module is running
             if piracyCities == []:
                 raise Exception('No city with pirate fortress capable of executing selected mission')
             html = session.post(city_url + str(piracyCities[0]['id']))  # this is needed because for some reason you need to look at the town where you are sending a request from in the line below, before you send that request
             if '"showPirateFortressShip":0' in html:  # this is in case the user has manually run a capture run, in that case, there is no need to wait 150secs instead we can check every 5
                 url = 'view=pirateFortress&cityId={}&position=17&backgroundView=city&currentCityId={}&actionRequest={}&ajax=1'.format(piracyCities[0]['id'], piracyCities[0]['id'], actionRequest)
@@ -94,14 +172,16 @@
             url = 'action=PiracyScreen&function=capture&buildingLevel={0}&view=pirateFortress&cityId={1}&position=17&activeTab=tabBootyQuest&backgroundView=city&currentCityId={1}&templateView=pirateFortress&actionRequest={2}&ajax=1'.format(piracyMissionToBuildingLevel[pirateMissionChoice], piracyCities[0]['id'], actionRequest)
             html = session.post(url)
 
             if 'function=createCaptcha' in html:
                 try:
                     for i in range(20):
                         if i == 19:
+                            msg = 'Failed to resolve captcha too many times, autoPirate has been terminated.'
+                            sendToBot(session, msg)
                             raise Exception("Failed to resolve captcha too many times")
                         picture = session.get('action=Options&function=createCaptcha', fullResponse=True).content
                         captcha = resolveCaptcha(session, picture)
                         if captcha == 'Error':
                             continue
                         session.post(city_url + str(piracyCities[0]['id']))
                         params = {'action': 'PiracyScreen', 'function': 'capture', 'cityId': piracyCities[0]['id'], 'position': '17', 'captchaNeeded': '1', 'buildingLevel': str(piracyMissionToBuildingLevel[pirateMissionChoice]), 'captcha': captcha, 'activeTab': 'tabBootyQuest', 'backgroundView': 'city', 'currentCityId': piracyCities[0]['id'], 'templateView': 'pirateFortress', 'actionRequest': actionRequest, 'ajax': '1'}
@@ -115,14 +195,17 @@
                     sendToBot(session, msg)
                     break
             if autoConvert.lower() == 'y':
                 convertCapturePoints(session, piracyCities, convertPerMission)
             wait(piracyMissionWaitingTime[pirateMissionChoice], maxRandomWaitingTime)
 
     except Exception:
+        info = ''
+        msg = _('Error in:\n{}\nCause:\n{}').format(info, traceback.format_exc())
+        sendToBot(session, msg)
         event.set()
         return
 
 
 def resolveCaptcha(session, picture):
     session_data = session.getSessionData()
     if 'decaptcha' not in session_data or session_data['decaptcha']['name'] == 'default':
```

### Comparing `ikabot-6.6.1/ikabot/function/buyResources.py` & `ikabot-6.6.2/ikabot/function/buyResources.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,16 @@
             'type': hit[9],
             'resource': hit[10]
         }
         
         #Parse CDN Images to material type
         if offer["tipo"] == '//gf2.geo.gfsrv.net/cdn19/c3527b2f694fb882563c04df6d8972':
              offer["tipo"] = 'wood'
+        elif offer["tipo"] == '//gf1.geo.gfsrv.net/cdnc6/94ddfda045a8f5ced3397d791fd064':
+            offer["tipo"] = 'wine'     
         elif  offer["tipo"] == '//gf3.geo.gfsrv.net/cdnbf/fc258b990c1a2a36c5aeb9872fc08a':
              offer["tipo"] = 'marble'
         elif  offer["tipo"] == '//gf2.geo.gfsrv.net/cdn1e/417b4059940b2ae2680c070a197d8c':
              offer["tipo"] = 'glass'
         elif  offer["tipo"] == '//gf1.geo.gfsrv.net/cdn9b/5578a7dfa3e98124439cca4a387a61':
              offer["tipo"] = 'sulfur'
         else:
```

### Comparing `ikabot-6.6.1/ikabot/function/checkForUpdate.py` & `ikabot-6.6.2/ikabot/function/checkForUpdate.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/function/constructBuilding.py` & `ikabot-6.6.2/ikabot/function/constructBuilding.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/function/constructionList.py` & `ikabot-6.6.2/ikabot/function/constructionList.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/function/decaptchaConf.py` & `ikabot-6.6.2/ikabot/function/decaptchaConf.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/function/distributeResources.py` & `ikabot-6.6.2/ikabot/function/distributeResources.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/function/donate.py` & `ikabot-6.6.2/ikabot/function/donate.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/function/donationBot.py` & `ikabot-6.6.2/ikabot/function/donationBot.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/function/dumpWorld.py` & `ikabot-6.6.2/ikabot/function/dumpWorld.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/function/getStatus.py` & `ikabot-6.6.2/ikabot/function/getStatus.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,14 +35,16 @@
         banner()
         color_arr = [bcolors.ENDC, bcolors.HEADER, bcolors.STONE, bcolors.BLUE, bcolors.WARNING]
 
         (ids, __) = getIdsOfCities(session)
         total_resources = [0] * len(materials_names)
         total_production = [0] * len(materials_names)
         total_wine_consumption = 0
+        housing_space = 0
+        citizens = 0
         available_ships = 0
         total_ships = 0
         for id in ids:
             session.get('view=city&cityId={}'.format(id), noIndex=True)
             data = session.get("view=updateGlobalData&ajax=1", noIndex=True)
             json_data = json.loads(data, strict=False)
             json_data = json_data[0][1]['headerData']
@@ -50,14 +52,16 @@
                 continue
             wood = Decimal(json_data['resourceProduction'])
             good = Decimal(json_data['tradegoodProduction'])
             typeGood = int(json_data['producedTradegood'])
             total_production[0] += wood * 3600
             total_production[typeGood] += good * 3600
             total_wine_consumption += json_data['wineSpendings']
+            housing_space += int(json_data['currentResources']['population'])
+            citizens += int(json_data['currentResources']['citizens'])
             total_resources[0] += json_data['currentResources']['resource']
             total_resources[1] += json_data['currentResources']['1']
             total_resources[2] += json_data['currentResources']['2']
             total_resources[3] += json_data['currentResources']['3']
             total_resources[4] += json_data['currentResources']['4']
             available_ships = json_data['freeTransporters']
             total_ships = json_data['maxTransporters']
@@ -91,14 +95,16 @@
         storageCapacity = city['storageCapacity']
         color_resources = []
         for i in range(len(materials_names)):
             if resources[i] == storageCapacity:
                 color_resources.append(bcolors.RED)
             else:
                 color_resources.append(bcolors.ENDC)
+        print(_('Population:'))
+        print('{}:{} {}:{}'.format('Housing space', addThousandSeparator(housing_space), 'Citizens', addThousandSeparator(citizens)))
         print(_('Storage:'))
         print(addThousandSeparator(storageCapacity))
         print(_('Resources:'))
         for i in range(len(materials_names)):
             print('{} {}{}{} '.format(materials_names[i], color_resources[i], addThousandSeparator(resources[i]), bcolors.ENDC), end='')
         print('')
 
@@ -114,15 +120,15 @@
                 if typeGood == 1 and (good*3600) > consumption_per_hour:
                     elapsed_time_run_out = '∞'
                 else:
                     consumption_per_second = Decimal(consumption_per_hour) / Decimal(3600)
                     remaining_resources_to_consume = Decimal(resources[1]) / Decimal(consumption_per_second)
                     elapsed_time_run_out = daysHoursMinutes(remaining_resources_to_consume)
                 print(_('There is wine for: {}').format(elapsed_time_run_out))
-
+        
         for building in [building for building in city['position'] if building['name'] != 'empty']:
             if building['isMaxLevel'] is True:
                 color = bcolors.BLACK
             elif building['canUpgrade'] is True:
                 color = bcolors.GREEN
             else:
                 color = bcolors.RED
```

### Comparing `ikabot-6.6.1/ikabot/function/importExportCookie.py` & `ikabot-6.6.2/ikabot/function/importExportCookie.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/function/investigate.py` & `ikabot-6.6.2/ikabot/function/investigate.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/function/killTasks.py` & `ikabot-6.6.2/ikabot/function/killTasks.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/function/loginDaily.py` & `ikabot-6.6.2/ikabot/function/loginDaily.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/function/proxyConf.py` & `ikabot-6.6.2/ikabot/function/proxyConf.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/function/searchForIslandSpaces.py` & `ikabot-6.6.2/ikabot/function/searchForIslandSpaces.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/function/sellResources.py` & `ikabot-6.6.2/ikabot/function/sellResources.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/function/sendResources.py` & `ikabot-6.6.2/ikabot/function/sendResources.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/function/shipMovements.py` & `ikabot-6.6.2/ikabot/function/shipMovements.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/function/trainArmy.py` & `ikabot-6.6.2/ikabot/function/trainArmy.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/function/update.py` & `ikabot-6.6.2/ikabot/function/update.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/function/vacationMode.py` & `ikabot-6.6.2/ikabot/function/vacationMode.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/helpers/aesCipher.py` & `ikabot-6.6.2/ikabot/helpers/aesCipher.py`

 * *Files 8% similar despite different names*

```diff
@@ -80,19 +80,23 @@
 
         for ciphertext in ciphertexts.split('\n'):
             if entry_key == ciphertext[:64]:
                 ciphertext = ciphertext[64:]
                 try:
                     plaintext = self.decrypt(ciphertext)
                 except Exception:
-                    msg = _('Error while decrypting session data\nSaved data will be deleted.')
+                    msg = _('Error while decrypting session data.\nYou may have entered a wrong password.')
                     if session.padre:
                         print(msg)
                     else:
                         sendToBot(session, msg)
+                    print(_('\nWould you like to delete the ikabot session data associated with this email address? [y/N]'))
+                    rta = read(values=['n', 'N', 'y', 'Y'])
+                    if rta.lower() == 'n':
+                        os._exit(0)
                     self.deleteSessionData(session)
                     os._exit(0)
                 data_dict = json.loads(plaintext, strict=False)
                 if all:
                     return data_dict
                 else:
                     try:
```

### Comparing `ikabot-6.6.1/ikabot/helpers/botComm.py` & `ikabot-6.6.2/ikabot/helpers/botComm.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/helpers/getJson.py` & `ikabot-6.6.2/ikabot/helpers/getJson.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/helpers/gui.py` & `ikabot-6.6.2/ikabot/helpers/gui.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/helpers/market.py` & `ikabot-6.6.2/ikabot/helpers/market.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/helpers/naval.py` & `ikabot-6.6.2/ikabot/helpers/naval.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/helpers/pedirInfo.py` & `ikabot-6.6.2/ikabot/helpers/pedirInfo.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/helpers/planRoutes.py` & `ikabot-6.6.2/ikabot/helpers/planRoutes.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/helpers/process.py` & `ikabot-6.6.2/ikabot/helpers/process.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/helpers/resources.py` & `ikabot-6.6.2/ikabot/helpers/resources.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/helpers/signals.py` & `ikabot-6.6.2/ikabot/helpers/signals.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/helpers/varios.py` & `ikabot-6.6.2/ikabot/helpers/varios.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/activateMiracle.po` & `ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/activateMiracle.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/aesCipher.po` & `ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/aesCipher.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/alertAttacks.po` & `ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/alertAttacks.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/alertLowWine.po` & `ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/alertLowWine.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/botComm.po` & `ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/botComm.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/buyResources.po` & `ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/buyResources.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/checkForUpdate.po` & `ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/checkForUpdate.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/command_line.po` & `ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/command_line.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/config.po` & `ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/config.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/constructBuilding.po` & `ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/constructBuilding.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/constructionList.po` & `ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/constructionList.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/distributeResources.po` & `ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/distributeResources.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/donate.po` & `ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/donate.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/donationBot.po` & `ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/donationBot.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/getStatus.po` & `ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/getStatus.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/gui.po` & `ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/gui.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/loginDaily.po` & `ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/loginDaily.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/pedirInfo.mo` & `ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/pedirInfo.mo`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/pedirInfo.po` & `ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/pedirInfo.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/searchForIslandSpaces.po` & `ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/searchForIslandSpaces.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/sellResources.po` & `ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/sellResources.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/sendResources.po` & `ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/sendResources.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/session.mo` & `ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/session.mo`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/session.po` & `ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/session.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/shipMovements.po` & `ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/shipMovements.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/signals.po` & `ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/signals.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/trainArmy.pot` & `ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/trainArmy.pot`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/trainFleets.po` & `ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/trainFleets.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/trainTroops.po` & `ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/trainTroops.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/update.po` & `ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/update.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/locale/es/LC_MESSAGES/vacationMode.po` & `ikabot-6.6.2/ikabot/locale/es/LC_MESSAGES/vacationMode.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/ikabot/web/session.py` & `ikabot-6.6.2/ikabot/web/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     'JVqc1PkrbpPF9zyxI5ICZ4y-BFe4Kov1WtA_ZJbI7R9iyCmVCG2SxAcsXpDSPqcVgKXXCS5go8j6LIPsWr4tpBc8bqDF9zpfkcMGbuBPvCFGeKrPAURpm80Ug_JZxSpPgbH6aMv5HlCCp9kcVHmr7iJHebzhE0WtH0yU5gs9gOhaf7H0Wcf0SZzB8zabCS5gkrfpLFGDtRtPhrkdUYi76xxPs-ggg-hNhLzzJli99i1hxSldviRWu_NXh7joHVGFviFUjMD2K2PGKI6_9CRZvvIih-tQhbXaDD5jldj9L2GoF4btWb7jFUWO_F-NsuQUPH3KDjdcjtESYKfzOF2Pv-codbneEFN4qtosjfFWxTNYiroMZIm76yBYiK3fD2LHOaIHep_RAUWuIIXoXI_TBDVajLwypQQ5mMjtH0-_MpHGJVV6rO8URna67TFik7zhE0VqnN8ENmjML1-W-FuS9CVblMwDZJn7Mpb8NGyk1ws8bM4AY5fIKozxV4u88yZblPhbj_EmW5P1WJHyU7UXS4HmHE5-30R4nc8BJlibwPIkiMEiiL8ggbIWRnbcDj5w1Q0_eKkPdKjhQ3yv4xd9s-wjV43D9iuQ9VaLviNavyCD6B5WueoagLPjFXjbFEd62wAyZIm7_i9omsrvIWSVxfkpToDD9SlOgMM3qR6DqNodkQN43QI0d5zOADGXx_pck8owlPUoW5LG-CpgkfNYuelNf7YbUYW36kyy5BZ6rA50qeBGqw1wpdg5ntUKbKXbDXOpDkN1qAtuntD1J1l-sPMYSnyxEkKnDT912z943kR0reMZUYrwVbYXe6sPQ3ziRHyx5hdPgbMYea8RRKYLQnbXBzlwqd1ActM0ZZX6W7_wJFW74BJEaZveAzVnnf5jxfsvYJL0Jlq8HVS4HEyEuu8ih-keTn-27x9Rh73tH1OMxf4vZsf9MWGRwvktk8wtkcgtZsgtk8oCY8UrXYK05gs9gKXXCT6j2hJFdq7gFE2x5Uuv4RpNfd4PQHbYDkB4ruESeLHqT7XuHlSM7yeNvyRXi8T4KFuOvvEpYpnSCGrOB2iY-luAsuQJO36v4RVDc6faDkV6rOMYSX-v5ho_cbTZCz2g0jNr0AVmmsosXY_zVIjuH4G5HFC2F01-tOpPhr8gWIzCJ4rD81S47h5RguMXSqvhRH2t5EqAsecaS3veQ6fbADJkibv-MGCRxPsza57UCzBipcr8LmCQwvUiUoWy5Bhsnc_0J2ibzfIlZpfO_DVqn_keUIKn2RxBc6UbTsY3nQF54kev4hhOg-pNr-UZgPRooAVy0zhdj8HmGFuQwfkeUJO46hxNfaLUBitdoMX3KY7USKDvIVXGKluxHnG1IYnrQpgJW673cb0SeuQtl-EvkddDds8WYKHrZJXMFWrZTqMOdaf2TLfsULoUSq_hFYDXK1uP9T1u0zd63USU6zWa_ECaE23FLWKy4lGD3DSc4zVnnABWwTmsD3iwI23nHJLkXo_HG4T3YasAVqn_VMQYfeo8tBdqqyNx2z5zwSuE_Emd6h1rr_wvVIa43Q9Sd6nbKJcReuZSs9gKUIWz4wg6apLpUsAkkwp9otQEUqbL_S1ejrzsEUSGq90NZM07caXK_T9klsY-dKjR9ihYmQl55UqhBmizHJC15y1ilcz6LWOIuuoSXaX5RpK36SxRg7MfiPNYfa_fJovuWcjxFkh4uyOVBHHW-y1zpNUGNGSSwvAgRXen-lvBIpT9IlSazwI5Z5rQ9SdZfrDzGEp8rt4QQ3Cg0wAyZrrrHUJ1tukbQHO05RxKeqraNFmLveIUV8U6phI3bLA',
     'JVqc1PkrbpPF9zyxI5ICZ4y-BFe4Kov1WtA_ZJbI7R9iyCmVCG2SxAcsXpDSPqcVgKXXCS5go8j6LIPsWr4tpBc8bqDF9zpfkcMGbuBPvCFGeKrPAURpm80Ug_JZxSpPgbH6aMv5HlCCp9kcVHmr7iJHebzhE0WtH0yU5gs9b5TGCS5gkvgsY5b6LmWYyPkskMX9YMUqYZnQAzWa0wo-ogY6mwEzmNA0ZJXF-i5im_4xaZ3TCECjBWuc0QE2m8__ZMgtYpK36RtAcrXaDD6F9GPKNpvA8iJr2Txqj8HxGVqn6xQ5a67vPYTQFTpsnMQFUpa77TBVh7cJas4zohA1Z5fpQWaYyP01ZYq87D-kFn_kV3yu3iKL_WLFOWyw4RI3aZkPguEWdaXK_CycD26jAjJXiczxI1OXyg4_cJm-8CJHebzhE0WpDDxz1Thv0QI4cangQXbYD3PZEUmBtOgZSavdQHSlB2nONGiZ0AM4cdU4bM4DOHDSNW7PMJL0KF7D-StbvCFVeqzeAzV4nc8BZZ7_ZZz9Xo_zI1O56xtNsuocVYbsUYW-IFmMwPRakMkANGqg0wht0jNomwA3nP1gxfszlsf3XZDA8lW48SRXuN0PQWaY2wxFd6fM_kFyotYGK12g0gYrXaAUhvtghbf6buBVut8RVHmr3Q50pNc5cKcNcdIFOG-j1Qc9btA1lsYqXJP4LmKUxymPwfNXietRhr0jiOpNgrUWe7LnSYK46lCG6yBShehLe63SBDZbjdD1J1mO7x-E6hxSuBxVuyFRisD2LmfNMpP0WIjsIFm_IVmOw_QsXpD1VozuIYPoH1O05BZNhrodT7ARQnLXOJzNATKYve8hRni74BJEettAotgMPW_RAzeZ-jGV-Slhl8z_ZMb7K1yTzPwuZJrK_DBpotsMQ6TaDj5un9YKcKkKbqUKQ6UKcKffQKIIOl-Rw-gaXYK05huAt-8iU4u98SqOwiiMvvcqWrvsHVO16x1Vi77vVY7HLJLL-zFpzARqnAE0aKHVBThrm84GP3av5Uer5EV11zhdj8HmGFuMvvIgUIS36yJXicD1JlyMw_ccTpG26Bp9rxBIreJDd6cJOmzQMWXL_F6W-S2T9CpbkccsY5z9NWmfBGeg0DGVy_suX8D0J4i-IVqKwSddjsT3KFi7IIS43Q9BZpjbDT1uodgQSHux6A0_gqfZCz1tn9L_L2KPwfVJeqzRBEV4rNEERXWu3AxDdtD1J1l-sPMYSnzrWsk3oA112Al_40246iOUCj-k1k-F617BIoit3xE2aKvfF090pukOQHKj0_gqXIGz9htNf-RRir8hZa_4XMc_tABEicEjVKoec6QQiO1azQBWqg5VpiCQCFfBNGzBCVe4HYjBN4zTOrEGN5_gQa_gTK0WfsgUfuZbwBNkibsBV8MNP5TZSav6P7brQa0De8cebKD3TqAWZs8ZXrDhNqMGSb0AWqH7NIX-M3_XGoLaJpP7TKXoHYnfSb0OaKvsZLIcf7QCbMU9ivRFeMZAiQInWYuw4iVKfK77auRNuSWGq90jWIa22w09Zbwlk_dm3VB1p9cleZ7QADFhj7_kF1l-sOA3oA5EeJ3QEjdpmRFHe6TJ-yts3Ey4HXTZO4bvY4i6ADVon80ANluNveUweMwZZYq8_yRWhvJbxitQgrL5XsEsm8TpG0uO9mjXRKnOAEZ3qNkHN2WVw_MYSnrNLpT1Z9D1J22i1Qw6baPI-ixRg8brHU-BseMWQ3Om0wU5jb7wFUiJvPAVSIm58R9Pf68JLmCSt-ksmg975wxBhQ',
 ]
 
 class Session:
     def __init__(self):
         if isWindows:
-            self.logfile = os.getenv('temp') + '/ikabot.log'
+            self.logfile = os.getenv('temp') + '\ikabot.log'
         else:
             self.logfile = '/tmp/ikabot.log'
         self.log = False
         self.padre = True
         self.logged = False
         self.blackbox = 'tra:' + random.choice(blackbox_tokens)
```

### Comparing `ikabot-6.6.1/ikabot.egg-info/SOURCES.txt` & `ikabot-6.6.2/ikabot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.1/setup.py` & `ikabot-6.6.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="ikabot",
-    version="6.6.1",
+    version="6.6.2",
     author="physics-sp",
     author_email="physics-sp@protonmail.com",
     license='MIT',
     description="A bot for ikariam",
     url="https://github.com/physics-sp/ikabot",
     include_package_data=True,
     packages=setuptools.find_packages(),
```

