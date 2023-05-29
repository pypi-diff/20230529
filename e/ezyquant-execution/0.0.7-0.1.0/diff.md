# Comparing `tmp/ezyquant-execution-0.0.7.tar.gz` & `tmp/ezyquant-execution-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezyquant-execution-0.0.7.tar", last modified: Wed May 24 03:39:53 2023, max compression
+gzip compressed data, was "ezyquant-execution-0.1.0.tar", last modified: Mon May 29 09:34:13 2023, max compression
```

## Comparing `ezyquant-execution-0.0.7.tar` & `ezyquant-execution-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:39:53.105048 ezyquant-execution-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-24 03:39:34.000000 ezyquant-execution-0.0.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-24 03:39:53.105048 ezyquant-execution-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-24 03:39:34.000000 ezyquant-execution-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:39:53.101048 ezyquant-execution-0.0.7/ezyquant_execution/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-24 03:39:34.000000 ezyquant-execution-0.0.7/ezyquant_execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-24 03:39:34.000000 ezyquant-execution-0.0.7/ezyquant_execution/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-24 03:39:34.000000 ezyquant-execution-0.0.7/ezyquant_execution/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)    15105 2023-05-24 03:39:34.000000 ezyquant-execution-0.0.7/ezyquant_execution/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    11597 2023-05-24 03:39:34.000000 ezyquant-execution-0.0.7/ezyquant_execution/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-05-24 03:39:34.000000 ezyquant-execution-0.0.7/ezyquant_execution/executing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-24 03:39:34.000000 ezyquant-execution-0.0.7/ezyquant_execution/realtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-05-24 03:39:34.000000 ezyquant-execution-0.0.7/ezyquant_execution/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:39:53.105048 ezyquant-execution-0.0.7/ezyquant_execution.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-24 03:39:53.000000 ezyquant-execution-0.0.7/ezyquant_execution.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-24 03:39:53.000000 ezyquant-execution-0.0.7/ezyquant_execution.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 03:39:53.000000 ezyquant-execution-0.0.7/ezyquant_execution.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-24 03:39:53.000000 ezyquant-execution-0.0.7/ezyquant_execution.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-24 03:39:53.000000 ezyquant-execution-0.0.7/ezyquant_execution.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-24 03:39:53.105048 ezyquant-execution-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-24 03:39:34.000000 ezyquant-execution-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:34:13.259866 ezyquant-execution-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-29 09:33:48.000000 ezyquant-execution-0.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-29 09:34:13.259866 ezyquant-execution-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-29 09:33:48.000000 ezyquant-execution-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:34:13.259866 ezyquant-execution-0.1.0/ezyquant_execution/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-29 09:33:48.000000 ezyquant-execution-0.1.0/ezyquant_execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-29 09:33:48.000000 ezyquant-execution-0.1.0/ezyquant_execution/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-29 09:33:48.000000 ezyquant-execution-0.1.0/ezyquant_execution/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20311 2023-05-29 09:33:48.000000 ezyquant-execution-0.1.0/ezyquant_execution/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11619 2023-05-29 09:33:48.000000 ezyquant-execution-0.1.0/ezyquant_execution/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-29 09:33:48.000000 ezyquant-execution-0.1.0/ezyquant_execution/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-05-29 09:33:48.000000 ezyquant-execution-0.1.0/ezyquant_execution/executing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-29 09:33:48.000000 ezyquant-execution-0.1.0/ezyquant_execution/realtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-05-29 09:33:48.000000 ezyquant-execution-0.1.0/ezyquant_execution/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:34:13.259866 ezyquant-execution-0.1.0/ezyquant_execution.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-29 09:34:13.000000 ezyquant-execution-0.1.0/ezyquant_execution.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-29 09:34:13.000000 ezyquant-execution-0.1.0/ezyquant_execution.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 09:34:13.000000 ezyquant-execution-0.1.0/ezyquant_execution.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-29 09:34:13.000000 ezyquant-execution-0.1.0/ezyquant_execution.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-29 09:34:13.000000 ezyquant-execution-0.1.0/ezyquant_execution.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-29 09:34:13.259866 ezyquant-execution-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-29 09:33:48.000000 ezyquant-execution-0.1.0/setup.py
```

### Comparing `ezyquant-execution-0.0.7/LICENSE.txt` & `ezyquant-execution-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ezyquant-execution-0.0.7/PKG-INFO` & `ezyquant-execution-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezyquant-execution
-Version: 0.0.7
+Version: 0.1.0
 Summary: Ezyquant execution
 Home-page: https://pydoc.ezyquant.com/
 Author: Fintech (Thailand) Company Limited
 Author-email: admin@fintech.co.th
 Maintainer: Fintech (Thailand) Company Limited
 Maintainer-email: admin@fintech.co.th
 License: The MIT License (MIT)
```

### Comparing `ezyquant-execution-0.0.7/ezyquant_execution/constant.py` & `ezyquant-execution-0.1.0/ezyquant_execution/constant.py`

 * *Files identical despite different names*

### Comparing `ezyquant-execution-0.0.7/ezyquant_execution/context.py` & `ezyquant-execution-0.1.0/ezyquant_execution/context.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,13 @@
+import logging
 import time as t
-import warnings
-from dataclasses import dataclass
 from datetime import datetime
 from functools import cached_property, lru_cache
-from typing import Any, Callable, Dict, List, Optional, TypeVar, Union
+from typing import Any, Callable, Dict, List, Literal, Optional, TypeVar, Union
 
-import pandas as pd
 from settrade_v2.context import Context
 from settrade_v2.equity import InvestorEquity, MarketRepEquity
 from settrade_v2.market import MarketData
 from settrade_v2.realtime import RealtimeDataConnection
 from settrade_v2.user import Investor, MarketRep, _BaseUser
 
 from . import utils
@@ -25,23 +23,27 @@
     EquityPortfolio,
     EquityTrade,
     PortfolioResponse,
     StockQuoteResponse,
 )
 from .realtime import BidOfferSubscriber, PriceInfoSubscriber
 
+logger = logging.getLogger(__name__)
+
 # Override _BaseUser.RealtimeDataConnection
 # because subscribe will error if init RealtimeDataConnection more than once
 # Can remove this line if this issue is fixed
 _BaseUser.RealtimeDataConnection = lru_cache(maxsize=1)(
     _BaseUser.RealtimeDataConnection
 )
 
 T = TypeVar("T")
 
+PLACE_ORDER_MODE_TYPE = Literal["none", "skip", "raise", "available"]
+
 
 def new_refresh(self):
     res = self.request(
         "POST",
         self.refresh_token_path,
         json={"apiKey": self.app_id, "refreshToken": self.refresh_token},
     )
@@ -53,294 +55,497 @@
     self.expired_at = int(t.time()) + res.json()["expires_in"]
 
 
 # Override refresh method
 Context.refresh = new_refresh
 
 
-@dataclass
 class ExecuteContext:
-    settrade_user: Union[Investor, MarketRep]
-    """Settrade user."""
-    account_no: str
-    """Account number."""
-    symbol: str
-    """Selected symbol."""
-    signal: Any = None
-    """Signal."""
-    pin: Optional[str] = None
-    """PIN.
+    def __init__(
+        self,
+        settrade_user: Union[Investor, MarketRep],
+        account_no: str,
+        pin: Optional[str] = None,
+    ):
+        """Execute context.
 
-    Only for investor.
-    """
+        Parameters
+        ----------
+        settrade_user : Union[Investor, MarketRep]
+            Settrade user
+        account_no : str
+            Account number
+        pin : Optional[str], optional
+            PIN. Only for investor.
+        """
+        self.settrade_user = settrade_user
+        self.account_no = account_no
+        self.pin = pin
+
+    def __eq__(self, other):
+        return self.__dict__ == other.__dict__
+
+    def __hash__(self):
+        return id(self)
+
+    @lru_cache
+    def Symbol(self, symbol: str) -> "ExecuteContextSymbol":
+        return ExecuteContextSymbol(
+            settrade_user=self.settrade_user,
+            symbol=symbol,
+            account_no=self.account_no,
+            pin=self.pin,
+        )
 
     @property
     def ts(self) -> datetime:
         """Current timestamp."""
         return datetime.now()
 
     """
-    Price functions
-    """
-
-    @property
-    def market_price(self) -> Optional[float]:
-        """Market price.
-
-        Return 0 at pre-open session.
-        """
-        return self._po_sub.data.last
-
-    @property
-    def best_bid_price(self) -> float:
-        """Best bid price."""
-        return self._bo_sub.data.best_bid_price
-
-    @property
-    def best_ask_price(self) -> float:
-        """Best ask price."""
-        return self._bo_sub.data.best_ask_price
-
-    """
     Account functions
     """
 
     @property
     def line_available(self) -> float:
-        """Line Available."""
+        """Line Available.
+
+        When place order line available will be decrease by order value.
+        """
         return self.get_account_info().line_available
 
     @property
     def cash_balance(self) -> float:
-        """Cash Balance."""
+        """Cash Balance.
+
+        When place order cash balance will **not** be decrease by order
+        value.
+        """
         return self.get_account_info().cash_balance
 
     @property
     def total_cost_value(self) -> float:
-        """Sum of all stock market value in portfolio."""
+        """Sum of all stock cost value in portfolio.
+
+        Include order that pending.
+        """
         return self.get_portfolios().total_portfolio.amount
 
     @property
     def total_market_value(self) -> float:
-        """Sum of all stock cost value in portfolio."""
+        """Sum of all stock market value in portfolio.
+
+        Include order that pending.
+        """
         return self.get_portfolios().total_portfolio.market_value
 
     @property
+    def pending_order_value(self) -> float:
+        """Sum of all pending order value.
+
+        Not include commission.
+        """
+        return sum(i.price * i.vol for i in self.get_orders(_is_pending_order))
+
+    @property
     def port_value(self) -> float:
-        """Total portfolio value."""
-        return self.cash_balance + self.total_market_value
+        """Total portfolio value.
+
+        Line available + Total market value + Pending order value
+        """
+        return self.line_available + self.total_market_value + self.pending_order_value
 
     @property
     def cash(self) -> float:
-        """Cash Balance."""
-        return self.cash_balance
+        """Line Available."""
+        return self.line_available
 
     """
-    Position functions
+    Cancel order functions
+    """
+
+    def cancel_orders(
+        self, condition: Callable[[EquityOrder], bool] = lambda _: True
+    ) -> List[CancelOrder]:
+        """Cancel orders.
+
+        Parameters
+        ----------
+        condition: Callable[[dict], bool]
+            condition function
+
+        Returns
+        -------
+        dict
+            cancel order result
+        """
+        orders = self.get_orders(lambda x: x.can_cancel and condition(x))
+        order_no_list = [i.order_no for i in orders]
+        return self._cancel_orders(order_no_list)
+
+    def cancel_buy_orders(self) -> List[CancelOrder]:
+        """Cancel all buy orders."""
+        return self.cancel_orders(lambda x: x.side.capitalize() == SIDE_BUY)
+
+    def cancel_sell_orders(self) -> List[CancelOrder]:
+        """Cancel all sell orders."""
+        return self.cancel_orders(lambda x: x.side.capitalize() == SIDE_SELL)
+
+    def cancel_price_orders(self, price: float) -> List[CancelOrder]:
+        """Cancel all orders with price."""
+        return self.cancel_orders(lambda x: x.price == price)
+
+    def _cancel_orders(self, order_no_list: List[str]) -> List[CancelOrder]:
+        if not order_no_list:
+            return []
+
+        res = self._settrade_equity.cancel_orders(
+            order_no_list=order_no_list, **self._pin_acc_no_kw
+        )
+        out = [CancelOrder.from_camel_dict(i) for i in res["results"]]
+
+        for i in out:
+            if i.error_response is not None:
+                logger.warn(
+                    f"Cancel order {i.order_no} failed: {i.error_response['message']}"
+                )
+
+        return out
+
+    """
+    Settrade SDK functions
     """
 
     @property
-    def volume(self) -> float:
-        """Actual volume."""
-        ps = self.get_portfolio_symbol()
-        return ps.actual_volume if ps else 0
+    def _acc_no_kw(self) -> dict:
+        return (
+            {"account_no": self.account_no}
+            if isinstance(self.settrade_user, MarketRep)
+            else {}
+        )
 
     @property
-    def cost_price(self) -> float:
-        """Cost price.
+    def _pin_acc_no_kw(self) -> dict:
+        return (
+            {"account_no": self.account_no}
+            if isinstance(self.settrade_user, MarketRep)
+            else {"pin": self.pin}
+        )
 
-        return 0.0 if no position.
-        """
-        ps = self.get_portfolio_symbol()
-        return ps.average_price if ps else 0.0
+    @property
+    def _settrade_equity(self) -> Union[InvestorEquity, MarketRepEquity]:
+        kw = (
+            {"account_no": self.account_no}
+            if isinstance(self.settrade_user, Investor)
+            else {}
+        )
+        return self.settrade_user.Equity(**kw)
 
     @property
-    def cost_value(self) -> float:
-        """Cost value."""
-        ps = self.get_portfolio_symbol()
-        return ps.amount if ps else 0.0
+    def _settrade_market_data(self) -> MarketData:
+        return self.settrade_user.MarketData()
 
     @property
-    def market_value(self) -> float:
-        """Market value of symbol in portfolio."""
-        ps = self.get_portfolio_symbol()
-        return ps.market_value if ps else 0.0
+    def _settrade_realtime_data_connection(self) -> RealtimeDataConnection:
+        return self.settrade_user.RealtimeDataConnection()
+
+    def get_account_info(self) -> BaseAccountInfo:
+        """Get account info."""
+        res = self._settrade_equity.get_account_info(**self._acc_no_kw)
+        return BaseAccountInfo.from_camel_dict(res)
+
+    def get_portfolios(self) -> PortfolioResponse:
+        """Get portfolios."""
+        res: Dict[str, Any] = self._settrade_equity.get_portfolios(**self._acc_no_kw)  # type: ignore
+        return PortfolioResponse.from_camel_dict(res)
+
+    def get_orders(self, condition: Callable = lambda _: True) -> List[EquityOrder]:
+        """Get orders."""
+        if isinstance(self._settrade_equity, InvestorEquity):
+            res = self._settrade_equity.get_orders()
+        else:
+            res = self._settrade_equity.get_orders_by_account_no(
+                account_no=self.account_no
+            )
+        out = [EquityOrder.from_camel_dict(i) for i in res]
+        out = self._filter_list(out, condition)
+        return out
+
+    def get_trades(self, condition: Callable = lambda _: True) -> List[EquityTrade]:
+        """Get trades."""
+        res = self._settrade_equity.get_trades(**self._acc_no_kw)
+        out = [EquityTrade.from_camel_dict(i) for i in res]
+        out = self._filter_list(out, condition)
+        return out
 
     """
-    Place order functions
+    Override functions
     """
 
+    def get_portfolio(self, symbol: str) -> Optional[EquityPortfolio]:
+        """Get portfolio of the symbol."""
+        res = self.get_portfolios()
+        for i in res.portfolio_list:
+            if i.symbol == symbol:
+                return i
+        return None
+
     def place_order(
         self,
+        symbol: str,
         side: SIDE_TYPE,
         volume: float,
-        price: float,
+        price: float = 0,
         qty_open: int = 0,
         trustee_id_type: str = "Local",
         price_type: PRICE_TYPE = "Limit",
         validity_type: VALIDITY_TYPE = "Day",
         bypass_warning: Optional[bool] = True,
         valid_till_date: Optional[str] = None,
+        is_round_up_volume: bool = False,
     ) -> Optional[EquityOrder]:
         """Place order.
 
         Round volume to 100. If volume is 0, return None.
         """
-        volume = utils.round_100(volume)
+        volume = utils.round_100(volume, is_round_up_volume)
         if volume == 0:
             return
 
         res = self._settrade_equity.place_order(
-            symbol=self.symbol,
+            symbol=symbol,
             side=side,
             volume=volume,
             price=price,
             qty_open=qty_open,
             trustee_id_type=trustee_id_type,
             price_type=price_type,
             validity_type=validity_type,
             bypass_warning=bypass_warning,
             valid_till_date=valid_till_date,
             **self._pin_acc_no_kw,
         )
         return EquityOrder.from_camel_dict(res)
 
-    def buy(self, volume: float, price: float) -> Optional[EquityOrder]:
+    def get_quote_symbol(self, symbol: str) -> StockQuoteResponse:
+        """Get quote symbol."""
+        res = self._settrade_market_data.get_quote_symbol(symbol=symbol)
+        return StockQuoteResponse.from_camel_dict(res)
+
+    def _filter_list(self, l: List[T], condition: Callable = lambda _: True) -> List[T]:
+        """Filter list by symbol and condition."""
+        return [i for i in l if condition(i)]
+
+
+class ExecuteContextSymbol(ExecuteContext):
+    def __init__(
+        self,
+        settrade_user: Union[Investor, MarketRep],
+        account_no: str,
+        symbol: str,
+        pin: Optional[str] = None,
+        signal: Any = None,
+    ):
+        """Execute context.
+
+        Parameters
+        ----------
+        settrade_user : Union[Investor, MarketRep]
+            Settrade user
+        account_no : str
+            Account number
+        symbol : str
+            Selected symbol
+        pin : Optional[str], optional
+            PIN. Only for investor.
+        signal : Any, optional
+            Signal, by default None
+        """
+        super().__init__(settrade_user=settrade_user, account_no=account_no, pin=pin)
+        self.symbol = symbol
+        self.signal = signal
+
+    """
+    Price functions
+    """
+
+    @property
+    def market_price(self) -> Optional[float]:
+        """Market price.
+
+        Return 0 at pre-open session.
+        """
+        return self._po_sub.data.last
+
+    @property
+    def best_bid_price(self) -> float:
+        """Best bid price."""
+        return self._bo_sub.data.best_bid_price
+
+    @property
+    def best_ask_price(self) -> float:
+        """Best ask price."""
+        return self._bo_sub.data.best_ask_price
+
+    """
+    Position functions
+    """
+
+    @property
+    def volume(self) -> float:
+        """Actual volume."""
+        return self.actual_volume
+
+    @property
+    def actual_volume(self) -> float:
+        """Actual volume. return 0.0 if no position.
+
+        Actual volume will **not** reduce when order is placed.
+        """
+        ps = self.get_portfolio()
+        return ps.actual_volume if ps else 0
+
+    @property
+    def current_volume(self) -> float:
+        """Current volume. return 0.0 if no position.
+
+        Current volume will reduce when order is placed.
+        """
+        ps = self.get_portfolio()
+        return ps.current_volume if ps else 0
+
+    @property
+    def cost_price(self) -> float:
+        """Cost price.
+
+        return 0.0 if no position.
+        """
+        ps = self.get_portfolio()
+        return ps.average_price if ps else 0.0
+
+    @property
+    def cost_value(self) -> float:
+        """Cost value.
+
+        return 0.0 if no position.
+        """
+        ps = self.get_portfolio()
+        return ps.amount if ps else 0.0
+
+    @property
+    def market_value(self) -> float:
+        """Market value of symbol in portfolio.
+
+        return 0.0 if no position.
+        """
+        ps = self.get_portfolio()
+        return ps.market_value if ps else 0.0
+
+    @property
+    def profit(self) -> float:
+        """Unrealized Profit (THB).
+
+        return 0.0 if no position.
+        """
+        ps = self.get_portfolio()
+        return ps.profit if ps else 0.0
+
+    def percent_profit(self) -> float:
+        """Unrealized Percent profit. return 0.0 if no position.
+
+        Example 1.0 = 1% profit.
+        """
+        ps = self.get_portfolio()
+        return ps.percent_profit if ps else 0.0
+
+    """
+    Place order functions
+    """
+
+    def buy(self, volume: float, price: float = 0, **kwargs) -> Optional[EquityOrder]:
         """Place buy order."""
-        return self.place_order(side=SIDE_BUY, volume=volume, price=price)
+        return self.place_order(side=SIDE_BUY, volume=volume, price=price, **kwargs)
 
-    def sell(self, volume: float, price: float) -> Optional[EquityOrder]:
+    def sell(self, volume: float, price: float = 0, **kwargs) -> Optional[EquityOrder]:
         """Place sell order."""
-        return self.place_order(side=SIDE_SELL, volume=volume, price=price)
+        return self.place_order(side=SIDE_SELL, volume=volume, price=price, **kwargs)
 
-    def buy_pct_port(self, pct_port: float) -> Optional[EquityOrder]:
+    def buy_pct_port(self, pct_port: float, **kwargs) -> Optional[EquityOrder]:
         """Buy from the percentage of the portfolio. calculate the buy volume by pct_port * port_value / best ask price.
 
         Parameters
         ----------
         pct_port: float
             percentage of the portfolio
         """
-        return self.buy_value(self.port_value * pct_port)
+        return self.buy_value(self.port_value * pct_port, **kwargs)
 
-    def buy_value(self, value: float) -> Optional[EquityOrder]:
+    def buy_value(self, value: float, **kwargs) -> Optional[EquityOrder]:
         """Buy from the given value. calculate the buy volume by value / best
         ask price.
 
         Parameters
         ----------
         value: float
             value
         """
         price = self.best_ask_price
         volume = value / price
-        return self.buy(volume=volume, price=price)
+        return self.buy(volume=volume, price=price, **kwargs)
 
-    def sell_pct_port(self, pct_port: float) -> Optional[EquityOrder]:
+    def sell_pct_port(self, pct_port: float, **kwargs) -> Optional[EquityOrder]:
         """Sell from the percentage of the portfolio. calculate the sell volume by pct_port * port_value / best ask price.
         Parameters
         ----------
         pct_port: float
             percentage of the portfolio
         """
-        return self.sell_value(self.port_value * pct_port)
+        return self.sell_value(self.port_value * pct_port, **kwargs)
 
-    def sell_value(self, value: float) -> Optional[EquityOrder]:
+    def sell_value(self, value: float, **kwargs) -> Optional[EquityOrder]:
         """Sell from the given value. calculate the sell volume by value / best
         bid price.
 
         Parameters
         ----------
         value: float
             value
         """
         price = self.best_bid_price
         volume = value / price
-        return self.sell(volume=volume, price=price)
+        return self.sell(volume=volume, price=price, **kwargs)
 
-    def target_pct_port(self, pct_port: float) -> Optional[EquityOrder]:
+    def target_pct_port(self, pct_port: float, **kwargs) -> Optional[EquityOrder]:
         """Buy/Sell to make the current position reach the target percentage of
         the portfolio. Calculate the buy/sell volume by compare between the
         best bid/ask price.
 
         Parameters
         ----------
         pct_port: float
             percentage of the portfolio
         """
-        return self.target_value(self.port_value * pct_port)
+        return self.target_value(self.port_value * pct_port, **kwargs)
 
-    def target_value(self, value: float) -> Optional[EquityOrder]:
+    def target_value(self, value: float, **kwargs) -> Optional[EquityOrder]:
         """Buy/Sell to make the current position reach the target value.
         Calculate the buy/sell volume by compare between the best bid/ask
         price.
 
         Parameters
         ----------
         value: float
             value
         """
         value -= self.market_value
 
         if value > 0:
-            return self.buy_value(value)
+            return self.buy_value(value, **kwargs)
         else:
-            return self.sell_value(-value)
-
-    """
-    Cancel order functions
-    """
-
-    def cancel_orders_symbol(
-        self, condition: Callable[[EquityOrder], bool] = lambda x: True
-    ) -> List[CancelOrder]:
-        """Cancel all orders with this symbol.
-
-        Parameters
-        ----------
-        condition: Callable[[dict], bool]
-            condition function
-
-        Returns
-        -------
-        dict
-            cancel order result
-        """
-        orders = self.get_orders_symbol(condition)
-        order_no_list = [i.order_no for i in orders if i.can_cancel]
-        return self._cancel_orders(order_no_list)
-
-    def cancel_buy_orders_symbol(self) -> List[CancelOrder]:
-        """Cancel all buy orders with this symbol."""
-        return self.cancel_orders_symbol(lambda x: x.side.capitalize() == SIDE_BUY)
-
-    def cancel_sell_orders_symbol(self) -> List[CancelOrder]:
-        """Cancel all sell orders with this symbol."""
-        return self.cancel_orders_symbol(lambda x: x.side.capitalize() == SIDE_SELL)
-
-    def cancel_price_orders_symbol(self, price: float) -> List[CancelOrder]:
-        """Cancel all orders with this symbol and price."""
-        return self.cancel_orders_symbol(lambda x: x.price == price)
-
-    def _cancel_orders(self, order_no_list: List[str]) -> List[CancelOrder]:
-        if not order_no_list:
-            return []
-
-        res = self._settrade_equity.cancel_orders(
-            order_no_list=order_no_list, **self._pin_acc_no_kw
-        )
-        out = [CancelOrder.from_camel_dict(i) for i in res["results"]]
-
-        for i in out:
-            if i.error_response is not None:
-                warnings.warn(
-                    f"Cancel order {i.order_no} failed: {i.error_response['message']}"
-                )
-
-        return out
+            return self.sell_value(-value, **kwargs)
 
     """
     Validate order functions
     """
 
     def is_buy_sufficient(
         self, volume: float, price: float, pct_commission: float = 0.0
@@ -362,132 +567,115 @@
         """Check if the volume is sufficient for sell order.
 
         Parameters
         ----------
         volume: float
             volume
         """
-        return self.volume >= volume
+        return self.current_volume >= volume
 
     """
     Settrade SDK functions
     """
 
-    @property
-    def _acc_no_kw(self) -> dict:
-        return (
-            {"account_no": self.account_no}
-            if isinstance(self.settrade_user, MarketRep)
-            else {}
-        )
-
-    @property
-    def _pin_acc_no_kw(self) -> dict:
-        return (
-            {"account_no": self.account_no}
-            if isinstance(self.settrade_user, MarketRep)
-            else {"pin": self.pin}
-        )
-
-    @property
-    def _settrade_equity(self) -> Union[InvestorEquity, MarketRepEquity]:
-        kw = (
-            {"account_no": self.account_no}
-            if isinstance(self.settrade_user, Investor)
-            else {}
-        )
-        return self.settrade_user.Equity(**kw)
-
-    @property
-    def _settrade_market_data(self) -> MarketData:
-        return self.settrade_user.MarketData()
-
-    @property
-    def _settrade_realtime_data_connection(self) -> RealtimeDataConnection:
-        return self.settrade_user.RealtimeDataConnection()
-
     @cached_property
     def _bo_sub(self) -> BidOfferSubscriber:
         return BidOfferSubscriber(
             symbol=self.symbol, rt_conn=self._settrade_realtime_data_connection
         )
 
     @cached_property
     def _po_sub(self) -> PriceInfoSubscriber:
         return PriceInfoSubscriber(
             symbol=self.symbol, rt_conn=self._settrade_realtime_data_connection
         )
 
-    # TODO: remove if unused
-    def get_candlestick_df(self, limit: int = 5) -> pd.DataFrame:
-        """Get candlestick data.
+    """
+    Override functions
+    """
 
-        Columns: ["lastSequence", "time", "open", "high", "low", "close", "volume", "value"]
+    def get_portfolio(self) -> Optional[EquityPortfolio]:
+        """Get portfolio of the symbol."""
+        return super().get_portfolio(self.symbol)
 
-        Example
-        -------
-        Pre-open
-        >>>     lastSequence                      time  open  ...  close    volume         value
-        ... 0              0 2023-01-10 00:00:00+07:00  75.5  ...  75.25  29748824  2.234758e+09
-        ... 1              0 2023-01-11 00:00:00+07:00  75.0  ...  74.25  42858395  3.189858e+09
-        ... 2              0 2023-01-12 00:00:00+07:00  74.0  ...  74.00  33256792  2.466415e+09
-        ... 3              0 2023-01-13 00:00:00+07:00  74.0  ...  73.50  41266018  3.042763e+09
-        ... 4              0 2023-01-25 00:00:00+07:00  70.0  ...  70.00   2001000  1.500700e+08
-        """
-        df = pd.DataFrame(
-            self._settrade_market_data.get_candlestick(
-                symbol=self.symbol, interval="1d", limit=limit
-            )
-        )
-        df["time"] = pd.to_datetime(df["time"], unit="s", utc=True).dt.tz_convert(
-            "Asia/Bangkok"
-        )
-        return df
+    def place_order(
+        self,
+        side: SIDE_TYPE,
+        volume: float,
+        price: float = 0,
+        qty_open: int = 0,
+        trustee_id_type: str = "Local",
+        price_type: PRICE_TYPE = "Limit",
+        validity_type: VALIDITY_TYPE = "Day",
+        bypass_warning: Optional[bool] = True,
+        valid_till_date: Optional[str] = None,
+        is_round_up_volume: bool = False,
+        mode: PLACE_ORDER_MODE_TYPE = "none",
+    ) -> Optional[EquityOrder]:
+        """Place order.
 
-    def get_quote_symbol(self) -> StockQuoteResponse:
-        """Get quote symbol."""
-        res = self._settrade_market_data.get_quote_symbol(symbol=self.symbol)
-        return StockQuoteResponse.from_camel_dict(res)
+        Round volume to 100. If volume is 0, return None.
 
-    def get_account_info(self) -> BaseAccountInfo:
-        """Get account info."""
-        res = self._settrade_equity.get_account_info(**self._acc_no_kw)
-        return BaseAccountInfo.from_camel_dict(res)
+        Parameters
+        ----------
+        side: SIDE_TYPE
+            Buy or sell
+        ...
+        mode: PLACE_ORDER_MODE_TYPE
+            none: no check
+            skip: skip if not insufficient
+            raise: raise error if not insufficient
+            available: use available volume
+        """
+        volume = utils.round_100(volume, is_round_up_volume)
+
+        if mode != "none":
+            if side == SIDE_BUY:
+                if price == 0:
+                    max_volume = self.line_available / self.best_ask_price
+                else:
+                    max_volume = self.line_available / price
+            else:
+                max_volume = self.current_volume
+
+            if max_volume < volume:
+                if mode == "skip":
+                    logger.warn(f"{side} {volume} is not sufficient")
+                    return
+                elif mode == "raise":
+                    raise ValueError(f"{side} {volume} is not sufficient")
+                elif mode == "available":
+                    logger.info(f"{side} {volume} is not sufficient use {max_volume}")
+                    volume = max_volume
+                    is_round_up_volume = False
+                else:
+                    raise ValueError(f"Invalid mode {mode}")
 
-    def get_portfolios(self) -> PortfolioResponse:
-        """Get portfolio."""
-        res: Dict[str, Any] = self._settrade_equity.get_portfolios(**self._acc_no_kw)  # type: ignore
-        return PortfolioResponse.from_camel_dict(res)
+        return super().place_order(
+            symbol=self.symbol,
+            side=side,
+            volume=volume,
+            price=price,
+            qty_open=qty_open,
+            trustee_id_type=trustee_id_type,
+            price_type=price_type,
+            validity_type=validity_type,
+            bypass_warning=bypass_warning,
+            valid_till_date=valid_till_date,
+            is_round_up_volume=is_round_up_volume,
+        )
 
-    def get_portfolio_symbol(self) -> Optional[EquityPortfolio]:
-        """Get portfolio of the symbol."""
-        res = self.get_portfolios()
-        for i in res.portfolio_list:
-            if i.symbol == self.symbol:
-                return i
-        return None
+    def get_quote_symbol(self) -> StockQuoteResponse:
+        """Get quote symbol."""
+        return super().get_quote_symbol(self.symbol)
 
-    def get_orders_symbol(
-        self, condition: Callable[[EquityOrder], bool] = lambda x: True
-    ) -> List[EquityOrder]:
-        """Get order of the symbol."""
-        if isinstance(self._settrade_equity, InvestorEquity):
-            out = self._settrade_equity.get_orders()
-        else:
-            out = self._settrade_equity.get_orders_by_account_no(
-                account_no=self.account_no
-            )
-        out = [EquityOrder.from_camel_dict(i) for i in out]
-        out = self._filter_list(out, condition)
-        return out
+    def _filter_list(self, l: List[T], condition: Callable = lambda _: True) -> List[T]:
+        """Filter list by symbol and condition."""
+        return super()._filter_list(
+            l, lambda x: x.symbol == self.symbol and condition(x)
+        )
 
-    def get_trades_symbol(
-        self, condition: Callable[[EquityTrade], bool] = lambda x: True
-    ) -> List[EquityTrade]:
-        out = self._settrade_equity.get_trades(**self._acc_no_kw)
-        out = [EquityTrade.from_camel_dict(i) for i in out]
-        out = self._filter_list(out, condition)
-        return out
 
-    def _filter_list(self, l: List[T], condition: Callable = lambda x: True) -> List[T]:
-        """Filter list by symbol and condition."""
-        return [i for i in l if i.symbol == self.symbol and condition(i)]  # type: ignore
+def _is_pending_order(order: EquityOrder) -> bool:
+    return order.balance > 0 and "Expired" not in order.show_order_status
+    # return order.can_cancel # This not work because GTC order can't cancel after market close
+    # return order.balance > 0 # This not work because Expired order still have balance > 0
```

### Comparing `ezyquant-execution-0.0.7/ezyquant_execution/entity.py` & `ezyquant-execution-0.1.0/ezyquant_execution/entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -301,15 +301,15 @@
     marketdescription: float
     """Market description"""
     market_value: float
     """Market value"""
     profit: float
     """Profit/Loss"""
     percent_profit: float
-    """Percentage of profit"""
+    """Percentage of profit. For example 1.0 = 1%"""
     realize_profit: float
     """Realized profit/loss"""
     start_volume: float
     """Initial volume"""
     current_volume: float
     """Current volume"""
     actual_volume: float
```

### Comparing `ezyquant-execution-0.0.7/ezyquant_execution/executing.py` & `ezyquant-execution-0.1.0/ezyquant_execution/executing.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 from datetime import time
 from threading import Event, Timer
 from typing import Any, Awaitable, Callable, Dict, Optional, Union
 
 from settrade_v2.user import Investor, MarketRep
 
 from . import utils
-from .context import ExecuteContext
+from .context import ExecuteContextSymbol
 
 
 def execute_on_timer(
     settrade_user: Union[Investor, MarketRep],
     account_no: str,
     signal_dict: Dict[str, Any],
-    on_timer: Callable[[ExecuteContext], None],
+    on_timer: Callable[[ExecuteContextSymbol], None],
     interval: float,
     start_time: time,
     end_time: time,
     pin: Optional[str] = None,
     event: Optional[Event] = None,
 ):
     """Execute.
@@ -30,15 +30,15 @@
     ----------
     settrade_user : Investor
         settrade sdk user.
     account_no : str
         account number.
     signal_dict : Dict[str, Any]
         signal dictionary. symbol as key and signal as value. this signal will pass to on_timer.
-    on_timer : Callable[[ExecuteContext], None]
+    on_timer : Callable[[ExecuteContextSymbol], None]
         custom function that iterate all symbol in signal_dict.
         if on_timer raise exception, this function will be stopped.
     interval : float
         seconds to sleep between each iteration.
     start_time : time
         time to start.
     end_time : time
@@ -55,15 +55,15 @@
     utils.sleep_until(start_time, event=event)
 
     timer = Timer(utils.seconds_until(end_time), event.set)
     timer.start()
 
     try:
         ctx_list = [
-            ExecuteContext(
+            ExecuteContextSymbol(
                 symbol=k,
                 signal=v,
                 settrade_user=settrade_user,
                 account_no=account_no,
                 pin=pin,
             )
             for k, v in signal_dict.items()
@@ -79,15 +79,15 @@
         timer.cancel()
 
 
 async def async_execute_on_timer(
     settrade_user: Union[Investor, MarketRep],
     account_no: str,
     signal_dict: Dict[str, Any],
-    on_timer: Callable[[ExecuteContext], Awaitable[None]],
+    on_timer: Callable[[ExecuteContextSymbol], Awaitable[None]],
     interval: float,
     start_time: time,
     end_time: time,
     pin: Optional[str] = None,
     event: Optional[asyncio.Event] = None,
 ):
     """Same as execute_on_timer but on_timer is async function."""
@@ -98,15 +98,15 @@
     await utils.async_sleep_until(start_time, event=event)
 
     timer = Timer(utils.seconds_until(end_time), event.set)
     timer.start()
 
     try:
         ctx_list = [
-            ExecuteContext(
+            ExecuteContextSymbol(
                 symbol=k,
                 signal=v,
                 settrade_user=settrade_user,
                 account_no=account_no,
                 pin=pin,
             )
             for k, v in signal_dict.items()
```

### Comparing `ezyquant-execution-0.0.7/ezyquant_execution/realtime.py` & `ezyquant-execution-0.1.0/ezyquant_execution/realtime.py`

 * *Files identical despite different names*

### Comparing `ezyquant-execution-0.0.7/ezyquant_execution/utils.py` & `ezyquant-execution-0.1.0/ezyquant_execution/utils.py`

 * *Files identical despite different names*

### Comparing `ezyquant-execution-0.0.7/ezyquant_execution.egg-info/PKG-INFO` & `ezyquant-execution-0.1.0/ezyquant_execution.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezyquant-execution
-Version: 0.0.7
+Version: 0.1.0
 Summary: Ezyquant execution
 Home-page: https://pydoc.ezyquant.com/
 Author: Fintech (Thailand) Company Limited
 Author-email: admin@fintech.co.th
 Maintainer: Fintech (Thailand) Company Limited
 Maintainer-email: admin@fintech.co.th
 License: The MIT License (MIT)
```

### Comparing `ezyquant-execution-0.0.7/setup.py` & `ezyquant-execution-0.1.0/setup.py`

 * *Files identical despite different names*

