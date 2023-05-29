# Comparing `tmp/problemator-1.0.5.tar.gz` & `tmp/problemator-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\main\GitHub ???????????\problemator\dist\tmpmpcrvzcg\problemator-1.0.5.tar", last modified: Fri Nov 18 04:40:42 2022, max compression
+gzip compressed data, was "problemator-1.1.0.tar", last modified: Mon May 29 19:51:56 2023, max compression
```

## Comparing `problemator-1.0.5.tar` & `problemator-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-11-18 04:40:42.000000 problemator-1.0.5/
--rw-rw-rw-   0        0        0     1080 2022-09-07 13:19:49.000000 problemator-1.0.5/LICENSE
--rw-rw-rw-   0        0        0       34 2022-04-12 16:05:18.000000 problemator-1.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1459 2022-11-18 04:40:42.000000 problemator-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      886 2022-11-18 04:37:29.000000 problemator-1.0.5/README.MD
-drwxrwxrwx   0        0        0        0 2022-11-18 04:40:42.000000 problemator-1.0.5/problemator/
--rw-rw-rw-   0        0        0       95 2022-11-18 04:30:40.000000 problemator-1.0.5/problemator/__init__.py
--rw-rw-rw-   0        0        0     2306 2022-11-18 04:36:30.000000 problemator-1.0.5/problemator/problemator.py
-drwxrwxrwx   0        0        0        0 2022-11-18 04:40:42.000000 problemator-1.0.5/problemator.egg-info/
--rw-rw-rw-   0        0        0     1459 2022-11-18 04:40:42.000000 problemator-1.0.5/problemator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2022-11-18 04:40:42.000000 problemator-1.0.5/problemator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-18 04:40:42.000000 problemator-1.0.5/problemator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2022-11-18 04:40:42.000000 problemator-1.0.5/problemator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2022-11-18 04:40:42.000000 problemator-1.0.5/problemator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-18 04:40:42.000000 problemator-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      892 2022-11-18 04:38:30.000000 problemator-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 19:51:56.891997 problemator-1.1.0/
+-rw-rw-rw-   0        0        0     1080 2023-05-29 19:44:03.000000 problemator-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0       34 2022-04-12 16:05:18.000000 problemator-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1499 2023-05-29 19:51:56.891997 problemator-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      926 2023-05-29 19:50:56.000000 problemator-1.1.0/README.MD
+drwxrwxrwx   0        0        0        0 2023-05-29 19:51:56.889006 problemator-1.1.0/problemator/
+-rw-rw-rw-   0        0        0       36 2023-05-29 19:50:54.000000 problemator-1.1.0/problemator/__init__.py
+-rw-rw-rw-   0        0        0     2580 2023-05-29 19:50:53.000000 problemator-1.1.0/problemator/problemator.py
+drwxrwxrwx   0        0        0        0 2023-05-29 19:51:56.891997 problemator-1.1.0/problemator.egg-info/
+-rw-rw-rw-   0        0        0     1499 2023-05-29 19:51:56.000000 problemator-1.1.0/problemator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2023-05-29 19:51:56.000000 problemator-1.1.0/problemator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 19:51:56.000000 problemator-1.1.0/problemator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-29 19:51:56.000000 problemator-1.1.0/problemator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-29 19:51:56.000000 problemator-1.1.0/problemator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 19:51:56.891997 problemator-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      892 2023-05-29 19:51:21.000000 problemator-1.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `problemator-1.0.5/LICENSE` & `problemator-1.1.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2022 Vladislav Zenkevich
+Copyright (c) 2023 Vladislav Zenkevich
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `problemator-1.0.5/PKG-INFO` & `problemator-1.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: problemator
-Version: 1.0.5
+Version: 1.1.0
 Summary: WolframAlpha's Unlimited AI-generated practice problems and answers API wrapper.
 Home-page: https://github.com/DedInc/problemator
 Author: Maehdakvan
 Author-email: visitanimation@google.com
 Project-URL: Bug Tracker, https://github.com/DedInc/problemator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,29 +16,29 @@
 <h1 align="center">problemator - WolframAlpha's Unlimited AI-generated practice problems and answers API wrapper.</h1>
 
 <br>
 
 <h1 align="center"> -How to use- </h1>
 
 ```python
-from problemator import *
+from problemator import Problemator
 from random import choice
 
-loadSession()  # Initialize
-print(getCategories())  # See categories
+p = Problemator()  # Initialize
+print(p.categories)  # See categories
 
-category = getCategory(0)  # Get Addition
+category = p.get_category(0)  # Get Addition
 
 # LVL: 0 - Beginner; 1 - Intermediate; 2 - Advanced
 # Count - Number of problems
 # type - Category
-problem = generateProblem(lvl=0, type=category) # Generate a problem
+problem = p.generate_problem(lvl=0, type=category) # Generate a problem
 
 print(problem['text'])  # Text of the problem
 print(problem['image'])  # Image of the problem
 print(problem['difficulty'])  # Difficulty of the problem
 
-c = checkProblem(problem, 'x+5')  # Check problem, where x+5 - answer
-print(c['correct'])  # True or False
-print(c['hint'])  # Image of the Hint
-print(c['solution'])  # Image of the Solution
+result = p.check_problem(problem, 'x+5')  # Check problem, where x+5 - answer
+print(result['correct'])  # True or False
+print(result['hint'])  # Image of the Hint
+print(result['solution'])  # Image of the Solution
 ```
```

### Comparing `problemator-1.0.5/problemator/problemator.py` & `problemator-1.1.0/problemator/problemator.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,60 +1,54 @@
 from requests import Session, get
 from requests.cookies import create_cookie
 from user_agent import generate_user_agent
 
-categories = {}
 
-
-def searchCategories(cats):
-    global categories
-    for c in cats:
-        if 'Subcategories' in c:
-            searchCategories(c['Subcategories'])
-        else:
-            categories[c['LinkTo']] = len(categories)
-
-
-def getCategories():
-    return categories
-
-
-def getCategory(id):
-    for cat in categories.keys():
-        if categories[cat] == id:
-            return cat
-
-
-def loadSession():
-    global API, s
-    s = Session()
-    s.headers['User-Agent'] = generate_user_agent()
-    s.headers['Accept'] = 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9'
-    s.headers['Accept-Encoding'] = 'gzip, deflate, br'
-    s.headers['Accept-Language'] = 'ru-RU,ru;q=0.9,kk-KZ;q=0.8,kk;q=0.7,en-US;q=0.6,en;q=0.5'
-
-    r = s.get('https://www.wolframalpha.com/input/wpg/categories.jsp?load=true').json()
-    searchCategories(r['Categories']['Categories'])
-    API = r['domain']
-
-def checkProblem(problem, answer):
-    lvl = problem['difficulty']
-    pid = problem['id']
-    machine = problem['machine']
-    for c in problem['session']:
-        cookie = create_cookie(name=c['name'], value=c['value'], domain=c['domain'])
-        s.cookies.set_cookie(cookie)
-    r = s.get(f'{API}/input/wpg/checkanswer.jsp?attempt=1&difficulty={lvl}&load=true&problemID={pid}&query={answer}&s={machine}&type=InputField').json()
-    return {'correct': r['correct'], 'hint': r['hint'], 'solution': r['solution']}
-
-
-def generateProblem(lvl=0, type='IntegerAddition'):
-    lvl = {0: 'Beginner', 1: 'Intermediate', 2: 'Advanced'}[lvl]
-    r = s.get(f'{API}/input/wpg/problem.jsp?count=1&difficulty={lvl}&load=1&type={type}').json()
-    problems = r['problems']
-    machine = r['machine']
-    cookies = []
-    for c in s.cookies:
-        if c.name == 'JSESSIONID':
-            cookies.append({'name': c.name, 'value': c.value, 'domain': c.domain})
-    problem = problems[0]
-    return {'text': problem['string_question'], 'image': problem['problem_image'], 'difficulty': lvl, 'id': problem['problem_id'], 'machine': machine, 'session': cookies}
+class Problemator:
+    def __init__(self):
+        self.categories = {}
+        self.load_session()
+
+    def search_categories(self, cats):
+        for c in cats:
+            if 'Subcategories' in c:
+                self.search_categories(c['Subcategories'])
+            else:
+                self.categories[c['LinkTo']] = len(self.categories)
+
+    def get_category(self, id):
+        for cat in self.categories.keys():
+            if self.categories[cat] == id:
+                return cat
+
+    def load_session(self):
+        self.s = Session()
+        self.s.headers['User-Agent'] = generate_user_agent()
+        self.s.headers['Accept'] = 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9'
+        self.s.headers['Accept-Encoding'] = 'gzip, deflate, br'
+        self.s.headers['Accept-Language'] = 'ru-RU,ru;q=0.9,kk-KZ;q=0.8,kk;q=0.7,en-US;q=0.6,en;q=0.5'
+
+        r = self.s.get('https://www.wolframalpha.com/input/wpg/categories.jsp?load=true').json()
+        self.search_categories(r['Categories']['Categories'])
+        self.API = r['domain']
+
+    def check_problem(self, problem, answer):
+        lvl = problem['difficulty']
+        pid = problem['id']
+        machine = problem['machine']
+        for c in problem['session']:
+            cookie = create_cookie(name=c['name'], value=c['value'], domain=c['domain'])
+            self.s.cookies.set_cookie(cookie)
+        r = self.s.get(f'{self.API}/input/wpg/checkanswer.jsp?attempt=1&difficulty={lvl}&load=true&problemID={pid}&query={answer}&s={machine}&type=InputField').json()
+        return {'correct': r['correct'], 'hint': r['hint'], 'solution': r['solution']}
+
+    def generate_problem(self, lvl=0, type='IntegerAddition'):
+        lvl = {0: 'Beginner', 1: 'Intermediate', 2: 'Advanced'}[lvl]
+        r = self.s.get(f'{self.API}/input/wpg/problem.jsp?count=1&difficulty={lvl}&load=1&type={type}').json()
+        problems = r['problems']
+        machine = r['machine']
+        cookies = []
+        for c in self.s.cookies:
+            if c.name == 'JSESSIONID':
+                cookies.append({'name': c.name, 'value': c.value, 'domain': c.domain})
+        problem = problems[0]
+        return {'text': problem['string_question'], 'image': problem['problem_image'], 'difficulty': lvl, 'id': problem['problem_id'], 'machine': machine, 'session': cookies}
```

### Comparing `problemator-1.0.5/problemator.egg-info/PKG-INFO` & `problemator-1.1.0/problemator.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: problemator
-Version: 1.0.5
+Version: 1.1.0
 Summary: WolframAlpha's Unlimited AI-generated practice problems and answers API wrapper.
 Home-page: https://github.com/DedInc/problemator
 Author: Maehdakvan
 Author-email: visitanimation@google.com
 Project-URL: Bug Tracker, https://github.com/DedInc/problemator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,29 +16,29 @@
 <h1 align="center">problemator - WolframAlpha's Unlimited AI-generated practice problems and answers API wrapper.</h1>
 
 <br>
 
 <h1 align="center"> -How to use- </h1>
 
 ```python
-from problemator import *
+from problemator import Problemator
 from random import choice
 
-loadSession()  # Initialize
-print(getCategories())  # See categories
+p = Problemator()  # Initialize
+print(p.categories)  # See categories
 
-category = getCategory(0)  # Get Addition
+category = p.get_category(0)  # Get Addition
 
 # LVL: 0 - Beginner; 1 - Intermediate; 2 - Advanced
 # Count - Number of problems
 # type - Category
-problem = generateProblem(lvl=0, type=category) # Generate a problem
+problem = p.generate_problem(lvl=0, type=category) # Generate a problem
 
 print(problem['text'])  # Text of the problem
 print(problem['image'])  # Image of the problem
 print(problem['difficulty'])  # Difficulty of the problem
 
-c = checkProblem(problem, 'x+5')  # Check problem, where x+5 - answer
-print(c['correct'])  # True or False
-print(c['hint'])  # Image of the Hint
-print(c['solution'])  # Image of the Solution
+result = p.check_problem(problem, 'x+5')  # Check problem, where x+5 - answer
+print(result['correct'])  # True or False
+print(result['hint'])  # Image of the Hint
+print(result['solution'])  # Image of the Solution
 ```
```

### Comparing `problemator-1.0.5/setup.py` & `problemator-1.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="problemator",
-    version="1.0.5",
+    version="1.1.0",
     author="Maehdakvan",
     author_email="visitanimation@google.com",
     description="WolframAlpha's Unlimited AI-generated practice problems and answers API wrapper.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/DedInc/problemator",
     project_urls={
```

