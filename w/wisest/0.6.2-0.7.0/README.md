# Comparing `tmp/wisest-0.6.2-py3-none-any.whl.zip` & `tmp/wisest-0.7.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 6566 bytes, number of entries: 12
--rw-r--r--  2.0 unx      416 b- defN 80-Jan-01 00:00 wise/__init__.py
--rw-r--r--  2.0 unx     1171 b- defN 80-Jan-01 00:00 wise/cli.py
--rw-r--r--  2.0 unx     1789 b- defN 80-Jan-01 00:00 wise/cost.py
+Zip file size: 6517 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      452 b- defN 80-Jan-01 00:00 wise/__init__.py
+-rw-r--r--  2.0 unx     1252 b- defN 80-Jan-01 00:00 wise/cli.py
+-rw-r--r--  2.0 unx      771 b- defN 80-Jan-01 00:00 wise/cost.py
 -rw-r--r--  2.0 unx      672 b- defN 80-Jan-01 00:00 wise/currency.py
 -rw-r--r--  2.0 unx     2157 b- defN 80-Jan-01 00:00 wise/method.py
--rw-r--r--  2.0 unx     2773 b- defN 80-Jan-01 00:00 wise/price.py
--rw-r--r--  2.0 unx     1698 b- defN 80-Jan-01 00:00 wise/rate.py
--rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 wisest-0.6.2.dist-info/LICENSE
--rw-r--r--  2.0 unx      595 b- defN 80-Jan-01 00:00 wisest-0.6.2.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 wisest-0.6.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       37 b- defN 80-Jan-01 00:00 wisest-0.6.2.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx      874 b- defN 16-Jan-01 00:00 wisest-0.6.2.dist-info/RECORD
-12 files, 13336 bytes uncompressed, 5130 bytes compressed:  61.5%
+-rw-r--r--  2.0 unx     3587 b- defN 80-Jan-01 00:00 wise/price.py
+-rw-r--r--  2.0 unx     1825 b- defN 80-Jan-01 00:00 wise/rate.py
+-rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 wisest-0.7.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      546 b- defN 80-Jan-01 00:00 wisest-0.7.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 wisest-0.7.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       37 b- defN 80-Jan-01 00:00 wisest-0.7.0.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx      873 b- defN 16-Jan-01 00:00 wisest-0.7.0.dist-info/RECORD
+12 files, 13326 bytes uncompressed, 5081 bytes compressed:  61.9%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: wise/price.py
 Comment: 
 
 Filename: wise/rate.py
 Comment: 
 
-Filename: wisest-0.6.2.dist-info/LICENSE
+Filename: wisest-0.7.0.dist-info/LICENSE
 Comment: 
 
-Filename: wisest-0.6.2.dist-info/METADATA
+Filename: wisest-0.7.0.dist-info/METADATA
 Comment: 
 
-Filename: wisest-0.6.2.dist-info/WHEEL
+Filename: wisest-0.7.0.dist-info/WHEEL
 Comment: 
 
-Filename: wisest-0.6.2.dist-info/entry_points.txt
+Filename: wisest-0.7.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: wisest-0.6.2.dist-info/RECORD
+Filename: wisest-0.7.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wise/__init__.py

```diff
@@ -1,14 +1,15 @@
-from .cost import Cost
-from .cost import create_cost
+from .cost import print_cost
 from .currency import Currency
 from .currency import CurrencyRequest
 from .method import PayInMethod
 from .method import PayOutMethod
 from .price import Price
 from .price import PriceRequest
 from .price import find_price
+from .price import query_price
 from .rate import Rate
 from .rate import RateHistoryRequest
 from .rate import RateRequest
 from .rate import Resolution
 from .rate import Unit
+from .rate import query_rate
```

## wise/cli.py

```diff
@@ -1,13 +1,14 @@
 from itertools import product
 
 import click
 from tqdm import tqdm
 
-from .cost import create_cost
+from .cost import print_cost
+from .price import query_price
 
 
 @click.command()
 @click.argument("source-currency", type=click.STRING)
 @click.argument("target-amount", type=click.STRING)
 @click.argument("target-currency", type=click.STRING)
 @click.option("-i", "--pay-in-method", type=click.STRING, default="VISA_CREDIT")
@@ -19,24 +20,24 @@
     pay_in_method: str,
     pay_out_method: str,
 ) -> None:
     sources = source_currency.split(",")
     amounts = [float(x) for x in target_amount.split(",")]
     targets = target_currency.split(",")
 
-    costs = [
-        create_cost(
-            source,
-            float(amount),
-            target,
+    prices = [
+        query_price(
+            source_currency=source,
+            target_amount=float(amount),
+            target_currency=target,
             pay_in_method=pay_in_method,
             pay_out_method=pay_out_method,
         )
         for source, amount, target in tqdm(list(product(sources, amounts, targets)))
     ]
 
     # sort by total fee rate
-    costs = sorted(costs, key=lambda x: x.price.variable_fee_percent)
+    prices = sorted(prices, key=lambda p: p.variable_fee_percent)
 
     # print costs
-    for cost in costs:
-        print(cost)
+    for price in prices:
+        print_cost(price)
```

## wise/cost.py

```diff
@@ -1,61 +1,16 @@
-from pydantic import BaseModel
-from pydantic import Field
-
 from .price import Price
-from .price import PriceRequest
-from .price import find_price
-
-
-class Cost(BaseModel):
-    price: Price
-    card_fee_percent: float = Field(default=1.5)
-    reward_rate: float = Field(default=0.1)
-
-    @property
-    def card_fee(self) -> float:
-        return self.price.source_amount * self.card_fee_percent / 100
-
-    @property
-    def wise_fee_percent(self) -> float:
-        return 100 * self.price.total / self.price.source_amount
-
-    @property
-    def fee(self) -> float:
-        return self.card_fee + self.price.total
-
-    @property
-    def fee_percent(self) -> float:
-        return 100 * self.fee / (self.price.source_amount + self.card_fee)
-
-    @property
-    def cost_per_mile(self) -> float:
-        return self.fee / (self.price.source_amount * self.reward_rate)
-
-    def __str__(self) -> str:
-        return (
-            f"Add {self.price.target_amount:.2f} { self.price.target_currency}"
-            f", pay {self.price.source_amount:.2f} {self.price.source_currency}"
-            f", wise fee: {self.price.total:.2f} {self.price.source_currency} ({self.wise_fee_percent:.2f}%)"
-            f", total fee: {self.fee:.2f} {self.price.source_currency} ({self.fee_percent:.2f}%)"
-            f", cost per mile: {self.cost_per_mile:.4f}"
-        )
 
 
-def create_cost(
-    source: str,
-    amount: float,
-    target: str,
-    pay_in_method: str = "VISA_CREDIT",
-    pay_out_method: str = "BALANCE",
-) -> Cost:
-    prices = PriceRequest(
-        source_currency=source,
-        target_amount=amount,
-        target_currency=target,
-    ).do()
-    price = find_price(
-        prices,
-        pay_in_method=pay_in_method,
-        pay_out_method=pay_out_method,
+def print_cost(price: Price, card_fee_percent: float = 1.5, reward_rate: float = 0.1) -> None:
+    card_fee = price.source_amount * card_fee_percent / 100
+    wise_fee_percent = 100 * price.total / price.source_amount
+    fee = card_fee + price.total
+    fee_percent = 100 * fee / (price.source_amount + card_fee)
+    cost_per_mile = fee / (price.source_amount * reward_rate)
+    print(
+        f"Add {price.target_amount:.2f} { price.target_currency}"
+        f", pay {price.source_amount:.2f} {price.source_currency}"
+        f", wise fee: {price.total:.2f} {price.source_currency} ({wise_fee_percent:.2f}%)"
+        f", total fee: {fee:.2f} {price.source_currency} ({fee_percent:.2f}%)"
+        f", cost per mile: {cost_per_mile:.4f}"
     )
-    return Cost(price=price)
```

## wise/price.py

```diff
@@ -1,12 +1,13 @@
-from typing import Optional
+from __future__ import annotations
 
 import requests
 from pydantic import BaseModel
 from pydantic import Field
+from pydantic import field_validator
 from requests.utils import default_headers
 
 default_timeout = 10
 
 
 class Price(BaseModel):
     price_set_id: int = Field(validation_alias="priceSetId")
@@ -25,22 +26,27 @@
     ecb_rate: float = Field(validation_alias="ecbRate")
     ecb_rate_timestamp: int = Field(validation_alias="ecbRateTimestamp")
     ecb_markup_percent: float = Field(validation_alias="ecbMarkupPercent")
     additional_fee_details: dict = Field(validation_alias="additionalFeeDetails")
 
 
 class PriceRequest(BaseModel):
-    source_amount: Optional[float] = Field(None, serialization_alias="sourceAmount")
-    source_currency: Optional[str] = Field(None, serialization_alias="sourceCurrency")
-    target_amount: Optional[float] = Field(None, serialization_alias="targetAmount")
-    target_currency: Optional[str] = Field(None, serialization_alias="targetCurrency")
-    profile_id: Optional[str] = Field(None, serialization_alias="profileId")
-    profile_country: Optional[str] = Field(None, serialization_alias="profileCountry")
-    profile_type: Optional[str] = Field(None, serialization_alias="profileType")
-    markers: Optional[str] = None
+    source_amount: float | None = Field(default=None, serialization_alias="sourceAmount")
+    source_currency: str | None = Field(default=None, serialization_alias="sourceCurrency")
+    target_amount: float | None = Field(default=None, serialization_alias="targetAmount")
+    target_currency: str | None = Field(default=None, serialization_alias="targetCurrency")
+    profile_id: str | None = Field(default=None, serialization_alias="profileId")
+    profile_country: str | None = Field(default=None, serialization_alias="profileCountry")
+    profile_type: str | None = Field(default=None, serialization_alias="profileType")
+    markers: str | None = None
+
+    @field_validator("source_currency", "target_currency")
+    @classmethod
+    def upper(cls, s: str) -> str:
+        return s.upper()
 
     def do(self) -> list[Price]:
         # https://wise.com/gb/pricing/receive
         # https://wise.com/gb/pricing/send-money
 
         resp = requests.get(
             url="http://wise.com/gateway/v1/price",
@@ -58,7 +64,29 @@
 ) -> Price:
     for price in prices:
         if price.pay_in_method == pay_in_method.upper() and price.pay_out_method == pay_out_method.upper():
             return price
 
     msg = f"Price not found for pay_in_method={pay_in_method} and pay_out_method={pay_out_method}"
     raise ValueError(msg)
+
+
+def query_price(
+    source_amount: float | None = None,
+    source_currency: str | None = None,
+    target_amount: float | None = None,
+    target_currency: str | None = None,
+    pay_in_method: str = "VISA_CREDIT",
+    pay_out_method: str = "BALANCE",
+) -> Price:
+    prices = PriceRequest(
+        source_amount=source_amount,
+        source_currency=source_currency,
+        target_amount=target_amount,
+        target_currency=target_currency,
+    ).do()
+    price = find_price(
+        prices,
+        pay_in_method=pay_in_method,
+        pay_out_method=pay_out_method,
+    )
+    return price
```

## wise/rate.py

```diff
@@ -15,14 +15,15 @@
 class Rate(BaseModel):
     source: str
     target: str
     value: float
     time: datetime
 
     @field_validator("time")
+    @classmethod
     def validate_time(cls, v: int | datetime) -> datetime:
         if isinstance(v, datetime):
             return v
         elif isinstance(v, int):
             return datetime.fromtimestamp(v // 1000)
         else:
             msg = f"invalid time: {v}"
@@ -50,14 +51,18 @@
             params=self.model_dump(),
             headers=default_headers(),
             timeout=default_timeout,
         )
         return Rate(**resp.json())
 
 
+def query_rate(source: str, target: str) -> Rate:
+    return RateRequest(source=source, target=target).do()
+
+
 # https://wise.com/rates/history?source=EUR&target=USD&length=10&resolution=daily&unit=day
 class RateHistoryRequest(BaseModel):
     source: str
     target: str
     length: int
     resolution: Resolution
     unit: Unit
```

## Comparing `wisest-0.6.2.dist-info/LICENSE` & `wisest-0.7.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `wisest-0.6.2.dist-info/METADATA` & `wisest-0.7.0.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: wisest
-Version: 0.6.2
+Version: 0.7.0
 Summary: 
 Author: narumi
 Author-email: toucans-cutouts0f@icloud.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: pydantic (>=2.4.2,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
```

