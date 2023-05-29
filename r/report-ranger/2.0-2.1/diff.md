# Comparing `tmp/Report-Ranger-2.0.tar.gz` & `tmp/report_ranger-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Report-Ranger-2.0.tar", max compression
+gzip compressed data, was "report_ranger-2.1.tar", max compression
```

## Comparing `Report-Ranger-2.0.tar` & `report_ranger-2.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rwxr-xr-x   0        0        0      463 2023-05-26 00:14:23.375274 Report-Ranger-2.0/pyproject.toml
--rwxr-xr-x   0        0        0       33 2021-09-15 13:25:33.000000 Report-Ranger-2.0/report_ranger/__init__.py
--rwxr-xr-x   0        0        0     1064 2023-04-24 00:31:02.414450 Report-Ranger-2.0/report_ranger/config.py
--rwxr-xr-x   0        0        0     8812 2023-05-02 03:51:52.380891 Report-Ranger-2.0/report_ranger/contentassistant.py
--rwxr-xr-x   0        0        0     3806 2023-05-02 06:44:16.057745 Report-Ranger-2.0/report_ranger/environment.py
--rwxr-xr-x   0        0        0      217 2021-09-15 13:25:33.000000 Report-Ranger-2.0/report_ranger/errors.py
--rwxr-xr-x   0        0        0    12991 2023-04-13 07:20:23.609912 Report-Ranger-2.0/report_ranger/helpers.py
--rwxr-xr-x   0        0        0     3034 2023-03-23 05:17:42.138978 Report-Ranger-2.0/report_ranger/imports/imports.py
--rwxr-xr-x   0        0        0     4473 2023-05-23 22:45:26.028951 Report-Ranger-2.0/report_ranger/imports/section.py
--rwxr-xr-x   0        0        0    20287 2023-05-23 07:27:07.987448 Report-Ranger-2.0/report_ranger/imports/vulnerability.py
--rwxr-xr-x   0        0        0     3210 2023-03-23 05:17:42.140109 Report-Ranger-2.0/report_ranger/markdown_renderer/csvrenderer.py
--rwxr-xr-x   0        0        0     4266 2023-04-28 02:59:32.119136 Report-Ranger-2.0/report_ranger/markdown_renderer/latexrenderer.py
--rwxr-xr-x   0        0        0     2682 2023-04-29 06:11:16.074523 Report-Ranger-2.0/report_ranger/markdown_renderer/typstrenderer.py
--rwxr-xr-x   0        0        0     3810 2023-05-23 07:19:00.069356 Report-Ranger-2.0/report_ranger/output_formatter/csvformatter.py
--rwxr-xr-x   0        0        0     1336 2023-05-23 07:18:57.380497 Report-Ranger-2.0/report_ranger/output_formatter/docxformatter.py
--rwxr-xr-x   0        0        0     4519 2023-05-23 07:18:54.540800 Report-Ranger-2.0/report_ranger/output_formatter/htmlformatter.py
--rwxr-xr-x   0        0        0    20061 2023-05-23 07:18:51.519431 Report-Ranger-2.0/report_ranger/output_formatter/latexformatter.py
--rwxr-xr-x   0        0        0    32470 2023-05-24 01:30:53.846118 Report-Ranger-2.0/report_ranger/output_formatter/outputformatter.py
--rwxr-xr-x   0        0        0     5764 2023-05-23 07:19:04.716847 Report-Ranger-2.0/report_ranger/output_formatter/typstformatter.py
--rwxr-xr-x   0        0        0    11488 2023-05-24 01:37:48.702425 Report-Ranger-2.0/report_ranger/report.py
--rwxr-xr-x   0        0        0     7227 2023-05-23 22:42:30.650688 Report-Ranger-2.0/report_ranger/report_ranger.py
--rwxr-xr-x   0        0        0     8290 2023-03-23 05:17:42.147623 Report-Ranger-2.0/report_ranger/riskassessment.py
--rwxr-xr-x   0        0        0     3019 2022-05-27 05:01:58.000000 Report-Ranger-2.0/report_ranger/styles.py
--rwxr-xr-x   0        0        0    19313 2023-03-23 05:17:42.148620 Report-Ranger-2.0/report_ranger/table.py
--rwxr-xr-x   0        0        0     1442 2023-05-02 06:37:25.929867 Report-Ranger-2.0/report_ranger/template.py
--rwxr-xr-x   0        0        0     2119 2023-03-23 05:17:42.150976 Report-Ranger-2.0/report_ranger/templatemapper.py
--rwxr-xr-x   0        0        0      555 2023-04-28 02:54:06.713280 Report-Ranger-2.0/report_ranger/utils/jinja_helpers.py
--rwxr-xr-x   0        0        0    20774 2023-05-24 08:00:56.417779 Report-Ranger-2.0/report_ranger/utils/mdread.py
--rwxr-xr-x   0        0        0     1138 2022-05-27 05:01:58.000000 Report-Ranger-2.0/report_ranger/validation.py
--rwxr-xr-x   0        0        0     2833 2023-05-23 22:43:39.663890 Report-Ranger-2.0/report_ranger/watcher.py
--rw-r--r--   0        0        0      893 2023-05-26 00:27:34.070409 Report-Ranger-2.0/setup.py
--rw-r--r--   0        0        0      597 2023-05-26 00:27:34.070641 Report-Ranger-2.0/PKG-INFO
+-rwxr-xr-x   0        0        0      696 2023-05-29 10:02:23.845368 report_ranger-2.1/pyproject.toml
+-rwxr-xr-x   0        0        0       33 2021-09-15 13:25:33.000000 report_ranger-2.1/report_ranger/__init__.py
+-rwxr-xr-x   0        0        0     1582 2023-05-29 09:44:19.406291 report_ranger-2.1/report_ranger/config.py
+-rwxr-xr-x   0        0        0     8812 2023-05-02 03:51:52.380891 report_ranger-2.1/report_ranger/contentassistant.py
+-rwxr-xr-x   0        0        0     3806 2023-05-02 06:44:16.057745 report_ranger-2.1/report_ranger/environment.py
+-rwxr-xr-x   0        0        0      217 2021-09-15 13:25:33.000000 report_ranger-2.1/report_ranger/errors.py
+-rwxr-xr-x   0        0        0    12991 2023-04-13 07:20:23.609912 report_ranger-2.1/report_ranger/helpers.py
+-rwxr-xr-x   0        0        0     3034 2023-03-23 05:17:42.138978 report_ranger-2.1/report_ranger/imports/imports.py
+-rwxr-xr-x   0        0        0     4473 2023-05-23 22:45:26.028951 report_ranger-2.1/report_ranger/imports/section.py
+-rwxr-xr-x   0        0        0    20287 2023-05-23 07:27:07.987448 report_ranger-2.1/report_ranger/imports/vulnerability.py
+-rwxr-xr-x   0        0        0     3210 2023-03-23 05:17:42.140109 report_ranger-2.1/report_ranger/markdown_renderer/csvrenderer.py
+-rwxr-xr-x   0        0        0     4266 2023-04-28 02:59:32.119136 report_ranger-2.1/report_ranger/markdown_renderer/latexrenderer.py
+-rwxr-xr-x   0        0        0     2682 2023-04-29 06:11:16.074523 report_ranger-2.1/report_ranger/markdown_renderer/typstrenderer.py
+-rwxr-xr-x   0        0        0     3810 2023-05-23 07:19:00.069356 report_ranger-2.1/report_ranger/output_formatter/csvformatter.py
+-rwxr-xr-x   0        0        0     1336 2023-05-23 07:18:57.380497 report_ranger-2.1/report_ranger/output_formatter/docxformatter.py
+-rwxr-xr-x   0        0        0     4519 2023-05-23 07:18:54.540800 report_ranger-2.1/report_ranger/output_formatter/htmlformatter.py
+-rwxr-xr-x   0        0        0    20061 2023-05-23 07:18:51.519431 report_ranger-2.1/report_ranger/output_formatter/latexformatter.py
+-rwxr-xr-x   0        0        0    32470 2023-05-24 01:30:53.846118 report_ranger-2.1/report_ranger/output_formatter/outputformatter.py
+-rwxr-xr-x   0        0        0     5764 2023-05-23 07:19:04.716847 report_ranger-2.1/report_ranger/output_formatter/typstformatter.py
+-rwxr-xr-x   0        0        0    11488 2023-05-24 01:37:48.702425 report_ranger-2.1/report_ranger/report.py
+-rwxr-xr-x   0        0        0     9434 2023-05-29 09:44:01.878256 report_ranger-2.1/report_ranger/report_ranger.py
+-rwxr-xr-x   0        0        0     8290 2023-03-23 05:17:42.147623 report_ranger-2.1/report_ranger/riskassessment.py
+-rwxr-xr-x   0        0        0     3019 2022-05-27 05:01:58.000000 report_ranger-2.1/report_ranger/styles.py
+-rwxr-xr-x   0        0        0    19313 2023-03-23 05:17:42.148620 report_ranger-2.1/report_ranger/table.py
+-rwxr-xr-x   0        0        0     1442 2023-05-02 06:37:25.929867 report_ranger-2.1/report_ranger/template.py
+-rwxr-xr-x   0        0        0     2119 2023-03-23 05:17:42.150976 report_ranger-2.1/report_ranger/templatemapper.py
+-rwxr-xr-x   0        0        0      555 2023-04-28 02:54:06.713280 report_ranger-2.1/report_ranger/utils/jinja_helpers.py
+-rwxr-xr-x   0        0        0    20774 2023-05-24 08:00:56.417779 report_ranger-2.1/report_ranger/utils/mdread.py
+-rwxr-xr-x   0        0        0     1138 2022-05-27 05:01:58.000000 report_ranger-2.1/report_ranger/validation.py
+-rwxr-xr-x   0        0        0     2833 2023-05-23 22:43:39.663890 report_ranger-2.1/report_ranger/watcher.py
+-rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 report_ranger-2.1/setup.py
+-rw-r--r--   0        0        0      956 1970-01-01 00:00:00.000000 report_ranger-2.1/PKG-INFO
```

### Comparing `Report-Ranger-2.0/report_ranger/contentassistant.py` & `report_ranger-2.1/report_ranger/contentassistant.py`

 * *Files identical despite different names*

### Comparing `Report-Ranger-2.0/report_ranger/environment.py` & `report_ranger-2.1/report_ranger/environment.py`

 * *Files identical despite different names*

### Comparing `Report-Ranger-2.0/report_ranger/helpers.py` & `report_ranger-2.1/report_ranger/helpers.py`

 * *Files identical despite different names*

### Comparing `Report-Ranger-2.0/report_ranger/imports/imports.py` & `report_ranger-2.1/report_ranger/imports/imports.py`

 * *Files identical despite different names*

### Comparing `Report-Ranger-2.0/report_ranger/imports/section.py` & `report_ranger-2.1/report_ranger/imports/section.py`

 * *Files identical despite different names*

### Comparing `Report-Ranger-2.0/report_ranger/imports/vulnerability.py` & `report_ranger-2.1/report_ranger/imports/vulnerability.py`

 * *Files identical despite different names*

### Comparing `Report-Ranger-2.0/report_ranger/markdown_renderer/csvrenderer.py` & `report_ranger-2.1/report_ranger/markdown_renderer/csvrenderer.py`

 * *Files identical despite different names*

### Comparing `Report-Ranger-2.0/report_ranger/markdown_renderer/latexrenderer.py` & `report_ranger-2.1/report_ranger/markdown_renderer/latexrenderer.py`

 * *Files identical despite different names*

### Comparing `Report-Ranger-2.0/report_ranger/markdown_renderer/typstrenderer.py` & `report_ranger-2.1/report_ranger/markdown_renderer/typstrenderer.py`

 * *Files identical despite different names*

### Comparing `Report-Ranger-2.0/report_ranger/output_formatter/csvformatter.py` & `report_ranger-2.1/report_ranger/output_formatter/csvformatter.py`

 * *Files identical despite different names*

### Comparing `Report-Ranger-2.0/report_ranger/output_formatter/docxformatter.py` & `report_ranger-2.1/report_ranger/output_formatter/docxformatter.py`

 * *Files identical despite different names*

### Comparing `Report-Ranger-2.0/report_ranger/output_formatter/htmlformatter.py` & `report_ranger-2.1/report_ranger/output_formatter/htmlformatter.py`

 * *Files identical despite different names*

### Comparing `Report-Ranger-2.0/report_ranger/output_formatter/latexformatter.py` & `report_ranger-2.1/report_ranger/output_formatter/latexformatter.py`

 * *Files identical despite different names*

### Comparing `Report-Ranger-2.0/report_ranger/output_formatter/outputformatter.py` & `report_ranger-2.1/report_ranger/output_formatter/outputformatter.py`

 * *Files identical despite different names*

### Comparing `Report-Ranger-2.0/report_ranger/output_formatter/typstformatter.py` & `report_ranger-2.1/report_ranger/output_formatter/typstformatter.py`

 * *Files identical despite different names*

### Comparing `Report-Ranger-2.0/report_ranger/report.py` & `report_ranger-2.1/report_ranger/report.py`

 * *Files identical despite different names*

### Comparing `Report-Ranger-2.0/report_ranger/riskassessment.py` & `report_ranger-2.1/report_ranger/riskassessment.py`

 * *Files identical despite different names*

### Comparing `Report-Ranger-2.0/report_ranger/styles.py` & `report_ranger-2.1/report_ranger/styles.py`

 * *Files identical despite different names*

### Comparing `Report-Ranger-2.0/report_ranger/table.py` & `report_ranger-2.1/report_ranger/table.py`

 * *Files identical despite different names*

### Comparing `Report-Ranger-2.0/report_ranger/template.py` & `report_ranger-2.1/report_ranger/template.py`

 * *Files identical despite different names*

### Comparing `Report-Ranger-2.0/report_ranger/templatemapper.py` & `report_ranger-2.1/report_ranger/templatemapper.py`

 * *Files identical despite different names*

### Comparing `Report-Ranger-2.0/report_ranger/utils/jinja_helpers.py` & `report_ranger-2.1/report_ranger/utils/jinja_helpers.py`

 * *Files identical despite different names*

### Comparing `Report-Ranger-2.0/report_ranger/utils/mdread.py` & `report_ranger-2.1/report_ranger/utils/mdread.py`

 * *Files identical despite different names*

### Comparing `Report-Ranger-2.0/report_ranger/validation.py` & `report_ranger-2.1/report_ranger/validation.py`

 * *Files identical despite different names*

### Comparing `Report-Ranger-2.0/report_ranger/watcher.py` & `report_ranger-2.1/report_ranger/watcher.py`

 * *Files identical despite different names*

### Comparing `Report-Ranger-2.0/setup.py` & `report_ranger-2.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,30 +17,35 @@
  'jinja2',
  'kaleido==0.2.1',
  'mistune',
  'num2words',
  'numpy',
  'openpyxl',
  'pandas',
+ 'platformdirs>=3.5.1,<4.0.0',
  'plotly',
  'pyyaml',
  'tabulate',
  'watchdog']
 
+entry_points = \
+{'console_scripts': ['reportranger = report_ranger:main']}
+
 setup_kwargs = {
     'name': 'report-ranger',
-    'version': '2.0',
+    'version': '2.1',
     'description': 'Create a report using markdown files.',
-    'long_description': None,
+    'long_description': 'None',
     'author': 'Matthew Strahan',
     'author_email': 'matt@volkis.com.au',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'https://gitlab.com/volkis/report-ranger/',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
+    'entry_points': entry_points,
     'python_requires': '>=3.10,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

