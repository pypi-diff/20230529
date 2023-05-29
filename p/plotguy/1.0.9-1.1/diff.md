# Comparing `tmp/plotguy-1.0.9.tar.gz` & `tmp/plotguy-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plotguy-1.0.9.tar", last modified: Mon May 22 09:17:30 2023, max compression
+gzip compressed data, was "plotguy-1.1.tar", last modified: Mon May 29 00:13:52 2023, max compression
```

## Comparing `plotguy-1.0.9.tar` & `plotguy-1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-05-22 09:17:30.312348 plotguy-1.0.9/
--rw-r--r--   0 cmw        (501) staff       (20)      353 2023-05-22 09:17:30.312129 plotguy-1.0.9/PKG-INFO
--rw-r--r--   0 cmw        (501) staff       (20)        9 2022-09-09 02:08:10.000000 plotguy-1.0.9/README.md
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-05-22 09:17:30.310790 plotguy-1.0.9/plotguy/
--rw-r--r--   0 cmw        (501) staff       (20)    24547 2023-05-21 22:31:41.000000 plotguy-1.0.9/plotguy/__init__.py
--rw-r--r--   0 cmw        (501) staff       (20)    16884 2023-05-22 09:16:53.000000 plotguy-1.0.9/plotguy/aggregate.py
--rw-r--r--   0 cmw        (501) staff       (20)    64059 2023-05-22 04:48:36.000000 plotguy-1.0.9/plotguy/components.py
--rw-r--r--   0 cmw        (501) staff       (20)    37762 2023-05-22 04:38:48.000000 plotguy-1.0.9/plotguy/equity_curves.py
--rw-r--r--   0 cmw        (501) staff       (20)    11123 2023-04-18 03:30:27.000000 plotguy-1.0.9/plotguy/signals.py
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-05-22 09:17:30.311839 plotguy-1.0.9/plotguy.egg-info/
--rw-r--r--   0 cmw        (501) staff       (20)      353 2023-05-22 09:17:30.000000 plotguy-1.0.9/plotguy.egg-info/PKG-INFO
--rw-r--r--   0 cmw        (501) staff       (20)      279 2023-05-22 09:17:30.000000 plotguy-1.0.9/plotguy.egg-info/SOURCES.txt
--rw-r--r--   0 cmw        (501) staff       (20)        1 2023-05-22 09:17:30.000000 plotguy-1.0.9/plotguy.egg-info/dependency_links.txt
--rw-r--r--   0 cmw        (501) staff       (20)      131 2023-05-22 09:17:30.000000 plotguy-1.0.9/plotguy.egg-info/requires.txt
--rw-r--r--   0 cmw        (501) staff       (20)        8 2023-05-22 09:17:30.000000 plotguy-1.0.9/plotguy.egg-info/top_level.txt
--rw-r--r--   0 cmw        (501) staff       (20)       38 2023-05-22 09:17:30.312417 plotguy-1.0.9/setup.cfg
--rw-r--r--   0 cmw        (501) staff       (20)      832 2023-05-22 09:17:19.000000 plotguy-1.0.9/setup.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-05-29 00:13:52.058445 plotguy-1.1/
+-rw-r--r--   0 cmw        (501) staff       (20)      351 2023-05-29 00:13:52.058188 plotguy-1.1/PKG-INFO
+-rw-r--r--   0 cmw        (501) staff       (20)        9 2022-09-09 02:08:10.000000 plotguy-1.1/README.md
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-05-29 00:13:52.057246 plotguy-1.1/plotguy/
+-rw-r--r--   0 cmw        (501) staff       (20)    25102 2023-05-29 00:11:51.000000 plotguy-1.1/plotguy/__init__.py
+-rw-r--r--   0 cmw        (501) staff       (20)    16884 2023-05-22 09:16:53.000000 plotguy-1.1/plotguy/aggregate.py
+-rw-r--r--   0 cmw        (501) staff       (20)    64059 2023-05-22 04:48:36.000000 plotguy-1.1/plotguy/components.py
+-rw-r--r--   0 cmw        (501) staff       (20)    37762 2023-05-22 04:38:48.000000 plotguy-1.1/plotguy/equity_curves.py
+-rw-r--r--   0 cmw        (501) staff       (20)    11123 2023-04-18 03:30:27.000000 plotguy-1.1/plotguy/signals.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-05-29 00:13:52.057999 plotguy-1.1/plotguy.egg-info/
+-rw-r--r--   0 cmw        (501) staff       (20)      351 2023-05-29 00:13:51.000000 plotguy-1.1/plotguy.egg-info/PKG-INFO
+-rw-r--r--   0 cmw        (501) staff       (20)      279 2023-05-29 00:13:51.000000 plotguy-1.1/plotguy.egg-info/SOURCES.txt
+-rw-r--r--   0 cmw        (501) staff       (20)        1 2023-05-29 00:13:51.000000 plotguy-1.1/plotguy.egg-info/dependency_links.txt
+-rw-r--r--   0 cmw        (501) staff       (20)      131 2023-05-29 00:13:51.000000 plotguy-1.1/plotguy.egg-info/requires.txt
+-rw-r--r--   0 cmw        (501) staff       (20)        8 2023-05-29 00:13:51.000000 plotguy-1.1/plotguy.egg-info/top_level.txt
+-rw-r--r--   0 cmw        (501) staff       (20)       38 2023-05-29 00:13:52.058492 plotguy-1.1/setup.cfg
+-rw-r--r--   0 cmw        (501) staff       (20)      830 2023-05-29 00:13:02.000000 plotguy-1.1/setup.py
```

### Comparing `plotguy-1.0.9/plotguy/__init__.py` & `plotguy-1.1/plotguy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,64 +70,73 @@
     # Purpose if this is to calculate unrealized pnl between open date and close date, aggreagte same day pnl with other trade,
     # also save realized pnl
 
     df_daily = apply_pnl.df_daily
 
     open_date = row.open_date
     close_date = row.date
-    now_close = df_daily.at[open_date, 'close']
+    now_close = float(df_daily.at[open_date, 'close'])
     dates = pd.date_range(start=open_date, end=close_date)
-    open_price = row.open_price
-    num_of_share = row.num_of_share
-    commission = row.commission
+    open_price = float(row.open_price)
+    num_of_share = int(row.num_of_share)
+    commission = float(row.commission)
     action = row.action
-    realized_pnl = row.realized_pnl
+    realized_pnl = float(row.realized_pnl)
 
     last_realized_capital = apply_pnl.last_realized_capital
-    multiplier = apply_pnl.multiplier
+    multiplier = float(apply_pnl.multiplier)
+
 
     for date in dates:
-        if date == open_date:
-            # Unrealized pnl on the open date, record on df_daily
-            df_daily.at[open_date, 'action'] = 'open'
-            unrealized_pnl = num_of_share * multiplier * (now_close - open_price) - commission
-            unrealized_pnl = round(unrealized_pnl, 3)
-            df_daily.at[open_date, 'unrealized_pnl'] = unrealized_pnl
-
-            # print(open_date, 'Open!', open_price, now_close, num_of_share, unrealized_pnl)
-
-        elif date == close_date:  # close position on this date, end of this trade
-            # this is a same day trade
-            # clear the open unrealized pnl as open and close same day should not aggregate
-            # it should be record as realized pnl directly
-            if open_date == close_date:
-                df_daily.at[date, 'unrealized_pnl'] = None
-
-            # unrealized_pnl
-            if df_daily.at[date, 'unrealized_pnl']:  # if there is already unrealized_pnl, aggregate
-                df_daily.at[date, 'unrealized_pnl'] = df_daily.at[date, 'unrealized_pnl'] + realized_pnl
-            else:
-                df_daily.at[date, 'unrealized_pnl'] = realized_pnl
+        if (date == open_date or date == close_date):
+            # open_date and close_date may be the first
+            # therefore, process open_date first, then close_date
+
+            if date == open_date:
+                # Unrealized pnl on the open date, record on df_daily
+                df_daily.at[open_date, 'action'] = 'open'
 
-            # realized pnl
-            if df_daily.at[date, 'realized_pnl']:  # if there is already realized_pnl, aggregate
-                df_daily.at[date, 'realized_pnl'] = df_daily.at[date, 'realized_pnl'] + realized_pnl
-            else:
-                df_daily.at[date, 'realized_pnl'] = realized_pnl
+                unrealized_pnl = num_of_share * multiplier * (now_close - open_price)#  - commission
+                unrealized_pnl = round(unrealized_pnl, 3)
+                df_daily.at[open_date, 'unrealized_pnl'] = unrealized_pnl
+
+                # print(open_date, 'Open!', open_price, now_close, num_of_share, unrealized_pnl)
+
+            if date == close_date:  # close position on this date, end of this trade
+                # this is a same day trade
+                # clear the open unrealized pnl as open and close same day should not aggregate
+                # it should be record as realized pnl directly
+                if open_date == close_date:
+                    df_daily.at[date, 'unrealized_pnl'] = None
+
+                # unrealized_pnl
+                if df_daily.at[date, 'unrealized_pnl']:  # if there is already unrealized_pnl, aggregate
+                    df_daily.at[date, 'unrealized_pnl'] = df_daily.at[date, 'unrealized_pnl'] + realized_pnl
+                else:
+                    df_daily.at[date, 'unrealized_pnl'] = realized_pnl
+
+                # realized pnl
+                if df_daily.at[date, 'realized_pnl']:  # if there is already realized_pnl, aggregate
+                    df_daily.at[date, 'realized_pnl'] = df_daily.at[date, 'realized_pnl'] + realized_pnl
+                else:
+                    df_daily.at[date, 'realized_pnl'] = realized_pnl
 
-            df_daily.at[date, 'action'] = action
-            df_daily.at[date, 'commission'] = commission
-            last_realized_capital = last_realized_capital + realized_pnl
+                df_daily.at[date, 'action'] = action
+                df_daily.at[date, 'commission'] = commission
+                last_realized_capital = last_realized_capital + realized_pnl
 
-            # print(date, 'Close!', open_price, close_date, realized_pnl)
-            # print()
+                # print(date, 'Close!', open_price, close_date, realized_pnl)
+                # print()
 
         else:
+            # it is not (date == open_date or date == close_date), so it is between two date
+            # calculate unrealized pnl only
             try:
                 now_close = df_daily.at[date, 'close']
+
                 unrealized_pnl = num_of_share * multiplier * (now_close - open_price) - commission
                 unrealized_pnl = round(unrealized_pnl, 3)
                 if df_daily.at[date, 'unrealized_pnl']:
                     df_daily.at[date, 'unrealized_pnl'] = df_daily.at[date, 'unrealized_pnl'] + unrealized_pnl
                 else:
                     df_daily.at[date, 'unrealized_pnl'] = unrealized_pnl
 
@@ -381,15 +390,15 @@
         df = pl.read_parquet(save_path)
     else:
         df = pl.read_csv(save_path, try_parse_dates=True)
 
     # Calculate initial capital before trim the dataframe
     if len(df) == 0:
         # This would happen when it is summary mode and no trade for the strategy
-        # Note that in intra day but not summary mode, length of df of  no trade df_bakctest is still > 0
+        # Note that in intraday but not summary mode, length of df of  no trade df_bakctest is still > 0
         initial_capital = sec_profile['initial_capital']
     else:
         if pl.sum(df.get_column('realized_pnl')) == None:  # when NOT summary mode but no trade
             initial_capital = sec_profile['initial_capital']
         else:
             initial_capital = df.row(-1, named=True)['equity_value'] - pl.sum(df.get_column('realized_pnl'))
 
@@ -436,25 +445,27 @@
           .with_columns(pl.col('datetime').alias('date'))
           .with_columns([
         (pl.col('close') * (initial_capital / df.head(1)['close'][0])).alias('bah'),
         pl.lit(None).alias('equity_value'),
         pl.lit(None).alias('action'),
         pl.lit(None).alias('realized_pnl'),
         pl.lit(None).alias('unrealized_pnl'),
+        pl.lit(None).alias('commission'),
     ])
           .collect()
           )
 
     df_daily = df.to_pandas()
     df_daily.index = pd.to_datetime(df_daily['datetime'], format='%Y-%m-%d')
 
     # Apply apply_pnl on backtes here
     apply_pnl.last_realized_capital = last_realized_capital
     apply_pnl.multiplier = multiplier
     apply_pnl.df_daily = df_daily
+
     df_backtest.apply(apply_pnl, axis=1)
 
     df_daily = apply_pnl.df_daily
 
     df_daily = df_daily.reset_index(drop=True)
     df_daily_equity.last_equity_value = initial_capital
     df_daily['equity_value'] = df_daily.apply(df_daily_equity, axis=1).fillna(method='ffill')
@@ -485,14 +496,15 @@
         df_backtest['date'] = pd.to_datetime(df_backtest['date'], format='%Y-%m-%d')
         df_backtest = df_backtest.loc[(df_backtest['date'] >= start_date) & (df_backtest['date'] <= end_date)]
         df_backtest = df_backtest.reset_index(drop=True)  # Reset Index
         df_daily = df_backtest
 
     df = df_daily
 
+
     # Deter if equity_value unchange = no tade
     equity_value_column = df['equity_value'].to_numpy()
     no_trade = (equity_value_column[0] == equity_value_column).all()
 
     result_dict = {}
 
     # Determine years at the beginning
@@ -566,15 +578,16 @@
 
         if mdd_dollar == 0:
             result_dict['net_profit_to_mdd'] = np.inf
         else:
             result_dict['net_profit_to_mdd'] = net_profit / mdd_dollar
 
         # Cov
-        df3 = df[df['action'] == 'open']
+        # df3 = df[df['action'] == 'open']
+        df3 = df[df['action'].notnull()]
         df3 = df3.set_index('date')
         signal_year_count = df3.groupby(lambda x: x.year).size()
 
         signal_year_std = np.std(signal_year_count)
         signal_year_mean = np.mean(signal_year_count)
         cov = round(signal_year_std / signal_year_mean, 3)
```

### Comparing `plotguy-1.0.9/plotguy/aggregate.py` & `plotguy-1.1/plotguy/aggregate.py`

 * *Files identical despite different names*

### Comparing `plotguy-1.0.9/plotguy/components.py` & `plotguy-1.1/plotguy/components.py`

 * *Files identical despite different names*

### Comparing `plotguy-1.0.9/plotguy/equity_curves.py` & `plotguy-1.1/plotguy/equity_curves.py`

 * *Files identical despite different names*

### Comparing `plotguy-1.0.9/plotguy/signals.py` & `plotguy-1.1/plotguy/signals.py`

 * *Files identical despite different names*

### Comparing `plotguy-1.0.9/setup.py` & `plotguy-1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="plotguy",
-    version="1.0.9",
+    version="1.1",
     author="Plotguy Team",
     author_email="plotguy.info@gmail.com",
     description="Plotguy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[         
         'pandas>=1.5.2',
```

