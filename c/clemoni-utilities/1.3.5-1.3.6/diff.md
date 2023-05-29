# Comparing `tmp/clemoni_utilities-1.3.5-py2.py3-none-any.whl.zip` & `tmp/clemoni_utilities-1.3.6-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 12240 bytes, number of entries: 18
--rw-r--r--  2.0 unx       48 b- defN 23-May-28 20:43 utilities/__init__.py
--rw-r--r--  2.0 unx     3146 b- defN 23-May-28 20:39 utilities/add_package.py
+Zip file size: 12233 bytes, number of entries: 18
+-rw-r--r--  2.0 unx       48 b- defN 23-May-28 20:57 utilities/__init__.py
+-rw-r--r--  2.0 unx     3100 b- defN 23-May-28 20:57 utilities/add_package.py
 -rw-r--r--  2.0 unx     3106 b- defN 23-May-28 20:39 utilities/branching_funcs.py
 -rw-r--r--  2.0 unx     3348 b- defN 23-May-28 20:39 utilities/db_funcs.py
 -rw-r--r--  2.0 unx     7072 b- defN 23-May-28 20:39 utilities/files_system_funcs.py
 -rw-r--r--  2.0 unx      777 b- defN 23-May-28 20:39 utilities/fp_funcs.py
 -rw-r--r--  2.0 unx     2457 b- defN 23-May-28 20:39 utilities/funcs.py
 -rw-r--r--  2.0 unx     1329 b- defN 23-May-28 20:39 utilities/logs_handler.py
 -rw-r--r--  2.0 unx      614 b- defN 23-May-28 20:39 utilities/re_funcs.py
 -rw-r--r--  2.0 unx     2165 b- defN 23-May-28 20:39 utilities/script_ui.py
 -rw-r--r--  2.0 unx     2165 b- defN 23-May-28 20:39 utilities/ui_funcs.py
 -rw-r--r--  2.0 unx     1598 b- defN 23-May-28 20:39 utilities/utils_funcs.py
 -rw-r--r--  2.0 unx      176 b- defN 23-May-28 20:39 utilities/yml_funcs.py
--rw-r--r--  2.0 unx     1072 b- defN 23-May-28 20:45 clemoni_utilities-1.3.5.dist-info/LICENSE
--rw-r--r--  2.0 unx      395 b- defN 23-May-28 20:45 clemoni_utilities-1.3.5.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-28 20:45 clemoni_utilities-1.3.5.dist-info/WHEEL
--rw-r--r--  2.0 unx      119 b- defN 23-May-28 20:45 clemoni_utilities-1.3.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1472 b- defN 23-May-28 20:45 clemoni_utilities-1.3.5.dist-info/RECORD
-18 files, 31169 bytes uncompressed, 9834 bytes compressed:  68.4%
+-rw-r--r--  2.0 unx     1072 b- defN 23-May-29 09:34 clemoni_utilities-1.3.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx      395 b- defN 23-May-29 09:34 clemoni_utilities-1.3.6.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-29 09:34 clemoni_utilities-1.3.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx      119 b- defN 23-May-29 09:34 clemoni_utilities-1.3.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1472 b- defN 23-May-29 09:34 clemoni_utilities-1.3.6.dist-info/RECORD
+18 files, 31123 bytes uncompressed, 9827 bytes compressed:  68.4%
```

## zipnote {}

```diff
@@ -33,23 +33,23 @@
 
 Filename: utilities/utils_funcs.py
 Comment: 
 
 Filename: utilities/yml_funcs.py
 Comment: 
 
-Filename: clemoni_utilities-1.3.5.dist-info/LICENSE
+Filename: clemoni_utilities-1.3.6.dist-info/LICENSE
 Comment: 
 
-Filename: clemoni_utilities-1.3.5.dist-info/METADATA
+Filename: clemoni_utilities-1.3.6.dist-info/METADATA
 Comment: 
 
-Filename: clemoni_utilities-1.3.5.dist-info/WHEEL
+Filename: clemoni_utilities-1.3.6.dist-info/WHEEL
 Comment: 
 
-Filename: clemoni_utilities-1.3.5.dist-info/top_level.txt
+Filename: clemoni_utilities-1.3.6.dist-info/top_level.txt
 Comment: 
 
-Filename: clemoni_utilities-1.3.5.dist-info/RECORD
+Filename: clemoni_utilities-1.3.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## utilities/__init__.py

```diff
@@ -1,2 +1,2 @@
-__version__="1.3.5"
+__version__="1.3.6"
 __author__="CLEMENT LISCOET"
```

## utilities/add_package.py

```diff
@@ -111,18 +111,16 @@
     checked_folder_name=handle_first_slash_path(folder_name) if checked_folder_name is None else checked_folder_name
 
 
     if start<=limit:
 
         tested_path=add_package_folder(current_file, checked_folder_name)
 
-        print(tested_path)
-
         if Path(tested_path).exists():
-            print(tested_path)
+            
             return tested_path
         else:
             checked_folder_name=f"../{checked_folder_name}"
             
             start+=1
 
             return get_path_dynamically(current_file, folder_name, limit, start, checked_folder_name)
```

## Comparing `clemoni_utilities-1.3.5.dist-info/LICENSE` & `clemoni_utilities-1.3.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `clemoni_utilities-1.3.5.dist-info/RECORD` & `clemoni_utilities-1.3.6.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-utilities/__init__.py,sha256=GFpyRvwsm-CBAtdSQUhkUjgvexhMBqJKPtYxs5oTQCA,48
-utilities/add_package.py,sha256=qAz175CW6-9XFVD0RBvWO6S9UrWexdATxsovZinLiCI,3146
+utilities/__init__.py,sha256=WGP_-tfxwqRGucvbz-o129Ajcxt49rojaYnhp57FiWg,48
+utilities/add_package.py,sha256=VDiHS9h7_27klqeT4objMRSETQCI6VXvjTICnDTJoTU,3100
 utilities/branching_funcs.py,sha256=3oW-yPQ0f5Fb8ANeLkiltmR_RB5Rvr_p26WF_pqYXA8,3106
 utilities/db_funcs.py,sha256=K20P5Cs-oJMh4aDve0it6vcbv1OVUlspL6oduvlIWJg,3348
 utilities/files_system_funcs.py,sha256=n-YaHoUglFfafRdDlgmg9P5y2Ny4KuJ9LF_QbfKRTF0,7072
 utilities/fp_funcs.py,sha256=mWCjnduVx_kl3-7gR0fYaQ1Kir1N8HRNrbyNugTFqZg,777
 utilities/funcs.py,sha256=kdHpcwrFbHN2vTApUBYKVBjC8AowNkcuKEKOjEqqhkY,2457
 utilities/logs_handler.py,sha256=DBk8JrytcH47sZxtuL0K6AWhp5J-A9Uth19UZns256U,1329
 utilities/re_funcs.py,sha256=WZpP_kWsh0ZM_yNYipb2Y-jzNz9_YYFSGP0aomrk6Lk,614
 utilities/script_ui.py,sha256=h7gAOZ_3H6BmOfBb1tnSLoRyf_N3YAhPlY11BfG3ZUg,2165
 utilities/ui_funcs.py,sha256=h7gAOZ_3H6BmOfBb1tnSLoRyf_N3YAhPlY11BfG3ZUg,2165
 utilities/utils_funcs.py,sha256=DqxENqvInxOGuvwo2FTVN92Og_QIEJv8QZgVbMMicxo,1598
 utilities/yml_funcs.py,sha256=c_wQ3nTfJ7UWoaY9vDkLPJ-99oo8DuHUK4vMkjgJDmI,176
-clemoni_utilities-1.3.5.dist-info/LICENSE,sha256=P54a64IUtuk1DPIrg4ZmTrEqmRvBzERr6mlEDlvrUiY,1072
-clemoni_utilities-1.3.5.dist-info/METADATA,sha256=Nk7rzRk5zSmTYtuhDwSXs2yHbpT-F04MlmpgwUlUp3g,395
-clemoni_utilities-1.3.5.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-clemoni_utilities-1.3.5.dist-info/top_level.txt,sha256=o0NApI9M1BCgd6W2HpNE2vz48XNmV9mftvVE6Rv_1jo,119
-clemoni_utilities-1.3.5.dist-info/RECORD,,
+clemoni_utilities-1.3.6.dist-info/LICENSE,sha256=P54a64IUtuk1DPIrg4ZmTrEqmRvBzERr6mlEDlvrUiY,1072
+clemoni_utilities-1.3.6.dist-info/METADATA,sha256=LH-cBfzP5Buq2VbLvRQ-bfnk8YjkXoV3wKUtBXSZrMQ,395
+clemoni_utilities-1.3.6.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+clemoni_utilities-1.3.6.dist-info/top_level.txt,sha256=o0NApI9M1BCgd6W2HpNE2vz48XNmV9mftvVE6Rv_1jo,119
+clemoni_utilities-1.3.6.dist-info/RECORD,,
```

