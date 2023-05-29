# Comparing `tmp/timona-0.0.2.tar.gz` & `tmp/timona-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timona-0.0.2.tar", max compression
+gzip compressed data, was "timona-0.0.3.tar", max compression
```

## Comparing `timona-0.0.2.tar` & `timona-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11357 2023-05-26 12:17:14.109740 timona-0.0.2/LICENSE
--rw-r--r--   0        0        0       46 2023-05-26 12:19:29.287039 timona-0.0.2/README.md
--rw-r--r--   0        0        0      542 2023-05-28 07:29:37.581550 timona-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-26 13:27:02.242952 timona-0.0.2/timona/__init__.py
--rw-r--r--   0        0        0       62 2023-05-26 12:53:23.927626 timona-0.0.2/timona/__main__.py
--rw-r--r--   0        0        0       38 2023-05-28 07:29:37.581550 timona-0.0.2/timona/__version__.py
--rw-r--r--   0        0        0     1177 2023-05-28 07:24:27.978336 timona-0.0.2/timona/config.py
--rw-r--r--   0        0        0     2715 2023-05-26 12:19:29.311040 timona-0.0.2/timona/helm.py
--rw-r--r--   0        0        0     2766 2023-05-26 13:16:03.924441 timona-0.0.2/timona/main.py
--rw-r--r--   0        0        0     5148 2023-05-28 06:06:31.058605 timona-0.0.2/timona/releases.py
--rw-r--r--   0        0        0     1190 2023-05-26 17:41:50.796484 timona-0.0.2/timona/template.py
--rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 timona-0.0.2/setup.py
--rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 timona-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-26 12:17:14.109740 timona-0.0.3/LICENSE
+-rw-r--r--   0        0        0       46 2023-05-26 12:19:29.287039 timona-0.0.3/README.md
+-rw-r--r--   0        0        0      542 2023-05-29 08:13:17.409564 timona-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-26 13:27:02.242952 timona-0.0.3/timona/__init__.py
+-rw-r--r--   0        0        0       62 2023-05-26 12:53:23.927626 timona-0.0.3/timona/__main__.py
+-rw-r--r--   0        0        0       38 2023-05-29 08:13:17.413564 timona-0.0.3/timona/__version__.py
+-rw-r--r--   0        0        0     1177 2023-05-28 07:24:27.978336 timona-0.0.3/timona/config.py
+-rw-r--r--   0        0        0     2715 2023-05-26 12:19:29.311040 timona-0.0.3/timona/helm.py
+-rw-r--r--   0        0        0     2766 2023-05-26 13:16:03.924441 timona-0.0.3/timona/main.py
+-rw-r--r--   0        0        0     4946 2023-05-29 07:37:05.204532 timona-0.0.3/timona/releases.py
+-rw-r--r--   0        0        0     1408 2023-05-29 07:40:45.722364 timona-0.0.3/timona/template.py
+-rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 timona-0.0.3/setup.py
+-rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 timona-0.0.3/PKG-INFO
```

### Comparing `timona-0.0.2/LICENSE` & `timona-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `timona-0.0.2/pyproject.toml` & `timona-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "timona"
-version = "0.0.2"
+version = "0.0.3"
 description = "Tool to automate Helm deployments"
 authors = ["mihaiush <mihaiush@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/mihaiush/timona"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `timona-0.0.2/timona/config.py` & `timona-0.0.3/timona/config.py`

 * *Files identical despite different names*

### Comparing `timona-0.0.2/timona/helm.py` & `timona-0.0.3/timona/helm.py`

 * *Files identical despite different names*

### Comparing `timona-0.0.2/timona/main.py` & `timona-0.0.3/timona/main.py`

 * *Files identical despite different names*

### Comparing `timona-0.0.2/timona/releases.py` & `timona-0.0.3/timona/releases.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 #!/usr/bin/env python3
 
 import yaml
 from threading import Thread
-import subprocess
 from pprint import pformat
 import os
 import itertools
 
 
 def flatten_matrix(matrix):
     flat_matrix = []
@@ -117,17 +116,14 @@
                 _releases.append(x['r']['d'])
             else:
                 msg = ''
                 msg = msg + 'Loop or template error\n'
                 msg = msg + 'Latest data:\n'
                 msg = msg + pformat(x['r']['e']['last']) + '\n'
                 msg = msg + 'Error: {}\n'.format(x['r']['e']['err'])
-                if type(x['r']['e']['err']) is subprocess.CalledProcessError:
-                    msg = msg + '  stderr: {}'.format(
-                        x['r']['e']['err'].stderr)
                 raise RuntimeError(msg)
         out = _releases
 
         # Cleanup variables staring with _
         # Check for duplicate names
         _releases = {}
         for release in out:
```

### Comparing `timona-0.0.2/timona/template.py` & `timona-0.0.3/timona/template.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,18 +21,23 @@
         self.version = v
         self.var_re = config.get('regex')
         if self.var_re:
             self.var_re = re.compile(self.var_re)
 
     def render(self, tpl, env):
         if self.cmd:
-            p = subprocess.run(
-                shlex.split(self.cmd),
-                input=tpl, env={**env, **os.environ},
-                capture_output=True, check=True, text=True,
-            )
+            try:
+                p = subprocess.run(
+                    shlex.split(self.cmd),
+                    input=tpl, env={**env, **os.environ},
+                    capture_output=True, check=True, text=True,
+                )
+            except subprocess.CalledProcessError as e:
+                raise subprocess.SubprocessError(e.stderr) from e
             if p.stderr.strip():
                 if self.stderr == 'print':
                     print(p.stderr, file=sys.stderr)
                 elif self.stderr == 'error':
-                    raise RuntimeError('Render error:\n{}'.format(p.stderr))
+                    raise subprocess.SubprocessError(
+                        'Render error:\n{}'.format(p.stderr)
+                    )
             return p.stdout
```

### Comparing `timona-0.0.2/setup.py` & `timona-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['deepmerge', 'jinja2', 'pyyaml', 'requests']
 
 entry_points = \
 {'console_scripts': ['timona = timona.main:main']}
 
 setup_kwargs = {
     'name': 'timona',
-    'version': '0.0.2',
+    'version': '0.0.3',
     'description': 'Tool to automate Helm deployments',
     'long_description': '# timona\n\nA tool to automate Helm deployments\n',
     'author': 'mihaiush',
     'author_email': 'mihaiush@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mihaiush/timona',
```

### Comparing `timona-0.0.2/PKG-INFO` & `timona-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timona
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tool to automate Helm deployments
 Home-page: https://github.com/mihaiush/timona
 Author: mihaiush
 Author-email: mihaiush@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

