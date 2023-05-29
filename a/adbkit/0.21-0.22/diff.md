# Comparing `tmp/adbkit-0.21.tar.gz` & `tmp/adbkit-0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adbkit-0.21.tar", last modified: Mon May 29 02:00:26 2023, max compression
+gzip compressed data, was "adbkit-0.22.tar", last modified: Mon May 29 02:08:30 2023, max compression
```

## Comparing `adbkit-0.21.tar` & `adbkit-0.22.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 02:00:26.016328 adbkit-0.21/
--rw-rw-rw-   0        0        0     1148 2023-05-29 01:59:52.000000 adbkit-0.21/LICENSE.rst
--rw-rw-rw-   0        0        0       89 2023-05-29 01:59:52.000000 adbkit-0.21/MANIFEST.in
--rw-rw-rw-   0        0        0   161921 2023-05-29 02:00:26.017290 adbkit-0.21/PKG-INFO
--rw-rw-rw-   0        0        0   160268 2023-05-28 22:13:52.000000 adbkit-0.21/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 02:00:26.012304 adbkit-0.21/adbkit/
--rw-rw-rw-   0        0        0   160268 2023-05-28 22:13:52.000000 adbkit-0.21/adbkit/README.MD
--rw-rw-rw-   0        0        0   130248 2023-05-29 00:06:17.000000 adbkit-0.21/adbkit/__init__.py
--rw-rw-rw-   0        0        0      696 2023-05-29 02:00:25.000000 adbkit-0.21/adbkit/requirements.txt
--rw-rw-rw-   0        0        0   284867 2023-05-29 02:00:25.000000 adbkit-0.21/adbkit/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-05-29 02:00:26.015324 adbkit-0.21/adbkit.egg-info/
--rw-rw-rw-   0        0        0   161921 2023-05-29 02:00:25.000000 adbkit-0.21/adbkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-05-29 02:00:25.000000 adbkit-0.21/adbkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 02:00:25.000000 adbkit-0.21/adbkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      660 2023-05-29 02:00:25.000000 adbkit-0.21/adbkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-29 02:00:25.000000 adbkit-0.21/adbkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-05-29 02:00:26.017290 adbkit-0.21/setup.cfg
--rw-rw-rw-   0        0        0     2803 2023-05-29 02:00:25.000000 adbkit-0.21/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 02:08:30.841754 adbkit-0.22/
+-rw-rw-rw-   0        0        0     1148 2023-05-29 02:07:59.000000 adbkit-0.22/LICENSE.rst
+-rw-rw-rw-   0        0        0       89 2023-05-29 02:07:58.000000 adbkit-0.22/MANIFEST.in
+-rw-rw-rw-   0        0        0   162034 2023-05-29 02:08:30.842752 adbkit-0.22/PKG-INFO
+-rw-rw-rw-   0        0        0   160379 2023-05-29 02:07:42.000000 adbkit-0.22/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 02:08:30.838761 adbkit-0.22/adbkit/
+-rw-rw-rw-   0        0        0   160379 2023-05-29 02:07:42.000000 adbkit-0.22/adbkit/README.MD
+-rw-rw-rw-   0        0        0   130248 2023-05-29 00:06:17.000000 adbkit-0.22/adbkit/__init__.py
+-rw-rw-rw-   0        0        0      696 2023-05-29 02:08:30.000000 adbkit-0.22/adbkit/requirements.txt
+-rw-rw-rw-   0        0        0   284867 2023-05-29 02:08:30.000000 adbkit-0.22/adbkit/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-05-29 02:08:30.841754 adbkit-0.22/adbkit.egg-info/
+-rw-rw-rw-   0        0        0   162034 2023-05-29 02:08:30.000000 adbkit-0.22/adbkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-05-29 02:08:30.000000 adbkit-0.22/adbkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 02:08:30.000000 adbkit-0.22/adbkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      660 2023-05-29 02:08:30.000000 adbkit-0.22/adbkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-29 02:08:30.000000 adbkit-0.22/adbkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-05-29 02:08:30.843748 adbkit-0.22/setup.cfg
+-rw-rw-rw-   0        0        0     2803 2023-05-29 02:08:30.000000 adbkit-0.22/setup.py
```

### Comparing `adbkit-0.21/LICENSE.rst` & `adbkit-0.22/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `adbkit-0.21/PKG-INFO` & `adbkit-0.22/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adbkit
-Version: 0.21
+Version: 0.22
 Summary: Big automation package for ADB
 Home-page: https://github.com/hansalemaos/adbkit
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: adb,android,automation,shell,root
 Classifier: Development Status :: 4 - Beta
@@ -19,14 +19,16 @@
 # Easier ADB automation 
 
 ## Tested against Windows 10, Python 3.9.13, BlueStacks 5.9.300.1014 N32
 ### Cygwin is necessary: https://www.cygwin.com/setup-x86_64.exe and needs to be added to the path variable!
 
 ### pip install adbkit
 
+#### If you are using Python 3.10 and get and Exception due to requests, execute pip install requests==2.31.0
+
 **Don't get confused about the instance "self". I did it because it is faster copying methods from the class :)** 
 
 **28/05/2023: Added fast screenshots with scrcpy - no root required and some other methods** 
 
 ```python
 from adbkit import ADBTools
 from kthread_sleep import sleep
```

### Comparing `adbkit-0.21/README.md` & `adbkit-0.22/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # Easier ADB automation 
 
 ## Tested against Windows 10, Python 3.9.13, BlueStacks 5.9.300.1014 N32
 ### Cygwin is necessary: https://www.cygwin.com/setup-x86_64.exe and needs to be added to the path variable!
 
 ### pip install adbkit
 
+#### If you are using Python 3.10 and get and Exception due to requests, execute pip install requests==2.31.0
+
 **Don't get confused about the instance "self". I did it because it is faster copying methods from the class :)** 
 
 **28/05/2023: Added fast screenshots with scrcpy - no root required and some other methods** 
 
 ```python
 from adbkit import ADBTools
 from kthread_sleep import sleep
```

### Comparing `adbkit-0.21/adbkit/README.MD` & `adbkit-0.22/adbkit/README.MD`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # Easier ADB automation 
 
 ## Tested against Windows 10, Python 3.9.13, BlueStacks 5.9.300.1014 N32
 ### Cygwin is necessary: https://www.cygwin.com/setup-x86_64.exe and needs to be added to the path variable!
 
 ### pip install adbkit
 
+#### If you are using Python 3.10 and get and Exception due to requests, execute pip install requests==2.31.0
+
 **Don't get confused about the instance "self". I did it because it is faster copying methods from the class :)** 
 
 **28/05/2023: Added fast screenshots with scrcpy - no root required and some other methods** 
 
 ```python
 from adbkit import ADBTools
 from kthread_sleep import sleep
```

### Comparing `adbkit-0.21/adbkit/__init__.py` & `adbkit-0.22/adbkit/__init__.py`

 * *Files identical despite different names*

### Comparing `adbkit-0.21/adbkit/requirements.txt` & `adbkit-0.22/adbkit/requirements.txt`

 * *Files identical despite different names*

### Comparing `adbkit-0.21/adbkit/thirdparty.json` & `adbkit-0.22/adbkit/thirdparty.json`

 * *Files identical despite different names*

### Comparing `adbkit-0.21/adbkit.egg-info/PKG-INFO` & `adbkit-0.22/adbkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adbkit
-Version: 0.21
+Version: 0.22
 Summary: Big automation package for ADB
 Home-page: https://github.com/hansalemaos/adbkit
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: adb,android,automation,shell,root
 Classifier: Development Status :: 4 - Beta
@@ -19,14 +19,16 @@
 # Easier ADB automation 
 
 ## Tested against Windows 10, Python 3.9.13, BlueStacks 5.9.300.1014 N32
 ### Cygwin is necessary: https://www.cygwin.com/setup-x86_64.exe and needs to be added to the path variable!
 
 ### pip install adbkit
 
+#### If you are using Python 3.10 and get and Exception due to requests, execute pip install requests==2.31.0
+
 **Don't get confused about the instance "self". I did it because it is faster copying methods from the class :)** 
 
 **28/05/2023: Added fast screenshots with scrcpy - no root required and some other methods** 
 
 ```python
 from adbkit import ADBTools
 from kthread_sleep import sleep
```

### Comparing `adbkit-0.21/adbkit.egg-info/requires.txt` & `adbkit-0.22/adbkit.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `adbkit-0.21/setup.py` & `adbkit-0.22/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 #long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.21'''
+VERSION = '''0.22'''
 DESCRIPTION = '''Big automation package for ADB'''
 
 # Setting up
 setup(
     name="adbkit",
     version=VERSION,
     license='MIT',
```

