# Comparing `tmp/fronty-0.0.4.tar.gz` & `tmp/fronty-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fronty-0.0.4.tar", last modified: Mon May 29 20:07:15 2023, max compression
+gzip compressed data, was "fronty-0.0.5.tar", last modified: Mon May 29 20:51:20 2023, max compression
```

## Comparing `fronty-0.0.4.tar` & `fronty-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 legend    (1000) legend    (1000)        0 2023-05-29 20:07:15.322857 fronty-0.0.4/
--rwxrwxrwx   0 legend    (1000) legend    (1000)     1065 2023-05-09 14:36:52.000000 fronty-0.0.4/LICENSE
--rwxrwxrwx   0 legend    (1000) legend    (1000)     4847 2023-05-29 20:07:15.321548 fronty-0.0.4/PKG-INFO
--rwxrwxrwx   0 legend    (1000) legend    (1000)     4069 2023-03-02 21:13:50.000000 fronty-0.0.4/README.md
-drwxrwxrwx   0 legend    (1000) legend    (1000)        0 2023-05-29 20:07:15.279060 fronty-0.0.4/fronty/
--rwxrwxrwx   0 legend    (1000) legend    (1000)      226 2023-03-02 21:10:25.000000 fronty-0.0.4/fronty/__init__.py
--rwxrwxrwx   0 legend    (1000) legend    (1000)      558 2023-02-28 18:10:59.000000 fronty-0.0.4/fronty/cli.py
-drwxrwxrwx   0 legend    (1000) legend    (1000)        0 2023-05-29 20:07:15.301821 fronty-0.0.4/fronty/css/
--rwxrwxrwx   0 legend    (1000) legend    (1000)     3722 2023-03-01 16:43:50.000000 fronty-0.0.4/fronty/css/__init__.py
-drwxrwxrwx   0 legend    (1000) legend    (1000)        0 2023-05-29 20:07:15.311311 fronty-0.0.4/fronty/html/
--rwxrwxrwx   0 legend    (1000) legend    (1000)    18671 2023-05-29 18:41:45.000000 fronty-0.0.4/fronty/html/__init__.py
--rwxrwxrwx   0 legend    (1000) legend    (1000)     7361 2023-05-29 18:43:53.000000 fronty-0.0.4/fronty/html/widgets.py
-drwxrwxrwx   0 legend    (1000) legend    (1000)        0 2023-05-29 20:07:15.317860 fronty-0.0.4/fronty/middlewares/
--rwxrwxrwx   0 legend    (1000) legend    (1000)        0 2023-02-28 17:53:45.000000 fronty-0.0.4/fronty/middlewares/__init__.py
-drwxrwxrwx   0 legend    (1000) legend    (1000)        0 2023-05-29 20:07:15.299119 fronty-0.0.4/fronty.egg-info/
--rwxrwxrwx   0 legend    (1000) legend    (1000)     4847 2023-05-29 20:07:15.000000 fronty-0.0.4/fronty.egg-info/PKG-INFO
--rwxrwxrwx   0 legend    (1000) legend    (1000)      313 2023-05-29 20:07:15.000000 fronty-0.0.4/fronty.egg-info/SOURCES.txt
--rwxrwxrwx   0 legend    (1000) legend    (1000)        1 2023-05-29 20:07:15.000000 fronty-0.0.4/fronty.egg-info/dependency_links.txt
--rwxrwxrwx   0 legend    (1000) legend    (1000)       43 2023-05-29 20:07:15.000000 fronty-0.0.4/fronty.egg-info/entry_points.txt
--rwxrwxrwx   0 legend    (1000) legend    (1000)        7 2023-05-29 20:07:15.000000 fronty-0.0.4/fronty.egg-info/top_level.txt
--rwxrwxrwx   0 legend    (1000) legend    (1000)       38 2023-05-29 20:07:15.323446 fronty-0.0.4/setup.cfg
--rwxrwxrwx   0 legend    (1000) legend    (1000)     1100 2023-05-29 20:06:15.000000 fronty-0.0.4/setup.py
+drwxrwxrwx   0 legend    (1000) legend    (1000)        0 2023-05-29 20:51:20.410585 fronty-0.0.5/
+-rwxrwxrwx   0 legend    (1000) legend    (1000)     1065 2023-05-09 14:36:52.000000 fronty-0.0.5/LICENSE
+-rwxrwxrwx   0 legend    (1000) legend    (1000)     4847 2023-05-29 20:51:20.409429 fronty-0.0.5/PKG-INFO
+-rwxrwxrwx   0 legend    (1000) legend    (1000)     4069 2023-03-02 21:13:50.000000 fronty-0.0.5/README.md
+drwxrwxrwx   0 legend    (1000) legend    (1000)        0 2023-05-29 20:51:20.381809 fronty-0.0.5/fronty/
+-rwxrwxrwx   0 legend    (1000) legend    (1000)      226 2023-03-02 21:10:25.000000 fronty-0.0.5/fronty/__init__.py
+-rwxrwxrwx   0 legend    (1000) legend    (1000)      558 2023-02-28 18:10:59.000000 fronty-0.0.5/fronty/cli.py
+drwxrwxrwx   0 legend    (1000) legend    (1000)        0 2023-05-29 20:51:20.398673 fronty-0.0.5/fronty/css/
+-rwxrwxrwx   0 legend    (1000) legend    (1000)     3722 2023-03-01 16:43:50.000000 fronty-0.0.5/fronty/css/__init__.py
+drwxrwxrwx   0 legend    (1000) legend    (1000)        0 2023-05-29 20:51:20.404427 fronty-0.0.5/fronty/html/
+-rwxrwxrwx   0 legend    (1000) legend    (1000)    18671 2023-05-29 18:41:45.000000 fronty-0.0.5/fronty/html/__init__.py
+-rwxrwxrwx   0 legend    (1000) legend    (1000)     7455 2023-05-29 20:31:12.000000 fronty-0.0.5/fronty/html/widgets.py
+drwxrwxrwx   0 legend    (1000) legend    (1000)        0 2023-05-29 20:51:20.407006 fronty-0.0.5/fronty/middlewares/
+-rwxrwxrwx   0 legend    (1000) legend    (1000)        0 2023-02-28 17:53:45.000000 fronty-0.0.5/fronty/middlewares/__init__.py
+drwxrwxrwx   0 legend    (1000) legend    (1000)        0 2023-05-29 20:51:20.396293 fronty-0.0.5/fronty.egg-info/
+-rwxrwxrwx   0 legend    (1000) legend    (1000)     4847 2023-05-29 20:51:20.000000 fronty-0.0.5/fronty.egg-info/PKG-INFO
+-rwxrwxrwx   0 legend    (1000) legend    (1000)      313 2023-05-29 20:51:20.000000 fronty-0.0.5/fronty.egg-info/SOURCES.txt
+-rwxrwxrwx   0 legend    (1000) legend    (1000)        1 2023-05-29 20:51:20.000000 fronty-0.0.5/fronty.egg-info/dependency_links.txt
+-rwxrwxrwx   0 legend    (1000) legend    (1000)       43 2023-05-29 20:51:20.000000 fronty-0.0.5/fronty.egg-info/entry_points.txt
+-rwxrwxrwx   0 legend    (1000) legend    (1000)        7 2023-05-29 20:51:20.000000 fronty-0.0.5/fronty.egg-info/top_level.txt
+-rwxrwxrwx   0 legend    (1000) legend    (1000)       38 2023-05-29 20:51:20.410944 fronty-0.0.5/setup.cfg
+-rwxrwxrwx   0 legend    (1000) legend    (1000)     1100 2023-05-29 20:48:04.000000 fronty-0.0.5/setup.py
```

### Comparing `fronty-0.0.4/LICENSE` & `fronty-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fronty-0.0.4/PKG-INFO` & `fronty-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fronty
-Version: 0.0.4
+Version: 0.0.5
 Summary: A frontend web framework
 Home-page: https://github.com/Almas-Ali/fronty
 Author: Almas Ali
 Author-email: almaspr3@gmail.com
 Keywords: web framework
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `fronty-0.0.4/README.md` & `fronty-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `fronty-0.0.4/fronty/cli.py` & `fronty-0.0.5/fronty/cli.py`

 * *Files identical despite different names*

### Comparing `fronty-0.0.4/fronty/css/__init__.py` & `fronty-0.0.5/fronty/css/__init__.py`

 * *Files identical despite different names*

### Comparing `fronty-0.0.4/fronty/html/__init__.py` & `fronty-0.0.5/fronty/html/__init__.py`

 * *Files identical despite different names*

### Comparing `fronty-0.0.4/fronty/html/widgets.py` & `fronty-0.0.5/fronty/html/widgets.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         self._action = kwargs['action'] if 'action' in kwargs else '#'
         self._method = kwargs['method'] if 'method' in kwargs else 'post'
         self.load_css = True if 'load_css' in kwargs else False
 
     def render(self):
         '''Renders the widget.'''
         if self._type in self.forms_type:
-            return self.__get_form()
+            return self.__get_form().render()
 
     def __get_form(self):
         '''Generates the form.'''
         if self._type == 'loginform':
             return self.__get_loginform()
         elif self._type == 'registrationform':
             return self.__get_registrationform()
@@ -129,15 +129,15 @@
 
             # All styles are included here if load_css is True.
             html.Style(
                 styles.render()
             ) if self.load_css is True else html.Style(),
 
             html.Form(
-                self._element['first'],  # First loaded elements
+                self._element.get('first') if 'first' in self._element else '',
                 html.Div(
                     html.Label('Username'),
                     html.Input(type='text', name='username',
                                placeholder='Username'),
                 ),
                 html.Div(
                     html.Label('Password'),
@@ -146,15 +146,15 @@
                     .name('password')
                     .placeholder('********')
                 ),
                 html.Div(
                     html.Button('Submit')
                     .type('submit'),
                 ),
-                self._element['last'],  # Last loaded elements
+                self._element.get('last') if 'last' in self._element else '',
             )
             .attr('action', self._action)
             .attr('method', self._method)
             .id('form-object'),
         )
 
     def __get_registrationform(self):
@@ -197,15 +197,15 @@
         return html.Section(
 
             html.Style(
                 styles.render()
             ) if self.load_css is True else html.Style(),
 
             html.Form(
-                self._element['first'],
+                self._element.get('first') if 'first' in self._element else '',
 
                 html.Div(
                     html.Label('Username'),
                     html.Input(type='text', name='username',
                                placeholder='Username'),
                 ),
                 html.Div(
@@ -213,10 +213,10 @@
                     html.Input(type='password', name='password', placeholder='****'
                                ),
                     html.Div(
                         html.Button('Submit', type='submit'),
                     ),
                 ),
 
-                self._element['last'],  # Last loaded elements
+                self._element.get('last') if 'last' in self._element else '',
             ).id('form-object'),
         )
```

### Comparing `fronty-0.0.4/fronty.egg-info/PKG-INFO` & `fronty-0.0.5/fronty.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fronty
-Version: 0.0.4
+Version: 0.0.5
 Summary: A frontend web framework
 Home-page: https://github.com/Almas-Ali/fronty
 Author: Almas Ali
 Author-email: almaspr3@gmail.com
 Keywords: web framework
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `fronty-0.0.4/setup.py` & `fronty-0.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='fronty',
-    version='0.0.4',
+    version='0.0.5',
     description='A frontend web framework',
     long_description_content_type='text/markdown',
     long_description=long_description,
     author='Almas Ali',
     author_email='almaspr3@gmail.com',
     url='https://github.com/Almas-Ali/fronty',
     packages=find_packages(),
```

