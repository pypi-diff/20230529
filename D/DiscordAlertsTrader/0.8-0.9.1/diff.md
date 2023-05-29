# Comparing `tmp/DiscordAlertsTrader-0.8.tar.gz` & `tmp/DiscordAlertsTrader-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DiscordAlertsTrader-0.8.tar", last modified: Fri May 19 18:58:26 2023, max compression
+gzip compressed data, was "DiscordAlertsTrader-0.9.1.tar", last modified: Mon May 29 02:33:47 2023, max compression
```

## Comparing `DiscordAlertsTrader-0.8.tar` & `DiscordAlertsTrader-0.9.1.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 18:58:26.656658 DiscordAlertsTrader-0.8/
-drwxrwxrwx   0        0        0        0 2023-05-19 18:58:26.621740 DiscordAlertsTrader-0.8/DiscordAlertsTrader/
--rw-rw-rw-   0        0        0       49 2023-05-16 00:10:52.000000 DiscordAlertsTrader-0.8/DiscordAlertsTrader/__init__.py
--rw-rw-rw-   0        0        0    13513 2023-05-18 15:07:18.000000 DiscordAlertsTrader-0.8/DiscordAlertsTrader/alerts_tracker.py
--rw-rw-rw-   0        0        0    51265 2023-05-17 16:26:21.000000 DiscordAlertsTrader-0.8/DiscordAlertsTrader/alerts_trader.py
-drwxrwxrwx   0        0        0        0 2023-05-19 18:58:26.639700 DiscordAlertsTrader-0.8/DiscordAlertsTrader/brokerages/
--rw-rw-rw-   0        0        0    11938 2023-05-16 00:10:52.000000 DiscordAlertsTrader-0.8/DiscordAlertsTrader/brokerages/TDA_api.py
--rw-rw-rw-   0        0        0     2055 2023-05-16 00:10:52.000000 DiscordAlertsTrader-0.8/DiscordAlertsTrader/brokerages/__init__.py
--rw-rw-rw-   0        0        0     2814 2023-05-19 12:29:33.000000 DiscordAlertsTrader-0.8/DiscordAlertsTrader/configurator.py
--rw-rw-rw-   0        0        0    10061 2023-05-17 13:08:19.000000 DiscordAlertsTrader-0.8/DiscordAlertsTrader/discord_bot.py
--rw-rw-rw-   0        0        0    10697 2023-05-19 12:29:33.000000 DiscordAlertsTrader-0.8/DiscordAlertsTrader/gui.py
--rw-rw-rw-   0        0        0    19169 2023-05-19 12:29:33.000000 DiscordAlertsTrader-0.8/DiscordAlertsTrader/gui_generator.py
--rw-rw-rw-   0        0        0    11894 2023-05-19 12:29:33.000000 DiscordAlertsTrader-0.8/DiscordAlertsTrader/gui_layouts.py
--rw-rw-rw-   0        0        0    21180 2023-05-19 14:45:25.000000 DiscordAlertsTrader-0.8/DiscordAlertsTrader/message_parser.py
-drwxrwxrwx   0        0        0        0 2023-05-19 18:58:26.634706 DiscordAlertsTrader-0.8/DiscordAlertsTrader.egg-info/
--rw-rw-rw-   0        0        0     7442 2023-05-19 18:58:26.000000 DiscordAlertsTrader-0.8/DiscordAlertsTrader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      863 2023-05-19 18:58:26.000000 DiscordAlertsTrader-0.8/DiscordAlertsTrader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 18:58:26.000000 DiscordAlertsTrader-0.8/DiscordAlertsTrader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2023-05-19 18:58:26.000000 DiscordAlertsTrader-0.8/DiscordAlertsTrader.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       77 2023-05-19 18:58:26.000000 DiscordAlertsTrader-0.8/DiscordAlertsTrader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-05-19 18:58:26.000000 DiscordAlertsTrader-0.8/DiscordAlertsTrader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1545 2023-05-16 00:10:52.000000 DiscordAlertsTrader-0.8/LICENSE
--rw-rw-rw-   0        0        0     7442 2023-05-19 18:58:26.655647 DiscordAlertsTrader-0.8/PKG-INFO
--rw-rw-rw-   0        0        0     6392 2023-05-17 00:54:31.000000 DiscordAlertsTrader-0.8/README.md
--rw-rw-rw-   0        0        0      921 2023-05-19 18:40:23.000000 DiscordAlertsTrader-0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-19 18:58:26.656658 DiscordAlertsTrader-0.8/setup.cfg
--rw-rw-rw-   0        0        0     1648 2023-05-19 18:58:22.000000 DiscordAlertsTrader-0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 18:58:26.653671 DiscordAlertsTrader-0.8/tests/
--rw-rw-rw-   0        0        0      119 2023-04-03 23:24:29.000000 DiscordAlertsTrader-0.8/tests/__init__.py
--rw-rw-rw-   0        0        0     2260 2023-05-16 17:53:11.000000 DiscordAlertsTrader-0.8/tests/msg_samples.py
--rw-rw-rw-   0        0        0    11167 2023-05-15 17:17:09.000000 DiscordAlertsTrader-0.8/tests/td_dummy.py
--rw-rw-rw-   0        0        0      622 2023-05-16 13:25:58.000000 DiscordAlertsTrader-0.8/tests/test_AlertsTracker.py
--rw-rw-rw-   0        0        0      872 2023-04-03 23:24:29.000000 DiscordAlertsTrader-0.8/tests/test_TDsession.py
--rw-rw-rw-   0        0        0      927 2023-05-16 00:15:43.000000 DiscordAlertsTrader-0.8/tests/test_configurator.py
--rw-rw-rw-   0        0        0     3067 2023-05-17 13:09:50.000000 DiscordAlertsTrader-0.8/tests/test_discord_bot.py
+drwxrwxrwx   0        0        0        0 2023-05-29 02:33:47.641187 DiscordAlertsTrader-0.9.1/
+drwxrwxrwx   0        0        0        0 2023-05-29 02:33:47.616120 DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/
+-rw-rw-rw-   0        0        0       47 2023-05-29 02:14:18.000000 DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/__init__.py
+-rw-rw-rw-   0        0        0    13816 2023-05-27 01:57:29.000000 DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/alerts_tracker.py
+-rw-rw-rw-   0        0        0    51976 2023-05-27 01:57:29.000000 DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/alerts_trader.py
+drwxrwxrwx   0        0        0        0 2023-05-29 02:33:47.630236 DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/brokerages/
+-rw-rw-rw-   0        0        0    11921 2023-05-24 00:30:53.000000 DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/brokerages/TDA_api.py
+-rw-rw-rw-   0        0        0     2337 2023-05-24 01:10:46.000000 DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/brokerages/__init__.py
+-rw-rw-rw-   0        0        0    22459 2023-05-27 01:57:29.000000 DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/brokerages/eTrade_api.py
+-rw-rw-rw-   0        0        0     2776 2023-05-20 18:48:10.000000 DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/configurator.py
+-rw-rw-rw-   0        0        0    10361 2023-05-24 02:30:34.000000 DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/discord_bot.py
+-rw-rw-rw-   0        0        0     1730 2023-05-22 13:47:39.000000 DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/fend_bot.py
+-rw-rw-rw-   0        0        0    12823 2023-05-27 21:36:28.000000 DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/gui.py
+-rw-rw-rw-   0        0        0    20630 2023-05-25 10:54:19.000000 DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/gui_generator.py
+-rw-rw-rw-   0        0        0    12478 2023-05-27 13:36:36.000000 DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/gui_layouts.py
+-rw-rw-rw-   0        0        0    22302 2023-05-23 19:53:15.000000 DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/message_parser.py
+drwxrwxrwx   0        0        0        0 2023-05-29 02:33:47.626224 DiscordAlertsTrader-0.9.1/DiscordAlertsTrader.egg-info/
+-rw-rw-rw-   0        0        0     7780 2023-05-29 02:33:47.000000 DiscordAlertsTrader-0.9.1/DiscordAlertsTrader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      953 2023-05-29 02:33:47.000000 DiscordAlertsTrader-0.9.1/DiscordAlertsTrader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 02:33:47.000000 DiscordAlertsTrader-0.9.1/DiscordAlertsTrader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2023-05-29 02:33:47.000000 DiscordAlertsTrader-0.9.1/DiscordAlertsTrader.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       86 2023-05-29 02:33:47.000000 DiscordAlertsTrader-0.9.1/DiscordAlertsTrader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-05-29 02:33:47.000000 DiscordAlertsTrader-0.9.1/DiscordAlertsTrader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1545 2023-05-16 00:10:52.000000 DiscordAlertsTrader-0.9.1/LICENSE
+-rw-rw-rw-   0        0        0     7780 2023-05-29 02:33:47.641187 DiscordAlertsTrader-0.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6918 2023-05-24 03:41:23.000000 DiscordAlertsTrader-0.9.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-29 02:33:47.642187 DiscordAlertsTrader-0.9.1/setup.cfg
+-rw-rw-rw-   0        0        0     1660 2023-05-29 02:33:10.000000 DiscordAlertsTrader-0.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 02:33:47.640190 DiscordAlertsTrader-0.9.1/tests/
+-rw-rw-rw-   0        0        0      119 2023-04-03 23:24:29.000000 DiscordAlertsTrader-0.9.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     2352 2023-05-23 17:16:45.000000 DiscordAlertsTrader-0.9.1/tests/msg_samples.py
+-rw-rw-rw-   0        0        0    11167 2023-05-15 17:17:09.000000 DiscordAlertsTrader-0.9.1/tests/td_dummy.py
+-rw-rw-rw-   0        0        0      622 2023-05-16 13:25:58.000000 DiscordAlertsTrader-0.9.1/tests/test_AlertsTracker.py
+-rw-rw-rw-   0        0        0      872 2023-04-03 23:24:29.000000 DiscordAlertsTrader-0.9.1/tests/test_TDsession.py
+-rw-rw-rw-   0        0        0      927 2023-05-16 00:15:43.000000 DiscordAlertsTrader-0.9.1/tests/test_configurator.py
+-rw-rw-rw-   0        0        0     3068 2023-05-20 18:46:17.000000 DiscordAlertsTrader-0.9.1/tests/test_discord_bot.py
+-rw-rw-rw-   0        0        0     2248 2023-05-20 17:13:46.000000 DiscordAlertsTrader-0.9.1/tests/test_gui_generator.py
```

### Comparing `DiscordAlertsTrader-0.8/DiscordAlertsTrader/alerts_tracker.py` & `DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/alerts_tracker.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,29 +24,30 @@
 
         if op.exists(self.portfolio_fname):
             self.portfolio = pd.read_csv(self.portfolio_fname)
         else:
             self.portfolio = pd.DataFrame(columns=cfg["col_names"]['tracker_portfolio'].split(",") )
             self.portfolio.to_csv(self.portfolio_fname, index=False)
 
-    def price_now(self, symbol, price_type="BTO"):
+    def price_now(self, symbol:str, price_type="BTO"):
         if self.bksession is None:
             return None
 
         if price_type in ["BTO", "BTC"]:
             ptype = 'askPrice'
         else:
             ptype = 'bidPrice'
 
         quote = self.bksession.get_quotes([symbol])
         if quote is None:
+            # Try it again in case of TDA
             quote = self.bksession.get_quotes([symbol])
             
-        if quote is not None and len(quote):
-            quote = quote.get(symbol)[ptype]
+        if quote is not None and len(quote) and quote.get(symbol).get('description' ) != 'Symbol not found':
+            quote = quote.get(symbol).get(ptype)
             if quote != 0:
                 return quote
             else:
                 print("quote 0 for", symbol, price_type)
 
     def trade_alert(self, order, live_alert=True, channel=None):
         open_trade, _ = find_last_trade(order, self.portfolio, open_only=True)
@@ -56,14 +57,15 @@
         if order["action"] in ["BTO", "STC"] and live_alert:
             if order.get('Actual Cost', 'None') == 'None':
                 order["Actual Cost"] = self.price_now(order["Symbol"], order["action"])
 
         if open_trade is None and order["action"] == "BTO":
             str_act = self.make_BTO(order, channel)
         elif order["action"] == "BTO":
+            # str_act = "BTO averaging disabled as it is mostly wrong alert messages"
             str_act = self.make_BTO_Avg(order, open_trade)
         elif order["action"] == "STC" and open_trade is None:
             str_act = "STC without BTO"
         elif order["action"] == "STC":
             str_act = self.make_STC(order, open_trade)
         elif order["action"] == "ExitUpdate":
             if open_trade is not None:
@@ -141,28 +143,30 @@
             self.portfolio.loc[open_trade, k] = v
         
         trailstat = self.compute_trail(open_trade)
         self.portfolio.loc[open_trade, "TrailStats"] = trailstat
         self.portfolio.loc[open_trade, "STC-Date"] = order["Date"]
         stc_price =  self.portfolio.loc[open_trade,"STC-Price"]
         stc_utotal = self.portfolio.loc[open_trade,"STC-Amount"]
-        
+        suffx = ''
+        if stc_utotal >= trade['Amount']:
+            suffx = " Closed"
+            self.portfolio.loc[open_trade, "isOpen"] = 0
+            
         if stc_price == "none" or stc_price is None:
-            str_STC = f"STC {order['Symbol']}  ({order['uQty']}), no price provided"
+            str_STC = f"STC {order['Symbol']}  ({order['uQty']}), no price provided" + suffx
         else:
-            str_STC = f"STC {order['Symbol']} ({order['uQty']}), {stc_price:.2f}"
+            str_STC = f"STC {order['Symbol']} ({order['uQty']}),{suffx} {stc_price:.2f}"
             if stc_info['STC-Price-current'] is not None:           
                        str_STC += f" current: {stc_info['STC-Price-current']:.2f} " 
             if stc_info["STC-PnL"] is not None:
                 str_STC += f'PnL:{round(stc_info["STC-PnL"])}% ${round(stc_info["STC-PnL$"])}' 
             if stc_info["STC-PnL-current"] is not None:
                 str_STC += f' Actual:{round(stc_info["STC-PnL-current"])}% ${round(stc_info["STC-PnL$-current"])}\n\t\t'
-        if stc_utotal >= trade['Amount']:
-            str_STC = str_STC +" Closed"
-            self.portfolio.loc[open_trade, "isOpen"] = 0
+
         if eval(order.get('# Closed', "0"))==1 :
             self.portfolio.loc[open_trade, "isOpen"]=0
         str_STC = str_STC + " " + trailstat.replace('|', '\n\t\t')
         return str_STC
 
     def compute_trail(self, open_trade):
         trade = self.portfolio.loc[open_trade]
@@ -202,14 +206,16 @@
             tdiff_str, trl_r = self.trailing_get_time(trade['Date'], quotes, ix)
             quotes_stats += f"{st},{trl_r['perc']}%,${trl_r[' quote']},in {tdiff_str}| "
         quotes_stats +=  "| " + max_trails
         return quotes_stats
 
     def trailing_get_time(self, trade_date, quotes, inx):
         trl_r = quotes.loc[inx]
+        if pd.isna(trl_r['timestamp']):
+            return "", trl_r
         tdiff =  datetime.fromtimestamp(trl_r['timestamp']) - pd.to_datetime(trade_date)
         tdiff_str = str(tdiff.round('s')).replace('0 days ','')
         return tdiff_str, trl_r
 
     def close_expired(self):
         for i, trade in  self.portfolio.iterrows():
             if trade["Asset"] != "option" or trade["isOpen"] == 0:
```

### Comparing `DiscordAlertsTrader-0.8/DiscordAlertsTrader/alerts_trader.py` & `DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/alerts_trader.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 import pandas as pd
 from datetime import datetime, date
 import time
 import threading
 import queue
 from colorama import Fore, Back
 
-from .configurator import cfg
-from .message_parser import parse_exit_plan, set_exit_price_type
+from DiscordAlertsTrader.configurator import cfg
+from DiscordAlertsTrader.message_parser import parse_exit_plan, set_exit_price_type
 
 
 def find_last_trade(order, trades_log, open_only=True):
     trades_authr = trades_log["Trader"] == order["Trader"]
     trades_log = trades_log.loc[trades_authr]
 
     msk_ticker = trades_log["Symbol"].str.match(f"{order['Symbol']}$")
@@ -141,15 +141,15 @@
     def price_now(self, symbol, price_type="BTO", pflag=0):
         if price_type in ["BTO", "BTC"]:
             ptype = 'askPrice'
         else:
             ptype= 'bidPrice'
         try:
             resp = self.bksession.get_quotes([symbol])
-            if resp is None or len(resp) == 0  or resp[symbol].get('description' ) == 'Symbol not found':
+            if resp is None or len(resp) == 0 or symbol not in resp.keys() or resp[symbol].get('description' ) == 'Symbol not found' :
                 str_msg =  f"{symbol} not found during price quote"
                 print (Back.RED + str_msg)
                 self.queue_prints.put([str_msg, "", "red"])
                 quote = -1
             else:
                 quote = resp[symbol][ptype]
         except KeyError as e:
@@ -240,15 +240,15 @@
                         uQty_ori = order['uQty']
                         order['uQty'] =  int(max(max_trade_val//price, 1))
                         if price * order['uQty'] <= max_trade_val:
                             str_msg = f"BTO trade exeeded max_trade_capital of ${max_trade_val}, order quantity reduced to {order['uQty']} from {uQty_ori}"
                             print(Back.GREEN + str_msg)
                             self.queue_prints.put([str_msg, "", "green"])
                         else:
-                            str_msg = "cancelled BTO: trade exeeded max_trade_capital of ${max_trade_val}"
+                            str_msg = f"cancelled BTO: trade exeeded max_trade_capital of ${max_trade_val}"
                             print(Back.RED + str_msg)
                             self.queue_prints.put([str_msg, "", "red"])
                             return "no", order, False
                 return "yes", order, False
 
             # Manual trade 
             resp = input(Back.RED  + question + "\n Make trade? (y, n or (c)hange) \n").lower()
@@ -262,15 +262,15 @@
                 new_order['price'] = float(input(f"Change price @{order['price']}" +
                                         f" {price_now(symb, act)}? Leave blank if NO \n")
                                       or order['price'])
 
                 if order['action'] == 'BTO':
                     PTs = [order[f'PT{i}'] for i in range(1,4)]
                     PTs = eval(input(f"Change PTs @{PTs} {price_now(symb, act)}? \
-                                      Leave blank if NO, respnd eg [1, 2, None] \n")
+                                      Leave blank if NO, respond eg [1, 2, None] \n")
                                       or str(PTs))
 
                     new_n = len([i for i in PTs if i is not None ])
                     if new_n != order['n_PTs']:
                         new_order['n_PTs']= new_n
                         new_order['PTs_Qty'] = [round(1/new_n,2) for i in range(new_n)]
                         new_order['PTs_Qty'][-1] = new_order['PTs_Qty'][-1] + (1- sum(new_order['PTs_Qty']))
@@ -296,15 +296,15 @@
         for i in STCn:
             if pd.isnull(position[ f"STC{i}-ordID"]):
                 continue
 
             order_id =  int(position[ f"STC{i}-ordID"])
             ord_stat, _ = self.get_order_info(order_id)
 
-            if ord_stat not in ["FILLED", 'CANCELED', 'REJECTED']:
+            if ord_stat not in ["FILLED", "EXECUTED", 'CANCELED','CANCEL_REQUESTED','REJECTED', 'EXPIRED']:
                 print(Back.GREEN + f"Cancelling {position['Symbol']} STC{i}")
                 self.queue_prints.put([f"Cancelling {position['Symbol']} STC{i}", "", "green"])
                 _ = self.bksession.cancel_order(order_id)
 
                 self.portfolio.loc[open_trade, f"STC{i}-Status"] = np.nan
                 self.portfolio.loc[open_trade, f"STC{i}-ordID"] = np.nan
                 self.save_logs("port")
@@ -433,30 +433,29 @@
                          "Trader" : order['Trader'],
                          "Risk" : order['risk'],
                          "SL_mental" : order.get("SL_mental")
                          }
 
             self.portfolio = pd.concat([self.portfolio, pd.DataFrame.from_records(new_trade, index=[0])], ignore_index=True)
             
-            if order_status == "FILLED":
+            if order_status in ["FILLED", "EXECUTED"]:
                 ot, _ = find_last_trade(order, self.portfolio)
                 self.portfolio.loc[ot, "Price"] = order_info['price']
                 self.portfolio.loc[ot, "filledQty"] = order_info['filledQuantity']
             print(Back.GREEN + f"BTO {order['Symbol']} executed @ {order_info['price']}. Status: {order_status}")
             self.queue_prints.put([f"BTO {order['Symbol']} executed. Status: {order_status}", "", "green"])
 
             #Log portfolio, trades_log
             log_alert['action'] = "BTO"
             log_alert["portfolio_idx"] = len(self.portfolio) - 1
             self.alerts_log = pd.concat([self.alerts_log, pd.DataFrame.from_records(log_alert, index=[0])], ignore_index=True)
             self.save_logs()
 
-
         elif order["action"] == "BTO" and order['avg'] is not None:
-            # if PT in order: cancel previous and make_BTO_PT_SL_order
+            # if PT in order: cancel previous and make_BTO_lim_rder
             # else : BTO
             alert_price = order['price']
             order_response, order_id, order, _ = self.confirm_and_send(order, pars,
                                                                        self.bksession.make_BTO_lim_order)
             self.save_logs("port")
             if order_response is None:  #Assume trade not accepted
                 log_alert['action'] = "BTO-Avg-notAccepted"
@@ -484,15 +483,15 @@
                 self.portfolio.loc[open_trade, "Avged-prices-alert"] = f"{al_pr},{alert_price}"
                 self.portfolio.loc[open_trade, "Avged-prices"] = f"{av_pr},{order_info['price']}"
                 self.portfolio.loc[open_trade, "Avged-uQty"] = f"{av_qt},{order_info['quantity']}"
 
             avg = self.portfolio.loc[open_trade, "Avged"]
 
             self.portfolio.loc[open_trade, "uQty"] += order_info['quantity']
-            if order_status == "FILLED":
+            if  order_status in ["FILLED", "EXECUTED"]:
                 self.portfolio.loc[open_trade, "filledQty"] += order_info['filledQuantity']
                 self.close_open_exit_orders(open_trade)
             str_msg =  f"BTO {avg} th AVG, {order['Symbol']} executed. Status: {order_status}"
             print(Back.GREEN + str_msg)
             self.queue_prints.put([str_msg, "", "green"])
 
             #Log portfolio, trades_log
@@ -511,16 +510,17 @@
 
         elif order["action"] == "STC" and isOpen == 0:
             open_trade, _ = find_last_trade(order, self.portfolio, open_only=False)
             if open_trade is None:
                 log_alert['action'] = str_msg = f"STC-alerted without open position"
                 self.alerts_log = pd.concat([self.alerts_log, pd.DataFrame.from_records(log_alert, index=[0])], ignore_index=True)
                 self.save_logs()
-                print(Back.GREEN + str_msg)
-                self.queue_prints.put([str_msg, "", "green"])
+                if cfg['general'].getboolean('DO_BTO_TRADES'):
+                    print(Back.GREEN + str_msg)
+                    self.queue_prints.put([str_msg, "", "green"])
                 return
 
             position = self.portfolio.iloc[open_trade]
             # Check if closed position was not alerted
             for i in range(1,4):
                 STC = f"STC{i}"
                 if pd.isnull(position[f"{STC}-Alerted"]):
@@ -581,16 +581,16 @@
                 log_alert["portfolio_idx"] = open_trade
                 self.alerts_log = pd.concat([self.alerts_log, pd.DataFrame.from_records(log_alert, index=[0])], ignore_index=True)
                 self.save_logs(["alert"])
                 return
 
             qty_bought = position["filledQty"]
 
-            if position["BTO-Status"] == "CANCELED":
-                log_alert['action'] = "STC-already cancelled"
+            if position["BTO-Status"] in ["CANCELED", "REJECTED", "EXPIRED", "CANCEL_REQUESTED"]:
+                log_alert['action'] = "Trade-already cancelled"
                 log_alert["portfolio_idx"] = open_trade
                 self.alerts_log = pd.concat([self.alerts_log, pd.DataFrame.from_records(log_alert, index=[0])], ignore_index=True)
                 self.save_logs(["alert"])
                 return
 
             # Close position of STC All or STC SL
             if qty_bought == 0 and order['xQty'] == 1:
@@ -631,22 +631,25 @@
 
                 log_alert['action'] = f"{STC}-DoneBefore"
                 log_alert["portfolio_idx"] = open_trade
                 self.alerts_log = pd.concat([self.alerts_log, pd.DataFrame.from_records(log_alert, index=[0])], ignore_index=True)
                 self.save_logs(["alert"])
                 return
 
-            if order['xQty'] == 1 and order['uQty'] is None:
+            # Sell all and close waiting stc orders
+            if order['xQty'] == 1:                
                 # Stop updater to avoid overlapping
                 self.update_paused = True
                 # Sell all and close waiting stc orders
                 self.close_open_exit_orders(open_trade)
-
-                position = self.portfolio.iloc[open_trade]
-                order['uQty'] = int(position["uQty"]) - qty_sold
+                
+                # if no uQty get all remaining
+                if order['uQty'] is None:
+                    position = self.portfolio.iloc[open_trade]
+                    order['uQty'] = int(position["uQty"]) - qty_sold
 
             elif order['xQty'] < 1:  # portion
                 # Stop updater to avoid overlapping
                 self.update_paused = True
                 self.close_open_exit_orders(open_trade)
                 order['uQty'] = round(max(qty_bought * order['xQty'], 1))
 
@@ -669,15 +672,15 @@
                 return
 
             order_status, order_info = self.get_order_info(order_id)
             self.portfolio.loc[open_trade, STC + "-ordID"] = order_id
             self.portfolio.loc[open_trade, STC + "-Price-Current"] = order["price_current"]
 
             # Check if STC price changed
-            if order_status == "FILLED":
+            if order_status in ["FILLED", 'EXECUTED', 'INDIVIDUAL_FILLS']:
                 self.log_filled_STC(order_id, open_trade, STC)
             else:
                 str_STC = f"Submitted: {STC} {order['Symbol']} @{order['price']} Qty:{order['uQty']} ({order['xQty']})"
                 print(Back.GREEN + str_STC)
                 self.queue_prints.put([str_STC, "", "green"])
 
             #Log trades_log
@@ -735,20 +738,20 @@
         self.portfolio.loc[open_trade, "$PnL"] =  stc_PnL_all* bto_price *mutipl*sold_tot
         self.portfolio.loc[open_trade, "$PnL-Alert"] =  stc_PnL_all_alert* bto_price_alert *mutipl*sold_tot
         self.portfolio.loc[open_trade, "$PnL-Current"] =  stc_PnL_all_curr* bto_price_current *mutipl*sold_tot
         
         
         symb = self.portfolio.loc[open_trade, 'Symbol']
 
-        sold_Qty =  self.portfolio.loc[open_trade, [f"STC{i}-xQty" for i in range(1,4)]].sum()
+        sold_Qty =  self.portfolio.loc[open_trade, [f"STC{i}-uQty" for i in range(1,4)]].sum()
 
         str_STC = f"{STC} {symb} @{stc_price} Qty:" + \
             f"{sold_unts}({int(xQty*100)}%), for {stc_PnL:.2f}%"
 
-        if sold_Qty == 1:
+        if sold_Qty == self.portfolio.loc[open_trade, "uQty"]:
             str_STC += " (Closed)"
             self.portfolio.loc[open_trade, "isOpen"] = 0
 
         print (Back.GREEN + f"Filled: {str_STC}")
         self.queue_prints.put([f"Filled: {str_STC}","", "green"])
         self.save_logs()
 
@@ -759,15 +762,15 @@
             self.close_expired(i)
             trade = self.portfolio.iloc[i]
             redo_orders = False
 
             if trade["isOpen"] == 0:
                 continue
 
-            if trade["BTO-Status"]  in ["QUEUED", "WORKING"]:
+            if trade["BTO-Status"]  in ["QUEUED", "WORKING", 'OPEN']:
                 _, order_info = self.get_order_info(trade['ordID'])
 
                 # Check if number filled Qty changed
                 qty_fill = order_info['filledQuantity']
                 qty_fill_old = self.portfolio.loc[i, "filledQty"]
                 # If so, redo orders
                 if not (pd.isnull(qty_fill_old) or qty_fill_old == 0) and \
@@ -778,30 +781,30 @@
                 self.portfolio.loc[i, "BTO-Status"] = order_info['status']
                 trade = self.portfolio.iloc[i]
                 self.save_logs("port")
 
             if pd.isnull(trade["filledQty"]) or trade["filledQty"] == 0:
                 continue
 
-            if trade.get("BTO-avg-Status") in ["QUEUED", "WORKING"]:
+            if trade.get("BTO-avg-Status") in ["QUEUED", "WORKING", 'OPEN']:
                 ordID = trade['ordID'].split(",")[-1]
                 _, order_info = self.get_order_info(ordID)
                 if order_info['status'] == 'FILLED' :
                     self.portfolio.loc[i, "BTO-avg-Status"] = order_info['status']
                     self.portfolio.loc[i, "filledQty"] += order_info['filledQuantity']
                     redo_orders = True
                     trade = self.portfolio.iloc[i]
                     self.save_logs("port")
 
             if redo_orders:
                 self.close_open_exit_orders(i)
 
             exit_plan = eval(trade["exit_plan"])
             if  exit_plan != {}:                
-                if any([isinstance(e, str) for e in exit_plan.values()]) and trade['Asset'] == 'option':
+                if any([isinstance(e, str) and "%" not in e for e in exit_plan.values()]) and trade['Asset'] == 'option':
                     self.check_opt_stock_price(i, exit_plan, "STC")
                 else:
                     self.make_exit_orders(i, exit_plan)
 
             # Go over STC orders and check status
             for ii in range(1, 4):
                 STC = f"STC{ii}"
@@ -813,25 +816,24 @@
 
                 # Get status exit orders
                 STC_ordID = int(float(STC_ordID))  # Might be read as a float
 
                 order_status, _ =  self.get_order_info(STC_ordID)
 
                 if order_status == 'CANCELED':
-                    # Try next order number. probably went through
+                    # Try next order number. probably went through. This is for TDA OCO
                     order_status, _ =  self.get_order_info(STC_ordID + 1)
-
                     if order_status == 'FILLED':
                         STC_ordID = STC_ordID + 1
                         self.portfolio.loc[i, STC + "-ordID"] =  STC_ordID
 
                 self.portfolio.loc[i, STC+"-Status"] = order_status
                 trade = self.portfolio.iloc[i]
 
-                if order_status == "FILLED" and np.isnan(trade[STC+"-xQty"]):
+                if order_status in ["FILLED", "EXECUTED"] and np.isnan(trade[STC+"-xQty"]):
                     self.log_filled_STC(STC_ordID, i, STC)
 
         self.save_logs("port")
 
 
     def check_opt_stock_price(self, open_trade, exit_plan, act="STC"):
         "Option exits in stock price"
@@ -1063,7 +1065,12 @@
             order['uQty'] = max(round(available * order['xQty']), 1)
         else:
             raise ValueError
         return order, True
     else:
         return order, False
 
+if __name__ == "__main__":
+    from DiscordAlertsTrader.brokerages import get_brokerage
+    
+    bksession = get_brokerage()
+    at = AlertsTrader(bksession)
```

### Comparing `DiscordAlertsTrader-0.8/DiscordAlertsTrader/brokerages/TDA_api.py` & `DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/brokerages/TDA_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 from ..configurator import cfg
 from . import BaseBroker
 
 from td.orders import Order, OrderLeg
 from td.client import TDClient
 
 class TDA(BaseBroker):
-    def __init__(self):
-        pass
+    def __init__(self,account_n=0, accountId=None):
+        self.account_n = account_n
+        self.accountId = accountId
 
-    def get_session(self, account_n=0, accountId=None):
+    def get_session(self, ):
         """Provide either:
             - account_n: indicating the orinal position from the accounts list
             (if only one account, it will be 0)
             - accountId: Number of the account
 
         auth is a dict with login info created with setup.py
         """
@@ -26,62 +27,61 @@
             redirect_uri=cfg['TDA']['redirect_url'],
             credentials_path=cfg['TDA']['credentials_path']
         )
 
         # Login to the session
         success = self.session.login()
 
-        if accountId is not None:
-            self.session.accountId = accountId
+        if self.accountId is not None:
+            self.session.accountId = self.accountId
         else:
-            account_n = 0
-            accounts_info = self.session.get_accounts(account="all")[account_n]
-            self.session.accountId = accounts_info['securitiesAccount']['accountId']
+            self.account_n = 0
+            accounts_info = self.session.get_accounts(account="all")[self.account_n]
+            self.accountId = accounts_info['securitiesAccount']['accountId']
         return success
 
     def send_order(self, new_order):
-        order_response = self.session.place_order(account=self.session.accountId,
+        order_response = self.session.place_order(account=self.accountId,
                                         order=new_order)
         order_id = order_response["order_id"]
         return order_response, order_id
     
     def cancel_order(self, order_id):
-        return self.session.cancel_order(self.session.accountId, order_id)
+        return self.session.cancel_order(self.accountId, order_id)
 
     def get_order_info(self, order_id):  
         """
         order_status = 'REJECTED' | "FILLED" | "WORKING"
         """      
-        order_info = self.session.get_orders(account=self.session.accountId,
-                                              order_id=order_id)
+        order_info = self.session.get_orders(account=self.accountId, order_id=order_id)
         if order_info['orderStrategyType'] == "OCO":
             order_status = [
                 order_info['childOrderStrategies'][0]['status'],
                 order_info['childOrderStrategies'][1]['status']]
             if not order_status[0]==order_status[1]:
-                print("OCO order status are different in ordID {order_id}: ",
+                print(f"OCO order status are different in ordID {order_id}: ",
                       f"{order_status[0]} vs {order_status[1]}")
             order_status = order_status[0]
         elif order_info['orderStrategyType'] in ['SINGLE', 'TRIGGER']:
             order_status = order_info['status']
         else:
             raise TypeError("Not sure type order. Check")
         return order_status, order_info
 
     def get_quotes(self, symbol:list):
         return self.session.get_quotes(instruments=symbol)
 
-    def get_open_orders(self):
+    def get_orders(self):
         pass
 
     def get_order_status(self, order_id):
         pass
     
     def get_account_info(self):
-        acc_inf = self.session.get_accounts(self.session.accountId, ['orders','positions'])
+        acc_inf = self.session.get_accounts(self.accountId, ['orders','positions'])
         return acc_inf
 
     def get_positions_orders(self):
         acc_inf = self.get_account_info()
 
         df_pos = pd.DataFrame(columns=["symbol", "asset", "type", "Qty", "Avg Price", "PnL", "PnL %"])
 
@@ -227,29 +227,29 @@
             order_leg.order_leg_asset(asset_type='OPTION', symbol=Symbol)
         else:
             order_leg.order_leg_instruction(instruction="SELL")
             order_leg.order_leg_asset(asset_type='EQUITY', symbol=Symbol)
         new_order.add_order_leg(order_leg=order_leg)
         return new_order
 
-    def make_STC_SL_trailstop(self, Symbol:str, uQty:int,  trail_stop_percent:float, new_order=None, strike=None, **kwarg):
+    def make_STC_SL_trailstop(self, Symbol:str, uQty:int,  trail_stop_percent:float, new_order=None, **kwarg):
         if new_order is None:
             new_order = Order()
         new_order.order_strategy_type("SINGLE")
         new_order.order_strategy_type("SINGLE")
         new_order.order_type("TRAILING_STOP")
         new_order.order_session('NORMAL')
         new_order.order_duration('GOOD_TILL_CANCEL')
         new_order.stop_price_offset(trail_stop_percent)
         new_order.stop_price_link_type('PERCENT')
         new_order.stop_price_link_basis('BID')
         
         child_order_leg = OrderLeg()
         child_order_leg.order_leg_quantity(quantity=uQty)
-        if strike is not None:
+        if len(Symbol.split("_")) > 1:
             child_order_leg.order_leg_instruction(instruction="SELL_TO_CLOSE")
             child_order_leg.order_leg_asset(asset_type='OPTION', symbol=Symbol)
         else:
             child_order_leg.order_leg_instruction(instruction="SELL")
             child_order_leg.order_leg_asset(asset_type='EQUITY', symbol=Symbol)
         new_order.add_order_leg(order_leg=child_order_leg)
         return new_order
```

### Comparing `DiscordAlertsTrader-0.8/DiscordAlertsTrader/brokerages/__init__.py` & `DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/brokerages/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,20 +19,20 @@
         pass
 
     @abstractmethod
     def cancel_order(self, order_id):
         pass
 
     @abstractmethod
-    def get_open_orders(self):
+    def get_orders(self):
         pass
 
-    @abstractmethod
-    def get_order_status(self, order_id):
-        pass
+    # @abstractmethod
+    # def get_order_status(self, order_id):
+    #     pass
     
     def get_order_info(self, order_id):
         #     sold_unts = order_info['orderLegCollection'][0]['quantity']
 
         # if 'price' in order_info.keys():
         #     stc_price = order_info['price']
         # elif 'stopPrice' in order_info.keys():
@@ -52,16 +52,23 @@
         # xQty = sold_unts/ self.portfolio.loc[open_trade, "uQty"]
 
         # date = order_info["closeTime"]
         pass
 
 
 def get_brokerage(name=cfg['general']['BROKERAGE']):
-    if name == 'TDA':
+    if name.lower() == 'tda':
         from .TDA_api import TDA
         tda = TDA()
         tda.get_session()
         return tda
     elif name == "webull":
         NotImplemented
-    elif name == 'etrades':
-        NotImplemented
+    elif name.lower() == 'etrade':
+        from .eTrade_api import eTrade
+        et = eTrade()
+        try:
+            et.get_session()
+        except Exception as e:
+            print("Got error: \n", e, "\n Trying again...if it fails again, rerun the application.")
+            et.get_session()
+        return et
```

### Comparing `DiscordAlertsTrader-0.8/DiscordAlertsTrader/configurator.py` & `DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/configurator.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 if ext == "":    
     cfg['general']['data_dir'] = os.path.join(package_dir, "..", data_dir)
     print("full data dir:", cfg['general']['data_dir'])
 
 # add path to file names
 for k, v in cfg['portfolio_names'].items():
     cfg['portfolio_names'][k] = op.join(cfg['general']['data_dir'], v)
-    print(cfg['portfolio_names'][k])
 cfg['portfolio_names']['mock_portfolio_fname'] = './tests/trader_portfolio_simulated.csv'
 cfg['portfolio_names']['mock_alerts_log_fname'] = './tests/trader_logger_simulated.csv'
 
 # Define column names for portfolios and hist messages
 portfolio_cols = ",".join([
                 "Date", "Symbol", "Trader", "isOpen", "BTO-Status", "Asset", "Type", "Price", "Price-Alert", "Price-Current",
                 "uQty", "filledQty", "Avged", "Avged-prices", "exit_plan", "ordID", "Risk", "SL_mental","PnL", "$PnL",
```

### Comparing `DiscordAlertsTrader-0.8/DiscordAlertsTrader/discord_bot.py` & `DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/discord_bot.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 
 import os
 import time
 import pandas as pd
-from datetime import datetime, timezone, date
+from datetime import datetime, timezone
 import threading
-from colorama import Fore, Back, Style, init
+from colorama import Fore, init
 import discord # this is discord.py-self package not discord
 
-from .message_parser import parser_alerts
+from .message_parser import parse_trade_alert
 from .configurator import cfg
 from .configurator import channel_ids
 from .alerts_trader import AlertsTrader
 from .alerts_tracker import AlertsTracker
-
-
+try:
+    from .fend_bot import bot_msgs
+    with_fend = True
+except ImportError:
+    with_fend = False
 
 
 init(autoreset=True)
 
 class dummy_queue():
     def __init__(self, maxsize=10):
         self.maxsize = maxsize
@@ -69,16 +72,17 @@
 
             # get unique symbols  from portfolios
             track_symb = set(self.tracker.portfolio.loc[self.tracker.portfolio['isOpen']==1, 'Symbol'].to_list() + \
                 self.trader.portfolio.loc[self.trader.portfolio['isOpen']==1, 'Symbol'].to_list())
             # save quotes to file
             try:
                 quote = self.bksession.get_quotes(track_symb)
-            except ConnectionError as e:
+            except Exception as e:
                 print('error during live quote:', e)
+                continue
             
             for q in quote: 
                 if quote[q]['description'] == 'Symbol not found':
                     continue
                 timestamp = quote[q]['quoteTimeInLong']//1000  # in ms
                 do_header = not os.path.exists(f"{dir_quotes}/{quote[q]['symbol']}.csv")
                 with open(f"{dir_quotes}/{quote[q]['symbol']}.csv", "a+") as f:
@@ -107,17 +111,22 @@
             self.chn_hist[ch]= ch_dt
 
     async def on_ready(self):
         print('Logged on as', self.user , '\n loading previous messages')
         await self.load_previous_msgs()
 
     async def on_message(self, message):
+        # handle fend bot messages
+        if with_fend:
+            alert = bot_msgs(message)
+            if alert is not None:
+                self.new_msg_acts(alert, False)
+                return
         # only respond to channels in config        
         if message.channel.id not in self.channel_IDS.values():
-            # print('not in cfg', message)
             return
         if message.content == 'ping':
             await message.channel.send('pong')
         if not len(message.content):
             return
         self.new_msg_acts(message)
 
@@ -170,19 +179,20 @@
         else:
             msg = message
         chn = msg['Channel']
         shrt_date = datetime.strptime(msg["Date"], self.time_strf).strftime('%Y-%m-%d %H:%M:%S')
         self.queue_prints.put([f"{shrt_date} \t {msg['Author']}: {msg['Content']} ", "blue"])
         print(Fore.BLUE + f"{shrt_date} \t {msg['Author']}: {msg['Content']} ")
 
-        pars, order =  parser_alerts(msg['Content'])
-        if pars is None and self.chn_hist.get(chn) is not None:
-            msg['Parsed'] = ""
-            self.chn_hist[chn] = pd.concat([self.chn_hist[chn], msg.to_frame().transpose()],axis=0, ignore_index=True)
-            self.chn_hist[chn].to_csv(self.chn_hist_fname[chn], index=False)
+        pars, order =  parse_trade_alert(msg['Content'])
+        if pars is None:
+            if self.chn_hist.get(chn) is not None:
+                msg['Parsed'] = ""
+                self.chn_hist[chn] = pd.concat([self.chn_hist[chn], msg.to_frame().transpose()],axis=0, ignore_index=True)
+                self.chn_hist[chn].to_csv(self.chn_hist_fname[chn], index=False)
             return
         else:
             if order['asset'] == "option":
                 # get option date with year
                 opt_dt = datetime.strptime(f"{order['expDate']} {datetime.now().year}" , "%m/%d %Y")
                 today = datetime.now().date()
                 past = opt_dt.date() < today
```

### Comparing `DiscordAlertsTrader-0.8/DiscordAlertsTrader/gui.py` & `DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/gui.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,37 +7,66 @@
 """
 import os
 import os.path as op
 import threading
 import pandas as pd
 from datetime import datetime
 import time
+import re
 import queue
 import PySimpleGUIQt as sg
 from PySide2.QtWidgets import QHeaderView
 
 from DiscordAlertsTrader.brokerages import get_brokerage
 from DiscordAlertsTrader import gui_generator as gg
 from DiscordAlertsTrader import gui_layouts as gl
 from DiscordAlertsTrader.discord_bot import DiscordBot
 from DiscordAlertsTrader.configurator import cfg, channel_ids
 
+def match_authors(author_str:str)->str:
+    """Author have an identifier in discord, it will try to find full author name
+
+    Parameters
+    ----------
+    author_str : str
+        string to match the author
+
+    Returns
+    -------
+    str
+        author with identifier
+    """
+    if "#" in author_str:
+        return author_str
+    authors = []
+    for chn in channel_ids.keys():
+        at = pd.read_csv(op.join(cfg['general']['data_dir'] , f"{chn}_message_history.csv"))["Author"].unique()
+        authors.extend(at)
+    authors = list(dict.fromkeys(authors))
+    authors = [a for a in authors if author_str.lower() in a.lower()]
+    if len(authors) == 0:
+        author = f"{author_str}#No match, find author identifier#1234"
+    elif len(authors) > 1:
+        author = f"{author_str}#Multiple matches, find author identifier#1234"
+    else:
+        author = authors[0]
+    return author
 
 def fit_table_elms(Widget_element):
     Widget_element.resizeRowsToContents()
     Widget_element.resizeColumnsToContents()
     Widget_element.resizeRowsToContents()
     Widget_element.resizeColumnsToContents()
 
 # sg.theme('Dark Blue 3')
-# sg.SetOptions(font=("Helvitica", "11"),  background_color="whitesmoke")#,,
+sg.SetOptions(font=("Helvitica 10"))
                 # element_padding=(0, 0), margins=(1, 1))
 
-fnt_b = ("Helvitica", "9")
-fnt_h = ("Helvitica", "10")
+fnt_b = "Arial 10"
+fnt_h = "Arial 10"
 
 ly_cons, MLINE_KEY = gl.layout_console()
 
 def mprint(*args, **kwargs):
     window[MLINE_KEY].print(*args, **kwargs)
 
 print(1)
@@ -63,28 +92,28 @@
     ly_ch = gl.layout_chan_msg(chn, gui_data[chn], fnt_b, fnt_h)
     ly_chns.append(ly_ch)
 
 bksession = get_brokerage()
 ly_accnt = gl.layout_account(bksession, fnt_b, fnt_h)
 
 layout = [[sg.TabGroup([
-                        [sg.Tab("Console", ly_cons)],
+                        [sg.Tab("Console", ly_cons, font=fnt_b)],
                         [sg.Tab('Portfolio', ly_port)],
                         [sg.Tab('Analysts portfolio', ly_track)],
                         [sg.Tab('Analysts stats', ly_stats)],
                         [sg.Tab(c, h) for c, h in zip(chns, ly_chns)],                        
                         [sg.Tab("Account", ly_accnt)]
-                        ],title_color='black')],
-          [sg.Input(default_text="Author, STC 1 AAA 05/30 115C @2.5",
-                    size= (140,1.5), key="-subm-msg",
-                    tooltip="User: any, Asset: {stock, option}"),
-           sg.Button("Submit alert", key="-subm-alert", size= (20,1))]
+                        ], title_color='black')],
+          [sg.Input(default_text="Author#1234, STC 1 AAA 115C 05/30 @2.5 [click portfolio row number to prefill]",
+                    size= (110,1.5), key="-subm-msg",
+                    tooltip="Click portfolio row number to prefill the STC alert"),
+           sg.Button("Trigger alert", key="-subm-alert", tooltip="Will generate alert in portfolio and tracker", size= (20,1))]
         ]
 print(3)
-window = sg.Window('BullTrader', layout,size=(800, 400), # force_toplevel=True,
+window = sg.Window('Discord Alerts Trader for BullTrades', layout,size=(100, 800), # force_toplevel=True,
                     auto_size_text=True, resizable=True)
 print(4)
 def mprint_queue(queue_item_list):
     # queue_item_list = [string, text_color, background_color]
     kwargs = {}
     text = queue_item_list[0]
     len_que = len(queue_item_list)
@@ -149,25 +178,42 @@
 print(10)
 dt, _  = gg.get_tracker_data(track_exc, **values)
 window.Element('_track_').Update(values=dt)
 fit_table_elms(window.Element("_track_").Widget)
 dt, hdr = gg.get_portf_data(port_exc)
 window.Element('_portfolio_').Update(values=dt)
 fit_table_elms(window.Element("_portfolio_").Widget)
-dt, hdr = gg.get_portf_data(port_exc)
-window.Element('_portfolio_').Update(values=dt)
-fit_table_elms(window.Element("_portfolio_").Widget)
+dt, hdr = gg.get_stats_data(port_exc)
+window.Element('_stat_').Update(values=dt)
+fit_table_elms(window.Element("_stat_").Widget)
 
 def run_gui():  
     while True:    
         event, values = window.read(1)#.1)
 
         if event == sg.WINDOW_CLOSED:
             break
-
+        if '_portfolio_' in event and values['_portfolio_'] != []:
+            pix = values['_portfolio_'][0]
+            dt, hdr = gg.get_portf_data(port_exc, **values)
+            symb = dt[pix][hdr.index('Symbol')]
+            auth = match_authors(dt[pix][hdr.index('Trader')])
+            qty = dt[pix][hdr.index('filledQty')]
+            price = dt[pix][hdr.index('1-$-Current')]
+            if "_" in symb:
+                # option
+                exp = r"(\w+)_(\d{6})([CP])([\d.]+)"        
+                match = re.search(exp, symb, re.IGNORECASE)
+                if match:
+                    symbol, date, type, strike = match.groups()
+                    symb_str = f"{auth}, STC {qty} {symbol} {strike}{type} {date[:2]}/{date[2:4]} @{price}"
+            else:
+                symb_str= f"{auth}, STC {qty} {symb} @{price}"
+            window.Element("-subm-msg").Update(value=symb_str)
+            
         if event == "_upd-portfolio_": # update button in portfolio
             ori_col = window.Element("_upd-portfolio_").ButtonColor
             window.Element("_upd-portfolio_").Update(button_color=("black", "white"))
             event, values = window.read(.1)
             dt, _ = gg.get_portf_data(port_exc, **values)
             window.Element('_portfolio_').Update(values=dt)
             fit_table_elms(window.Element("_portfolio_").Widget)
@@ -187,30 +233,30 @@
             window.Element("_upd-stat_").Update(button_color=("black", "white"))
             event, values = window.read(.1)
             dt, _  = gg.get_stats_data(stat_exc, **values)
             window.Element('_stat_').Update(values=dt)
             fit_table_elms(window.Element("_stat_").Widget)
             window.Element("_upd-stat_").Update(button_color=ori_col)
 
-        elif event[:6] == "-port-":
-            key =  event[6:]
+        elif event.startswith("-port-"): # radial click, update portfolio
+            key =  event.replace("-port-", "")
             state = window.Element(event).get()
             port_exc[key] = state
             dt, _ = gg.get_portf_data(port_exc, **values)
             window.Element('_portfolio_').Update(values=dt)
 
-        elif event[:7] == "-track-":
-            key =  event[7:]
+        elif event.startswith("-track-"): # radial click, update analyst alerts
+            key =  event.replace("-track-", "")
             state = window.Element(event).get()
             track_exc[key] = state
             dt, _ = gg.get_tracker_data(track_exc, **values)
             window.Element('_track_').Update(values=dt)
 
-        elif event[:7] == "-stat-":
-            key =  event[7:]
+        elif event.startswith("-stat-"): # radial click, update analyst stats
+            key =  event.replace("-stat-", "")
             state = window.Element(event).get()
             stat_exc[key] = state
             dt, _ = gg.get_stats_data(stat_exc, **values)
             window.Element('_stat_').Update(values=dt)
 
         elif event[-3:] == "UPD":
             chn = event[:-4]
@@ -246,15 +292,15 @@
             ori_col = window.Element("-subm-alert").ButtonColor
             window.Element("-subm-alert").Update(button_color=("black", "white"))
             event, values = window.read(.1)
             try:        
                 author, msg = values['-subm-msg'].split(',')
             except ValueError:
                 author, msg = values['-subm-msg'].split(':')
-            author = author.strip()
+            author = match_authors(author.strip())
             msg = msg.strip()
             date = datetime.now().strftime("%Y-%m-%d %H:%M:%S.%f")
             new_msg = pd.Series({
                 'AuthorID': None,
                 'Author': author,
                 'Date': date, 
                 'Content': msg,
@@ -281,13 +327,12 @@
     # start the threads
     client_thread.start()
     run_gui()
 
     # close the GUI window
     window.close()
     alistner.close_bot()
-    # alistner.close()
     exit()
 
 
 if __name__ == '__main__':
     gui()
```

### Comparing `DiscordAlertsTrader-0.8/DiscordAlertsTrader/gui_generator.py` & `DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/gui_generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     plan = "PT:" + ",".join(PT) if PT else ""
     sl_str = ", SL:" if plan else "SL:"
     plan = plan + sl_str + str(SL) if SL else plan
 
     return plan
 
 def get_portf_data(exclude={}, port_filt_author='', port_filt_date_frm='',
-                     port_filt_date_to='', port_filt_sym='', **kwargs ):
+                     port_filt_date_to='', port_filt_chn='', **kwargs ):
     fname_port = cfg['portfolio_names']['portfolio_fname']
     if not op.exists(fname_port):
         return [],[]
     try:
         data = pd.read_csv(fname_port,sep=",")
     except:
         data = pd.read_csv(fname_port,sep=",")
@@ -89,17 +89,20 @@
         data[f'STC{i}-PnL'] = pd_col_str_frmt(data[f'STC{i}-PnL'])
         data[f'STC{i}-uQty'] = pd_col_str_frmt(data[f'STC{i}-uQty'])
 
     frm_cols = ['Price', 'Price-Alert', "Price-Current", 'uQty', 'filledQty', 'N Alerts', 
                 "PnL", "$PnL","PnL-Alert", "$PnL-Alert","PnL-Current","$PnL-Current"]
     for cfrm in frm_cols:
         data[cfrm] = pd_col_str_frmt(data[cfrm])
-
-    data = filter_data(data,exclude, port_filt_author, port_filt_date_frm,
-                        port_filt_date_to, port_filt_sym)
+    
+    try:
+        data = filter_data(data,exclude, port_filt_author, port_filt_date_frm,
+                        port_filt_date_to, port_filt_chn)
+    except:
+        pass
     cols = ['isOpen', "PnL", "$PnL", 'Date', 'Symbol', 'Trader', 'BTO-Status', 'Price',
             'Price-Alert', "Price-Current", 'uQty', 'filledQty', 'N Alerts',"PnL-Alert",
             "$PnL-Alert","PnL-Current","$PnL-Current", "STC1-Price", "STC1-Price-Alerted",
             "STC1-Price-Current", 'STC1-PnL', 'STC1-Status','STC1-uQty','STC2-PnL',
             'STC2-Status', 'STC2-uQty', 'STC3-PnL', 'STC3-Status',  'STC3-uQty'
             ]
     data = data[cols]
@@ -118,15 +121,16 @@
         sumtotal['Trader'] = "Average"
         data = pd.concat([data, pd.DataFrame.from_records(sumtotal, index=[0])], ignore_index=True)
     
     data = data.values.tolist()
     return data, header_list
 
 def get_tracker_data(exclude={}, track_filt_author='', track_filt_date_frm='',
-                     track_filt_date_to='', track_filt_sym='', **kwargs ):
+                     track_filt_date_to='', track_filt_sym='', track_exc_author='',
+                     track_exc_chn='',**kwargs ):
     fname_port = cfg['portfolio_names']['tracker_portfolio_name']
     if not op.exists(fname_port):
         return [],[]
     
     data = pd.read_csv(fname_port, sep=",")
 
     data['Date'] = data['Date'].apply(lambda x: short_date(x))
@@ -138,17 +142,19 @@
         data =  get_live_quotes(data)
     
     frm_cols = ['Amount', 'N Alerts', 'STC-Amount','STC-Price','STC-Price-current','STC-PnL','STC-PnL-current',
                 'STC-PnL$','STC-PnL$-current', 'Price', 'Price-current']
     for cfrm in frm_cols:
         data[cfrm] = pd_col_str_frmt(data[cfrm])
     
-    data = filter_data(data,exclude, track_filt_author, track_filt_date_frm,
-                        track_filt_date_to, track_filt_sym )
-
+    try:
+        data = filter_data(data,exclude, track_filt_author, track_filt_date_frm,
+                        track_filt_date_to, track_filt_sym, track_exc_author, track_exc_chn)
+    except:
+        pass
     cols = ['isOpen','STC-PnL','STC-PnL-current', 'STC-PnL$','STC-PnL$-current', 'Date', 'Symbol', 'Trader', 'Price',
             "Price-current", 'Amount', 'N Alerts','STC-Amount','STC-Price','STC-Price-current','STC-Date','Channel'
             ]
     # data['Trader'] = data['Trader'].apply(lambda x: x.split('(')[0].split('#')[0])
     data = data[cols]
     data.fillna("", inplace=True)
     header_list = data.columns.tolist()
@@ -167,51 +173,57 @@
     data = data.values.tolist()
     return data, header_list
 
 
 def get_stats_data(exclude={}, stat_filt_author='', stat_filt_date_frm='',
                      stat_filt_date_to='', stat_filt_sym='', 
                      stat_max_trade_cap='', stat_max_qty='', trail_stop_perc='',
+                     stat_exc_author='', stat_exc_chn='', stat_exc_sym='',
+                     fname_port=None,
                      **kwargs ):
-    fname_port = cfg['portfolio_names']['tracker_portfolio_name']
+    if fname_port is None:
+        fname_port = cfg['portfolio_names']['tracker_portfolio_name']
     if not op.exists(fname_port):
         return [],[]
     
     data = pd.read_csv(fname_port, sep=",")
 
     data['Date'] = data['Date'].apply(lambda x: datetime.strptime(x, "%Y-%m-%d %H:%M:%S.%f").strftime("%m/%d/%Y"))
     data["isOpen"] = data["isOpen"].map({1:"Yes", 0:"No"})
     data["N Alerts"]= data['Avged']
     data['Trader'] = data['Trader'].apply(lambda x: x.split('(')[0].split('#')[0])
-
-    data = filter_data(data,exclude, stat_filt_author, stat_filt_date_frm,
-                        stat_filt_date_to, stat_filt_sym )
-
+    try:
+        data = filter_data(data,exclude, stat_filt_author, stat_filt_date_frm,
+                        stat_filt_date_to, stat_filt_sym, stat_exc_author, stat_exc_chn, stat_exc_sym)
+    except:
+        pass
     if stat_max_qty != "" or stat_max_trade_cap != "":
-        if stat_max_qty != "":
+        if stat_max_qty != "" and stat_max_qty.isnumeric():
             stat_max_qty = int(stat_max_qty)
             print("stat_max_qty:", stat_max_qty)
             option_mult = (data['Asset'] == 'option').astype(int)
             option_mult[option_mult==1] = 100
             exceeds_cap = data['Amount'] > stat_max_qty
             data.loc[exceeds_cap, 'Amount'] = stat_max_qty
 
-        if stat_max_trade_cap != "":
+        if stat_max_trade_cap != "" and stat_max_trade_cap.isnumeric():
             stat_max_trade_cap = int(stat_max_trade_cap)
             print("stat_max_trade_cap:", stat_max_trade_cap)
             option_mult = (data['Asset'] == 'option').astype(int)
             option_mult[option_mult==1] = 100
             trade_value = data['Amount'] * data['Price'] * option_mult
             exceeds_cap = trade_value > stat_max_trade_cap
             data.loc[exceeds_cap, 'Amount'] = np.floor(stat_max_trade_cap / (data['Price'] * option_mult))
             data = data[data['Amount'] * data['Price'] * option_mult <= stat_max_trade_cap]
         mult =(data['Asset'] == 'option').astype(int) 
         mult[mult==0] = .01  # pnl already in %
         data['STC-PnL$'] = data['Amount'] * data['STC-PnL'] * data['Price'] * mult
-        data['STC-PnL$-current'] = data['Amount'] * data['STC-PnL'] * data['Price-current'] * mult
+        data['STC-PnL$-current'] = data['Amount'] * data['STC-PnL-current'] * data['Price-current'] * mult
+        data['STC-PnL$'] = data['STC-PnL$'].round()
+        data['STC-PnL$-current'] = data['STC-PnL$-current'].round()
 
     data['PnL diff'] = data['STC-PnL-current'] - data['STC-PnL']
     # Define the aggregation functions for each column
     agg_funcs = {'STC-PnL$': 'sum',
                  'STC-PnL$-current': 'sum',
                  'STC-PnL': 'mean',
                  'STC-PnL-current': 'mean',
@@ -236,30 +248,30 @@
     result_td = pd.concat([result_td, agg_values_all, result_ch],axis=0, ignore_index=True)
     result_td.drop('all', axis=1, level=0, inplace=True)
     new_cols =[k for k in result_td.columns.get_level_values(0)]
     new_cols[-3] = "N Trades"
     new_cols[-2] = "Since"
     new_cols[-1] = "Last"
     result_td.columns = new_cols
-    result_td = result_td.round(2)
+    result_td = result_td.round(1)
 
     for cfrm in result_td.columns[1:-2]:
         result_td[cfrm] = pd_col_str_frmt(result_td[cfrm])
     result_td = result_td.fillna("")
     header_list = result_td.columns.tolist()
     header_list = [d.replace('STC-', '') for d in header_list]
     data = result_td.values.tolist()
     return data, header_list
 
 
 def filter_data(data,exclude={}, track_filt_author='', track_filt_date_frm='',
-                track_filt_date_to='', track_filt_sym=''):
+                track_filt_date_to='', track_filt_sym='', track_exc_author='', track_exc_chn='', stat_exc_sym=''):
     if len(exclude):
         for k, v in exclude.items():
-            if k == "Cancelled" and v:
+            if k == "Cancelled" and v and k in data.columns:
                 data = data[data["BTO-Status"] !="CANCELED"]
             elif k == "Closed" and v:
                 data = data[data["isOpen"] !="No"]
             elif k == "Open" and v:
                 data = data[data["isOpen"] !="Yes"]
             elif k == "NegPnL" and v:
                 col = "PnL" if "PnL" in data else 'STC-PnL'                
@@ -271,21 +283,32 @@
                 data = data[pnl < 0 ]
             elif k == "stocks" and v:
                 data = data[data["Asset"] !="stock"]
             elif k == "options" and v:
                 data = data[data["Asset"] !="option"]
 
     if track_filt_author:
-        data = data[data['Trader'].str.contains(track_filt_author, case=False)]
+        msk = [x.strip() for x in track_filt_author.split(",")]
+        data = data[data['Trader'].str.contains('|'.join(msk), case=False)]
     if track_filt_date_frm:
         data = data[data['Date'] >= track_filt_date_frm]
     if track_filt_date_to:
         data = data[data['Date'] <= track_filt_date_to]
     if track_filt_sym:
-        data = data[data['Symbol'].str.contains(track_filt_sym, case=False)]
+        msk = [x.strip() for x in track_filt_sym.split(",")]
+        data = data[data['Symbol'].str.contains('|'.join(msk), case=False)]
+    if track_exc_author:
+        msk = [x.strip() for x in track_exc_author.split(",")]
+        data = data[~data['Trader'].str.contains('|'.join(msk), case=False)]
+    if track_exc_chn:
+        msk = [x.strip() for x in track_exc_chn.split(",")]
+        data = data[~data['Channel'].str.contains('|'.join(msk), case=False)]
+    if stat_exc_sym:
+        msk = [x.strip() for x in stat_exc_sym.split(",")]
+        data = data[~data['Symbol'].str.contains('|'.join(msk), case=False)]
     return data
 
 def get_live_quotes(portfolio):
     dir_quotes = cfg['general']['data_dir'] + '/live_quotes'
     track_symb = portfolio.loc[portfolio['isOpen']=='Yes', 'Symbol'].to_list()
     
     quotes_sym = {}
@@ -348,22 +371,22 @@
 
 def get_acc_bals(bksession):
     acc_inf = bksession.get_account_info()
     # if grabing new access token return None, try again
     if acc_inf is None:  
         acc_inf = bksession.get_account_info()
     accnt= {"id" : acc_inf['securitiesAccount']['accountId'],
-        "balance": acc_inf['securitiesAccount']['currentBalances']['liquidationValue'],
-        "cash": acc_inf['securitiesAccount']['currentBalances']['cashBalance'],
-        "funds": acc_inf['securitiesAccount']['currentBalances']['availableFunds'],
+        "balance": acc_inf['securitiesAccount']['currentBalances'].get('liquidationValue', 0),
+        "cash": acc_inf['securitiesAccount']['currentBalances'].get('cashBalance',0),
+        "funds": acc_inf['securitiesAccount']['currentBalances'].get('availableFunds', 0),
         }
     return acc_inf, accnt
 
 def get_pos(acc_inf):
-    positions = acc_inf['securitiesAccount']['positions']
+    positions = acc_inf['securitiesAccount'].get('positions', [])
     pos_tab = []
     pos_headings = ["Sym", "Last", "price", "PnL_%", "PnL","Qty", "Val", "Cost"]
     for pos in positions:
         price= round(pos['averagePrice'], 2)
         # pnl = pos['currentDayProfitLoss']
         pnl_p = pos['currentDayProfitLossPercentage'] * 100
         uQty = pos['longQuantity']
@@ -425,15 +448,17 @@
         sing_ord_c.insert(0, leg['instrument']['symbol'])
         sing_ord_c.insert(1, leg["instruction"].replace('BUY_TO_OPEN', "BUY").replace('SELL_TO_CLOSE', "SELL"))
         ord_list.append(sing_ord_c)
 
     return ord_list, ord_headings
 
 def get_orders(acc_inf):
-    orders =acc_inf['securitiesAccount']['orderStrategies']
+    orders =acc_inf['securitiesAccount'].get('orderStrategies', [])
+    if len(orders) == 0:
+        return ["NoOrders"],  ["Sym", "Act", "Strat", "Price/stp","Date", "Qty/fill", "Status", "ordId"], []
     ord_tab, cols = [], []
     col = 0
     for ordr in orders:
         col = not col
         ord_type = ordr['orderStrategyType']
         if ord_type == "OCO":
             for chl in ordr['childOrderStrategies']:
```

### Comparing `DiscordAlertsTrader-0.8/DiscordAlertsTrader/gui_layouts.py` & `DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/gui_layouts.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,124 +6,136 @@
 @author: adonay
 """
 
 import PySimpleGUIQt as sg
 from . import gui_generator as gg
 
 
+tip = "coma separed patterns, e.g. string1,string2"
 
 def layout_console():
     MLINE_KEY = '-MLINE-__WRITE ONLY__'
     layout = [[sg.Text('Real Time Discord Alert Trader', size=(50,1))],
-              [sg.Multiline(size=(1500,800), key=MLINE_KEY)]]
-     # [sg.Column([[sg.Multiline(key=MLINE_KEY),sg.Stretch()]])]]
+              [sg.Multiline(size=(1200,None), key=MLINE_KEY, autoscroll=True, enable_events=False),sg.Stretch()]]
     return layout, MLINE_KEY
 
 
 def layout_portfolio(data_n_headers, font_body, font_header):
-    
     if data_n_headers[0] == []: 
         values = [""*21 ]
     else:
         values=data_n_headers[0]
     
     layout = [
-         [sg.Column([[sg.Text('Filter:  Author: ', size=(20, 1)), sg.Input(key=f'port_filt_author', size=(20, 1)),
-                      sg.Text('Date from: ', size=(15, 1)), sg.Input(key=f'port_filt_date_frm', size=(18, 1), default_text='05/10/2023'),
-                      sg.Text(' To: ', size=(5, 1)), sg.Input(key=f'port_filt_date_to', size=(15, 1)),
-                      sg.Text('   Contains symbol: ', size=(20, 1)), sg.Input(key=f'port_filt_sym', size=(20, 1)),
-                      ],
-                     [sg.Text("Exclude: "),
-                      sg.Checkbox("Closed", key="-port-Closed", enable_events=True),
-                      sg.Checkbox("Open", key="-port-Open", enable_events=True),
-                      sg.Checkbox("Cancelled", key="-port-Cancelled", default=True, enable_events=True),
-                      sg.Checkbox("Neg PnL", key="-port-NegPnL", enable_events=True),
-                      sg.Checkbox("Pos PnL", key="-port-PosPnL", enable_events=True),
-                      sg.Checkbox("Live PnL", key="-port-live PnL", enable_events=True),
-                      sg.Checkbox("Stocks", key="-port-stocks", default=True, enable_events=True),
-                      sg.Checkbox("Options", key="-port-options", enable_events=True),
-                      ],
-             [sg.ReadButton("Update", button_color=('white', 'black'), key="_upd-portfolio_")]])],
+         [sg.Column([[
+            sg.Text('Include:  Authors: ', auto_size_text=True,tooltip=tip), sg.Input(key=f'port_filt_author',tooltip=tip),
+            sg.Text('Date from: '), sg.Input(key=f'port_filt_date_frm', size=(16, 1), default_text='05/10/2023'),
+            sg.Text(' To: '), sg.Input(key=f'port_filt_date_to', size=(16, 1)),
+            sg.Text(' Symbols: ', tooltip=tip), sg.Input(key=f'port_filt_sym', tooltip=tip),
+            sg.Text(' Channels: ',tooltip=tip), sg.Input(key=f'port_filt_chn',tooltip=tip)
+            ],                                        
+            [sg.Text("Exclude: |"),
+            sg.Checkbox("Closed", key="-port-Closed", enable_events=True),
+            sg.Checkbox("Open", key="-port-Open", enable_events=True),
+            sg.Checkbox("Cancelled", key="-port-Cancelled", default=True, enable_events=True),
+            sg.Checkbox("Neg PnL", key="-port-NegPnL", enable_events=True),
+            sg.Checkbox("Pos PnL", key="-port-PosPnL", enable_events=True),
+            sg.Checkbox("Live PnL", key="-port-live PnL", enable_events=True),
+            sg.Checkbox("Stocks", key="-port-stocks", default=True, enable_events=True),
+            sg.Checkbox("Options", key="-port-options", enable_events=True),
+            sg.Text('| Authors: ', auto_size_text=True,tooltip=tip), sg.Input(key=f'port_exc_author', tooltip=tip),
+            sg.Text('Channels: ', auto_size_text=True,tooltip=tip), sg.Input(key=f'port_exc_chn',tooltip=tip),
+            ],
+            [sg.ReadButton("Update", button_color=('white', 'black'), key="_upd-portfolio_")]])],
          [sg.Column([[sg.Table(values=values,
                         headings=data_n_headers[1],
                         display_row_numbers=True,
                         auto_size_columns=True,
                         header_font=font_header,
                         text_color='black',
                         font=font_body,
                         justification='left',
                         alternating_row_color='grey',
                         # num_rows=30, #len(data_n_headers[0]),
+                        enable_events=True,
                         key='_portfolio_'), sg.Stretch()]])]
          ]
     return layout
 
 
 def layout_traders(data_n_headers, font_body, font_header):
     
     if data_n_headers[0] == []: 
         values = [""*21 ]
     else:
         values=data_n_headers[0]
     
-    layout = [
-        [sg.Column([[sg.Text('Filter:  Author: ', size=(20, 1)), sg.Input(key=f'track_filt_author', size=(20, 1)),
-                     sg.Text('Date from: ', size=(15, 1)), sg.Input(key=f'track_filt_date_frm', size=(18, 1), default_text='05/10/2023'),
-                     sg.Text(' To: ', size=(5, 1)), sg.Input(key=f'track_filt_date_to', size=(18, 1)),
-                     sg.Text('   Contains symbol: ', size=(20, 1)), sg.Input(key=f'track_filt_sym', size=(20, 1)),
-                     ],
-                     [sg.Text("Exclude: "),
-                      sg.Checkbox("Closed", key="-track-Closed", enable_events=True),
-                      sg.Checkbox("Open", key="-track-Open", enable_events=True),
-                      sg.Checkbox("Neg PnL", key="-track-NegPnL", enable_events=True),
-                      sg.Checkbox("Pos PnL", key="-track-PosPnL", enable_events=True),
-                      sg.Checkbox("Live PnL", key="-track-live PnL", enable_events=True),                   
-                      sg.Checkbox("Stocks", key="-track-stocks", default=True, enable_events=True),
-                      sg.Checkbox("Options", key="-track-options", enable_events=True)
-                      ],
-                     [sg.ReadButton("Update", button_color=('white', 'black'), key="_upd-track_")]])
-                    ],
-         [sg.Column([[sg.Table(values=values,
-                        headings=data_n_headers[1],
-                        display_row_numbers=True,
-                        auto_size_columns=True,
-                        header_font=font_header,
-                        text_color='black',
-                        font=font_body,
-                        justification='left',
-                        alternating_row_color='grey',
-                        # num_rows=30, #len(data_n_headers[0]),
-                        key='_track_'), sg.Stretch()]])]
+    layout = [[
+        sg.Column([
+            [
+            sg.Text('Include:  Authors: ', auto_size_text=True,tooltip=tip), sg.Input(key=f'track_filt_author',tooltip=tip),
+            sg.Text('Date from: '), sg.Input(key=f'track_filt_date_frm', default_text='05/10/2023', size=(16, 1)),
+            sg.Text(' To: '), sg.Input(key=f'track_filt_date_to', size=(16, 1)),
+            sg.Text(' Symbols: ',tooltip=tip), sg.Input(key=f'track_filt_sym',tooltip=tip),
+            sg.Text(' Channels: ',tooltip=tip), sg.Input(key=f'track_filt_chn',tooltip=tip)
+            ],[ 
+            sg.Text("Exclude: |"),
+            sg.Checkbox("Closed", key="-track-Closed", enable_events=True),
+            sg.Checkbox("Open", key="-track-Open", enable_events=True),
+            sg.Checkbox("Neg PnL", key="-track-NegPnL", enable_events=True),
+            sg.Checkbox("Pos PnL", key="-track-PosPnL", enable_events=True),
+            sg.Checkbox("Live PnL", key="-track-live PnL", enable_events=True), 
+            sg.Checkbox("Stocks", key="-track-stocks", default=True, enable_events=True),
+            sg.Checkbox("Options", key="-track-options", enable_events=True),
+            sg.Text('| Authors: ', auto_size_text=True,tooltip=tip), sg.Input(key=f'track_exc_author', tooltip=tip),
+            sg.Text('Channels: ', auto_size_text=True,tooltip=tip), sg.Input(key=f'track_exc_chn',tooltip=tip),
+            ],[sg.ReadButton("Update", button_color=('white', 'black'), key="_upd-track_")]
+            ])],
+         [sg.Column([
+            [
+            sg.Table(values=values,
+                headings=data_n_headers[1],
+                display_row_numbers=True,
+                auto_size_columns=True,
+                header_font=font_header,
+                text_color='black',
+                font=font_body,
+                justification='left',
+                alternating_row_color='grey',
+                # num_rows=30, #len(data_n_headers[0]),
+                key='_track_'), sg.Stretch()]])]
          ]
     return layout
 
 
 def layout_stats(data_n_headers, font_body, font_header):
     
     if data_n_headers[0] == []: 
         values = [""*21 ]
     else:
         values=data_n_headers[0]
     
     layout = [
-        [sg.Column([[sg.Text('Filter:  Author: ', size=(20, 1)), sg.Input(key=f'stat_filt_author', size=(20, 1)),
-                     sg.Text('Date from: ', size=(15, 1)), sg.Input(key=f'stat_filt_date_frm', size=(18, 1), default_text='05/10/2023'),
-                     sg.Text(' To: ', size=(5, 1)), sg.Input(key=f'stat_filt_date_to', size=(18, 1)),
-                     sg.Text('  Contains symbol: ', size=(20, 1)), sg.Input(key=f'stat_filt_sym', size=(20, 1)),
-                     sg.Text(' Max $: ', size=(10, 1)), sg.Input(key=f'stat_max_trade_cap', size=(10, 1)),
-                     sg.Text(' Max quantity: ', size=(10, 1)), sg.Input(key=f'stat_max_qty', size=(10, 1)),
+        [sg.Column([[sg.Text('Include:  Authors: ', auto_size_text=True, tooltip=tip), sg.Input(key=f'stat_filt_author', tooltip=tip),
+                     sg.Text('Date from:'), sg.Input(key=f'stat_filt_date_frm', size=(16, 1), default_text='05/10/2023'),
+                     sg.Text(' To:', size=(5, 1)), sg.Input(key=f'stat_filt_date_to', size=(16, 1)),
+                     sg.Text(' Symbols:'), sg.Input(key=f'stat_filt_sym', tooltip=tip),
+                     sg.Text(' Max $:', tooltip="calculate stats limiting trades to max $"), 
+                     sg.Input(key=f'stat_max_trade_cap', tooltip="calculate stats limiting trades to max $"),
+                     sg.Text(' Max quantity:', tooltip="calculate stats limiting trades to max quantity"), 
+                     sg.Input(key=f'stat_max_qty', tooltip="calculate stats limiting trades to max quantity"),
                      ],
                      [sg.Text("Exclude: "),
-                      sg.Checkbox("Closed", key="-stat-Closed", enable_events=True),
-                      sg.Checkbox("Open", key="-stat-Open", enable_events=True),
                       sg.Checkbox("Neg PnL", key="-stat-NegPnL", enable_events=True),
-                      sg.Checkbox("Pos PnL", key="-stat-PosPnL", enable_events=True),
-                      sg.Checkbox("Live PnL", key="-stat-live PnL", enable_events=True),                   
+                      sg.Checkbox("Pos PnL", key="-stat-PosPnL", enable_events=True),                  
                       sg.Checkbox("Stocks", key="-stat-stocks", default=True, enable_events=True),
-                      sg.Checkbox("Options", key="-stat-options", enable_events=True)
+                      sg.Checkbox("Options", key="-stat-options", enable_events=True),
+                      sg.Text('| Authors: ', auto_size_text=True,tooltip=tip), sg.Input(key=f'stat_exc_author', tooltip=tip),
+                      sg.Text('Symbols: ', auto_size_text=True,tooltip=tip), sg.Input(key=f'stat_exc_sym',tooltip=tip),
+                      sg.Text('Channels: ', auto_size_text=True,tooltip=tip), sg.Input(key=f'stat_exc_chn',tooltip=tip),
                       ],
                      [sg.ReadButton("Update", button_color=('white', 'black'), key="_upd-stat_")]])
                     ],
          [sg.Column([[sg.Table(values=values,
                         headings=data_n_headers[1],
                         display_row_numbers=True,
                         auto_size_columns=True,
@@ -141,41 +153,41 @@
     # Handle empy chan history
     if data_n_headers[0] == []: 
         values = [[""*len(data_n_headers[1])] ]
     else:
         values=data_n_headers[0]
 
     layout = [
-        [sg.Text('Filter:  Author: ', size=(20, 1)), sg.Input(key=f'{chn}_filt_author', size=(20, 1)),
+        [sg.Text('Filter:  Authors: '), sg.Input(key=f'{chn}_filt_author'),
            # sg.Text(' '*2),
-         sg.Text('Date from: ', size=(15, 1)), sg.Input(key=f'{chn}_filt_date_frm', size=(10, 1), default_text='05/09'),
-         sg.Text(' To: ', size=(5, 1)), sg.Input(key=f'{chn}_filt_date_to', size=(10, 1)),
+         sg.Text('Date from: '), sg.Input(key=f'{chn}_filt_date_frm', default_text='05/09/23'),
+         sg.Text(' To: '), sg.Input(key=f'{chn}_filt_date_to'),
           # sg.Text(' '*1),
-         sg.Text('Message contains: ', size=(25, 1)), sg.Input(key=f'{chn}_filt_cont', size=(20, 1)),
-         sg.Text('Num. rows display: '), sg.Input(key=f'{chn}_n_rows', size=(5, 1)),
+         sg.Text('Message contains: '), sg.Input(key=f'{chn}_filt_cont'),
+         sg.Text('Num. rows display: '), sg.Input(key=f'{chn}_n_rows'),
          ],
         [sg.ReadFormButton("Update", button_color=('white', 'black'), key=f'{chn}_UPD', bind_return_key=True)],
         [sg.Column([[sg.Table(values=values,
                   headings=data_n_headers[1],
                   justification='left',
                   display_row_numbers=False,
                   text_color='black',
                   font=font_body,
                   # col_widths=[30,200, 300],
                   header_font=font_header,
-                  auto_size_columns =True, max_col_width=50,
+                  auto_size_columns =True, max_col_width=30,
                   # auto_size_columns=True,
                   # vertical_scroll_only=False,
                    alternating_row_color='grey',
                   # col_widths=[30,300, 1300],
                   # row_height=20,
                   # num_rows=30,
                   # enable_events = False,
                   # bind_return_key = True,
-                  tooltip = "Selecting row and pressing enter will parse message",
+                #   tooltip = "Selecting row and pressing enter will parse message",
                   key=f"{chn}_table")]])]
         ]
     return layout
 
 
 def tt_acnt(text, fsize=12, bold=True, underline=True, font_name="Arial", size=None, k=None):
     font = [font_name, fsize]
```

### Comparing `DiscordAlertsTrader-0.8/DiscordAlertsTrader/message_parser.py` & `DiscordAlertsTrader-0.9.1/DiscordAlertsTrader/message_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 import re
 import pandas as pd
 from datetime import datetime
 import numpy as np
 
 def parse_trade_alert(msg, asset=None):
-    pattern = r'\b(BTO|STC)\b\s*(\d+)?\s*([A-Z]+)\s*(\d+[cp]?)?\s*(\d{1,2}\/\d{1,2})?\s*@\s*[$]*[ ]*(\d+(?:[,.]\d+)?|\.\d+)'
+    pattern = r'\b(BTO|STC)\b\s*(\d+)?\s*([A-Z]+)\s*(\d+[.\d+]*[cp]?)?\s*(\d{1,2}\/\d{1,2})?(?:\/2023|\/23)?\s*@\s*[$]*[ ]*(\d+(?:[,.]\d+)?|\.\d+)'
     match = re.search(pattern, msg, re.IGNORECASE)
     
     if match:
         action, quantity, ticker, strike, expDate, price = match.groups()
 
         asset_type = 'option' if strike and expDate else 'stock'
         symbol =  ticker.upper()
@@ -32,30 +32,55 @@
             if "c" not in strike.lower() and "p" not in strike.lower():
                 strike = strike + "c"
                 order['strike'] = strike.upper()
                 str_ext = " No direction found in option strike, assuming Call"
 
             order['strike'] = strike.upper()
             order['expDate'] = expDate
-            symbol = fix_index_symbols(symbol)            
+            order['Symbol'] = fix_index_symbols(symbol)            
             order['Symbol'] = make_optionID(**order)
 
         risk_level = parse_risk(msg)
         order['risk'] = risk_level
-        []
-        pars =  " ".join(match.groups()) + f" {risk_level}{str_ext}"
-        pars = pars.replace("None", "")
-        return order, pars
+
+        pars = []
+        for el in [action, quantity, ticker, strike, expDate, price, risk_level, str_ext]:
+            if el is not None:
+                pars.append(el)
+        pars = " ".join(pars)
+        if action.upper() == "BTO":
+            if "avg" in msg.lower() or "average" in msg.lower():
+                avg_price, _ = parse_avg(msg)
+                pars = pars + f"AVG to {avg_price} "
+                order["avg"] = avg_price
+            else:
+                order["avg"] = None
+            pt1_v, pt2_v, pt3_v, sl_v = parse_exits(msg)
+            n_pts = 3 if pt3_v else 2 if pt2_v else 1 if pt1_v else 0
+            pts_qty = set_pt_qts(n_pts)
+            order, pars = make_order_exits(order, msg, pars, asset_type)
+            sl_mental = True if "mental" in msg.lower() else False
+            if sl_mental: order["SL_mental"] = True
+            order["n_PTs"] = n_pts
+            order["PTs_Qty"] = pts_qty
+
+        elif action.upper() == "STC":
+            xamnt = parse_sell_ratio_amount(msg, asset_type)
+            if order["uQty"] is None:
+                pars = pars + f" xamount: {xamnt}"
+            order["xQty"] = xamnt
+        
+        return pars, order
     else:
-        return None
+        return None, None
 
 def fix_index_symbols(symbol):
-    if symbol == "SPX": 
+    if symbol.upper() == "SPX": 
         symbol = "SPXW"
-    elif symbol == "NDX":
+    elif symbol.upper() == "NDX":
         symbol = "NDXP"
     return symbol
     
 
 def parser_alerts(msg, asset=None):
     msg = msg.replace("STc", "STC").replace("StC", "STC").replace("stC", "STC").replace("STc", "STC")
     msg = msg.replace("BtO", "BTO").replace("btO", "BTO").replace("bTO", "BTO").replace("BTo", "BTO")
```

### Comparing `DiscordAlertsTrader-0.8/DiscordAlertsTrader.egg-info/PKG-INFO` & `DiscordAlertsTrader-0.9.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: DiscordAlertsTrader
-Version: 0.8
-Summary: Package for automating discord stock and option alerts.
-Home-page: 
-Download-URL: https://github.com/AdoNunes/DiscordAlertsTrader
-Author: Adonay Nunes
-Author-email: Adonay Nunes <adonay.s.nunes@example.com>
-License: BSD (3-clause)
-Project-URL: Homepage, https://github.com/AdoNunes/DiscordAlertsTrader
-Project-URL: Bug Tracker, https://github.com/AdoNunes/DiscordAlertsTrader/issues
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Communications :: Chat
-Classifier: Topic :: Office/Business :: Financial
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Financial and Insurance Industry
-Classifier: Intended Audience :: Information Technology
-Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # DiscordAlertsTrader: *Discord Alerts Trader Bot*
 ________________________
 
 DiscordAlertsTrader is a python package to get messages from a subscribed discord channel where buy
  and sell stock and options signals are messaged. The package will parse the messages and execute
  the trades for traders specified in the config file. It will track the messages from all channels,
  the analysts portfolio and the bot portfolio.
@@ -42,15 +18,15 @@
 - Read messages and parse trading singals, e.g. BTO (Buy to Open), STC (Sell to Close), partial STC, SL (Stop Limits), PT (Profit Taking)
 - Track trading signals and performance of traders using message history and realtime price
 - Execute and cancel orders, check order status, account status and current ticker prices
 - If in config.ini auto_trade = False, trades are executed manually through promts and optionally choose QTY, price, etc
 
 **Currently, the package is for parsing signals of the discord server BullTrades.** 
 
-Invite link to BullTrades: https://discord.gg/bulltrades
+Invite link to BullTrades with referral: [https://discord.gg/bulltrades](https://bulltrades.net/?ref=ndrjogi)
 
 <img src="media/GUI_analysts_portfolio.PNG" alt="Analysts Portfolio" width="500" height="300">
 <img src="media/GUI_messages.PNG" alt="Channel message history" width="500" height="300">
 (older version shots)
 <img src="media/xtrader_console.png" alt="Console with discord mesages" width="500" height="300">
 <img src="media/xtrader_portfolio.png" alt="Portfolio" width="500" height="300">
 
@@ -119,14 +95,25 @@
 
 Make sure to keep the terminal or command prompt window open while the application is running to see any output or errors.
 
 **Closing the Application**
 
 To stop the DiscordAlertsTrader application, simply close the terminal or command prompt window where it is running.
 
+## Etrade
+
+create a sandbox (mock) api key:
+https://us.etrade.com/etx/ris/apikey
+then fill out the forms at the bottom of:
+https://developer.etrade.com/getting-started
+
+Make sure to select free real-time quote data:
+https://us.etrade.com/etx/hw/subscriptioncenter#/subscription
+
+Before running the package and send orders, in etrade make a trailing stop order and preview to sign an Advanced Order Disclosure, otherwise an error will rise when posting the order
 
 ## TDAmeritrade
 _______________
 
 *CURRENTLY NO NEW DEVELOPER ACCOUNT ARE CREATED UNTIL THE MERGE*
 
 To access the TDAmeritrade account for trading and info is necessary to install
```

### Comparing `DiscordAlertsTrader-0.8/DiscordAlertsTrader.egg-info/SOURCES.txt` & `DiscordAlertsTrader-0.9.1/DiscordAlertsTrader.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 LICENSE
 README.md
-pyproject.toml
 setup.py
 DiscordAlertsTrader/__init__.py
 DiscordAlertsTrader/alerts_tracker.py
 DiscordAlertsTrader/alerts_trader.py
 DiscordAlertsTrader/configurator.py
 DiscordAlertsTrader/discord_bot.py
+DiscordAlertsTrader/fend_bot.py
 DiscordAlertsTrader/gui.py
 DiscordAlertsTrader/gui_generator.py
 DiscordAlertsTrader/gui_layouts.py
 DiscordAlertsTrader/message_parser.py
 DiscordAlertsTrader.egg-info/PKG-INFO
 DiscordAlertsTrader.egg-info/SOURCES.txt
 DiscordAlertsTrader.egg-info/dependency_links.txt
 DiscordAlertsTrader.egg-info/entry_points.txt
 DiscordAlertsTrader.egg-info/requires.txt
 DiscordAlertsTrader.egg-info/top_level.txt
 DiscordAlertsTrader/brokerages/TDA_api.py
 DiscordAlertsTrader/brokerages/__init__.py
+DiscordAlertsTrader/brokerages/eTrade_api.py
 tests/__init__.py
 tests/msg_samples.py
 tests/td_dummy.py
 tests/test_AlertsTracker.py
 tests/test_TDsession.py
 tests/test_configurator.py
-tests/test_discord_bot.py
+tests/test_discord_bot.py
+tests/test_gui_generator.py
```

### Comparing `DiscordAlertsTrader-0.8/LICENSE` & `DiscordAlertsTrader-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `DiscordAlertsTrader-0.8/PKG-INFO` & `DiscordAlertsTrader-0.9.1/DiscordAlertsTrader.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 Metadata-Version: 2.1
 Name: DiscordAlertsTrader
-Version: 0.8
-Summary: Package for automating discord stock and option alerts.
+Version: 0.9.1
+Summary: Package for automating discord trade alerts in TDA or eTrade.
 Home-page: 
 Download-URL: https://github.com/AdoNunes/DiscordAlertsTrader
 Author: Adonay Nunes
-Author-email: Adonay Nunes <adonay.s.nunes@example.com>
+Author-email: adonays.nunes@gmail.com
 License: BSD (3-clause)
-Project-URL: Homepage, https://github.com/AdoNunes/DiscordAlertsTrader
-Project-URL: Bug Tracker, https://github.com/AdoNunes/DiscordAlertsTrader/issues
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Information Technology
 Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DiscordAlertsTrader: *Discord Alerts Trader Bot*
 ________________________
 
 DiscordAlertsTrader is a python package to get messages from a subscribed discord channel where buy
@@ -42,15 +39,15 @@
 - Read messages and parse trading singals, e.g. BTO (Buy to Open), STC (Sell to Close), partial STC, SL (Stop Limits), PT (Profit Taking)
 - Track trading signals and performance of traders using message history and realtime price
 - Execute and cancel orders, check order status, account status and current ticker prices
 - If in config.ini auto_trade = False, trades are executed manually through promts and optionally choose QTY, price, etc
 
 **Currently, the package is for parsing signals of the discord server BullTrades.** 
 
-Invite link to BullTrades: https://discord.gg/bulltrades
+Invite link to BullTrades with referral: [https://discord.gg/bulltrades](https://bulltrades.net/?ref=ndrjogi)
 
 <img src="media/GUI_analysts_portfolio.PNG" alt="Analysts Portfolio" width="500" height="300">
 <img src="media/GUI_messages.PNG" alt="Channel message history" width="500" height="300">
 (older version shots)
 <img src="media/xtrader_console.png" alt="Console with discord mesages" width="500" height="300">
 <img src="media/xtrader_portfolio.png" alt="Portfolio" width="500" height="300">
 
@@ -119,14 +116,25 @@
 
 Make sure to keep the terminal or command prompt window open while the application is running to see any output or errors.
 
 **Closing the Application**
 
 To stop the DiscordAlertsTrader application, simply close the terminal or command prompt window where it is running.
 
+## Etrade
+
+create a sandbox (mock) api key:
+https://us.etrade.com/etx/ris/apikey
+then fill out the forms at the bottom of:
+https://developer.etrade.com/getting-started
+
+Make sure to select free real-time quote data:
+https://us.etrade.com/etx/hw/subscriptioncenter#/subscription
+
+Before running the package and send orders, in etrade make a trailing stop order and preview to sign an Advanced Order Disclosure, otherwise an error will rise when posting the order
 
 ## TDAmeritrade
 _______________
 
 *CURRENTLY NO NEW DEVELOPER ACCOUNT ARE CREATED UNTIL THE MERGE*
 
 To access the TDAmeritrade account for trading and info is necessary to install
```

### Comparing `DiscordAlertsTrader-0.8/README.md` & `DiscordAlertsTrader-0.9.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: DiscordAlertsTrader
+Version: 0.9.1
+Summary: Package for automating discord trade alerts in TDA or eTrade.
+Home-page: 
+Download-URL: https://github.com/AdoNunes/DiscordAlertsTrader
+Author: Adonay Nunes
+Author-email: adonays.nunes@gmail.com
+License: BSD (3-clause)
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Communications :: Chat
+Classifier: Topic :: Office/Business :: Financial
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Financial and Insurance Industry
+Classifier: Intended Audience :: Information Technology
+Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # DiscordAlertsTrader: *Discord Alerts Trader Bot*
 ________________________
 
 DiscordAlertsTrader is a python package to get messages from a subscribed discord channel where buy
  and sell stock and options signals are messaged. The package will parse the messages and execute
  the trades for traders specified in the config file. It will track the messages from all channels,
  the analysts portfolio and the bot portfolio.
@@ -18,15 +39,15 @@
 - Read messages and parse trading singals, e.g. BTO (Buy to Open), STC (Sell to Close), partial STC, SL (Stop Limits), PT (Profit Taking)
 - Track trading signals and performance of traders using message history and realtime price
 - Execute and cancel orders, check order status, account status and current ticker prices
 - If in config.ini auto_trade = False, trades are executed manually through promts and optionally choose QTY, price, etc
 
 **Currently, the package is for parsing signals of the discord server BullTrades.** 
 
-Invite link to BullTrades: https://discord.gg/bulltrades
+Invite link to BullTrades with referral: [https://discord.gg/bulltrades](https://bulltrades.net/?ref=ndrjogi)
 
 <img src="media/GUI_analysts_portfolio.PNG" alt="Analysts Portfolio" width="500" height="300">
 <img src="media/GUI_messages.PNG" alt="Channel message history" width="500" height="300">
 (older version shots)
 <img src="media/xtrader_console.png" alt="Console with discord mesages" width="500" height="300">
 <img src="media/xtrader_portfolio.png" alt="Portfolio" width="500" height="300">
 
@@ -95,14 +116,25 @@
 
 Make sure to keep the terminal or command prompt window open while the application is running to see any output or errors.
 
 **Closing the Application**
 
 To stop the DiscordAlertsTrader application, simply close the terminal or command prompt window where it is running.
 
+## Etrade
+
+create a sandbox (mock) api key:
+https://us.etrade.com/etx/ris/apikey
+then fill out the forms at the bottom of:
+https://developer.etrade.com/getting-started
+
+Make sure to select free real-time quote data:
+https://us.etrade.com/etx/hw/subscriptioncenter#/subscription
+
+Before running the package and send orders, in etrade make a trailing stop order and preview to sign an Advanced Order Disclosure, otherwise an error will rise when posting the order
 
 ## TDAmeritrade
 _______________
 
 *CURRENTLY NO NEW DEVELOPER ACCOUNT ARE CREATED UNTIL THE MERGE*
 
 To access the TDAmeritrade account for trading and info is necessary to install
```

### Comparing `DiscordAlertsTrader-0.8/setup.py` & `DiscordAlertsTrader-0.9.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,20 +13,21 @@
     for line in (line.strip() for line in fid):
         if line.startswith('__version__'):
             version = line.split('=')[1].strip().strip('\'')
             break
 
 setup(
     name='DiscordAlertsTrader',
-    version='1.0.0',
+    version='0.9.1',
     author='Adonay Nunes',
     author_email='adonays.nunes@gmail.com',
-    description='Package for automating discord stock and option alerts.',
+    description='Package for automating discord trade alerts in TDA or eTrade.',
     license='BSD (3-clause)',
-    long_description='Listen to discord alerts, track profits, execute alerts in brokerage',
+    long_description=open('README.md').read(),
+    long_description_content_type='text/markdown',
     url='',
     download_url='https://github.com/AdoNunes/DiscordAlertsTrader',
     packages=find_packages(),
     install_requires=requirements,
     classifiers=[
         'License :: OSI Approved :: BSD License',
         'Programming Language :: Python :: 3.9',
```

### Comparing `DiscordAlertsTrader-0.8/tests/msg_samples.py` & `DiscordAlertsTrader-0.9.1/tests/msg_samples.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 
 '\b(BTO|STC)\b\s*(\d+)?\s*([A-Z,a-z]+)\s*(\d+[cp])?\s*((\d{1,2}\/\d{1,2}(\/(20\d{2}))?))?\s*@\s*[$]*[ ]*(\d+(?:\.\d+)?|\.\d+)'
 
 exit_examples = [("BTO AEHL @ 7 (risky scalp. PT 8.39, SL below 6.45) @everyone", (8.39, None, None, 6.45)),
                  ("BTO CPB @ 45.95 (SL $43, PT 49, posted this in watchlist on monday", (49.0, None, None, 43.0)),
                  ("Price Target: 185 Stop: 200", (185, None,None, 200)),
                  ("SL around 388.5 PT 380"),
-                 ("BTO 1 COIN 73c 04/06 @ 1.03 @here (Swing) @Cblast Alert")
+                 ("BTO 1 COIN 73c 04/06 @ 1.03 @here (Swing) @Cblast Alert"),
+                 "AVI#9896: STC PNC 140c 07/21/2023 @ 1.4 <@&1037722002145935360> ( 79%)"
                  
 ]
 
 alert = exit_examples[0][0]
 option = re.search(exp, alert, re.IGNORECASE)
 print(option.groups())
```

### Comparing `DiscordAlertsTrader-0.8/tests/td_dummy.py` & `DiscordAlertsTrader-0.9.1/tests/td_dummy.py`

 * *Files identical despite different names*

### Comparing `DiscordAlertsTrader-0.8/tests/test_AlertsTracker.py` & `DiscordAlertsTrader-0.9.1/tests/test_AlertsTracker.py`

 * *Files identical despite different names*

### Comparing `DiscordAlertsTrader-0.8/tests/test_TDsession.py` & `DiscordAlertsTrader-0.9.1/tests/test_TDsession.py`

 * *Files identical despite different names*

### Comparing `DiscordAlertsTrader-0.8/tests/test_configurator.py` & `DiscordAlertsTrader-0.9.1/tests/test_configurator.py`

 * *Files identical despite different names*

### Comparing `DiscordAlertsTrader-0.8/tests/test_discord_bot.py` & `DiscordAlertsTrader-0.9.1/tests/test_discord_bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
         # Example assertions for queue_prints
         print("here:", queue_prints.put.call_args_list)
         self.assertEqual(queue_prints.put.call_count, 3)
         self.assertEqual(queue_prints.put.call_args_list[0][0][0],
                          [f'2022-01-01 10:00:00 \t JonP: BTO 5 AI 25c {expdate} @ 1 <@&940418825235619910> swinging ', 'blue'])
         self.assertEqual(queue_prints.put.call_args_list[1][0][0],
-                         [f'\t \t BTO A {expdate} 25C @1.0 amount: 5', 'green'])
+                         [f'\t \t BTO AI {expdate} 25C @1.0 amount: 5', 'green'])
 
         # Delete the generated file
         os.remove(self.tracker_portfolio_fname)
 
     def test_new_msg_acts_wrong_date(self):
         self.tracker_portfolio_fname="test_tracker_portfolio.csv"
         queue_prints = MagicMock()
```

