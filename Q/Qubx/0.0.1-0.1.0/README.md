# Comparing `tmp/qubx-0.0.1.tar.gz` & `tmp/qubx-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qubx-0.0.1.tar", max compression
+gzip compressed data, was "qubx-0.1.0.tar", max compression
```

## Comparing `qubx-0.0.1.tar` & `qubx-0.1.0.tar`

### file list

```diff
@@ -1,25 +1,34 @@
--rw-r--r--   0        0        0      213 2024-02-29 14:43:31.699720 qubx-0.0.1/README.md
--rw-r--r--   0        0        0     9312 2024-02-29 14:43:31.699720 qubx-0.0.1/build.py
--rw-r--r--   0        0        0     1315 2024-02-29 14:43:31.739720 qubx-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     5133 2024-02-29 14:43:31.739720 qubx-0.0.1/src/qubx/__init__.py
--rw-r--r--   0        0        0     2357 2024-02-29 14:43:31.739720 qubx-0.0.1/src/qubx/_nb_magic.py
--rw-r--r--   0        0        0        0 2024-02-29 14:43:31.739720 qubx-0.0.1/src/qubx/core/__init__.py
--rw-r--r--   0        0        0    10251 2024-02-29 14:43:31.739720 qubx-0.0.1/src/qubx/core/basics.py
--rw-r--r--   0        0        0     6284 2024-02-29 14:43:31.739720 qubx-0.0.1/src/qubx/core/lookups.py
--rw-r--r--   0        0        0     2283 2024-02-29 14:43:31.739720 qubx-0.0.1/src/qubx/core/series.pxd
--rw-r--r--   0        0        0    25097 2024-02-29 14:43:31.739720 qubx-0.0.1/src/qubx/core/series.pyx
--rw-r--r--   0        0        0     2342 2024-02-29 14:43:31.739720 qubx-0.0.1/src/qubx/core/strategy.py
--rw-r--r--   0        0        0     1368 2024-02-29 14:43:31.739720 qubx-0.0.1/src/qubx/core/utils.pyx
--rw-r--r--   0        0        0    14928 2024-02-29 14:43:31.739720 qubx-0.0.1/src/qubx/data/readers.py
--rw-r--r--   0        0        0       33 2024-02-29 14:43:31.739720 qubx-0.0.1/src/qubx/math/__init__.py
--rw-r--r--   0        0        0     1176 2024-02-29 14:43:31.739720 qubx-0.0.1/src/qubx/math/stats.py
--rw-r--r--   0        0        0        0 2024-02-29 14:43:31.739720 qubx-0.0.1/src/qubx/ta/__init__.py
--rw-r--r--   0        0        0     7708 2024-02-29 14:43:31.739720 qubx-0.0.1/src/qubx/ta/indicators.pyx
--rw-r--r--   0        0        0      283 2024-02-29 14:43:31.739720 qubx-0.0.1/src/qubx/utils/__init__.py
--rw-r--r--   0        0        0    11894 2024-02-29 14:43:31.739720 qubx-0.0.1/src/qubx/utils/_pyxreloader.py
--rw-r--r--   0        0        0     5937 2024-02-29 14:43:31.739720 qubx-0.0.1/src/qubx/utils/charting/mpl_helpers.py
--rw-r--r--   0        0        0     9162 2024-02-29 14:43:31.739720 qubx-0.0.1/src/qubx/utils/marketdata/binance.py
--rw-r--r--   0        0        0     6908 2024-02-29 14:43:31.739720 qubx-0.0.1/src/qubx/utils/misc.py
--rw-r--r--   0        0        0     7281 2024-02-29 14:43:31.739720 qubx-0.0.1/src/qubx/utils/pandas.py
--rw-r--r--   0        0        0     4604 2024-02-29 14:43:31.739720 qubx-0.0.1/src/qubx/utils/time.py
--rw-r--r--   0        0        0     1292 1970-01-01 00:00:00.000000 qubx-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      940 2024-04-25 07:51:17.473695 qubx-0.1.0/README.md
+-rw-r--r--   0        0        0     9305 2024-04-21 10:35:06.164526 qubx-0.1.0/build.py
+-rw-r--r--   0        0        0     1338 2024-04-25 07:51:17.477695 qubx-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5428 2024-04-21 10:35:06.176526 qubx-0.1.0/src/qubx/__init__.py
+-rw-r--r--   0        0        0     1730 2024-04-25 07:51:17.477695 qubx-0.1.0/src/qubx/_nb_magic.py
+-rw-r--r--   0        0        0        0 2024-02-29 14:43:31.739720 qubx-0.1.0/src/qubx/core/__init__.py
+-rw-r--r--   0        0        0     6707 2024-04-25 07:51:17.477695 qubx-0.1.0/src/qubx/core/account.py
+-rw-r--r--   0        0        0    14763 2024-04-25 07:51:17.477695 qubx-0.1.0/src/qubx/core/basics.py
+-rw-r--r--   0        0        0    11899 2024-04-25 07:51:17.477695 qubx-0.1.0/src/qubx/core/loggers.py
+-rw-r--r--   0        0        0    13688 2024-04-21 10:35:06.176526 qubx-0.1.0/src/qubx/core/lookups.py
+-rw-r--r--   0        0        0     2847 2024-04-21 10:35:06.176526 qubx-0.1.0/src/qubx/core/series.pxd
+-rw-r--r--   0        0        0    28108 2024-04-21 10:35:06.176526 qubx-0.1.0/src/qubx/core/series.pyx
+-rw-r--r--   0        0        0    25029 2024-04-25 07:51:17.477695 qubx-0.1.0/src/qubx/core/strategy.py
+-rw-r--r--   0        0        0     1368 2024-02-29 14:43:31.739720 qubx-0.1.0/src/qubx/core/utils.pyx
+-rw-r--r--   0        0        0    15531 2024-04-21 10:35:06.176526 qubx-0.1.0/src/qubx/data/readers.py
+-rw-r--r--   0        0        0     9013 2024-04-25 07:51:17.481695 qubx-0.1.0/src/qubx/impl/ccxt_connector.py
+-rw-r--r--   0        0        0     9092 2024-04-25 07:51:17.481695 qubx-0.1.0/src/qubx/impl/ccxt_trading.py
+-rw-r--r--   0        0        0     3488 2024-04-21 10:35:06.176526 qubx-0.1.0/src/qubx/impl/exchange_customizations.py
+-rw-r--r--   0        0        0     3565 2024-04-25 07:51:17.481695 qubx-0.1.0/src/qubx/impl/utils.py
+-rw-r--r--   0        0        0       33 2024-02-29 14:43:31.739720 qubx-0.1.0/src/qubx/math/__init__.py
+-rw-r--r--   0        0        0     1176 2024-02-29 14:43:31.739720 qubx-0.1.0/src/qubx/math/stats.py
+-rw-r--r--   0        0        0        0 2024-02-29 14:43:31.739720 qubx-0.1.0/src/qubx/ta/__init__.py
+-rw-r--r--   0        0        0     7708 2024-02-29 14:43:31.739720 qubx-0.1.0/src/qubx/ta/indicators.pyx
+-rw-r--r--   0        0        0       60 2024-04-21 10:35:06.176526 qubx-0.1.0/src/qubx/trackers/__init__.py
+-rw-r--r--   0        0        0     5522 2024-04-21 10:35:06.176526 qubx-0.1.0/src/qubx/trackers/rebalancers.py
+-rw-r--r--   0        0        0      262 2024-04-21 10:35:06.176526 qubx-0.1.0/src/qubx/utils/__init__.py
+-rw-r--r--   0        0        0    12076 2024-04-21 10:35:06.176526 qubx-0.1.0/src/qubx/utils/_pyxreloader.py
+-rw-r--r--   0        0        0     5937 2024-02-29 14:43:31.739720 qubx-0.1.0/src/qubx/utils/charting/mpl_helpers.py
+-rw-r--r--   0        0        0    10999 2024-04-21 10:35:06.176526 qubx-0.1.0/src/qubx/utils/marketdata/binance.py
+-rw-r--r--   0        0        0     9821 2024-04-25 07:51:17.481695 qubx-0.1.0/src/qubx/utils/misc.py
+-rw-r--r--   0        0        0    18583 2024-04-21 10:35:06.176526 qubx-0.1.0/src/qubx/utils/pandas.py
+-rw-r--r--   0        0        0     8656 2024-04-25 07:51:17.481695 qubx-0.1.0/src/qubx/utils/runner.py
+-rw-r--r--   0        0        0     4604 2024-02-29 14:43:31.739720 qubx-0.1.0/src/qubx/utils/time.py
+-rw-r--r--   0        0        0     2062 1970-01-01 00:00:00.000000 qubx-0.1.0/PKG-INFO
```

### Comparing `qubx-0.0.1/build.py` & `qubx-0.1.0/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,15 +149,15 @@
 
     print("Copied all compiled dynamic library files into source")
 
 
 def _strip_unneeded_symbols() -> None:
     try:
         print("Stripping unneeded symbols from binaries...")
-        for so in itertools.chain(Path("nautilus_trader").rglob("*.so")):
+        for so in itertools.chain(Path("src/qubx").rglob("*.so")):
             if platform.system() == "Linux":
                 strip_cmd = ["strip", "--strip-unneeded", so]
             elif platform.system() == "Darwin":
                 strip_cmd = ["strip", "-x", so]
             else:
                 raise RuntimeError(f"Cannot strip symbols for platform {platform.system()}")
             subprocess.run(
```

### Comparing `qubx-0.0.1/pyproject.toml` & `qubx-0.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 [tool.poetry]
 name = "Qubx"
-version = "0.0.1"
+version = "0.1.0"
 description = "Qubx - quantitative trading framework"
 authors = ["Dmitry Marienko <dmitry@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "qubx", from = "src" },
 ]
 repository = "https://github.com/dmarienko/Qubx"
 include = [
     # Compiled extensions must be included in the wheel distributions
     { path = "src/**/*.so", format = "wheel" },
     { path = "src/**/*.pyd", format = "wheel" },
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.9,<4.0"
+python = ">=3.10,<4.0"
 pytest = {extras = ["lazyfixture"], version = "^7.2.0"}
 numpy = "^1.26.3"
 ntplib = "^0.4.0"
 loguru = "^0.7.2"
+tqdm = "*"
+importlib-metadata = "*"
 stackprinter = "^0.2.10"
-#websocket-client = "^1.6.3"
-#websockets = "^11.0.3"
 pymongo = "^4.6.1"
 pydantic = "^1.10.2"
 python-dotenv = "^1.0.0"
 python-binance = "^1.0.19"
 pyarrow = "^15.0.0"
 scipy = "^1.12.0"
 cython = "3.0.8"
+ccxt = "^4.2.68"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^2.20.0"
 pytest = "^7.1.3"
 
 #[project.optional-dependencies]
 #numba = "^0.57.1"
+ipykernel = "^6.29.4"
 
 [build-system]
 requires = ["poetry-core", "setuptools", "numpy>=1.26.3", "cython==3.0.8", "toml>=0.10.2",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.build]
 script = "build.py"
```

### Comparing `qubx-0.0.1/src/qubx/__init__.py` & `qubx-0.1.0/src/qubx/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from qubx.utils import set_mpl_theme, runtime_env, install_pyx_recompiler_for_dev
-install_pyx_recompiler_for_dev()
+from qubx.utils import set_mpl_theme, runtime_env
+from qubx.utils.misc import install_pyx_recompiler_for_dev
 
 from loguru import logger
 import os, sys, stackprinter
-from qubx.core.lookups import InstrumentsLookup
+from qubx.core.lookups import FeesLookup, GlobalLookup, InstrumentsLookup
 
 
 def formatter(record):
     end = record["extra"].get("end", "\n")
     fmt = "<lvl>{message}</lvl>%s" % end
     if record["level"].name in {"WARNING", "SNAKY"}:
         fmt = "<cyan>{name}</cyan>:<cyan>{function}</cyan>:<cyan>{line}</cyan> - %s" % fmt
@@ -32,43 +32,49 @@
 
 
 logger.configure(**config)
 logger.remove(None)
 logger.add(sys.stdout, format=formatter, colorize=True)
 logger = logger.opt(colors=True)
 
-lookup = InstrumentsLookup()
+# - global lookup helper
+lookup = GlobalLookup(InstrumentsLookup(), FeesLookup())
+
 
 # registering magic for jupyter notebook
 if runtime_env() in ['notebook', 'shell']:
     from IPython.core.magic import (Magics, magics_class, line_magic, line_cell_magic)
     from IPython import get_ipython
 
     @magics_class
     class QubxMagics(Magics):
         # process data manager
         __manager = None
 
         @line_magic
         def qubxd(self, line: str):
-            self.qubx_setup('dark')
+            self.qubx_setup('dark' + ' ' + line)
 
         @line_magic
         def qubxl(self, line: str):
-            self.qubx_setup('light')
+            self.qubx_setup('light' + ' ' + line)
 
         @line_magic
         def qubx_setup(self, line: str):
             """
-            QUBE framework initialization
+            QUBX framework initialization
             """
             import os
+            args = [x.strip() for x in line.split(' ')]
+            
+            # setup cython dev hooks - only if 'dev' is passed as argument
+            if line and 'dev' in args: 
+                install_pyx_recompiler_for_dev()
 
             tpl_path = os.path.join(os.path.dirname(__file__), "_nb_magic.py")
-            # print("TPL:", tpl_path)
             with open(tpl_path, 'r', encoding="utf8") as myfile:
                 s = myfile.read()
 
             exec(s, self.shell.user_ns)
 
             # setup more funcy mpl theme instead of ugly default
             if line:
```

### Comparing `qubx-0.0.1/src/qubx/_nb_magic.py` & `qubx-0.1.0/src/qubx/_nb_magic.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """"
 Here stuff we want to have in every Jupyter notebook after calling %qube magic
 """
 import importlib_metadata
 
 import qubx
 from qubx.utils import runtime_env
-from qubx.utils.misc import add_project_to_system_path
+from qubx.utils.misc import add_project_to_system_path, logo
 
 
 def np_fmt_short():
     # default np output is 75 columns so extend it a bit and suppress scientific fmt for small floats
     np.set_printoptions(linewidth=240, suppress=True)
 
 
@@ -42,28 +42,12 @@
 
     # - setup short numpy output format
     np_fmt_short()
     
     # - add project home to system path
     add_project_to_system_path()
 
-    # - check current version
-    try: 
-        version = importlib_metadata.version('qube2')
-    except:
-        version = 'Dev'
-
-    # some new logo
+    # show logo first time
     if not hasattr(qubx.QubxMagics, '__already_initialized__'):
-        from qubx.utils.misc import (green, yellow, cyan, magenta, white, blue, red)
-
-        print(
-        f"""
-                   {red("╻")}
-   {green("┏┓      ╻     ")}  {red("┃")}  {yellow("┏┓")}       {cyan("Quantitative Backtesting Environment")} 
-   {green("┃┃  ┓┏  ┣┓  ┏┓")}  {red("┃")}  {yellow("┏┛")}       
-   {green("┗┻  ┗┻  ┗┛  ┗ ")}  {red("┃")}  {yellow("┗━")}       (c) 2024,  ver. {magenta(version.rstrip())}
-                   {red("╹")}       
-"""
-        )
-        qubx.QubxMagics.__already_initialized__ = True
+        setattr(qubx.QubxMagics, "__already_initialized__", True)
+        logo()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `qubx-0.0.1/src/qubx/core/basics.py` & `qubx-0.1.0/src/qubx/core/basics.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 from datetime import datetime
 from typing import Callable, Dict, List, Optional, Union
 import numpy as np
+import pandas as pd
 import math
 from dataclasses import dataclass, field
+
+import asyncio
+# from multiprocessing import Queue, Process, Event, Lock
+from threading import Thread, Event, Lock
+from queue import Queue
+
 from qubx.core.series import Quote, Trade, time_as_nsec
 from qubx.core.utils import time_to_str, time_delta_to_str, recognize_timeframe
 
 
 dt_64 = np.datetime64
+td_64 = np.timedelta64
 
 
 @dataclass
 class FuturesInfo:
     contract_type: Optional[str] = None             # contract type  
     delivery_date: Optional[datetime] = None        # delivery date
     onboard_date: Optional[datetime] = None         # futures contract size
@@ -76,83 +84,159 @@
     stop: Optional[float] = None
     take: Optional[float] = None
     group: Optional[str] = None 
     comment: Optional[str] = None
 
 
 class TransactionCostsCalculator:
-    def __init__(self, maker: float, taker: float):
-        self.maker = maker
-        self.taker = taker
+    """
+    A class for calculating transaction costs for a trading strategy.
+    Attributes
+    ----------
+    name : str
+        The name of the transaction costs calculator.
+    maker : float
+        The maker fee, as a percentage of the transaction value.
+    taker : float
+        The taker fee, as a percentage of the transaction value.
+
+    """
+    name: str
+    maker: float
+    taker: float
+
+    def __init__(self, name: str, maker: float, taker: float):
+        self.name = name
+        self.maker = maker / 100.0
+        self.taker = taker / 100.0
 
     def get_execution_fees(self, instrument: Instrument, exec_price: float, amount: float, crossed_market=False, conversion_rate=1.0):
         if crossed_market:
             return abs(amount * exec_price) * self.taker / conversion_rate
         else:
             return abs(amount * exec_price) * self.maker / conversion_rate
 
     def get_overnight_fees(self, instrument: Instrument, amount: float):
         return 0.0
 
     def get_funding_rates_fees(self, instrument: Instrument, amount: float):
         return 0.0
 
     def __repr__(self):
-        return f'<TCC: {self.maker * 100:.4f} / {self.taker * 100:.4f}>'
+        return f'<{self.name}: {self.maker * 100:.4f} / {self.taker * 100:.4f}>'
+
 
+ZERO_COSTS = TransactionCostsCalculator('Zero', 0.0, 0.0)
 
-ZERO_COSTS = TransactionCostsCalculator(0.0, 0.0)
+
+@dataclass
+class Deal:
+    id: str | int         # trade id
+    order_id: str | int   # order's id
+    time: dt_64           # time of trade
+    amount: float         # signed traded amount: positive for buy and negative for selling
+    price: float
+    aggressive: bool
+    fee_amount: float | None = None
+    fee_currency: str | None = None
+
+
+@dataclass
+class Order:
+    id: str
+    type: str
+    symbol: str
+    time: dt_64
+    quantity: float
+    price: float
+    side: str
+    status: str
+    time_in_force: str
+    client_id: str | None = None
+    cost: float = 0.0
+    
+    def __str__(self) -> str:
+        return f"[{self.id}] {self.type} {self.side} {self.quantity} of {self.symbol} {('@ ' + str(self.price)) if self.price > 0 else ''} ({self.time_in_force}) [{self.status}]"
+
+
+def round_down(x, n):
+    dvz = 10**(-n)
+    return (int(x / dvz)) * dvz
 
 
 class Position:
     instrument: Instrument                      # instrument for this poisition
     quantity: float = 0.0                       # quantity positive for long and negative for short
     tcc: TransactionCostsCalculator             # transaction costs calculator
     pnl: float = 0.0                            # total cumulative position PnL in portfolio basic funds currency
     r_pnl: float = 0.0                          # total cumulative position PnL in portfolio basic funds currency
     market_value: float = 0.0                   # position's market value in quote currency
     market_value_funds: float = 0.0             # position market value in portfolio funded currency
     position_avg_price: float = 0.0             # average position price
     position_avg_price_funds: float = 0.0       # average position price
     commissions: float = 0.0                    # cumulative commissions paid for this position
 
-    last_update_time: Optional[int] = None      # when price updated or position changed
-    last_update_price: Optional[float] = None   # last update price (actually instrument's price) in quoted currency
+    last_update_time: int = np.nan              # when price updated or position changed
+    last_update_price: float = np.nan           # last update price (actually instrument's price) in quoted currency
+    last_update_conversion_rate: float = np.nan # last update conversion rate
 
     # - helpers for position processing 
     _formatter: str
     _prc_formatter: str
     _qty_multiplier: float = 1.0
+    __pos_incr_qty: float = 0
 
     def __init__(self, instrument: Instrument, tcc: TransactionCostsCalculator, 
-                 quantity=0.0, average_price=0.0, aux_price=1.0, 
+                 quantity=0.0, pos_average_price=0.0, r_pnl=0.0
                  ) -> None:
         self.instrument = instrument
         self.tcc = tcc
         
         # - size/price formaters
         #                 time         [symbol]                                                        qty                                                  
         self._formatter = f'%s [{instrument.exchange}:{instrument.symbol}] %{instrument.size_precision+8}.{instrument.size_precision}f'
         #                           pos_avg_px                 pnl  | mkt_price mkt_value
         self._formatter += f'%10.{instrument.price_precision}f %+10.4f | %s  %10.2f'
         self._prc_formatter = f"%.{instrument.price_precision}f"
         if instrument.is_futures:
-            self._qty_multiplier = instrument.futures_info.contract_size
+            self._qty_multiplier = instrument.futures_info.contract_size # type: ignore
 
-        if quantity != 0.0 and average_price > 0.0:
+        self.reset()
+        if quantity != 0.0 and pos_average_price > 0.0:
             self.quantity = quantity
-            raise ValueError("[TODO] Position: restore state by quantity and avg price !!!!")
+            self.position_avg_price = pos_average_price
+            self.r_pnl = r_pnl
 
-    def _price(self, update: Union[Quote, Trade]) -> float:
+    def reset(self):
+        """
+        Reset position to zero
+        """
+        self.quantity = 0.0
+        self.pnl = 0.0
+        self.r_pnl = 0.0
+        self.market_value = 0.0
+        self.market_value_funds = 0.0
+        self.position_avg_price = 0.0
+        self.position_avg_price_funds = 0.0
+        self.commissions = 0.0
+        self.last_update_time = np.nan # type: ignore
+        self.last_update_price = np.nan
+        self.last_update_conversion_rate = np.nan
+        self.__pos_incr_qty = 0
+
+    def _price(self, update: Quote | Trade) -> float:
         if isinstance(update, Quote):
             return update.bid if np.sign(self.quantity) > 0 else update.ask
         elif isinstance(update, Trade):
             return update.price
         raise ValueError(f"Unknown update type: {type(update)}")
 
+    def change_position_by(self, timestamp: dt_64, amount: float, exec_price: float, aggressive=True, conversion_rate:float=1) -> float:
+        return self.update_position(timestamp, self.quantity + amount, exec_price, aggressive=aggressive, conversion_rate=conversion_rate)
+
     def update_position(self, timestamp: dt_64, position: float, exec_price: float, aggressive=True, conversion_rate:float=1) -> float:
         # - realized PnL of this fill
         deal_pnl = 0
         quantity = self.quantity
 
         if quantity != position:
             pos_change = position - quantity
@@ -167,58 +251,105 @@
             if qty_closing != 0:
                 deal_pnl = qty_closing * (self.position_avg_price - exec_price)
                 quantity += qty_closing
                 # - reset average price to 0 if smaller than minimal price change to avoid cumulative error
                 if abs(quantity) < self.instrument.min_size_step:
                     quantity = 0.0
                     self.position_avg_price = 0.0
+                    self.__pos_incr_qty = 0
 
             # - if it has something to add to position let's update price and cost
             if qty_opening != 0:
-                qa_open, qas = abs(qty_opening), abs(quantity)
-                self.position_avg_price = (qa_open * exec_price + qas * self.position_avg_price) / (qas + qa_open)
+                _abs_qty_open = abs(qty_opening)
+                pos_avg_price_raw = (_abs_qty_open * exec_price + self.__pos_incr_qty * self.position_avg_price) / (self.__pos_incr_qty + _abs_qty_open)
+                # - round position average price to be in line with how it's calculated by broker
+                self.position_avg_price = round_down(pos_avg_price_raw, self.instrument.price_precision)
+                self.__pos_incr_qty += _abs_qty_open
 
             # - update position and position's price
             self.position_avg_price_funds = self.position_avg_price / conversion_rate
             self.quantity = position
 
             # - convert PnL to fund currency
             self.r_pnl += deal_pnl / conversion_rate
 
             # - update pnl
-            self._update_market_price(time_as_nsec(timestamp), exec_price, conversion_rate)
+            self.update_market_price(time_as_nsec(timestamp), exec_price, conversion_rate)
 
             # - calculate transaction costs
             comms = self.tcc.get_execution_fees(self.instrument, exec_price, pos_change, aggressive, conversion_rate)
             self.commissions += comms
 
         return deal_pnl
 
-    def update_market_price(self, price: Union[Quote, Trade], conversion_rate:float=1) -> float:
-        return self._update_market_price(price.time, self._price(price), conversion_rate)
+    def update_market_price_by_tick(self, tick: Quote | Trade, conversion_rate:float=1) -> float:
+        return self.update_market_price(tick.time, self._price(tick), conversion_rate)
+
+    def update_position_by_deal(self, deal: Deal, conversion_rate:float=1) -> float:
+        time = deal.time.as_unit('ns').asm8 if isinstance(deal.time, pd.Timestamp) else deal.time
+        return self.change_position_by(time, deal.amount, deal.price, deal.aggressive, conversion_rate)
+        # - deal contains cumulative amount
+        # return self.update_position(time, deal.amount, deal.price, deal.aggressive, conversion_rate)
 
-    def _update_market_price(self, timestamp: dt_64, price: float, conversion_rate:float) -> float:
-        self.last_update_time = timestamp
+    def update_market_price(self, timestamp: dt_64, price: float, conversion_rate:float) -> float:
+        self.last_update_time = timestamp # type: ignore
         self.last_update_price = price
+        self.last_update_conversion_rate = conversion_rate
 
         if not np.isnan(price):
             self.pnl = self.quantity * (price - self.position_avg_price) / conversion_rate + self.r_pnl
             self.market_value = self.quantity * self.last_update_price * self._qty_multiplier
 
             # calculate mkt value in funded currency
             self.market_value_funds = self.market_value / conversion_rate
         return self.pnl
 
-    def total_pnl(self, conversion_rate:float=1.0) -> float:
+    def total_pnl(self) -> float:
         pnl = self.r_pnl
-        if not np.isnan(self.last_update_price):
-            pnl += self.quantity * (self.last_update_price - self.position_avg_price) / conversion_rate
+        if not np.isnan(self.last_update_price): # type: ignore
+            pnl += self.quantity * (self.last_update_price - self.position_avg_price) / self.last_update_conversion_rate # type: ignore
         return pnl
 
+    def get_amount_released_funds_after_closing(self, to_remain: float = 0.0) -> float:
+        """
+        Estimate how much funds would be released if part of position closed
+        """
+        d = np.sign(self.quantity)
+        funds_release = self.market_value_funds
+        if to_remain != 0 and self.quantity != 0 and np.sign(to_remain) == d:
+            qty_to_release = max(self.quantity - to_remain, 0) if d > 0 else min(self.quantity - to_remain, 0)
+            funds_release = qty_to_release * self.last_update_price / self.last_update_conversion_rate
+        return abs(funds_release)
+
     @staticmethod
     def _t2s(t) -> str:
-        return np.datetime64(t, 'ns').astype('datetime64[ms]').item().strftime('%Y-%m-%d %H:%M:%S') if t else '---'
+        return np.datetime64(t, 'ns').astype('datetime64[ms]').item().strftime('%Y-%m-%d %H:%M:%S') if not np.isnan(t) else '???'
 
     def __str__(self):
         _mkt_price = (self._prc_formatter % self.last_update_price) if self.last_update_price else "---"
         return self._formatter % (Position._t2s(self.last_update_time), self.quantity, self.position_avg_price_funds,self.pnl, _mkt_price,  self.market_value_funds)
     
+
+class CtrlChannel:
+    """
+    Controlled data communication channel
+    """
+    control: Event
+    queue: Queue     # we need something like disruptor here (Queue is temporary)
+    name: str
+    lock: Lock
+
+    def __init__(self, name: str, sent=(None, None)):
+        self.name = name
+        self.control = Event()
+        self.queue = Queue()
+        self.lock = Lock()
+        self.sent = sent
+        self.start()
+
+    def stop(self):
+        if self.control.is_set():
+            self.control.clear()
+            self.queue.put(self.sent) # send sentinel
+
+    def start(self):
+        self.control.set()
```

### Comparing `qubx-0.0.1/src/qubx/core/series.pxd` & `qubx-0.1.0/src/qubx/core/series.pxd`

 * *Files 20% similar despite different names*

```diff
@@ -16,14 +16,17 @@
     cdef public Indexed times
     cdef public Indexed values
     cdef float max_series_length
     cdef unsigned short _is_new_item
     cdef public str name
     cdef dict indicators        # it's used for indicators caching
     cdef list calculation_order # calculation order as list: [ (input_id, indicator_obj, indicator_id) ]
+    cdef double _process_every_update
+    cdef double _last_bar_update_value
+    cdef long long _last_bar_update_time
 
     cdef _update_indicators(TimeSeries self, long long time, object value, short new_item_started)
 
 
 cdef class Indicator(TimeSeries):
     cdef TimeSeries series
     cdef TimeSeries parent
@@ -44,51 +47,57 @@
 
 cdef class Bar:
     cdef public long long time
     cdef public double open
     cdef public double high
     cdef public double low
     cdef public double close
-    cdef public double volume
+    cdef public double volume          # total volume (in quote asset)
+    cdef public double bought_volume   # volume bought (in quote asset) if presented
 
-    cpdef Bar update(Bar self, double price, double volume)
+    cpdef Bar update(Bar self, double price, double volume, double bought_volume=*)
 
     cpdef dict to_dict(Bar self, unsigned short skip_time=*)
 
 
 cdef class OHLCV(TimeSeries):
     cdef public TimeSeries open
     cdef public TimeSeries high
     cdef public TimeSeries low
     cdef public TimeSeries close
     cdef public TimeSeries volume
+    cdef public TimeSeries bvolume
 
-    cpdef short update(OHLCV self, long long time, double price, double volume=*)
+    cpdef short update(OHLCV self, long long time, double price, double volume=*, double bvolume=*)
+
+    cpdef short update_by_bar(OHLCV self, long long time, double open, double high, double low, double close, double vol_incr=*, double b_vol_incr=*)
 
     cpdef _update_indicators(OHLCV self, long long time, object value, short new_item_started)
 
     cpdef object append_data(
         OHLCV self, 
         np.ndarray times, 
         np.ndarray opens,
         np.ndarray highs, 
         np.ndarray lows,
         np.ndarray closes, 
-        np.ndarray volumes
+        np.ndarray volumes,
+        np.ndarray bvolumes
     )
 
 
 cdef class Trade:
     cdef public long long time
     cdef public double price
     cdef public double size
     cdef public short taker
+    cdef public long long trade_id
 
 
 cdef class Quote:
     cdef public long long time
-    cdef public bid
-    cdef public ask
-    cdef public bid_size
-    cdef public ask_size
+    cdef public double bid
+    cdef public double ask
+    cdef public double bid_size
+    cdef public double ask_size
 
     cpdef double mid_price(Quote self)
```

### Comparing `qubx-0.0.1/src/qubx/core/series.pyx` & `qubx-0.1.0/src/qubx/core/series.pyx`

 * *Files 6% similar despite different names*

```diff
@@ -118,29 +118,35 @@
 
 
 global _plot_func
 
 
 cdef class TimeSeries:
 
-    def __init__(self, str name, timeframe, max_series_length=INFINITY) -> None:
+    def __init__(
+        self, str name, timeframe, max_series_length=INFINITY, 
+        process_every_update=True, # calculate indicators on every update (tick) - by default
+    ) -> None:
         self.name = name
         self.max_series_length = max_series_length
         self.timeframe = recognize_timeframe(timeframe)
         self.times = Indexed(max_series_length)
         self.values = Indexed(max_series_length)
         self.indicators = dict()
         self.calculation_order = []
 
+        # - processing every update
+        self._process_every_update = process_every_update
+        self._last_bar_update_value = np.nan
+        self._last_bar_update_time = -1
+
     def __len__(self) -> int:
         return len(self.times)
 
-    def _lift_up(self, indicator: Indicator, indicator_input: TimeSeries):
-        # print(f"> Received: {indicator_input.name}[{id(indicator_input)}] -> {indicator.name}[{id(indicator)}]")
-        # collect indicators calculation order as list: [ (input_id, indicator_obj, indicator_id) ]
+    def _on_attach_indicator(self, indicator: Indicator, indicator_input: TimeSeries):
         self.calculation_order.append((
             id(indicator_input), indicator, id(indicator)
         ))
 
     def __getitem__(self, idx):
         return self.values[idx]
 
@@ -163,23 +169,36 @@
             # - disable first notification because first item may be incomplete
             self._is_new_item = False
 
         elif time - self.times[0] >= self.timeframe:
             # - add new item
             self._add_new_item(item_start_time, value)
 
-            # - update indicators
-            self._update_indicators(item_start_time, value, True)
+            # - if it's needed to process every tick in indicator
+            if self._process_every_update:
+                self._update_indicators(item_start_time, value, True)
+            else:
+                # - it's required to update indicators only on closed (formed) bar
+                self._update_indicators(self._last_bar_update_time, self._last_bar_update_value, True)
+
+            # - store last data
+            self._last_bar_update_time = item_start_time
+            self._last_bar_update_value = value
 
             return self._is_new_item
         else:
             self._update_last_item(item_start_time, value)
 
         # - update indicators by new data
-        self._update_indicators(item_start_time, value, False)
+        if self._process_every_update:
+            self._update_indicators(item_start_time, value, False)
+
+        # - store last data
+        self._last_bar_update_time = item_start_time
+        self._last_bar_update_value = value
 
         return self._is_new_item
 
     cdef _update_indicators(self, long long time, value, short new_item_started):
         mem = dict()              # store calculated values during this update
         mem[id(self)] = value     # initail value - new data from itself
         for input, indicator, iid in self.calculation_order:
@@ -288,21 +307,23 @@
         super().__init__(name, series.timeframe, series.max_series_length)
         series.indicators[name] = self
         self.name = name
 
         # - we need to make a empty copy and fill it 
         self.series = TimeSeries(series.name, series.timeframe, series.max_series_length)
         self.parent = series 
-        self._lift_up(self, series)
+        
+        # - notify the parent series that indicator has been attached
+        self._on_attach_indicator(self, series)
 
         # - recalculate indicator on data as if it would being streamed
         self._initial_data_recalculate(series)
 
-    def _lift_up(self, indicator: Indicator, indicator_input: TimeSeries):
-        self.parent._lift_up(indicator, indicator_input)
+    def _on_attach_indicator(self, indicator: Indicator, indicator_input: TimeSeries):
+        self.parent._on_attach_indicator(indicator, indicator_input)
 
     def _initial_data_recalculate(self, TimeSeries series):
         for t, v in zip(series.times[::-1], series.values[::-1]):
             self.update(t, v, True)
 
     def update(self, long long time, value, short new_item_started) -> object:
         if new_item_started or len(self) == 0:
@@ -542,24 +563,26 @@
 
 
 def neg(series: TimeSeries):
     return Neg.wrap(series)
 
 
 cdef class Trade:
-    def __init__(self, time, double price, double size, short taker=-1):
+    def __init__(self, time, double price, double size, short taker=-1, long long trade_id=0):
         self.time = time_as_nsec(time)
         self.price = price
         self.size = size
         self.taker = taker
+        self.trade_id = trade_id
 
     def __repr__(self):
-        return "[%s]\t%.5f (%.1f) <%s>" % ( 
+        return "[%s]\t%.5f (%.1f) <%s> %s" % ( 
             time_to_str(self.time, 'ns'), self.price, self.size, 
-            'take' if self.taker == 1 else 'make' if self.taker == 0 else '???'
+            'take' if self.taker == 1 else 'make' if self.taker == 0 else '???',
+            str(self.trade_id) if self.trade_id > 0 else ''
         ) 
 
 
 cdef class Quote:
     def __init__(self, time, double bid, double ask, double bid_size, double ask_size):
         self.time = time_as_nsec(time)
         self.bid = bid
@@ -574,35 +597,42 @@
         return "[%s]\t%.5f (%.1f) | %.5f (%.1f)" % (
             time_to_str(self.time, 'ns'), self.bid, self.bid_size, self.ask, self.ask_size
         )
 
 
 cdef class Bar:
 
-    def __init__(self, long long time, double open, double high, double low, double close, double volume) -> None:
+    def __init__(self, long long time, double open, double high, double low, double close, double volume, double bought_volume=0) -> None:
+        self.time = time
         self.open = open
         self.high = high
         self.low = low
         self.close = close
         self.volume = volume
+        self.bought_volume = bought_volume
 
-    cpdef Bar update(self, double price, double volume):
+    cpdef Bar update(self, double price, double volume, double bought_volume=0):
         self.close = price
         self.high = max(price, self.high)
         self.low = min(price, self.low)
         self.volume += volume
+        self.bought_volume += bought_volume
         return self
 
     cpdef dict to_dict(self, unsigned short skip_time=0):
         if skip_time:
             return {
-                'open': self.open, 'high': self.high, 'low': self.low, 'close': self.close, 'volume': self.volume,
+                'open': self.open, 'high': self.high, 'low': self.low, 'close': self.close,
+                'volume': self.volume, 'bought_volume': self.bought_volume,
             }
         return {
-            'timestamp': np.datetime64(self.time, 'ns'), 'open': self.open, 'high': self.high, 'low': self.low, 'close': self.close, 'volume': self.volume,
+            'timestamp': np.datetime64(self.time, 'ns'), 
+            'open': self.open, 'high': self.high, 'low': self.low, 'close': self.close, 
+            'volume': self.volume,
+            'bought_volume': self.bought_volume,
         }
 
     def __repr__(self):
         return "{o:%f | h:%f | l:%f | c:%f | v:%f}" % (self.open, self.high, self.low, self.close, self.volume)
 
 
 cdef class OHLCV(TimeSeries):
@@ -610,30 +640,33 @@
     def __init__(self, str name, timeframe, max_series_length=INFINITY) -> None:
         super().__init__(name, timeframe, max_series_length)
         self.open = TimeSeries('open', timeframe, max_series_length)
         self.high = TimeSeries('high', timeframe, max_series_length)
         self.low = TimeSeries('low', timeframe, max_series_length)
         self.close = TimeSeries('close', timeframe, max_series_length)
         self.volume = TimeSeries('volume', timeframe, max_series_length)
+        self.bvolume = TimeSeries('bvolume', timeframe, max_series_length)
 
     cpdef object append_data(self, 
                     np.ndarray times, 
                     np.ndarray opens,
                     np.ndarray highs,
                     np.ndarray lows,
                     np.ndarray closes,
                     np.ndarray volumes,
+                    np.ndarray bvolumes
                 ):
         cdef long long t
         cdef short _conv
         cdef short _upd_inds, _has_vol
         cdef Bar b 
 
         # - check if volume data presented
         _has_vol = len(volumes) > 0
+        _has_bvol = len(bvolumes) > 0
 
         # - check if need to convert time to nanosec
         _conv = 0
         if not isinstance(times[0].item(), long):
             _conv = 1
 
         # - check if need to update any indicators
@@ -650,15 +683,17 @@
 
         for i in range(len(times)):
             if _conv:
                 t = times[i].astype('datetime64[ns]').item()
             else:
                 t = times[i].item()
 
-            b = Bar(t, opens[i], highs[i], lows[i], closes[i], volumes[i] if _has_vol else 0)
+            b = Bar(t, opens[i], highs[i], lows[i], closes[i], 
+                    volumes[i] if _has_vol else 0, 
+                    bvolumes[i] if _has_bvol else 0)
             self._add_new_item(t, b)
 
             if _upd_inds:
                 self._update_indicators(t, b, True)
 
         return self
 
@@ -666,54 +701,91 @@
         self.times.add(time)
         self.values.add(value)
         self.open._add_new_item(time, value.open)
         self.high._add_new_item(time, value.high)
         self.low._add_new_item(time, value.low)
         self.close._add_new_item(time, value.close)
         self.volume._add_new_item(time, value.volume)
+        self.bvolume._add_new_item(time, value.bought_volume)
         self._is_new_item = True
 
     def _update_last_item(self, long long time, Bar value):
         self.times.update_last(time)
         self.values.update_last(value)
         self.open._update_last_item(time, value.open)
         self.high._update_last_item(time, value.high)
         self.low._update_last_item(time, value.low)
         self.close._update_last_item(time, value.close)
         self.volume._update_last_item(time, value.volume)
+        self.bvolume._update_last_item(time, value.bought_volume)
         self._is_new_item = False
 
-    cpdef short update(self, long long time, double price, double volume=0.0):
+    cpdef short update(self, long long time, double price, double volume=0.0, double bvolume=0.0):
         cdef Bar b
         bar_start_time = floor_t64(time, self.timeframe)
 
         if not self.times:
-            self._add_new_item(bar_start_time, Bar(bar_start_time, price, price, price, price, volume))
+            self._add_new_item(bar_start_time, Bar(bar_start_time, price, price, price, price, volume, bvolume))
 
             # Here we disable first notification because first item may be incomplete
             self._is_new_item = False
 
         elif time - self.times[0] >= self.timeframe:
-            b = Bar(bar_start_time, price, price, price, price, volume)
+            b = Bar(bar_start_time, price, price, price, price, volume, bvolume)
 
             # - add new item
             self._add_new_item(bar_start_time, b)
 
             # - update indicators
             self._update_indicators(bar_start_time, b, True)
 
             return self._is_new_item
         else:
-            self._update_last_item(bar_start_time, self[0].update(price, volume))
+            self._update_last_item(bar_start_time, self[0].update(price, volume, bvolume))
 
         # - update indicators by new data
         self._update_indicators(bar_start_time, self[0], False)
 
         return self._is_new_item
 
+    cpdef short update_by_bar(self, long long time, double open, double high, double low, double close, double vol_incr=0.0, double b_vol_incr=0.0):
+        cdef Bar b
+        cdef Bar l_bar
+        bar_start_time = floor_t64(time, self.timeframe)
+
+        if not self.times:
+            self._add_new_item(bar_start_time, Bar(bar_start_time, open, high, low, close, vol_incr, b_vol_incr))
+
+            # Here we disable first notification because first item may be incomplete
+            self._is_new_item = False
+
+        elif time - self.times[0] >= self.timeframe:
+            b = Bar(bar_start_time, open, high, low, close, vol_incr, b_vol_incr)
+
+            # - add new item
+            self._add_new_item(bar_start_time, b)
+
+            # - update indicators
+            self._update_indicators(bar_start_time, b, True)
+
+            return self._is_new_item
+        else:
+            l_bar = self[0]
+            l_bar.high = max(high, l_bar.high)
+            l_bar.low = min(low, l_bar.low)
+            l_bar.close = close
+            l_bar.volume += vol_incr
+            l_bar.bought_volume += b_vol_incr
+            self._update_last_item(bar_start_time, l_bar)
+
+        # # - update indicators by new data
+        self._update_indicators(bar_start_time, self[0], False)
+
+        return self._is_new_item
+
     # - TODO: need to check if it's safe to drop value series (series of Bar) to avoid duplicating data
     # def __getitem__(self, idx):
     #     if isinstance(idx, slice):
     #         return [
     #             Bar(self.times[i], self.open[i], self.high[i], self.low[i], self.close[i], self.volume[i])
     #             for i in range(*idx.indices(len(self.times)))
     #         ]
@@ -730,15 +802,16 @@
 
     def to_series(self) -> pd.DataFrame:
         df = pd.DataFrame({
             'open': self.open.to_series(),
             'high': self.high.to_series(),
             'low': self.low.to_series(),
             'close': self.close.to_series(),
-            'volume': self.volume.to_series(),
+            'volume': self.volume.to_series(),         # total volume
+            'bought_volume': self.bvolume.to_series(), # bought volume
         })
         df.index.name = 'timestamp'
         return df
 
     def to_records(self) -> dict:
         ts = [np.datetime64(t, 'ns') for t in self.times[::-1]]
         bs = [v.to_dict(skip_time=True) for v in self.values[::-1]]
```

### Comparing `qubx-0.0.1/src/qubx/core/utils.pyx` & `qubx-0.1.0/src/qubx/core/utils.pyx`

 * *Files identical despite different names*

### Comparing `qubx-0.0.1/src/qubx/data/readers.py` & `qubx-0.1.0/src/qubx/data/readers.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pyarrow import csv
 
 from qubx import logger
 from qubx.core.series import TimeSeries, OHLCV, time_as_nsec, Quote, Trade
 from qubx.utils.time import infer_series_frequency, handle_start_stop
 
 _DT = lambda x: pd.Timedelta(x).to_numpy().item()
-D1, H1 = _DT('1D'), _DT('1H')
+D1, H1 = _DT('1D'), _DT('1h')
 
 DEFAULT_DAILY_SESSION = (_DT('00:00:00.100'), _DT('23:59:59.900'))
 STOCK_DAILY_SESSION = (_DT('9:30:00.100'), _DT('15:59:59.900'))
 CME_FUTURES_DAILY_SESSION = (_DT('8:30:00.100'), _DT('15:14:59.900'))
 
 
 def _recognize_t(t: Union[int, str], defaultvalue, timeunit) -> int:
@@ -208,34 +208,39 @@
     def start_processing(self, fieldnames: List[str]):
         self._time_idx = _find_column_index_in_list(fieldnames, 'time', 'timestamp', 'datetime', 'date')
         self._open_idx = _find_column_index_in_list(fieldnames, 'open')
         self._high_idx = _find_column_index_in_list(fieldnames, 'high')
         self._low_idx = _find_column_index_in_list(fieldnames, 'low')
         self._close_idx = _find_column_index_in_list(fieldnames, 'close')
         self._volume_idx = None
+        self._b_volume_idx = None
         self._timeframe = None
 
         try:
-            self._volume_idx = _find_column_index_in_list(fieldnames, 'volume', 'vol')
-        except:
-            pass
+            self._volume_idx = _find_column_index_in_list(fieldnames, 'quote_volume', 'volume', 'vol')
+        except: pass
+
+        try:
+            self._b_volume_idx = _find_column_index_in_list(fieldnames, 'taker_buy_volume', 'taker_buy_quote_volume', 'buy_volume')
+        except: pass
 
         self.ohlc = None
 
     def process_data(self, data: list) -> Optional[Iterable]:
         if self._timeframe is None:
             self._timeframe = infer_series_frequency(data[self._time_idx]).astype('timedelta64[s]')
 
             # - create instance after first data received
             self.ohlc = OHLCV(self._name, self._timeframe)
 
         self.ohlc.append_data(
             data[self._time_idx],
             data[self._open_idx], data[self._high_idx], data[self._low_idx], data[self._close_idx], 
-            data[self._volume_idx] if self._volume_idx else []
+            data[self._volume_idx] if self._volume_idx else np.empty(0),
+            data[self._b_volume_idx] if self._b_volume_idx else np.empty(0)
         )
         return None
 
     def get_result(self) -> Any:
         return self.ohlc
 
 
@@ -249,29 +254,34 @@
     def start_processing(self, fieldnames: List[str]):
         self._time_idx = _find_column_index_in_list(fieldnames, 'time', 'timestamp', 'datetime', 'date')
         self._open_idx = _find_column_index_in_list(fieldnames, 'open')
         self._high_idx = _find_column_index_in_list(fieldnames, 'high')
         self._low_idx = _find_column_index_in_list(fieldnames, 'low')
         self._close_idx = _find_column_index_in_list(fieldnames, 'close')
         self._volume_idx = None
+        self._b_volume_idx = None
         self._timeframe = None
 
         try:
-            self._volume_idx = _find_column_index_in_list(fieldnames, 'volume', 'vol')
-        except:
-            pass
+            self._volume_idx = _find_column_index_in_list(fieldnames, 'quote_volume', 'volume', 'vol')
+        except: pass
+
+        try:
+            self._b_volume_idx = _find_column_index_in_list(fieldnames, 'taker_buy_volume', 'taker_buy_quote_volume', 'buy_volume')
+        except: pass
 
         # self.ohlc = pd.DataFrame()
 
         self._time = np.array([], dtype=np.datetime64)
         self._open = np.array([])
         self._high = np.array([])
         self._low = np.array([])
         self._close = np.array([])
         self._volume = np.array([])
+        self._bvolume = np.array([])
 
     def process_data(self, data: list) -> Optional[Iterable]:
         # p = pd.DataFrame({
         #     'open': data[self._open_idx], 
         #     'high': data[self._high_idx], 
         #     'low': data[self._low_idx], 
         #     'close': data[self._close_idx], 
@@ -282,39 +292,39 @@
         self._time = np.concatenate((self._time, data[self._time_idx]))
         self._open = np.concatenate((self._open, data[self._open_idx]))
         self._high = np.concatenate((self._high, data[self._high_idx]))
         self._low = np.concatenate((self._low, data[self._low_idx]))
         self._close = np.concatenate((self._close, data[self._close_idx]))
         if self._volume_idx:
             self._volume = np.concatenate((self._volume, data[self._volume_idx]))
+        if self._b_volume_idx:
+            self._bvolume = np.concatenate((self._bvolume, data[self._b_volume_idx]))
 
         return None
 
     def get_result(self) -> Any:
-        # self.ohlc.index.name = 'time'
-        # return self.ohlc
+        rd = {
+            'open': self._open, 'high': self._high, 'low': self._low, 'close': self._close, 
+        }
+
+        if self._volume_idx:
+            rd['volume'] = self._volume
+
+        if self._b_volume_idx:
+            rd['taker_buy_quote_volume'] = self._bvolume
 
-        return pd.DataFrame(
-            {
-                'open': self._open, 
-                'high': self._high, 
-                'low': self._low, 
-                'close': self._close, 
-                'volume': self._volume if self._volume_idx else []
-            },
-            index = self._time
-        ).sort_index()
+        return pd.DataFrame(rd, index = self._time).sort_index()
  
 
 class CsvDataReader(DataReader):
     """
     CSV data file reader
     """
 
-    def __init__(self, path: str, processor: DataProcessor=None, timestamp_parsers=None) -> None:
+    def __init__(self, path: str, processor: DataProcessor|None=None, timestamp_parsers=None) -> None:
         if not exists(path):
             raise ValueError(f"CSV file not found at {path}")
         super().__init__(processor)
         self.time_parsers = timestamp_parsers
         self.path = path
 
     def __find_time_idx(self, arr: pa.ChunkedArray, v) -> int:
```

### Comparing `qubx-0.0.1/src/qubx/math/stats.py` & `qubx-0.1.0/src/qubx/math/stats.py`

 * *Files identical despite different names*

### Comparing `qubx-0.0.1/src/qubx/ta/indicators.pyx` & `qubx-0.1.0/src/qubx/ta/indicators.pyx`

 * *Files identical despite different names*

### Comparing `qubx-0.0.1/src/qubx/utils/_pyxreloader.py` & `qubx-0.1.0/src/qubx/utils/_pyxreloader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,19 @@
-import importlib, glob, imp, os, sys
+
+import importlib, glob, os, sys
 from importlib.abc import MetaPathFinder
 from importlib.util import spec_from_file_location
 from importlib.machinery import ExtensionFileLoader, SourceFileLoader
 from typing import List
 
+# - disable warn about deprecation of imp module: after dev stage _pyxreloader will be removed
+import warnings
+warnings.filterwarnings("ignore", category=DeprecationWarning)
+import imp
+
 PYX_EXT = ".pyx"
 PYXDEP_EXT = ".pyxdep"
 PYXBLD_EXT = ".pyxbld"
 
 
 def handle_dependencies(pyxfilename):
     testing = '_test_files' in globals()
```

### Comparing `qubx-0.0.1/src/qubx/utils/charting/mpl_helpers.py` & `qubx-0.1.0/src/qubx/utils/charting/mpl_helpers.py`

 * *Files identical despite different names*

### Comparing `qubx-0.0.1/src/qubx/utils/misc.py` & `qubx-0.1.0/src/qubx/utils/misc.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,38 @@
+from typing import Dict, Optional, Union, List
 import glob, os
-from collections import OrderedDict, namedtuple
+from collections import OrderedDict, defaultdict, namedtuple
 from os.path import basename, exists, dirname, join, expanduser
-from typing import Optional, Union
+import time
 from pathlib import Path
 
 
 def version() -> str:
     # - check current version
     version = 'Dev'
     try: 
         import importlib_metadata
-        version = importlib_metadata.version('qube2')
+        version = importlib_metadata.version('qubx')
     except:
         pass
 
     return version
 
 
-from ._pyxreloader import pyx_install_loader
-
 def install_pyx_recompiler_for_dev():
-    if version().lower() == 'dev':
-        print(f" >  [{green('dev')}] {red('installed cython rebuilding hook')}")
-        pyx_install_loader(['qubx.core', 'qubx.ta', 'qubx.data', 'qubx.strategies'])
+    from ._pyxreloader import pyx_install_loader
+
+    # if version().lower() == 'dev':
+    print(f" >  [{green('dev')}] {red('installing cython rebuilding hook')}")
+    pyx_install_loader([
+        'qubx.core', 
+        'qubx.ta', 
+        'qubx.data', 
+        'qubx.strategies'
+    ])
 
 
 def runtime_env():
     """
     Check what environment this script is being run under
     :return: environment name, possible values:
              - 'notebook' jupyter notebook
@@ -114,14 +120,27 @@
     __wrap_with_color('34'),
     __wrap_with_color('35'),
     __wrap_with_color('36'),
     __wrap_with_color('37'),
 )
 
 
+def logo():
+    """
+    Some fancy Qubx logo
+    """
+    print(f"""
+⠀⠀⡰⡖⠒⠒⢒⢦⠀⠀   
+⠀⢠⠃⠈⢆⣀⣎⣀⣱⡀  {red("QUBX")} | {cyan("Quantitative Backtesting Environment")} 
+⠀⢳⠒⠒⡞⠚⡄⠀⡰⠁         (c) 2024, ver. {magenta(version().rstrip())}
+⠀⠀⠱⣜⣀⣀⣈⣦⠃⠀⠀⠀ 
+        """ 
+    )
+
+
 class Struct:
     """
     Dynamic structure (similar to matlab's struct it allows to add new properties dynamically)
 
     >>> a = Struct(x=1, y=2)
     >>> a.z = 'Hello'
     >>> print(a)
@@ -227,8 +246,88 @@
         return m
 
 
 def makedirs(path: str, *args) -> str:
     path = os.path.expanduser(os.path.join(*[path, *args]))
     if not exists(path):
         os.makedirs(path)
-    return path
+    return path
+
+
+class Stopwatch:
+    """
+    Stopwatch timer for performance 
+    """
+    starts: Dict[str|None, int] = {} 
+    counts: Dict[str|None, int] = defaultdict(lambda: 0)
+    latencies: Dict[str|None, int] = {} 
+    
+    def __new__(cls):
+        if not hasattr(cls, 'instance'):
+            cls.instance = super(Stopwatch, cls).__new__(cls)
+        return cls.instance
+    
+    def start(self, scope: str | None):
+        self.starts[scope] = time.perf_counter_ns()
+        self.counts[scope] += 1
+        
+    def stop(self, scope: str|None=None) -> int | None:
+        t = time.perf_counter_ns()
+        s = self.starts.get(scope, None)
+        lat = None
+        if s:
+            lat = t - s
+            n = self.counts[scope]
+            self.latencies[scope] = (lat * (n - 1) + self.latencies.get(scope, lat)) // n
+            del self.starts[scope]
+        return lat
+
+    def latency_sec(self, scope: str | None) -> float:
+        return self.latencies.get(scope, 0) / 1e9
+
+    def watch(self, scope='global'):
+        def _decorator(func):
+            info = scope + '.' + func.__name__
+            def wrapper(*args, **kwargs):
+                self.start(info)
+                output = func(*args, **kwargs)
+                self.stop(info)
+                return output
+            return wrapper
+        return _decorator
+    
+    def reset(self):
+        self.starts.clear()
+        self.counts.clear()
+        self.latencies.clear()
+
+    def __str__(self) -> str:
+        r = ""
+        for l in self.latencies.keys():
+            r += f"\n\t<w>{l}</w> took <r>{self.latency_sec(l):.7f}</r> secs"
+        return r
+
+
+def quotify(sx: Union[str, List[str]], quote='USDT'):
+    """
+    Make XXX<quote> from anything if that anything doesn't end with <quote>
+    """
+    if isinstance(sx, str):
+        return (sx if sx.endswith(quote) else sx + quote).upper()
+    elif isinstance(sx, (list, set, tuple)):
+        return [quotify(s, quote) for s in sx]
+    raise ValueError("Can't process input data !")
+
+
+def dequotify(sx: Union[str, List[str]], quote='USDT'):
+    """
+    Turns XXX<quote> to XXX (reverse of quotify)
+    """
+    if isinstance(sx, str):
+        quote = quote.upper()
+        if (s:=sx.upper()).endswith(quote):
+            s = s.split(':')[1] if ':' in s else s # remove exch: if presented
+            return s.split(quote)[0]
+    elif isinstance(sx, (list, set, tuple)):
+        return [dequotify(s, quote) for s in sx]
+
+    raise ValueError("Can't process input data !")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `qubx-0.0.1/src/qubx/utils/time.py` & `qubx-0.1.0/src/qubx/utils/time.py`

 * *Files identical despite different names*

