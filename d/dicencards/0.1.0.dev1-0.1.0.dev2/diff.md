# Comparing `tmp/dicencards-0.1.0.dev1.tar.gz` & `tmp/dicencards-0.1.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicencards-0.1.0.dev1.tar", last modified: Sat May 13 05:21:06 2023, max compression
+gzip compressed data, was "dicencards-0.1.0.dev2.tar", last modified: Mon May 29 10:01:10 2023, max compression
```

## Comparing `dicencards-0.1.0.dev1.tar` & `dicencards-0.1.0.dev2.tar`

### file list

```diff
@@ -1,29 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 05:21:06.719627 dicencards-0.1.0.dev1/
--rw-rw-rw-   0        0        0    11556 2023-01-28 10:07:36.000000 dicencards-0.1.0.dev1/LICENSE.txt
--rw-rw-rw-   0        0        0       60 2023-01-28 10:07:36.000000 dicencards-0.1.0.dev1/MANIFEST.in
--rw-rw-rw-   0        0        0      801 2023-05-13 05:21:06.718629 dicencards-0.1.0.dev1/PKG-INFO
--rw-rw-rw-   0        0        0      180 2023-05-13 05:19:00.000000 dicencards-0.1.0.dev1/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-13 05:21:06.635368 dicencards-0.1.0.dev1/demo/
--rw-rw-rw-   0        0        0      306 2023-04-24 16:27:46.000000 dicencards-0.1.0.dev1/demo/BRP_demo.py
--rw-rw-rw-   0        0        0        0 2023-04-24 16:27:46.000000 dicencards-0.1.0.dev1/demo/__init__.py
--rw-rw-rw-   0        0        0      124 2023-04-24 16:27:46.000000 dicencards-0.1.0.dev1/demo/deadlands_demo.py
-drwxrwxrwx   0        0        0        0 2023-05-13 05:21:06.650237 dicencards-0.1.0.dev1/dicencards/
--rw-rw-rw-   0        0        0        0 2023-04-24 16:27:46.000000 dicencards-0.1.0.dev1/dicencards/__init__.py
--rw-rw-rw-   0        0        0     5355 2023-04-24 16:27:46.000000 dicencards-0.1.0.dev1/dicencards/cards.py
--rw-rw-rw-   0        0        0     1833 2023-04-24 16:27:46.000000 dicencards-0.1.0.dev1/dicencards/dice.py
-drwxrwxrwx   0        0        0        0 2023-05-13 05:21:06.715671 dicencards-0.1.0.dev1/dicencards/rpg/
--rw-rw-rw-   0        0        0     2022 2023-04-24 16:27:46.000000 dicencards-0.1.0.dev1/dicencards/rpg/BRP.py
--rw-rw-rw-   0        0        0     1325 2023-04-24 16:27:46.000000 dicencards-0.1.0.dev1/dicencards/rpg/D6.py
--rw-rw-rw-   0        0        0       48 2023-04-24 16:27:46.000000 dicencards-0.1.0.dev1/dicencards/rpg/Fuzion.py
--rw-rw-rw-   0        0        0      997 2023-04-24 16:27:46.000000 dicencards-0.1.0.dev1/dicencards/rpg/SW.py
--rw-rw-rw-   0        0        0        4 2023-04-24 16:27:46.000000 dicencards-0.1.0.dev1/dicencards/rpg/__init__.py
--rw-rw-rw-   0        0        0       56 2023-04-24 16:27:46.000000 dicencards-0.1.0.dev1/dicencards/rpg/d20.py
--rw-rw-rw-   0        0        0     3904 2023-04-29 06:16:12.000000 dicencards-0.1.0.dev1/dicencards/rpg/deadlands.py
-drwxrwxrwx   0        0        0        0 2023-05-13 05:21:06.684635 dicencards-0.1.0.dev1/dicencards.egg-info/
--rw-rw-rw-   0        0        0      801 2023-05-13 05:21:06.000000 dicencards-0.1.0.dev1/dicencards.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      481 2023-05-13 05:21:06.000000 dicencards-0.1.0.dev1/dicencards.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 05:21:06.000000 dicencards-0.1.0.dev1/dicencards.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-13 05:21:06.000000 dicencards-0.1.0.dev1/dicencards.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-01-28 10:07:36.000000 dicencards-0.1.0.dev1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-13 05:21:06.720509 dicencards-0.1.0.dev1/setup.cfg
--rw-rw-rw-   0        0        0     1282 2023-05-13 05:17:37.000000 dicencards-0.1.0.dev1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 10:01:10.387775 dicencards-0.1.0.dev2/
+-rw-rw-rw-   0        0        0      427 2023-05-29 10:01:10.383792 dicencards-0.1.0.dev2/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2023-05-29 09:59:03.000000 dicencards-0.1.0.dev2/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-29 10:01:10.208829 dicencards-0.1.0.dev2/demo/
+-rw-rw-rw-   0        0        0      306 2023-05-14 06:55:48.000000 dicencards-0.1.0.dev2/demo/BRP_demo.py
+-rw-rw-rw-   0        0        0        0 2023-05-14 06:55:48.000000 dicencards-0.1.0.dev2/demo/__init__.py
+-rw-rw-rw-   0        0        0      124 2023-05-14 06:55:48.000000 dicencards-0.1.0.dev2/demo/deadlands_demo.py
+drwxrwxrwx   0        0        0        0 2023-05-29 10:01:10.240787 dicencards-0.1.0.dev2/dicencards/
+-rw-rw-rw-   0        0        0       84 2023-05-14 07:26:52.000000 dicencards-0.1.0.dev2/dicencards/__init__.py
+-rw-rw-rw-   0        0        0     5355 2023-05-14 06:55:48.000000 dicencards-0.1.0.dev2/dicencards/cards.py
+-rw-rw-rw-   0        0        0     1833 2023-05-14 06:55:48.000000 dicencards-0.1.0.dev2/dicencards/dice.py
+drwxrwxrwx   0        0        0        0 2023-05-29 10:01:10.373805 dicencards-0.1.0.dev2/dicencards/rpg/
+-rw-rw-rw-   0        0        0     2022 2023-05-14 06:55:48.000000 dicencards-0.1.0.dev2/dicencards/rpg/BRP.py
+-rw-rw-rw-   0        0        0     1325 2023-05-14 06:55:48.000000 dicencards-0.1.0.dev2/dicencards/rpg/D6.py
+-rw-rw-rw-   0        0        0       48 2023-05-14 06:55:48.000000 dicencards-0.1.0.dev2/dicencards/rpg/Fuzion.py
+-rw-rw-rw-   0        0        0      997 2023-05-14 06:55:48.000000 dicencards-0.1.0.dev2/dicencards/rpg/SW.py
+-rw-rw-rw-   0        0        0        4 2023-05-14 06:55:48.000000 dicencards-0.1.0.dev2/dicencards/rpg/__init__.py
+-rw-rw-rw-   0        0        0       56 2023-05-14 06:55:48.000000 dicencards-0.1.0.dev2/dicencards/rpg/d20.py
+-rw-rw-rw-   0        0        0     3210 2023-05-14 06:55:48.000000 dicencards-0.1.0.dev2/dicencards/rpg/deadlands.py
+drwxrwxrwx   0        0        0        0 2023-05-29 10:01:10.301637 dicencards-0.1.0.dev2/dicencards.egg-info/
+-rw-rw-rw-   0        0        0      427 2023-05-29 10:01:09.000000 dicencards-0.1.0.dev2/dicencards.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      440 2023-05-29 10:01:09.000000 dicencards-0.1.0.dev2/dicencards.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 10:01:09.000000 dicencards-0.1.0.dev2/dicencards.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-29 10:01:09.000000 dicencards-0.1.0.dev2/dicencards.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 10:01:10.388832 dicencards-0.1.0.dev2/setup.cfg
+-rw-rw-rw-   0        0        0     1080 2023-05-29 10:00:59.000000 dicencards-0.1.0.dev2/setup.py
```

### Comparing `dicencards-0.1.0.dev1/dicencards/cards.py` & `dicencards-0.1.0.dev2/dicencards/cards.py`

 * *Files identical despite different names*

### Comparing `dicencards-0.1.0.dev1/dicencards/dice.py` & `dicencards-0.1.0.dev2/dicencards/dice.py`

 * *Files identical despite different names*

### Comparing `dicencards-0.1.0.dev1/dicencards/rpg/BRP.py` & `dicencards-0.1.0.dev2/dicencards/rpg/BRP.py`

 * *Files identical despite different names*

### Comparing `dicencards-0.1.0.dev1/dicencards/rpg/D6.py` & `dicencards-0.1.0.dev2/dicencards/rpg/D6.py`

 * *Files identical despite different names*

### Comparing `dicencards-0.1.0.dev1/dicencards/rpg/SW.py` & `dicencards-0.1.0.dev2/dicencards/rpg/SW.py`

 * *Files identical despite different names*

### Comparing `dicencards-0.1.0.dev1/dicencards/rpg/deadlands.py` & `dicencards-0.1.0.dev2/dicencards/rpg/deadlands.py`

 * *Files 20% similar despite different names*

```diff
@@ -77,23 +77,19 @@
     cards.append(Card(Rank.JOKER, color=Color.BLACK))
     cards.append(Card(Rank.JOKER, color=Color.RED))
     deck: Deck = Deck(cards)
     deck.shuffle()
     return deck
 
 
-def trait_from_card(card: Card, deck: Deck):
+def trait_from_card(card):
     die_type = TRAIT_DIE_TYPE_CARD_RANK_MAP[card.rank].side_count
     if card.rank == Rank.JOKER:
-        # Immediately after you draw a Joker (which has no suit of its own), draw another card
-        # and use its suit to determine the Joker’s Trait Level ([fr] coordination).
-        # coordination = D4.roll()
-        extra_card = deck.draw(1).pop()
-        print(str(card) + ' trait level card: ' + str(extra_card))
-        coordination = TRAIT_COORDINATION_CARD_COLOR_MAP[extra_card.suite]
+        # Les règles ne fournissent aucunes instructions en ce qui concerne la coordination lors du tirage d'un Joker
+        coordination = D4.roll()
     else:
         coordination = TRAIT_COORDINATION_CARD_COLOR_MAP[card.suite]
     return BunchOfDice(coordination, die_type)
 
 
 def character_draw():
     deck: Deck = build_deck()
@@ -110,26 +106,10 @@
             del hand[i]
         i = i - 1
 
     print(' |'.join(str(c) for c in hand))
 
     trait_dice = []
     for card in hand:
-        trait_dice.append(trait_from_card(card, deck))
+        trait_dice.append(trait_from_card(card))
 
     print(' | '.join(str(d) for d in trait_dice))
-
-    # Mysterious past
-    joker_count = 0
-    for card in hand:
-        if card.rank is Rank.JOKER:
-            joker_count += 1
-    if joker_count > 0:
-        action_deck: Deck = build_deck()
-        mysterious_past_cards = action_deck.draw(joker_count)
-        print('Mysterious past')
-        print(' |'.join(str(c) for c in mysterious_past_cards))
-    else:
-        print('No mysterious past')
-
-
-
```

### Comparing `dicencards-0.1.0.dev1/setup.py` & `dicencards-0.1.0.dev2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import os
 from setuptools import setup, find_packages
 
 __name__ = 'dicencards'
-__version__ = '0.1.0.dev1'
+__version__ = '0.1.0.dev2'
 __author__ = 'Xavier ROY'
 __author_email__ = 'xavier@regbuddy.eu'
 
 project_dir = os.path.dirname(os.path.realpath(__file__))
 requirement_file_path = project_dir + '/requirements.txt'
 requirements = []
 if os.path.isfile(requirement_file_path):
@@ -17,25 +17,23 @@
         requirements = f.read().splitlines()
 
 setup(
     name=__name__,
     version=__version__,
     author=__author__,
     author_email=__author_email__,
-    url='https://bitbucket.org/monkeytechnologies/monkey-crawler',
-    description='Small API to manage dice rolls and cards draws.',
-    long_description=open('README.rst').read(),
+    url='https://bitbucket.org/xroy/dicencards/',
+    description='Dice\'n\'Cards project',
+    
     license="Apache License, Version 2.0",
 
     packages=find_packages(),
     include_package_data=True,
     install_requires=requirements,
 
     classifiers=[
         'Programming Language :: Python',
         'Development Status :: 1 - Planning',
         'Operating System :: OS Independent',
-        'Programming Language :: Python :: 3.8',
-        'Topic :: Software Development :: Libraries :: Python Modules',
-        'Intended Audience :: Developers'
+        'Programming Language :: Python :: 3.9'
     ]
 )
```

