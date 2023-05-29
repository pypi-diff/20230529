# Comparing `tmp/tailraiders-0.0.7.tar.gz` & `tmp/tailraiders-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tailraiders-0.0.7.tar", last modified: Tue May 23 10:02:39 2023, max compression
+gzip compressed data, was "tailraiders-0.0.8.tar", last modified: Mon May 29 14:05:52 2023, max compression
```

## Comparing `tailraiders-0.0.7.tar` & `tailraiders-0.0.8.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 10:02:39.647758 tailraiders-0.0.7/
--rw-rw-rw-   0        0        0      696 2023-05-15 11:30:33.000000 tailraiders-0.0.7/LICENSE
--rw-rw-rw-   0        0        0       34 2023-05-15 11:31:16.000000 tailraiders-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     1012 2023-05-23 10:02:39.646287 tailraiders-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      687 2023-05-23 10:01:41.000000 tailraiders-0.0.7/README.md
--rw-rw-rw-   0        0        0       42 2023-05-23 10:02:39.648816 tailraiders-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      646 2023-05-23 10:01:43.000000 tailraiders-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-23 10:02:39.589107 tailraiders-0.0.7/tailraiders/
--rw-rw-rw-   0        0        0      932 2023-05-23 09:55:55.000000 tailraiders-0.0.7/tailraiders/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 10:02:39.623887 tailraiders-0.0.7/tailraiders/boaboa/
--rw-rw-rw-   0        0        0      141 2023-05-23 09:34:49.000000 tailraiders-0.0.7/tailraiders/boaboa/__init__.py
--rw-rw-rw-   0        0        0     2521 2023-05-23 09:27:58.000000 tailraiders-0.0.7/tailraiders/boaboa/doc.py
-drwxrwxrwx   0        0        0        0 2023-05-23 10:02:39.627076 tailraiders-0.0.7/tailraiders/bugtrapper/
--rw-rw-rw-   0        0        0      110 2023-05-23 09:36:01.000000 tailraiders-0.0.7/tailraiders/bugtrapper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 10:02:39.633554 tailraiders-0.0.7/tailraiders/gajalaka/
--rw-rw-rw-   0        0        0      132 2023-05-23 09:35:13.000000 tailraiders-0.0.7/tailraiders/gajalaka/__init__.py
--rw-rw-rw-   0        0        0     6208 2023-05-23 10:02:12.000000 tailraiders-0.0.7/tailraiders/gajalaka/plots.py
-drwxrwxrwx   0        0        0        0 2023-05-23 10:02:39.635733 tailraiders-0.0.7/tailraiders/plunderer/
--rw-rw-rw-   0        0        0        0 2023-05-15 09:46:55.000000 tailraiders-0.0.7/tailraiders/plunderer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 10:02:39.640741 tailraiders-0.0.7/tailraiders/protector/
--rw-rw-rw-   0        0        0      135 2023-05-23 09:35:05.000000 tailraiders-0.0.7/tailraiders/protector/__init__.py
--rw-rw-rw-   0        0        0     3635 2023-05-23 09:24:23.000000 tailraiders-0.0.7/tailraiders/protector/nan.py
-drwxrwxrwx   0        0        0        0 2023-05-23 10:02:39.644139 tailraiders-0.0.7/tailraiders/trouper/
--rw-rw-rw-   0        0        0        0 2023-05-15 10:03:58.000000 tailraiders-0.0.7/tailraiders/trouper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 10:02:39.618686 tailraiders-0.0.7/tailraiders.egg-info/
--rw-rw-rw-   0        0        0     1012 2023-05-23 10:02:38.000000 tailraiders-0.0.7/tailraiders.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      520 2023-05-23 10:02:39.000000 tailraiders-0.0.7/tailraiders.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 10:02:38.000000 tailraiders-0.0.7/tailraiders.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-05-23 10:02:38.000000 tailraiders-0.0.7/tailraiders.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-23 10:02:38.000000 tailraiders-0.0.7/tailraiders.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-29 14:05:52.072926 tailraiders-0.0.8/
+-rw-rw-rw-   0        0        0     1087 2023-05-29 12:00:40.000000 tailraiders-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-05-15 11:31:16.000000 tailraiders-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      875 2023-05-29 14:05:52.071926 tailraiders-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      592 2023-05-29 13:52:37.000000 tailraiders-0.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-29 14:05:52.072926 tailraiders-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      649 2023-05-29 13:56:02.000000 tailraiders-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:05:52.024768 tailraiders-0.0.8/tailraiders/
+-rw-rw-rw-   0        0        0     1066 2023-05-29 13:46:05.000000 tailraiders-0.0.8/tailraiders/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:05:52.046000 tailraiders-0.0.8/tailraiders/boaboa/
+-rw-rw-rw-   0        0        0      142 2023-05-29 13:21:30.000000 tailraiders-0.0.8/tailraiders/boaboa/__init__.py
+-rw-rw-rw-   0        0        0     2556 2023-05-29 13:46:50.000000 tailraiders-0.0.8/tailraiders/boaboa/doc.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:05:52.048203 tailraiders-0.0.8/tailraiders/bugtrapper/
+-rw-rw-rw-   0        0        0       54 2023-05-29 13:21:39.000000 tailraiders-0.0.8/tailraiders/bugtrapper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:05:52.052832 tailraiders-0.0.8/tailraiders/gajalaka/
+-rw-rw-rw-   0        0        0      134 2023-05-29 13:22:06.000000 tailraiders-0.0.8/tailraiders/gajalaka/__init__.py
+-rw-rw-rw-   0        0        0     6313 2023-05-29 13:47:35.000000 tailraiders-0.0.8/tailraiders/gajalaka/plots.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:05:52.055832 tailraiders-0.0.8/tailraiders/plunderer/
+-rw-rw-rw-   0        0        0       53 2023-05-29 13:30:09.000000 tailraiders-0.0.8/tailraiders/plunderer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:05:52.066364 tailraiders-0.0.8/tailraiders/protector/
+-rw-rw-rw-   0        0        0      235 2023-05-29 13:44:08.000000 tailraiders-0.0.8/tailraiders/protector/__init__.py
+-rw-rw-rw-   0        0        0     3789 2023-05-29 13:47:59.000000 tailraiders-0.0.8/tailraiders/protector/nan.py
+-rw-rw-rw-   0        0        0     5395 2023-05-29 13:51:30.000000 tailraiders-0.0.8/tailraiders/protector/prep.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:05:52.068364 tailraiders-0.0.8/tailraiders/trouper/
+-rw-rw-rw-   0        0        0      149 2023-05-29 13:44:18.000000 tailraiders-0.0.8/tailraiders/trouper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:05:52.042748 tailraiders-0.0.8/tailraiders.egg-info/
+-rw-rw-rw-   0        0        0      875 2023-05-29 14:05:51.000000 tailraiders-0.0.8/tailraiders.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      550 2023-05-29 14:05:51.000000 tailraiders-0.0.8/tailraiders.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 14:05:51.000000 tailraiders-0.0.8/tailraiders.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2023-05-29 14:05:51.000000 tailraiders-0.0.8/tailraiders.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-29 14:05:51.000000 tailraiders-0.0.8/tailraiders.egg-info/top_level.txt
```

### Comparing `tailraiders-0.0.7/PKG-INFO` & `tailraiders-0.0.8/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: tailraiders
-Version: 0.0.7
-Summary: A package for making Data Science easier, versions with 0.0.x are trials and tests
+Version: 0.0.8
+Summary: A package for making Data Science easier
 Author: Busse Heemskerk
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Tailraiders
 Tailraiders is a package currently **under development**. It is meant to be used for school and potentially later for Data Science. Modeled after the Tailraiders Alliance Factions, all subpackages are named after those.
 
 ## Installation
-You can install the package by using the following code:<br>
-**pip install tailraiders**
+You can install the package by using the following code:
+```
+pip install tailraiders
+```
+
+## New additions: Version 0.0.8
+- Nan now has a function renamed: df_from_file is now use_file
+- tailraiders.protector has the class Outliers, for checking skewness and dealing w outliers using IQR
+- All files now follow pep8 accordingly
 
-## New additions: Version 0.0.7
-- All functionalities can be imported from tailraiders, no need for calling the subpackages at this point in time
-- docstring function now has inputs
-- Plot now has an additional child-class: MeltPlot
-- Nan is moved to tailraiders.protector
-- Nan now has a function to read from csv-files: df_from_file
```

### Comparing `tailraiders-0.0.7/README.md` & `tailraiders-0.0.8/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Tailraiders
 Tailraiders is a package currently **under development**. It is meant to be used for school and potentially later for Data Science. Modeled after the Tailraiders Alliance Factions, all subpackages are named after those.
 
 ## Installation
-You can install the package by using the following code:<br>
-**pip install tailraiders**
+You can install the package by using the following code:
+```
+pip install tailraiders
+```
 
-## New additions: Version 0.0.7
-- All functionalities can be imported from tailraiders, no need for calling the subpackages at this point in time
-- docstring function now has inputs
-- Plot now has an additional child-class: MeltPlot
-- Nan is moved to tailraiders.protector
-- Nan now has a function to read from csv-files: df_from_file
+## New additions: Version 0.0.8
+- Nan now has a function renamed: df_from_file is now use_file
+- tailraiders.protector has the class Outliers, for checking skewness and dealing w outliers using IQR
+- All files now follow pep8 accordingly
```

### Comparing `tailraiders-0.0.7/setup.py` & `tailraiders-0.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     author = 'Busse Heemskerk',
-    description = 'A package for making Data Science easier, versions with 0.0.x are trials and tests',
+    description = 'A package for making Data Science easier',
     long_description = open('README.md').read(),
     long_description_content_type = 'text/markdown',
     name = 'tailraiders',
-    version = '0.0.7',
+    version = '0.0.8',
     packages = find_packages(include = ['tailraiders', 'tailraiders.*']),
     install_requires = ['pandas>=1.0',
                         'numpy>=1.0',
                         'matplotlib>=2.2.3',
-                        'seaborn>=0.9.0'],
+                        'seaborn>=0.9.0',
+                        'sklearn>=1.0.0'],
     python_requires = '>=2.7, !=3.0.*, !=3.1.*'
-    )
+    )
```

### Comparing `tailraiders-0.0.7/tailraiders/__init__.py` & `tailraiders-0.0.8/tailraiders/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 """
 Tailraiders
 =======================================
 
 The tailraiders package is made to help with general Data Sciency stuff.
 """
 
-#Checking if dependencies are installed, the dependencies of my libary are stored in the dependency_module value
+# Checking if dependencies are installed, the dependencies
+# of my libary are stored in the dependency_module value
 dependency_module = ['pandas',
-                    'numpy',
-                    'matplotlib',
-                    'seaborn']
+                     'numpy',
+                     'matplotlib',
+                     'seaborn',
+                     'sklearn']
 
-#For-loop to check for modules
+# For-loop to check for modules
 for module in dependency_module:
-    #Try to import modules
+    # Try to import modules
     try:
         __import__(module)
-    #Raise an error when it fails, telling them to install the failed module
+    # Raise an error when it fails, telling them to install the failed module
     except ImportError:
-        raise ImportError(f"The required package {module} was not found. Please install it.")
-    
-#Making it so you can, for certain parts, just import tailraiders
+        raise ImportError(f"The required package {module} \
+                            was not found. Please install it.")
+
+# Making it so you can, for certain parts, use from tailraiders import _blank_
 from tailraiders.boaboa.doc import docstring
 from tailraiders.gajalaka.plots import Plot, MeltPlot
-from tailraiders.protector.nan import Nan
+from tailraiders.protector.nan import Nan
+from tailraiders.protector.prep import Outliers
```

### Comparing `tailraiders-0.0.7/tailraiders/boaboa/doc.py` & `tailraiders-0.0.8/tailraiders/boaboa/doc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,57 +1,61 @@
-def docstring(amount_args = 1):
+def docstring(amount_args=1):
     """
-    Makes a docstring, dependend on what you put in. It will be formatted like this docstring.
+    Makes a docstring, dependend on what you put in.
+    It will be formatted like this docstring.
     When a enter is passed instead of an input, no text will be displayed.
     Default values should be passed by the argument type.
-    
+
     Parameters:
-    --------------------        
+    --------------------
     amount_args : int (default = 1)
         The amount of arguments used in the function
 
     Returns:
     --------------------
-    docstring : str 
+    docstring : str
         The docstring following the information given and following this format
     """
-    
-    #If-statement for checking the type passed for amount_args
+
+    # If-statement for checking the type passed for amount_args
     if isinstance(amount_args, int):
-        #Values are being made by using inputs
-        #input for summary of the function
+        # Values are being made by using inputs
+        # input for summary of the function
         summary = input("Write the summary of your function: ")
-        
-        #input for the arguments, making sure that x amount_args are being called and filled
+
+        # input for the arguments, making sure
+        # that x amount_args are being called and filled
         arguments = []
         argument_expl = []
         for x in range(1, amount_args + 1):
-            #input for arguments, type, default values and explanations
+            # input for arguments, type, default values and explanations
             arg = input(f"Write the name of parameter {x}: ")
             typ = input(f"Write the type of parameter {x}: ")
             default = input(f"Write the (default = x) of parameter {x}: ")
             typ_def = f'{typ} {default}'
             arguments.append((arg, typ_def))
             expl = input(f"Write the explanation of parameter {x}: ")
             argument_expl.append(expl)
-        
-        #input for return value name, type and explanation
+
+        # input for return value name, type and explanation
         return_name = input("Write the name of the returned value: ")
         return_type = input("Write the type of the returned value: ")
         return_expl = input("Write the explanation of the returned value: ")
-        
-        #Assembling the docstring
+
+        # Assembling the docstring
         doc = f'\n    """\n    {summary}\n\n'
         doc += '    Parameters:'
         doc += '\n    ' + '-' * 20 + '\n'
         for argument, explain in zip(arguments, argument_expl):
             doc += f'    {argument[0]} : {argument[1]}\n        {explain}\n\n'
         doc += '    Returns:'
         doc += '\n    ' + '-' * 20 + '\n'
         doc += f'    {return_name} : {return_type}\n        {return_expl}\n'
         doc += '    """'
 
         return print(doc)
-    
-    #Raises an error when amount_args != an integer
+
+    # Raises an error when amount_args != an integer
     else:
-        raise ValueError(f'The amount of arguments {amount_args} is not an integer, please refrain from trying non-integers')
+        raise ValueError(f'The amount of arguments {amount_args} \
+                         is not an integer, please refrain from \
+                         trying non-integers')
```

### Comparing `tailraiders-0.0.7/tailraiders/gajalaka/plots.py` & `tailraiders-0.0.8/tailraiders/gajalaka/plots.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 import seaborn as sns
 import matplotlib.pyplot as plt
 
+
 class Plot:
     """ Code for making catplots and relplots """
-    #Adding standard values for heigt, aspect and palette
+    # Adding standard values for heigt, aspect and palette
     PALETTE = "plasma"
     HEIGHT = 4
     ASPECT = 3
-    def __init__(self, df, xlim_low = None, xlim_high = None):
+
+    def __init__(self, df, xlim_low=None, xlim_high=None):
         self.data = df
         self._df = self.data
         self.xlim_low = xlim_low
         self.xlim_high = xlim_high
         sns.set_style('darkgrid')
 
-    def cat(self, x, y, hue = None, kind = 'bar'):
+    def cat(self, x, y, hue=None, kind='bar'):
         """
         A function to make a catplot, based on the dataframe used for Plot
 
         Parameters:
         --------------
         self :
             The given name of the class
 
         x : str
             Column name for x parameter
-        
+
         y : str
             Column name for y parameter
 
         hue : str (default = None)
             A column name for differentiating per category
 
         kind : str (default = 'bar')
@@ -37,38 +39,40 @@
                 strip, swarm, box, violin, boxen, point, bar and count
 
         Returns:
         --------------
         None :
             Instead it shows the plot for which the parameters are given
         """
-        
-        #try-except so it will show all columns if you use the wrong column
+
+        # try-except so it will show all columns if you use the wrong column
         try:
-            #making the catplot using seaborn and defining certain attributes
-            sns.catplot(data = self._df, x = x, y = y, palette = Plot.PALETTE, hue = hue, kind = kind,
-                   height = Plot.HEIGHT, aspect = Plot.ASPECT)
+            # making the catplot using seaborn and defining certain attributes
+            sns.catplot(data=self._df, x=x, y=y, palette=Plot.PALETTE,
+                        hue=hue, kind=kind, height=Plot.HEIGHT,
+                        aspect=Plot.ASPECT)
             plt.xlim(self.xlim_low, self.xlim_high)
-            plt.title(label = f'{kind}plot with x: {x} and y: {y}')
+            plt.title(label=f'{kind}plot with x: {x} and y: {y}')
             plt.show()
         except ValueError:
-            raise ValueError(f"Make sure x, y and hue are a column name. Check {[*self._df.columns]}")  
-     
-    def rel(self, x, y, hue = None, kind = 'scatter'):
+            raise ValueError(f"Make sure x, y and hue are \
+                             a column name. Check {[*self._df.columns]}")
+
+    def rel(self, x, y, hue=None, kind='scatter'):
         """
         A function to make a relplot, based on the dataframe used for Plot
 
         Parameters:
         --------------
         self :
             The given name of the class
 
         x : str
             Column name for x parameter
-        
+
         y : str
             Column name for y parameter
 
         hue : str (default = None)
             A column name for differentiating per category
 
         kind : str (default = 'bar')
@@ -76,101 +80,108 @@
                 strip, swarm, box, violin, boxen, point, bar and count
 
         Returns:
         --------------
         None :
             Instead it shows the plot for which the parameters are given
         """
-        
-        #try-except so it will show all columns if you use the wrong column
+
+        # try-except so it will show all columns if you use the wrong column
         try:
-            #making the relplot using seaborn and defining certain attributes
-            sns.relplot(data = self._df, x = x, y = y, palette = Plot.PALETTE, hue = hue, kind = kind,
-                    height = Plot.HEIGHT, aspect = Plot.ASPECT)
+            # making the relplot using seaborn and defining certain attributes
+            sns.relplot(data=self._df, x=x, y=y, palette=Plot.PALETTE,
+                        hue=hue, kind=kind,
+                        height=Plot.HEIGHT, aspect=Plot.ASPECT)
             plt.xlim(self.xlim_low, self.xlim_high)
-            plt.title(label = f'{kind}plot with x: {x} and y: {y}')
+            plt.title(label=f'{kind}plot with x: {x} and y: {y}')
             plt.show()
         except ValueError:
-            raise ValueError(f"Make sure x, y and hue are a column name. Check {[*self._df.columns]}") 
+            raise ValueError(f"Make sure x, y and hue are \
+                             a column name. Check {[*self._df.columns]}")
+
 
 class MeltPlot(Plot):
     """ A child-class that uses a melted dataframe to make visualisations """
-    def __init__(self, data, xlim_low = None, xlim_high = None):
+    def __init__(self, data, xlim_low=None, xlim_high=None):
         Plot.__init__(self, data, xlim_low, xlim_high)
-    
-    def cat(self, x, y, kind = 'bar'):
+
+    def cat(self, x, y, kind='bar'):
         """
         A function to make a catplot, based on the dataframe used for Plot
 
         Parameters:
         --------------
         self :
             The given name of the class
 
         x : str
             Column name for x parameter
-        
+
         y : str
             Column name for y parameter
 
         kind : str (default = 'bar')
             The kind of plot you want to make, options are:
                 strip, swarm, box, violin, boxen, point, bar and count
 
         Returns:
         --------------
         None :
             Instead it shows the plot for which the parameters are given
         """
 
-        #try-except so it will show all columns if you use the wrong column
+        # try-except so it will show all columns if you use the wrong column
         try:
-            #if-statement so that the function will work as the normal Plot.cat as well
+            # if-statement so that the function will work
+            # as the normal Plot.cat as well
             if type(x) is str:
-                Plot.cat(self, x, y, kind = kind) 
+                Plot.cat(self, x, y, kind=kind)
             else:
-                #making a melted df to use for Plot.cat
-                self._df = self.data[x + [y]].melt(id_vars = y) 
+                # making a melted df to use for Plot.cat
+                self._df = self.data[x + [y]].melt(id_vars=y)
                 hue = 'variable'
                 x = 'value'
                 Plot.cat(self, x, y, hue, kind)
         except KeyError:
-            raise KeyError(f"Make sure x, y and hue are a column name. Check {[*self._df.columns]}")
+            raise KeyError(f"Make sure x, y and hue are \
+                           a column name. Check {[*self._df.columns]}")
 
-    def rel(self, x, y, kind = 'scatter'):
+    def rel(self, x, y, kind='scatter'):
         """
         A function to make a relplot, based on the dataframe used for Plot
 
         Parameters:
         --------------
         self :
             The given name of the class
 
         x : str
             Column name for x parameter
-        
+
         y : str
             Column name for y parameter
 
         kind : str (default = 'scatter')
             The kind of plot you want to make, options are:
                 strip, swarm, box, violin, boxen, point, bar and count
 
         Returns:
         --------------
         None :
             Instead it shows the plot for which the parameters are given
         """
 
-        #try-except so it will show all columns if you use the wrong column
+        # try-except so it will show all columns if you use the wrong column
         try:
-            #if-statement so that the function will work as the normal Plot.rel as well
-            if type(x) is str:
-                Plot.rel(self, x, y, kind = kind)
+            # if-statement so that the function will work
+            # as the normal Plot.rel as well
+            if type(y) is str:
+                Plot.rel(self, x, y, kind=kind)
             else:
-                #making a melted df to use for Plot.rel
-                self._df = self.data[x + [y]].melt(id_vars = y) 
+                # making a melted df to use for Plot.rel
+                self._df = self.data[[x] + y].melt(id_vars=x)
                 hue = 'variable'
                 x = 'value'
                 Plot.rel(self, x, y, hue, kind)
         except KeyError:
-            raise KeyError(f"Make sure x, y and hue are a column name. Check {[*self._df.columns]}")
+            raise KeyError(f"Make sure x, y and hue are \
+                           a column name. Check {[*self._df.columns]}")
```

### Comparing `tailraiders-0.0.7/tailraiders/protector/nan.py` & `tailraiders-0.0.8/tailraiders/protector/nan.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,113 +1,125 @@
 import pandas as pd
 
+
 class Nan:
     """ Checks for NaN values and manipulate them """
     def __init__(self, df):
         self.df = df
         self.missing = df.isna().sum().to_frame()
         self.values = df.count().to_frame()
         self.rows = self.missing + self.values
         self.perc = round(self.missing / self.rows * 100, 2)
-        self.dfnan = pd.concat([self.missing, self.values, self.rows, self.perc], axis = 1)
-        self.dfnan.columns = ['total rows', 'rows with nan', 'rows without nan', 'perc nan']     
+        self.dfnan = pd.concat([self.missing, self.values,
+                                self.rows, self.perc], axis=1)
+        self.dfnan.columns = ['total rows', 'rows with nan',
+                              'rows without nan', 'perc nan']
 
-    def drop_cols(self, th = 20):
+    def drop_cols(self, th=20):
         """
         Drops columns based on a given threshold
 
         Parameters:
         ---------------
         self :
             The given name of the class
 
         th : int (default = 20)
-            The percentage threshold of when columns should be dropped
+            The percentage threshold of when
+            columns should be dropped
 
         Returns:
         ----------------
         None :
-            It makes it so that self.df is now edited to no longer has the dropped columns
+            It makes it so that self.df is now edited
+            to no longer has the dropped columns
         """
 
-        #making a temp df to see what columns go over the threshold
+        # making a temp df to see what columns go over the threshold
         self.nan_df = self.dfnan[self.dfnan['perc nan'] > th]
-        
-        #making a list from the index to use for drop
+
+        # making a list from the index to use for drop
         dropcols = list(self.nan_df.index)
         print(f'The columns {dropcols} are being dropped')
 
-        #dropping the columns in the list
-        self.df = self.df.drop(dropcols, axis = 1)
+        # dropping the columns in the list
+        self.df = self.df.drop(dropcols, axis=1)
         self.__init__(self.df)
-    
-    def fill_na(self, col, group, stat = 'mean'):
+
+    def fill_na(self, col, group, stat='mean'):
         """
-        Fills dataframe columns based on a given group and method
+        Fills dataframe columns based on
+        a given group and method
 
         Parameters:
         --------------
         self :
             The given name of the class
-        
+
         col : str
             The column name that will be filled
-        
+
         group : str
             Column name that will be used to group by
-        
+
         stat : str (default = 'mean')
             The stat on how people will be grouped
-            
+
         Returns:
         ----------------
         None :
-            It makes it so that self.df is now edited to no longer have the dropped columns
+            It makes it so that self.df is now edited
+            to no longer have the dropped columns
         """
 
-        #using fillna to fill the given column with given groupby column using the given method
-        self.df[col] = self.df[col].fillna(self.df.groupby(group)[col].transform(stat))
+        # using fillna to fill the given column with
+        # given groupby column using the given method
+        self.df[col] = self.df[col].fillna(self.df
+                                           .groupby(group)[col]
+                                           .transform(stat))
         self.__init__(self.df)
-        
-    def drop_na(self, axis = 0):
+
+    def drop_na(self, axis=0):
         """
         Drops columns based on the given axis
 
         Parameters:
         ---------------
         self :
             The given name of the class
 
         axis : int (default = 0)
-            Bool value, either 0 or 1. 0 is for rows and 1 is for columns
+            Bool value, either 0 or 1. 0 is
+            for rows and 1 is for columns
 
         Returns:
         ----------------
         None :
-            It makes it so that self.df is now edited to no longer have the dropped rows or columns
+            It makes it so that self.df is now edited
+            to no longer have the dropped rows or columns
         """
 
-        #dropna to drop rows or columns, based on given axis
-        self.df = self.df.dropna(axis = axis)
+        # dropna to drop rows or columns, based on given axis
+        self.df = self.df.dropna(axis=axis)
         self.__init__(self.df)
 
     @classmethod
-    def df_from_file(cls, file_path):
+    def use_file(cls, file_path):
         """
         A function to immediately convert files to be used for Nan
 
         Parameters
         --------------------
-        cls : 
+        cls :
             The class it is in (will not be filled in when using the function)
-        
+
         file_path : str
             The file_path to the file containing the data you want to use
 
         returns:
         --------------------
         cls(df) : pandas.Dataframe
             A pandas dataframe that is immediately used for Nan.__init__
         """
-        
+
         df = pd.read_csv(file_path)
-        return cls(df)
+        return cls(df)
```

### Comparing `tailraiders-0.0.7/tailraiders.egg-info/PKG-INFO` & `tailraiders-0.0.8/tailraiders.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: tailraiders
-Version: 0.0.7
-Summary: A package for making Data Science easier, versions with 0.0.x are trials and tests
+Version: 0.0.8
+Summary: A package for making Data Science easier
 Author: Busse Heemskerk
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Tailraiders
 Tailraiders is a package currently **under development**. It is meant to be used for school and potentially later for Data Science. Modeled after the Tailraiders Alliance Factions, all subpackages are named after those.
 
 ## Installation
-You can install the package by using the following code:<br>
-**pip install tailraiders**
+You can install the package by using the following code:
+```
+pip install tailraiders
+```
+
+## New additions: Version 0.0.8
+- Nan now has a function renamed: df_from_file is now use_file
+- tailraiders.protector has the class Outliers, for checking skewness and dealing w outliers using IQR
+- All files now follow pep8 accordingly
 
-## New additions: Version 0.0.7
-- All functionalities can be imported from tailraiders, no need for calling the subpackages at this point in time
-- docstring function now has inputs
-- Plot now has an additional child-class: MeltPlot
-- Nan is moved to tailraiders.protector
-- Nan now has a function to read from csv-files: df_from_file
```

### Comparing `tailraiders-0.0.7/tailraiders.egg-info/SOURCES.txt` & `tailraiders-0.0.8/tailraiders.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -12,8 +12,9 @@
 tailraiders/boaboa/doc.py
 tailraiders/bugtrapper/__init__.py
 tailraiders/gajalaka/__init__.py
 tailraiders/gajalaka/plots.py
 tailraiders/plunderer/__init__.py
 tailraiders/protector/__init__.py
 tailraiders/protector/nan.py
+tailraiders/protector/prep.py
 tailraiders/trouper/__init__.py
```

