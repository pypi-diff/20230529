# Comparing `tmp/bioumlsim-0.2.4.tar.gz` & `tmp/bioumlsim-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioumlsim-0.2.4.tar", last modified: Fri May 26 10:53:54 2023, max compression
+gzip compressed data, was "bioumlsim-0.3.0.tar", last modified: Mon May 29 18:39:02 2023, max compression
```

## Comparing `bioumlsim-0.2.4.tar` & `bioumlsim-0.3.0.tar`

### file list

```diff
@@ -1,40 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 10:53:54.301473 bioumlsim-0.2.4/
--rw-rw-rw-   0        0        0     1088 2023-05-17 07:27:39.000000 bioumlsim-0.2.4/LICENSE
--rw-rw-rw-   0        0        0       18 2023-05-26 09:58:37.000000 bioumlsim-0.2.4/MANIFEST.in
--rw-rw-rw-   0        0        0      771 2023-05-26 10:53:54.302476 bioumlsim-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0       60 2023-05-17 07:27:39.000000 bioumlsim-0.2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 10:53:54.266592 bioumlsim-0.2.4/java/
--rw-rw-rw-   0        0        0   386547 2023-05-26 08:30:49.000000 bioumlsim-0.2.4/java/biouml.plugins.sbml_0.9.10.jar
--rw-rw-rw-   0        0        0   615951 2023-05-26 08:30:49.000000 bioumlsim-0.2.4/java/biouml.plugins.simulation_0.9.10.jar
--rw-rw-rw-   0        0        0  2085692 2023-05-26 08:30:49.000000 bioumlsim-0.2.4/java/biouml.workbench_0.9.10.jar
--rw-rw-rw-   0        0        0   581945 2023-05-26 08:30:49.000000 bioumlsim-0.2.4/java/colt.jar
--rw-rw-rw-   0        0        0   396595 2023-05-26 08:30:49.000000 bioumlsim-0.2.4/java/com.developmentontheedge.beans-3.0.4.jar
--rw-rw-rw-   0        0        0    94331 2023-05-26 08:30:48.000000 bioumlsim-0.2.4/java/com.developmentontheedge.util_0.9.10.jar
--rw-rw-rw-   0        0        0    31222 2023-05-26 08:30:49.000000 bioumlsim-0.2.4/java/com.eclipsesource.json_0.9.4.jar
--rw-rw-rw-   0        0        0   575606 2023-05-26 08:30:49.000000 bioumlsim-0.2.4/java/org.apache.commons.collections_3.2.1.jar
--rw-rw-rw-   0        0        0   262026 2023-05-26 08:30:48.000000 bioumlsim-0.2.4/java/org.apache.commons.lang_2.4.0.jar
--rw-rw-rw-   0        0        0   421287 2023-05-26 08:30:49.000000 bioumlsim-0.2.4/java/org.apache.velocity_1.6.2.jar
--rw-rw-rw-   0        0        0    58013 2023-05-26 08:30:48.000000 bioumlsim-0.2.4/java/org.json-20170516.jar
--rw-rw-rw-   0        0        0  1251757 2023-05-26 08:30:49.000000 bioumlsim-0.2.4/java/ru.biosoft.access_0.9.10.jar
--rw-rw-rw-   0        0        0    14541 2023-05-26 08:30:49.000000 bioumlsim-0.2.4/java/ru.biosoft.exception-1.0.0.jar
--rw-rw-rw-   0        0        0   231950 2023-05-26 08:30:48.000000 bioumlsim-0.2.4/java/ru.biosoft.graph_0.9.10.jar
--rw-rw-rw-   0        0        0   197773 2023-05-26 08:30:48.000000 bioumlsim-0.2.4/java/ru.biosoft.graphics_0.9.10.jar
--rw-rw-rw-   0        0        0    26578 2023-05-26 08:30:49.000000 bioumlsim-0.2.4/java/ru.biosoft.jobcontrol-2.0.0.jar
--rw-rw-rw-   0        0        0   163699 2023-05-26 08:30:48.000000 bioumlsim-0.2.4/java/ru.biosoft.math_0.9.10.jar
--rw-rw-rw-   0        0        0    20343 2023-05-26 08:30:49.000000 bioumlsim-0.2.4/java/src.jar
--rw-rw-rw-   0        0        0   299064 2023-05-26 08:30:49.000000 bioumlsim-0.2.4/java/streamex-0.7.0.jar
--rw-rw-rw-   0        0        0      185 2023-05-17 10:21:02.000000 bioumlsim-0.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       55 2023-05-17 13:19:23.000000 bioumlsim-0.2.4/requirements_dev.txt
--rw-rw-rw-   0        0        0      827 2023-05-26 10:53:54.314716 bioumlsim-0.2.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-26 10:53:54.272593 bioumlsim-0.2.4/src/
--rw-rw-rw-   0        0        0        0 2023-05-17 07:30:52.000000 bioumlsim-0.2.4/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 10:53:54.300477 bioumlsim-0.2.4/src/bioumlsim.egg-info/
--rw-rw-rw-   0        0        0      771 2023-05-26 10:53:54.000000 bioumlsim-0.2.4/src/bioumlsim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      996 2023-05-26 10:53:54.000000 bioumlsim-0.2.4/src/bioumlsim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 10:53:54.000000 bioumlsim-0.2.4/src/bioumlsim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-17 10:19:31.000000 bioumlsim-0.2.4/src/bioumlsim.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       20 2023-05-26 10:53:54.000000 bioumlsim-0.2.4/src/bioumlsim.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-05-26 10:53:54.000000 bioumlsim-0.2.4/src/bioumlsim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2909 2023-05-26 08:34:47.000000 bioumlsim-0.2.4/src/bioumlsim.py
--rw-rw-rw-   0        0        0      390 2023-05-22 19:11:01.000000 bioumlsim-0.2.4/src/test.py
--rw-rw-rw-   0        0        0        3 2023-05-26 09:41:30.000000 bioumlsim-0.2.4/text.txt
+drwxrwxrwx   0        0        0        0 2023-05-29 18:39:02.700861 bioumlsim-0.3.0/
+-rw-rw-rw-   0        0        0     1088 2023-05-17 07:27:39.000000 bioumlsim-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0      771 2023-05-29 18:39:02.701862 bioumlsim-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0       60 2023-05-17 07:27:39.000000 bioumlsim-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 18:39:02.627863 bioumlsim-0.3.0/bioumlsim/
+-rw-rw-rw-   0        0        0     2995 2023-05-29 18:25:05.000000 bioumlsim-0.3.0/bioumlsim/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 18:39:02.698866 bioumlsim-0.3.0/bioumlsim/jars/
+-rw-rw-rw-   0        0        0   386547 2023-05-26 08:30:49.000000 bioumlsim-0.3.0/bioumlsim/jars/biouml.plugins.sbml_0.9.10.jar
+-rw-rw-rw-   0        0        0   615951 2023-05-26 08:30:49.000000 bioumlsim-0.3.0/bioumlsim/jars/biouml.plugins.simulation_0.9.10.jar
+-rw-rw-rw-   0        0        0  2085692 2023-05-26 08:30:49.000000 bioumlsim-0.3.0/bioumlsim/jars/biouml.workbench_0.9.10.jar
+-rw-rw-rw-   0        0        0   581945 2023-05-26 08:30:49.000000 bioumlsim-0.3.0/bioumlsim/jars/colt.jar
+-rw-rw-rw-   0        0        0   396595 2023-05-26 08:30:49.000000 bioumlsim-0.3.0/bioumlsim/jars/com.developmentontheedge.beans-3.0.4.jar
+-rw-rw-rw-   0        0        0    94331 2023-05-26 08:30:48.000000 bioumlsim-0.3.0/bioumlsim/jars/com.developmentontheedge.util_0.9.10.jar
+-rw-rw-rw-   0        0        0    31222 2023-05-26 08:30:49.000000 bioumlsim-0.3.0/bioumlsim/jars/com.eclipsesource.json_0.9.4.jar
+-rw-rw-rw-   0        0        0   575606 2023-05-26 08:30:49.000000 bioumlsim-0.3.0/bioumlsim/jars/org.apache.commons.collections_3.2.1.jar
+-rw-rw-rw-   0        0        0   262026 2023-05-26 08:30:48.000000 bioumlsim-0.3.0/bioumlsim/jars/org.apache.commons.lang_2.4.0.jar
+-rw-rw-rw-   0        0        0   421287 2023-05-26 08:30:49.000000 bioumlsim-0.3.0/bioumlsim/jars/org.apache.velocity_1.6.2.jar
+-rw-rw-rw-   0        0        0    58013 2023-05-26 08:30:48.000000 bioumlsim-0.3.0/bioumlsim/jars/org.json-20170516.jar
+-rw-rw-rw-   0        0        0  1251757 2023-05-26 08:30:49.000000 bioumlsim-0.3.0/bioumlsim/jars/ru.biosoft.access_0.9.10.jar
+-rw-rw-rw-   0        0        0    14541 2023-05-26 08:30:49.000000 bioumlsim-0.3.0/bioumlsim/jars/ru.biosoft.exception-1.0.0.jar
+-rw-rw-rw-   0        0        0   231950 2023-05-26 08:30:48.000000 bioumlsim-0.3.0/bioumlsim/jars/ru.biosoft.graph_0.9.10.jar
+-rw-rw-rw-   0        0        0   197773 2023-05-26 08:30:48.000000 bioumlsim-0.3.0/bioumlsim/jars/ru.biosoft.graphics_0.9.10.jar
+-rw-rw-rw-   0        0        0    26578 2023-05-26 08:30:49.000000 bioumlsim-0.3.0/bioumlsim/jars/ru.biosoft.jobcontrol-2.0.0.jar
+-rw-rw-rw-   0        0        0   163699 2023-05-26 08:30:48.000000 bioumlsim-0.3.0/bioumlsim/jars/ru.biosoft.math_0.9.10.jar
+-rw-rw-rw-   0        0        0    20343 2023-05-26 08:30:49.000000 bioumlsim-0.3.0/bioumlsim/jars/src.jar
+-rw-rw-rw-   0        0        0   299064 2023-05-26 08:30:49.000000 bioumlsim-0.3.0/bioumlsim/jars/streamex-0.7.0.jar
+-rw-rw-rw-   0        0        0      390 2023-05-22 19:11:01.000000 bioumlsim-0.3.0/bioumlsim/test.py
+drwxrwxrwx   0        0        0        0 2023-05-29 18:39:02.647864 bioumlsim-0.3.0/bioumlsim.egg-info/
+-rw-rw-rw-   0        0        0      771 2023-05-29 18:39:02.000000 bioumlsim-0.3.0/bioumlsim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1083 2023-05-29 18:39:02.000000 bioumlsim-0.3.0/bioumlsim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 18:39:02.000000 bioumlsim-0.3.0/bioumlsim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-29 18:17:58.000000 bioumlsim-0.3.0/bioumlsim.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       10 2023-05-29 18:39:02.000000 bioumlsim-0.3.0/bioumlsim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      185 2023-05-27 18:48:00.000000 bioumlsim-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0      863 2023-05-29 18:39:02.703863 bioumlsim-0.3.0/setup.cfg
```

### Comparing `bioumlsim-0.2.4/LICENSE` & `bioumlsim-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.2.4/PKG-INFO` & `bioumlsim-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: bioumlsim
-Version: 0.2.4
+Version: 0.3.0
 Summary: Python interface for simulation with BioUML
 Home-page: https://www.biouml.org/
 Author: Ilya Kiselev, Biosoft.ru
 Author-email: 4x3cut0r@gmail.com
 Project-URL: Bug Tracker, https://github.com/Biosoft-ru/bioumlsim/issues
 Project-URL: Source Code, https://github.com/Biosoft-ru/bioumlsim
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Mathematics
-Requires-Python: >=3.8
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # bioumlsim
 Python interface to BioUML numeric simulators
```

### Comparing `bioumlsim-0.2.4/java/biouml.plugins.sbml_0.9.10.jar` & `bioumlsim-0.3.0/bioumlsim/jars/biouml.plugins.sbml_0.9.10.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.2.4/java/biouml.plugins.simulation_0.9.10.jar` & `bioumlsim-0.3.0/bioumlsim/jars/biouml.plugins.simulation_0.9.10.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.2.4/java/biouml.workbench_0.9.10.jar` & `bioumlsim-0.3.0/bioumlsim/jars/biouml.workbench_0.9.10.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.2.4/java/colt.jar` & `bioumlsim-0.3.0/bioumlsim/jars/colt.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.2.4/java/com.developmentontheedge.beans-3.0.4.jar` & `bioumlsim-0.3.0/bioumlsim/jars/com.developmentontheedge.beans-3.0.4.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.2.4/java/com.developmentontheedge.util_0.9.10.jar` & `bioumlsim-0.3.0/bioumlsim/jars/com.developmentontheedge.util_0.9.10.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.2.4/java/com.eclipsesource.json_0.9.4.jar` & `bioumlsim-0.3.0/bioumlsim/jars/com.eclipsesource.json_0.9.4.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.2.4/java/org.apache.commons.collections_3.2.1.jar` & `bioumlsim-0.3.0/bioumlsim/jars/org.apache.commons.collections_3.2.1.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.2.4/java/org.apache.commons.lang_2.4.0.jar` & `bioumlsim-0.3.0/bioumlsim/jars/org.apache.commons.lang_2.4.0.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.2.4/java/org.apache.velocity_1.6.2.jar` & `bioumlsim-0.3.0/bioumlsim/jars/org.apache.velocity_1.6.2.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.2.4/java/org.json-20170516.jar` & `bioumlsim-0.3.0/bioumlsim/jars/org.json-20170516.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.2.4/java/ru.biosoft.access_0.9.10.jar` & `bioumlsim-0.3.0/bioumlsim/jars/ru.biosoft.access_0.9.10.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.2.4/java/ru.biosoft.exception-1.0.0.jar` & `bioumlsim-0.3.0/bioumlsim/jars/ru.biosoft.exception-1.0.0.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.2.4/java/ru.biosoft.graph_0.9.10.jar` & `bioumlsim-0.3.0/bioumlsim/jars/ru.biosoft.graph_0.9.10.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.2.4/java/ru.biosoft.graphics_0.9.10.jar` & `bioumlsim-0.3.0/bioumlsim/jars/ru.biosoft.graphics_0.9.10.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.2.4/java/ru.biosoft.jobcontrol-2.0.0.jar` & `bioumlsim-0.3.0/bioumlsim/jars/ru.biosoft.jobcontrol-2.0.0.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.2.4/java/ru.biosoft.math_0.9.10.jar` & `bioumlsim-0.3.0/bioumlsim/jars/ru.biosoft.math_0.9.10.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.2.4/java/src.jar` & `bioumlsim-0.3.0/bioumlsim/jars/src.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.2.4/java/streamex-0.7.0.jar` & `bioumlsim-0.3.0/bioumlsim/jars/streamex-0.7.0.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.2.4/src/bioumlsim.egg-info/PKG-INFO` & `bioumlsim-0.3.0/bioumlsim.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: bioumlsim
-Version: 0.2.4
+Version: 0.3.0
 Summary: Python interface for simulation with BioUML
 Home-page: https://www.biouml.org/
 Author: Ilya Kiselev, Biosoft.ru
 Author-email: 4x3cut0r@gmail.com
 Project-URL: Bug Tracker, https://github.com/Biosoft-ru/bioumlsim/issues
 Project-URL: Source Code, https://github.com/Biosoft-ru/bioumlsim
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Mathematics
-Requires-Python: >=3.8
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # bioumlsim
 Python interface to BioUML numeric simulators
```

### Comparing `bioumlsim-0.2.4/src/bioumlsim.py` & `bioumlsim-0.3.0/bioumlsim/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import jpype
 import jpype.imports
-import numpy
+import numpy as np
+import pandas as pd
 import os
 
 class BioUMLSim:
     
     bioUMLPath = None
     atol = 1E-8
     rtol = 1E-8
     engine = None
 
-    def __init__(self, path = 'C:/lib'):
+    def __init__(self):
+        path = os.path.dirname(__file__)+'/jars'
         self.bioUMLPath = path
         print("JVM is starting up")
         jpype.startJVM(classpath=[path+'/*'], convertStrings=True)
-        path = os.path.abspath(__file__)
-        print(path)
         
     def load(self, file):
         """
         Loads SBML file and transforms it into object which represents mathematical model.
         Args:
             file (str): path to file
         Returns:
@@ -57,34 +57,35 @@
     
 class Result:
     
     def __init__(self, sr, engine):
         self.sr = sr
         self.engine = engine
         species = engine.getFloatingSpecies()
-        self.values = numpy.array(sr.getValuesTransposed(species))
-        self.names = numpy.array(species)
-        self.times = numpy.array(sr.getTimes());
+        self.values = np.array(sr.getValuesTransposed(species))
+        self.names = np.array(species)
+        self.times = np.array(sr.getTimes());
+        self.df = pd.DataFrame(self.values, columns = self.names, index = pd.Index(self.times, name ="Time"))
         
     def toFile(self, file, precision=3, separator ='\t'):
         f = open(file, 'w')
-        f.write(numpy.array2string(self.names, separator=separator)[1:-1])
+        f.write(np.array2string(self.names, separator=separator)[1:-1])
         f.write('\n')
         for row in self.values:
-            f.write(numpy.array2string(row, precision=precision, separator=separator)[1:-1])
+            f.write(np.array2string(row, precision=precision, separator=separator)[1:-1])
             f.write('\n')
         f.close()
     
     def __str__(self):
-        return str(self.values)
+        return str(self.df)
     
     def getTimes(self):
         return self.times
     
     def getNames(self):
         return self.names
         
     def getValues(self, variable=None):
         if (variable!=None):
-            return numpy.array(self.sr.getValues(variable))
+            return np.array(self.sr.getValues(variable))
         else:
             return self.values
```

