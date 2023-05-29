# Comparing `tmp/ot_my_libs-0.0.12.tar.gz` & `tmp/ot_my_libs-0.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ot_my_libs-0.0.12.tar", last modified: Sun May 28 20:06:32 2023, max compression
+gzip compressed data, was "ot_my_libs-0.0.14.tar", last modified: Mon May 29 01:28:38 2023, max compression
```

## Comparing `ot_my_libs-0.0.12.tar` & `ot_my_libs-0.0.14.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-05-28 20:06:32.936776 ot_my_libs-0.0.12/
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     1068 2023-05-12 13:21:05.000000 ot_my_libs-0.0.12/LICENSE.txt
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     4320 2023-05-28 20:06:32.936776 ot_my_libs-0.0.12/PKG-INFO
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     3687 2023-05-28 19:58:34.000000 ot_my_libs-0.0.12/README.md
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)      667 2023-05-28 20:00:47.000000 ot_my_libs-0.0.12/pyproject.toml
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       38 2023-05-28 20:06:32.936776 ot_my_libs-0.0.12/setup.cfg
-drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-05-28 20:06:32.928776 ot_my_libs-0.0.12/src/
-drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-05-28 20:06:32.932776 ot_my_libs-0.0.12/src/ot_my_libs/
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     1369 2023-05-21 11:47:37.000000 ot_my_libs-0.0.12/src/ot_my_libs/ArgsParse.py
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     8182 2023-05-13 23:15:03.000000 ot_my_libs-0.0.12/src/ot_my_libs/FileActions.py
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)     3534 2020-12-13 15:12:40.000000 ot_my_libs-0.0.12/src/ot_my_libs/MyCalculate.py
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     5876 2023-05-28 19:53:25.000000 ot_my_libs-0.0.12/src/ot_my_libs/PlugsHelper.py
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       43 2023-05-28 16:09:50.000000 ot_my_libs-0.0.12/src/ot_my_libs/PlugsHelperTest_plug1_a.py
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       91 2023-05-28 16:33:34.000000 ot_my_libs-0.0.12/src/ot_my_libs/PlugsHelperTest_plug2_a.py
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       43 2023-05-28 16:09:38.000000 ot_my_libs-0.0.12/src/ot_my_libs/PlugsHelperTest_plug3_a.py
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     2452 2021-11-25 22:30:22.000000 ot_my_libs-0.0.12/src/ot_my_libs/TimeHelper.py
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     4222 2021-08-18 16:59:52.000000 ot_my_libs-0.0.12/src/ot_my_libs/XMLHelper.py
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       84 2023-05-28 20:05:46.000000 ot_my_libs-0.0.12/src/ot_my_libs/__init__.py
--rw-r--r--   0 yoyo      (1000) yoyo      (1000)     4036 2023-05-19 11:11:30.000000 ot_my_libs-0.0.12/src/ot_my_libs/db_helper.py
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     1508 2023-05-12 16:10:01.000000 ot_my_libs-0.0.12/src/ot_my_libs/example.py
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     3673 2021-03-23 17:12:02.000000 ot_my_libs-0.0.12/src/ot_my_libs/myFastPlot.py
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     2619 2023-05-21 11:44:07.000000 ot_my_libs-0.0.12/src/ot_my_libs/myLoger.py
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     1710 2023-05-12 15:48:52.000000 ot_my_libs-0.0.12/src/ot_my_libs/myMqttClient.py
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     9935 2023-05-13 22:54:38.000000 ot_my_libs-0.0.12/src/ot_my_libs/mysql_helper.py
-drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-05-28 20:06:32.936776 ot_my_libs-0.0.12/src/ot_my_libs.egg-info/
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     4320 2023-05-28 20:06:32.000000 ot_my_libs-0.0.12/src/ot_my_libs.egg-info/PKG-INFO
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)      724 2023-05-28 20:06:32.000000 ot_my_libs-0.0.12/src/ot_my_libs.egg-info/SOURCES.txt
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)        1 2023-05-28 20:06:32.000000 ot_my_libs-0.0.12/src/ot_my_libs.egg-info/dependency_links.txt
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       25 2023-05-28 20:06:32.000000 ot_my_libs-0.0.12/src/ot_my_libs.egg-info/requires.txt
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       11 2023-05-28 20:06:32.000000 ot_my_libs-0.0.12/src/ot_my_libs.egg-info/top_level.txt
+drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-05-29 01:28:38.845585 ot_my_libs-0.0.14/
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     1068 2023-05-12 13:21:05.000000 ot_my_libs-0.0.14/LICENSE.txt
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     4438 2023-05-29 01:28:38.845585 ot_my_libs-0.0.14/PKG-INFO
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     3805 2023-05-29 01:09:45.000000 ot_my_libs-0.0.14/README.md
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)      667 2023-05-28 22:37:03.000000 ot_my_libs-0.0.14/pyproject.toml
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       38 2023-05-29 01:28:38.845585 ot_my_libs-0.0.14/setup.cfg
+drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-05-29 01:28:38.837585 ot_my_libs-0.0.14/src/
+drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-05-29 01:28:38.845585 ot_my_libs-0.0.14/src/ot_my_libs/
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     1369 2023-05-21 11:47:37.000000 ot_my_libs-0.0.14/src/ot_my_libs/ArgsParse.py
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     8182 2023-05-13 23:15:03.000000 ot_my_libs-0.0.14/src/ot_my_libs/FileActions.py
+-rw-r--r--   0 yoyo      (1000) yoyo      (1000)     3534 2020-12-13 15:12:40.000000 ot_my_libs-0.0.14/src/ot_my_libs/MyCalculate.py
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     8144 2023-05-29 01:27:33.000000 ot_my_libs-0.0.14/src/ot_my_libs/PlugsHelper.py
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       43 2023-05-28 16:09:50.000000 ot_my_libs-0.0.14/src/ot_my_libs/PlugsHelperTest_plug1_a.py
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       91 2023-05-28 16:33:34.000000 ot_my_libs-0.0.14/src/ot_my_libs/PlugsHelperTest_plug2_a.py
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       43 2023-05-28 16:09:38.000000 ot_my_libs-0.0.14/src/ot_my_libs/PlugsHelperTest_plug3_a.py
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     2452 2021-11-25 22:30:22.000000 ot_my_libs-0.0.14/src/ot_my_libs/TimeHelper.py
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     4222 2021-08-18 16:59:52.000000 ot_my_libs-0.0.14/src/ot_my_libs/XMLHelper.py
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       84 2023-05-28 22:48:05.000000 ot_my_libs-0.0.14/src/ot_my_libs/__init__.py
+-rw-r--r--   0 yoyo      (1000) yoyo      (1000)     4036 2023-05-19 11:11:30.000000 ot_my_libs-0.0.14/src/ot_my_libs/db_helper.py
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     2518 2023-05-29 00:39:23.000000 ot_my_libs-0.0.14/src/ot_my_libs/example.py
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     3673 2021-03-23 17:12:02.000000 ot_my_libs-0.0.14/src/ot_my_libs/myFastPlot.py
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     2619 2023-05-21 11:44:07.000000 ot_my_libs-0.0.14/src/ot_my_libs/myLoger.py
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     1710 2023-05-12 15:48:52.000000 ot_my_libs-0.0.14/src/ot_my_libs/myMqttClient.py
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     9935 2023-05-13 22:54:38.000000 ot_my_libs-0.0.14/src/ot_my_libs/mysql_helper.py
+drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-05-29 01:28:38.845585 ot_my_libs-0.0.14/src/ot_my_libs.egg-info/
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     4438 2023-05-29 01:28:38.000000 ot_my_libs-0.0.14/src/ot_my_libs.egg-info/PKG-INFO
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)      724 2023-05-29 01:28:38.000000 ot_my_libs-0.0.14/src/ot_my_libs.egg-info/SOURCES.txt
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)        1 2023-05-29 01:28:38.000000 ot_my_libs-0.0.14/src/ot_my_libs.egg-info/dependency_links.txt
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       25 2023-05-29 01:28:38.000000 ot_my_libs-0.0.14/src/ot_my_libs.egg-info/requires.txt
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       11 2023-05-29 01:28:38.000000 ot_my_libs-0.0.14/src/ot_my_libs.egg-info/top_level.txt
```

### Comparing `ot_my_libs-0.0.12/LICENSE.txt` & `ot_my_libs-0.0.14/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ot_my_libs-0.0.12/PKG-INFO` & `ot_my_libs-0.0.14/src/ot_my_libs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ot_my_libs
-Version: 0.0.12
+Name: ot-my-libs
+Version: 0.0.14
 Summary: oiyshTerminal my basic libs: myLoger | FileActions | PlugsHelper | MyCalculate | db_helper | mysql_helper | ...
 Author-email: Bartlomiej Ceglik <yoyoek@wp.pl>
 Project-URL: Homepage, https://github.com/yOyOeK1/oiyshTerminal/tree/main/OTPIPS/ot_my_libs
 Project-URL: Bug Tracker, https://github.com/yOyOeK1/oiyshTerminal/labels/ot_my_libs
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -150,14 +150,18 @@
 ### TODO
 
 - [ ] more examples
 - [ ] more def xdoc descriptions
 
 ### change log
 
+* 0.0.14
+  - PlugsHelper in examples
+  - Refine PlugsHelper can do custom filter and return preinit object if set so
+
 * 0.0.12
 
   - PlugsHelper
 
 * 0.0.11
 
   - fix some README errors parsing and ...
```

### Comparing `ot_my_libs-0.0.12/README.md` & `ot_my_libs-0.0.14/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -136,14 +136,18 @@
 ### TODO
 
 - [ ] more examples
 - [ ] more def xdoc descriptions
 
 ### change log
 
+* 0.0.14
+  - PlugsHelper in examples
+  - Refine PlugsHelper can do custom filter and return preinit object if set so
+
 * 0.0.12
 
   - PlugsHelper
 
 * 0.0.11
 
   - fix some README errors parsing and ...
```

### Comparing `ot_my_libs-0.0.12/pyproject.toml` & `ot_my_libs-0.0.14/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ot_my_libs"
-version = "0.0.12"
+version = "0.0.14"
 authors = [
   { name="Bartlomiej Ceglik", email="yoyoek@wp.pl" },
 ]
 description = "oiyshTerminal my basic libs: myLoger | FileActions | PlugsHelper | MyCalculate | db_helper | mysql_helper | ..."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `ot_my_libs-0.0.12/src/ot_my_libs/ArgsParse.py` & `ot_my_libs-0.0.14/src/ot_my_libs/ArgsParse.py`

 * *Files identical despite different names*

### Comparing `ot_my_libs-0.0.12/src/ot_my_libs/FileActions.py` & `ot_my_libs-0.0.14/src/ot_my_libs/FileActions.py`

 * *Files identical despite different names*

### Comparing `ot_my_libs-0.0.12/src/ot_my_libs/MyCalculate.py` & `ot_my_libs-0.0.14/src/ot_my_libs/MyCalculate.py`

 * *Files identical despite different names*

### Comparing `ot_my_libs-0.0.12/src/ot_my_libs/PlugsHelper.py` & `ot_my_libs-0.0.14/src/ot_my_libs/PlugsHelper.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,112 +2,176 @@
 from ot_my_libs.myLoger import myLoger as mlog
 from ot_my_libs.FileActions import *
 
 import sys,os
 import importlib as il
 
 class PlugsHelper:
+    """ To play with plugins idea fast ...
+
+        __returns__ by default _array_ of _json_
+        ```json
+        [
+            {
+                "o": #_def_ or _object_,
+                "type": "driver",
+                "cname": #_str_ string,
+                "name": #_str_ string name
+            }, ...
+        ]
+        ```
+
+    """
 
     args={}
     conf={}
     deb=False
 
-    def __init__( self, args=None, conf=None ):
+    def __init__( self, oAsInitObject = False, args=None, conf=None ):
+        """
+        **oAsInitObject** _bool_ _default_ False - return ['o'] as init object with args,conf as argument or as definition to init
+        **args** - to pass to your plugin
+        **conf** - to pass to your plugin
+        """
         self.log = mlog( "PlugsHelper",
             silenc={
-                'info': True,
+                'info': False,
                 'debug': False,
                 'error': True,
                 'critical': True
                 })
 
         self.log.debug(f"PlugsHelper args:[{args}]")
         self.log.debug( sys.path )
 
+
+        self.oAsInitObject = oAsInitObject
         self.fa = FileActions()
         self.args=args
         self.conf=conf
         self.drivers=[]
 
 
     def ifNoArgExit( self, arg, msgOnErr ):
         if self.args.get( arg, "" ) == "":
             self.log.error(f"No argument [-{arg}] found in argument. {msgOnErr}")
             sys.exit(1)
         else:
             return self.args.get( arg )
 
-    def dirPlugs( self, pPrefix, pDiffThen ):
+    def dirPlugs( self, pPrefix, pDiffThen, extraPaths = None ):
+        """
+        To look for library like by mache prefix and different then ...
+        **pPrefix** _str_ - need to mache to go to list
+        **pDiffThen** _str_|_filter_function - string is exact mache then no. If filter function arg as `name` is pass and your function need to return _bool_ on add it
+        **extraPaths** _array_ of _str_ - to add extra paths to look for
+        """
         preLen = len( pPrefix )
         minLen = preLen+1
 
-        self.log.debug("[ i ] looking for dir drivers ....")
+        self.log.debug("[ i ] looking for dir drivers ....extra:{extraPaths}")
         tr = []
+        pathsToChk = []
+        if extraPaths != None:
+            pathsToChk = extraPaths
         for p in sys.path:
+            pathsToChk.append(p)
+
+        for p in pathsToChk:
             self.log.debug(f" looking in [{p}]")
             if p in [ "/usr/lib/python38.zip" ]:
                 continue
 
             dList = self.fa.getDirList( p )
             #print(dList)
             if isinstance(dList, list):
                 for f in dList:
                     tname = f
                     if len(tname) >= minLen:
 
+                        difTestRes = False
+                        if isinstance( pDiffThen, str) and tname != pDiffThen:
+                            difTestRes = True
+                        else:
+                            difTestRes = pDiffThen( tname )
+
                         if tname[:preLen] == pPrefix and \
                             tname[-10:] != ".dist-info" and \
-                            tname != pDiffThen:
+                            difTestRes:
                             cname=tname.replace(".py","")
                             self.log.debug("GOT it ! %s"%cname)
                             d=il.import_module( cname )
+                            if self.oAsInitObject:
+                                d=eval(f"d.{cname}( self.args, self.conf ) ")
                             tr.append( {
                                 "o": d,
                                 "type": "driver",
                                 "cname": cname,
                                 "name": d
                             } )
 
 
         self.log.info(f"got ({len(tr)}) libs useng [{pPrefix}] ...  but not [{pDiffThen}] dir look up")
         return tr
 
 
-    def lookForDrivers( self, pPrefix, pSufix, pDiffThen, acts = None ):
+    def lookForDrivers( self, pPrefix, pSufix, pDiffThen, extraPaths = None):
+        """
+        To look for files in current library or paths by maching ...
+        **pPrefix** _str_ - need to mache to go to list
+        **pSufix** _str_ - need to mache to go to list
+        **pDiffThen** _str_|_filter_function - string is exact mache then no. If filter function arg as `name` is pass and your function need to return _bool_ on add it
+        **extraPaths** _array_ of _str_ - to add extra paths to look for
+        """
         preLen = len( pPrefix )
         sufLen = len( pSufix )
         minLen = preLen+sufLen+1
 
-        self.log.debug("[ i ] looking for drivers ....")
+        self.log.debug("[ i ] looking for drivers .... extra:{extraPaths}")
         tr = []
+        pathsToChk = []
+        if extraPaths != None:
+            pathsToChk = extraPaths
         for p in sys.path:
+            pathsToChk.append(p)
+
+        for p in pathsToChk:
             self.log.debug(f" looking in [{p}]")
             if p in [ "/usr/lib/python38.zip" ]:
                 continue
 
-            fList = self.fa.getFileList( p )
+            fList = self.fa.getFileList( "." if p == "" else p )
+            self.log.debug(fList)
             #dList = self.fa.getDirList( p )
             #print(dList)
             if isinstance(fList, list):
                 for f in fList:
                     tname = f
                     if 1:#f.get("isFile"):
                         #otdmDriverXXXXX.py
                         if len(tname) >= minLen:
 
+                            difTestRes = False
+                            if isinstance( pDiffThen, str) and tname != pDiffThen:
+                                difTestRes = True
+                            else:
+                                difTestRes = pDiffThen( tname )
+
                             if tname[:preLen] == pPrefix and \
                                 tname[-3:] == ".py" and \
                                 tname[-sufLen:] == pSufix and \
-                                tname != pDiffThen:
+                                difTestRes:
                                 cname=tname.replace(".py","")
                                 self.log.debug("GOT it ! %s"%cname)
 
                                 #eval( f"import {cname}" )
                                 #print("importing")
                                 d=il.import_module( cname )
+                                if self.oAsInitObject:
+                                    d=eval(f"d.{cname}( self.args, self.conf ) ")
                                 #d=eval(f"d.{cname}( self.args, self.conf ) ")
                                 #d=f"{cname}"( args, conf )
                                 #print
                                 #d=d.otdmDriverProto( args, conf )
                                 #print("getName")
                                 #d.getName()
                                 tr.append( {
@@ -132,53 +196,40 @@
             print(" + ", end=" ")
         print("")
 
         return acts
 
 
 
-
-
-
-if __name__ == '__main__':
+def PlugsHelperExample():
     """
-    Main in this case is to have aka example section where you can see how to use it
-    We need to make some steps. Plugin system can work on file system in current
-    directory or in directory of python libsrary path. Or plugins by directory
-    so looking for key maths and ther include it as is ...
-
-    in directory of installation run to check ...
-    `python3 ./ot_my_libs/PlugsHelper.py`
-
+    **PlugsHelperExample** example use look up for files / dirs to load as plugins ...
     """
 
-    """ setting up logging settings """
-    log = mlog( "PlugsHelper.Main",
-        silenc={
-            'info': False,
-            'debug': False,
-            'error': True,
-            'critical': True
-            })
-    log.info("as test run / maint ....")
-
-    """ to make instance """
+    print("* instance of PlugsHelper ..")
     ph = PlugsHelper()
 
-    libs = ph.lookForDrivers( "PlugsHelperTest_", "_a.py", "abc.py" )
-    log.info(f"Libs found ({len(libs)}) ")
-    log.debug(libs)
-    log.debug("-----------------------------------")
+    print("* looking for local plugins ...")
+    libs = ph.lookForDrivers( "PlugsHelperTest_", "_a.py", "abc.py")
+    print(f"  * Libs found ({len(libs)}) ")
+    print(libs)
+    print("-----------------------------------")
     if len(libs) > 0:
-        log.info("Executing lib 0 ...")
+        print("* Executing lib 0 ...")
         libs[0]['o'].plug()
 
-    log.info("DONE")
-
+    print("DONE")
 
     libs = ph.dirPlugs( "ot_my_", "abc.py" )
-    log.info(f"Libs dirs found ({len(libs)}) \n {libs}")
+    print(f"* looking for dirs plugings ... found ({len(libs)}) \n {libs}")
     if len(libs) > 0:
-        log.info("Executing lib 0 as directory plugin ...")
+        print("* Executing lib 0 as directory plugin ...")
         libs[0]['o'].ot_my_libs()
 
-    log.info("DONE")
+    print("DONE")
+
+
+if __name__ == '__main__':
+    """
+    look in example PlugsHelperExample
+
+    """
```

### Comparing `ot_my_libs-0.0.12/src/ot_my_libs/TimeHelper.py` & `ot_my_libs-0.0.14/src/ot_my_libs/TimeHelper.py`

 * *Files identical despite different names*

### Comparing `ot_my_libs-0.0.12/src/ot_my_libs/XMLHelper.py` & `ot_my_libs-0.0.14/src/ot_my_libs/XMLHelper.py`

 * *Files identical despite different names*

### Comparing `ot_my_libs-0.0.12/src/ot_my_libs/db_helper.py` & `ot_my_libs-0.0.14/src/ot_my_libs/db_helper.py`

 * *Files identical despite different names*

### Comparing `ot_my_libs-0.0.12/src/ot_my_libs/example.py` & `ot_my_libs-0.0.14/src/ot_my_libs/example.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 
 # using TimeHelper as benchmark timer ...
 from ot_my_libs.TimeHelper import TimeHelper as thd
 import time
 
 
 def benchmarkTimer():
+    """
+    **TimeHelper** as benchmark timer ...
+    """
 
     th = thd()
 
     bKey = th.benStart()
 
     print("making test run ...")
     time.sleep(1)
@@ -19,23 +22,32 @@
         bKey,
         f"Result of benStart / benDone [run at:{th.getNiceShortDate()}]", printIt=True )
 
 
 # using db_helper
 from ot_my_libs.db_helper import db_helper as dbh
 class mdb ( dbh ):
+    """
+    **db_helper** needs - overiting ours data structure and types
+    """
     ## set your structure of db / table
     def set_struct(self):
         self.struct = {
             'tableA' : {
                       'lat':     "float",
                       'lon':     "float",
                       }
             }
+
+
 def dbHelperExample():
+    """
+    **db_helper** example use case: from init, to inser, more inserts, some selections ...
+    """
+
     db = mdb('/tmp/mdbTest1.db')
 
     print("select tableA ... ")
     print( db.select('tableA') )
 
     print("inserting ....")
     insertRecordId = db.insert('tableA', {"lat":1.1,"lon":1.1} )
@@ -49,17 +61,46 @@
     print(db.select('tableA','id,lat,lon', 'id=2'))
 
     print("delete all ...")
     db.query('delete from tableA where 1')
     print("after delete ... select tableA")
     print(db.select('tableA'))
 
+# using PlugsHelper
+from ot_my_libs.PlugsHelper import *
+def PlugsHelperExampleTest():
+    """
+    **PlugsHelperExample** example use look up for files / dirs to load as plugins ...
+
+    ## with filter
+      To have custom filter on what not to ...
+      ```python3
+      def phYesNo( nameTest ):
+          if nameTest == "otdmDriverManager.py":
+              return False
+          elif nameTest[-8:] == "Proto.py":
+              return False
+          else:
+              return True
+
+      ph = PlugsHelper()
+      plugs = ph.lookForDrivers( "otdmDriver", ".py", phYesNo ):
+      ```
+    """
+    PlugsHelperExample()
+
 
 def testRunAll():
+    """
+    will run them all so you can see it in action
+    """
+
     print("can show some examples .....")
     print("- benchmarkTimer")
     benchmarkTimer()
     print("- db_helper making instance of db ...")
-    dbHelperExample()
+    PlugsHelperExampleTest()
+    print("- PlugsHelper test run ...")
+    PlugsHelperExample()
 
 if __name__ == "__main__":
     testRunAll()
```

### Comparing `ot_my_libs-0.0.12/src/ot_my_libs/myFastPlot.py` & `ot_my_libs-0.0.14/src/ot_my_libs/myFastPlot.py`

 * *Files identical despite different names*

### Comparing `ot_my_libs-0.0.12/src/ot_my_libs/myLoger.py` & `ot_my_libs-0.0.14/src/ot_my_libs/myLoger.py`

 * *Files identical despite different names*

### Comparing `ot_my_libs-0.0.12/src/ot_my_libs/myMqttClient.py` & `ot_my_libs-0.0.14/src/ot_my_libs/myMqttClient.py`

 * *Files identical despite different names*

### Comparing `ot_my_libs-0.0.12/src/ot_my_libs/mysql_helper.py` & `ot_my_libs-0.0.14/src/ot_my_libs/mysql_helper.py`

 * *Files identical despite different names*

### Comparing `ot_my_libs-0.0.12/src/ot_my_libs.egg-info/PKG-INFO` & `ot_my_libs-0.0.14/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ot-my-libs
-Version: 0.0.12
+Name: ot_my_libs
+Version: 0.0.14
 Summary: oiyshTerminal my basic libs: myLoger | FileActions | PlugsHelper | MyCalculate | db_helper | mysql_helper | ...
 Author-email: Bartlomiej Ceglik <yoyoek@wp.pl>
 Project-URL: Homepage, https://github.com/yOyOeK1/oiyshTerminal/tree/main/OTPIPS/ot_my_libs
 Project-URL: Bug Tracker, https://github.com/yOyOeK1/oiyshTerminal/labels/ot_my_libs
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -150,14 +150,18 @@
 ### TODO
 
 - [ ] more examples
 - [ ] more def xdoc descriptions
 
 ### change log
 
+* 0.0.14
+  - PlugsHelper in examples
+  - Refine PlugsHelper can do custom filter and return preinit object if set so
+
 * 0.0.12
 
   - PlugsHelper
 
 * 0.0.11
 
   - fix some README errors parsing and ...
```

### Comparing `ot_my_libs-0.0.12/src/ot_my_libs.egg-info/SOURCES.txt` & `ot_my_libs-0.0.14/src/ot_my_libs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

