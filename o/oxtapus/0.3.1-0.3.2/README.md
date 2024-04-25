# Comparing `tmp/oxtapus-0.3.1-py3-none-any.whl.zip` & `tmp/oxtapus-0.3.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,27 +1,27 @@
-Zip file size: 37774 bytes, number of entries: 25
+Zip file size: 38065 bytes, number of entries: 25
 -rw-r--r--  2.0 unx     6148 b- defN 80-Jan-01 00:00 oxtapus/.DS_Store
 -rw-r--r--  2.0 unx      102 b- defN 80-Jan-01 00:00 oxtapus/__init__.py
 -rw-r--r--  2.0 unx     2746 b- defN 80-Jan-01 00:00 oxtapus/codal.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 oxtapus/models/__init__.py
 -rw-r--r--  2.0 unx     2122 b- defN 80-Jan-01 00:00 oxtapus/models/rahavard.py
--rw-r--r--  2.0 unx     2731 b- defN 80-Jan-01 00:00 oxtapus/models/tsetmc.py
+-rw-r--r--  2.0 unx     4817 b- defN 80-Jan-01 00:00 oxtapus/models/tsetmc.py
 -rw-r--r--  2.0 unx    25365 b- defN 80-Jan-01 00:00 oxtapus/rahavard.py
 -rw-r--r--  2.0 unx     6082 b- defN 80-Jan-01 00:00 oxtapus/tgju.py
--rw-r--r--  2.0 unx    83931 b- defN 80-Jan-01 00:00 oxtapus/tsetmc.py
+-rw-r--r--  2.0 unx    84268 b- defN 80-Jan-01 00:00 oxtapus/tsetmc.py
 -rw-r--r--  2.0 unx      165 b- defN 80-Jan-01 00:00 oxtapus/utils/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 oxtapus/utils/codal/__init__.py
 -rw-r--r--  2.0 unx    10916 b- defN 80-Jan-01 00:00 oxtapus/utils/codal/clean_data.py
 -rw-r--r--  2.0 unx     6854 b- defN 80-Jan-01 00:00 oxtapus/utils/codal/items.py
 -rw-r--r--  2.0 unx     4882 b- defN 80-Jan-01 00:00 oxtapus/utils/codal/models.py
 -rw-r--r--  2.0 unx     1036 b- defN 80-Jan-01 00:00 oxtapus/utils/codal/request.py
 -rw-r--r--  2.0 unx     1042 b- defN 80-Jan-01 00:00 oxtapus/utils/codal/utils.py
 -rw-r--r--  2.0 unx     5767 b- defN 80-Jan-01 00:00 oxtapus/utils/columns.py
 -rw-r--r--  2.0 unx       47 b- defN 80-Jan-01 00:00 oxtapus/utils/http/__init__.py
 -rw-r--r--  2.0 unx     2156 b- defN 80-Jan-01 00:00 oxtapus/utils/http/requests.py
 -rw-r--r--  2.0 unx     2926 b- defN 80-Jan-01 00:00 oxtapus/utils/models.py
 -rw-r--r--  2.0 unx      825 b- defN 80-Jan-01 00:00 oxtapus/utils/normalize.py
--rw-r--r--  2.0 unx     1071 b- defN 80-Jan-01 00:00 oxtapus-0.3.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx    19557 b- defN 80-Jan-01 00:00 oxtapus-0.3.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 oxtapus-0.3.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx     2004 b- defN 16-Jan-01 00:00 oxtapus-0.3.1.dist-info/RECORD
-25 files, 188563 bytes uncompressed, 34568 bytes compressed:  81.7%
+-rw-r--r--  2.0 unx     1071 b- defN 80-Jan-01 00:00 oxtapus-0.3.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx    19557 b- defN 80-Jan-01 00:00 oxtapus-0.3.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 oxtapus-0.3.2.dist-info/WHEEL
+?rw-r--r--  2.0 unx     2004 b- defN 16-Jan-01 00:00 oxtapus-0.3.2.dist-info/RECORD
+25 files, 190986 bytes uncompressed, 34859 bytes compressed:  81.7%
```

## zipnote {}

```diff
@@ -57,20 +57,20 @@
 
 Filename: oxtapus/utils/models.py
 Comment: 
 
 Filename: oxtapus/utils/normalize.py
 Comment: 
 
-Filename: oxtapus-0.3.1.dist-info/LICENSE.txt
+Filename: oxtapus-0.3.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: oxtapus-0.3.1.dist-info/METADATA
+Filename: oxtapus-0.3.2.dist-info/METADATA
 Comment: 
 
-Filename: oxtapus-0.3.1.dist-info/WHEEL
+Filename: oxtapus-0.3.2.dist-info/WHEEL
 Comment: 
 
-Filename: oxtapus-0.3.1.dist-info/RECORD
+Filename: oxtapus-0.3.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## oxtapus/models/tsetmc.py

```diff
@@ -1,9 +1,11 @@
 import datetime as dt
-from pydantic import BaseModel, Field, field_validator
+from typing import Optional
+from pydantic import BaseModel, Field, field_validator, model_validator
+from pydantic.v1.utils import GetterDict
 
 
 class MarketWatchOrderBook(BaseModel):
     ob_level: int = Field(alias="n")
     bid_count: int = Field(alias="zmd")
     bid_size: float = Field(alias="qmd")
     bid_price: float = Field(alias="pmd")
@@ -71,7 +73,67 @@
     volume: float = Field(alias="qTotTran5J")
     value: float = Field(alias="qTotCap")
     trade_count: float = Field(alias="zTotTran")
 
     @field_validator("date", mode="before")
     def parse_date(cls, value):
         return dt.datetime.strptime(str(value), "%Y%m%d").date()
+
+
+class EPS(BaseModel):
+    eps: Optional[float] = Field(alias="estimatedEPS")
+    sector_pe: Optional[float] = Field(alias="sectorPE")
+
+
+class Sector(BaseModel):
+    code: str = Field(alias="cSecVal")
+    name: str = Field(alias="lSecVal")
+
+
+class StaticThreshold(BaseModel):
+    min_threshold: float = Field(alias="psGelStaMin")
+    max_threshold: float = Field(alias="psGelStaMax")
+
+
+class InsInfo(BaseModel):
+    ins_code: str = Field(alias="insCode")
+    ins_id: str = Field(alias="instrumentID")
+    isin: str = Field(alias="cIsin")
+    symbol: str = Field(alias="lVal18AFC")
+    name: str = Field(alias="lVal30")
+    name_en: str = Field(alias="lVal18")
+    eps: Optional[float]
+    sector_pe: Optional[float]
+    static_threshold: StaticThreshold = Field(alias="staticThreshold")
+    min_week: float = Field(alias="minWeek")
+    max_week: float = Field(alias="maxWeek")
+    min_year: float = Field(alias="minYear")
+    max_year: float = Field(alias="maxYear")
+    mean_vol_monthly: float = Field(alias="qTotTran5JAvg")
+    pct_float_shares: Optional[str] = Field(alias="kAjCapValCpsIdx")
+    base_vol: int = Field(alias="baseVol")
+    capital: float = Field(alias="zTitad")
+    contract_size: float = Field(alias="contractSize")
+    sector_code: str
+    sector_name: str
+    market_name: str = Field(alias="flowTitle")
+    market_code: int = Field(alias="flow")
+    market_type: str = Field(alias="cgrValCotTitle")
+    group_type: str = Field(alias="cgrValCot")
+
+    @model_validator(mode="before")
+    def flatten_eps_sector(cls, values: GetterDict):
+        eps = values.get("eps")
+        sector = values.get("sector")
+        eps = EPS.model_validate(eps)
+        sector = Sector.model_validate(sector)
+
+        result = {
+            "eps": eps.eps,
+            "sector_pe": eps.sector_pe,
+            "sector_code": sector.code,
+            "sector_name": sector.name,
+        }
+        values.pop("eps")
+        values.pop("sector")
+        result.update(values)
+        return result
```

## oxtapus/tsetmc.py

```diff
@@ -2,26 +2,27 @@
 import datetime
 from enum import Enum
 import polars as pl
 from typing import List
 from pydantic import validate_call
 from urllib.parse import urlencode
 import itertools
-from oxtapus.models.tsetmc import HistPrice, MarketWatch, ClientTypeAll
+from oxtapus.models.tsetmc import HistPrice, MarketWatch, ClientTypeAll, InsInfo
 
 from oxtapus.utils.http import requests, async_requests
 from oxtapus.utils import (
     json_normalize,
     word_normalize,
     manipulation_cols,
     cols,
     normalize_nested_dict,
 )
 from oxtapus.utils.models import AdjustPriceFlow, InsShareChangeFlow, OptionsMW
 
+
 __all__ = ["TSETMC", "MWSections"]
 
 
 class MWSections(str, Enum):
     stock = "stock"
     ifb_paye = "ifb_paye"
     mortgage = "mortgage"
@@ -522,70 +523,61 @@
         polars.DataFrame
 
         example
         ------
         >>> from oxtapus import TSETMC
         >>> tsetmc = TSETMC(async_req=True)
         >>> tsetmc.ins_info(ins_code = ["7745894403636165", "65883838195688438"])
-        shape: (2, 17)
-        ┌────────────┬────────────┬───────────┬────────────┬───┬──────────┬───────┬────────────┬───────────┐
-        │ ins_code   ┆ ins_id     ┆ symbol_en ┆ name_en    ┆ … ┆ base_vol ┆ eps   ┆ pct_float_ ┆ contract_ │
-        │ ---        ┆ ---        ┆ ---       ┆ ---        ┆   ┆ ---      ┆ ---   ┆ shares     ┆ size      │
-        │ str        ┆ str        ┆ str       ┆ str        ┆   ┆ i64      ┆ str   ┆ ---        ┆ ---       │
-        │            ┆            ┆           ┆            ┆   ┆          ┆       ┆ str        ┆ i64       │
-        ╞════════════╪════════════╪═══════════╪════════════╪═══╪══════════╪═══════╪════════════╪═══════════╡
-        │ 7745894403 ┆ IRO1PNES00 ┆ PNES      ┆ S*Isf. Oil ┆ … ┆ 14760148 ┆ 1675  ┆ 43         ┆ 0         │
-        │ 636165     ┆ 01         ┆           ┆ Ref.Co.    ┆   ┆          ┆       ┆            ┆           │
-        │ 6588383819 ┆ IRO1IKCO00 ┆ IKCO      ┆ Iran       ┆ … ┆ 51746442 ┆ -1359 ┆ 36         ┆ 0         │
-        │ 5688438    ┆ 01         ┆           ┆ Khodro     ┆   ┆          ┆       ┆            ┆           │
-        └────────────┴────────────┴───────────┴────────────┴───┴──────────┴───────┴────────────┴───────────┘
+        shape: (2, 24)
+        ┌────────────┬────────────┬───────────┬────────┬───┬───────────┬───────────┬───────────┬───────────┐
+        │ ins_code   ┆ ins_id     ┆ isin      ┆ symbol ┆ … ┆ market_na ┆ market_co ┆ market_ty ┆ group_typ │
+        │ ---        ┆ ---        ┆ ---       ┆ ---    ┆   ┆ me        ┆ de        ┆ pe        ┆ e         │
+        │ str        ┆ str        ┆ str       ┆ str    ┆   ┆ ---       ┆ ---       ┆ ---       ┆ ---       │
+        │            ┆            ┆           ┆        ┆   ┆ str       ┆ i64       ┆ str       ┆ str       │
+        ╞════════════╪════════════╪═══════════╪════════╪═══╪═══════════╪═══════════╪═══════════╪═══════════╡
+        │ 7745894403 ┆ IRO1PNES00 ┆ IRO1PNES0 ┆ شپنا   ┆ … ┆ بازار     ┆ 1         ┆ بازار اول ┆ N1        │
+        │ 636165     ┆ 01         ┆ 000       ┆        ┆   ┆ بورس      ┆           ┆ (تابلوی   ┆           │
+        │            ┆            ┆           ┆        ┆   ┆           ┆           ┆ اصلی)     ┆           │
+        │            ┆            ┆           ┆        ┆   ┆           ┆           ┆ بورس      ┆           │
+        │ 6588383819 ┆ IRO1IKCO00 ┆ IRO1IKCO0 ┆ خودرو  ┆ … ┆ بازار     ┆ 1         ┆ بازار دوم ┆ N2        │
+        │ 5688438    ┆ 01         ┆ 008       ┆        ┆   ┆ بورس      ┆           ┆ (تابلوی   ┆           │
+        │            ┆            ┆           ┆        ┆   ┆           ┆           ┆ فرعی)     ┆           │
+        │            ┆            ┆           ┆        ┆   ┆           ┆           ┆ بورس      ┆           │
+        └────────────┴────────────┴───────────┴────────┴───┴───────────┴───────────┴───────────┴───────────┘
 
         >>> tsetmc.ins_info(symbol = ["شپنا", "خودرو"])
-        shape: (2, 17)
-        ┌────────────┬────────────┬───────────┬────────────┬───┬──────────┬───────┬────────────┬───────────┐
-        │ ins_code   ┆ ins_id     ┆ symbol_en ┆ name_en    ┆ … ┆ base_vol ┆ eps   ┆ pct_float_ ┆ contract_ │
-        │ ---        ┆ ---        ┆ ---       ┆ ---        ┆   ┆ ---      ┆ ---   ┆ shares     ┆ size      │
-        │ str        ┆ str        ┆ str       ┆ str        ┆   ┆ i64      ┆ str   ┆ ---        ┆ ---       │
-        │            ┆            ┆           ┆            ┆   ┆          ┆       ┆ str        ┆ i64       │
-        ╞════════════╪════════════╪═══════════╪════════════╪═══╪══════════╪═══════╪════════════╪═══════════╡
-        │ 7745894403 ┆ IRO1PNES00 ┆ PNES      ┆ S*Isf. Oil ┆ … ┆ 14760148 ┆ 1675  ┆ 43         ┆ 0         │
-        │ 636165     ┆ 01         ┆           ┆ Ref.Co.    ┆   ┆          ┆       ┆            ┆           │
-        │ 6588383819 ┆ IRO1IKCO00 ┆ IKCO      ┆ Iran       ┆ … ┆ 51746442 ┆ -1359 ┆ 36         ┆ 0         │
-        │ 5688438    ┆ 01         ┆           ┆ Khodro     ┆   ┆          ┆       ┆            ┆           │
-        └────────────┴────────────┴───────────┴────────────┴───┴──────────┴───────┴────────────┴───────────┘
-        """
-
-        def map_json(data: dict) -> dict:
-            return {
-                "ins_code": data["insCode"],
-                "ins_id": data["instrumentID"],
-                "symbol_en": data["cIsin"][4:8],
-                "name_en": data["lVal18"],
-                "symbol": data["lVal18AFC"],
-                "name": data["lVal30"],
-                "capital": data["zTitad"],
-                "sector_name": data["sector"]["lSecVal"],
-                "sector_code": data["sector"]["cSecVal"].replace(" ", ""),
-                "group_type": data["cgrValCot"],
-                "market_name": data["flowTitle"],
-                "market_code": data["flow"],
-                "market_type": data["cgrValCotTitle"],
-                "base_vol": data["baseVol"],
-                "eps": data["eps"]["estimatedEPS"],
-                "pct_float_shares": data["kAjCapValCpsIdx"],
-                "contract_size": data["contractSize"],
-            }
+        shape: (2, 24)
+        ┌────────────┬────────────┬───────────┬────────┬───┬───────────┬───────────┬───────────┬───────────┐
+        │ ins_code   ┆ ins_id     ┆ isin      ┆ symbol ┆ … ┆ market_na ┆ market_co ┆ market_ty ┆ group_typ │
+        │ ---        ┆ ---        ┆ ---       ┆ ---    ┆   ┆ me        ┆ de        ┆ pe        ┆ e         │
+        │ str        ┆ str        ┆ str       ┆ str    ┆   ┆ ---       ┆ ---       ┆ ---       ┆ ---       │
+        │            ┆            ┆           ┆        ┆   ┆ str       ┆ i64       ┆ str       ┆ str       │
+        ╞════════════╪════════════╪═══════════╪════════╪═══╪═══════════╪═══════════╪═══════════╪═══════════╡
+        │ 7745894403 ┆ IRO1PNES00 ┆ IRO1PNES0 ┆ شپنا   ┆ … ┆ بازار     ┆ 1         ┆ بازار اول ┆ N1        │
+        │ 636165     ┆ 01         ┆ 000       ┆        ┆   ┆ بورس      ┆           ┆ (تابلوی   ┆           │
+        │            ┆            ┆           ┆        ┆   ┆           ┆           ┆ اصلی)     ┆           │
+        │            ┆            ┆           ┆        ┆   ┆           ┆           ┆ بورس      ┆           │
+        │ 6588383819 ┆ IRO1IKCO00 ┆ IRO1IKCO0 ┆ خودرو  ┆ … ┆ بازار     ┆ 1         ┆ بازار دوم ┆ N2        │
+        │ 5688438    ┆ 01         ┆ 008       ┆        ┆   ┆ بورس      ┆           ┆ (تابلوی   ┆           │
+        │            ┆            ┆           ┆        ┆   ┆           ┆           ┆ فرعی)     ┆           │
+        │            ┆            ┆           ┆        ┆   ┆           ┆           ┆ بورس      ┆           │
+        └────────────┴────────────┴───────────┴────────┴───┴───────────┴───────────┴───────────┴───────────┘
+        """
 
         ins_code = symbol if symbol else ins_code
 
         if isinstance(ins_code, str):
             ins_code = [ins_code]
         url = [self.url.ins_info(i) for i in ins_code]
         r = self.requests(url)
-        return pl.from_records([map_json(i.get("instrumentInfo")) for i in r])
+        records = [
+            InsInfo.model_validate(i.get("instrumentInfo")).model_dump() for i in r
+        ]
+        df = pl.from_dicts(records)
+        return df
 
     def specific_option_data(self, ins_id: str | list[str]) -> pl.DataFrame:
         """
         Get complimentary option info.
 
         Parameters
         ----------
```

## Comparing `oxtapus-0.3.1.dist-info/LICENSE.txt` & `oxtapus-0.3.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `oxtapus-0.3.1.dist-info/METADATA` & `oxtapus-0.3.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oxtapus
-Version: 0.3.1
+Version: 0.3.2
 Summary: 
 Home-page: https://github.com/yghaderi/oxtapus
 Author: Yaghoub Ghadri
 Author-email: y.ghaderi@outlook.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: oxtapus Version: 0.3.1 Summary: Home-page: https://
+Metadata-Version: 2.1 Name: oxtapus Version: 0.3.2 Summary: Home-page: https://
 github.com/yghaderi/oxtapus Author: Yaghoub Ghadri Author-email:
 y.ghaderi@outlook.com Requires-Python: >=3.10,<4.0 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Requires-Dist: httpx (>=0.25.0,<0.26.0) Requires-
 Dist: polars (>=0.20.3,<0.21.0) Requires-Dist: pydantic (>=2.5.3,<3.0.0)
 Requires-Dist: tarix (>=0.1.1,<0.2.0) Requires-Dist: tenacity (>=8.2.3,<9.0.0)
```

## Comparing `oxtapus-0.3.1.dist-info/RECORD` & `oxtapus-0.3.2.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 oxtapus/.DS_Store,sha256=0rDOK8ZfHcSrcVGAzbYz4wStqJsCIq6ategrLYGyzp0,6148
 oxtapus/__init__.py,sha256=savGpOWlYPsqBhLAEXxOPKd1_sepJIF71yGDQHthrrU,102
 oxtapus/codal.py,sha256=iWVcQxJVAabma40UWSJVp-lfONrGOARnzPzODbdW6Qo,2746
 oxtapus/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 oxtapus/models/rahavard.py,sha256=pqD5p5EKDboB022qFCh_MTSGRHV7mzuU_yowo-e5y2k,2122
-oxtapus/models/tsetmc.py,sha256=1YokgDyML5TZX5fVxdhNBDqHWj5Ib9zLfriETnjidb4,2731
+oxtapus/models/tsetmc.py,sha256=VgVywEc-KOIDCsrkutk9AGAU0OsZj_RIhIvEnQMfZKA,4817
 oxtapus/rahavard.py,sha256=C5ra8ZpVspqKkYLuO3zKq7827z6dSo9t_ayKrIESXAQ,25365
 oxtapus/tgju.py,sha256=jIseeQuldq1FdHp9BIlau0KQimVvu_oydLuOfO5wakU,6082
-oxtapus/tsetmc.py,sha256=L1Cse_AfZoD_jpx3wxwEIVemJH0qo0RUYl7rSs9-Z6w,83931
+oxtapus/tsetmc.py,sha256=MbSeQf5z_NPd9MuWeGCEa3LDhX4qClnWd5P4ulGQkyo,84268
 oxtapus/utils/__init__.py,sha256=8R6IZMUVZHW9E-ka0u-nyVq6lQsHMk7kv6qjkloUZIo,165
 oxtapus/utils/codal/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 oxtapus/utils/codal/clean_data.py,sha256=UR7jX36zzbX0qgekHnnzQ9tcZJRbIlehm24NjAk1NzQ,10916
 oxtapus/utils/codal/items.py,sha256=71sV_8bkpp1CdiiXnzfK_R74vng7l_oQWpj_z6liy9s,6854
 oxtapus/utils/codal/models.py,sha256=uLm7nlhKIlrbs06_jFl0oyTtA-JUMBdYJm0ZkQPaOrs,4882
 oxtapus/utils/codal/request.py,sha256=i5P-0UEces2sy_VHypap8TqcNEgV9FXEOp4OIY1JwQs,1036
 oxtapus/utils/codal/utils.py,sha256=FLcEbzFBMybCK5Xmmb_HrNETDM2cH_bwC5zegx97oBY,1042
 oxtapus/utils/columns.py,sha256=ZZNfyzYMCGCHYk5hb5fPFLCLU_egpVgtZQBtA2_mMpg,5767
 oxtapus/utils/http/__init__.py,sha256=447GDWyNp9xpyt7tERfZfZtS-jH34wOdFJITVmwXVkE,47
 oxtapus/utils/http/requests.py,sha256=_foEzr-vqdlyng0FdiIJjMN4AjJGiz2kTYP0RFLjnyM,2156
 oxtapus/utils/models.py,sha256=Y8WOP--2d9dbtCOnL125zHVXSuki_F3QZ5e630Mtu6k,2926
 oxtapus/utils/normalize.py,sha256=aCTA3bGdxx4_8Lm_Qc7dpVaue-L8ANTzr_LL5xaCX_Y,825
-oxtapus-0.3.1.dist-info/LICENSE.txt,sha256=rk-2xVGc7h8PusLyqRcXBBh3TiYtJXA-EE_YXpDfyC0,1071
-oxtapus-0.3.1.dist-info/METADATA,sha256=Uz80Sw_gY32QA4MrqV3k-KAZXGqcAioGP6_ugQGAi2Q,19557
-oxtapus-0.3.1.dist-info/WHEEL,sha256=FMvqSimYX_P7y0a7UY-_Mc83r5zkBZsCYPm7Lr0Bsq4,88
-oxtapus-0.3.1.dist-info/RECORD,,
+oxtapus-0.3.2.dist-info/LICENSE.txt,sha256=rk-2xVGc7h8PusLyqRcXBBh3TiYtJXA-EE_YXpDfyC0,1071
+oxtapus-0.3.2.dist-info/METADATA,sha256=_Y8ih49HFzxa8E7GJPnz7Y7u5iRdIWy-yG5IJH015k8,19557
+oxtapus-0.3.2.dist-info/WHEEL,sha256=FMvqSimYX_P7y0a7UY-_Mc83r5zkBZsCYPm7Lr0Bsq4,88
+oxtapus-0.3.2.dist-info/RECORD,,
```

