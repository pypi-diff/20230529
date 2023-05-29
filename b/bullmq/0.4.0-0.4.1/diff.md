# Comparing `tmp/bullmq-0.4.0.tar.gz` & `tmp/bullmq-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bullmq-0.4.0.tar", last modified: Thu May 18 22:19:58 2023, max compression
+gzip compressed data, was "bullmq-0.4.1.tar", last modified: Mon May 29 08:06:36 2023, max compression
```

## Comparing `bullmq-0.4.0.tar` & `bullmq-0.4.1.tar`

### file list

```diff
@@ -1,52 +1,61 @@
-drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-05-18 22:19:58.659998 bullmq-0.4.0/
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1651 2023-05-18 22:19:58.659561 bullmq-0.4.0/PKG-INFO
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      999 2023-05-04 10:32:52.000000 bullmq-0.4.0/README.md
-drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-05-18 22:19:58.629815 bullmq-0.4.0/bullmq/
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      269 2023-05-04 10:32:52.000000 bullmq-0.4.0/bullmq/__init__.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1291 2023-05-04 10:32:52.000000 bullmq-0.4.0/bullmq/backoffs.py
-drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-05-18 22:19:58.658790 bullmq-0.4.0/bullmq/commands/
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     8245 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/addJob-8.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      810 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/changeDelay-3.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     9375 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/cleanJobsInSet-2.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     5979 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/drain-4.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      501 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/extendLock-2.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      809 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/getCounts-1.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1748 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/getRanges-1.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1313 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/getState-7.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      934 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/getStateV2-7.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      897 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/isFinished-3.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      424 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/isJobInList-1.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      543 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/moveJobFromActiveToWait-4.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)    11863 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/moveStalledJobsToWait-8.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     7013 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/moveToActive-9.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     4123 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/moveToDelayed-8.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)    21423 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/moveToFinished-12.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1315 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/moveToWaitingChildren-4.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     7844 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/obliterate-2.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      522 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/pause-4.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1967 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/promote-6.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      292 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/releaseLock-1.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     7980 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/removeJob-1.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      666 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/removeRepeatable-2.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      846 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/reprocessJob-4.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     3150 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/retryJob-8.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1830 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/retryJobs-6.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      282 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/takeLock-1.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      246 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/updateData-1.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      420 2023-02-13 17:54:41.000000 bullmq-0.4.0/bullmq/commands/updateProgress-2.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      200 2023-04-18 08:29:50.000000 bullmq-0.4.0/bullmq/error_code.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      632 2023-04-18 08:29:50.000000 bullmq-0.4.0/bullmq/event_emitter.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     7277 2023-05-18 22:16:17.000000 bullmq-0.4.0/bullmq/job.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     4852 2023-05-04 10:32:52.000000 bullmq-0.4.0/bullmq/queue.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      833 2023-05-04 10:32:52.000000 bullmq-0.4.0/bullmq/redis_connection.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)    14763 2023-05-18 22:16:17.000000 bullmq-0.4.0/bullmq/scripts.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      699 2023-04-18 08:29:50.000000 bullmq-0.4.0/bullmq/timer.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     7481 2023-05-04 10:32:52.000000 bullmq-0.4.0/bullmq/worker.py
-drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-05-18 22:19:58.632254 bullmq-0.4.0/bullmq.egg-info/
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1651 2023-05-18 22:19:58.000000 bullmq-0.4.0/bullmq.egg-info/PKG-INFO
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1352 2023-05-18 22:19:58.000000 bullmq-0.4.0/bullmq.egg-info/SOURCES.txt
--rw-r--r--   0 manuelastudillo   (501) staff       (20)        1 2023-05-18 22:19:58.000000 bullmq-0.4.0/bullmq.egg-info/dependency_links.txt
--rw-r--r--   0 manuelastudillo   (501) staff       (20)       14 2023-05-18 22:19:58.000000 bullmq-0.4.0/bullmq.egg-info/requires.txt
--rw-r--r--   0 manuelastudillo   (501) staff       (20)        7 2023-05-18 22:19:58.000000 bullmq-0.4.0/bullmq.egg-info/top_level.txt
--rw-r--r--   0 manuelastudillo   (501) staff       (20)       38 2023-05-18 22:19:58.660251 bullmq-0.4.0/setup.cfg
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1183 2023-05-18 22:18:20.000000 bullmq-0.4.0/setup.py
+drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-05-29 08:06:36.483868 bullmq-0.4.1/
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1651 2023-05-29 08:06:36.483544 bullmq-0.4.1/PKG-INFO
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      999 2023-05-04 10:32:52.000000 bullmq-0.4.1/README.md
+drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-05-29 08:06:36.449809 bullmq-0.4.1/bullmq/
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      269 2023-05-04 10:32:52.000000 bullmq-0.4.1/bullmq/__init__.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1291 2023-05-04 10:32:52.000000 bullmq-0.4.1/bullmq/backoffs.py
+drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-05-29 08:06:36.477110 bullmq-0.4.1/bullmq/commands/
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     8245 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/addJob-8.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      810 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/changeDelay-3.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     9375 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/cleanJobsInSet-2.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     5979 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/drain-4.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      501 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/extendLock-2.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      809 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/getCounts-1.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1748 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/getRanges-1.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1313 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/getState-7.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      934 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/getStateV2-7.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      897 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/isFinished-3.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      424 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/isJobInList-1.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      543 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/moveJobFromActiveToWait-4.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)    11863 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/moveStalledJobsToWait-8.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     7013 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/moveToActive-9.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     4123 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/moveToDelayed-8.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)    21423 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/moveToFinished-12.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1315 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/moveToWaitingChildren-4.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     7844 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/obliterate-2.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      522 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/pause-4.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1967 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/promote-6.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      292 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/releaseLock-1.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     7980 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/removeJob-1.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      666 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/removeRepeatable-2.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      846 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/reprocessJob-4.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     3150 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/retryJob-8.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1830 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/retryJobs-6.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      282 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/takeLock-1.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      246 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/updateData-1.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      420 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/updateProgress-2.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      200 2023-04-18 08:29:50.000000 bullmq-0.4.1/bullmq/error_code.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      632 2023-04-18 08:29:50.000000 bullmq-0.4.1/bullmq/event_emitter.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     7343 2023-05-29 08:02:35.000000 bullmq-0.4.1/bullmq/job.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     4847 2023-05-29 08:02:35.000000 bullmq-0.4.1/bullmq/queue.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1356 2023-05-29 08:02:35.000000 bullmq-0.4.1/bullmq/redis_connection.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)    15741 2023-05-29 08:02:35.000000 bullmq-0.4.1/bullmq/scripts.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      699 2023-04-18 08:29:50.000000 bullmq-0.4.1/bullmq/timer.py
+drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-05-29 08:06:36.482827 bullmq-0.4.1/bullmq/types/
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      314 2023-05-04 10:32:52.000000 bullmq-0.4.1/bullmq/types/__init__.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      207 2023-05-04 10:32:52.000000 bullmq-0.4.1/bullmq/types/backoff_options.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1920 2023-05-04 10:32:52.000000 bullmq-0.4.1/bullmq/types/job_options.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      395 2023-05-04 10:32:52.000000 bullmq-0.4.1/bullmq/types/keep_jobs.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      189 2023-05-04 10:32:52.000000 bullmq-0.4.1/bullmq/types/queue_options.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      129 2023-05-04 10:32:52.000000 bullmq-0.4.1/bullmq/types/retry_job_options.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1190 2023-05-04 10:32:52.000000 bullmq-0.4.1/bullmq/types/worker_options.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      144 2023-05-29 08:02:35.000000 bullmq-0.4.1/bullmq/utils.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     7490 2023-05-29 08:02:35.000000 bullmq-0.4.1/bullmq/worker.py
+drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-05-29 08:06:36.452051 bullmq-0.4.1/bullmq.egg-info/
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1651 2023-05-29 08:06:36.000000 bullmq-0.4.1/bullmq.egg-info/PKG-INFO
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1574 2023-05-29 08:06:36.000000 bullmq-0.4.1/bullmq.egg-info/SOURCES.txt
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)        1 2023-05-29 08:06:36.000000 bullmq-0.4.1/bullmq.egg-info/dependency_links.txt
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)       14 2023-05-29 08:06:36.000000 bullmq-0.4.1/bullmq.egg-info/requires.txt
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)        7 2023-05-29 08:06:36.000000 bullmq-0.4.1/bullmq.egg-info/top_level.txt
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)       38 2023-05-29 08:06:36.483971 bullmq-0.4.1/setup.cfg
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1194 2023-05-29 08:03:42.000000 bullmq-0.4.1/setup.py
```

### Comparing `bullmq-0.4.0/PKG-INFO` & `bullmq-0.4.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 0.4.0
+Version: 0.4.1
 Summary: BullMQ for Python
 Home-page: https://bullmq.io
 Author: Taskforce.sh Inc.
 Author-email: manast@taskforce.sh
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bullmq-0.4.0/README.md` & `bullmq-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.0/bullmq/backoffs.py` & `bullmq-0.4.1/bullmq/backoffs.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.0/bullmq/commands/addJob-8.lua` & `bullmq-0.4.1/bullmq/commands/addJob-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.0/bullmq/commands/changeDelay-3.lua` & `bullmq-0.4.1/bullmq/commands/changeDelay-3.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.0/bullmq/commands/cleanJobsInSet-2.lua` & `bullmq-0.4.1/bullmq/commands/cleanJobsInSet-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.0/bullmq/commands/drain-4.lua` & `bullmq-0.4.1/bullmq/commands/drain-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.0/bullmq/commands/getCounts-1.lua` & `bullmq-0.4.1/bullmq/commands/getCounts-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.0/bullmq/commands/getRanges-1.lua` & `bullmq-0.4.1/bullmq/commands/getRanges-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.0/bullmq/commands/getState-7.lua` & `bullmq-0.4.1/bullmq/commands/getState-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.0/bullmq/commands/getStateV2-7.lua` & `bullmq-0.4.1/bullmq/commands/getStateV2-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.0/bullmq/commands/isFinished-3.lua` & `bullmq-0.4.1/bullmq/commands/isFinished-3.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.0/bullmq/commands/moveJobFromActiveToWait-4.lua` & `bullmq-0.4.1/bullmq/commands/moveJobFromActiveToWait-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.0/bullmq/commands/moveStalledJobsToWait-8.lua` & `bullmq-0.4.1/bullmq/commands/moveStalledJobsToWait-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.0/bullmq/commands/moveToActive-9.lua` & `bullmq-0.4.1/bullmq/commands/moveToActive-9.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.0/bullmq/commands/moveToDelayed-8.lua` & `bullmq-0.4.1/bullmq/commands/moveToDelayed-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.0/bullmq/commands/moveToFinished-12.lua` & `bullmq-0.4.1/bullmq/commands/moveToFinished-12.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.0/bullmq/commands/moveToWaitingChildren-4.lua` & `bullmq-0.4.1/bullmq/commands/moveToWaitingChildren-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.0/bullmq/commands/obliterate-2.lua` & `bullmq-0.4.1/bullmq/commands/obliterate-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.0/bullmq/commands/pause-4.lua` & `bullmq-0.4.1/bullmq/commands/pause-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.0/bullmq/commands/promote-6.lua` & `bullmq-0.4.1/bullmq/commands/promote-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.0/bullmq/commands/removeJob-1.lua` & `bullmq-0.4.1/bullmq/commands/removeJob-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.0/bullmq/commands/removeRepeatable-2.lua` & `bullmq-0.4.1/bullmq/commands/removeRepeatable-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.0/bullmq/commands/reprocessJob-4.lua` & `bullmq-0.4.1/bullmq/commands/reprocessJob-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.0/bullmq/commands/retryJob-8.lua` & `bullmq-0.4.1/bullmq/commands/retryJob-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.0/bullmq/commands/retryJobs-6.lua` & `bullmq-0.4.1/bullmq/commands/retryJobs-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.0/bullmq/event_emitter.py` & `bullmq-0.4.1/bullmq/event_emitter.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.0/bullmq/job.py` & `bullmq-0.4.1/bullmq/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,27 +45,30 @@
         self.removeOnFail = opts.get("removeOnFail", False)
         self.processedOn = 0
         self.finishedOn = 0
         self.returnvalue = None
         self.failedReason = None
         self.repeatJobKey = None
         self.stacktrace: List[str] = []
-        self.scripts = Scripts(queue.prefix, queue.name, queue.redisConnection.conn)
+        self.scripts = Scripts(queue.prefix, queue.name, queue.redisConnection)
 
     def updateData(self, data):
         self.data = data
         return self.scripts.updateData(self.id, data)
 
     def retry(self, state: str = "failed"):
         self.failedReason = None
         self.finishedOn = None
         self.processedOn = None
         self.returnvalue = None
         return self.scripts.reprocessJob(self, state)
 
+    def getState(self):
+        return self.scripts.getState(self.id)
+
     def updateProgress(self, progress):
         self.progress = progress
         return self.scripts.updateProgress(self.id, progress)
 
     async def moveToFailed(self, err, token:str, fetchNext:bool = False):
         error_message = str(err)
         self.failedReason = error_message
```

### Comparing `bullmq-0.4.0/bullmq/queue.py` & `bullmq-0.4.1/bullmq/queue.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         """
         self.name = name
         self.redisConnection = RedisConnection(redisOpts)
         self.client = self.redisConnection.conn
         self.opts = opts
         self.prefix = opts.get("prefix", "bull")
         self.scripts = Scripts(
-            self.prefix, name, self.redisConnection.conn)
+            self.prefix, name, self.redisConnection)
 
     async def add(self, name: str, data, opts: JobOptions = {}):
         """
         Adds a new job to the queue.
 
         @param name: Name of the job to be added to the queue,.
         @param data: Arbitrary data to append to the job.
```

### Comparing `bullmq-0.4.0/bullmq/scripts.py` & `bullmq-0.4.1/bullmq/scripts.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,55 +2,60 @@
     This class is used to load and execute Lua scripts.
     It is a wrapper around the Redis client.
 """
 
 from __future__ import annotations
 from redis import Redis
 from bullmq.error_code import ErrorCode
+from bullmq.utils import isRedisVersionLowerThan
 from typing import Any, TYPE_CHECKING
 if TYPE_CHECKING:
     from bullmq.job import Job
+    from bullmq.redis_connection import RedisConnection
 
 import time
 import json
 import msgpack
 import os
 
 
 basePath = os.path.dirname(os.path.realpath(__file__))
 
 
 class Scripts:
 
-    def __init__(self, prefix: str, queueName: str, redisClient: Redis):
+    def __init__(self, prefix: str, queueName: str, redisConnection: RedisConnection):
         self.prefix = prefix
         self.queueName = queueName
         self.keys = {}
-        self.redisClient = redisClient
+        self.redisConnection = redisConnection
+        self.redisClient = redisConnection.conn
         self.commands = {
-            "addJob": redisClient.register_script(self.getScript("addJob-8.lua")),
-            "extendLock": redisClient.register_script(self.getScript("extendLock-2.lua")),
-            "getCounts": redisClient.register_script(self.getScript("getCounts-1.lua")),
-            "moveToActive": redisClient.register_script(self.getScript("moveToActive-9.lua")),
-            "moveToDelayed": redisClient.register_script(self.getScript("moveToDelayed-8.lua")),
-            "moveToFinished": redisClient.register_script(self.getScript("moveToFinished-12.lua")),
-            "moveStalledJobsToWait": redisClient.register_script(self.getScript("moveStalledJobsToWait-8.lua")),
-            "pause": redisClient.register_script(self.getScript("pause-4.lua")),
-            "obliterate": redisClient.register_script(self.getScript("obliterate-2.lua")),
-            "reprocessJob": redisClient.register_script(self.getScript("reprocessJob-6.lua")),
-            "retryJob": redisClient.register_script(self.getScript("retryJob-8.lua")),
-            "retryJobs": redisClient.register_script(self.getScript("retryJobs-6.lua")),
-            "saveStacktrace": redisClient.register_script(self.getScript("saveStacktrace-1.lua")),
-            "updateData": redisClient.register_script(self.getScript("updateData-1.lua")),
-            "updateProgress": redisClient.register_script(self.getScript("updateProgress-2.lua")),
+            "addJob": self.redisClient.register_script(self.getScript("addJob-8.lua")),
+            "extendLock": self.redisClient.register_script(self.getScript("extendLock-2.lua")),
+            "getCounts": self.redisClient.register_script(self.getScript("getCounts-1.lua")),
+            "getState": self.redisClient.register_script(self.getScript("getState-7.lua")),
+            "getStateV2": self.redisClient.register_script(self.getScript("getStateV2-7.lua")),
+            "moveToActive": self.redisClient.register_script(self.getScript("moveToActive-9.lua")),
+            "moveToDelayed": self.redisClient.register_script(self.getScript("moveToDelayed-8.lua")),
+            "moveToFinished": self.redisClient.register_script(self.getScript("moveToFinished-12.lua")),
+            "moveStalledJobsToWait": self.redisClient.register_script(self.getScript("moveStalledJobsToWait-8.lua")),
+            "pause": self.redisClient.register_script(self.getScript("pause-4.lua")),
+            "obliterate": self.redisClient.register_script(self.getScript("obliterate-2.lua")),
+            "reprocessJob": self.redisClient.register_script(self.getScript("reprocessJob-6.lua")),
+            "retryJob": self.redisClient.register_script(self.getScript("retryJob-8.lua")),
+            "retryJobs": self.redisClient.register_script(self.getScript("retryJobs-6.lua")),
+            "saveStacktrace": self.redisClient.register_script(self.getScript("saveStacktrace-1.lua")),
+            "updateData": self.redisClient.register_script(self.getScript("updateData-1.lua")),
+            "updateProgress": self.redisClient.register_script(self.getScript("updateProgress-2.lua")),
         }
 
         # loop all the names and add them to the keys object
         names = ["", "active", "wait", "paused", "completed", "failed", "delayed",
-                 "stalled", "limiter", "priority", "id", "stalled-check", "meta", "events"]
+                 "stalled", "limiter", "priority", "id", "stalled-check", "meta", "events", "waiting-children"]
         for name in names:
             self.keys[name] = self.toKey(name)
 
     def toKey(self, name: str):
         return f"{self.prefix}:{self.queueName}:{name}"
 
     def getScript(self, name: str):
@@ -144,14 +149,29 @@
     def getCounts(self, types):
         keys = self.getKeys([''])
         transformed_types = list(
             map(lambda type: 'wait' if type == 'waiting' else type, types))
 
         return self.commands["getCounts"](keys=keys, args=transformed_types)
 
+    async def getState(self, job_id):
+        keys = self.getKeys(['completed', 'failed', 'delayed', 'active', 'wait',
+                'paused', 'waiting-children'])
+
+        args = [job_id]
+
+        redis_version = await self.redisConnection.getRedisVersion()
+
+        if isRedisVersionLowerThan(redis_version, '6.0.6'):
+            result = await self.commands["getState"](keys=keys, args=args)
+            return result
+
+        result = await self.commands["getStateV2"](keys=keys, args=args)
+        return result
+
     async def updateData(self, job_id: str, data):
         keys = [self.toKey(job_id)]
         data_json = json.dumps(data, separators=(',', ':'))
         args = [data_json]
 
         result = await self.commands["updateData"](keys=keys, args=args)
```

### Comparing `bullmq-0.4.0/bullmq/timer.py` & `bullmq-0.4.1/bullmq/timer.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.0/bullmq/worker.py` & `bullmq-0.4.1/bullmq/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         self.opts = final_opts
         redis_opts = opts.get("connection", {})
         self.redisConnection = RedisConnection(redis_opts)
         self.blockingRedisConnection = RedisConnection(redis_opts)
         self.client = self.redisConnection.conn
         self.bclient = self.blockingRedisConnection.conn
         self.prefix = opts.get("prefix", "bull")
-        self.scripts = Scripts(opts.get("prefix", "bull"), name, self.client)
+        self.scripts = Scripts(opts.get("prefix", "bull"), name, self.redisConnection)
         self.closing = False
         self.forceClosing = False
         self.closed = False
         self.running = False
         self.processing = set()
         self.jobs = set()
```

### Comparing `bullmq-0.4.0/bullmq.egg-info/PKG-INFO` & `bullmq-0.4.1/bullmq.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 0.4.0
+Version: 0.4.1
 Summary: BullMQ for Python
 Home-page: https://bullmq.io
 Author: Taskforce.sh Inc.
 Author-email: manast@taskforce.sh
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bullmq-0.4.0/setup.py` & `bullmq-0.4.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 
 # Get the long description from the README file
 with open(path.join(".", 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='bullmq',
-    version='0.4.0',    
+    version='0.4.1',    
     description='BullMQ for Python',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://bullmq.io',
     author='Taskforce.sh Inc.',
     author_email='manast@taskforce.sh',
     license='MIT',
     packages=['bullmq'],
-    package_data={'bullmq': ['commands/*.lua']},
+    package_data={'bullmq': ['commands/*.lua', 'types/*']},
     install_requires=['redis',
                       'msgpack',            
                       ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
```

