# Comparing `tmp/coffeefetch-1.0.0.tar.gz` & `tmp/coffeefetch-1.1.0.tar.gz`

## Comparing `coffeefetch-1.0.0.tar` & `coffeefetch-1.1.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 coffeefetch-1.0.0/requirements.txt
--rw-r--r--   0        0        0     5499 2020-02-02 00:00:00.000000 coffeefetch-1.0.0/src/coffeefetch/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 coffeefetch-1.0.0/src/coffeefetch/__main__.py
--rw-r--r--   0        0        0     5499 2020-02-02 00:00:00.000000 coffeefetch-1.0.0/src/coffeefetch/coffeefetch.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 coffeefetch-1.0.0/LICENCE
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 coffeefetch-1.0.0/README.md
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 coffeefetch-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 coffeefetch-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 coffeefetch-1.1.0/requirements.txt
+-rw-r--r--   0        0        0     6324 2020-02-02 00:00:00.000000 coffeefetch-1.1.0/src/coffeefetch/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 coffeefetch-1.1.0/src/coffeefetch/__main__.py
+-rw-r--r--   0        0        0     6316 2020-02-02 00:00:00.000000 coffeefetch-1.1.0/src/coffeefetch/coffeefetch.py
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 coffeefetch-1.1.0/src/coffeefetch/quotes/quotes.txt
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 coffeefetch-1.1.0/LICENCE
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 coffeefetch-1.1.0/README.md
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 coffeefetch-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 coffeefetch-1.1.0/PKG-INFO
```

### Comparing `coffeefetch-1.0.0/src/coffeefetch/__init__.py` & `coffeefetch-1.1.0/src/coffeefetch/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # TTY system information grabber, written in Python
 # Built to run on Unix-like systems, but may function on other systems
-# Written and tested by Logan Allen, 2023
+# Written and tested by Logan Allen, 2023, quotes written at http://www.yaldex.com/
 # PLEASE REPORT ANY ISSUES TO THE GITHUB REPOSITORY!!! www.github.com/TeaPixl
 from socket import gethostname, gethostbyname
 from platform import machine, system, processor, release
 from datetime import datetime
 import psutil
 import logging
 import sys
 import time
 import getpass
 import shutil
+import random
+import os
 
 cupImage= """                                                                                       
                                       ██    ██    ██                                    
                                     ██      ██  ██                                      
                                     ██    ██    ██                                      
                                       ██  ██      ██                                    
                                       ██    ██    ██                                    
@@ -24,33 +26,55 @@
                                   ██                ██  ██                              
                                   ██                ██  ██                              
                                   ██                ██████                              
                                     ██            ██                                    
                                 ████████████████████████                                
                                 ██                    ██                                
                                   ████████████████████"""
-                                     
+
+# randomly pick from a list of random quotes
+def quoteGen():
+    try:
+         path = os.path.dirname(__file__)
+         realPath = "quotes/quotes.txt"
+         location = os.path.join(path, realPath)
+         with open(location, 'r') as f:
+             quotes = [] # all quotes in list, randomly pick 1 out of 20
+             text = f.readlines()
+             quotes.append(text)
+             chosen = random.choice(text)
+             print("\n                             " + chosen)
+    except Exception as e:
+        logging.exception(e)
+        print("\nQuoteGen failed... Proceeding.")
+        pass
+
 def spinningCursor(): # shows the script is running, dosent actually mean anything :/
-    while True:
-        for cursor in "|/-\\":
-            yield cursor
+    try:
+        while True:
+            for cursor in "|/-\\":
+                yield cursor
+    except Exception as e:
+        logging.exception(e)
+        print("spinningCursor failed... Proceeding.")
 
 def currentUser(): #current user logged in
     user = getpass.getuser()
     print("Hello, " + user)
     
 def getTime():
     try:
         now = datetime.now()
         current_time = now.strftime("%H:%M:%S")
         print("It is: "+ current_time)
     except Exception as e:
         logging.exception(e)
-        print("\nSomething's wrong, Unable to display the current time")
-
+        print("\nSomething's wrong, Unable to display the current time.")
+        exit()
+        
 # display the system uptime in a readable format
 def bootTime():
     return time.time() - psutil.boot_time()
 
 boot = bootTime()/60
 approxBoot = round(boot, 1)
 
@@ -64,28 +88,28 @@
     totalDisk = round(total, 1)
     used = int(info[1]) / (1024 * 1024 * 1024) # total used space
     usedDisk = round(used, 1)
     fraction = (usedDisk / totalDisk) *100
     newFraction = str(round(fraction, 1))
 except Exception as e:
     logging.exception(e)
-    print("\nSomething went wrong while trying to access your disk... Proceeding.")
-    pass
+    print("\nSomething went wrong while trying to access your disk.")
+    exit()
 
 # get CPU frequency
 try:
     data = []
     cpuData = psutil.cpu_freq() # tuple with (current, min, max)
     data = list(cpuData)
     floatFreq = int(data[0])/1000 #convert MHz to GHz
     freq = str(round(floatFreq, 2))
 except Exception as e:
     logging.exception(e)
-    print("\nSomething went wrong while trying to access your CPU info.... Proceeding.")
-    pass
+    print("\nSomething went wrong while trying to access your CPU info.")
+    exit()
 
 def infoGrabber():
     try:
         data = [] # data fills this list from 0-6
         data.append(str(system())) # OS
         data.append(str(release())) # version
         data.append(str(machine())) # architecture
@@ -98,14 +122,15 @@
         spinner = spinningCursor()
         for _ in range(7):
             sys.stdout.write(next(spinner))
             sys.stdout.flush()
             time.sleep(0.1)
             sys.stdout.write('\b')
         print(cupImage)
+        quoteGen()
         currentUser()
         getTime()
         print("*------------------------------*") # display the data
         print("OS: "+ data[0])
         print("VERSION: "+ data[1])
         print("CPU: "+ data[5] + " ("+ freq + " GHz)")
         print("ARCHITECTURE: "+ data[2])
@@ -114,8 +139,9 @@
         print("IP: "+ data[4])
         print("RAM: "+ newUsage + "% used / " + data[6] + " total")
         print("DISK:", newFraction + "% used / "+ str(totalDisk) +" GB total")
         print("*------------------------------*")
     except Exception as e:
         logging.exception(e)
         print("\nSomething has failed, please check for any issues!!!")
+        exit()
```

### Comparing `coffeefetch-1.0.0/src/coffeefetch/coffeefetch.py` & `coffeefetch-1.1.0/src/coffeefetch/coffeefetch.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # TTY system information grabber, written in Python
 # Built to run on Unix-like systems, but may function on other systems
-# Written and tested by Logan Allen, 2023
+# Written and tested by Logan Allen, 2023, quotes written at http://www.yaldex.com/
 # PLEASE REPORT ANY ISSUES TO THE GITHUB REPOSITORY!!! www.github.com/TeaPixl
 from socket import gethostname, gethostbyname
 from platform import machine, system, processor, release
 from datetime import datetime
 import psutil
 import logging
 import sys
 import time
 import getpass
 import shutil
+import random
+import os
 
 cupImage= """                                                                                       
                                       ██    ██    ██                                    
                                     ██      ██  ██                                      
                                     ██    ██    ██                                      
                                       ██  ██      ██                                    
                                       ██    ██    ██                                    
@@ -24,33 +26,55 @@
                                   ██                ██  ██                              
                                   ██                ██  ██                              
                                   ██                ██████                              
                                     ██            ██                                    
                                 ████████████████████████                                
                                 ██                    ██                                
                                   ████████████████████"""
-                                     
+
+# randomly pick from a list of random quotes
+def quoteGen():
+    try:
+         path = os.path.dirname(__file__)
+         realPath = "quotes/quotes.txt"
+         location = os.path.join(path, realPath)
+         with open(location, 'r') as f:
+             quotes = [] # all quotes in list, randomly pick 1 out of 20
+             text = f.readlines()
+             quotes.append(text)
+             chosen = random.choice(text)
+             print("\n                             " + chosen)
+    except Exception as e:
+        logging.exception(e)
+        print("\nQuoteGen failed... Proceeding.")
+        pass
+
 def spinningCursor(): # shows the script is running, dosent actually mean anything :/
-    while True:
-        for cursor in "|/-\\":
-            yield cursor
+    try:
+        while True:
+            for cursor in "|/-\\":
+                yield cursor
+    except Exception as e:
+        logging.exception(e)
+        print("spinningCursor failed... Proceeding.")
 
 def currentUser(): #current user logged in
     user = getpass.getuser()
     print("Hello, " + user)
     
 def getTime():
     try:
         now = datetime.now()
         current_time = now.strftime("%H:%M:%S")
         print("It is: "+ current_time)
     except Exception as e:
         logging.exception(e)
-        print("\nSomething's wrong, Unable to display the current time")
-
+        print("\nSomething's wrong, Unable to display the current time.")
+        exit()
+        
 # display the system uptime in a readable format
 def bootTime():
     return time.time() - psutil.boot_time()
 
 boot = bootTime()/60
 approxBoot = round(boot, 1)
 
@@ -64,28 +88,28 @@
     totalDisk = round(total, 1)
     used = int(info[1]) / (1024 * 1024 * 1024) # total used space
     usedDisk = round(used, 1)
     fraction = (usedDisk / totalDisk) *100
     newFraction = str(round(fraction, 1))
 except Exception as e:
     logging.exception(e)
-    print("\nSomething went wrong while trying to access your disk... Proceeding.")
-    pass
+    print("\nSomething went wrong while trying to access your disk.")
+    exit()
 
 # get CPU frequency
 try:
     data = []
     cpuData = psutil.cpu_freq() # tuple with (current, min, max)
     data = list(cpuData)
     floatFreq = int(data[0])/1000 #convert MHz to GHz
     freq = str(round(floatFreq, 2))
 except Exception as e:
     logging.exception(e)
-    print("\nSomething went wrong while trying to access your CPU info.... Proceeding.")
-    pass
+    print("\nSomething went wrong while trying to access your CPU info.")
+    exit()
 
 def infoGrabber():
     try:
         data = [] # data fills this list from 0-6
         data.append(str(system())) # OS
         data.append(str(release())) # version
         data.append(str(machine())) # architecture
@@ -98,14 +122,15 @@
         spinner = spinningCursor()
         for _ in range(7):
             sys.stdout.write(next(spinner))
             sys.stdout.flush()
             time.sleep(0.1)
             sys.stdout.write('\b')
         print(cupImage)
+        quoteGen()
         currentUser()
         getTime()
         print("*------------------------------*") # display the data
         print("OS: "+ data[0])
         print("VERSION: "+ data[1])
         print("CPU: "+ data[5] + " ("+ freq + " GHz)")
         print("ARCHITECTURE: "+ data[2])
@@ -114,8 +139,8 @@
         print("IP: "+ data[4])
         print("RAM: "+ newUsage + "% used / " + data[6] + " total")
         print("DISK:", newFraction + "% used / "+ str(totalDisk) +" GB total")
         print("*------------------------------*")
     except Exception as e:
         logging.exception(e)
         print("\nSomething has failed, please check for any issues!!!")
-        
+        exit()
```

### Comparing `coffeefetch-1.0.0/LICENCE` & `coffeefetch-1.1.0/LICENCE`

 * *Files identical despite different names*

### Comparing `coffeefetch-1.0.0/README.md` & `coffeefetch-1.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # CoffeeFetch
-![image](https://github.com/TeaPixl/CoffeeFetch/assets/106362493/b814fc52-e229-41a8-97a0-70b91c9eb051)
+![image](https://github.com/TeaPixl/CoffeeFetch/assets/106362493/d4a4ee47-d3d1-4581-a9a8-e5a54605799d)
 ## A lightweight system info grabber written in Python
 
 ## Introduction
 CoffeeFetch is a system information grabber for Unix systems that fetches your system information and displays it to the screen. This is a lightweight package and is built to be run on systems without the use of a Window Manager or Desktop Enviornment and is displayed directly in in TTY. It will attempt to grab you CPU model, CPU frequency, current RAM consumption, current disk usage, Operating System, CPU architecture, IP Address, hostname, and OS version.
 
 ## Installation
 It is required to use Python 3.7 or greater for this package. 
@@ -33,13 +33,13 @@
 ## Usage
 To use CoffeeFetch, type into your terminal:
 ```
 python3 -m coffeefetch
 ```
 
 ## NOTE
-This project is currently in the works and I have not finished it yet
+This project is currently in the works and I have not finished it yet.
 This is a NEW repository so feel free to post any issues you may find.
 
 Currently working on:
-+ converting this project into a Python Package
-+ adding random quotes that appear below the image
++ adding -help and other discrete commands
++ testing
```

### Comparing `coffeefetch-1.0.0/pyproject.toml` & `coffeefetch-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "coffeefetch"
-version = "1.0.0"
+version = "1.1.0"
 authors = [
   { name="Logan Allen", email="ltallen392@gmail.com" },
 ]
 description = "A lightweight system information grabber written in Python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `coffeefetch-1.0.0/PKG-INFO` & `coffeefetch-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: coffeefetch
-Version: 1.0.0
+Version: 1.1.0
 Summary: A lightweight system information grabber written in Python
 Project-URL: Homepage, https://github.com/TeaPixl/CoffeeFetch
 Project-URL: Bug Tracker, https://github.com/TeaPixl/CoffeeFetch/issues
 Author-email: Logan Allen <ltallen392@gmail.com>
 License-File: LICENCE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # CoffeeFetch
-![image](https://github.com/TeaPixl/CoffeeFetch/assets/106362493/b814fc52-e229-41a8-97a0-70b91c9eb051)
+![image](https://github.com/TeaPixl/CoffeeFetch/assets/106362493/d4a4ee47-d3d1-4581-a9a8-e5a54605799d)
 ## A lightweight system info grabber written in Python
 
 ## Introduction
 CoffeeFetch is a system information grabber for Unix systems that fetches your system information and displays it to the screen. This is a lightweight package and is built to be run on systems without the use of a Window Manager or Desktop Enviornment and is displayed directly in in TTY. It will attempt to grab you CPU model, CPU frequency, current RAM consumption, current disk usage, Operating System, CPU architecture, IP Address, hostname, and OS version.
 
 ## Installation
 It is required to use Python 3.7 or greater for this package. 
@@ -47,13 +47,13 @@
 ## Usage
 To use CoffeeFetch, type into your terminal:
 ```
 python3 -m coffeefetch
 ```
 
 ## NOTE
-This project is currently in the works and I have not finished it yet
+This project is currently in the works and I have not finished it yet.
 This is a NEW repository so feel free to post any issues you may find.
 
 Currently working on:
-+ converting this project into a Python Package
-+ adding random quotes that appear below the image
++ adding -help and other discrete commands
++ testing
```

