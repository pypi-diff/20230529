# Comparing `tmp/damo-1.8.2.tar.gz` & `tmp/damo-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "damo-1.8.2.tar", last modified: Mon May 22 22:44:21 2023, max compression
+gzip compressed data, was "damo-1.8.3.tar", last modified: Mon May 29 19:25:42 2023, max compression
```

## Comparing `damo-1.8.2.tar` & `damo-1.8.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-05-22 22:44:21.654233 damo-1.8.2/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     6986 2023-05-22 22:44:21.654233 damo-1.8.2/PKG-INFO
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     6465 2023-05-22 22:44:17.000000 damo-1.8.2/README.md
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      104 2023-05-22 22:44:17.000000 damo-1.8.2/pyproject.toml
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       38 2023-05-22 22:44:21.654233 damo-1.8.2/setup.cfg
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1104 2023-05-22 22:44:17.000000 damo-1.8.2/setup.py
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-05-22 22:44:21.638234 damo-1.8.2/src/
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-05-22 22:44:21.654233 damo-1.8.2/src/damo/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        0 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/__init__.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      963 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/_damo_deprecation_notice.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      620 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/_damo_dist.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     9673 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/_damo_fmt_str.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2995 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/_damo_fs.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5345 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/_damo_paddr_layout.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      825 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/_damo_python2_support.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      739 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/_damo_subcmds.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    35686 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/_damon.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    10453 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/_damon_args.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8303 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/_damon_args_schemes.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    17745 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/_damon_dbgfs.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    20974 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/_damon_result.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    19321 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/_damon_sysfs.py
--rwxrwxr-x   0 sjpark    (1000) sjpark    (1000)     3753 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2002 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_adjust.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      891 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_convert_record_format.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1147 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_features.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      746 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_fmt_json.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    13289 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_heats.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4668 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_lru_sort.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3029 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_monitor.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2749 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_nr_regions.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4458 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_reclaim.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5077 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_record.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1312 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_report.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1094 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_report_json.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2947 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_report_raw.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1588 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_schemes.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      542 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_start.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2383 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_stat.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1522 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_stat_kdamonds.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3056 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_stat_regions.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2786 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_stat_schemes.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      654 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_stop.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      705 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_translate_damos.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      627 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_tune.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3943 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_validate.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       22 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_version.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5553 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_wss.py
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-05-22 22:44:21.654233 damo-1.8.2/src/damo.egg-info/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     6986 2023-05-22 22:44:21.000000 damo-1.8.2/src/damo.egg-info/PKG-INFO
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1240 2023-05-22 22:44:21.000000 damo-1.8.2/src/damo.egg-info/SOURCES.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        1 2023-05-22 22:44:21.000000 damo-1.8.2/src/damo.egg-info/dependency_links.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       40 2023-05-22 22:44:21.000000 damo-1.8.2/src/damo.egg-info/entry_points.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        5 2023-05-22 22:44:21.000000 damo-1.8.2/src/damo.egg-info/top_level.txt
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-05-29 19:25:42.989174 damo-1.8.3/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8106 2023-05-29 19:25:42.989174 damo-1.8.3/PKG-INFO
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7585 2023-05-29 19:25:38.000000 damo-1.8.3/README.md
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      104 2023-05-29 19:25:38.000000 damo-1.8.3/pyproject.toml
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       38 2023-05-29 19:25:42.989174 damo-1.8.3/setup.cfg
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1104 2023-05-29 19:25:38.000000 damo-1.8.3/setup.py
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-05-29 19:25:42.977174 damo-1.8.3/src/
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-05-29 19:25:42.989174 damo-1.8.3/src/damo/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        0 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/__init__.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7186 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/_damo_deprecated.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      963 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/_damo_deprecation_notice.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      620 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/_damo_dist.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     9673 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/_damo_fmt_str.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2995 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/_damo_fs.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5345 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/_damo_paddr_layout.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      825 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/_damo_python2_support.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      739 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/_damo_subcmds.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    34482 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/_damon.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    11111 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/_damon_args.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    17105 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/_damon_dbgfs.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    21100 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/_damon_result.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    19142 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/_damon_sysfs.py
+-rwxrwxr-x   0 sjpark    (1000) sjpark    (1000)     3753 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2002 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_adjust.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      891 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_convert_record_format.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1147 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_features.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      746 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_fmt_json.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    13289 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_heats.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4668 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_lru_sort.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3029 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_monitor.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2749 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_nr_regions.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4458 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_reclaim.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5278 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_record.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1312 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_report.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1094 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_report_json.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2947 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_report_raw.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1584 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_schemes.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      542 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_start.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2383 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_stat.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1522 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_stat_kdamonds.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3056 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_stat_regions.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2786 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_stat_schemes.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      654 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_stop.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      865 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_translate_damos.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      627 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_tune.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3943 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_validate.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       22 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_version.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5553 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_wss.py
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-05-29 19:25:42.989174 damo-1.8.3/src/damo.egg-info/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8106 2023-05-29 19:25:42.000000 damo-1.8.3/src/damo.egg-info/PKG-INFO
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1237 2023-05-29 19:25:42.000000 damo-1.8.3/src/damo.egg-info/SOURCES.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        1 2023-05-29 19:25:42.000000 damo-1.8.3/src/damo.egg-info/dependency_links.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       40 2023-05-29 19:25:42.000000 damo-1.8.3/src/damo.egg-info/entry_points.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        5 2023-05-29 19:25:42.000000 damo-1.8.3/src/damo.egg-info/top_level.txt
```

### Comparing `damo-1.8.2/PKG-INFO` & `damo-1.8.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: damo
-Version: 1.8.2
-Summary: DAMON user-space tool
-Home-page: https://github.com/awslabs/damo
-Author: SeongJae Park
-Author-email: sj@kernel.org
-Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
-Project-URL: DAMON, https://damonitor.github.io
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 DAMO: Data Access Monitoring Operator
 =====================================
 
 `damo` is a user space tool for [DAMON](https://damonitor.github.io).  Using
 this, you can monitor the data access patterns of your system or workloads and
 make data access-aware memory management optimizations.
 
@@ -42,16 +27,16 @@
     $ # ensure your kernel is built with CONFIG_DAMON_*=y
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.2/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.2/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.3/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.3/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -59,15 +44,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.2/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.3/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -87,37 +72,22 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-I show --rbuf option from `damo record` is removed.  What happened?
--------------------------------------------------------------------
-
-The option is deprecated.  Please report your usecase to sj@kernel.org,
-damon@lists.linux.dev and linux-mm@kvack.org if you depend on those.
-
-
-damo suddenly exit with `You're using deprecated single line DAMOS format` message. Why?
-----------------------------------------------------------------------------------------
-
-Because the single line DAMOS scheme format is no more supported.  You can
-convert your old DAMOS schemes to supported format by checking v1.8.1 of damo
-and using `damo translate_damos` command.  Please report your usecase to
-sj@kernel.org, damon@lists.linux.dev and linux-mm@kvack.org if you depend on
-the old format.
-
+Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.3/USAGE.md) file?
+---------------------------------------------------------------------
 
-damo suddenly prints `Python2 support of damo is deprecated` message. Why?
---------------------------------------------------------------------------
-
-Because Python2 is no more supported.  Please report your usecase to
-sj@kernel.org, damon@lists.linux.dev and linux-mm@kvack.org if you depend on
-those.
+Only sufficiently stabilized features are documented there.  In other words,
+any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.3/USAGE.md) are in experimental
+stage.  Such experimental features could be deprecated and removed without any
+notice and grace priods.  The documented features could also be deprecated, but
+those will provide some notification and grace periods.
 
 
 Recording Data Access Patterns
 ==============================
 
 Below commands record memory access patterns of a program and save the
 monitoring results in `damon.data` file.
@@ -167,15 +137,62 @@
 make your workload more memory efficient with only a modest performance
 overhead.
 
     $ sudo damo schemes --damos_access_rate 0 0 --damos_sz_region 4K max \
                         --damos_age 60s max --damos_action pageout \
                         <pid of your workload>
 
-Note: Previously, one-line scheme specification format like below was used.  It
-is now DEPRECATED.  Please report your usecase to sj@kernel.org,
-damon@lists.linux.dev and linux-mm@kvack.org if you depend on those.
-
-    $ # !!! BELOW IS NO MORE SUPPORTED
-    $ echo "#min-size max-size min-acc max-acc min-age max-age action" > my_scheme
-    $ echo "4K        max      0       0       60s     max     pageout" >> my_scheme
-    $ sudo damo schemes -c my_scheme <pid of your workload>
+
+Deprecated Features
+===================
+
+Below are features that deprecated, or will be deprecated.  If you depend on
+any of those, please report your usecase to the community via github issue,
+sj@kernel.org, damon@lists.linux.dev, and/or linux-mm@kvack.org.
+
+--rbuf option of `damo record`
+------------------------------
+
+Deprecated.
+
+Early versions of DAMON supported in-kernel direct monitoring results record
+file generation.  To control the overhead of it, DAMO allowed user to specify
+the size of buffer for the work.  The feature has not merged into the mainline,
+and discarded.  Hence the option was available for only few kernels that ported
+the feature.  For most of kernels, tracepoint based record file generation is
+being used, and the overhead of the approach is subtle.  Hence, the option has
+deprecated.
+
+
+DAMOS singline format
+---------------------
+
+Deprecated.  Use `--damos_*` command line options or json format input.
+
+One-line scheme specification format like below was initially supported.
+Because it is not flexible for extension of features, it has deprecated now.
+You may use `--damos_*` command line options or json format instead.  You may
+use `damo translate_damos` to convert your old single line DAMOS schemes
+specification to the new json format.
+
+
+`Python2 support
+----------------
+
+Deprecated.  Use Python3.
+
+For some old distros, DAMO initially supported Python2.  Because Python2 is
+really old now, the support has deprecated.  Please use Python3 or newer.
+
+
+DAMON record binary format
+--------------------------
+
+Will be deprecated by 2023 Q3.
+
+At the beginning, DAMO used its special binary format, namely `record`.  It is
+designed for lightweight saving of the monitoring results.  It is difficult to
+read, and not that efficient compared to fancy compression techniques.  `json`
+based monitoring results can be easier to read, and more efficient when
+compression technique is used.  Hence, the format will be deprecated.  You may
+use `damo convert_record_format` to convert your old record binary format
+monitoring results files to the new format.
```

### Comparing `damo-1.8.2/README.md` & `damo-1.8.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: damo
+Version: 1.8.3
+Summary: DAMON user-space tool
+Home-page: https://github.com/awslabs/damo
+Author: SeongJae Park
+Author-email: sj@kernel.org
+Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
+Project-URL: DAMON, https://damonitor.github.io
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
+Classifier: Operating System :: POSIX :: Linux
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
 DAMO: Data Access Monitoring Operator
 =====================================
 
 `damo` is a user space tool for [DAMON](https://damonitor.github.io).  Using
 this, you can monitor the data access patterns of your system or workloads and
 make data access-aware memory management optimizations.
 
@@ -27,16 +42,16 @@
     $ # ensure your kernel is built with CONFIG_DAMON_*=y
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.2/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.2/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.3/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.3/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -44,15 +59,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.2/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.3/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -72,37 +87,22 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-I show --rbuf option from `damo record` is removed.  What happened?
--------------------------------------------------------------------
-
-The option is deprecated.  Please report your usecase to sj@kernel.org,
-damon@lists.linux.dev and linux-mm@kvack.org if you depend on those.
-
-
-damo suddenly exit with `You're using deprecated single line DAMOS format` message. Why?
-----------------------------------------------------------------------------------------
-
-Because the single line DAMOS scheme format is no more supported.  You can
-convert your old DAMOS schemes to supported format by checking v1.8.1 of damo
-and using `damo translate_damos` command.  Please report your usecase to
-sj@kernel.org, damon@lists.linux.dev and linux-mm@kvack.org if you depend on
-the old format.
-
+Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.3/USAGE.md) file?
+---------------------------------------------------------------------
 
-damo suddenly prints `Python2 support of damo is deprecated` message. Why?
---------------------------------------------------------------------------
-
-Because Python2 is no more supported.  Please report your usecase to
-sj@kernel.org, damon@lists.linux.dev and linux-mm@kvack.org if you depend on
-those.
+Only sufficiently stabilized features are documented there.  In other words,
+any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.3/USAGE.md) are in experimental
+stage.  Such experimental features could be deprecated and removed without any
+notice and grace priods.  The documented features could also be deprecated, but
+those will provide some notification and grace periods.
 
 
 Recording Data Access Patterns
 ==============================
 
 Below commands record memory access patterns of a program and save the
 monitoring results in `damon.data` file.
@@ -152,15 +152,62 @@
 make your workload more memory efficient with only a modest performance
 overhead.
 
     $ sudo damo schemes --damos_access_rate 0 0 --damos_sz_region 4K max \
                         --damos_age 60s max --damos_action pageout \
                         <pid of your workload>
 
-Note: Previously, one-line scheme specification format like below was used.  It
-is now DEPRECATED.  Please report your usecase to sj@kernel.org,
-damon@lists.linux.dev and linux-mm@kvack.org if you depend on those.
-
-    $ # !!! BELOW IS NO MORE SUPPORTED
-    $ echo "#min-size max-size min-acc max-acc min-age max-age action" > my_scheme
-    $ echo "4K        max      0       0       60s     max     pageout" >> my_scheme
-    $ sudo damo schemes -c my_scheme <pid of your workload>
+
+Deprecated Features
+===================
+
+Below are features that deprecated, or will be deprecated.  If you depend on
+any of those, please report your usecase to the community via github issue,
+sj@kernel.org, damon@lists.linux.dev, and/or linux-mm@kvack.org.
+
+--rbuf option of `damo record`
+------------------------------
+
+Deprecated.
+
+Early versions of DAMON supported in-kernel direct monitoring results record
+file generation.  To control the overhead of it, DAMO allowed user to specify
+the size of buffer for the work.  The feature has not merged into the mainline,
+and discarded.  Hence the option was available for only few kernels that ported
+the feature.  For most of kernels, tracepoint based record file generation is
+being used, and the overhead of the approach is subtle.  Hence, the option has
+deprecated.
+
+
+DAMOS singline format
+---------------------
+
+Deprecated.  Use `--damos_*` command line options or json format input.
+
+One-line scheme specification format like below was initially supported.
+Because it is not flexible for extension of features, it has deprecated now.
+You may use `--damos_*` command line options or json format instead.  You may
+use `damo translate_damos` to convert your old single line DAMOS schemes
+specification to the new json format.
+
+
+`Python2 support
+----------------
+
+Deprecated.  Use Python3.
+
+For some old distros, DAMO initially supported Python2.  Because Python2 is
+really old now, the support has deprecated.  Please use Python3 or newer.
+
+
+DAMON record binary format
+--------------------------
+
+Will be deprecated by 2023 Q3.
+
+At the beginning, DAMO used its special binary format, namely `record`.  It is
+designed for lightweight saving of the monitoring results.  It is difficult to
+read, and not that efficient compared to fancy compression techniques.  `json`
+based monitoring results can be easier to read, and more efficient when
+compression technique is used.  Hence, the format will be deprecated.  You may
+use `damo convert_record_format` to convert your old record binary format
+monitoring results files to the new format.
```

### Comparing `damo-1.8.2/setup.py` & `damo-1.8.3/setup.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.2/src/damo/_damo_deprecation_notice.py` & `damo-1.8.3/src/damo/_damo_deprecation_notice.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.2/src/damo/_damo_dist.py` & `damo-1.8.3/src/damo/_damo_dist.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.2/src/damo/_damo_fmt_str.py` & `damo-1.8.3/src/damo/_damo_fmt_str.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.2/src/damo/_damo_fs.py` & `damo-1.8.3/src/damo/_damo_fs.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.2/src/damo/_damo_paddr_layout.py` & `damo-1.8.3/src/damo/_damo_paddr_layout.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.2/src/damo/_damo_python2_support.py` & `damo-1.8.3/src/damo/_damo_python2_support.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.2/src/damo/_damo_subcmds.py` & `damo-1.8.3/src/damo/_damo_subcmds.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.2/src/damo/_damon.py` & `damo-1.8.3/src/damo/_damon.py`

 * *Files 2% similar despite different names*

```diff
@@ -703,58 +703,27 @@
         return (type(self) == type(other) and
                 self.access_pattern.effectively_equal(
                     other.access_pattern, intervals) and
                 self.action == other.action and self.quotas == other.quotas and
                 self.watermarks == other.watermarks and
                 self.filters == other.filters)
 
-class DamonRecord:
-    rfile_buf = None
-    rfile_path = None
-
-    def __init__(self, rfile_buf, rfile_path):
-        self.rfile_buf = _damo_fmt_str.text_to_bytes(rfile_buf)
-        self.rfile_path = rfile_path
-
-    def to_str(self, raw):
-        return 'path: %s, buffer sz: %s' % (self.rfile_path,
-                _damo_fmt_str.format_sz(self.rfile_buf, raw))
-
-    def __str__(self):
-        return self.to_str(False)
-
-    def __eq__(self, other):
-        return type(self) == type(other) and '%s' % self == '%s' % other
-
-    @classmethod
-    def from_kvpairs(cls, kv):
-        return DamonRecord(kv['rfile_buf'], kv['rfile_path'])
-
-    def to_kvpairs(self, raw=False):
-        return collections.OrderedDict(
-                [(attr, getattr(self, attr)) for attr in
-                    ['rfile_buf', 'rfile_path']])
-
 class DamonCtx:
     intervals = None
     nr_regions = None
     ops = None
     targets = None
     schemes = None
-    # For old downstream kernels that supports record feature
-    record_request = None
 
-    def __init__(self, intervals, nr_regions, ops, targets, schemes,
-            record_request=None):
+    def __init__(self, intervals, nr_regions, ops, targets, schemes):
         self.intervals = intervals
         self.nr_regions = nr_regions
         self.ops = ops
         self.targets = targets
         self.schemes = schemes
-        self.record_request = record_request
 
     def to_str(self, raw):
         lines = ['ops: %s' % self.ops]
         lines.append('intervals: %s' % self.intervals.to_str(raw))
         lines.append('nr_regions: %s' % self.nr_regions.to_str(raw))
         for idx, target in enumerate(self.targets):
             lines.append('target %d' % idx)
@@ -780,27 +749,23 @@
                     if 'intervals' in kv else DamonIntervals(),
                 DamonNrRegionsRange.from_kvpairs(kv['nr_regions'])
                     if 'nr_regions' in kv else DAmonNrRegionsRange(),
                 kv['ops'],
                 [DamonTarget.from_kvpairs(t) for t in kv['targets']],
                 [Damos.from_kvpairs(s) for s in kv['schemes']]
                     if 'schemes' in kv else [])
-        if 'record_request' in kv:
-            ctx.record_request = DamonRecord.from_kvpairs(kv['record_request'])
         return ctx
 
     def to_kvpairs(self, raw=False):
         kv = collections.OrderedDict({})
         kv['intervals'] = self.intervals.to_kvpairs(raw)
         kv['nr_regions'] = self.nr_regions.to_kvpairs(raw)
         kv['ops'] = self.ops
         kv['targets'] = [t.to_kvpairs(raw) for t in self.targets]
         kv['schemes'] = [s.to_kvpairs(raw) for s in self.schemes]
-        if self.record_request:
-            kv['record_request'] = self.record_request.to_kvpairs(raw)
         return kv
 
 def target_has_pid(ops):
     return ops in ['vaddr', 'fvaddr']
 
 class Kdamond:
     state = None
```

### Comparing `damo-1.8.2/src/damo/_damon_args.py` & `damo-1.8.3/src/damo/_damon_args.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 """
 Command line arguments handling
 """
 
 import argparse
 import json
+import os
 import subprocess
 
 import _damo_paddr_layout
-import _damon_args_schemes
 import _damon
 
 # Kdamonds construction from command line arguments
 
 def init_regions_for(args):
     init_regions = []
     if args.regions:
@@ -60,14 +60,50 @@
     range2 = _damon.DamonNrRegionsRange(*args.monitoring_nr_regions_range)
     if not range1 == default_range:
         return range1
     if not range2 == default_range:
         return range2
     return default_range
 
+def schemes_option_to_damos(schemes):
+    if os.path.isfile(schemes):
+        with open(schemes, 'r') as f:
+            schemes = f.read()
+
+    try:
+        kvpairs = json.loads(schemes)
+        return [_damon.Damos.from_kvpairs(kv) for kv in kvpairs], None
+    except Exception as json_err:
+        return None, '%s' % json_err
+
+def damos_options_to_scheme(args):
+    try:
+        return _damon.Damos(
+                access_pattern=_damon.DamosAccessPattern(
+                    args.damos_sz_region, args.damos_access_rate,
+                    _damon.unit_percent, args.damos_age, _damon.unit_usec),
+                action=args.damos_action), None
+    except Exception as e:
+        return None, 'Wrong \'--damos_*\' argument (%s)' % e
+
+def damos_for(args):
+    if args.damos_action:
+        damos, err = damos_options_to_scheme(args)
+        if err != None:
+            return None, err
+        return [damos], None
+
+    if not 'schemes' in args or args.schemes == None:
+        return [], None
+
+    schemes, err = schemes_option_to_damos(args.schemes)
+    if err:
+        return None, 'failed damo schemes arguents parsing (%s)' % err
+    return schemes, None
+
 def damon_ctx_for(args):
     try:
         intervals = damon_intervals_for(args)
     except Exception as e:
         return None, 'invalid intervals arguments (%s)' % e
     try:
         nr_regions = damon_nr_regions_range_for(args)
@@ -81,28 +117,20 @@
 
     try:
         target = _damon.DamonTarget(args.target_pid
                 if _damon.target_has_pid(ops) else None, init_regions)
     except Exception as e:
         return 'Wrong \'--target_pid\' argument (%s)' % e
 
-    record_request = None
-    if 'rbuf' in args and args.rbuf != None:
-        try:
-            record_request = _damon.DamonRecord(args.rbuf, args.out)
-        except Exception as e:
-            return None, 'Wrong record arguments (%s)' % e
-
-    schemes, err = _damon_args_schemes.damos_for(args)
+    schemes, err = damos_for(args)
     if err:
         return None, err
 
     try:
-        ctx = _damon.DamonCtx(intervals, nr_regions, ops, [target], schemes,
-                record_request)
+        ctx = _damon.DamonCtx(intervals, nr_regions, ops, [target], schemes)
         return ctx, None
     except Exception as e:
         return None, 'Creating context from arguments failed (%s)' % e
 
 def kdamonds_from_json_arg(arg):
     try:
         if os.path.isfile(arg):
@@ -272,14 +300,11 @@
 	    help='data access monitoring-based operation schemes')
     parser.add_argument('--kdamonds', metavar='<json string or file>',
             help='json format kdamonds specification to run DAMON for')
     parser.add_argument('deducible_target', type=str,
             metavar='<deducible target>', nargs='?',
             help='the target (command, pid, or special keywords) to monitor')
     if add_record_options:
-        # Uncomment if some dependant user found
-        # parser.add_argument('-l', '--rbuf', metavar='<len>', type=int,
-        #         help='length of record result buffer (!! DEPRECATED)')
         parser.add_argument('-o', '--out', metavar='<file path>', type=str,
                 default='damon.data', help='output file path')
     set_common_argparser(parser)
     return parser
```

### Comparing `damo-1.8.2/src/damo/_damon_args_schemes.py` & `damo-1.8.3/src/damo/_damo_deprecated.py`

 * *Files 16% similar despite different names*

```diff
@@ -170,58 +170,24 @@
         else:
             return None, 'expected %s fields, but \'%s\'' % (
                     [7, 9, 12, 17, 18], line)
     except:
         return None, 'wrong input field'
     return None, 'unsupported version of single line scheme'
 
-def schemes_option_to_damos(schemes):
+def damo_single_line_schemes_to_damos(schemes):
     if os.path.isfile(schemes):
         with open(schemes, 'r') as f:
             schemes = f.read()
 
-    try:
-        kvpairs = json.loads(schemes)
-        return [_damon.Damos.from_kvpairs(kv) for kv in kvpairs], None
-    except Exception as json_err:
-        # The input is not json file
-        pass
-
     # remove comments, empty lines, and unnecessary white spaces
     damo_schemes_lines = [l.strip() for l in schemes.strip().split('\n')
             if not l.strip().startswith('#') and l.strip() != '']
 
     damos_list = []
     for line in damo_schemes_lines:
         damos, err = damo_single_line_scheme_to_damos(line)
         if err != None:
-            return None, ('invalid input: ' +
-                    'neither json (%s), nor per-line scheme (%s)'
-                    % (json_err, err))
+            return None, 'invalid input: %s' % err
         damos.name = '%d' % len(damos_list)
         damos_list.append(damos)
     return damos_list, None
-
-def options_to_scheme(args):
-    try:
-        return _damon.Damos(
-                access_pattern=_damon.DamosAccessPattern(
-                    args.damos_sz_region, args.damos_access_rate,
-                    _damon.unit_percent, args.damos_age, _damon.unit_usec),
-                action=args.damos_action), None
-    except Exception as e:
-        return None, 'Wrong \'--damos_*\' argument (%s)' % e
-
-def damos_for(args):
-    if args.damos_action:
-        damos, err = options_to_scheme(args)
-        if err != None:
-            return None, err
-        return [damos], None
-
-    if not 'schemes' in args or args.schemes == None:
-        return [], None
-
-    schemes, err = schemes_option_to_damos(args.schemes)
-    if err:
-        return None, 'failed damo schemes arguents parsing (%s)' % err
-    return schemes, None
```

### Comparing `damo-1.8.2/src/damo/_damon_dbgfs.py` & `damo-1.8.3/src/damo/_damon_dbgfs.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 import _damo_deprecation_notice
 import _damo_fs
 import _damon
 
 debugfs = '/sys/kernel/debug'
 debugfs_damon = os.path.join(debugfs, 'damon')
 debugfs_attrs = os.path.join(debugfs_damon, 'attrs')
-debugfs_record = os.path.join(debugfs_damon, 'record')
 debugfs_schemes = os.path.join(debugfs_damon, 'schemes')
 debugfs_target_ids = os.path.join(debugfs_damon, 'target_ids')
 debugfs_init_regions = os.path.join(debugfs_damon, 'init_regions')
 debugfs_monitor_on = os.path.join(debugfs_damon, 'monitor_on')
 
 def turn_damon_on(kdamonds_idxs):
     return _damo_fs.write_files({debugfs_monitor_on: 'on'})
@@ -174,19 +173,14 @@
     write_contents = []
     write_contents.append({debugfs_attrs: attr_str_ctx(ctx)})
 
     if len(ctx.targets) > 0:
         write_contents += wops_for_target(ctx.targets[0],
                 _damon.target_has_pid(ctx.ops))
 
-    if feature_supported('record') and ctx.record_request != None:
-        record_file_input = '%s %s' % (ctx.record_request.rfile_buf,
-                ctx.record_request.rfile_path)
-        write_contents.append({debugfs_record: record_file_input})
-
     if not feature_supported('schemes'):
         return write_contents
 
     write_contents += wops_for_schemes(ctx.schemes, ctx.intervals)
 
     return write_contents
 
@@ -291,28 +285,22 @@
     for idx, target_id in enumerate(target_ids):
         targets.append(_damon.DamonTarget(
             pid=target_id if not is_paddr else None,
             regions=regions_dict[idx
                 if feature_supported('init_regions_target_idx')
                 else target_id] if len(regions_dict) > 0 else []))
 
-    if feature_supported('record'):
-        fields = files_content['record'].strip().split()
-        record_request = _damon.DamonRecord(int(fields[0]), fields[1].strip())
-
     schemes = []
     if feature_supported('schemes'):
         for line in files_content['schemes'].split('\n'):
             if line.strip() == '':
                 continue
             schemes.append(debugfs_output_to_damos(line, intervals))
 
     ctx = _damon.DamonCtx(intervals, nr_regions, ops, targets, schemes)
-    if feature_supported('record'):
-        ctx.record_request = record_request
     state = files_content['monitor_on'].strip()
     pid = files_content['kdamond_pid'].strip()
     return [_damon.Kdamond(state, pid, [ctx])]
 
 def current_kdamonds():
     return files_content_to_kdamonds(
             _damo_fs.read_files(debugfs_damon))
@@ -424,16 +412,14 @@
 
     if not os.path.isdir(debugfs_damon):
         return 'damon debugfs dir (%s) not found' % debugfs_damon
 
     if _damon.any_kdamond_running():
         return 'debugfs feature update cannot be done while DAMON running'
 
-    if os.path.isfile(debugfs_record):
-        feature_supports['record'] = True
     if os.path.isfile(debugfs_schemes):
         feature_supports['schemes'] = True
 
     # virtual address space has supported since the beginning
     feature_supports['vaddr'] = True
     if test_debugfs_file(debugfs_target_ids, 'paddr\n', '42\n'):
         feature_supports['paddr'] = True
```

### Comparing `damo-1.8.2/src/damo/_damon_result.py` & `damo-1.8.3/src/damo/_damon_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,16 +103,16 @@
         nr_accesses = struct.unpack('I', f.read(4))[0]
         region = _damon.DamonRegion(start_addr, end_addr,
                 nr_accesses, _damon.unit_samples,
                 None, _damon.unit_aggr_intervals)
         snapshot.regions.append(region)
     return snapshot
 
-# if number of snapshots is one, write_damon_record() adds a fake snapshot for
-# snapshot start time deduction.
+# if number of snapshots is one and the file type is record or perf script,
+# write_damon_result() adds a fake snapshot for snapshot start time deduction.
 def is_fake_snapshot(snapshot):
     if len(snapshot.regions) != 1:
         return False
     r = snapshot.regions[0]
     return (r.start == 0 and r.end == 0 and
             r.nr_accesses.samples == -1 and r.age.aggr_intervals == -1)
 
@@ -275,15 +275,15 @@
         try:
             with open(os.devnull, 'w') as fnull:
                 script_output = subprocess.check_output(
                         [PERF, 'script', '-i', result_file],
                         stderr=fnull).decode()
         except:
             pass
-    if script_output:
+    if script_output != None:
         result, err = perf_script_to_damon_result(script_output)
     else:
         warn_record_type_deprecation()
         result, err = record_to_damon_result(result_file)
 
     return result, err
 
@@ -362,15 +362,16 @@
 def write_damon_result(result, file_path, file_type, file_permission=None):
     '''Returns None if success, an error string otherwise'''
     if not file_type in self_write_supported_file_types:
         return 'write unsupported file type: %s' % file_type
 
     for record in result.records:
         snapshots = record.snapshots
-        if len(snapshots) == 1:
+        if len(snapshots) == 1 and file_type in [file_type_record,
+                file_type_perf_script]:
             # we cannot know start/end time of single snapshot from the file
             # to allow it with later read, write a fake snapshot
             snapshot = snapshots[0]
             snap_duration = snapshot.end_time - snapshot.start_time
             fake_snapshot = DAMONSnapshot(snapshot.end_time,
                     snapshot.end_time + snap_duration)
             # -1 nr_accesses.samples / -1 age.aggr_intervals means fake
```

### Comparing `damo-1.8.2/src/damo/_damon_sysfs.py` & `damo-1.8.3/src/damo/_damon_sysfs.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,17 +287,14 @@
         exit(1)
 
 def stage_kdamonds(kdamonds):
     if len(kdamonds) > 1:
         return 'currently only <=one kdamond is supported'
     if len(kdamonds) == 1 and len(kdamonds[0].contexts) > 1:
         return 'currently only <=one damon_ctx is supported'
-    if (len(kdamonds) == 1 and len(kdamonds[0].contexts) == 1 and
-            len(kdamonds[0].contexts[0].targets) > 1):
-        return 'currently only <=one target is supported'
     ensure_dirs_populated_for(kdamonds)
 
     return _damo_fs.write_files({kdamonds_dir: wops_for_kdamonds(kdamonds)})
 
 # for current_kdamonds()
 
 def numbered_dirs_content(files_content, nr_filename):
```

### Comparing `damo-1.8.2/src/damo/damo.py` & `damo-1.8.3/src/damo/damo.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.2/src/damo/damo_adjust.py` & `damo-1.8.3/src/damo/damo_adjust.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.2/src/damo/damo_convert_record_format.py` & `damo-1.8.3/src/damo/damo_convert_record_format.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.2/src/damo/damo_features.py` & `damo-1.8.3/src/damo/damo_features.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.2/src/damo/damo_fmt_json.py` & `damo-1.8.3/src/damo/damo_fmt_json.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.2/src/damo/damo_heats.py` & `damo-1.8.3/src/damo/damo_heats.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.2/src/damo/damo_lru_sort.py` & `damo-1.8.3/src/damo/damo_lru_sort.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.2/src/damo/damo_monitor.py` & `damo-1.8.3/src/damo/damo_monitor.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.2/src/damo/damo_nr_regions.py` & `damo-1.8.3/src/damo/damo_nr_regions.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.2/src/damo/damo_reclaim.py` & `damo-1.8.3/src/damo/damo_reclaim.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.2/src/damo/damo_record.py` & `damo-1.8.3/src/damo/damo_record.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,152 +2,170 @@
 
 """
 Record monitored data access patterns.
 """
 
 import os
 import signal
+import subprocess
+import time
 
-import _damo_deprecation_notice
 import _damon
 import _damon_args
 import _damon_result
 
 class DataForCleanup:
-    kdamonds_names = None
+    kdamonds_idxs = None
     orig_kdamonds = None
-    rfile_path = None
-    rfile_format = None
-    rfile_permission = None
     perf_pipe = None
 
 data_for_cleanup = DataForCleanup()
 
 def cleanup_exit(exit_code):
-    if data_for_cleanup.kdamonds_names != None:
+    if data_for_cleanup.kdamonds_idxs != None:
         # ignore returning error, as kdamonds may already finished
-        _damon.turn_damon_off(data_for_cleanup.kdamonds_names)
+        _damon.turn_damon_off(data_for_cleanup.kdamonds_idxs)
         err = _damon.stage_kdamonds(data_for_cleanup.orig_kdamonds)
         if err:
             print('failed restoring previous kdamonds setup (%s)' % err)
 
-    if exit_code in [-2, -3]:
-        exit(exit_code)
-
     if data_for_cleanup.perf_pipe:
         _damon_result.stop_monitoring_record(data_for_cleanup.perf_pipe)
-        exit(exit_code)
-
-    if data_for_cleanup.rfile_format != _damon_result.file_type_record:
-        err = _damon_result.update_result_file(data_for_cleanup.rfile_path,
-                data_for_cleanup.rfile_format)
-        if err != None:
-            print('converting format from record to %s failed (%s)' %
-                    (data_for_cleanup.rfile_format, err))
-    os.chmod(data_for_cleanup.rfile_path, data_for_cleanup.rfile_permission)
 
     exit(exit_code)
 
 def sighandler(signum, frame):
     print('\nsignal %s received' % signum)
     cleanup_exit(signum)
 
-def set_data_for_cleanup(data_for_cleanup, args, output_permission):
-    data_for_cleanup.rfile_format = args.output_type
-    data_for_cleanup.rfile_path = args.out
-    data_for_cleanup.rfile_permission = output_permission
-    data_for_cleanup.orig_kdamonds = _damon.current_kdamonds()
+def handle_args(args):
+    if _damon.any_kdamond_running() and not args.deducible_target:
+        args.deducible_target = 'ongoing'
 
-def chk_handle_record_feature_support(args):
-    # Comment below line if --rbuf dependent user found
-    return False
-
-    damon_record_supported = _damon.feature_supported('record')
-    if not damon_record_supported:
-        if args.rbuf:
-            print('# \'--rbuf\' will be ignored')
-
-    if damon_record_supported or args.rbuf:
-        _damo_deprecation_notice.deprecated(
-                feature='--rbuf option and in-kernel record feature support',
-                deadline='2023-Q2')
-
-    if not args.rbuf:
-        args.rbuf = 1024 * 1024
-
-    return damon_record_supported
-
-def chk_handle_output_permission(output_permission_option):
-    output_permission, err = _damon_result.parse_file_permission_str(
-            output_permission_option)
+    args.output_permission, err = _damon_result.parse_file_permission_str(
+            args.output_permission)
     if err != None:
-        print('wrong --output_permission (%s) (%s)' %
-                (output_permission_option, err))
+        print('wrong --output permission (%s) (%s)' %
+                (args.output_permission, err))
         exit(1)
-    return output_permission
 
-def backup_duplicate_output_file(output_file):
-    if os.path.isfile(output_file):
-        os.rename(output_file, output_file + '.old')
+    # backup duplicate output file
+    if os.path.isfile(args.out):
+        os.rename(args.out, args.out + '.old')
+
+    err = _damon_result.set_perf_path(args.perf_path)
+    if err != None:
+        print(err)
+        exit(-3)
+
+def pid_running(pid):
+    '''pid should be string'''
+    try:
+        subprocess.check_output(['ps', '--pid', pid])
+        return True
+    except:
+        return False
+
+def all_targets_terminated(targets):
+    for target in targets:
+        if pid_running('%s' % target.pid):
+            return False
+    return True
+
+def poll_target_pids(kdamonds, add_childs):
+    '''Return if polling should continued'''
+    current_targets = kdamonds[0].contexts[0].targets
+    if all_targets_terminated(current_targets):
+        return False
+    if not add_childs:
+        return True
+
+    for target in current_targets:
+        if target.pid == None:
+            continue
+        try:
+            childs_pids = subprocess.check_output(
+                    ['ps', '--ppid', '%s' % target.pid, '-o', 'pid=']
+                    ).decode().split()
+        except:
+            childs_pids = []
+        if len(childs_pids) == 0:
+            continue
+
+        # TODO: Commit all at once, out of this loop
+        new_targets = []
+        for child_pid in childs_pids:
+            # skip the child if already in the targets
+            if child_pid in ['%s' % t.pid for t in current_targets]:
+                continue
+            # remove already terminated targets, since committing already
+            # terminated targets to DAMON fails
+            new_targets = [target for target in current_targets
+                    if pid_running('%s' % target.pid)]
+            new_targets.append(_damon.DamonTarget(pid=child_pid, regions=[]))
+        if new_targets == []:
+            continue
+
+        # commit the new set of targets
+        kdamonds[0].contexts[0].targets = new_targets
+        err = _damon.commit(kdamonds)
+        if err != None:
+            # this might be not a problem; some of processes might
+            # finished meanwhile
+            print('adding child as target failed (%s)' % err)
+            cleanup_exit(1)
+    return True
 
 def set_argparser(parser):
     parser = _damon_args.set_argparser(parser, add_record_options=True)
     parser.add_argument('--output_type',
             choices=_damon_result.file_types,
             default=_damon_result.file_type_json_compressed,
             help='output file\'s type')
     parser.add_argument('--output_permission', type=str, default='600',
             help='permission of the output file')
     parser.add_argument('--perf_path', type=str, default='perf',
             help='path of perf tool ')
+    parser.add_argument('--include_childs', action='store_true',
+            help='record accesses of child processes')
     return parser
 
 def main(args=None):
     global data_for_cleanup
 
     if not args:
         parser = set_argparser(None)
         args = parser.parse_args()
 
     _damon.ensure_root_and_initialized(args)
 
-    # Check/handle the arguments and options
-    if _damon.any_kdamond_running() and not args.deducible_target:
-        args.deducible_target = 'ongoing'
-    damon_record_supported = chk_handle_record_feature_support(args)
-    output_permission = chk_handle_output_permission(args.output_permission)
-    backup_duplicate_output_file(args.out)
-
-    err = _damon_result.set_perf_path(args.perf_path)
-    if err != None:
-        print(err)
-        cleanup_exit(-3)
+    handle_args(args)
 
     # Setup for cleanup
-    set_data_for_cleanup(data_for_cleanup, args, output_permission)
+    data_for_cleanup.orig_kdamonds = _damon.current_kdamonds()
     signal.signal(signal.SIGINT, sighandler)
     signal.signal(signal.SIGTERM, sighandler)
 
     # Now the real works
     is_ongoing = _damon_args.is_ongoing_target(args)
     if not is_ongoing:
         err, kdamonds = _damon_args.turn_damon_on(args)
         if err:
             print('could not turn DAMON on (%s)' % err)
             cleanup_exit(-2)
-        data_for_cleanup.kdamonds_names = ['%d' % idx
+        data_for_cleanup.kdamonds_idxs = ['%d' % idx
                 for idx, k in enumerate(kdamonds)]
 
-    if not damon_record_supported or is_ongoing:
-        data_for_cleanup.perf_pipe = _damon_result.start_monitoring_record(
-                data_for_cleanup.rfile_path, data_for_cleanup.rfile_format,
-                data_for_cleanup.rfile_permission)
+    data_for_cleanup.perf_pipe = _damon_result.start_monitoring_record(
+            args.out, args.output_type, args.output_permission)
     print('Press Ctrl+C to stop')
 
     if _damon_args.self_started_target(args):
-        os.waitpid(kdamonds[0].contexts[0].targets[0].pid, 0)
+        while poll_target_pids(kdamonds, args.include_childs):
+            time.sleep(1)
+
     _damon.wait_current_kdamonds_turned_off()
 
     cleanup_exit(0)
 
 if __name__ == '__main__':
     main()
```

### Comparing `damo-1.8.2/src/damo/damo_report.py` & `damo-1.8.3/src/damo/damo_report.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.2/src/damo/damo_report_json.py` & `damo-1.8.3/src/damo/damo_report_json.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.2/src/damo/damo_report_raw.py` & `damo-1.8.3/src/damo/damo_report_raw.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.2/src/damo/damo_schemes.py` & `damo-1.8.3/src/damo/damo_schemes.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import signal
 
 import _damon
 import _damon_args
 
 def cleanup_exit(exit_code):
     # ignore returning error, as kdamonds may already finished
-    _damon.turn_damon_off(kdamonds_names)
+    _damon.turn_damon_off(kdamonds_idxs)
     if err:
         print('failed to turn damon off (%s)' % err)
     err = _damon.stage_kdamonds(orig_kdamonds)
     if err:
         print('failed restoring previous kdamonds setup (%s)' % err)
     exit(exit_code)
 
@@ -25,34 +25,34 @@
     cleanup_exit(signum)
 
 def set_argparser(parser):
     return _damon_args.set_argparser(parser, add_record_options=False)
 
 def main(args=None):
     global orig_kdamonds
-    global kdamonds_names
+    global kdamonds_idxs
 
     if not args:
         parser = set_argparser(None)
         args = parser.parse_args()
 
     _damon.ensure_root_and_initialized(args)
 
     orig_kdamonds = _damon.current_kdamonds()
-    kdamonds_names = []
+    kdamonds_idxs = []
 
     signal.signal(signal.SIGINT, sighandler)
     signal.signal(signal.SIGTERM, sighandler)
 
     err, kdamonds = _damon_args.turn_damon_on(args)
     if err:
         print('could not turn DAMON on (%s)' % err)
         cleanup_exit(-3)
 
-    kdamonds_names = ['%d' % idx for idx, k in enumerate(kdamonds)]
+    kdamonds_idxs = ['%d' % idx for idx, k in enumerate(kdamonds)]
 
     print('Press Ctrl+C to stop')
     if _damon_args.self_started_target(args):
         os.waitpid(kdamonds[0].contexts[0].targets[0].pid, 0)
     # damon will turn it off by itself if the target tasks are terminated.
     _damon.wait_current_kdamonds_turned_off()
```

### Comparing `damo-1.8.2/src/damo/damo_start.py` & `damo-1.8.3/src/damo/damo_start.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.2/src/damo/damo_stat.py` & `damo-1.8.3/src/damo/damo_stat.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.2/src/damo/damo_stat_kdamonds.py` & `damo-1.8.3/src/damo/damo_stat_kdamonds.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.2/src/damo/damo_stat_regions.py` & `damo-1.8.3/src/damo/damo_stat_regions.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.2/src/damo/damo_stat_schemes.py` & `damo-1.8.3/src/damo/damo_stat_schemes.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.2/src/damo/damo_stop.py` & `damo-1.8.3/src/damo/damo_stop.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.2/src/damo/damo_tune.py` & `damo-1.8.3/src/damo/damo_tune.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.2/src/damo/damo_validate.py` & `damo-1.8.3/src/damo/damo_validate.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.2/src/damo/damo_wss.py` & `damo-1.8.3/src/damo/damo_wss.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.2/src/damo.egg-info/PKG-INFO` & `damo-1.8.3/src/damo.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damo
-Version: 1.8.2
+Version: 1.8.3
 Summary: DAMON user-space tool
 Home-page: https://github.com/awslabs/damo
 Author: SeongJae Park
 Author-email: sj@kernel.org
 Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
 Project-URL: DAMON, https://damonitor.github.io
 Classifier: Programming Language :: Python :: 3
@@ -42,16 +42,16 @@
     $ # ensure your kernel is built with CONFIG_DAMON_*=y
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.2/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.2/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.3/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.3/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -59,15 +59,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.2/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.3/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -87,37 +87,22 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-I show --rbuf option from `damo record` is removed.  What happened?
--------------------------------------------------------------------
+Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.3/USAGE.md) file?
+---------------------------------------------------------------------
 
-The option is deprecated.  Please report your usecase to sj@kernel.org,
-damon@lists.linux.dev and linux-mm@kvack.org if you depend on those.
-
-
-damo suddenly exit with `You're using deprecated single line DAMOS format` message. Why?
-----------------------------------------------------------------------------------------
-
-Because the single line DAMOS scheme format is no more supported.  You can
-convert your old DAMOS schemes to supported format by checking v1.8.1 of damo
-and using `damo translate_damos` command.  Please report your usecase to
-sj@kernel.org, damon@lists.linux.dev and linux-mm@kvack.org if you depend on
-the old format.
-
-
-damo suddenly prints `Python2 support of damo is deprecated` message. Why?
---------------------------------------------------------------------------
-
-Because Python2 is no more supported.  Please report your usecase to
-sj@kernel.org, damon@lists.linux.dev and linux-mm@kvack.org if you depend on
-those.
+Only sufficiently stabilized features are documented there.  In other words,
+any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.3/USAGE.md) are in experimental
+stage.  Such experimental features could be deprecated and removed without any
+notice and grace priods.  The documented features could also be deprecated, but
+those will provide some notification and grace periods.
 
 
 Recording Data Access Patterns
 ==============================
 
 Below commands record memory access patterns of a program and save the
 monitoring results in `damon.data` file.
@@ -167,15 +152,62 @@
 make your workload more memory efficient with only a modest performance
 overhead.
 
     $ sudo damo schemes --damos_access_rate 0 0 --damos_sz_region 4K max \
                         --damos_age 60s max --damos_action pageout \
                         <pid of your workload>
 
-Note: Previously, one-line scheme specification format like below was used.  It
-is now DEPRECATED.  Please report your usecase to sj@kernel.org,
-damon@lists.linux.dev and linux-mm@kvack.org if you depend on those.
-
-    $ # !!! BELOW IS NO MORE SUPPORTED
-    $ echo "#min-size max-size min-acc max-acc min-age max-age action" > my_scheme
-    $ echo "4K        max      0       0       60s     max     pageout" >> my_scheme
-    $ sudo damo schemes -c my_scheme <pid of your workload>
+
+Deprecated Features
+===================
+
+Below are features that deprecated, or will be deprecated.  If you depend on
+any of those, please report your usecase to the community via github issue,
+sj@kernel.org, damon@lists.linux.dev, and/or linux-mm@kvack.org.
+
+--rbuf option of `damo record`
+------------------------------
+
+Deprecated.
+
+Early versions of DAMON supported in-kernel direct monitoring results record
+file generation.  To control the overhead of it, DAMO allowed user to specify
+the size of buffer for the work.  The feature has not merged into the mainline,
+and discarded.  Hence the option was available for only few kernels that ported
+the feature.  For most of kernels, tracepoint based record file generation is
+being used, and the overhead of the approach is subtle.  Hence, the option has
+deprecated.
+
+
+DAMOS singline format
+---------------------
+
+Deprecated.  Use `--damos_*` command line options or json format input.
+
+One-line scheme specification format like below was initially supported.
+Because it is not flexible for extension of features, it has deprecated now.
+You may use `--damos_*` command line options or json format instead.  You may
+use `damo translate_damos` to convert your old single line DAMOS schemes
+specification to the new json format.
+
+
+`Python2 support
+----------------
+
+Deprecated.  Use Python3.
+
+For some old distros, DAMO initially supported Python2.  Because Python2 is
+really old now, the support has deprecated.  Please use Python3 or newer.
+
+
+DAMON record binary format
+--------------------------
+
+Will be deprecated by 2023 Q3.
+
+At the beginning, DAMO used its special binary format, namely `record`.  It is
+designed for lightweight saving of the monitoring results.  It is difficult to
+read, and not that efficient compared to fancy compression techniques.  `json`
+based monitoring results can be easier to read, and more efficient when
+compression technique is used.  Hence, the format will be deprecated.  You may
+use `damo convert_record_format` to convert your old record binary format
+monitoring results files to the new format.
```

### Comparing `damo-1.8.2/src/damo.egg-info/SOURCES.txt` & `damo-1.8.3/src/damo.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 README.md
 pyproject.toml
 setup.py
 src/damo/__init__.py
+src/damo/_damo_deprecated.py
 src/damo/_damo_deprecation_notice.py
 src/damo/_damo_dist.py
 src/damo/_damo_fmt_str.py
 src/damo/_damo_fs.py
 src/damo/_damo_paddr_layout.py
 src/damo/_damo_python2_support.py
 src/damo/_damo_subcmds.py
 src/damo/_damon.py
 src/damo/_damon_args.py
-src/damo/_damon_args_schemes.py
 src/damo/_damon_dbgfs.py
 src/damo/_damon_result.py
 src/damo/_damon_sysfs.py
 src/damo/damo.py
 src/damo/damo_adjust.py
 src/damo/damo_convert_record_format.py
 src/damo/damo_features.py
```

