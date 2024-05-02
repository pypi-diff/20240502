# Comparing `tmp/martin_binance-3.0.6.tar.gz` & `tmp/martin_binance-3.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "martin_binance-3.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "martin_binance-3.0.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `martin_binance-3.0.6.tar` & `martin_binance-3.0.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1079 2024-04-19 15:23:47.148182 martin_binance-3.0.6/LICENSE
--rwxr-xr-x   0        0        0     3854 2024-04-19 15:23:47.148182 martin_binance-3.0.6/README.md
--rwxr-xr-x   0        0        0     1890 2024-04-19 15:23:47.184182 martin_binance-3.0.6/martin_binance/__init__.py
--rw-r--r--   0        0        0     5007 2024-04-19 15:23:47.184182 martin_binance-3.0.6/martin_binance/backtest/OoTSP.py
--rw-r--r--   0        0        0     2786 2024-04-19 15:23:47.184182 martin_binance-3.0.6/martin_binance/backtest/VCoSEL.py
--rw-r--r--   0        0        0        0 2024-04-19 15:23:47.184182 martin_binance-3.0.6/martin_binance/backtest/__init__.py
--rw-r--r--   0        0        0    13214 2024-04-19 15:23:47.184182 martin_binance-3.0.6/martin_binance/backtest/exchange_simulator.py
--rwxr-xr-x   0        0        0     4165 2024-04-19 15:23:47.184182 martin_binance-3.0.6/martin_binance/backtest/optimizer.py
--rw-r--r--   0        0        0     4781 2024-04-19 15:23:47.184182 martin_binance-3.0.6/martin_binance/client.py
--rw-r--r--   0        0        0     6935 2024-04-19 15:23:47.184182 martin_binance-3.0.6/martin_binance/db_utils.py
--rwxr-xr-x   0        0        0   139982 2024-04-19 15:23:47.184182 martin_binance-3.0.6/martin_binance/executor.py
--rw-r--r--   0        0        0    15709 2024-04-19 15:23:47.184182 martin_binance-3.0.6/martin_binance/lib.py
--rw-r--r--   0        0        0     3287 2024-04-19 15:23:47.184182 martin_binance-3.0.6/martin_binance/params.py
--rw-r--r--   0        0        0      485 2024-04-19 15:23:47.184182 martin_binance-3.0.6/martin_binance/service/.tmux.conf
--rwxr-xr-x   0        0        0      319 2024-04-19 15:23:47.184182 martin_binance-3.0.6/martin_binance/service/funds_export.service
--rwxr-xr-x   0        0        0    14650 2024-04-19 15:23:47.184182 martin_binance-3.0.6/martin_binance/service/funds_rate_exporter.py
--rwxr-xr-x   0        0        0    75764 2024-04-19 15:23:47.184182 martin_binance-3.0.6/martin_binance/service/grafana.json
--rwxr-xr-x   0        0        0     1269 2024-04-19 15:23:47.184182 martin_binance-3.0.6/martin_binance/service/relaunch.py
--rwxr-xr-x   0        0        0      271 2024-04-19 15:23:47.184182 martin_binance-3.0.6/martin_binance/service/relaunch.service
--rw-r--r--   0        0        0    83599 2024-04-19 15:23:47.188182 martin_binance-3.0.6/martin_binance/strategy_base.py
--rw-r--r--   0        0        0     7151 2024-04-19 15:23:47.188182 martin_binance-3.0.6/martin_binance/telegram_utils.py
--rw-r--r--   0        0        0     7217 2024-04-19 15:23:47.188182 martin_binance-3.0.6/martin_binance/templates/cli_0_BTCUSDT.py
--rw-r--r--   0        0        0     7219 2024-04-19 15:23:47.188182 martin_binance-3.0.6/martin_binance/templates/cli_1_BTCUSDT.py
--rw-r--r--   0        0        0     7223 2024-04-19 15:23:47.188182 martin_binance-3.0.6/martin_binance/templates/cli_2_TESTBTCTESTUSDT.py
--rwxr-xr-x   0        0        0     7212 2024-04-19 15:23:47.188182 martin_binance-3.0.6/martin_binance/templates/cli_3_BTCUSDT.py
--rw-r--r--   0        0        0   237568 2024-04-19 15:23:47.188182 martin_binance-3.0.6/martin_binance/templates/funds_rate.db
--rw-r--r--   0        0        0     1723 2024-04-19 15:23:47.188182 martin_binance-3.0.6/martin_binance/templates/ms_cfg.toml
--rw-r--r--   0        0        0      639 2024-04-19 15:23:47.188182 martin_binance-3.0.6/martin_binance/templates/trial_params.json
--rw-r--r--   0        0        0     1425 2024-04-19 15:23:47.188182 martin_binance-3.0.6/pyproject.toml
--rw-r--r--   0        0        0     5155 1970-01-01 00:00:00.000000 martin_binance-3.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-05-02 19:41:19.615981 martin_binance-3.0.7/LICENSE
+-rwxr-xr-x   0        0        0     4065 2024-05-02 19:41:19.615981 martin_binance-3.0.7/README.md
+-rwxr-xr-x   0        0        0     1890 2024-05-02 19:41:19.651981 martin_binance-3.0.7/martin_binance/__init__.py
+-rw-r--r--   0        0        0     5007 2024-05-02 19:41:19.651981 martin_binance-3.0.7/martin_binance/backtest/OoTSP.py
+-rw-r--r--   0        0        0     2786 2024-05-02 19:41:19.651981 martin_binance-3.0.7/martin_binance/backtest/VCoSEL.py
+-rw-r--r--   0        0        0        0 2024-05-02 19:41:19.651981 martin_binance-3.0.7/martin_binance/backtest/__init__.py
+-rw-r--r--   0        0        0    13214 2024-05-02 19:41:19.651981 martin_binance-3.0.7/martin_binance/backtest/exchange_simulator.py
+-rw-r--r--   0        0        0     4245 2024-05-02 19:41:19.651981 martin_binance-3.0.7/martin_binance/backtest/optimizer.py
+-rw-r--r--   0        0        0     4781 2024-05-02 19:41:19.651981 martin_binance-3.0.7/martin_binance/client.py
+-rw-r--r--   0        0        0     6935 2024-05-02 19:41:19.651981 martin_binance-3.0.7/martin_binance/db_utils.py
+-rw-r--r--   0        0        0   140099 2024-05-02 19:41:19.651981 martin_binance-3.0.7/martin_binance/executor.py
+-rw-r--r--   0        0        0    15709 2024-05-02 19:41:19.651981 martin_binance-3.0.7/martin_binance/lib.py
+-rw-r--r--   0        0        0     3287 2024-05-02 19:41:19.651981 martin_binance-3.0.7/martin_binance/params.py
+-rw-r--r--   0        0        0      485 2024-05-02 19:41:19.651981 martin_binance-3.0.7/martin_binance/service/.tmux.conf
+-rwxr-xr-x   0        0        0      319 2024-05-02 19:41:19.651981 martin_binance-3.0.7/martin_binance/service/funds_export.service
+-rwxr-xr-x   0        0        0    14650 2024-05-02 19:41:19.651981 martin_binance-3.0.7/martin_binance/service/funds_rate_exporter.py
+-rwxr-xr-x   0        0        0    75764 2024-05-02 19:41:19.651981 martin_binance-3.0.7/martin_binance/service/grafana.json
+-rwxr-xr-x   0        0        0     1269 2024-05-02 19:41:19.651981 martin_binance-3.0.7/martin_binance/service/relaunch.py
+-rwxr-xr-x   0        0        0      271 2024-05-02 19:41:19.651981 martin_binance-3.0.7/martin_binance/service/relaunch.service
+-rw-r--r--   0        0        0    83858 2024-05-02 19:41:19.651981 martin_binance-3.0.7/martin_binance/strategy_base.py
+-rw-r--r--   0        0        0     7151 2024-05-02 19:41:19.651981 martin_binance-3.0.7/martin_binance/telegram_utils.py
+-rw-r--r--   0        0        0     7217 2024-05-02 19:41:19.655981 martin_binance-3.0.7/martin_binance/templates/cli_0_BTCUSDT.py
+-rw-r--r--   0        0        0     7219 2024-05-02 19:41:19.655981 martin_binance-3.0.7/martin_binance/templates/cli_1_BTCUSDT.py
+-rw-r--r--   0        0        0     7223 2024-05-02 19:41:19.655981 martin_binance-3.0.7/martin_binance/templates/cli_2_TESTBTCTESTUSDT.py
+-rwxr-xr-x   0        0        0     7212 2024-05-02 19:41:19.655981 martin_binance-3.0.7/martin_binance/templates/cli_3_BTCUSDT.py
+-rw-r--r--   0        0        0   237568 2024-05-02 19:41:19.655981 martin_binance-3.0.7/martin_binance/templates/funds_rate.db
+-rw-r--r--   0        0        0     1723 2024-05-02 19:41:19.655981 martin_binance-3.0.7/martin_binance/templates/ms_cfg.toml
+-rw-r--r--   0        0        0      639 2024-05-02 19:41:19.655981 martin_binance-3.0.7/martin_binance/templates/trial_params.json
+-rw-r--r--   0        0        0     1425 2024-05-02 19:41:19.655981 martin_binance-3.0.7/pyproject.toml
+-rw-r--r--   0        0        0     5366 1970-01-01 00:00:00.000000 martin_binance-3.0.7/PKG-INFO
```

### Comparing `martin_binance-3.0.6/LICENSE` & `martin_binance-3.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.6/README.md` & `martin_binance-3.0.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 
 >Valid: (BTC/USDT), (ETH/BUSD), (SOL/LTC)
 > 
 >Incorrectly: (BTC/USDT), (ETH/USDT), (BTC/ETH)
 > 
 >As a result of the mutual impact on the operating balance sheet, the liquidity control system will block the work.
 
+* Due to a limitation in the implementation of asyncio under Windows, this program cannot be executed. [Use Docker on Windows instead.](https://github.com/DogsTailFarmer/martin-binance/wiki/Quick-start#docker)
+
 ## References
 * Detailed information about use this strategy placed to [wiki](https://github.com/DogsTailFarmer/martin-binance/wiki)
 * [Trade idea](https://github.com/DogsTailFarmer/martin-binance/wiki/Trade-idea)
 * [Quick start](https://github.com/DogsTailFarmer/martin-binance/wiki/Quick-start)
 * [Back testing and parameters optimization](https://github.com/DogsTailFarmer/martin-binance/wiki/Back-testing-and-parameters-optimization)
 
 ## Referral link
```

#### html2text {}

```diff
@@ -15,21 +15,24 @@
 strategy lie with you. Strongly recommended that you test the strategy in the
 demo mode before using real bidding. ## Important notices * After update to
 `3.0.1`, the configuration files `cli_XX_AAABBB.py` for all running trading
 pairs should be updated. Use templates for reference. * You cannot run multiple
 pairs with overlapping currencies on the same account! >Valid: (BTC/USDT),
 (ETH/BUSD), (SOL/LTC) > >Incorrectly: (BTC/USDT), (ETH/USDT), (BTC/ETH) > >As a
 result of the mutual impact on the operating balance sheet, the liquidity
-control system will block the work. ## References * Detailed information about
-use this strategy placed to [wiki](https://github.com/DogsTailFarmer/martin-
-binance/wiki) * [Trade idea](https://github.com/DogsTailFarmer/martin-binance/
-wiki/Trade-idea) * [Quick start](https://github.com/DogsTailFarmer/martin-
-binance/wiki/Quick-start) * [Back testing and parameters optimization](https://
-github.com/DogsTailFarmer/martin-binance/wiki/Back-testing-and-parameters-
-optimization) ## Referral link
+control system will block the work. * Due to a limitation in the implementation
+of asyncio under Windows, this program cannot be executed. [Use Docker on
+Windows instead.](https://github.com/DogsTailFarmer/martin-binance/wiki/Quick-
+start#docker) ## References * Detailed information about use this strategy
+placed to [wiki](https://github.com/DogsTailFarmer/martin-binance/wiki) *
+[Trade idea](https://github.com/DogsTailFarmer/martin-binance/wiki/Trade-idea)
+* [Quick start](https://github.com/DogsTailFarmer/martin-binance/wiki/Quick-
+start) * [Back testing and parameters optimization](https://github.com/
+DogsTailFarmer/martin-binance/wiki/Back-testing-and-parameters-optimization) ##
+Referral link
 Create account on [Binance](https://accounts.binance.com/en/
 register?ref=QCS4OGWR) and get 10% discount on all trading fee Create account
 on [HUOBI](https://www.huobi.com/en-us/topic/double-reward/
 ?invite_code=9uaw3223) and will get 50 % off trading fees Create account on
 [Bitfinex](https://www.bitfinex.com/sign-up?refcode=v_4az2nCP) and get 6%
 rebate fee Create account on [OKEX](https://www.okex.com/join/2607649) and get
 Mystery Boxes worth up to $10,000 Create account on [Bybit](https://
```

### Comparing `martin_binance-3.0.6/martin_binance/__init__.py` & `martin_binance-3.0.7/martin_binance/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 """
 Free trading system for Binance SPOT API
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "3.0.6"
+__version__ = "3.0.7"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 from pathlib import Path
 from shutil import copy
 
 from exchanges_wrapper.definitions import Interval
```

### Comparing `martin_binance-3.0.6/martin_binance/backtest/OoTSP.py` & `martin_binance-3.0.7/martin_binance/backtest/OoTSP.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.6/martin_binance/backtest/VCoSEL.py` & `martin_binance-3.0.7/martin_binance/backtest/VCoSEL.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.6/martin_binance/backtest/exchange_simulator.py` & `martin_binance-3.0.7/martin_binance/backtest/exchange_simulator.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.6/martin_binance/backtest/optimizer.py` & `martin_binance-3.0.7/martin_binance/backtest/optimizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,19 @@
 
 import optuna
 import ujson as json
 
 from martin_binance import LOG_PATH, TRIAL_PARAMS
 
 OPTIMIZER = Path(__file__).absolute()
-OPTIMIZER.chmod(OPTIMIZER.stat().st_mode | stat.S_IEXEC)
+try:
+    OPTIMIZER.chmod(OPTIMIZER.stat().st_mode | stat.S_IEXEC)
+except PermissionError:
+    pass  # if executed in Docker environment
+
 PARAMS_FLOAT = ['KBB']
 STRATEGY = None
 
 
 # noinspection PyUnusedLocal
 def notify_exception(*args):
     pass  # Supress message from sys.excepthook
```

### Comparing `martin_binance-3.0.6/martin_binance/client.py` & `martin_binance-3.0.7/martin_binance/client.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.6/martin_binance/db_utils.py` & `martin_binance-3.0.7/martin_binance/db_utils.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.6/martin_binance/executor.py` & `martin_binance-3.0.7/martin_binance/executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Cyclic grid strategy based on martingale
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "3.0.6"
+__version__ = "3.0.7"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = 'https://github.com/DogsTailFarmer'
 ##################################################################
 import logging
 import sys
 import gc
 import statistics
@@ -34,14 +34,23 @@
 from martin_binance.strategy_base import StrategyBase, __version__ as msb_ver
 from martin_binance.lib import Ticker, FundsEntry, OrderBook, Style, any2str, Order, OrderUpdate, Orders, f2d, solve
 from martin_binance.params import *
 
 O_DEC = Decimal()
 
 
+def get_mode_details(mode):
+    mode_mapping = {
+        'T': ("Trade", Style.B_WHITE),
+        'TC': ("Trade & Collect", Style.B_RED),
+        'S': ("Simulate", Style.GREEN)
+    }
+    return mode_mapping.get(mode, ("Unknown Mode", Style.RESET))
+
+
 class Strategy(StrategyBase):
     def __init__(self, call_super=True):
         if call_super:
             super().__init__()
         if LOGGING:
             print(f"Init Strategy, ver: {HEAD_VERSION} + {__version__} + {msb_ver}")
         self.cycle_buy = not START_ON_BUY if REVERSE else START_ON_BUY  # + Direction (Buy/Sell) for current cycle
@@ -163,17 +172,18 @@
         self.martin = (MARTIN + 100) / 100
         if not check_funds:
             self.first_run = False
         if GRID_ONLY:
             self.message_log(f"Mode for {'Buy' if self.cycle_buy else 'Sell'} {self.f_currency} by grid orders"
                              f" placement ON",
                              color=Style.B_WHITE)
-        self.message_log(f"This is {'Trade' if MODE == 'T' else ('Trade & Collect' if MODE == 'TC' else 'Simulate')}"
-                         f" mode",
-                         color=Style.B_WHITE if MODE == 'T' else (Style.B_RED if MODE == 'TC' else Style.GREEN))
+
+        mode_message, mode_color = get_mode_details(MODE)
+        self.message_log(f"This is {mode_message} mode", color=mode_color)
+
         if MODE == 'TC' and SELF_OPTIMIZATION:
             self.message_log("Auto update parameters mode!", log_level=logging.WARNING, color=Style.B_RED)
         # Calculate round float multiplier
         self.round_base = ROUND_BASE or str(tcm.round_amount(f2d(1.123456789), ROUND_FLOOR))
         self.round_quote = ROUND_QUOTE or str(Decimal(self.round_base) *
                                               Decimal(str(tcm.round_price(f2d(1.123456789), ROUND_FLOOR))))
         self.message_log(f"Round pattern, for base: {self.round_base}, quote: {self.round_quote}")
```

### Comparing `martin_binance-3.0.6/martin_binance/lib.py` & `martin_binance-3.0.7/martin_binance/lib.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.6/martin_binance/params.py` & `martin_binance-3.0.7/martin_binance/params.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.6/martin_binance/service/funds_rate_exporter.py` & `martin_binance-3.0.7/martin_binance/service/funds_rate_exporter.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.6/martin_binance/service/grafana.json` & `martin_binance-3.0.7/martin_binance/service/grafana.json`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.6/martin_binance/service/relaunch.py` & `martin_binance-3.0.7/martin_binance/service/relaunch.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.6/martin_binance/strategy_base.py` & `martin_binance-3.0.7/martin_binance/strategy_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 martin-binance base class and methods definitions
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "3.0.6"
+__version__ = "3.0.7"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 import ast
 import asyncio
 import csv
 import logging
@@ -47,15 +47,15 @@
 if prm.MODE == 'S':
     logger = logging.getLogger('logger_S')
 else:
     logger = logging.getLogger('logger')
 
 color_init()
 
-RATE_LIMITER = HEARTBEAT * 5
+RATE_LIMITER = HEARTBEAT * (60 if prm.GRID_ONLY else 10)
 KLINES_LIM = 50  # Number of candles must be <= 1000
 CANCEL_ALL_ORDERS = True  # Ask about cancel all active orders before start strategy and par.LOAD_LAST_STATE = 0
 TRADES_LIST_LIMIT = 50
 TRY_LIMIT = 30
 PYARROW_BATCH_BUFFER_SIZE = 20480  # Rows
 ORDER_BOOK_PRKT = "order_book.parquet"
 TICKER_PRKT = "ticker.parquet"
@@ -1027,14 +1027,15 @@
         else:
             for i in _intervals:
                 self.tasks_manage(self.aiter_candles(_klines, i), name='wss')
 
     async def create_limit_order(self, _id: int, buy: bool, amount: str, price: str) -> None:
         self.wait_order_id.append(_id)
         _fetch_order = False
+        msg = None
         try:
             if prm.MODE in ('T', 'TC'):
                 ts = time.time()
                 res = await self.send_request(
                     self.stub.create_limit_order, mr.CreateLimitOrderRequest,
                     symbol=self.symbol,
                     buy_side=buy,
@@ -1055,34 +1056,38 @@
                     lt=int(self.get_time() * 1000)
                 )
         except asyncio.CancelledError:
             pass  # Task cancellation should not be logged as an error
         except GRPCError as ex:
             status_code = ex.status
             if status_code == Status.FAILED_PRECONDITION:
+                self.message_log(f"Order {_id}: {status_code.name}, {ex.message}")
                 if _id in self.wait_order_id:
                     # Supress call strategy handler
                     self.wait_order_id.remove(_id)
             else:
                 _fetch_order = True
-            self.on_place_order_error(_id, f"{status_code.name}, {ex.message}")
+            msg = f"Create order {_id}: {status_code.name}, {ex.message}"
         except Exception as _ex:
             _fetch_order = True
-            self.message_log(f"Exception creating order {_id}: {_ex}")
+            msg = f"Exception creating order {_id}: {_ex}"
         else:
             if result:
                 await self.create_order_handler(_id, result)
             else:
                 _fetch_order = True
+                msg = f"Creating order {_id}: no result getting"
         finally:
             if prm.MODE in ('T', 'TC') and _fetch_order:
                 await asyncio.sleep(HEARTBEAT)
                 res = await self.fetch_order(0, str(_id), _filled_update_call=True)
                 if res.get('status') in ('NEW', 'PARTIALLY_FILLED', 'FILLED'):
                     await self.create_order_handler(_id, res)
+                else:
+                    self.on_place_order_error(_id, msg)
 
     async def create_order_handler(self, _id, result):
         # print(f"create_order_handler.result: {result}")
         if _id in self.wait_order_id and not self.order_exist(result['orderId']):
             self.wait_order_id.remove(_id)
             order = Order(result)
             self.message_log(
@@ -1374,15 +1379,15 @@
                 restore = True
             except GRPCError as ex_3:
                 status_code = ex_3.status
                 self.message_log(f"Exception buffered_orders 3: {status_code.name}, {ex_3.message}",
                                  log_level=logging.WARNING, color=Style.B_RED, tlg=True)
                 if status_code == Status.RESOURCE_EXHAUSTED:
                     # Decrease requests frequency
-                    self.rate_limiter += HEARTBEAT
+                    self.rate_limiter += HEARTBEAT * 5
                     self.message_log(f"RATE_LIMITER set to {self.rate_limiter}s", log_level=logging.WARNING)
                     await asyncio.sleep(ORDER_TIMEOUT)
                     try:
                         await self.send_request(self.stub.reset_rate_limit, mr.OpenClientConnectionId,
                                                 rate_limiter=self.rate_limiter)
                     except Exception as ex_4:
                         self.message_log(f"Exception buffered_orders 4:ResetRateLimit: {ex_4}",
```

### Comparing `martin_binance-3.0.6/martin_binance/telegram_utils.py` & `martin_binance-3.0.7/martin_binance/telegram_utils.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.6/martin_binance/templates/cli_0_BTCUSDT.py` & `martin_binance-3.0.7/martin_binance/templates/cli_0_BTCUSDT.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.6/martin_binance/templates/cli_1_BTCUSDT.py` & `martin_binance-3.0.7/martin_binance/templates/cli_1_BTCUSDT.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.6/martin_binance/templates/cli_2_TESTBTCTESTUSDT.py` & `martin_binance-3.0.7/martin_binance/templates/cli_2_TESTBTCTESTUSDT.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.6/martin_binance/templates/cli_3_BTCUSDT.py` & `martin_binance-3.0.7/martin_binance/templates/cli_3_BTCUSDT.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.6/martin_binance/templates/funds_rate.db` & `martin_binance-3.0.7/martin_binance/templates/funds_rate.db`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.6/martin_binance/templates/ms_cfg.toml` & `martin_binance-3.0.7/martin_binance/templates/ms_cfg.toml`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.6/martin_binance/templates/trial_params.json` & `martin_binance-3.0.7/martin_binance/templates/trial_params.json`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.6/pyproject.toml` & `martin_binance-3.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
              "Operating System :: Unix",
              "Operating System :: Microsoft :: Windows",
              "Operating System :: MacOS"]
 dynamic = ["version", "description"]
 requires-python = ">=3.9"
 
 dependencies = [
-    "exchanges-wrapper==2.1.11",
+    "exchanges-wrapper==2.1.12",
     "jsonpickle==3.0.2",
     "psutil==5.9.6",
     "requests==2.31.0",
     "libtmux==0.23.2",
     "colorama==0.4.6",
     "prometheus-client==0.18.0",
     "optuna==3.4.0",
```

### Comparing `martin_binance-3.0.6/PKG-INFO` & `martin_binance-3.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: martin-binance
-Version: 3.0.6
+Version: 3.0.7
 Summary: Free trading system for Binance SPOT API
 Author-email: Jerry Fedorenko <jerry.fedorenko@yahoo.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
-Requires-Dist: exchanges-wrapper==2.1.11
+Requires-Dist: exchanges-wrapper==2.1.12
 Requires-Dist: jsonpickle==3.0.2
 Requires-Dist: psutil==5.9.6
 Requires-Dist: requests==2.31.0
 Requires-Dist: libtmux==0.23.2
 Requires-Dist: colorama==0.4.6
 Requires-Dist: prometheus-client==0.18.0
 Requires-Dist: optuna==3.4.0
@@ -71,14 +71,16 @@
 
 >Valid: (BTC/USDT), (ETH/BUSD), (SOL/LTC)
 > 
 >Incorrectly: (BTC/USDT), (ETH/USDT), (BTC/ETH)
 > 
 >As a result of the mutual impact on the operating balance sheet, the liquidity control system will block the work.
 
+* Due to a limitation in the implementation of asyncio under Windows, this program cannot be executed. [Use Docker on Windows instead.](https://github.com/DogsTailFarmer/martin-binance/wiki/Quick-start#docker)
+
 ## References
 * Detailed information about use this strategy placed to [wiki](https://github.com/DogsTailFarmer/martin-binance/wiki)
 * [Trade idea](https://github.com/DogsTailFarmer/martin-binance/wiki/Trade-idea)
 * [Quick start](https://github.com/DogsTailFarmer/martin-binance/wiki/Quick-start)
 * [Back testing and parameters optimization](https://github.com/DogsTailFarmer/martin-binance/wiki/Back-testing-and-parameters-optimization)
 
 ## Referral link
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: martin-binance Version: 3.0.6 Summary: Free trading
+Metadata-Version: 2.1 Name: martin-binance Version: 3.0.7 Summary: Free trading
 system for Binance SPOT API Author-email: Jerry Fedorenko
 yahoo.com> Requires-Python: >=3.9 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3 Classifier: Development Status
 :: 5 - Production/Stable Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix Classifier: Operating System :: Microsoft
 :: Windows Classifier: Operating System :: MacOS Requires-Dist: exchanges-
-wrapper==2.1.11 Requires-Dist: jsonpickle==3.0.2 Requires-Dist: psutil==5.9.6
+wrapper==2.1.12 Requires-Dist: jsonpickle==3.0.2 Requires-Dist: psutil==5.9.6
 Requires-Dist: requests==2.31.0 Requires-Dist: libtmux==0.23.2 Requires-Dist:
 colorama==0.4.6 Requires-Dist: prometheus-client==0.18.0 Requires-Dist:
 optuna==3.4.0 Requires-Dist: plotly==5.18.0 Requires-Dist: pandas==2.1.2
 Requires-Dist: dash>=2.15.0 Requires-Dist: future==0.18.3 Requires-Dist:
 inquirer==3.1.3 Requires-Dist: scikit-learn==1.3.2 Requires-Dist: tqdm==4.66.1
 Requires-Dist: ujson~=5.9.0 Requires-Dist: orjson~=3.9.15 Requires-Dist:
 pyarrow~=14.0.2 Requires-Dist: shortuuid~=1.0.11 Requires-Dist: numpy~=1.23.4
@@ -33,21 +33,24 @@
 strategy lie with you. Strongly recommended that you test the strategy in the
 demo mode before using real bidding. ## Important notices * After update to
 `3.0.1`, the configuration files `cli_XX_AAABBB.py` for all running trading
 pairs should be updated. Use templates for reference. * You cannot run multiple
 pairs with overlapping currencies on the same account! >Valid: (BTC/USDT),
 (ETH/BUSD), (SOL/LTC) > >Incorrectly: (BTC/USDT), (ETH/USDT), (BTC/ETH) > >As a
 result of the mutual impact on the operating balance sheet, the liquidity
-control system will block the work. ## References * Detailed information about
-use this strategy placed to [wiki](https://github.com/DogsTailFarmer/martin-
-binance/wiki) * [Trade idea](https://github.com/DogsTailFarmer/martin-binance/
-wiki/Trade-idea) * [Quick start](https://github.com/DogsTailFarmer/martin-
-binance/wiki/Quick-start) * [Back testing and parameters optimization](https://
-github.com/DogsTailFarmer/martin-binance/wiki/Back-testing-and-parameters-
-optimization) ## Referral link
+control system will block the work. * Due to a limitation in the implementation
+of asyncio under Windows, this program cannot be executed. [Use Docker on
+Windows instead.](https://github.com/DogsTailFarmer/martin-binance/wiki/Quick-
+start#docker) ## References * Detailed information about use this strategy
+placed to [wiki](https://github.com/DogsTailFarmer/martin-binance/wiki) *
+[Trade idea](https://github.com/DogsTailFarmer/martin-binance/wiki/Trade-idea)
+* [Quick start](https://github.com/DogsTailFarmer/martin-binance/wiki/Quick-
+start) * [Back testing and parameters optimization](https://github.com/
+DogsTailFarmer/martin-binance/wiki/Back-testing-and-parameters-optimization) ##
+Referral link
 Create account on [Binance](https://accounts.binance.com/en/
 register?ref=QCS4OGWR) and get 10% discount on all trading fee Create account
 on [HUOBI](https://www.huobi.com/en-us/topic/double-reward/
 ?invite_code=9uaw3223) and will get 50 % off trading fees Create account on
 [Bitfinex](https://www.bitfinex.com/sign-up?refcode=v_4az2nCP) and get 6%
 rebate fee Create account on [OKEX](https://www.okex.com/join/2607649) and get
 Mystery Boxes worth up to $10,000 Create account on [Bybit](https://
```

