# Comparing `tmp/backtestify-0.1.0.tar.gz` & `tmp/backtestify-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backtestify-0.1.0.tar", last modified: Sun May 28 19:02:35 2023, max compression
+gzip compressed data, was "dist\backtestify-0.1.1.tar", last modified: Mon May 29 00:16:43 2023, max compression
```

## Comparing `backtestify-0.1.0.tar` & `backtestify-0.1.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 19:02:35.885617 backtestify-0.1.0/
--rw-rw-rw-   0        0        0    11558 2023-05-19 19:02:52.000000 backtestify-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      409 2023-05-28 19:02:35.885617 backtestify-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-05-19 19:02:52.000000 backtestify-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 19:02:35.877098 backtestify-0.1.0/backtestify/
--rw-rw-rw-   0        0        0     1362 2023-05-28 18:33:09.000000 backtestify-0.1.0/backtestify/__init__.py
--rw-rw-rw-   0        0        0      142 2023-05-19 19:02:52.000000 backtestify-0.1.0/backtestify/account.py
--rw-rw-rw-   0        0        0     2503 2023-05-28 18:36:38.000000 backtestify-0.1.0/backtestify/backtester.py
--rw-rw-rw-   0        0        0      691 2023-05-28 18:38:27.000000 backtestify-0.1.0/backtestify/cfd.py
--rw-rw-rw-   0        0        0     1931 2023-05-19 19:02:52.000000 backtestify-0.1.0/backtestify/event.py
--rw-rw-rw-   0        0        0      296 2023-05-19 19:02:52.000000 backtestify-0.1.0/backtestify/event_execution_context.py
--rw-rw-rw-   0        0        0      498 2023-05-19 19:02:52.000000 backtestify-0.1.0/backtestify/event_execution_strategy.py
--rw-rw-rw-   0        0        0       74 2023-05-19 19:02:52.000000 backtestify-0.1.0/backtestify/event_type.py
--rw-rw-rw-   0        0        0      431 2023-05-19 19:02:52.000000 backtestify-0.1.0/backtestify/financial_instrument.py
--rw-rw-rw-   0        0        0       98 2023-05-19 19:02:52.000000 backtestify-0.1.0/backtestify/instrument_type.py
--rw-rw-rw-   0        0        0    10199 2023-05-28 18:37:17.000000 backtestify-0.1.0/backtestify/signal_event.py
--rw-rw-rw-   0        0        0      160 2023-05-19 23:36:19.000000 backtestify-0.1.0/backtestify/signal_type.py
--rw-rw-rw-   0        0        0     4721 2023-05-28 18:39:00.000000 backtestify-0.1.0/backtestify/strategy.py
--rw-rw-rw-   0        0        0      494 2023-05-23 03:39:36.000000 backtestify-0.1.0/backtestify/trade.py
--rw-rw-rw-   0        0        0    11120 2023-05-28 18:37:46.000000 backtestify-0.1.0/backtestify/trade_executor.py
--rw-rw-rw-   0        0        0     2518 2023-05-28 18:35:43.000000 backtestify-0.1.0/backtestify/trade_state.py
-drwxrwxrwx   0        0        0        0 2023-05-28 19:02:35.883096 backtestify-0.1.0/backtestify.egg-info/
--rw-rw-rw-   0        0        0      409 2023-05-28 19:02:35.000000 backtestify-0.1.0/backtestify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      642 2023-05-28 19:02:35.000000 backtestify-0.1.0/backtestify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 19:02:35.000000 backtestify-0.1.0/backtestify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-28 19:02:35.000000 backtestify-0.1.0/backtestify.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-28 19:02:35.000000 backtestify-0.1.0/backtestify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-28 19:02:35.886613 backtestify-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      662 2023-05-28 18:15:57.000000 backtestify-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:16:43.000000 backtestify-0.1.1/
+-rw-rw-rw-   0        0        0    11558 2023-05-19 19:02:52.000000 backtestify-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      409 2023-05-29 00:16:43.000000 backtestify-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-05-19 19:02:52.000000 backtestify-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 00:16:43.000000 backtestify-0.1.1/backtestify/
+-rw-rw-rw-   0        0        0     1362 2023-05-28 18:33:09.000000 backtestify-0.1.1/backtestify/__init__.py
+-rw-rw-rw-   0        0        0      142 2023-05-19 19:02:52.000000 backtestify-0.1.1/backtestify/account.py
+-rw-rw-rw-   0        0        0     2503 2023-05-28 23:36:45.000000 backtestify-0.1.1/backtestify/backtester.py
+-rw-rw-rw-   0        0        0      696 2023-05-28 19:31:49.000000 backtestify-0.1.1/backtestify/cfd.py
+-rw-rw-rw-   0        0        0     1931 2023-05-19 19:02:52.000000 backtestify-0.1.1/backtestify/event.py
+-rw-rw-rw-   0        0        0      296 2023-05-19 19:02:52.000000 backtestify-0.1.1/backtestify/event_execution_context.py
+-rw-rw-rw-   0        0        0      498 2023-05-19 19:02:52.000000 backtestify-0.1.1/backtestify/event_execution_strategy.py
+-rw-rw-rw-   0        0        0       74 2023-05-19 19:02:52.000000 backtestify-0.1.1/backtestify/event_type.py
+-rw-rw-rw-   0        0        0      431 2023-05-19 19:02:52.000000 backtestify-0.1.1/backtestify/financial_instrument.py
+-rw-rw-rw-   0        0        0       98 2023-05-19 19:02:52.000000 backtestify-0.1.1/backtestify/instrument_type.py
+-rw-rw-rw-   0        0        0    10196 2023-05-29 00:05:22.000000 backtestify-0.1.1/backtestify/signal_event.py
+-rw-rw-rw-   0        0        0      160 2023-05-19 23:36:19.000000 backtestify-0.1.1/backtestify/signal_type.py
+-rw-rw-rw-   0        0        0     4822 2023-05-28 22:45:19.000000 backtestify-0.1.1/backtestify/strategy.py
+-rw-rw-rw-   0        0        0      494 2023-05-23 03:39:36.000000 backtestify-0.1.1/backtestify/trade.py
+-rw-rw-rw-   0        0        0    11120 2023-05-28 18:37:46.000000 backtestify-0.1.1/backtestify/trade_executor.py
+-rw-rw-rw-   0        0        0     2872 2023-05-28 23:20:05.000000 backtestify-0.1.1/backtestify/trade_state.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:16:43.000000 backtestify-0.1.1/backtestify.egg-info/
+-rw-rw-rw-   0        0        0      409 2023-05-29 00:16:43.000000 backtestify-0.1.1/backtestify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      642 2023-05-29 00:16:43.000000 backtestify-0.1.1/backtestify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 00:16:43.000000 backtestify-0.1.1/backtestify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-29 00:16:43.000000 backtestify-0.1.1/backtestify.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-29 00:16:43.000000 backtestify-0.1.1/backtestify.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 00:16:43.000000 backtestify-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      662 2023-05-29 00:15:02.000000 backtestify-0.1.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `backtestify-0.1.0/LICENSE` & `backtestify-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `backtestify-0.1.0/backtestify/__init__.py` & `backtestify-0.1.1/backtestify/__init__.py`

 * *Files identical despite different names*

### Comparing `backtestify-0.1.0/backtestify/backtester.py` & `backtestify-0.1.1/backtestify/backtester.py`

 * *Files identical despite different names*

### Comparing `backtestify-0.1.0/backtestify/cfd.py` & `backtestify-0.1.1/backtestify/cfd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from backtestify.financial_instrument import FinancialInstrument
 
 class CFD(FinancialInstrument):
-    def __init__(self, symbol, instrument_type, lot_size, entry_lots, commission, point_value, leverage, period, point, spread, pips, currency_ratio=1):
+    def __init__(self, instrument_type, lot_size, entry_lots, commission, point_value, leverage, period, point, spread, pips, currency_ratio=1, symbol=None):
         super().__init__(symbol, lot_size, entry_lots, commission, leverage, period, currency_ratio)
         self.instrument_type = instrument_type
         self.pips = pips
         self.point_value = point_value
         self.point = point
         self.spread = spread
         self.spread_points = spread * point
```

### Comparing `backtestify-0.1.0/backtestify/event.py` & `backtestify-0.1.1/backtestify/event.py`

 * *Files identical despite different names*

### Comparing `backtestify-0.1.0/backtestify/signal_event.py` & `backtestify-0.1.1/backtestify/signal_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,20 +42,20 @@
         self.previous_event = previous_event
         self.open_price = None
         self.high_price = None
         self.low_price = None
         self.close_price = None
         self.volume = None
         self.swap_long = None
-        self.swap_short = None
+        self.swap_short = None,
 
     def execute(self, instrument, current_trade_state, balance, current_bar):
         if current_bar == 0:
             return TradeState(balance)
-        
+    
         trade = None
         is_trade_open = False
 
         trade_state = TradeState.copy_and_update(
             current_trade_state=current_trade_state,
             swap_long=self.swap_long,
             swap_short=self.swap_short,
@@ -72,15 +72,15 @@
             current_bar=current_bar,
             equity=trade_state.equity,
             margin=instrument.margin,
             currency_ratio=instrument.currency_ratio,
         )
 
         if trade_state.signal is None:
-            if trade_state.equity <= instrument.required_margin and (self.signal == SignalType.BUY or self.signal == SignalType.SELL):
+            if trade_state.equity <= instrument.required_margin or (self.signal != SignalType.BUY and self.signal != SignalType.SELL):
                 return trade_state
             
             trade = trade_executor.open_trade(
                 trade_state=trade_state,
                 commission=instrument.commission,
                 position_size=instrument.position_size,
                 event_signal=self.signal,
```

### Comparing `backtestify-0.1.0/backtestify/strategy.py` & `backtestify-0.1.1/backtestify/strategy.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,66 +5,66 @@
 
 class Strategy:
     def __init__(self, prices_info):
         self.prices_info = prices_info
         self.current_index = 0
         self.events = []
 
-    def get_past_info(self):
-        return self.prices_info.iloc[:self.current_index + 1]
+    def get_past_info(self, shift=1):
+        return self.prices_info.iloc[:self.current_index + shift]
     
     def set_ohlcv(self, signal):
-        required_columns = ['open', 'high', 'low', 'close']
-        optional_columns = ['volume']
+        required_columns = ["open", "high", "low", "close"]
+        optional_columns = ["volume"]
 
         past_info = self.get_past_info()
 
         for column in required_columns:
             if column not in past_info.columns:
                 raise ValueError(f"The market info must have a '{column}' column.")
-            setattr(signal, f'{column}_price', past_info[column].iloc[-1])
+            setattr(signal, f"{column}_price", past_info[column].iloc[-1])
 
         for column in optional_columns:
             if column in past_info.columns:
                 setattr(signal, column, past_info[column].iloc[-1])
 
     def set_timestamp_if_none(self, signal):
         if signal.timestamp is not None:
             return None
 
         past_info = self.get_past_info()
 
-        if past_info.index.name == 'timestamp':
+        if past_info.index.name == "timestamp":
             signal.timestamp = past_info.index[-1]
-        elif 'timestamp' in past_info.columns:
-            signal.timestamp = past_info['timestamp'].iloc[-1]
+        elif "timestamp" in past_info.columns:
+            signal.timestamp = past_info["timestamp"].iloc[-1]
         else:
-            raise ValueError("The market info must have a 'timestamp' column or index.")
+            raise ValueError("The market info must have a 'timestam' column or index.")
 
         return None
         
     def set_swap_info_if_none(self, signal):
         past_info = self.get_past_info()
 
         if signal.swap_long is not None and signal.swap_short is not None:
             return None
 
         past_info = self.get_past_info()
 
-        for attr in ['swap_long', 'swap_short']:
+        for attr in ["swap_long", "swap_short"]:
             last_value = past_info.get(attr)
             setattr(signal, attr, last_value.iloc[-1] if last_value is not None else 0)
 
     def set_symbol_if_none(self, signal):
         past_info = self.get_past_info()
 
-        if signal.symbol is not None or 'symbol' not in past_info.columns:
+        if signal.symbol is not None or "symbol" not in past_info.columns:
             return
         
-        signal.symbol = past_info['symbol'].iloc[-1]
+        signal.symbol = past_info["symbol"].iloc[-1]
 
     def get_signal_events(self, events):
         return [event for event in events if event.event_type == EventType.SIGNAL]
 
     def get_signal_event(self, events):
         signal_events = self.get_signal_events(events)
 
@@ -93,40 +93,41 @@
             self.set_symbol_if_none(signal)
             self.set_previous_event(signal)
             self.set_bar_index(signal)
 
     def apply_strategy(self, next_candle):
         # Save the amount of size of the prices_info
         prices_info_size = len(self.prices_info)
-            
-        for index, current in enumerate(self.prices_info.itertuples()):
+
+        for index, _ in enumerate(self.prices_info.itertuples()):
             self.current_index = index
-            history = self.get_past_info()
-            result_events = next_candle(current, history)
+            history = self.get_past_info(shift=1)
+            result_events = next_candle(history)
 
             # Create initial event to open the first trade
             initial_event = SignalEvent(signal=None) if index == 0 else None
 
             # Create last event to close the last trade
             last_event = SignalEvent(signal=SignalType.EXIT) if index == prices_info_size - 1 else None
 
             if result_events is None or (isinstance(result_events, (list, tuple)) and not result_events):
                 result_events = [SignalEvent(signal=None)]
             elif isinstance(result_events, Event):
                 result_events = [result_events]
 
             if initial_event:
-                result_events.append(initial_event)
+                # The initial event is always none because is the way to create the trade state
+                result_events = [initial_event, *result_events]
             if last_event:
                 result_events.append(last_event)
 
             self.set_information(result_events)
             self.events.extend(result_events)
 
         return self.events
 
     def generate_signals(self):
-        if not hasattr(self, 'next_candle'):
+        if not hasattr(self, "next_candle"):
             raise NotImplementedError("Subclasses should implement a next_candle method.")
         
         events = self.apply_strategy(self.next_candle)
         return events
```

### Comparing `backtestify-0.1.0/backtestify/trade_executor.py` & `backtestify-0.1.1/backtestify/trade_executor.py`

 * *Files identical despite different names*

### Comparing `backtestify-0.1.0/backtestify/trade_state.py` & `backtestify-0.1.1/backtestify/trade_state.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,12 +52,18 @@
         swap = -swap_long if current_trade_state.signal == SignalType.BUY else swap_short
         days_per_year = 252
         adjusted_price = current_trade_state.adjusted_price + swap / days_per_year * point
 
         return cls(
             balance=current_trade_state.balance,
             size=current_trade_state.size,
-            signal=current_trade_state.signal,
+            signal=current_trade_state.signal if current_trade_state.signal != SignalType.EXIT else None,
             stop_loss=current_trade_state.stop_loss,
             take_profit=current_trade_state.take_profit,
             adjusted_price=adjusted_price
-        )
+        )
+
+    def __str__(self):
+        return "Trade Signal: %s, Balance: %s, Equity: %s, Amount: %s, Unrealized Profit: %s, Realized Profit: %s" % (self.signal, self.balance, self.equity, self.size, self.unrealized_profit, self.realized_profit)
+
+    def __repr__(self):
+        return str(self)
```

### Comparing `backtestify-0.1.0/backtestify.egg-info/SOURCES.txt` & `backtestify-0.1.1/backtestify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backtestify-0.1.0/setup.py` & `backtestify-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as file:
     more_description = file.read()
 
 setuptools.setup(
     name="backtestify",
-    version="0.1.0",
+    version="0.1.1",
     author="Eladio Rocha Vizcaino",
     author_email="eladio.rocha99@gmail.com",
     description="A package for backtesting trading strategies",
     more_description=more_description,
     long_description_content_type="text/markdown",
     url="https://github.com/EladioRocha/backtestify",
     project_urls={
```

