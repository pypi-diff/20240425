# Comparing `tmp/pyield-0.7.6.tar.gz` & `tmp/pyield-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyield-0.7.6.tar", last modified: Tue Apr 23 10:03:02 2024, max compression
+gzip compressed data, was "pyield-0.7.7.tar", last modified: Thu Apr 25 00:26:44 2024, max compression
```

## Comparing `pyield-0.7.6.tar` & `pyield-0.7.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1072 2023-12-14 08:54:49.496702 pyield-0.7.6/LICENSE
--rw-r--r--   0        0        0     6467 2024-04-21 17:20:40.545037 pyield-0.7.6/README.md
--rw-r--r--   0        0        0       22 2024-04-23 10:00:53.888741 pyield-0.7.6/pyield/__about__.py
--rw-r--r--   0        0        0      422 2024-04-20 13:36:59.541311 pyield-0.7.6/pyield/__init__.py
--rw-r--r--   0        0        0    13136 2024-04-13 12:39:44.026704 pyield-0.7.6/pyield/bday.py
--rw-r--r--   0        0        0     6073 2024-04-21 13:45:50.722682 pyield-0.7.6/pyield/data_access.py
--rw-r--r--   0        0        0     1276 2024-04-17 08:50:12.086620 pyield-0.7.6/pyield/data_analysis.py
--rw-r--r--   0        0        0      333 2024-04-21 13:45:50.722682 pyield-0.7.6/pyield/futures/__init__.py
--rw-r--r--   0        0        0     7564 2024-04-22 23:37:56.705516 pyield-0.7.6/pyield/futures/common.py
--rw-r--r--   0        0        0     4888 2024-04-23 09:52:39.684729 pyield-0.7.6/pyield/futures/ddi.py
--rw-r--r--   0        0        0     6840 2024-04-23 09:41:51.097815 pyield-0.7.6/pyield/futures/di.py
--rw-r--r--   0        0        0    11499 2024-04-19 11:12:40.009362 pyield-0.7.6/pyield/futures/di_xml.py
--rw-r--r--   0        0        0     3190 2024-04-21 16:43:54.862383 pyield-0.7.6/pyield/futures/frc.py
--rw-r--r--   0        0        0       55 2024-04-06 05:23:30.068485 pyield-0.7.6/pyield/holidays/__init__.py
--rw-r--r--   0        0        0    14278 2024-01-16 09:33:28.571746 pyield-0.7.6/pyield/holidays/br_holidays_new.txt
--rw-r--r--   0        0        0    14314 2023-12-28 23:26:42.737321 pyield-0.7.6/pyield/holidays/br_holidays_old.txt
--rw-r--r--   0        0        0     2192 2024-04-07 10:57:52.523509 pyield-0.7.6/pyield/holidays/core.py
--rw-r--r--   0        0        0     4268 2024-04-21 10:44:43.260419 pyield-0.7.6/pyield/indicators.py
--rw-r--r--   0        0        0     3395 2024-04-21 10:47:45.706989 pyield-0.7.6/pyield/projections.py
--rw-r--r--   0        0        0        0 2024-03-24 19:54:34.284748 pyield-0.7.6/pyield/py.typed
--rw-r--r--   0        0        0     6617 2024-04-21 13:41:53.731824 pyield-0.7.6/pyield/treasuries.py
--rw-r--r--   0        0        0     2190 2024-04-20 08:17:03.148377 pyield-0.7.6/pyield/utils.py
--rw-r--r--   0        0        0     1195 2024-04-23 10:03:02.864605 pyield-0.7.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-12-14 18:12:36.515393 pyield-0.7.6/tests/__init__.py
--rw-r--r--   0        0        0     1114 2024-04-16 12:01:55.676922 pyield-0.7.6/tests/test_bday.py
--rw-r--r--   0        0        0     2585 2024-04-22 23:45:59.541771 pyield-0.7.6/tests/test_futures.py
--rw-r--r--   0        0        0     8522 1970-01-01 00:00:00.000000 pyield-0.7.6/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-12-14 08:54:49.496702 pyield-0.7.7/LICENSE
+-rw-r--r--   0        0        0     6467 2024-04-21 17:20:40.545037 pyield-0.7.7/README.md
+-rw-r--r--   0        0        0       22 2024-04-25 00:10:29.617147 pyield-0.7.7/pyield/__about__.py
+-rw-r--r--   0        0        0      422 2024-04-20 13:36:59.541311 pyield-0.7.7/pyield/__init__.py
+-rw-r--r--   0        0        0    13136 2024-04-13 12:39:44.026704 pyield-0.7.7/pyield/bday.py
+-rw-r--r--   0        0        0     6091 2024-04-25 00:25:19.404158 pyield-0.7.7/pyield/data_access.py
+-rw-r--r--   0        0        0     1276 2024-04-17 08:50:12.086620 pyield-0.7.7/pyield/data_analysis.py
+-rw-r--r--   0        0        0      333 2024-04-21 13:45:50.722682 pyield-0.7.7/pyield/futures/__init__.py
+-rw-r--r--   0        0        0    10269 2024-04-25 00:06:20.078463 pyield-0.7.7/pyield/futures/common.py
+-rw-r--r--   0        0        0     3433 2024-04-24 23:25:56.361359 pyield-0.7.7/pyield/futures/ddi.py
+-rw-r--r--   0        0        0     5369 2024-04-24 23:27:06.122355 pyield-0.7.7/pyield/futures/di.py
+-rw-r--r--   0        0        0    11499 2024-04-19 11:12:40.009362 pyield-0.7.7/pyield/futures/di_xml.py
+-rw-r--r--   0        0        0     2185 2024-04-24 23:24:39.630264 pyield-0.7.7/pyield/futures/frc.py
+-rw-r--r--   0        0        0       55 2024-04-06 05:23:30.068485 pyield-0.7.7/pyield/holidays/__init__.py
+-rw-r--r--   0        0        0    14278 2024-01-16 09:33:28.571746 pyield-0.7.7/pyield/holidays/br_holidays_new.txt
+-rw-r--r--   0        0        0    14314 2023-12-28 23:26:42.737321 pyield-0.7.7/pyield/holidays/br_holidays_old.txt
+-rw-r--r--   0        0        0     2192 2024-04-07 10:57:52.523509 pyield-0.7.7/pyield/holidays/core.py
+-rw-r--r--   0        0        0     4268 2024-04-21 10:44:43.260419 pyield-0.7.7/pyield/indicators.py
+-rw-r--r--   0        0        0     3500 2024-04-25 00:22:37.836841 pyield-0.7.7/pyield/projections.py
+-rw-r--r--   0        0        0        0 2024-03-24 19:54:34.284748 pyield-0.7.7/pyield/py.typed
+-rw-r--r--   0        0        0     6617 2024-04-21 13:41:53.731824 pyield-0.7.7/pyield/treasuries.py
+-rw-r--r--   0        0        0     2190 2024-04-20 08:17:03.148377 pyield-0.7.7/pyield/utils.py
+-rw-r--r--   0        0        0     1195 2024-04-25 00:26:44.621381 pyield-0.7.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-12-14 18:12:36.515393 pyield-0.7.7/tests/__init__.py
+-rw-r--r--   0        0        0     1114 2024-04-16 12:01:55.676922 pyield-0.7.7/tests/test_bday.py
+-rw-r--r--   0        0        0     2585 2024-04-22 23:45:59.541771 pyield-0.7.7/tests/test_futures.py
+-rw-r--r--   0        0        0     8522 1970-01-01 00:00:00.000000 pyield-0.7.7/PKG-INFO
```

### Comparing `pyield-0.7.6/LICENSE` & `pyield-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyield-0.7.6/README.md` & `pyield-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `pyield-0.7.6/pyield/bday.py` & `pyield-0.7.7/pyield/bday.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.6/pyield/data_access.py` & `pyield-0.7.7/pyield/data_access.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         return it.fetch_di(reference_date=normalized_date)
     elif indicator_code.lower() == "vna_lft":
         return it.fetch_vna_selic(reference_date=normalized_date)
     else:
         raise ValueError("Indicator type not supported.")
 
 
-def fetch_projection(projection_code: str) -> dict:
+def fetch_projection(projection_code: str) -> pr.IndicatorProjection:
     """
     Fetches a financial projection for a specified code and reference date.
 
     Args:
         projection_code (str): The code for the financial projection. Supported options:
             - "IPCA_CM": IPCA projection for the current month from ANBIMA.
```

### Comparing `pyield-0.7.6/pyield/data_analysis.py` & `pyield-0.7.7/pyield/data_analysis.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.6/pyield/futures/ddi.py` & `pyield-0.7.7/pyield/futures/di.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,145 +1,160 @@
 import pandas as pd
 
-from . import common
+from .. import bday as bd
+from . import common as cm
 
 
-def _convert_prices_to_rates(prices: pd.Series, n_days: pd.Series) -> pd.Series:
+def _convert_prices_to_rates(prices: pd.Series, bd: pd.Series) -> pd.Series:
     """
-    Internal function to convert DDI futures prices to rates.
+    Internal function to convert DI futures prices to rates.
 
     Args:
-        prices (pd.Series): A pd.Series containing DDI futures prices.
-        bd (pd.Series): A serie containing the number of days to expiration.
+        prices (pd.Series): A pd.Series containing DI futures prices.
+        bd (pd.Series): A serie containing the number of business days to expiration.
 
     Returns:
-        pd.Series: A pd.Series containing DDI futures rates.
+        pd.Series: A pd.Series containing DI futures rates.
     """
-    rates = (100_000 / prices - 1) * (360 / n_days)
+    rates = (100_000 / prices) ** (252 / bd) - 1
+
     # Round to 5 (3 in %) dec. places (contract's current max. precision)
     return rates.round(5)
 
 
-def _process_raw_df(df: pd.DataFrame, trade_date: pd.Timestamp) -> pd.DataFrame:
+def _adjust_older_contracts_rates(df: pd.DataFrame, rate_cols: list) -> pd.DataFrame:
+    for col in rate_cols:
+        df[col] = _convert_prices_to_rates(df[col], df["BDaysToExp"])
+
+    # Invert low and high prices
+    df["MinRate"], df["MaxRate"] = df["MaxRate"], df["MinRate"]
+
+    return df
+
+
+def _process_past_raw_df(df: pd.DataFrame, trade_date: pd.Timestamp) -> pd.DataFrame:
     """
     Internal function to process and transform raw DI futures data.
 
     Args:
         df (pd.DataFrame): the raw DI DataFrame.
         trade_date: a datetime-like object representing the trade date.
 
     Returns:
         pd.DataFrame: Processed and transformed data as a Pandas pd.DataFrame.
     """
-    # Check if the pd.DataFrame is empty
-    if df.empty:
-        return df
-
-    rename_dict = {
-        "VENCTO": "ExpirationCode",
-        "CONTR. ABERT.(1)": "OpenContracts",  # At the start of the day
-        "CONTR. FECH.(2)": "OpenContractsEndSession",  # At the end of the day
-        "NÚM. NEGOC.": "TradeCount",
-        "CONTR. NEGOC.": "TradeVolume",
-        "VOL.": "FinancialVolume",
-        "AJUSTE": "SettlementPrice",
-        "AJUSTE ANTER. (3)": "PrevSettlementRate",
-        "AJUSTE CORRIG. (4)": "AdjSettlementRate",
-        "PREÇO MÍN.": "MinRate",
-        "PREÇO MÉD.": "AvgRate",
-        "PREÇO MÁX.": "MaxRate",
-        "PREÇO ABERTU.": "FirstRate",
-        "ÚLT. PREÇO": "LastRate",
-        "VAR. PTOS.": "PointsVariation",
-        # Attention: bid/ask rates are inverted
-        "ÚLT.OF. COMPRA": "LastAskRate",
-        "ÚLT.OF. VENDA": "LastBidRate",
-    }
-
-    df = df.rename(columns=rename_dict)
+    df = cm.rename_columns(df)
 
     df["TradeDate"] = trade_date
     # Convert to datetime64[ns] since it is pandas default type for timestamps
     df["TradeDate"] = df["TradeDate"].astype("datetime64[ns]")
 
     # Contract code format was changed in 22/05/2006
     if trade_date < pd.Timestamp("2006-05-22"):
         df["ExpirationDate"] = df["ExpirationCode"].apply(
-            common.get_old_expiration_date, args=(trade_date,)
+            cm.get_old_expiration_date, args=(trade_date,)
         )
     else:
-        df["ExpirationDate"] = df["ExpirationCode"].apply(common.get_expiration_date)
+        df["ExpirationDate"] = df["ExpirationCode"].apply(cm.get_expiration_date)
 
-    df["DaysToExp"] = (df["ExpirationDate"] - trade_date).dt.days
-    # Convert to nullable integer, since other columns use this data type
-    df["DaysToExp"] = df["DaysToExp"].astype(pd.Int64Dtype())
+    df["BDaysToExp"] = bd.count_bdays(trade_date, df["ExpirationDate"])
 
     # Remove expired contracts
-    df.query("DaysToExp > 0", inplace=True)
+    df.query("BDaysToExp > 0", inplace=True)
 
     # Columns where 0 means NaN
     rate_cols = [col for col in df.columns if "Rate" in col]
     cols_with_nan = rate_cols + ["SettlementPrice"]
     # Replace 0 with NaN in these columns
     df[cols_with_nan] = df[cols_with_nan].replace(0, pd.NA)
 
-    df[rate_cols] = df[rate_cols].div(100).round(5)
+    # Prior to 17/01/2002 (inclusive), prices were not converted to rates
+    if trade_date > pd.Timestamp("2002-01-17"):
+        # Remove % and round to 5 (3 in %) dec. places in rate columns
+        df[rate_cols] = df[rate_cols].div(100).round(5)
+    else:
+        df = _adjust_older_contracts_rates(df, rate_cols)
 
     # Calculate SettlementRate
     df["SettlementRate"] = _convert_prices_to_rates(
-        df["SettlementPrice"], df["DaysToExp"]
+        df["SettlementPrice"], df["BDaysToExp"]
     )
 
     df["TickerSymbol"] = "DI1" + df["ExpirationCode"]
 
     # Filter and order columns
-    ordered_cols = [
-        "TradeDate",
-        "ExpirationCode",
-        "ExpirationDate",
-        "DaysToExp",
-        "OpenContracts",
-        # "OpenContractsEndSession" since there is no OpenContracts at the end of the
-        # day in XML data, it will be removed to avoid confusion with XML data
-        "TradeCount",
-        "TradeVolume",
-        "FinancialVolume",
-        "SettlementPrice",
-        "MinRate",
-        "AvgRate",
-        "MaxRate",
-        "FirstRate",
-        "LastRate",
-        "LastAskRate",
-        "LastBidRate",
-        "SettlementRate",
-    ]
-    return df[ordered_cols]
+    df = cm.reorder_columns(df)
+    return df
+
+
+def _process_last_raw_di_df(raw_df: pd.DataFrame) -> pd.DataFrame:
+    df = raw_df.copy()
+
+    # Columns to be renamed
+    rename_columns = {
+        "TradeTimestamp": "TradeTimestamp",
+        "symb": "TickerSymbol",
+        "mtrtyCode": "ExpirationDate",
+        "BDaysToExp": "BDaysToExp",
+        "opnCtrcts": "OpenContracts",
+        "tradQty": "TradeCount",
+        "traddCtrctsQty": "TradeVolume",
+        "grssAmt": "FinancialVolume",
+        "prvsDayAdjstmntPric": "PrevSettlementRate",
+        "bottomLmtPric": "MinLimitRate",
+        "topLmtPric": "MaxLimitRate",
+        "opngPric": "OpenRate",
+        "minPric": "MinRate",
+        "avrgPric": "AvgRate",
+        "maxPric": "MaxRate",
+        "buyOffer.price": "LastAskRate",
+        "sellOffer.price": "LastBidRate",
+        "curPrc": "LastRate",
+    }
+    # Rename columns
+    df = df.rename(columns=rename_columns)
 
+    df["BDaysToExp"] = bd.count_bdays(df["TradeTimestamp"], df["ExpirationDate"])
 
-def fetch_past_ddi(trade_date: pd.Timestamp, return_raw: bool = False) -> pd.DataFrame:
+    # Remove percentage in all rate columns
+    rate_cols = [col for col in df.columns if "Rate" in col]
+    df[rate_cols] = df[rate_cols] / 100
+
+    # Reorder columns based on the order of the dictionary
+    return df[rename_columns.values()]
+
+
+def fetch_last_di() -> pd.DataFrame:
     """
-    Fetchs the DDI futures data for a given date from B3.
+    Fetch the latest DI futures data from B3.
+
+    Returns:
+        pd.DataFrame: A Pandas pd.DataFrame containing the latest DI futures data.
+    """
+    raw_df = cm.fetch_last_raw_df(future_code="DI1")
+    return _process_last_raw_di_df(raw_df)
+
+
+def fetch_past_di(trade_date: pd.Timestamp, return_raw: bool = False) -> pd.DataFrame:
+    """
+    Fetchs the DI futures data for a given date from B3.
 
     This function fetches and processes the DI futures data from B3 for a specific
-    trade date. It's the primary external interface for accessing DI data.
+    trade date. It's the primary external interface for accessing DI data. If the data
+    is not available, an empty DataFrame is returned.
 
     Args:
         trade_date (pd.Timestamp): The trade date to fetch the DI futures data.
-        raw (bool): If True, returns the raw data as a Pandas pd.DataFrame.
+        return_raw (bool): If True, returns the raw data as a Pandas pd.DataFrame.
             Defaults to False.
 
     Returns:
         pd.DataFrame: A Pandas pd.DataFrame containing processed DI futures data.
 
-    Examples:
-        >>> from pyield.futures import di
-        >>> di.fetch_ddi(pd.Timestamp("2021-01-04"))
-
     Notes:
-        - DaysToExp: number of business days to ExpirationDate.
+        - BDaysToExp: number of business days to ExpirationDate.
         - OpenContracts: number of open contracts at the start of the trading day.
     """
-    df_raw = common.fetch_past_raw_df(asset_code="DDI", trade_date=trade_date)
-    if return_raw:
+    df_raw = cm.fetch_past_raw_df(asset_code="DI1", trade_date=trade_date)
+    if return_raw or df_raw.empty:
         return df_raw
-    return _process_raw_df(df_raw, trade_date)
+    return _process_past_raw_df(df_raw, trade_date)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyield-0.7.6/pyield/futures/di_xml.py` & `pyield-0.7.7/pyield/futures/di_xml.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.6/pyield/futures/frc.py` & `pyield-0.7.7/pyield/futures/ddi.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,98 +1,101 @@
 import pandas as pd
 
-from . import common
+from . import common as cm
 
 
-def _process_past_data(df: pd.DataFrame, trade_date: pd.Timestamp) -> pd.DataFrame:
+def _convert_prices_to_rates(prices: pd.Series, n_days: pd.Series) -> pd.Series:
+    """
+    Internal function to convert DDI futures prices to rates.
+
+    Args:
+        prices (pd.Series): A pd.Series containing DDI futures prices.
+        bd (pd.Series): A serie containing the number of days to expiration.
+
+    Returns:
+        pd.Series: A pd.Series containing DDI futures rates.
+    """
+    rates = (100_000 / prices - 1) * (360 / n_days)
+    # Round to 5 (3 in %) dec. places (contract's current max. precision)
+    return rates.round(5)
+
+
+def _process_raw_df(df: pd.DataFrame, trade_date: pd.Timestamp) -> pd.DataFrame:
     """
     Internal function to process and transform raw DI futures data.
 
     Args:
         df (pd.DataFrame): the raw DI DataFrame.
         trade_date: a datetime-like object representing the trade date.
 
     Returns:
         pd.DataFrame: Processed and transformed data as a Pandas pd.DataFrame.
     """
-    # Check if the pd.DataFrame is empty
-    if df.empty:
-        return df
-
-    rename_dict = {
-        "VENCTO": "ExpirationCode",
-        "NÚM. NEGOC.": "TradeCount",
-        "CONTR. NEGOC.": "TradeVolume",
-        "VOL.": "FinancialVolume",
-        "AJUSTE  DE REF.": "SettlementRate",
-        "PREÇO ABERTU.": "FirstRate",
-        "PREÇO MÍN.": "MinRate",
-        "PREÇO MÉD.": "AvgRate",
-        "PREÇO MÁX.": "MaxRate",
-        "ÚLT. PREÇO": "CloseRate",
-        "VAR. PTOS.": "PointsVariation",
-        # Attention: bid/ask rates are inverted
-        "ÚLT.OF. COMPRA": "CloseAskRate",
-        "ÚLT.OF. VENDA": "CloseBidRate",
-    }
-
-    df = df.rename(columns=rename_dict)
+    df = cm.rename_columns(df)
 
     df["TradeDate"] = trade_date
     # Convert to datetime64[ns] since it is pandas default type for timestamps
     df["TradeDate"] = df["TradeDate"].astype("datetime64[ns]")
 
     # Contract code format was changed in 22/05/2006
     if trade_date < pd.Timestamp("2006-05-22"):
         df["ExpirationDate"] = df["ExpirationCode"].apply(
-            common.get_old_expiration_date, args=(trade_date,)
+            cm.get_old_expiration_date, args=(trade_date,)
         )
     else:
-        df["ExpirationDate"] = df["ExpirationCode"].apply(common.get_expiration_date)
+        df["ExpirationDate"] = df["ExpirationCode"].apply(cm.get_expiration_date)
+
+    df["DaysToExp"] = (df["ExpirationDate"] - trade_date).dt.days
+    # Convert to nullable integer, since other columns use this data type
+    df["DaysToExp"] = df["DaysToExp"].astype(pd.Int64Dtype())
 
-    # Replace 0 values in rate columns with pd.NA and remove percentage
+    # Remove expired contracts
+    df.query("DaysToExp > 0", inplace=True)
+
+    # Columns where 0 means NaN
     rate_cols = [col for col in df.columns if "Rate" in col]
-    # Round to 5 decimal places (3 in %) since it is the contract's precision
-    df[rate_cols] = df[rate_cols].replace(0, pd.NA).div(100).round(5)
+    cols_with_nan = rate_cols + ["SettlementPrice"]
+    # Replace 0 with NaN in these columns
+    df[cols_with_nan] = df[cols_with_nan].replace(0, pd.NA)
+
+    df[rate_cols] = df[rate_cols].div(100).round(5)
+
+    # Calculate SettlementRate
+    df["SettlementRate"] = _convert_prices_to_rates(
+        df["SettlementPrice"], df["DaysToExp"]
+    )
 
-    df["TickerSymbol"] = "FRC" + df["ExpirationCode"]
+    df["TickerSymbol"] = "DI1" + df["ExpirationCode"]
 
     # Filter and order columns
-    ordered_cols = [
-        "TradeDate",
-        "TickerSymbol",
-        # "ExpirationCode",
-        "ExpirationDate",
-        "TradeCount",
-        "TradeVolume",
-        "FinancialVolume",
-        "SettlementRate",
-        "FirstRate",
-        "MinRate",
-        "AvgRate",
-        "MaxRate",
-        "CloseAskRate",
-        "CloseBidRate",
-        "CloseRate",
-    ]
-    return df[ordered_cols]
+    df = cm.reorder_columns(df)
+
+    return df
 
 
-def fetch_past_frc(trade_date: pd.Timestamp, return_raw: bool = False) -> pd.DataFrame:
+def fetch_past_ddi(trade_date: pd.Timestamp, return_raw: bool = False) -> pd.DataFrame:
     """
-    Fetchs the DI futures data for a given date from B3.
+    Fetchs the DDI futures data for a given date from B3.
 
     This function fetches and processes the DI futures data from B3 for a specific
     trade date. It's the primary external interface for accessing DI data.
 
     Args:
         trade_date (pd.Timestamp): The trade date to fetch the DI futures data.
         raw (bool): If True, returns the raw data as a Pandas pd.DataFrame.
             Defaults to False.
 
     Returns:
         pd.DataFrame: A Pandas pd.DataFrame containing processed DI futures data.
+
+    Examples:
+        >>> from pyield.futures import di
+        >>> di.fetch_ddi(pd.Timestamp("2021-01-04"))
+
+    Notes:
+        - DaysToExp: number of business days to ExpirationDate.
+        - OpenContracts: number of open contracts at the start of the trading day.
     """
-    df_raw = common.fetch_past_raw_df(asset_code="FRC", trade_date=trade_date)
-    if return_raw:
+    df_raw = cm.fetch_past_raw_df(asset_code="DDI", trade_date=trade_date)
+    if return_raw or df_raw.empty:
         return df_raw
-    return _process_past_data(df_raw, trade_date)
+    return _process_raw_df(df_raw, trade_date)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyield-0.7.6/pyield/holidays/br_holidays_new.txt` & `pyield-0.7.7/pyield/holidays/br_holidays_new.txt`

 * *Files identical despite different names*

### Comparing `pyield-0.7.6/pyield/holidays/br_holidays_old.txt` & `pyield-0.7.7/pyield/holidays/br_holidays_old.txt`

 * *Files identical despite different names*

### Comparing `pyield-0.7.6/pyield/holidays/core.py` & `pyield-0.7.7/pyield/holidays/core.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.6/pyield/indicators.py` & `pyield-0.7.7/pyield/indicators.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.6/pyield/projections.py` & `pyield-0.7.7/pyield/projections.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,27 +59,30 @@
 
     # Load the workbook and select the first sheet
     workbook = pc.load_workbook(excel_data)
     first_sheet = workbook.sheet_names[0]
     data = workbook.get_sheet_by_name(first_sheet).to_python(skip_empty_area=True)
 
     # Extract projection update date and time from the first row
-    last_update_str = data[0][0].split("Atualização:")[-1].strip()
+    update_str = str(data[0][0])
+    last_update_str = update_str.split("Atualização:")[-1].strip()
     last_updated = pd.to_datetime(last_update_str, format="%d/%m/%Y - %H:%M h")
 
     # Find the row containing the IPCA projection and extract its data
     ipca_data = next(line for line in data if "IPCA1" in line)
+    ipca_text = str(ipca_data[-1])
 
     # Convert the last element of the IPCA data row to float for the projection value
-    ipca_value = round(float(ipca_data[-1]) / 100, 4)
+    ipca_value = round(float(ipca_text) / 100, 4)
 
     # Extract and format the reference month
-    month_text = ipca_data[1].split("(")[-1].split(")")[0]
+    projection_text = str(ipca_data[1])
+    month_str = projection_text.split("(")[-1].split(")")[0]
     locale.setlocale(locale.LC_TIME, "pt_BR.UTF-8")
-    ipca_month_ts = pd.to_datetime(month_text, format="%b/%y")
+    ipca_month_ts = pd.to_datetime(month_str, format="%b/%y")
     ipca_month_br = ipca_month_ts.strftime("%b/%Y").upper()
     locale.setlocale(locale.LC_TIME, "")  # Reset locale to default
 
     return IndicatorProjection(
         last_updated=last_updated,
         reference_month_ts=ipca_month_ts,
         reference_month_br=ipca_month_br,
```

### Comparing `pyield-0.7.6/pyield/treasuries.py` & `pyield-0.7.7/pyield/treasuries.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.6/pyield/utils.py` & `pyield-0.7.7/pyield/utils.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.6/pyproject.toml` & `pyield-0.7.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     "numpy",
     "beautifulsoup4",
     "html5lib",
     "lxml",
     "python-calamine>=0.2.0",
 ]
 dynamic = []
-version = "0.7.6"
+version = "0.7.7"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Source = "https://github.com/crdcj/PYield"
```

### Comparing `pyield-0.7.6/tests/test_bday.py` & `pyield-0.7.7/tests/test_bday.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.6/tests/test_futures.py` & `pyield-0.7.7/tests/test_futures.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.6/PKG-INFO` & `pyield-0.7.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PYield
-Version: 0.7.6
+Version: 0.7.7
 Summary: A Python library for analysis of fixed income instruments in Brazil
 Keywords: fixed-income, brazil, finance, analysis, bonds
 Author-Email: Carlos Carvalho <cr.cj@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Carlos Carvalho
```

