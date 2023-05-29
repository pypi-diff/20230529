# Comparing `tmp/tap-stripe-2.0.4.tar.gz` & `tmp/tap-stripe-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap-stripe-2.0.4.tar", last modified: Fri Feb 24 15:49:17 2023, max compression
+gzip compressed data, was "tap-stripe-2.0.5.tar", last modified: Mon May 29 14:32:34 2023, max compression
```

## Comparing `tap-stripe-2.0.4.tar` & `tap-stripe-2.0.5.tar`

### file list

```diff
@@ -1,40 +1,54 @@
-drwxrwxr-x   0 dsprayberry  (1001) dsprayberry  (1001)        0 2023-02-24 15:49:17.794812 tap-stripe-2.0.4/
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)    32387 2023-02-23 18:18:11.000000 tap-stripe-2.0.4/LICENSE
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)       91 2023-02-23 18:18:11.000000 tap-stripe-2.0.4/MANIFEST.in
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      259 2023-02-24 15:49:17.794812 tap-stripe-2.0.4/PKG-INFO
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     2187 2023-02-23 18:18:11.000000 tap-stripe-2.0.4/README.md
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)       79 2023-02-24 15:49:17.794812 tap-stripe-2.0.4/setup.cfg
--rwxrwxr-x   0 dsprayberry  (1001) dsprayberry  (1001)      879 2023-02-24 15:48:29.000000 tap-stripe-2.0.4/setup.py
-drwxrwxr-x   0 dsprayberry  (1001) dsprayberry  (1001)        0 2023-02-24 15:49:17.790812 tap-stripe-2.0.4/tap_stripe/
--rwxrwxr-x   0 dsprayberry  (1001) dsprayberry  (1001)    54478 2023-02-23 18:52:42.000000 tap-stripe-2.0.4/tap_stripe/__init__.py
-drwxrwxr-x   0 dsprayberry  (1001) dsprayberry  (1001)        0 2023-02-24 15:49:17.794812 tap-stripe-2.0.4/tap_stripe/schemas/
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     2168 2023-02-23 18:18:11.000000 tap-stripe-2.0.4/tap_stripe/schemas/balance_transactions.json
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)       33 2023-02-23 18:18:11.000000 tap-stripe-2.0.4/tap_stripe/schemas/charges.json
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     1696 2023-02-23 18:18:11.000000 tap-stripe-2.0.4/tap_stripe/schemas/coupons.json
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     8637 2023-02-23 18:18:11.000000 tap-stripe-2.0.4/tap_stripe/schemas/customers.json
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     4215 2023-02-23 18:18:11.000000 tap-stripe-2.0.4/tap_stripe/schemas/disputes.json
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      941 2023-02-23 18:18:11.000000 tap-stripe-2.0.4/tap_stripe/schemas/events.json
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     4088 2023-02-23 18:18:11.000000 tap-stripe-2.0.4/tap_stripe/schemas/invoice_items.json
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     9102 2023-02-23 18:18:11.000000 tap-stripe-2.0.4/tap_stripe/schemas/invoice_line_items.json
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)    16200 2023-02-23 18:18:11.000000 tap-stripe-2.0.4/tap_stripe/schemas/invoices.json
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)    31986 2023-02-24 15:48:29.000000 tap-stripe-2.0.4/tap_stripe/schemas/payment_intents.json
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      226 2023-02-23 18:18:11.000000 tap-stripe-2.0.4/tap_stripe/schemas/payout_transactions.json
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     4310 2023-02-23 18:18:11.000000 tap-stripe-2.0.4/tap_stripe/schemas/payouts.json
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)       31 2023-02-23 18:18:11.000000 tap-stripe-2.0.4/tap_stripe/schemas/plans.json
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     2613 2023-02-23 18:18:11.000000 tap-stripe-2.0.4/tap_stripe/schemas/products.json
-drwxrwxr-x   0 dsprayberry  (1001) dsprayberry  (1001)        0 2023-02-24 15:49:17.794812 tap-stripe-2.0.4/tap_stripe/schemas/shared/
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)    40067 2023-02-23 18:18:11.000000 tap-stripe-2.0.4/tap_stripe/schemas/shared/charge.json
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     2880 2023-02-23 18:18:11.000000 tap-stripe-2.0.4/tap_stripe/schemas/shared/discount.json
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     2817 2023-02-23 18:18:11.000000 tap-stripe-2.0.4/tap_stripe/schemas/shared/plan.json
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     9410 2023-02-23 18:18:11.000000 tap-stripe-2.0.4/tap_stripe/schemas/shared/source.json
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     1680 2023-02-23 18:18:11.000000 tap-stripe-2.0.4/tap_stripe/schemas/shared/tax_ids.json
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     8262 2023-02-23 18:18:11.000000 tap-stripe-2.0.4/tap_stripe/schemas/subscription_items.json
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     8358 2023-02-23 18:18:11.000000 tap-stripe-2.0.4/tap_stripe/schemas/subscriptions.json
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     2469 2023-02-23 18:18:11.000000 tap-stripe-2.0.4/tap_stripe/schemas/transfers.json
-drwxrwxr-x   0 dsprayberry  (1001) dsprayberry  (1001)        0 2023-02-24 15:49:17.790812 tap-stripe-2.0.4/tap_stripe.egg-info/
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      259 2023-02-24 15:49:17.000000 tap-stripe-2.0.4/tap_stripe.egg-info/PKG-INFO
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     1083 2023-02-24 15:49:17.000000 tap-stripe-2.0.4/tap_stripe.egg-info/SOURCES.txt
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)        1 2023-02-24 15:49:17.000000 tap-stripe-2.0.4/tap_stripe.egg-info/dependency_links.txt
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)       47 2023-02-24 15:49:17.000000 tap-stripe-2.0.4/tap_stripe.egg-info/entry_points.txt
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      132 2023-02-24 15:49:17.000000 tap-stripe-2.0.4/tap_stripe.egg-info/requires.txt
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)       11 2023-02-24 15:49:17.000000 tap-stripe-2.0.4/tap_stripe.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-29 14:32:34.214258 tap-stripe-2.0.5/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32387 2023-04-18 13:12:15.000000 tap-stripe-2.0.5/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       91 2023-04-18 13:12:15.000000 tap-stripe-2.0.5/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      293 2023-05-29 14:32:34.214258 tap-stripe-2.0.5/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2187 2023-04-18 13:12:15.000000 tap-stripe-2.0.5/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-05-29 14:32:34.214258 tap-stripe-2.0.5/setup.cfg
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      879 2023-05-29 14:18:12.000000 tap-stripe-2.0.5/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-29 14:32:34.206258 tap-stripe-2.0.5/tap_stripe/
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    55854 2023-05-29 12:00:36.000000 tap-stripe-2.0.5/tap_stripe/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-29 14:32:34.210258 tap-stripe-2.0.5/tap_stripe/schemas/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2168 2023-04-18 13:12:15.000000 tap-stripe-2.0.5/tap_stripe/schemas/balance_transactions.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       33 2023-04-18 13:12:15.000000 tap-stripe-2.0.5/tap_stripe/schemas/charges.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1696 2023-04-18 13:12:15.000000 tap-stripe-2.0.5/tap_stripe/schemas/coupons.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8637 2023-04-18 13:12:15.000000 tap-stripe-2.0.5/tap_stripe/schemas/customers.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4215 2023-04-18 13:12:15.000000 tap-stripe-2.0.5/tap_stripe/schemas/disputes.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      941 2023-04-18 13:12:15.000000 tap-stripe-2.0.5/tap_stripe/schemas/events.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4088 2023-04-18 13:12:15.000000 tap-stripe-2.0.5/tap_stripe/schemas/invoice_items.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9102 2023-04-18 13:12:15.000000 tap-stripe-2.0.5/tap_stripe/schemas/invoice_line_items.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16200 2023-04-18 13:12:15.000000 tap-stripe-2.0.5/tap_stripe/schemas/invoices.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    31986 2023-04-18 13:12:15.000000 tap-stripe-2.0.5/tap_stripe/schemas/payment_intents.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      226 2023-04-18 13:12:15.000000 tap-stripe-2.0.5/tap_stripe/schemas/payout_transactions.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4310 2023-04-18 13:12:15.000000 tap-stripe-2.0.5/tap_stripe/schemas/payouts.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       31 2023-04-18 13:12:15.000000 tap-stripe-2.0.5/tap_stripe/schemas/plans.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2613 2023-04-18 13:12:15.000000 tap-stripe-2.0.5/tap_stripe/schemas/products.json
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-29 14:32:34.214258 tap-stripe-2.0.5/tap_stripe/schemas/shared/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    40067 2023-04-18 13:12:15.000000 tap-stripe-2.0.5/tap_stripe/schemas/shared/charge.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2880 2023-04-18 13:12:15.000000 tap-stripe-2.0.5/tap_stripe/schemas/shared/discount.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2817 2023-04-18 13:12:15.000000 tap-stripe-2.0.5/tap_stripe/schemas/shared/plan.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9410 2023-04-18 13:12:15.000000 tap-stripe-2.0.5/tap_stripe/schemas/shared/source.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1680 2023-04-18 13:12:15.000000 tap-stripe-2.0.5/tap_stripe/schemas/shared/tax_ids.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8262 2023-04-18 13:12:15.000000 tap-stripe-2.0.5/tap_stripe/schemas/subscription_items.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8358 2023-04-18 13:12:15.000000 tap-stripe-2.0.5/tap_stripe/schemas/subscriptions.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2469 2023-04-18 13:12:15.000000 tap-stripe-2.0.5/tap_stripe/schemas/transfers.json
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-29 14:32:34.210258 tap-stripe-2.0.5/tap_stripe.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      293 2023-05-29 14:32:34.000000 tap-stripe-2.0.5/tap_stripe.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1478 2023-05-29 14:32:34.000000 tap-stripe-2.0.5/tap_stripe.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-29 14:32:34.000000 tap-stripe-2.0.5/tap_stripe.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       58 2023-05-29 14:32:34.000000 tap-stripe-2.0.5/tap_stripe.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      132 2023-05-29 14:32:34.000000 tap-stripe-2.0.5/tap_stripe.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2023-05-29 14:32:34.000000 tap-stripe-2.0.5/tap_stripe.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-29 14:32:34.214258 tap-stripe-2.0.5/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24637 2023-04-18 13:12:15.000000 tap-stripe-2.0.5/tests/test_all_fields.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1997 2023-04-18 13:12:15.000000 tap-stripe-2.0.5/tests/test_all_tests_run.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3357 2023-04-18 13:12:15.000000 tap-stripe-2.0.5/tests/test_automatic_fields.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4874 2023-04-18 13:12:15.000000 tap-stripe-2.0.5/tests/test_automatic_payout_transactions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19925 2023-04-18 13:12:15.000000 tap-stripe-2.0.5/tests/test_bookmarks.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2782 2023-04-18 13:12:15.000000 tap-stripe-2.0.5/tests/test_configurable_lookback_window.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6584 2023-04-18 13:12:15.000000 tap-stripe-2.0.5/tests/test_create_object.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8989 2023-04-18 13:12:15.000000 tap-stripe-2.0.5/tests/test_discovery.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11643 2023-04-18 13:12:15.000000 tap-stripe-2.0.5/tests/test_event_updates.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4207 2023-04-18 13:12:15.000000 tap-stripe-2.0.5/tests/test_full_replication.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8777 2023-04-18 13:12:15.000000 tap-stripe-2.0.5/tests/test_pagination.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2110 2023-04-18 13:12:15.000000 tap-stripe-2.0.5/tests/test_parent_child_independent.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8838 2023-04-18 13:12:15.000000 tap-stripe-2.0.5/tests/test_start_date.py
```

### Comparing `tap-stripe-2.0.4/LICENSE` & `tap-stripe-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tap-stripe-2.0.4/README.md` & `tap-stripe-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `tap-stripe-2.0.4/setup.py` & `tap-stripe-2.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name="tap-stripe",
-    version="2.0.4",
+    version="2.0.5",
     description="Singer.io tap for extracting data",
     author="Stitch",
     url="http://singer.io",
     classifiers=["Programming Language :: Python :: 3 :: Only"],
     py_modules=["tap_stripe"],
     install_requires=[
         "singer-python==5.5.1",
```

### Comparing `tap-stripe-2.0.4/tap_stripe/__init__.py` & `tap-stripe-2.0.5/tap_stripe/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -948,54 +948,59 @@
     look at 'events update' bookmark and pull events after that
     :param
     stream_name - Name of the stream
     is_sub_stream - Check whether the function is called via the parent stream(only parent/both are selected)
                     or when called through only child stream i.e. when parent is not selected.
     '''
     LOGGER.info("Started syncing event based updates")
+    reset_brk_flag_value = False
     event_update_window_size = Context.event_update_window_size
     events_update_date_window_size = int(60 * 60 * 24 * event_update_window_size) # event_update_window_size in seconds
     sync_start_time = dt_to_epoch(utils.now())
+    start_date = int(utils.strptime_to_utc(Context.config["start_date"]).timestamp())
 
     if is_sub_stream:
         # We need to get the parent data first for syncing the child streams. Hence,
         # changing stream_name to parent stream when only child is selected.
         stream_name = PARENT_STREAM_MAP.get(stream_name)
 
     sub_stream_name = SUB_STREAMS.get(stream_name)
 
     parent_bookmark_value = singer.get_bookmark(Context.state,
                                                 stream_name + '_events',
-                                                'updates_created') or \
-        int(utils.strptime_to_utc(Context.config["start_date"]).timestamp())
+                                                'updates_created') or start_date
 
     # Get the bookmark value of the sub_stream if its selected and present
     if sub_stream_name:
         sub_stream_bookmark_value = singer.get_bookmark(Context.state,
                                                         sub_stream_name + '_events',
-                                                        'updates_created') or \
-            int(utils.strptime_to_utc(Context.config["start_date"]).timestamp())
-
+                                                        'updates_created') or start_date
     # If only child stream is selected, update bookmark to sub-stream bookmark value
     if is_sub_stream:
         bookmark_value = sub_stream_bookmark_value
 
     elif sub_stream_name and Context.is_selected(sub_stream_name):
         # Get the minimum bookmark value from parent and child streams if both are selected.
         bookmark_value = min(parent_bookmark_value, sub_stream_bookmark_value)
 
+        if parent_bookmark_value != sub_stream_bookmark_value and bookmark_value == start_date:
+            reset_brk_flag_value = True
+
     # Update the bookmark to parent bookmark value, if child is not selected
     else:
         bookmark_value = parent_bookmark_value
 
     # Start sync for event updates record from the last 30 days before if bookmark/start_date is older than 30 days.
-    max_created = int(max(bookmark_value, (epoch_to_dt(sync_start_time) - timedelta(days=30)).timestamp()))
-    if max_created != bookmark_value:
-        LOGGER.warning("Provided start_date or current bookmark for event updates is older than 30 days.")
-        LOGGER.warning("The Stripe Event API returns data for the last 30 days only. So, syncing event data from 30 days only.")
+    max_event_start_date = (epoch_to_dt(sync_start_time) - timedelta(days=30)).timestamp()
+    max_created = int(max(bookmark_value, max_event_start_date))
+
+    if max_created != bookmark_value and (bookmark_value != start_date or reset_brk_flag_value is True):
+        reset_bookmark_for_event_updates(is_sub_stream, stream_name, sub_stream_name, start_date)
+        raise Exception("Provided current bookmark date for event updates is older than 30 days."\
+            " Hence, resetting the bookmark date of respective {}/{} stream to start date.".format(stream_name, sub_stream_name))
 
     date_window_start = max_created
     date_window_end = max_created + events_update_date_window_size
     stop_paging = False
 
     # Create a map to hold relate event object ids to timestamps
     updated_object_timestamps = {}
@@ -1110,14 +1115,36 @@
         singer.write_bookmark(Context.state,
                               sub_stream_name + '_events',
                               'updates_created',
                               max_created)
 
     singer.write_state(Context.state)
 
+def reset_bookmark_for_event_updates(is_sub_stream, stream_name, sub_stream_name, start_date):
+    """
+    Reset bookmark for parent and child streams to start date and clear the bookmark date for event updates.
+    """
+    # Write the parent bookmark value only when the parent is selected
+    if not is_sub_stream:
+        singer.write_bookmark(Context.state,
+                              stream_name,
+                              STREAM_REPLICATION_KEY.get(stream_name),
+                              start_date)
+        Context.state.get("bookmarks").pop(stream_name + '_events', None)
+
+    # Write the child bookmark value only when the child is selected
+    if sub_stream_name and Context.is_selected(sub_stream_name):
+        singer.write_bookmark(Context.state,
+                              sub_stream_name,
+                              STREAM_REPLICATION_KEY.get(sub_stream_name),
+                              start_date)
+        Context.state.get("bookmarks").pop(sub_stream_name + '_events', None)
+
+    singer.write_state(Context.state)
+
 
 def sync():
     """
     The sync function called for the sync mode.
     """
     # Write all schemas and init count to 0
     for catalog_entry in Context.catalog['streams']:
```

### Comparing `tap-stripe-2.0.4/tap_stripe/schemas/balance_transactions.json` & `tap-stripe-2.0.5/tap_stripe/schemas/balance_transactions.json`

 * *Files identical despite different names*

### Comparing `tap-stripe-2.0.4/tap_stripe/schemas/coupons.json` & `tap-stripe-2.0.5/tap_stripe/schemas/coupons.json`

 * *Files identical despite different names*

### Comparing `tap-stripe-2.0.4/tap_stripe/schemas/customers.json` & `tap-stripe-2.0.5/tap_stripe/schemas/customers.json`

 * *Files identical despite different names*

### Comparing `tap-stripe-2.0.4/tap_stripe/schemas/disputes.json` & `tap-stripe-2.0.5/tap_stripe/schemas/disputes.json`

 * *Files identical despite different names*

### Comparing `tap-stripe-2.0.4/tap_stripe/schemas/events.json` & `tap-stripe-2.0.5/tap_stripe/schemas/events.json`

 * *Files identical despite different names*

### Comparing `tap-stripe-2.0.4/tap_stripe/schemas/invoice_items.json` & `tap-stripe-2.0.5/tap_stripe/schemas/invoice_items.json`

 * *Files identical despite different names*

### Comparing `tap-stripe-2.0.4/tap_stripe/schemas/invoice_line_items.json` & `tap-stripe-2.0.5/tap_stripe/schemas/invoice_line_items.json`

 * *Files identical despite different names*

### Comparing `tap-stripe-2.0.4/tap_stripe/schemas/invoices.json` & `tap-stripe-2.0.5/tap_stripe/schemas/invoices.json`

 * *Files identical despite different names*

### Comparing `tap-stripe-2.0.4/tap_stripe/schemas/payment_intents.json` & `tap-stripe-2.0.5/tap_stripe/schemas/payment_intents.json`

 * *Files identical despite different names*

### Comparing `tap-stripe-2.0.4/tap_stripe/schemas/payouts.json` & `tap-stripe-2.0.5/tap_stripe/schemas/payouts.json`

 * *Files identical despite different names*

### Comparing `tap-stripe-2.0.4/tap_stripe/schemas/products.json` & `tap-stripe-2.0.5/tap_stripe/schemas/products.json`

 * *Files identical despite different names*

### Comparing `tap-stripe-2.0.4/tap_stripe/schemas/shared/charge.json` & `tap-stripe-2.0.5/tap_stripe/schemas/shared/charge.json`

 * *Files identical despite different names*

### Comparing `tap-stripe-2.0.4/tap_stripe/schemas/shared/discount.json` & `tap-stripe-2.0.5/tap_stripe/schemas/shared/discount.json`

 * *Files identical despite different names*

### Comparing `tap-stripe-2.0.4/tap_stripe/schemas/shared/plan.json` & `tap-stripe-2.0.5/tap_stripe/schemas/shared/plan.json`

 * *Files identical despite different names*

### Comparing `tap-stripe-2.0.4/tap_stripe/schemas/shared/source.json` & `tap-stripe-2.0.5/tap_stripe/schemas/shared/source.json`

 * *Files identical despite different names*

### Comparing `tap-stripe-2.0.4/tap_stripe/schemas/shared/tax_ids.json` & `tap-stripe-2.0.5/tap_stripe/schemas/shared/tax_ids.json`

 * *Files identical despite different names*

### Comparing `tap-stripe-2.0.4/tap_stripe/schemas/subscription_items.json` & `tap-stripe-2.0.5/tap_stripe/schemas/subscription_items.json`

 * *Files identical despite different names*

### Comparing `tap-stripe-2.0.4/tap_stripe/schemas/subscriptions.json` & `tap-stripe-2.0.5/tap_stripe/schemas/subscriptions.json`

 * *Files identical despite different names*

### Comparing `tap-stripe-2.0.4/tap_stripe/schemas/transfers.json` & `tap-stripe-2.0.5/tap_stripe/schemas/transfers.json`

 * *Files identical despite different names*

