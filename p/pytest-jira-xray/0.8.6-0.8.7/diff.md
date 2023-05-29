# Comparing `tmp/pytest_jira_xray-0.8.6-py3-none-any.whl.zip` & `tmp/pytest_jira_xray-0.8.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 18651 bytes, number of entries: 16
+Zip file size: 18700 bytes, number of entries: 16
 -rw-r--r--  2.0 unx        0 b- defN 22-May-08 18:35 pytest_xray/__init__.py
 -rw-r--r--  2.0 unx     1202 b- defN 22-Oct-23 10:23 pytest_xray/constant.py
 -rw-r--r--  2.0 unx      990 b- defN 23-Apr-25 17:54 pytest_xray/evidence.py
 -rw-r--r--  2.0 unx      137 b- defN 22-May-08 18:35 pytest_xray/exceptions.py
 -rw-r--r--  2.0 unx      836 b- defN 23-Feb-08 22:24 pytest_xray/file_publisher.py
 -rw-r--r--  2.0 unx     9205 b- defN 23-Feb-08 22:08 pytest_xray/helper.py
 -rw-r--r--  2.0 unx      298 b- defN 22-Sep-25 16:30 pytest_xray/hooks.py
--rw-r--r--  2.0 unx     3599 b- defN 23-Mar-13 19:16 pytest_xray/plugin.py
--rw-r--r--  2.0 unx     6689 b- defN 23-Mar-12 18:23 pytest_xray/xray_plugin.py
+-rw-r--r--  2.0 unx     3648 b- defN 23-May-29 18:01 pytest_xray/plugin.py
+-rw-r--r--  2.0 unx     6777 b- defN 23-May-29 18:01 pytest_xray/xray_plugin.py
 -rw-r--r--  2.0 unx     4389 b- defN 23-Mar-13 19:16 pytest_xray/xray_publisher.py
--rw-rw-r--  2.0 unx    11357 b- defN 23-May-15 13:19 pytest_jira_xray-0.8.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     8691 b- defN 23-May-15 13:19 pytest_jira_xray-0.8.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-15 13:19 pytest_jira_xray-0.8.6.dist-info/WHEEL
--rw-rw-r--  2.0 unx       37 b- defN 23-May-15 13:19 pytest_jira_xray-0.8.6.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       12 b- defN 23-May-15 13:19 pytest_jira_xray-0.8.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1339 b- defN 23-May-15 13:19 pytest_jira_xray-0.8.6.dist-info/RECORD
-16 files, 48873 bytes uncompressed, 16427 bytes compressed:  66.4%
+-rw-rw-r--  2.0 unx    11357 b- defN 23-May-29 18:04 pytest_jira_xray-0.8.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8691 b- defN 23-May-29 18:04 pytest_jira_xray-0.8.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-29 18:04 pytest_jira_xray-0.8.7.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       37 b- defN 23-May-29 18:04 pytest_jira_xray-0.8.7.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       12 b- defN 23-May-29 18:04 pytest_jira_xray-0.8.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1339 b- defN 23-May-29 18:04 pytest_jira_xray-0.8.7.dist-info/RECORD
+16 files, 49010 bytes uncompressed, 16476 bytes compressed:  66.4%
```

## zipnote {}

```diff
@@ -24,26 +24,26 @@
 
 Filename: pytest_xray/xray_plugin.py
 Comment: 
 
 Filename: pytest_xray/xray_publisher.py
 Comment: 
 
-Filename: pytest_jira_xray-0.8.6.dist-info/LICENSE
+Filename: pytest_jira_xray-0.8.7.dist-info/LICENSE
 Comment: 
 
-Filename: pytest_jira_xray-0.8.6.dist-info/METADATA
+Filename: pytest_jira_xray-0.8.7.dist-info/METADATA
 Comment: 
 
-Filename: pytest_jira_xray-0.8.6.dist-info/WHEEL
+Filename: pytest_jira_xray-0.8.7.dist-info/WHEEL
 Comment: 
 
-Filename: pytest_jira_xray-0.8.6.dist-info/entry_points.txt
+Filename: pytest_jira_xray-0.8.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: pytest_jira_xray-0.8.6.dist-info/top_level.txt
+Filename: pytest_jira_xray-0.8.7.dist-info/top_level.txt
 Comment: 
 
-Filename: pytest_jira_xray-0.8.6.dist-info/RECORD
+Filename: pytest_jira_xray-0.8.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pytest_xray/plugin.py

```diff
@@ -83,14 +83,16 @@
     pluginmanager.add_hookspecs(hooks)
 
 
 def pytest_configure(config: Config) -> None:
     config.addinivalue_line(
         'markers', 'xray(JIRA_ID): mark test with JIRA XRAY test case ID'
     )
+    if config.option.collectonly:
+        return
 
     if not config.getoption(JIRA_XRAY_FLAG):
         return
 
     xray_path = config.getoption(XRAYPATH)
 
     if xray_path:
```

## pytest_xray/xray_plugin.py

```diff
@@ -149,14 +149,16 @@
 
         return None
 
     def pytest_collection_modifyitems(self, config: Config, items: List[Item]) -> None:
         self._verify_jira_ids_for_items(items)
 
     def pytest_sessionfinish(self, session: pytest.Session) -> None:
+        if hasattr(self.config, 'workerinput'):  # skipping on xdist
+            return
         self.test_execution.finish_date = dt.datetime.now(tz=dt.timezone.utc)
         results = self.test_execution.as_dict()
         session.config.pluginmanager.hook.pytest_xray_results(
             results=results, session=session
         )
         try:
             self.issue_id = self.publisher.publish(results)
```

## Comparing `pytest_jira_xray-0.8.6.dist-info/LICENSE` & `pytest_jira_xray-0.8.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pytest_jira_xray-0.8.6.dist-info/METADATA` & `pytest_jira_xray-0.8.7.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-jira-xray
-Version: 0.8.6
+Version: 0.8.7
 Summary: pytest plugin to integrate tests with JIRA XRAY
 Home-page: https://github.com/fundakol/pytest-jira-xray
 Author: Lukasz Fundakowski
 Author-email: fundakol@yahoo.com
 Keywords: pytest,JIRA,XRAY
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

## Comparing `pytest_jira_xray-0.8.6.dist-info/RECORD` & `pytest_jira_xray-0.8.7.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 pytest_xray/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pytest_xray/constant.py,sha256=MpbsAbTU2MsPMvDvklaYMBUCOn59p47CDLc8pHjR4bY,1202
 pytest_xray/evidence.py,sha256=R35eGmJxozw8Rb49kpn6fs7lB0haBDJH5XHRVqm72u4,990
 pytest_xray/exceptions.py,sha256=IS-_20kUX3rUTdg_22x5itn2rq-JgpXXO1r5BMq42Xo,137
 pytest_xray/file_publisher.py,sha256=lgB8Vfy8wbWWncj17-aE8v_hIM8hLbAUVkmzHQXrhRk,836
 pytest_xray/helper.py,sha256=3jxNEGQ3OBs1T-txXNTc8PeXHMx_CC1SALh05QVhH2g,9205
 pytest_xray/hooks.py,sha256=Jk9kkIXFdY_WaG7jiDlmWMrlWt-KTXWgy954X5021HY,298
-pytest_xray/plugin.py,sha256=fMAPiF9m_xBImsm-gbGwx_C67GcPYLJVWsfyeTd-LUc,3599
-pytest_xray/xray_plugin.py,sha256=oqSaez1oT0s1tCID_8KUJ_7RCkqDuKksCQVbvxrT1lE,6689
+pytest_xray/plugin.py,sha256=HWiStDkcWIOzB6y9BpjWbs6Y1eOJPhWbfWHx1x1z9_A,3648
+pytest_xray/xray_plugin.py,sha256=ht7TYbcTEJsuAMs5Fg9vJK4dlm_4PGIUU_uz55FAMRo,6777
 pytest_xray/xray_publisher.py,sha256=LA-geG9YpYXgB1G7CfJzCy_w8fh0FPoar8y3h_0S8PM,4389
-pytest_jira_xray-0.8.6.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-pytest_jira_xray-0.8.6.dist-info/METADATA,sha256=tQT0ihtYMoET_2-_9rQ5S4CAv44f1GpAakgl1jnZupM,8691
-pytest_jira_xray-0.8.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pytest_jira_xray-0.8.6.dist-info/entry_points.txt,sha256=uRmCo_t9ZkNt-7ffZAO7IpCbHFKw21w7d8veBr6hjjk,37
-pytest_jira_xray-0.8.6.dist-info/top_level.txt,sha256=gDf8RZBMKKaQj9pocszUu1-vQZm_vkT4UGrzVxiKpPY,12
-pytest_jira_xray-0.8.6.dist-info/RECORD,,
+pytest_jira_xray-0.8.7.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+pytest_jira_xray-0.8.7.dist-info/METADATA,sha256=08e9kn61mxTK3Mp7fcHts-r1YI5dY5GimBsa5Dp7Yr8,8691
+pytest_jira_xray-0.8.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pytest_jira_xray-0.8.7.dist-info/entry_points.txt,sha256=uRmCo_t9ZkNt-7ffZAO7IpCbHFKw21w7d8veBr6hjjk,37
+pytest_jira_xray-0.8.7.dist-info/top_level.txt,sha256=gDf8RZBMKKaQj9pocszUu1-vQZm_vkT4UGrzVxiKpPY,12
+pytest_jira_xray-0.8.7.dist-info/RECORD,,
```

