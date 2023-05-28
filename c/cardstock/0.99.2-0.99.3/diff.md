# Comparing `tmp/cardstock-0.99.2.tar.gz` & `tmp/cardstock-0.99.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cardstock-0.99.2.tar", last modified: Wed Dec 28 00:47:14 2022, max compression
+gzip compressed data, was "cardstock-0.99.3.tar", last modified: Sun May 28 23:20:22 2023, max compression
```

## Comparing `cardstock-0.99.2.tar` & `cardstock-0.99.3.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 benjie     (501) staff       (20)        0 2022-12-28 00:47:14.739637 cardstock-0.99.2/
--rw-r--r--   0 benjie     (501) staff       (20)    16725 2021-11-02 20:40:58.000000 cardstock-0.99.2/LICENSE
--rw-r--r--   0 benjie     (501) staff       (20)     6948 2022-12-28 00:47:14.739879 cardstock-0.99.2/PKG-INFO
--rw-r--r--   0 benjie     (501) staff       (20)     6418 2022-12-28 00:38:48.000000 cardstock-0.99.2/README.md
-drwxr-xr-x   0 benjie     (501) staff       (20)        0 2022-12-28 00:47:14.710185 cardstock-0.99.2/cardstock/
--rw-r--r--   0 benjie     (501) staff       (20)     1715 2022-12-28 00:38:48.000000 cardstock-0.99.2/cardstock/CardStock_Designer_mac.spec
--rw-r--r--   0 benjie     (501) staff       (20)     1613 2021-11-02 20:40:58.000000 cardstock-0.99.2/cardstock/CardStock_Viewer_mac.spec
--rw-r--r--   0 benjie     (501) staff       (20)      204 2021-11-02 20:40:58.000000 cardstock-0.99.2/cardstock/__init__.py
--rw-r--r--   0 benjie     (501) staff       (20)      101 2021-11-02 20:40:58.000000 cardstock-0.99.2/cardstock/__main__.py
--rw-r--r--   0 benjie     (501) staff       (20)     5890 2022-09-14 20:33:21.000000 cardstock-0.99.2/cardstock/allCodeWindow.py
--rw-r--r--   0 benjie     (501) staff       (20)    14495 2022-09-14 20:33:21.000000 cardstock-0.99.2/cardstock/analyzer.py
--rw-r--r--   0 benjie     (501) staff       (20)    16760 2022-12-28 00:38:48.000000 cardstock-0.99.2/cardstock/appCommands.py
--rw-r--r--   0 benjie     (501) staff       (20)     4198 2021-12-10 23:35:58.000000 cardstock-0.99.2/cardstock/build.py
--rw-r--r--   0 benjie     (501) staff       (20)     4089 2022-09-14 20:33:21.000000 cardstock-0.99.2/cardstock/cardstockFrameParts.py
--rw-r--r--   0 benjie     (501) staff       (20)     6420 2022-02-08 19:39:00.000000 cardstock-0.99.2/cardstock/codeInspector.py
--rw-r--r--   0 benjie     (501) staff       (20)    23657 2022-09-14 23:59:07.000000 cardstock-0.99.2/cardstock/codeInspectorMulti.py
--rw-r--r--   0 benjie     (501) staff       (20)     5138 2022-09-14 20:33:21.000000 cardstock-0.99.2/cardstock/codeRunnerThread.py
--rw-r--r--   0 benjie     (501) staff       (20)    12862 2022-12-28 00:38:48.000000 cardstock-0.99.2/cardstock/consoleWindow.py
--rw-r--r--   0 benjie     (501) staff       (20)    19514 2022-09-14 20:33:21.000000 cardstock-0.99.2/cardstock/controlPanel.py
--rw-r--r--   0 benjie     (501) staff       (20)    57788 2022-12-28 00:38:48.000000 cardstock-0.99.2/cardstock/designer.py
--rw-r--r--   0 benjie     (501) staff       (20)   131030 2022-09-14 20:33:21.000000 cardstock-0.99.2/cardstock/embeddedImages.py
--rw-r--r--   0 benjie     (501) staff       (20)     3639 2022-09-14 20:33:21.000000 cardstock-0.99.2/cardstock/errorListWindow.py
-drwxr-xr-x   0 benjie     (501) staff       (20)        0 2022-12-28 00:47:14.735159 cardstock-0.99.2/cardstock/examples/
--rw-r--r--   0 benjie     (501) staff       (20)     8066 2022-12-28 00:38:48.000000 cardstock-0.99.2/cardstock/examples/Asteroids.cds
--rw-r--r--   0 benjie     (501) staff       (20)     4787 2022-09-14 20:33:21.000000 cardstock-0.99.2/cardstock/examples/Browser.cds
--rw-r--r--   0 benjie     (501) staff       (20)     9975 2022-09-14 20:33:21.000000 cardstock-0.99.2/cardstock/examples/Calculator.cds
--rw-r--r--   0 benjie     (501) staff       (20)     4003 2022-09-14 20:33:21.000000 cardstock-0.99.2/cardstock/examples/Catch.cds
--rw-r--r--   0 benjie     (501) staff       (20)     5667 2022-09-14 20:33:21.000000 cardstock-0.99.2/cardstock/examples/Diary.cds
--rw-r--r--   0 benjie     (501) staff       (20)     7872 2022-09-14 20:33:21.000000 cardstock-0.99.2/cardstock/examples/Dice-stats.cds
--rw-r--r--   0 benjie     (501) staff       (20)     4422 2022-09-14 20:33:21.000000 cardstock-0.99.2/cardstock/examples/Dice.cds
--rw-r--r--   0 benjie     (501) staff       (20)     3451 2022-09-14 20:33:21.000000 cardstock-0.99.2/cardstock/examples/Factor.cds
--rw-r--r--   0 benjie     (501) staff       (20)    33761 2022-12-28 00:38:48.000000 cardstock-0.99.2/cardstock/examples/Fifteen.cds
--rw-r--r--   0 benjie     (501) staff       (20)     4907 2022-09-14 20:33:21.000000 cardstock-0.99.2/cardstock/examples/Flappy.cds
--rw-r--r--   0 benjie     (501) staff       (20)     7885 2022-09-14 20:33:21.000000 cardstock-0.99.2/cardstock/examples/Graph.cds
--rw-r--r--   0 benjie     (501) staff       (20)     8049 2022-09-14 20:33:21.000000 cardstock-0.99.2/cardstock/examples/Guess.cds
--rw-r--r--   0 benjie     (501) staff       (20)     9259 2022-12-28 00:38:48.000000 cardstock-0.99.2/cardstock/examples/Hanoi.cds
--rw-r--r--   0 benjie     (501) staff       (20)    29952 2022-12-28 00:38:48.000000 cardstock-0.99.2/cardstock/examples/Logo.cds
--rw-r--r--   0 benjie     (501) staff       (20)     3083 2022-09-14 20:33:21.000000 cardstock-0.99.2/cardstock/examples/Magic.cds
--rw-r--r--   0 benjie     (501) staff       (20)    16438 2022-09-14 20:33:21.000000 cardstock-0.99.2/cardstock/examples/Mastermind.cds
--rw-r--r--   0 benjie     (501) staff       (20)     9318 2022-09-14 20:33:21.000000 cardstock-0.99.2/cardstock/examples/Maze.cds
--rw-r--r--   0 benjie     (501) staff       (20)    25585 2022-09-14 20:33:21.000000 cardstock-0.99.2/cardstock/examples/Morph.cds
--rw-r--r--   0 benjie     (501) staff       (20)    22300 2022-09-14 20:33:21.000000 cardstock-0.99.2/cardstock/examples/Navigation.cds
--rw-r--r--   0 benjie     (501) staff       (20)     8298 2022-09-14 20:33:21.000000 cardstock-0.99.2/cardstock/examples/Number-puzzle.cds
--rw-r--r--   0 benjie     (501) staff       (20)     4052 2022-09-14 20:33:21.000000 cardstock-0.99.2/cardstock/examples/Pong.cds
--rw-r--r--   0 benjie     (501) staff       (20)     2032 2022-09-14 20:33:21.000000 cardstock-0.99.2/cardstock/examples/Requests.cds
--rw-r--r--   0 benjie     (501) staff       (20)     5108 2022-09-14 20:33:21.000000 cardstock-0.99.2/cardstock/examples/Scene.cds
--rw-r--r--   0 benjie     (501) staff       (20)     3328 2022-09-14 20:33:21.000000 cardstock-0.99.2/cardstock/examples/Serial.cds
--rw-r--r--   0 benjie     (501) staff       (20)    10074 2022-09-14 20:33:21.000000 cardstock-0.99.2/cardstock/examples/Snake.cds
--rw-r--r--   0 benjie     (501) staff       (20)     8889 2022-09-14 20:33:21.000000 cardstock-0.99.2/cardstock/examples/Tanks.cds
--rw-r--r--   0 benjie     (501) staff       (20)     7988 2022-12-28 00:38:48.000000 cardstock-0.99.2/cardstock/examples/Tetris.cds
--rw-r--r--   0 benjie     (501) staff       (20)    14073 2022-09-14 20:33:21.000000 cardstock-0.99.2/cardstock/examples/TicTacToe.cds
--rw-r--r--   0 benjie     (501) staff       (20)    84929 2022-09-14 20:33:21.000000 cardstock-0.99.2/cardstock/examples/Welcome.cds
--rw-r--r--   0 benjie     (501) staff       (20)    24364 2022-12-28 00:38:48.000000 cardstock-0.99.2/cardstock/examples/Wordel.cds
--rw-r--r--   0 benjie     (501) staff       (20)   103912 2021-11-02 20:40:58.000000 cardstock-0.99.2/cardstock/examples/click.wav
--rw-r--r--   0 benjie     (501) staff       (20)    17826 2021-11-02 20:40:58.000000 cardstock-0.99.2/cardstock/examples/puff.wav
--rw-r--r--   0 benjie     (501) staff       (20)    20544 2021-11-02 20:40:58.000000 cardstock-0.99.2/cardstock/examples/ship-off.png
--rw-r--r--   0 benjie     (501) staff       (20)    20749 2021-11-02 20:40:58.000000 cardstock-0.99.2/cardstock/examples/ship-on.png
--rw-r--r--   0 benjie     (501) staff       (20)    16127 2022-02-18 23:23:29.000000 cardstock-0.99.2/cardstock/examples/simple-red-apple.png
--rw-r--r--   0 benjie     (501) staff       (20)   451172 2021-11-02 20:40:58.000000 cardstock-0.99.2/cardstock/examples/yay.wav
--rw-r--r--   0 benjie     (501) staff       (20)     7930 2022-09-14 20:33:21.000000 cardstock-0.99.2/cardstock/findEngineDesigner.py
--rw-r--r--   0 benjie     (501) staff       (20)     5938 2022-02-08 19:39:00.000000 cardstock-0.99.2/cardstock/findEngineViewer.py
--rw-r--r--   0 benjie     (501) staff       (20)     1612 2022-09-14 20:33:21.000000 cardstock-0.99.2/cardstock/flippedGCDC.py
--rw-r--r--   0 benjie     (501) staff       (20)     3074 2022-02-18 23:23:29.000000 cardstock-0.99.2/cardstock/generator.py
--rw-r--r--   0 benjie     (501) staff       (20)    97881 2022-12-28 00:38:48.000000 cardstock-0.99.2/cardstock/helpData.py
--rw-r--r--   0 benjie     (501) staff       (20)    38551 2022-12-28 00:38:48.000000 cardstock-0.99.2/cardstock/helpDialogs.py
--rw-r--r--   0 benjie     (501) staff       (20)     1086 2022-02-08 19:39:00.000000 cardstock-0.99.2/cardstock/imageFactory.py
--rw-r--r--   0 benjie     (501) staff       (20)     7297 2022-12-28 00:38:48.000000 cardstock-0.99.2/cardstock/mediaSearchDialogs.py
--rw-r--r--   0 benjie     (501) staff       (20)    21888 2022-09-14 20:33:21.000000 cardstock-0.99.2/cardstock/migrations.py
--rw-r--r--   0 benjie     (501) staff       (20)    24460 2022-09-14 20:33:21.000000 cardstock-0.99.2/cardstock/propertyInspector.py
--rw-r--r--   0 benjie     (501) staff       (20)    12990 2022-09-14 20:33:21.000000 cardstock-0.99.2/cardstock/pythonEditor.py
--rw-r--r--   0 benjie     (501) staff       (20)     1475 2021-11-02 20:40:58.000000 cardstock-0.99.2/cardstock/resourcePathManager.py
--rw-r--r--   0 benjie     (501) staff       (20)    43204 2022-12-28 00:38:48.000000 cardstock-0.99.2/cardstock/runner.py
--rw-r--r--   0 benjie     (501) staff       (20)     1480 2021-11-02 20:40:58.000000 cardstock-0.99.2/cardstock/sanitizer.py
--rw-r--r--   0 benjie     (501) staff       (20)     6308 2022-09-14 20:33:21.000000 cardstock-0.99.2/cardstock/simpleListBox.py
--rw-r--r--   0 benjie     (501) staff       (20)    25490 2022-12-28 00:38:48.000000 cardstock-0.99.2/cardstock/stackExporter.py
--rw-r--r--   0 benjie     (501) staff       (20)    51895 2022-12-28 00:38:48.000000 cardstock-0.99.2/cardstock/stackManager.py
--rw-r--r--   0 benjie     (501) staff       (20)     4449 2022-09-14 20:33:21.000000 cardstock-0.99.2/cardstock/stackModel.py
--rw-r--r--   0 benjie     (501) staff       (20)     2796 2022-09-14 20:33:21.000000 cardstock-0.99.2/cardstock/standalone.py
--rw-r--r--   0 benjie     (501) staff       (20)    38050 2022-12-28 00:38:48.000000 cardstock-0.99.2/cardstock/tools.py
--rw-r--r--   0 benjie     (501) staff       (20)    12511 2022-12-28 00:38:48.000000 cardstock-0.99.2/cardstock/uiButton.py
--rw-r--r--   0 benjie     (501) staff       (20)    18415 2022-12-28 00:38:48.000000 cardstock-0.99.2/cardstock/uiCard.py
--rw-r--r--   0 benjie     (501) staff       (20)    12053 2022-09-14 20:33:21.000000 cardstock-0.99.2/cardstock/uiGroup.py
--rw-r--r--   0 benjie     (501) staff       (20)     7219 2022-12-28 00:38:48.000000 cardstock-0.99.2/cardstock/uiImage.py
--rw-r--r--   0 benjie     (501) staff       (20)    24917 2022-12-28 00:38:48.000000 cardstock-0.99.2/cardstock/uiShape.py
--rw-r--r--   0 benjie     (501) staff       (20)    11895 2022-12-28 00:38:48.000000 cardstock-0.99.2/cardstock/uiTextBase.py
--rw-r--r--   0 benjie     (501) staff       (20)    14328 2022-12-28 00:38:48.000000 cardstock-0.99.2/cardstock/uiTextField.py
--rw-r--r--   0 benjie     (501) staff       (20)     8381 2022-09-14 20:33:21.000000 cardstock-0.99.2/cardstock/uiTextLabel.py
--rw-r--r--   0 benjie     (501) staff       (20)    71126 2022-12-28 00:38:48.000000 cardstock-0.99.2/cardstock/uiView.py
--rw-r--r--   0 benjie     (501) staff       (20)     8337 2022-12-28 00:38:48.000000 cardstock-0.99.2/cardstock/uiWebView.py
--rw-r--r--   0 benjie     (501) staff       (20)     9873 2022-09-14 20:33:21.000000 cardstock-0.99.2/cardstock/variablesWindow.py
--rw-r--r--   0 benjie     (501) staff       (20)       43 2022-12-28 00:38:48.000000 cardstock-0.99.2/cardstock/version.py
--rw-r--r--   0 benjie     (501) staff       (20)    26210 2022-12-28 00:38:48.000000 cardstock-0.99.2/cardstock/viewer.py
-drwxr-xr-x   0 benjie     (501) staff       (20)        0 2022-12-28 00:47:14.739297 cardstock-0.99.2/cardstock.egg-info/
--rw-r--r--   0 benjie     (501) staff       (20)     6948 2022-12-28 00:47:14.000000 cardstock-0.99.2/cardstock.egg-info/PKG-INFO
--rw-r--r--   0 benjie     (501) staff       (20)     3737 2022-12-28 00:47:14.000000 cardstock-0.99.2/cardstock.egg-info/SOURCES.txt
--rw-r--r--   0 benjie     (501) staff       (20)        1 2022-12-28 00:47:14.000000 cardstock-0.99.2/cardstock.egg-info/dependency_links.txt
--rw-r--r--   0 benjie     (501) staff       (20)      102 2022-12-28 00:47:14.000000 cardstock-0.99.2/cardstock.egg-info/entry_points.txt
--rw-r--r--   0 benjie     (501) staff       (20)       52 2022-12-28 00:47:14.000000 cardstock-0.99.2/cardstock.egg-info/requires.txt
--rw-r--r--   0 benjie     (501) staff       (20)       10 2022-12-28 00:47:14.000000 cardstock-0.99.2/cardstock.egg-info/top_level.txt
--rw-r--r--   0 benjie     (501) staff       (20)      103 2021-11-02 20:40:58.000000 cardstock-0.99.2/pyproject.toml
--rw-r--r--   0 benjie     (501) staff       (20)      957 2022-12-28 00:47:14.740936 cardstock-0.99.2/setup.cfg
+drwxr-xr-x   0 benjie     (501) staff       (20)        0 2023-05-28 23:20:22.496571 cardstock-0.99.3/
+-rw-r--r--   0 benjie     (501) staff       (20)    16725 2021-11-02 20:40:58.000000 cardstock-0.99.3/LICENSE
+-rw-r--r--   0 benjie     (501) staff       (20)     7087 2023-05-28 23:20:22.496695 cardstock-0.99.3/PKG-INFO
+-rw-r--r--   0 benjie     (501) staff       (20)     6557 2023-05-28 23:12:56.000000 cardstock-0.99.3/README.md
+drwxr-xr-x   0 benjie     (501) staff       (20)        0 2023-05-28 23:20:22.471427 cardstock-0.99.3/cardstock/
+-rw-r--r--   0 benjie     (501) staff       (20)     1715 2022-12-28 00:38:48.000000 cardstock-0.99.3/cardstock/CardStock_Designer_mac.spec
+-rw-r--r--   0 benjie     (501) staff       (20)     1613 2021-11-02 20:40:58.000000 cardstock-0.99.3/cardstock/CardStock_Viewer_mac.spec
+-rw-r--r--   0 benjie     (501) staff       (20)      521 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/__init__.py
+-rw-r--r--   0 benjie     (501) staff       (20)      418 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/__main__.py
+-rw-r--r--   0 benjie     (501) staff       (20)     6207 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/allCodeWindow.py
+-rw-r--r--   0 benjie     (501) staff       (20)    14812 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/analyzer.py
+-rw-r--r--   0 benjie     (501) staff       (20)    17077 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/appCommands.py
+-rw-r--r--   0 benjie     (501) staff       (20)     4515 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/build.py
+-rw-r--r--   0 benjie     (501) staff       (20)     4406 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/cardstockFrameParts.py
+-rw-r--r--   0 benjie     (501) staff       (20)     6737 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/codeInspector.py
+-rw-r--r--   0 benjie     (501) staff       (20)    23974 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/codeInspectorMulti.py
+-rw-r--r--   0 benjie     (501) staff       (20)     5455 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/codeRunnerThread.py
+-rw-r--r--   0 benjie     (501) staff       (20)    14000 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/consoleWindow.py
+-rw-r--r--   0 benjie     (501) staff       (20)    19831 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/controlPanel.py
+-rw-r--r--   0 benjie     (501) staff       (20)    57979 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/designer.py
+-rw-r--r--   0 benjie     (501) staff       (20)   141197 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/embeddedImages.py
+-rw-r--r--   0 benjie     (501) staff       (20)     3956 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/errorListWindow.py
+drwxr-xr-x   0 benjie     (501) staff       (20)        0 2023-05-28 23:20:22.492609 cardstock-0.99.3/cardstock/examples/
+-rw-r--r--   0 benjie     (501) staff       (20)     8066 2022-12-28 00:38:48.000000 cardstock-0.99.3/cardstock/examples/Asteroids.cds
+-rw-r--r--   0 benjie     (501) staff       (20)     4787 2022-09-14 20:33:21.000000 cardstock-0.99.3/cardstock/examples/Browser.cds
+-rw-r--r--   0 benjie     (501) staff       (20)     9975 2022-09-14 20:33:21.000000 cardstock-0.99.3/cardstock/examples/Calculator.cds
+-rw-r--r--   0 benjie     (501) staff       (20)     4003 2022-09-14 20:33:21.000000 cardstock-0.99.3/cardstock/examples/Catch.cds
+-rw-r--r--   0 benjie     (501) staff       (20)     5667 2022-09-14 20:33:21.000000 cardstock-0.99.3/cardstock/examples/Diary.cds
+-rw-r--r--   0 benjie     (501) staff       (20)     7872 2022-09-14 20:33:21.000000 cardstock-0.99.3/cardstock/examples/Dice-stats.cds
+-rw-r--r--   0 benjie     (501) staff       (20)     4422 2022-09-14 20:33:21.000000 cardstock-0.99.3/cardstock/examples/Dice.cds
+-rw-r--r--   0 benjie     (501) staff       (20)     3451 2022-09-14 20:33:21.000000 cardstock-0.99.3/cardstock/examples/Factor.cds
+-rw-r--r--   0 benjie     (501) staff       (20)    33761 2022-12-28 00:38:48.000000 cardstock-0.99.3/cardstock/examples/Fifteen.cds
+-rw-r--r--   0 benjie     (501) staff       (20)     4907 2022-09-14 20:33:21.000000 cardstock-0.99.3/cardstock/examples/Flappy.cds
+-rw-r--r--   0 benjie     (501) staff       (20)     7885 2022-09-14 20:33:21.000000 cardstock-0.99.3/cardstock/examples/Graph.cds
+-rw-r--r--   0 benjie     (501) staff       (20)     8049 2022-09-14 20:33:21.000000 cardstock-0.99.3/cardstock/examples/Guess.cds
+-rw-r--r--   0 benjie     (501) staff       (20)     9259 2022-12-28 00:38:48.000000 cardstock-0.99.3/cardstock/examples/Hanoi.cds
+-rw-r--r--   0 benjie     (501) staff       (20)    29952 2022-12-28 00:38:48.000000 cardstock-0.99.3/cardstock/examples/Logo.cds
+-rw-r--r--   0 benjie     (501) staff       (20)     3083 2022-09-14 20:33:21.000000 cardstock-0.99.3/cardstock/examples/Magic.cds
+-rw-r--r--   0 benjie     (501) staff       (20)    16438 2022-09-14 20:33:21.000000 cardstock-0.99.3/cardstock/examples/Mastermind.cds
+-rw-r--r--   0 benjie     (501) staff       (20)     9318 2022-09-14 20:33:21.000000 cardstock-0.99.3/cardstock/examples/Maze.cds
+-rw-r--r--   0 benjie     (501) staff       (20)    25585 2022-09-14 20:33:21.000000 cardstock-0.99.3/cardstock/examples/Morph.cds
+-rw-r--r--   0 benjie     (501) staff       (20)    22300 2022-09-14 20:33:21.000000 cardstock-0.99.3/cardstock/examples/Navigation.cds
+-rw-r--r--   0 benjie     (501) staff       (20)     8298 2022-09-14 20:33:21.000000 cardstock-0.99.3/cardstock/examples/Number-puzzle.cds
+-rw-r--r--   0 benjie     (501) staff       (20)     4052 2022-09-14 20:33:21.000000 cardstock-0.99.3/cardstock/examples/Pong.cds
+-rw-r--r--   0 benjie     (501) staff       (20)     2032 2022-09-14 20:33:21.000000 cardstock-0.99.3/cardstock/examples/Requests.cds
+-rw-r--r--   0 benjie     (501) staff       (20)     5108 2022-09-14 20:33:21.000000 cardstock-0.99.3/cardstock/examples/Scene.cds
+-rw-r--r--   0 benjie     (501) staff       (20)     3328 2022-09-14 20:33:21.000000 cardstock-0.99.3/cardstock/examples/Serial.cds
+-rw-r--r--   0 benjie     (501) staff       (20)    10074 2022-09-14 20:33:21.000000 cardstock-0.99.3/cardstock/examples/Snake.cds
+-rw-r--r--   0 benjie     (501) staff       (20)     8889 2022-09-14 20:33:21.000000 cardstock-0.99.3/cardstock/examples/Tanks.cds
+-rw-r--r--   0 benjie     (501) staff       (20)    12616 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/examples/Tetris.cds
+-rw-r--r--   0 benjie     (501) staff       (20)    14073 2022-09-14 20:33:21.000000 cardstock-0.99.3/cardstock/examples/TicTacToe.cds
+-rw-r--r--   0 benjie     (501) staff       (20)    84929 2022-09-14 20:33:21.000000 cardstock-0.99.3/cardstock/examples/Welcome.cds
+-rw-r--r--   0 benjie     (501) staff       (20)    24364 2022-12-28 00:38:48.000000 cardstock-0.99.3/cardstock/examples/Wordel.cds
+-rw-r--r--   0 benjie     (501) staff       (20)   103912 2021-11-02 20:40:58.000000 cardstock-0.99.3/cardstock/examples/click.wav
+-rw-r--r--   0 benjie     (501) staff       (20)    17826 2021-11-02 20:40:58.000000 cardstock-0.99.3/cardstock/examples/puff.wav
+-rw-r--r--   0 benjie     (501) staff       (20)    20544 2021-11-02 20:40:58.000000 cardstock-0.99.3/cardstock/examples/ship-off.png
+-rw-r--r--   0 benjie     (501) staff       (20)    20749 2021-11-02 20:40:58.000000 cardstock-0.99.3/cardstock/examples/ship-on.png
+-rw-r--r--   0 benjie     (501) staff       (20)    16127 2022-02-18 23:23:29.000000 cardstock-0.99.3/cardstock/examples/simple-red-apple.png
+-rw-r--r--   0 benjie     (501) staff       (20)   451172 2021-11-02 20:40:58.000000 cardstock-0.99.3/cardstock/examples/yay.wav
+-rw-r--r--   0 benjie     (501) staff       (20)     8247 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/findEngineDesigner.py
+-rw-r--r--   0 benjie     (501) staff       (20)     6255 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/findEngineViewer.py
+-rw-r--r--   0 benjie     (501) staff       (20)     1929 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/flippedGCDC.py
+-rw-r--r--   0 benjie     (501) staff       (20)     3391 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/generator.py
+-rw-r--r--   0 benjie     (501) staff       (20)    98557 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/helpData.py
+-rw-r--r--   0 benjie     (501) staff       (20)    35856 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/helpDialogs.py
+-rw-r--r--   0 benjie     (501) staff       (20)     1403 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/imageFactory.py
+-rw-r--r--   0 benjie     (501) staff       (20)     7614 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/mediaSearchDialogs.py
+-rw-r--r--   0 benjie     (501) staff       (20)    22848 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/migrations.py
+-rw-r--r--   0 benjie     (501) staff       (20)    24777 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/propertyInspector.py
+-rw-r--r--   0 benjie     (501) staff       (20)    13307 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/pythonEditor.py
+-rw-r--r--   0 benjie     (501) staff       (20)     1792 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/resourcePathManager.py
+-rw-r--r--   0 benjie     (501) staff       (20)    44284 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/runner.py
+-rw-r--r--   0 benjie     (501) staff       (20)     1797 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/sanitizer.py
+-rw-r--r--   0 benjie     (501) staff       (20)     6625 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/simpleListBox.py
+-rw-r--r--   0 benjie     (501) staff       (20)    25807 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/stackExporter.py
+-rw-r--r--   0 benjie     (501) staff       (20)    52175 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/stackManager.py
+-rw-r--r--   0 benjie     (501) staff       (20)     4747 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/stackModel.py
+-rw-r--r--   0 benjie     (501) staff       (20)     3077 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/standalone.py
+-rw-r--r--   0 benjie     (501) staff       (20)    38367 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/tools.py
+-rw-r--r--   0 benjie     (501) staff       (20)    12828 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/uiButton.py
+-rw-r--r--   0 benjie     (501) staff       (20)    18732 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/uiCard.py
+-rw-r--r--   0 benjie     (501) staff       (20)    12370 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/uiGroup.py
+-rw-r--r--   0 benjie     (501) staff       (20)     7536 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/uiImage.py
+-rw-r--r--   0 benjie     (501) staff       (20)    25234 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/uiShape.py
+-rw-r--r--   0 benjie     (501) staff       (20)    12212 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/uiTextBase.py
+-rw-r--r--   0 benjie     (501) staff       (20)    14645 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/uiTextField.py
+-rw-r--r--   0 benjie     (501) staff       (20)     8698 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/uiTextLabel.py
+-rw-r--r--   0 benjie     (501) staff       (20)    71637 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/uiView.py
+-rw-r--r--   0 benjie     (501) staff       (20)     8654 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/uiWebView.py
+-rw-r--r--   0 benjie     (501) staff       (20)    10190 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/variablesWindow.py
+-rw-r--r--   0 benjie     (501) staff       (20)      360 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/version.py
+-rw-r--r--   0 benjie     (501) staff       (20)    26514 2023-05-28 23:12:56.000000 cardstock-0.99.3/cardstock/viewer.py
+drwxr-xr-x   0 benjie     (501) staff       (20)        0 2023-05-28 23:20:22.496345 cardstock-0.99.3/cardstock.egg-info/
+-rw-r--r--   0 benjie     (501) staff       (20)     7087 2023-05-28 23:20:22.000000 cardstock-0.99.3/cardstock.egg-info/PKG-INFO
+-rw-r--r--   0 benjie     (501) staff       (20)     3737 2023-05-28 23:20:22.000000 cardstock-0.99.3/cardstock.egg-info/SOURCES.txt
+-rw-r--r--   0 benjie     (501) staff       (20)        1 2023-05-28 23:20:22.000000 cardstock-0.99.3/cardstock.egg-info/dependency_links.txt
+-rw-r--r--   0 benjie     (501) staff       (20)      102 2023-05-28 23:20:22.000000 cardstock-0.99.3/cardstock.egg-info/entry_points.txt
+-rw-r--r--   0 benjie     (501) staff       (20)       52 2023-05-28 23:20:22.000000 cardstock-0.99.3/cardstock.egg-info/requires.txt
+-rw-r--r--   0 benjie     (501) staff       (20)       10 2023-05-28 23:20:22.000000 cardstock-0.99.3/cardstock.egg-info/top_level.txt
+-rw-r--r--   0 benjie     (501) staff       (20)      103 2021-11-02 20:40:58.000000 cardstock-0.99.3/pyproject.toml
+-rw-r--r--   0 benjie     (501) staff       (20)      957 2023-05-28 23:20:22.497288 cardstock-0.99.3/setup.cfg
```

### Comparing `cardstock-0.99.2/LICENSE` & `cardstock-0.99.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.2/PKG-INFO` & `cardstock-0.99.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardstock
-Version: 0.99.2
+Version: 0.99.3
 Summary: A simple development and rapid prototyping tool for quickly building multi-platform desktop programs.
 Home-page: https://github.com/benjie-git/CardStock/wiki
 Author: Ben Levitt
 Author-email: benjie@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
@@ -29,15 +29,15 @@
 ## Features
 
 ### The Basics
 * CardStock lets you design stacks on MacOS, Windows, and GNU/Linux.  You can run CardStock stacks on those platforms, or on any modern web browser, include on Chromebooks and smartphones.
 * You can build programs using objects including text and graphics, images, buttons, text entry fields, and web views.
 * You can use your own python code to manipulate the objects and respond to mouse and keyboard events.
 * You can play sound files from your code.
-* You can search and use clip art in your stacks, thanks to integration with https://openclipart.com.
+* You can search and use clip art in your stacks, thanks to integration with https://openclipart.org.
 * In-context help appears in the app, right where you need it.  And can be turned off when you no longer want it taking up space.
 * All of the creature comforts you've come to expect from a proper application, like full Undo/Redo, and a Find/Replace system that works throughout all of your code and object properties.
 
 ### More Advanced
 * You can animate changes to most properties of objects, to bring your creations to life.
 * Objects can have speed, and can be set up to automatically bounce off of other objects.
 * You can **import** other python modules into your code, and use them make web requests and display the results, control robots, or run machine learning code, all from within your CardStock stack.
@@ -47,14 +47,16 @@
 * View all code used in a whole stack in one place, and click a line to jump to that line in that object's code editor for that event.
 * View recent error messages, and click one to jump to the offending line of code in the Designer.
 * You can export a stack into a standalone application that you can share and distribute, or upload it to the web, on https://cardstock.run.
 
 ### Future Plans
 * Build a web-based design tool to allow creating and editing stacks directly on https://cardstock.run.
 * Add a built-in library of sounds to use, and the ability to record your own sounds.
+* Allow looping sounds, and playing synthesized notes.
+* Add more tutorials for CardStock, and for learning python through CardStock.
 * Allow filling shapes with color gradients.
 * Add app icons for the CardStock Designer and Viewer.
 
 ________
 ## Known Issues
 * TextFields, and WebViews always remain in front of shapes and images, which get drawn directly on the card view.
 * Visual selection indicators (the blue dotted outlines) are drawn behind native views, and so can hide behind overlapping text fields and web views.
@@ -90,9 +92,9 @@
 2. Note that the pre-built Windows app is not yet code-signed, so Windows will complain the first time you open the app. If a window appears saying "Windows protected your PC", click the More Info link at the end of the warning paragraph, and then the "Run Anyway" button that appears at the bottom of the window.
 
 
 ## Reference
 * [CardStock Wiki](https://github.com/benjie-git/CardStock/wiki)
 * [CardStock on Reddit](https://www.reddit.com/r/CardStockPython/)
 * [CardStock Manual](https://github.com/benjie-git/CardStock/wiki/Manual)
-* [CardStock Tutorial](https://github.com/benjie-git/CardStock/wiki/Tutorial)
+* [CardStock Tutorial](https://github.com/benjie-git/CardStock/wiki/Tutorial-Dice)
 * [CardStock Reference Guide](https://github.com/benjie-git/CardStock/wiki/Reference)
```

### Comparing `cardstock-0.99.2/README.md` & `cardstock-0.99.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 ## Features
 
 ### The Basics
 * CardStock lets you design stacks on MacOS, Windows, and GNU/Linux.  You can run CardStock stacks on those platforms, or on any modern web browser, include on Chromebooks and smartphones.
 * You can build programs using objects including text and graphics, images, buttons, text entry fields, and web views.
 * You can use your own python code to manipulate the objects and respond to mouse and keyboard events.
 * You can play sound files from your code.
-* You can search and use clip art in your stacks, thanks to integration with https://openclipart.com.
+* You can search and use clip art in your stacks, thanks to integration with https://openclipart.org.
 * In-context help appears in the app, right where you need it.  And can be turned off when you no longer want it taking up space.
 * All of the creature comforts you've come to expect from a proper application, like full Undo/Redo, and a Find/Replace system that works throughout all of your code and object properties.
 
 ### More Advanced
 * You can animate changes to most properties of objects, to bring your creations to life.
 * Objects can have speed, and can be set up to automatically bounce off of other objects.
 * You can **import** other python modules into your code, and use them make web requests and display the results, control robots, or run machine learning code, all from within your CardStock stack.
@@ -33,14 +33,16 @@
 * View all code used in a whole stack in one place, and click a line to jump to that line in that object's code editor for that event.
 * View recent error messages, and click one to jump to the offending line of code in the Designer.
 * You can export a stack into a standalone application that you can share and distribute, or upload it to the web, on https://cardstock.run.
 
 ### Future Plans
 * Build a web-based design tool to allow creating and editing stacks directly on https://cardstock.run.
 * Add a built-in library of sounds to use, and the ability to record your own sounds.
+* Allow looping sounds, and playing synthesized notes.
+* Add more tutorials for CardStock, and for learning python through CardStock.
 * Allow filling shapes with color gradients.
 * Add app icons for the CardStock Designer and Viewer.
 
 ________
 ## Known Issues
 * TextFields, and WebViews always remain in front of shapes and images, which get drawn directly on the card view.
 * Visual selection indicators (the blue dotted outlines) are drawn behind native views, and so can hide behind overlapping text fields and web views.
@@ -76,9 +78,9 @@
 2. Note that the pre-built Windows app is not yet code-signed, so Windows will complain the first time you open the app. If a window appears saying "Windows protected your PC", click the More Info link at the end of the warning paragraph, and then the "Run Anyway" button that appears at the bottom of the window.
 
 
 ## Reference
 * [CardStock Wiki](https://github.com/benjie-git/CardStock/wiki)
 * [CardStock on Reddit](https://www.reddit.com/r/CardStockPython/)
 * [CardStock Manual](https://github.com/benjie-git/CardStock/wiki/Manual)
-* [CardStock Tutorial](https://github.com/benjie-git/CardStock/wiki/Tutorial)
+* [CardStock Tutorial](https://github.com/benjie-git/CardStock/wiki/Tutorial-Dice)
 * [CardStock Reference Guide](https://github.com/benjie-git/CardStock/wiki/Reference)
```

### Comparing `cardstock-0.99.2/cardstock/CardStock_Designer_mac.spec` & `cardstock-0.99.3/cardstock/CardStock_Designer_mac.spec`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.2/cardstock/CardStock_Viewer_mac.spec` & `cardstock-0.99.3/cardstock/CardStock_Viewer_mac.spec`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.2/cardstock/allCodeWindow.py` & `cardstock-0.99.3/cardstock/allCodeWindow.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# This file is part of CardStock.
+#     https://github.com/benjie-git/CardStock
+#
+# Copyright Ben Levitt 2020-2023
+#
+# This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
+# of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
+
 import wx
 import pythonEditor
 import wx.stc as stc
 from uiView import UiView
 
 
 class AllCodeWindow(wx.Frame):
```

### Comparing `cardstock-0.99.2/cardstock/analyzer.py` & `cardstock-0.99.3/cardstock/analyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# This file is part of CardStock.
+#     https://github.com/benjie-git/CardStock
+#
+# Copyright Ben Levitt 2020-2023
+#
+# This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
+# of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
+
 import wx
 import ast
 import helpData
 import threading
 import re
 import types
```

### Comparing `cardstock-0.99.2/cardstock/appCommands.py` & `cardstock-0.99.3/cardstock/appCommands.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# This file is part of CardStock.
+#     https://github.com/benjie-git/CardStock
+#
+# Copyright Ben Levitt 2020-2023
+#
+# This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
+# of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
+
 from wx.lib.docview import Command
 
 """
 These are the Undoable/Redoable commands used while editing the stack in the designer.  All modifications to the stack
 are done through these commands, so that everything is undoable.
 """
```

### Comparing `cardstock-0.99.2/cardstock/build.py` & `cardstock-0.99.3/cardstock/build.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# This file is part of CardStock.
+#     https://github.com/benjie-git/CardStock
+#
+# Copyright Ben Levitt 2020-2023
+#
+# This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
+# of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
+
 import wx
 import os
 import shutil
 import PyInstaller.__main__
 import version
 
 EXTRA_MODULES = []
```

### Comparing `cardstock-0.99.2/cardstock/cardstockFrameParts.py` & `cardstock-0.99.3/cardstock/cardstockFrameParts.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# This file is part of CardStock.
+#     https://github.com/benjie-git/CardStock
+#
+# Copyright Ben Levitt 2020-2023
+#
+# This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
+# of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
+
 import wx
 import sys
 
 # CardStock-specific Point, Size, RealPoint subclasses
 # These notify their model when their components are changed, so that, for example:
 # button.center.x = 100  will notify the button's model that the center changed.
```

### Comparing `cardstock-0.99.2/cardstock/codeInspector.py` & `cardstock-0.99.3/cardstock/codeInspector.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# This file is part of CardStock.
+#     https://github.com/benjie-git/CardStock
+#
+# Copyright Ben Levitt 2020-2023
+#
+# This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
+# of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
+
 import wx
 import pythonEditor
 import wx.stc
 import helpData
 import appCommands
 from uiView import UiView
```

### Comparing `cardstock-0.99.2/cardstock/codeInspectorMulti.py` & `cardstock-0.99.3/cardstock/codeInspectorMulti.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# This file is part of CardStock.
+#     https://github.com/benjie-git/CardStock
+#
+# Copyright Ben Levitt 2020-2023
+#
+# This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
+# of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
+
 import wx
 import pythonEditor
 import wx.stc
 import helpData
 import appCommands
 from uiView import UiView
 from simpleListBox import SimpleListBox
```

### Comparing `cardstock-0.99.2/cardstock/codeRunnerThread.py` & `cardstock-0.99.3/cardstock/codeRunnerThread.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# This file is part of CardStock.
+#     https://github.com/benjie-git/CardStock
+#
+# Copyright Ben Levitt 2020-2023
+#
+# This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
+# of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
+
 """
 Modified from the Killable Threads post by tomer filiba:
 http://tomerfiliba.com/recipes/Thread2/
 """
 
 import threading
 import inspect
```

### Comparing `cardstock-0.99.2/cardstock/consoleWindow.py` & `cardstock-0.99.3/cardstock/consoleWindow.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# This file is part of CardStock.
+#     https://github.com/benjie-git/CardStock
+#
+# Copyright Ben Levitt 2020-2023
+#
+# This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
+# of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
+
 import wx
 import wx.stc as stc
 from io import StringIO
 import pythonEditor
 from wx.lib.docview import CommandProcessor, Command
 from codeRunnerThread import RunOnMainSync
 import sys
@@ -62,14 +70,15 @@
         self.runner = None
         self.didSetDown = False
 
         self.textBox.Bind(stc.EVT_STC_ZOOM, self.OnZoom)
         self.textBox.Bind(stc.EVT_STC_CHARADDED, self.OnChar)
         self.textBox.Bind(stc.EVT_STC_CHANGE, self.OnTextChange)
         self.textBox.Bind(wx.EVT_KEY_DOWN, self.OnKeyDown)
+        self.textBox.Bind(wx.EVT_LEFT_UP, self.OnMouseUp)
         self.textBox.Bind(stc.EVT_STC_UPDATEUI, self.UpdateEditable)
         self.Bind(wx.EVT_SIZE, self.OnResize)
         self.Bind(wx.EVT_CLOSE, self.OnClose)
 
     def Show(self, doShow=True):
         super().Show(doShow)
         if doShow and not self.hasShown:
@@ -180,14 +189,19 @@
                     self.historyPos += 1
                     self.SetCommandText(cmdHistory[self.historyPos])
                     return
                 elif self.historyPos == len(cmdHistory)-1:
                     self.historyPos = None
                     self.SetCommandText(self.workingCommand)
                     return
+        elif chr(event.GetUnicodeKey()).isalnum() and self.allowInput and not self.textBox.IsEditable():
+            last = self.textBox.GetLastPosition()
+            self.textBox.SetSelection(last, last)
+            self.UpdateEditable()
+
         event.Skip()
 
     def OnClose(self, event):
         event.Veto()
         self.Hide()
 
     def SetStreamsUp(self):
@@ -220,32 +234,44 @@
         self.stderrIO = None
 
     def UpdateEditable(self, event=None):
         # Only make the text editable when the cursor is in the current command
         if self.allowInput:
             start = self.textBox.GetSelectionStart()
             end = self.textBox.GetSelectionEnd()
+            if not wx.GetMouseState().LeftIsDown() and start == end and start < self.lastOutputPos and start >= self.lastOutputPos - 2:
+                start = self.lastOutputPos
+                end = start
+                self.textBox.SetSelection(start, end)
             editable = (start >= self.lastOutputPos and end >= self.lastOutputPos)
             self.textBox.SetEditable(editable)
         else:
             self.textBox.SetEditable(False)
 
+    def OnMouseUp(self, event):
+        if self.allowInput:
+            wx.CallAfter(self.UpdateEditable)
+        event.Skip()
+
     def Clear(self):
         if self.allowInput:
             self.textBox.SetEditable(True)
             self.textBox.ChangeValue("> ")
             self.lastOutputPos = 2
             self.UpdateEditable()
             self.textBox.SetSelection(self.lastOutputPos, self.lastOutputPos)
         else:
             self.textBox.ChangeValue("  ")
 
     def OnReturn(self):
         # Return key was pressed, and not for autocompletion, nor in the middle of a multiline command entry
         if self.allowInput:
+            last = self.textBox.GetLastPosition()
+            self.textBox.SetSelection(last, last)
+            self.UpdateEditable()
             code = self.GetCommandText()
             self.textBox.AppendText('\n')
             self.lastOutputPos = self.textBox.GetLastPosition()
             self.textBox.SetSelection(self.lastOutputPos, self.lastOutputPos)
             if len(code.strip()) > 0:
                 cmdHistory.append(code)
                 self.historyPos = None
```

### Comparing `cardstock-0.99.2/cardstock/controlPanel.py` & `cardstock-0.99.3/cardstock/controlPanel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# This file is part of CardStock.
+#     https://github.com/benjie-git/CardStock
+#
+# Copyright Ben Levitt 2020-2023
+#
+# This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
+# of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
+
 import wx
 import wx.grid
 import wx.html
 import os
 import mediaSearchDialogs
 import propertyInspector
 from codeInspectorMulti import CodeInspectorContainer
```

### Comparing `cardstock-0.99.2/cardstock/designer.py` & `cardstock-0.99.3/cardstock/designer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 #!/usr/bin/python3
+# This file is part of CardStock.
+#     https://github.com/benjie-git/CardStock
+#
+# Copyright Ben Levitt 2020-2023
+#
+# This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
+# of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
-# designer.py
 """
 This is the root of the main CardStock stack designer application.
 It allows building and editing a stack, and running it to test it.
 Use the viewer.py app to run and use a stack, without being able to edit it.
 """
 
 import os
 import sys
 import json
 import configparser
 import wx
+import embeddedImages
 from time import sleep
 import version
 from tools import *
 from stackManager import StackManager
 from controlPanel import ControlPanel
 from viewer import ViewerFrame
 import helpDialogs
@@ -111,15 +118,16 @@
         self.editMenu = None
         self.MakeMenuBar()
         self.filename = None
         self.app = None
         # self.lastStats = {}
 
         self.toolbar = self.CreateToolBar(style=wx.TB_TEXT)
-        self.toolbar.AddTool(ID_RUN, 'Run Stack', wx.ArtProvider.GetBitmap(wx.ART_FULL_SCREEN), wx.NullBitmap)
+        icn = embeddedImages.run.GetBitmap()
+        self.toolbar.AddTool(ID_RUN, 'Run Stack', icn, wx.NullBitmap)
 
         self.toolbar.AddStretchableSpace()
 
         self.cardPicker = wx.Choice(parent=self.toolbar)
         self.cardPicker.Bind(wx.EVT_CHOICE, self.OnPickCard)
         self.cardPickerToolId = self.toolbar.AddControl(self.cardPicker).GetId()
 
@@ -439,15 +447,15 @@
         self.Bind(wx.EVT_MENU, self.OnMenuRunFrom, id=ID_RUN_FROM)
         self.Bind(wx.EVT_MENU, self.OnMenuSearchImage, id=ID_SEARCH_IMAGE)
         # self.Bind(wx.EVT_MENU, self.OnMenuSearchSound, id=ID_SEARCH_SOUND)
         self.Bind(wx.EVT_MENU, self.OnMenuExit, id=wx.ID_EXIT)
 
         self.Bind(wx.EVT_MENU, self.OnMenuAbout, id=wx.ID_ABOUT)
         self.Bind(wx.EVT_MENU, self.OnMenuHelp, id=wx.ID_HELP)
-        self.Bind(wx.EVT_MENU, self.OnMenuBasics, id=ID_BASICS)
+        # self.Bind(wx.EVT_MENU, self.OnMenuBasics, id=ID_BASICS)
         self.Bind(wx.EVT_MENU, self.OnMenuReference, id=wx.ID_REFRESH)
         self.Bind(wx.EVT_MENU, self.OnMenuContextHelp, id=wx.ID_CONTEXT_HELP)
 
         self.Bind(wx.EVT_MENU, self.OnUndo, id=wx.ID_UNDO)
         self.Bind(wx.EVT_MENU, self.OnRedo, id=wx.ID_REDO)
         self.Bind(wx.EVT_MENU, self.OnSelectAll, id=wx.ID_SELECTALL)
         self.Bind(wx.EVT_MENU, self.OnCut, id=wx.ID_CUT)
@@ -1037,15 +1045,16 @@
 
         if wx.Platform == "__WXMAC__":
             self.toolbar.RemoveTool(self.cardPickerToolId)
 
         # Update toolbar to show 'Run This Card' only when on card 2+
         isShowingTool = self.toolbar.FindById(ID_RUN_FROM)
         if not isShowingTool and self.stackManager.cardIndex > 0:
-            self.toolbar.InsertTool(1, ID_RUN_FROM, 'Run This Card', wx.ArtProvider.GetBitmap(wx.ART_FULL_SCREEN), wx.NullBitmap)
+            icn = embeddedImages.run_card.GetBitmap()
+            self.toolbar.InsertTool(1, ID_RUN_FROM, 'Run This Card', icn, wx.NullBitmap)
         elif isShowingTool and self.stackManager.cardIndex == 0:
             self.toolbar.RemoveTool(ID_RUN_FROM)
 
         if wx.Platform == "__WXMAC__":
             self.cardPickerToolId = self.toolbar.InsertControl(2 if (self.stackManager.cardIndex == 0) else 3, self.cardPicker).GetId()
         self.toolbar.Realize()
 
@@ -1171,19 +1180,14 @@
         self.findEngine.ReplaceAll()
 
     def OnMenuAbout(self, event):
         dlg = helpDialogs.CardStockAbout(self)
         dlg.ShowModal()
         dlg.Destroy()
 
-    def OnMenuBasics(self, event):
-        dlg = helpDialogs.CardStockBasics(self)
-        dlg.Bind(wx.EVT_CLOSE, self.OnHelpClose)
-        dlg.Show()
-
     def OnMenuHelp(self, event):
         dlg = helpDialogs.CardStockManual(self)
         dlg.Bind(wx.EVT_CLOSE, self.OnHelpClose)
         dlg.Show()
 
     def OnMenuReference(self, event):
         dlg = helpDialogs.CardStockReference(self)
```

### Comparing `cardstock-0.99.2/cardstock/embeddedImages.py` & `cardstock-0.99.3/cardstock/embeddedImages.py`

 * *Files 4% similar despite different names*

```diff
@@ -1692,7 +1692,138 @@
     b'yR6woNT+tBtH+oEEdnZ2emTUNI18Pg9AtVqlVCqNLf1QRXhyctJz75qmUSgUJpY+zA98+fDw'
     b'8H2nB5AkCcMwWF9fH9gJp6enj55eCNHlDeLx+DrwQ6gCvpnww++Afvc6rPTB3EECsr8huDGT'
     b'yXB0dBSadFjpA7nl0Bpw3cen8cbGRtdcH7fqPacUCrQKzJumKVqtlrBtO9QTFItFkc1mRTab'
     b'Fefn5wO9geu6wrZt0Wq1hGmaApj3sHqKcBmI3N/fv/ILUZKkif2B67oIIdoFODMz89zzA78F'
     b'r+B3IHV7e6s5jkPwc113pC8sR7PZdIGUhxVqy+eBF9fX1zsLCwt7siyPbMmDRewRetNsNmPp'
     b'dPor4FfPFz76MJkHnnubGoZh3IxjTj3Z7WQy+RR44uV91Qne72mmAkveaybm7RNjDDnh+f+G'
     b'J/tb/o9A/AMSM0NrGYtWTwAAAABJRU5ErkJggg==')
+
+run = PyEmbeddedImage(
+    b'iVBORw0KGgoAAAANSUhEUgAAABwAAAAcCAYAAAByDd+UAAABrWlDQ1BJQ0MgUHJvZmlsZQAA'
+    b'KJF9kTtII1EUhj+jooiPQguLFFOolYqohaXGQgWFEBV8FU4mr4VkvEwSll22FGwVBdHGV2El'
+    b'WKnFFlsIguADBN0F2XYbK8VlQWQ8N6MkruiBw/345/znnjkXfAemUsmSNkjZGSfUFzDGxieM'
+    b'sj+U4qeaIvymlVY9weAgEi/n6/h7KXUSFy2611nr93+nezvZrzXX/cdH2YW39a+iKhJNW1Bk'
+    b'CHdbyskITwsHP2eU5l3hOkeGEj7UHPf4p+awxze5mpFQL/h0T8NKmBFh3bPZSjgpYT13QyQV'
+    b'0bry2Na8pDlc4I0XcCqZtZ7n1H9YGbVHh3W9pJ8+BhgiiEGYLJ9IkqFFTluUNCH5HnjH35nz'
+    b'9zKD4guOeOIkxG3QI4qSTlHhAelk0UqzcDttkh36bf7feV6bWYeueyiez2vhZdifg/pfea1h'
+    b'DWpmYe9QmY6Zk4olfbEY3G7Lk4xD7TlUTKZjHe3e9JUBKP3tuneNULYIj/Ou+7Dhuo+bYr6G'
+    b'H7a35+debF3ByDcYPIGVVWiKy51T7+yjPLePj3dWXrjzJ53OgWf+1WfBAAAAsmVYSWZNTQAq'
+    b'AAAACAAHARIAAwAAAAEAAQAAARoABQAAAAEAAABiARsABQAAAAEAAABqASgAAwAAAAEAAwAA'
+    b'ATEAAgAAAA0AAAByATIAAgAAABQAAACAh2kABAAAAAEAAACUAAAAAAAAAGAAAAABAAAAYAAA'
+    b'AAFHSU1QIDIuMTAuMzIAADIwMjM6MDU6MjcgMjA6MzA6MDYAAAKgAgAEAAAAAQAAABygAwAE'
+    b'AAAAAQAAABwAAAAAQ7GHmgAAAAlwSFlzAAAOxAAADsQBlSsOGwAACFFpVFh0WE1MOmNvbS5h'
+    b'ZG9iZS54bXAAAAAAADx4OnhtcG1ldGEgeG1sbnM6eD0iYWRvYmU6bnM6bWV0YS8iIHg6eG1w'
+    b'dGs9IlhNUCBDb3JlIDYuMC4wIj4KICAgPHJkZjpSREYgeG1sbnM6cmRmPSJodHRwOi8vd3d3'
+    b'LnczLm9yZy8xOTk5LzAyLzIyLXJkZi1zeW50YXgtbnMjIj4KICAgICAgPHJkZjpEZXNjcmlw'
+    b'dGlvbiByZGY6YWJvdXQ9IiIKICAgICAgICAgICAgeG1sbnM6ZXhpZj0iaHR0cDovL25zLmFk'
+    b'b2JlLmNvbS9leGlmLzEuMC8iCiAgICAgICAgICAgIHhtbG5zOkdJTVA9Imh0dHA6Ly93d3cu'
+    b'Z2ltcC5vcmcveG1wLyIKICAgICAgICAgICAgeG1sbnM6ZGM9Imh0dHA6Ly9wdXJsLm9yZy9k'
+    b'Yy9lbGVtZW50cy8xLjEvIgogICAgICAgICAgICB4bWxuczp4bXA9Imh0dHA6Ly9ucy5hZG9i'
+    b'ZS5jb20veGFwLzEuMC8iCiAgICAgICAgICAgIHhtbG5zOnhtcE1NPSJodHRwOi8vbnMuYWRv'
+    b'YmUuY29tL3hhcC8xLjAvbW0vIgogICAgICAgICAgICB4bWxuczpzdEV2dD0iaHR0cDovL25z'
+    b'LmFkb2JlLmNvbS94YXAvMS4wL3NUeXBlL1Jlc291cmNlRXZlbnQjIgogICAgICAgICAgICB4'
+    b'bWxuczp0aWZmPSJodHRwOi8vbnMuYWRvYmUuY29tL3RpZmYvMS4wLyI+CiAgICAgICAgIDxl'
+    b'eGlmOkNvbG9yU3BhY2U+MTwvZXhpZjpDb2xvclNwYWNlPgogICAgICAgICA8R0lNUDpBUEk+'
+    b'Mi4wPC9HSU1QOkFQST4KICAgICAgICAgPEdJTVA6VmVyc2lvbj4yLjEwLjMyPC9HSU1QOlZl'
+    b'cnNpb24+CiAgICAgICAgIDxHSU1QOlRpbWVTdGFtcD4xNjg1MjQ0NjA5MjE5NzAxPC9HSU1Q'
+    b'OlRpbWVTdGFtcD4KICAgICAgICAgPEdJTVA6UGxhdGZvcm0+TWFjIE9TPC9HSU1QOlBsYXRm'
+    b'b3JtPgogICAgICAgICA8ZGM6Rm9ybWF0PmltYWdlL3BuZzwvZGM6Rm9ybWF0PgogICAgICAg'
+    b'ICA8eG1wOk1vZGlmeURhdGU+MjAyMy0wNS0yN1QyMDozMDowNjwveG1wOk1vZGlmeURhdGU+'
+    b'CiAgICAgICAgIDx4bXA6Q3JlYXRvclRvb2w+R0lNUCAyLjEwLjMyPC94bXA6Q3JlYXRvclRv'
+    b'b2w+CiAgICAgICAgIDx4bXA6TWV0YWRhdGFEYXRlPjIwMjM6MDU6MjdUMjA6MzA6MDYtMDc6'
+    b'MDA8L3htcDpNZXRhZGF0YURhdGU+CiAgICAgICAgIDx4bXBNTTpPcmlnaW5hbERvY3VtZW50'
+    b'SUQ+eG1wLmRpZDo1ZWRkOTg5Mi00MmU3LTQyYmQtOGMxNy03ZGU5ZDQ2ZWIwNWE8L3htcE1N'
+    b'Ok9yaWdpbmFsRG9jdW1lbnRJRD4KICAgICAgICAgPHhtcE1NOkhpc3Rvcnk+CiAgICAgICAg'
+    b'ICAgIDxyZGY6U2VxPgogICAgICAgICAgICAgICA8cmRmOmxpIHJkZjpwYXJzZVR5cGU9IlJl'
+    b'c291cmNlIj4KICAgICAgICAgICAgICAgICAgPHN0RXZ0OmNoYW5nZWQ+Lzwvc3RFdnQ6Y2hh'
+    b'bmdlZD4KICAgICAgICAgICAgICAgICAgPHN0RXZ0OnNvZnR3YXJlQWdlbnQ+R2ltcCAyLjEw'
+    b'IChNYWMgT1MpPC9zdEV2dDpzb2Z0d2FyZUFnZW50PgogICAgICAgICAgICAgICAgICA8c3RF'
+    b'dnQ6d2hlbj4yMDIzLTA1LTI3VDIwOjMwOjA5LTA3OjAwPC9zdEV2dDp3aGVuPgogICAgICAg'
+    b'ICAgICAgICAgICA8c3RFdnQ6aW5zdGFuY2VJRD54bXAuaWlkOjA0NWYxMTgwLTkxZGUtNGYx'
+    b'NS05MDU1LTljYjBkOTBkMWIwYjwvc3RFdnQ6aW5zdGFuY2VJRD4KICAgICAgICAgICAgICAg'
+    b'ICAgPHN0RXZ0OmFjdGlvbj5zYXZlZDwvc3RFdnQ6YWN0aW9uPgogICAgICAgICAgICAgICA8'
+    b'L3JkZjpsaT4KICAgICAgICAgICAgPC9yZGY6U2VxPgogICAgICAgICA8L3htcE1NOkhpc3Rv'
+    b'cnk+CiAgICAgICAgIDx4bXBNTTpEb2N1bWVudElEPmdpbXA6ZG9jaWQ6Z2ltcDphYzRkMmY0'
+    b'NC02Njc2LTRmMzYtYmQ0OC0yNjAxNmM4Nzg4Yzc8L3htcE1NOkRvY3VtZW50SUQ+CiAgICAg'
+    b'ICAgIDx4bXBNTTpJbnN0YW5jZUlEPnhtcC5paWQ6YjQwMzhhZTgtODA0NS00M2JlLWEwOTAt'
+    b'OWNlMzM0YzkxNDk1PC94bXBNTTpJbnN0YW5jZUlEPgogICAgICAgICA8dGlmZjpSZXNvbHV0'
+    b'aW9uVW5pdD4zPC90aWZmOlJlc29sdXRpb25Vbml0PgogICAgICAgICA8dGlmZjpPcmllbnRh'
+    b'dGlvbj4xPC90aWZmOk9yaWVudGF0aW9uPgogICAgICAgICA8dGlmZjpYUmVzb2x1dGlvbj45'
+    b'NjwvdGlmZjpYUmVzb2x1dGlvbj4KICAgICAgICAgPHRpZmY6WVJlc29sdXRpb24+OTY8L3Rp'
+    b'ZmY6WVJlc29sdXRpb24+CiAgICAgIDwvcmRmOkRlc2NyaXB0aW9uPgogICA8L3JkZjpSREY+'
+    b'CjwveDp4bXBtZXRhPgrcaa+GAAAB40lEQVRIDb2WPU7DQBCFw38LHYIuUiR6GgSHAJqUVOQK'
+    b'cAhoaFI7KeAUcAIEJR2CO4AEEn/v2+ygwSbENuuM9Ly74/V7ntnZtVutos3INefc8+rPunHy'
+    b'LoJ5w7eQd6YYWyQ7IhsKmUDfbEkdm2O+2q1FsCWGF+HT4VT9FQEj3TY3OOpcfMr6IkCsK2wK'
+    b't3F8r3ZfMFu0Tp0WQYoDI5UIrjKQEc2RYBFfqL8umPkCM9/E1gtmmg15J/fUhsaX8d6z2p67'
+    b'j2iltfWCg0jajoRE7qM41PgpzrlSy4uYld5Cfwnam3vRNSmcC5bmY/VtSZg/sajKCIonmC8W'
+    b'iohiQvhG2BbM2ELw/mpVBCEgAouc7XIiWLRsoWUBY86volUFjYwozIiOKBF+FPYEDO6CaB3B'
+    b'wKaLj5aI/BY6iJMKa/ofQTj984yp3A/hmkG0UHS2DuZM2RbSCHkKQdIF+VvkI6V3AnY2akLa'
+    b'32M/ND4lA3lY+HacMO6l8I8rmgfd243Pww1+WFVBXyiNb4upbfypHW35w7unxUh6eGcipGg6'
+    b'grfGPk9DqSDY+AeYysP6AoJdobFfDHF/f8P4iXoVEDUk/4kSdzDb5Jz8HACZ0NhvoriDFU4F'
+    b'efFZykezEl4h93uu9H9KmXf4AggRaoZT/061AAAAAElFTkSuQmCC')
+
+#----------------------------------------------------------------------
+run_card = PyEmbeddedImage(
+    b'iVBORw0KGgoAAAANSUhEUgAAABwAAAAcCAYAAAByDd+UAAABrGlDQ1BJQ0MgUHJvZmlsZQAA'
+    b'KJF9kTtII1EUhj+jQVl8FGthYTGFWiUiKuxiZWIhggshKvgqnExeC8l4mUREsFRsBYVlt1kf'
+    b'ha2VEWwUbAVB0F0QO7HQStFCkdlzMy6Ju+iBw/345/znnjkXfLumUpmqDsjaeSfaHzZGx8aN'
+    b'6iv8NFNPBYZp5VQoEhlE4u/5Oh5OpU7iJKh7XX/aC14urk8c+K2dnsJj5v/6V1EXT+QsqDCE'
+    b'ey3l5IWnhCOzeaV5W7jRkaGEDzWnPP6lOebxTbFmONoHPt3TsNJmXFj3DFhpJyus526JZ+Na'
+    b'Vx7bmlc1x8q8qTLOZmaslzn1H9Ym7JEhXS/ZTD8DfCGCQYwZvpIhT1BOW5QcUfkefsPfXfT3'
+    b'MY1iDkc8KdLiNgiJoqRTQnhAOlm0ExDupEOyS7/NvzsvadNr8PkeKpdLWuwbFJag6XdJa/kJ'
+    b'DQuwc6hMxyxKlZK+ZBJut+RJxuDjMXyYyCW7Or3pa8Pgv3Ddu1aoXoHnZdd9Wnfd5w0xn8O+'
+    b'7e35pRebZzA8D4NH8P0HtKXkzsk39lFT3Mf7O6sp3/kfYtiAdnHYnBAAAACyZVhJZk1NACoA'
+    b'AAAIAAcBEgADAAAAAQABAAABGgAFAAAAAQAAAGIBGwAFAAAAAQAAAGoBKAADAAAAAQADAAAB'
+    b'MQACAAAADQAAAHIBMgACAAAAFAAAAICHaQAEAAAAAQAAAJQAAAAAAAAAYAAAAAEAAABgAAAA'
+    b'AUdJTVAgMi4xMC4zMgAAMjAyMzowNToyNyAyMDozMDozOAAAAqACAAQAAAABAAAAHKADAAQA'
+    b'AAABAAAAHAAAAACy/RXkAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAIUWlUWHRYTUw6Y29tLmFk'
+    b'b2JlLnhtcAAAAAAAPHg6eG1wbWV0YSB4bWxuczp4PSJhZG9iZTpuczptZXRhLyIgeDp4bXB0'
+    b'az0iWE1QIENvcmUgNi4wLjAiPgogICA8cmRmOlJERiB4bWxuczpyZGY9Imh0dHA6Ly93d3cu'
+    b'dzMub3JnLzE5OTkvMDIvMjItcmRmLXN5bnRheC1ucyMiPgogICAgICA8cmRmOkRlc2NyaXB0'
+    b'aW9uIHJkZjphYm91dD0iIgogICAgICAgICAgICB4bWxuczpleGlmPSJodHRwOi8vbnMuYWRv'
+    b'YmUuY29tL2V4aWYvMS4wLyIKICAgICAgICAgICAgeG1sbnM6R0lNUD0iaHR0cDovL3d3dy5n'
+    b'aW1wLm9yZy94bXAvIgogICAgICAgICAgICB4bWxuczpkYz0iaHR0cDovL3B1cmwub3JnL2Rj'
+    b'L2VsZW1lbnRzLzEuMS8iCiAgICAgICAgICAgIHhtbG5zOnhtcD0iaHR0cDovL25zLmFkb2Jl'
+    b'LmNvbS94YXAvMS4wLyIKICAgICAgICAgICAgeG1sbnM6eG1wTU09Imh0dHA6Ly9ucy5hZG9i'
+    b'ZS5jb20veGFwLzEuMC9tbS8iCiAgICAgICAgICAgIHhtbG5zOnN0RXZ0PSJodHRwOi8vbnMu'
+    b'YWRvYmUuY29tL3hhcC8xLjAvc1R5cGUvUmVzb3VyY2VFdmVudCMiCiAgICAgICAgICAgIHht'
+    b'bG5zOnRpZmY9Imh0dHA6Ly9ucy5hZG9iZS5jb20vdGlmZi8xLjAvIj4KICAgICAgICAgPGV4'
+    b'aWY6Q29sb3JTcGFjZT4xPC9leGlmOkNvbG9yU3BhY2U+CiAgICAgICAgIDxHSU1QOkFQST4y'
+    b'LjA8L0dJTVA6QVBJPgogICAgICAgICA8R0lNUDpWZXJzaW9uPjIuMTAuMzI8L0dJTVA6VmVy'
+    b'c2lvbj4KICAgICAgICAgPEdJTVA6VGltZVN0YW1wPjE2ODUyNDQ2NDA0Njk3MTY8L0dJTVA6'
+    b'VGltZVN0YW1wPgogICAgICAgICA8R0lNUDpQbGF0Zm9ybT5NYWMgT1M8L0dJTVA6UGxhdGZv'
+    b'cm0+CiAgICAgICAgIDxkYzpGb3JtYXQ+aW1hZ2UvcG5nPC9kYzpGb3JtYXQ+CiAgICAgICAg'
+    b'IDx4bXA6TW9kaWZ5RGF0ZT4yMDIzLTA1LTI3VDIwOjMwOjM4PC94bXA6TW9kaWZ5RGF0ZT4K'
+    b'ICAgICAgICAgPHhtcDpDcmVhdG9yVG9vbD5HSU1QIDIuMTAuMzI8L3htcDpDcmVhdG9yVG9v'
+    b'bD4KICAgICAgICAgPHhtcDpNZXRhZGF0YURhdGU+MjAyMzowNToyN1QyMDozMDozOC0wNzow'
+    b'MDwveG1wOk1ldGFkYXRhRGF0ZT4KICAgICAgICAgPHhtcE1NOk9yaWdpbmFsRG9jdW1lbnRJ'
+    b'RD54bXAuZGlkOjE2OGFmMGEwLWExMjctNDVlYi05ZGI5LTM1YzFkMmZjOWZhMjwveG1wTU06'
+    b'T3JpZ2luYWxEb2N1bWVudElEPgogICAgICAgICA8eG1wTU06SGlzdG9yeT4KICAgICAgICAg'
+    b'ICAgPHJkZjpTZXE+CiAgICAgICAgICAgICAgIDxyZGY6bGkgcmRmOnBhcnNlVHlwZT0iUmVz'
+    b'b3VyY2UiPgogICAgICAgICAgICAgICAgICA8c3RFdnQ6Y2hhbmdlZD4vPC9zdEV2dDpjaGFu'
+    b'Z2VkPgogICAgICAgICAgICAgICAgICA8c3RFdnQ6c29mdHdhcmVBZ2VudD5HaW1wIDIuMTAg'
+    b'KE1hYyBPUyk8L3N0RXZ0OnNvZnR3YXJlQWdlbnQ+CiAgICAgICAgICAgICAgICAgIDxzdEV2'
+    b'dDp3aGVuPjIwMjMtMDUtMjdUMjA6MzA6NDAtMDc6MDA8L3N0RXZ0OndoZW4+CiAgICAgICAg'
+    b'ICAgICAgICAgIDxzdEV2dDppbnN0YW5jZUlEPnhtcC5paWQ6YTI0NDdhMWEtYTdmMi00Yjk3'
+    b'LTk5NjgtMzkxNzAwOWNjMGFiPC9zdEV2dDppbnN0YW5jZUlEPgogICAgICAgICAgICAgICAg'
+    b'ICA8c3RFdnQ6YWN0aW9uPnNhdmVkPC9zdEV2dDphY3Rpb24+CiAgICAgICAgICAgICAgIDwv'
+    b'cmRmOmxpPgogICAgICAgICAgICA8L3JkZjpTZXE+CiAgICAgICAgIDwveG1wTU06SGlzdG9y'
+    b'eT4KICAgICAgICAgPHhtcE1NOkRvY3VtZW50SUQ+Z2ltcDpkb2NpZDpnaW1wOmQ4YWNlZDE3'
+    b'LTM2YzMtNDE1My04MDQ0LTNhOTRmYTkwNTNiOTwveG1wTU06RG9jdW1lbnRJRD4KICAgICAg'
+    b'ICAgPHhtcE1NOkluc3RhbmNlSUQ+eG1wLmlpZDplOGUzMTkyYi0yZTZiLTQzYmMtYjQ1Zi05'
+    b'MDVhNzM2Njk0ODA8L3htcE1NOkluc3RhbmNlSUQ+CiAgICAgICAgIDx0aWZmOlJlc29sdXRp'
+    b'b25Vbml0PjM8L3RpZmY6UmVzb2x1dGlvblVuaXQ+CiAgICAgICAgIDx0aWZmOk9yaWVudGF0'
+    b'aW9uPjE8L3RpZmY6T3JpZW50YXRpb24+CiAgICAgICAgIDx0aWZmOlhSZXNvbHV0aW9uPjk2'
+    b'PC90aWZmOlhSZXNvbHV0aW9uPgogICAgICAgICA8dGlmZjpZUmVzb2x1dGlvbj45NjwvdGlm'
+    b'ZjpZUmVzb2x1dGlvbj4KICAgICAgPC9yZGY6RGVzY3JpcHRpb24+CiAgIDwvcmRmOlJERj4K'
+    b'PC94OnhtcG1ldGE+CnxoxFYAAAJOSURBVEgNtZaxTxRREMZXBFQq7AgkhBBI1JbmIhUJPdCc'
+    b'FVbnvyC1tdZY2NwdCfwNFtIQOyP/AYHOjkaMNuD3230fmbtbFr3sTvLtvDdv3nxv3s7sXZaN'
+    b'ygOZHgbzpMYTYV77EMJhwTY1bKxj7kzWFawvdAXGlkca2Me2sbUzaCnCb+Em4IPGTwWE67Zv'
+    b'bhjnEa9sXwEgawtrwmman0nvCJZpD8bREFIcCFcJ4RwTCdm8FZzxkcYLgiUWmG336kjYlTfB'
+    b'V4d2PdP8S1q7kn4T1iH9r3cbCXsp6HIKSOYxi47mP5PPsTQHsfxzC1UR+uS8M6oUmRcOBV/z'
+    b'nsZ+JfjfW1RVhKzdFWBbaxQTxN+Fl4KFw7G3VKoII9lz7Z5NEZwR7fJecLa0kH3ItpS0ilB7'
+    b'siXhs0B/ktErAXlSqPxJdmQJ8YVA9gixwYBg8Il7GrNpJXkQ9GuyOQv0Rlh3QDKKLfQ6+cRb'
+    b'yk1VhJvygIDs/gi/0vyjNMJB435sVO618I1JkrzSXYE2lml6DnGFukUuC/OdT2dd6hBP2JNH'
+    b'vFI2fEo2X+kPzRdZkMRqHL7S3cJltMrLCJeTs4O+0+BEOBBeYJTMFCp/xqI5l2UrrREbDEgV'
+    b'oYtpYIMmLoTa24LD8N787h4HZn49aBOuurbGd2GRqUkb/bRFInFmHaHWj3dXAbmiVSEKvdXI'
+    b'z1NfgSFs/AfYVbefCNvSjf3FUOzbMm9pzCfMTY6u/U+UYubiiqSJe0JXaOxvomLnMvJVkBWb'
+    b'r7zwqvHpRndI2sKZ2za2/gt+0YIMN1o1aQAAAABJRU5ErkJggg==')
```

### Comparing `cardstock-0.99.2/cardstock/errorListWindow.py` & `cardstock-0.99.3/cardstock/errorListWindow.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# This file is part of CardStock.
+#     https://github.com/benjie-git/CardStock
+#
+# Copyright Ben Levitt 2020-2023
+#
+# This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
+# of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
+
 import wx
 import wx.html
 
 
 class CardStockError(object):
     def __init__(self, card, obj, handlerName, lineNum, msg):
         self.card = card
```

### Comparing `cardstock-0.99.2/cardstock/examples/Asteroids.cds` & `cardstock-0.99.3/cardstock/examples/Asteroids.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.2/cardstock/examples/Browser.cds` & `cardstock-0.99.3/cardstock/examples/Browser.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.2/cardstock/examples/Calculator.cds` & `cardstock-0.99.3/cardstock/examples/Calculator.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.2/cardstock/examples/Catch.cds` & `cardstock-0.99.3/cardstock/examples/Catch.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.2/cardstock/examples/Diary.cds` & `cardstock-0.99.3/cardstock/examples/Diary.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.2/cardstock/examples/Dice-stats.cds` & `cardstock-0.99.3/cardstock/examples/Dice-stats.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.2/cardstock/examples/Dice.cds` & `cardstock-0.99.3/cardstock/examples/Dice.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.2/cardstock/examples/Factor.cds` & `cardstock-0.99.3/cardstock/examples/Factor.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.2/cardstock/examples/Fifteen.cds` & `cardstock-0.99.3/cardstock/examples/Fifteen.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.2/cardstock/examples/Flappy.cds` & `cardstock-0.99.3/cardstock/examples/Flappy.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.2/cardstock/examples/Graph.cds` & `cardstock-0.99.3/cardstock/examples/Graph.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.2/cardstock/examples/Guess.cds` & `cardstock-0.99.3/cardstock/examples/Guess.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.2/cardstock/examples/Hanoi.cds` & `cardstock-0.99.3/cardstock/examples/Hanoi.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.2/cardstock/examples/Logo.cds` & `cardstock-0.99.3/cardstock/examples/Logo.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.2/cardstock/examples/Magic.cds` & `cardstock-0.99.3/cardstock/examples/Magic.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.2/cardstock/examples/Mastermind.cds` & `cardstock-0.99.3/cardstock/examples/Mastermind.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.2/cardstock/examples/Maze.cds` & `cardstock-0.99.3/cardstock/examples/Maze.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.2/cardstock/examples/Morph.cds` & `cardstock-0.99.3/cardstock/examples/Morph.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.2/cardstock/examples/Navigation.cds` & `cardstock-0.99.3/cardstock/examples/Navigation.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.2/cardstock/examples/Number-puzzle.cds` & `cardstock-0.99.3/cardstock/examples/Number-puzzle.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.2/cardstock/examples/Pong.cds` & `cardstock-0.99.3/cardstock/examples/Pong.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.2/cardstock/examples/Requests.cds` & `cardstock-0.99.3/cardstock/examples/Requests.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.2/cardstock/examples/Scene.cds` & `cardstock-0.99.3/cardstock/examples/Scene.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.2/cardstock/examples/Serial.cds` & `cardstock-0.99.3/cardstock/examples/Serial.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.2/cardstock/examples/Snake.cds` & `cardstock-0.99.3/cardstock/examples/Snake.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.2/cardstock/examples/Tanks.cds` & `cardstock-0.99.3/cardstock/examples/Tanks.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.2/cardstock/examples/TicTacToe.cds` & `cardstock-0.99.3/cardstock/examples/TicTacToe.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.2/cardstock/examples/Welcome.cds` & `cardstock-0.99.3/cardstock/examples/Welcome.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.2/cardstock/examples/Wordel.cds` & `cardstock-0.99.3/cardstock/examples/Wordel.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.2/cardstock/examples/click.wav` & `cardstock-0.99.3/cardstock/examples/click.wav`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.2/cardstock/examples/puff.wav` & `cardstock-0.99.3/cardstock/examples/puff.wav`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.2/cardstock/examples/ship-off.png` & `cardstock-0.99.3/cardstock/examples/ship-off.png`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.2/cardstock/examples/ship-on.png` & `cardstock-0.99.3/cardstock/examples/ship-on.png`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.2/cardstock/examples/simple-red-apple.png` & `cardstock-0.99.3/cardstock/examples/simple-red-apple.png`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.2/cardstock/examples/yay.wav` & `cardstock-0.99.3/cardstock/examples/yay.wav`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.2/cardstock/findEngineDesigner.py` & `cardstock-0.99.3/cardstock/findEngineDesigner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# This file is part of CardStock.
+#     https://github.com/benjie-git/CardStock
+#
+# Copyright Ben Levitt 2020-2023
+#
+# This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
+# of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
+
 import wx
 import stackManager
 from uiView import ViewModel
 from appCommands import SetPropertyCommand, SetHandlerCommand, CommandGroup
 import re
 
 SEARCHABLE_PROPERTIES = ["name", "text", "title", "file", "text_color", "pen_color", "fill_color"]
```

### Comparing `cardstock-0.99.2/cardstock/findEngineViewer.py` & `cardstock-0.99.3/cardstock/findEngineViewer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# This file is part of CardStock.
+#     https://github.com/benjie-git/CardStock
+#
+# Copyright Ben Levitt 2020-2023
+#
+# This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
+# of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
+
 import wx
 import stackManager
 from uiView import ViewModel
 from appCommands import SetPropertyCommand, CommandGroup
 import re
 
 """
```

### Comparing `cardstock-0.99.2/cardstock/flippedGCDC.py` & `cardstock-0.99.3/cardstock/flippedGCDC.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# This file is part of CardStock.
+#     https://github.com/benjie-git/CardStock
+#
+# Copyright Ben Levitt 2020-2023
+#
+# This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
+# of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
+
 import wx
 
 class FlippedGCDC(wx.GCDC):
     """
     Vertically flip the output to the stack view, so the origin is the bottom-left corner.
     """
     def __init__(self, dc, stackManager, **kwargs):
```

### Comparing `cardstock-0.99.2/cardstock/generator.py` & `cardstock-0.99.3/cardstock/generator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# This file is part of CardStock.
+#     https://github.com/benjie-git/CardStock
+#
+# Copyright Ben Levitt 2020-2023
+#
+# This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
+# of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
+
 import wx
 import uiButton
 import uiTextField
 import uiTextLabel
 import uiImage
 import uiWebView
 import uiShape
```

### Comparing `cardstock-0.99.2/cardstock/helpData.py` & `cardstock-0.99.3/cardstock/helpData.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# This file is part of CardStock.
+#     https://github.com/benjie-git/CardStock
+#
+# Copyright Ben Levitt 2020-2023
+#
+# This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
+# of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
+
 import uiView
 import keyword
 
 """
 This file includes descriptions of all CardStock objects, properties, methods, and event handlers for use in
 context help, reference docs, and in the future, code completion.
 """
@@ -545,23 +553,25 @@
                          "currently, all text fields and web views will be displayed in front of other objects."},
         "order_to_index": {"args": {"toIndex": {"type": "int", "info": "The index to move this object to, in the list of "
                                  "the card or group's children.  Index 0 is at the back."}},
                        "return": None,
                          "info": "Moves this object to the given index, in the list of "
                                  "its parent's children, with 0 being at the back.  But note that "
                          "currently, all text fields and web views will be displayed in front of other objects."},
-        "get_event_code": {"args": {"eventName": {"type": "string", "info": "The name of the event to look up."}},
+        "get_code_for_event": {"args": {"eventName": {"type": "string", "info": "The name of the event to look up."}},
                             "return": "string",
                             "info": "Returns a string containing this object's event code for the given "
-                                    "<b>eventName</b>"},
-        "set_event_code": {"args": {"eventName": {"type": "string", "info": "The name of the event to set."},
+                                    "<b>eventName</b>.  For example, button_1.get_code_for_event('on_click') will "
+                                    "return the code in the object named button_1 for the 'on_click' event."},
+        "set_code_for_event": {"args": {"eventName": {"type": "string", "info": "The name of the event to set."},
                                      "code": {"type": "string", "info": "The code to run on this event."}},
                             "return": None,
-                            "info": "Sets this object's event code for the given <b>eventName</b> to"
-                                    "<b>code</b>."},
+                            "info": "Sets the <b>code</b> to be run when the event named <b>eventName</b> triggers for this object.  "
+                                    "For example, button_1.set_code_for_event('on_click', 'alert(\"Hello\")') will set up "
+                                    "button_1 to show an alert when clicked."},
         "stop_handling_mouse_event": {"args": {},
                                    "return": None,
                                    "info": "If you call this method from your event code for any on_mouse_press(), on_mouse_move(), "
                                            "or on_mouse_release() event, CardStock will skip running code for this event "
                                            "for any overlapping objects underneath this object, which would otherwise "
                                            "be run immediately after this object's event code finishes.  Calling "
                                            "this method from any non-mouse event code does nothing.  Should be run as self.stop_handling_mouse_event()."},
@@ -692,15 +702,15 @@
     parent = HelpDataObject
     types = ["button"]
 
     properties = {
         "title": {"type": "string",
                   "info": "The <b>title</b> property is the visible text on the button."},
         "style": {"type": "[Border, Borderless, Checkbox, Radio]",
-                   "info": "Buttons with style <b>Border</b> show a rectangular or rounded border, "
+                   "info": "Buttons with style <b>Border</b> show a rounded rectangular border, "
                            "depending on your computer's operating system.  This is the most commonly seen style of "
                            "button.  The <b>Borderless</b> style behaves the same, but is drawn without a border."
                            "You can also set style to be <b>Checkbox</b>, which allows users to alternately select and "
                            "deselect this button, and it is drawn with a checkbox to show the selection state.  "
                            "You can set the style to <b>Radio</b>, which allows selecting only one button at a time from a "
                            "group of Radio buttons, and is drawn with a round selection indicator.  All <b>Radio</b> "
                            "buttons with the same immediate parent (the Card, or a Group) are considered to be in the "
@@ -1094,15 +1104,15 @@
         "add_text_field": {"args": {"name": {"type": "string", "info": "an optional argument giving the name to use for this "
                                                                 "new Text Field object.  If omitted, the name will be "
                                                                 "'field_{N}'."},
                                   "...": {"info": "optionally set more properties here.  For example, "
                                                                  "include position=(10,10)"}},
                     "return": "textfield",
                     "info": "Adds a new Text Field to the card, and returns the new object."},
-        "add_text_tabel": {"args": {"name": {"type": "string", "info": "an optional argument giving the name to use for this "
+        "add_text_label": {"args": {"name": {"type": "string", "info": "an optional argument giving the name to use for this "
                                                                 "new Text Label object.  If omitted, the name will be "
                                                                 "'label_{N}'."},
                                   "...": {"info": "optionally set more properties here.  For example, "
                                                                  "include position=(10,10)"}},
                          "return": "textlabel",
                     "info": "Adds a new Text Label object to the card, and returns the new object."},
         "add_image": {"args": {"name": {"type": "string", "info": "an optional argument giving the name to use for this "
```

### Comparing `cardstock-0.99.2/cardstock/helpDialogs.py` & `cardstock-0.99.3/cardstock/helpDialogs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,23 @@
+# This file is part of CardStock.
+#     https://github.com/benjie-git/CardStock
+#
+# Copyright Ben Levitt 2020-2023
+#
+# This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
+# of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
+
 import wx
 import wx.html
 import version
 import platform
 from helpData import HelpData, HelpDataTypes
 
+OUTPUT_HTML = False
+
 
 class CardStockAbout(wx.Dialog):
     """ An about box that uses an HTML view. """
 
     def GetHTML(self):
         return f'''
 <html>
@@ -50,86 +60,14 @@
     def OnKeyDown(self, event):
         code = event.GetKeyCode()
         if code == wx.WXK_ESCAPE or (code == ord("W") and event.ControlDown()):
             self.Close()
         event.Skip()
 
 
-class CardStockBasics(wx.Frame):
-    """ A help window that uses an HTML view.  This is the Python Basics window. """
-
-    def GetHTML(self):
-        hints = {
-            "Basic types":'int: 5, 1000, -2\nfloat: 3.1415, 1000.0, 0.5\nstring: "Hello", "CardStock", "100 is a number"\nlist: [1,1,2,3,5], ["Bob", "Jane", "Gandalf"]\nobject: oval_1, card, stack, label_1',
-            "Convert types":'int("100") == 100\nstr(57) == "57"\nint(12.5) == 12',
-            "Get a property of an object": 'oval_1.fill_color\nlabel_1.text',
-            "Expressions": '4 + 7\n"Hello" + " friend"\nlabel_1.text + " BEEP"\nint(field_1.text) + 1\nstr(age) + " years old"',
-            "Set a value":'x = 2\noval_1.fill_color = "red"\nlabel_1.text = "Hello friend"',
-            "Change a value": 'x = x + 1, x += 1\nfield_1.text = int(field_1.text) + 1\nfield_1.text += ", and this"',
-            "Check a value": 'if x == 3:\n   alert("x is three!")\n\nif field_1.text == "Hello friend":\n   print("Enter")\nelse:\n   print("Nope")\n\n'
-                             'if key_name == "Right":\n   oval.position.x += 10\nelif key_name == "Left":\n   oval.position.x -= 10\nelse:\n   print("Why\'d you press " + key_name)',
-            "Make a list": 'odds = [1, 3, 5, 7, 9]\nprint([2, 4, 6])\nnames = ["Jonas", "Martha", "Magnus"]\novals = [oval_1, oval_2, oval_3]',
-            "Do something for each item in a list": 'for num in odds:\n   print(num)\n\nfor oval in ovals:\n   oval.fill_color = "red"',
-            "Do something a set number of times": 'for i in range(10):\n   print(i)',
-        }
-        html = f'''
-<html>
-<body bgcolor="#EEEEEE">
-<center><table cellspacing="0" cellpadding="4" border="0">
-<tr>
-    <td align="center"><h1>CardStock: Python Basics</h1>
-    </td>
-</tr>
-</table>
-</center>
-<table border='0' cellpadding='5' cellspacing='0'>
-'''
-        bgcolors = [" bgcolor='#D0DFEE'", " bgcolor='#CCCCCC'"]
-        bg = bgcolors[0]
-        for title,content in hints.items():
-            bg = bgcolors[0 if bg==bgcolors[1] else 1]
-            html += f"""
-    <tr><th align='left' valign='top'{bg}>{title}</th>
-    <td align='left' valign='top'{bg}><pre>{content}</pre></td></tr>
-        """
-
-        html += '''
-</table>
-</body>
-</html>
-'''
-        return html
-
-    def __init__(self, parent):
-        super().__init__(parent, -1, 'CardStock: Python Basics', size=(parent.FromDIP(800), parent.FromDIP(600)))
-
-        html = wx.html.HtmlWindow(self, -1)
-        htmlStr = self.GetHTML()
-        # f = open("manual.html","w")
-        # f.write(htmlStr)
-        # f.close()
-        html.SetPage(htmlStr)
-        html.Bind(wx.EVT_KEY_DOWN, self.OnKeyDown)
-
-        # Set up the layout with a Sizer
-        sizer = wx.BoxSizer(wx.VERTICAL)
-        sizer.Add(html, wx.SizerFlags(1).Expand().Border(wx.ALL, 5))
-        self.SetSizer(sizer)
-        self.Layout()
-
-        self.CentreOnParent(wx.BOTH)
-
-
-    def OnKeyDown(self, event):
-        code = event.GetKeyCode()
-        if code == wx.WXK_ESCAPE or (code == ord("W") and event.ControlDown()):
-            self.Close()
-        event.Skip()
-
-
 class CardStockManual(wx.Frame):
     """ A help window that uses an HTML view.  This is the manual, which explains how to use CardStock. """
 
     def GetHTML(self):
         return f'''
 <html>
 <body bgcolor="#EEEEEE">
@@ -410,17 +348,18 @@
 '''
 
     def __init__(self, parent):
         super().__init__(parent, -1, 'CardStock Manual', size=(parent.FromDIP(800), parent.FromDIP(600)))
 
         html = wx.html.HtmlWindow(self, -1)
         htmlStr = self.GetHTML()
-        # f = open("manual.html","w")
-        # f.write(htmlStr)
-        # f.close()
+        if OUTPUT_HTML:
+            f = open("manual.html","w")
+            f.write(htmlStr)
+            f.close()
         html.SetPage(htmlStr)
         html.Bind(wx.EVT_KEY_DOWN, self.OnKeyDown)
 
         # Set up the layout with a Sizer
         sizer = wx.BoxSizer(wx.VERTICAL)
         sizer.Add(html, wx.SizerFlags(1).Expand().Border(wx.ALL, 5))
         self.SetSizer(sizer)
@@ -576,17 +515,18 @@
         super().__init__(parent, -1, 'CardStock Reference',
                           size=(parent.FromDIP(900), parent.FromDIP(950)))
 
         self.splitter = wx.SplitterWindow(self, style=wx.SP_3DSASH | wx.SP_LIVE_UPDATE)
 
         self.html = wx.html.HtmlWindow(self.splitter, -1)
         htmlStr = self.GetHTML()
-        # f = open("reference.html","w")
-        # f.write(htmlStr)
-        # f.close()
+        if OUTPUT_HTML:
+            f = open("reference.html","w")
+            f.write(htmlStr)
+            f.close()
         self.html.SetPage(htmlStr)
         self.html.Bind(wx.EVT_KEY_DOWN, self.OnKeyDown)
 
         toc = wx.html.HtmlWindow(self.splitter)
         toc.SetPage(HelpData.TOCPage())
         toc.Bind(wx.html.EVT_HTML_LINK_CLICKED, self.TOCLinkClicked)
         toc.Bind(wx.EVT_KEY_DOWN, self.OnKeyDown)
```

### Comparing `cardstock-0.99.2/cardstock/mediaSearchDialogs.py` & `cardstock-0.99.3/cardstock/mediaSearchDialogs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# This file is part of CardStock.
+#     https://github.com/benjie-git/CardStock
+#
+# Copyright Ben Levitt 2020-2023
+#
+# This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
+# of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
+
 import wx
 import wx.html2
 import requests
 import os
 import uiImage
 
 '''
```

### Comparing `cardstock-0.99.2/cardstock/migrations.py` & `cardstock-0.99.3/cardstock/migrations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# This file is part of CardStock.
+#     https://github.com/benjie-git/CardStock
+#
+# Copyright Ben Levitt 2020-2023
+#
+# This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
+# of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
+
 # Allow migrating older file formats to newer ones
 
 import re
 
 def MigrateDataFromFormatVersion(fromVer, dataDict):
     # Migration code to run on json before loading it into models
 
@@ -341,7 +349,23 @@
                     val = re.sub(r"\bHide\b", "hide", val)
                     val = re.sub(r"\bEnter\b", "enter", val)
                     val = re.sub(r"\bClick\b", "click", val)
                     obj.handlers[k] = val
             for child in obj.childModels:
                 replaceNames(child)
         replaceNames(stackModel)
+
+    if fromVer <= 6:
+        """
+        In File Format Version 7, get and set event_code functions were renamed
+        """
+        # Update names of StopAnimating methods, OnIdle->OnPeriodic
+        def replaceNames(obj):
+            for k ,v in obj.handlers.items():
+                if len(v):
+                    val = v
+                    val = val.replace(".get_event_code(", ".get_code_for_event(")
+                    val = val.replace(".set_event_code(", ".set_code_for_event(")
+                    obj.handlers[k] = val
+            for child in obj.childModels:
+                replaceNames(child)
+        replaceNames(stackModel)
```

### Comparing `cardstock-0.99.2/cardstock/propertyInspector.py` & `cardstock-0.99.3/cardstock/propertyInspector.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# This file is part of CardStock.
+#     https://github.com/benjie-git/CardStock
+#
+# Copyright Ben Levitt 2020-2023
+#
+# This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
+# of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
+
 import wx
 import wx.grid
 from uiView import ViewModel, ViewProxy
 from simpleListBox import SimpleListBox
 import mediaSearchDialogs
 from appCommands import SetPropertyCommand
 import os
```

### Comparing `cardstock-0.99.2/cardstock/pythonEditor.py` & `cardstock-0.99.3/cardstock/pythonEditor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# This file is part of CardStock.
+#     https://github.com/benjie-git/CardStock
+#
+# Copyright Ben Levitt 2020-2023
+#
+# This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
+# of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
+
 import wx
 import wx.stc as stc
 import keyword
 import helpData
 
 """
 The PythonEditor is used for the CodeEditor in the Designer's ControlPanel.
```

### Comparing `cardstock-0.99.2/cardstock/runner.py` & `cardstock-0.99.3/cardstock/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# This file is part of CardStock.
+#     https://github.com/benjie-git/CardStock
+#
+# Copyright Ben Levitt 2020-2023
+#
+# This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
+# of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
+
 import re
 import sys
 import os
 import traceback
 import wx
 import uiView
 import types
@@ -137,14 +145,15 @@
             wx.WXK_BACK: "Backspace",
             wx.WXK_CAPITAL: "CapsLock"
         }
         if wx.GetOsVersion()[0] == wx.OS_MAC_OSX_DARWIN:
             self.keyCodeStringMap[wx.WXK_ALT] = "Option"
             self.keyCodeStringMap[wx.WXK_CONTROL] = "Command"
             self.keyCodeStringMap[wx.WXK_RAW_CONTROL] = "Control"
+        self.keyCodeStringReverseMap = None
 
     def AddSyntaxErrors(self, analyzerSyntaxErrors):
         for path, e in analyzerSyntaxErrors.items():
             parts = path.split('.')
             modelPath = '.'.join(path.split('.')[:-1])
             model = self.stackManager.stackModel.GetModelFromPath(modelPath)
             handlerName = parts[-1]
@@ -726,14 +735,22 @@
         code = event.GetKeyCode()
         if code in self.keyCodeStringMap:
             return self.keyCodeStringMap[code]
         elif event.GetUnicodeKey() != wx.WXK_NONE:
             return chr(event.GetUnicodeKey())
         return None
 
+    def KeyCodeForName(self, name):
+        if not self.keyCodeStringReverseMap:
+            self.keyCodeStringReverseMap = {value:key for key,value in self.keyCodeStringMap.items()}
+        if name in self.keyCodeStringReverseMap:
+            return self.keyCodeStringReverseMap[name]
+        else:
+            return ord(name)
+
     def OnKeyDown(self, event):
         key_name = self.KeyNameForEvent(event)
         if key_name and key_name not in self.pressedKeys:
             self.pressedKeys.append(key_name)
             self.keyTimings[key_name] = time()
             return True
         return False
@@ -761,14 +778,21 @@
             vars.pop(v)
         if '__builtins__' in vars:
             vars.pop('__builtins__')
         if '__warningregistry__' in vars:
             vars.pop('__warningregistry__')
         return vars
 
+    def EnqueueSyncPressedKeys(self):
+        for name in self.pressedKeys:
+            e = wx.KeyEvent()
+            code = self.KeyCodeForName(name)
+            e.SetKeyCode(code)
+            self.stackManager.uiCard.OnKeyUp(e)
+
     @RunOnMainAsync
     def SetFocus(self, obj):
         if obj:
             uiView = self.stackManager.GetUiViewByModel(obj._model)
             if uiView:
                 if uiView.model.type == "textfield":
                     sel = uiView.view.GetSelection()
@@ -783,15 +807,16 @@
 
     def broadcast_message(self, message):
         if not isinstance(message, str):
             raise TypeError("broadcast_message(): message must be a string")
 
         self.RunHandler(self.stackManager.uiCard.model, "on_message", None, message)
         for ui in self.stackManager.uiCard.GetAllUiViews():
-            self.RunHandler(ui.model, "on_message", None, message)
+            if not ui.model.didDelete:
+                self.RunHandler(ui.model, "on_message", None, message)
 
     def goto_card(self, card):
         index = None
         if isinstance(card, str):
             cardName = card
         elif isinstance(card, Card):
             cardName = card._model.GetProperty("name")
@@ -876,24 +901,27 @@
     def alert(self, message):
         if self.stopRunnerThread or self.generatingThumbnail:
             return
 
         @RunOnMainSync
         def func():
             wx.MessageDialog(None, str(message), "", wx.OK).ShowModal()
+
+        self.EnqueueSyncPressedKeys()
         func()
 
     def ask_yes_no(self, message):
         if self.stopRunnerThread or self.generatingThumbnail:
             return None
 
         @RunOnMainSync
         def func():
             return wx.MessageDialog(None, str(message), "", wx.YES_NO).ShowModal() == wx.ID_YES
 
+        self.EnqueueSyncPressedKeys()
         return func()
 
     def ask_text(self, message, defaultResponse=None):
         if self.stopRunnerThread or self.generatingThumbnail:
             return None
 
         @RunOnMainSync
@@ -901,14 +929,15 @@
             dlg = wx.TextEntryDialog(None, str(message), '')
             if defaultResponse is not None:
                 dlg.SetValue(str(defaultResponse))
             if dlg.ShowModal() == wx.ID_OK:
                 return dlg.GetValue()
             return None
 
+        self.EnqueueSyncPressedKeys()
         return func()
 
     def open_url(self, URL, in_place=False):
         if not isinstance(URL, str):
             raise TypeError("open_url(): URL must be a string")
 
         wx.LaunchDefaultBrowser(URL)
```

### Comparing `cardstock-0.99.2/cardstock/simpleListBox.py` & `cardstock-0.99.3/cardstock/simpleListBox.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# This file is part of CardStock.
+#     https://github.com/benjie-git/CardStock
+#
+# Copyright Ben Levitt 2020-2023
+#
+# This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
+# of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
+
 import wx
 LINE_HEIGHT = 20
 
 
 class SimpleListBox(wx.Control):
     def __init__(self, parent, shouldCapture, **kwargs):
         super().__init__(parent, style=wx.WANTS_CHARS, **kwargs)
```

### Comparing `cardstock-0.99.2/cardstock/stackExporter.py` & `cardstock-0.99.3/cardstock/stackExporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# This file is part of CardStock.
+#     https://github.com/benjie-git/CardStock
+#
+# Copyright Ben Levitt 2020-2023
+#
+# This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
+# of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
+
 import requests
 import wx
 import os
 import sys
 import re
 import random
 import json
```

### Comparing `cardstock-0.99.2/cardstock/stackManager.py` & `cardstock-0.99.3/cardstock/stackManager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,14 @@
-#!/usr/bin/python
-# stackManager.py
+# This file is part of CardStock.
+#     https://github.com/benjie-git/CardStock
+#
+# Copyright Ben Levitt 2020-2023
+#
+# This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
+# of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 """
 This module contains the StackManager class which manages painting, editing, and
 interacting with the stack.
 This class is very central to CardStock, and right now, probably contains a bit more than it should.  :)
 """
```

### Comparing `cardstock-0.99.2/cardstock/stackModel.py` & `cardstock-0.99.3/cardstock/stackModel.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,14 @@
-#!/usr/bin/python
+# This file is part of CardStock.
+#     https://github.com/benjie-git/CardStock
+#
+# Copyright Ben Levitt 2020-2023
+#
+# This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
+# of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 import wx
 from uiView import ViewModel, ViewProxy
 from uiCard import CardModel
 import version
 import migrations
 from codeRunnerThread import RunOnMainSync
```

### Comparing `cardstock-0.99.2/cardstock/standalone.py` & `cardstock-0.99.3/cardstock/standalone.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,15 @@
-#!/usr/bin/python3
+# This file is part of CardStock.
+#     https://github.com/benjie-git/CardStock
+#
+# Copyright Ben Levitt 2020-2023
+#
+# This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
+# of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
-# standalone.py
 """
 This is the root of the CardStock exported stack application.
 It loads the embedded stack and ResourceMap, and runs the viewer.
 """
 
 import os
 import sys
```

### Comparing `cardstock-0.99.2/cardstock/tools.py` & `cardstock-0.99.3/cardstock/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# This file is part of CardStock.
+#     https://github.com/benjie-git/CardStock
+#
+# Copyright Ben Levitt 2020-2023
+#
+# This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
+# of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
+
 import wx
 
 import generator
 from appCommands import *
 from uiShape import UiShape, ShapeModel
 import math
```

### Comparing `cardstock-0.99.2/cardstock/uiButton.py` & `cardstock-0.99.3/cardstock/uiButton.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# This file is part of CardStock.
+#     https://github.com/benjie-git/CardStock
+#
+# Copyright Ben Levitt 2020-2023
+#
+# This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
+# of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
+
 import wx
 from uiView import *
 from embeddedImages import radio_on, radio_off, checkbox_on, checkbox_off
 from uiTextLabel import wordwrap
 
 # Native Button Mouse event positions on Mac are offset (?!?)
 MAC_BUTTON_OFFSET_HACK = wx.Point(6,4)
```

### Comparing `cardstock-0.99.2/cardstock/uiCard.py` & `cardstock-0.99.3/cardstock/uiCard.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# This file is part of CardStock.
+#     https://github.com/benjie-git/CardStock
+#
+# Copyright Ben Levitt 2020-2023
+#
+# This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
+# of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
+
 import wx
 from uiView import *
 import uiShape
 import generator
 from codeRunnerThread import RunOnMainSync, RunOnMainAsync
```

### Comparing `cardstock-0.99.2/cardstock/uiGroup.py` & `cardstock-0.99.3/cardstock/uiGroup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# This file is part of CardStock.
+#     https://github.com/benjie-git/CardStock
+#
+# Copyright Ben Levitt 2020-2023
+#
+# This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
+# of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
+
 import wx
 from uiView import *
 import generator
 from codeRunnerThread import RunOnMainSync
 
 
 class UiGroup(UiView):
```

### Comparing `cardstock-0.99.2/cardstock/uiImage.py` & `cardstock-0.99.3/cardstock/uiImage.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# This file is part of CardStock.
+#     https://github.com/benjie-git/CardStock
+#
+# Copyright Ben Levitt 2020-2023
+#
+# This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
+# of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
+
 import os
 import wx
 import generator
 from uiView import *
 
 
 class UiImage(UiView):
```

### Comparing `cardstock-0.99.2/cardstock/uiShape.py` & `cardstock-0.99.3/cardstock/uiShape.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# This file is part of CardStock.
+#     https://github.com/benjie-git/CardStock
+#
+# Copyright Ben Levitt 2020-2023
+#
+# This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
+# of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
+
 import wx
 from uiView import *
 from imageFactory import ImageFactory
 
 
 class UiShape(UiView):
     """
```

### Comparing `cardstock-0.99.2/cardstock/uiTextBase.py` & `cardstock-0.99.3/cardstock/uiTextBase.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# This file is part of CardStock.
+#     https://github.com/benjie-git/CardStock
+#
+# Copyright Ben Levitt 2020-2023
+#
+# This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
+# of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
+
 import wx
 import wx.stc as stc
 from uiView import *
 
 
 class UiTextBase(UiView):
     """
```

### Comparing `cardstock-0.99.2/cardstock/uiTextField.py` & `cardstock-0.99.3/cardstock/uiTextField.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# This file is part of CardStock.
+#     https://github.com/benjie-git/CardStock
+#
+# Copyright Ben Levitt 2020-2023
+#
+# This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
+# of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
+
 import wx
 from uiView import *
 from appCommands import SetPropertyCommand
 from uiTextBase import *
 import wx.stc as stc
 from wx.lib.docview import CommandProcessor, Command
```

### Comparing `cardstock-0.99.2/cardstock/uiTextLabel.py` & `cardstock-0.99.3/cardstock/uiTextLabel.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# This file is part of CardStock.
+#     https://github.com/benjie-git/CardStock
+#
+# Copyright Ben Levitt 2020-2023
+#
+# This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
+# of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
+
 import wx
 from appCommands import SetPropertyCommand
 from uiView import *
 from uiTextBase import *
 from uiTextField import CDSTextCtrl
```

### Comparing `cardstock-0.99.2/cardstock/uiView.py` & `cardstock-0.99.3/cardstock/uiView.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,14 @@
-import threading
+# This file is part of CardStock.
+#     https://github.com/benjie-git/CardStock
+#
+# Copyright Ben Levitt 2020-2023
+#
+# This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
+# of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 import wx
 import threading
 import ast
 import re
 import generator
 import helpData
@@ -663,14 +669,15 @@
         self.proxy = None
         self.lastOnPeriodicTime = None
         self.animations = {}
         self.bounceObjs = {}
         self.proxyClass = ViewProxy
         self.animLock = threading.Lock()
         self.didSetDown = False
+        self.didDelete = False
         self.clonedFrom = None
 
     def __repr__(self):
         return f"<{self.GetDisplayType()}:'{self.GetProperty('name')}'>"
 
     def SetBackUp(self, stackManager):
         if self.didSetDown:
@@ -745,15 +752,18 @@
             if card.GetDirty():
                 return True
         return False
 
     def CanRotate(self):
         return ("rotation" in self.properties)
 
-    def GetPath(self):
+    def GetPath(self, subName=None):
+        parts = []
+        if subName:
+            parts.append(subName)
         parts = []
         m = self
         while m.parent:
             parts.append(m.GetProperty("name"))
             m = m.parent
         return ".".join(reversed(parts))
 
@@ -1246,15 +1256,15 @@
     def send_message(self, message):
         if not isinstance(message, str):
             raise TypeError("send_message(): message must be a string")
 
         model = self._model
         if not model: return
 
-        if not model.stackManager.isEditing and model.stackManager.runner:
+        if not model.stackManager.isEditing and model.stackManager.runner and not model.didDelete:
            model.stackManager.runner.RunHandler(model, "on_message", None, message)
 
     def clone(self, name=None, **kwargs):
         model = self._model
         if not model: return None
 
         if model.type != "card":
@@ -1302,17 +1312,18 @@
                 return newModel
             newModel = func()
 
         return newModel.GetProxy()
 
     def delete(self):
         model = self._model
-        if not model or not model.parent or model.parent.type == "group":
+        if not model or not model.parent or model.parent.type == "group" or model.didDelete:
             return
 
+        model.didDelete = True
         # immediately update the model
         sm = model.stackManager
         if model.type != "card":
             model.parent.RemoveChild(model)
 
         if model.type != "card":
             @RunOnMainAsync
@@ -1525,28 +1536,28 @@
             raise TypeError("object does not support rotation")
         if not isinstance(val, (int, float)):
             raise TypeError("rotation must be a number")
         model = self._model
         if not model: return
         model.SetProperty("rotation", val)
 
-    def get_event_code(self, eventName):
+    def get_code_for_event(self, eventName):
         model = self._model
         if not model: return ""
         return model.handlers[eventName]
 
-    def set_event_code(self, eventName, code):
+    def set_code_for_event(self, eventName, code):
         model = self._model
         if not model: return
         if not isinstance(eventName, str):
-            raise TypeError("set_event_code(): eventName must be a string")
+            raise TypeError("set_code_for_event(): eventName must be a string")
         if not isinstance(code, str):
-            raise TypeError("set_event_code(): code must be a string")
+            raise TypeError("set_code_for_event(): code must be a string")
         if eventName not in model.handlers:
-            raise TypeError(f"set_event_code(): this object has no event called '{eventName}'")
+            raise TypeError(f"set_code_for_event(): this object has no event called '{eventName}'")
 
         model.handlers[eventName] = code
 
     def set_bounce_objects(self, objects):
         if not isinstance(objects, (list, tuple)):
             raise TypeError("set_bounce_objects(): objects needs to be a list of cardstock objects")
         models = [o._model for o in objects if isinstance(o, ViewProxy)]
```

### Comparing `cardstock-0.99.2/cardstock/uiWebView.py` & `cardstock-0.99.3/cardstock/uiWebView.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# This file is part of CardStock.
+#     https://github.com/benjie-git/CardStock
+#
+# Copyright Ben Levitt 2020-2023
+#
+# This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
+# of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
+
 import wx
 from uiView import *
 from urllib.parse import urlparse
 import wx.html2
 
 
 class UiWebView(UiView):
```

### Comparing `cardstock-0.99.2/cardstock/variablesWindow.py` & `cardstock-0.99.3/cardstock/variablesWindow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# This file is part of CardStock.
+#     https://github.com/benjie-git/CardStock
+#
+# Copyright Ben Levitt 2020-2023
+#
+# This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
+# of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
+
 import wx
 import wx.grid
 import propertyInspector
 import uiView
 
 
 class VariablesWindow(wx.Frame):
```

### Comparing `cardstock-0.99.2/cardstock/viewer.py` & `cardstock-0.99.3/cardstock/viewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 #!/usr/bin/python3
+# This file is part of CardStock.
+#     https://github.com/benjie-git/CardStock
+#
+# Copyright Ben Levitt 2020-2023
+#
+# This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
+# of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
-# viewer.py
 """
 This is the root frame of the CardStock stack viewer application.  It also is used to run stacks from within
 the designer, and is used to run the stack from a standalone, exported app as well.
 It allows running and using a stack, and even saving its updated state, if the stack has its can_save flag set to True.
 
 Another thing to note is that this class manages the nesting of stacks when calling run_stack() and return_from_stack().
 The list stackStack is a stack of cardstock stacks, and keeps the runner, stackModel, filename, and current cardIndex
```

### Comparing `cardstock-0.99.2/cardstock.egg-info/PKG-INFO` & `cardstock-0.99.3/cardstock.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardstock
-Version: 0.99.2
+Version: 0.99.3
 Summary: A simple development and rapid prototyping tool for quickly building multi-platform desktop programs.
 Home-page: https://github.com/benjie-git/CardStock/wiki
 Author: Ben Levitt
 Author-email: benjie@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
@@ -29,15 +29,15 @@
 ## Features
 
 ### The Basics
 * CardStock lets you design stacks on MacOS, Windows, and GNU/Linux.  You can run CardStock stacks on those platforms, or on any modern web browser, include on Chromebooks and smartphones.
 * You can build programs using objects including text and graphics, images, buttons, text entry fields, and web views.
 * You can use your own python code to manipulate the objects and respond to mouse and keyboard events.
 * You can play sound files from your code.
-* You can search and use clip art in your stacks, thanks to integration with https://openclipart.com.
+* You can search and use clip art in your stacks, thanks to integration with https://openclipart.org.
 * In-context help appears in the app, right where you need it.  And can be turned off when you no longer want it taking up space.
 * All of the creature comforts you've come to expect from a proper application, like full Undo/Redo, and a Find/Replace system that works throughout all of your code and object properties.
 
 ### More Advanced
 * You can animate changes to most properties of objects, to bring your creations to life.
 * Objects can have speed, and can be set up to automatically bounce off of other objects.
 * You can **import** other python modules into your code, and use them make web requests and display the results, control robots, or run machine learning code, all from within your CardStock stack.
@@ -47,14 +47,16 @@
 * View all code used in a whole stack in one place, and click a line to jump to that line in that object's code editor for that event.
 * View recent error messages, and click one to jump to the offending line of code in the Designer.
 * You can export a stack into a standalone application that you can share and distribute, or upload it to the web, on https://cardstock.run.
 
 ### Future Plans
 * Build a web-based design tool to allow creating and editing stacks directly on https://cardstock.run.
 * Add a built-in library of sounds to use, and the ability to record your own sounds.
+* Allow looping sounds, and playing synthesized notes.
+* Add more tutorials for CardStock, and for learning python through CardStock.
 * Allow filling shapes with color gradients.
 * Add app icons for the CardStock Designer and Viewer.
 
 ________
 ## Known Issues
 * TextFields, and WebViews always remain in front of shapes and images, which get drawn directly on the card view.
 * Visual selection indicators (the blue dotted outlines) are drawn behind native views, and so can hide behind overlapping text fields and web views.
@@ -90,9 +92,9 @@
 2. Note that the pre-built Windows app is not yet code-signed, so Windows will complain the first time you open the app. If a window appears saying "Windows protected your PC", click the More Info link at the end of the warning paragraph, and then the "Run Anyway" button that appears at the bottom of the window.
 
 
 ## Reference
 * [CardStock Wiki](https://github.com/benjie-git/CardStock/wiki)
 * [CardStock on Reddit](https://www.reddit.com/r/CardStockPython/)
 * [CardStock Manual](https://github.com/benjie-git/CardStock/wiki/Manual)
-* [CardStock Tutorial](https://github.com/benjie-git/CardStock/wiki/Tutorial)
+* [CardStock Tutorial](https://github.com/benjie-git/CardStock/wiki/Tutorial-Dice)
 * [CardStock Reference Guide](https://github.com/benjie-git/CardStock/wiki/Reference)
```

### Comparing `cardstock-0.99.2/cardstock.egg-info/SOURCES.txt` & `cardstock-0.99.3/cardstock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.2/setup.cfg` & `cardstock-0.99.3/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cardstock
-version = 0.99.2
+version = 0.99.3
 author = Ben Levitt
 author_email = benjie@gmail.com
 description = A simple development and rapid prototyping tool for quickly building multi-platform desktop programs.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/benjie-git/CardStock/wiki
 classifiers =
```

