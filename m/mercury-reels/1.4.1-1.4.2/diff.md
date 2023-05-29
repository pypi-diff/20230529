# Comparing `tmp/mercury-reels-1.4.1.tar.gz` & `tmp/mercury-reels-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercury-reels-1.4.1.tar", last modified: Thu May 11 08:07:21 2023, max compression
+gzip compressed data, was "mercury-reels-1.4.2.tar", last modified: Mon May 29 11:42:09 2023, max compression
```

## Comparing `mercury-reels-1.4.1.tar` & `mercury-reels-1.4.2.tar`

### file list

```diff
@@ -1,22 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:07:21.821433 mercury-reels-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10793 2023-05-11 08:07:14.000000 mercury-reels-1.4.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18996 2023-05-11 08:07:21.821433 mercury-reels-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-05-11 08:07:14.000000 mercury-reels-1.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-11 08:07:21.000000 mercury-reels-1.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 08:07:21.821433 mercury-reels-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-11 08:07:14.000000 mercury-reels-1.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:07:21.817433 mercury-reels-1.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:07:21.817433 mercury-reels-1.4.1/src/mercury_reels.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18996 2023-05-11 08:07:21.000000 mercury-reels-1.4.1/src/mercury_reels.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-11 08:07:21.000000 mercury-reels-1.4.1/src/mercury_reels.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 08:07:21.000000 mercury-reels-1.4.1/src/mercury_reels.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-11 08:07:21.000000 mercury-reels-1.4.1/src/mercury_reels.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:07:21.821433 mercury-reels-1.4.1/src/reels/
--rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-05-11 08:07:14.000000 mercury-reels-1.4.1/src/reels/Clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     8400 2023-05-11 08:07:14.000000 mercury-reels-1.4.1/src/reels/Clips.py
--rw-r--r--   0 runner    (1001) docker     (123)    13253 2023-05-11 08:07:14.000000 mercury-reels-1.4.1/src/reels/Events.py
--rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-05-11 08:07:14.000000 mercury-reels-1.4.1/src/reels/Intake.py
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-11 08:07:14.000000 mercury-reels-1.4.1/src/reels/Targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-05-11 08:07:14.000000 mercury-reels-1.4.1/src/reels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   170626 2023-05-11 08:07:14.000000 mercury-reels-1.4.1/src/reels/py_reels_wrap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    84411 2023-05-11 08:07:14.000000 mercury-reels-1.4.1/src/reels/reels.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 11:42:09.730301 mercury-reels-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10793 2023-05-29 11:42:00.000000 mercury-reels-1.4.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-29 11:42:00.000000 mercury-reels-1.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18897 2023-05-29 11:42:09.730301 mercury-reels-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-05-29 11:42:00.000000 mercury-reels-1.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-29 11:42:00.000000 mercury-reels-1.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 11:42:09.730301 mercury-reels-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-29 11:42:00.000000 mercury-reels-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 11:42:09.726301 mercury-reels-1.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 11:42:09.726301 mercury-reels-1.4.2/src/mercury_reels.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18897 2023-05-29 11:42:09.000000 mercury-reels-1.4.2/src/mercury_reels.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-29 11:42:09.000000 mercury-reels-1.4.2/src/mercury_reels.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 11:42:09.000000 mercury-reels-1.4.2/src/mercury_reels.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-29 11:42:09.000000 mercury-reels-1.4.2/src/mercury_reels.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 11:42:09.730301 mercury-reels-1.4.2/src/reels/
+-rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-05-29 11:42:00.000000 mercury-reels-1.4.2/src/reels/Clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8400 2023-05-29 11:42:00.000000 mercury-reels-1.4.2/src/reels/Clips.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13253 2023-05-29 11:42:00.000000 mercury-reels-1.4.2/src/reels/Events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-05-29 11:42:00.000000 mercury-reels-1.4.2/src/reels/Intake.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-29 11:42:00.000000 mercury-reels-1.4.2/src/reels/Targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-05-29 11:42:00.000000 mercury-reels-1.4.2/src/reels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-29 11:42:00.000000 mercury-reels-1.4.2/src/reels/imports.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-29 11:42:00.000000 mercury-reels-1.4.2/src/reels/main.dox
+-rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-05-29 11:42:00.000000 mercury-reels-1.4.2/src/reels/py_reels.i
+-rw-r--r--   0 runner    (1001) docker     (123)   170626 2023-05-29 11:42:00.000000 mercury-reels-1.4.2/src/reels/py_reels_wrap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    84431 2023-05-29 11:42:00.000000 mercury-reels-1.4.2/src/reels/reels.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    45065 2023-05-29 11:42:00.000000 mercury-reels-1.4.2/src/reels/reels.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15947 2023-05-29 11:42:00.000000 mercury-reels-1.4.2/src/reels/reels_main.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-29 11:42:00.000000 mercury-reels-1.4.2/src/reels/reels_main.h
+-rw-r--r--   0 runner    (1001) docker     (123)    56793 2023-05-29 11:42:00.000000 mercury-reels-1.4.2/src/reels/reels_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-29 11:42:00.000000 mercury-reels-1.4.2/src/reels/reels_test.h
+-rw-r--r--   0 runner    (1001) docker     (123)   123064 2023-05-29 11:42:00.000000 mercury-reels-1.4.2/src/reels/thousand_sequences.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    21065 2023-05-29 11:42:00.000000 mercury-reels-1.4.2/src/test_all.py
```

### Comparing `mercury-reels-1.4.1/LICENSE.txt` & `mercury-reels-1.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mercury-reels-1.4.1/PKG-INFO` & `mercury-reels-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: mercury-reels
-Version: 1.4.1
+Version: 1.4.2
 Summary: Reels helps identify patterns in event data and can predict target events.
-Home-page: https://github.com/BBVA/mercury-reels
 Author-email: Mercury Team <mercury.group@bbva.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
         
              Copyright 2022-23, Banco de Bilbao Vizcaya Argentaria, S.A.
@@ -194,17 +193,14 @@
               defend, and hold each Contributor harmless for any liability
               incurred by, or claims asserted against, such Contributor by reason
               of your accepting any such warranty or additional liability.
         
            END OF TERMS AND CONDITIONS
         
 Keywords: event detection,event prediction,time series
-Platform: Linux
-Platform: MacOS
-Platform: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `mercury-reels-1.4.1/README.md` & `mercury-reels-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `mercury-reels-1.4.1/src/mercury_reels.egg-info/PKG-INFO` & `mercury-reels-1.4.2/src/mercury_reels.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: mercury-reels
-Version: 1.4.1
+Version: 1.4.2
 Summary: Reels helps identify patterns in event data and can predict target events.
-Home-page: https://github.com/BBVA/mercury-reels
 Author-email: Mercury Team <mercury.group@bbva.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
         
              Copyright 2022-23, Banco de Bilbao Vizcaya Argentaria, S.A.
@@ -194,17 +193,14 @@
               defend, and hold each Contributor harmless for any liability
               incurred by, or claims asserted against, such Contributor by reason
               of your accepting any such warranty or additional liability.
         
            END OF TERMS AND CONDITIONS
         
 Keywords: event detection,event prediction,time series
-Platform: Linux
-Platform: MacOS
-Platform: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `mercury-reels-1.4.1/src/reels/Clients.py` & `mercury-reels-1.4.2/src/reels/Clients.py`

 * *Files identical despite different names*

### Comparing `mercury-reels-1.4.1/src/reels/Clips.py` & `mercury-reels-1.4.2/src/reels/Clips.py`

 * *Files identical despite different names*

### Comparing `mercury-reels-1.4.1/src/reels/Events.py` & `mercury-reels-1.4.2/src/reels/Events.py`

 * *Files identical despite different names*

### Comparing `mercury-reels-1.4.1/src/reels/Intake.py` & `mercury-reels-1.4.2/src/reels/Intake.py`

 * *Files identical despite different names*

### Comparing `mercury-reels-1.4.1/src/reels/Targets.py` & `mercury-reels-1.4.2/src/reels/Targets.py`

 * *Files identical despite different names*

### Comparing `mercury-reels-1.4.1/src/reels/__init__.py` & `mercury-reels-1.4.2/src/reels/__init__.py`

 * *Files identical despite different names*

### Comparing `mercury-reels-1.4.1/src/reels/py_reels_wrap.cpp` & `mercury-reels-1.4.2/src/reels/py_reels_wrap.cpp`

 * *Files identical despite different names*

### Comparing `mercury-reels-1.4.1/src/reels/reels.cpp` & `mercury-reels-1.4.2/src/reels/reels.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1980,15 +1980,16 @@
 		return answer_buffer;
 
 	int ll = strlen(prev_event);
 
 	char e[1024];
 	char d[1024];
 	BinEventPt ev;
-	EventMap::iterator it_ev = (EventMap::iterator) nullptr;
+	EventMap::iterator it_ev_end = it->second->events_end();
+	EventMap::iterator it_ev = it_ev_end;
 
 	if (ll == 0)
 		it_ev = it->second->events_begin();
 	else if (sscanf(prev_event, "%s\t%s\t%lf", e, d, &ev.w) == 3) {
 		int l = strlen(e);
 
 		if (e[0] != '<' || l != 18 || sscanf(e, "<%016lx>", &ev.e) != 1)
@@ -1998,15 +1999,15 @@
 
 		if (d[0] != '<' || l != 18 || sscanf(d, "<%016lx>", &ev.d) != 1)
 			ev.d = MurmurHash64A(&d, l);
 
 		it_ev = it->second->events_next_after_find(ev);
 	}
 
-	if (it_ev != (EventMap::iterator) nullptr) {
+	if (it_ev != it_ev_end) {
 		if (it->second->store_strings) {
 			String e = it->second->get_str(it_ev->first.e);
 			String d = it->second->get_str(it_ev->first.d);
 			sprintf(answer_buffer, "%s\t%s\t%.5f\t%li", e.c_str(), d.c_str(), it_ev->first.w, it_ev->second.code);
 		} else
 			sprintf(answer_buffer, "<%016lx>\t<%016lx>\t%.5f\t%li", it_ev->first.e, it_ev->first.d, it_ev->first.w, it_ev->second.code);
 	}
```

