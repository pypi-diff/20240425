# Comparing `tmp/lnurl-0.4.2.tar.gz` & `tmp/lnurl-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnurl-0.4.2.tar", max compression
+gzip compressed data, was "lnurl-0.5.0.tar", max compression
```

## Comparing `lnurl-0.4.2.tar` & `lnurl-0.5.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1111 2023-12-05 18:11:31.110099 lnurl-0.4.2/LICENSE
--rwxr-xr-x   0        0        0     5779 2023-12-05 18:11:31.110099 lnurl-0.4.2/README.md
--rw-r--r--   0        0        0      660 2023-12-05 18:11:31.110099 lnurl-0.4.2/lnurl/__init__.py
--rwxr-xr-x   0        0        0     1762 2023-12-05 18:11:31.110099 lnurl-0.4.2/lnurl/cli.py
--rw-r--r--   0        0        0     1596 2023-12-05 18:11:31.110099 lnurl-0.4.2/lnurl/core.py
--rw-r--r--   0        0        0      486 2023-12-05 18:11:31.110099 lnurl-0.4.2/lnurl/exceptions.py
--rw-r--r--   0        0        0     1597 2023-12-05 18:11:31.110099 lnurl-0.4.2/lnurl/helpers.py
--rw-r--r--   0        0        0     5459 2023-12-05 18:11:31.110099 lnurl-0.4.2/lnurl/models.py
--rw-r--r--   0        0        0       26 2023-12-05 18:11:31.110099 lnurl-0.4.2/lnurl/py.typed
--rw-r--r--   0        0        0     8102 2023-12-05 18:11:31.110099 lnurl-0.4.2/lnurl/types.py
--rw-r--r--   0        0        0     1736 2023-12-05 18:11:31.110099 lnurl-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     6417 1970-01-01 00:00:00.000000 lnurl-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1111 2024-04-25 14:28:25.816641 lnurl-0.5.0/LICENSE
+-rwxr-xr-x   0        0        0     6163 2024-04-25 14:28:25.816641 lnurl-0.5.0/README.md
+-rw-r--r--   0        0        0      816 2024-04-25 14:28:25.816641 lnurl-0.5.0/lnurl/__init__.py
+-rwxr-xr-x   0        0        0     1521 2024-04-25 14:28:25.816641 lnurl-0.5.0/lnurl/cli.py
+-rw-r--r--   0        0        0     4863 2024-04-25 14:28:25.816641 lnurl-0.5.0/lnurl/core.py
+-rw-r--r--   0        0        0      486 2024-04-25 14:28:25.816641 lnurl-0.5.0/lnurl/exceptions.py
+-rw-r--r--   0        0        0     3781 2024-04-25 14:28:25.816641 lnurl-0.5.0/lnurl/helpers.py
+-rw-r--r--   0        0        0     5498 2024-04-25 14:28:25.816641 lnurl-0.5.0/lnurl/models.py
+-rw-r--r--   0        0        0       26 2024-04-25 14:28:25.816641 lnurl-0.5.0/lnurl/py.typed
+-rw-r--r--   0        0        0     8693 2024-04-25 14:28:25.816641 lnurl-0.5.0/lnurl/types.py
+-rw-r--r--   0        0        0     1796 2024-04-25 14:28:25.816641 lnurl-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     6878 1970-01-01 00:00:00.000000 lnurl-0.5.0/PKG-INFO
```

### Comparing `lnurl-0.4.2/LICENSE` & `lnurl-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lnurl-0.4.2/README.md` & `lnurl-0.5.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -49,42 +49,50 @@
 -----------------------
 
 You can use a `LnurlResponse` to wrap responses you get from a LNURL.
 The different types of responses defined in the [LNURL spec][lnurl-spec] have a different model
 with different properties (see `models.py`):
 
 ```python
-import requests
+import httpx
 
 from lnurl import Lnurl, LnurlResponse
 
 lnurl = Lnurl('LNURL1DP68GURN8GHJ7MRWW4EXCTNZD9NHXATW9EU8J730D3H82UNV94MKJARGV3EXZAELWDJHXUMFDAHR6WFHXQERSVPCA649RV')
+try:
+  async with httpx.AsyncClient() as client:
+    r = await client.get(lnurl.url)
+    res = LnurlResponse.from_dict(r.json())  # LnurlPayResponse
+    res.ok  # bool
+    res.max_sendable  # int
+    res.max_sats  # int
+    res.callback.base  # str
+    res.callback.query_params # dict
+    res.metadata  # str
+    res.metadata.list()  # list
+    res.metadata.text  # str
+    res.metadata.images  # list
 r = requests.get(lnurl.url)
-
-res = LnurlResponse.from_dict(r.json())  # LnurlPayResponse
-res.ok  # bool
-res.max_sendable  # int
-res.max_sats  # int
-res.callback.base  # str
-res.callback.query_params # dict
-res.metadata  # str
-res.metadata.list()  # list
-res.metadata.text  # str
-res.metadata.images  # list
 ```
 
-If you have already `requests` installed, you can also use the `.handle()` function directly.
+If you have already `httpx` installed, you can also use the `.handle()` function directly.
 It will return the appropriate response for a LNURL.
 
 ```python
 >>> import lnurl
 >>> lnurl.handle('lightning:LNURL1DP68GURN8GHJ7MRWW4EXCTNZD9NHXATW9EU8J730D3H82UNV94CXZ7FLWDJHXUMFDAHR6V33XCUNSVE38QV6UF')
 LnurlPayResponse(tag='payRequest', callback=WebUrl('https://lnurl.bigsun.xyz/lnurl-pay/callback/2169831', scheme='https', host='lnurl.bigsun.xyz', tld='xyz', host_type='domain', path='/lnurl-pay/callback/2169831'), min_sendable=10000, max_sendable=10000, metadata=LnurlPayMetadata('[["text/plain","NgHaEyaZNDnW iI DsFYdkI"],["image/png;base64","iVBOR...uQmCC"]]'))
 ```
 
+You can execute and LNURL with either payRequest, withdrawRequest or login tag using the `execute` function.
+```python
+>>> import lnurl
+>>> lnurl.execute('lightning:LNURL1DP68GURN8GHJ7MRWW4EXCTNZD9NHXATW9EU8J730D3H82UNV94CXZ7FLWDJHXUMFDAHR6V33XCUNSVE38QV6UF', 100000)
+```
+
 Building your own LNURL responses
 ---------------------------------
 
 For LNURL services, the `lnurl` package can be used to build **valid** responses.
 
 ```python
 from lnurl import LnurlWithdrawResponse
@@ -138,9 +146,9 @@
 Options:
   --help  Show this message and exit.
 
 Commands:
   decode           decode a LNURL
   encode           encode a URL
   handle           handle a LNURL
-  payment-request  make a payment_request
+  execute          execute a LNURL
 ```
```

### Comparing `lnurl-0.4.2/lnurl/__init__.py` & `lnurl-0.5.0/lnurl/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from .core import decode, encode, get, handle
+from .core import decode, encode, execute, execute_login, execute_pay_request, get, handle
 from .models import (
+    LnurlAuthResponse,
     LnurlChannelResponse,
     LnurlErrorResponse,
     LnurlHostedChannelResponse,
     LnurlPayActionResponse,
     LnurlPayResponse,
     LnurlPayResponseComment,
     LnurlResponse,
@@ -11,17 +12,21 @@
     LnurlWithdrawResponse,
 )
 from .types import Lnurl
 
 __all__ = [
     "decode",
     "encode",
+    "execute",
+    "execute_login",
+    "execute_pay_request",
     "get",
     "handle",
     "Lnurl",
+    "LnurlAuthResponse",
     "LnurlChannelResponse",
     "LnurlErrorResponse",
     "LnurlHostedChannelResponse",
     "LnurlPayActionResponse",
     "LnurlPayResponse",
     "LnurlPayResponseComment",
     "LnurlResponse",
```

### Comparing `lnurl-0.4.2/lnurl/cli.py` & `lnurl-0.5.0/lnurl/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-""" lnurl CLI """
+"""lnurl CLI"""
 
-import json
+import asyncio
 import sys
 
 import click
-import requests
 
 from .core import encode as encode_lnurl
+from .core import execute as execute_lnurl
 from .core import handle as handle_lnurl
 from .types import Lnurl
 
 # disable tracebacks on exceptions
 sys.tracebacklimit = 0
 
 
@@ -43,44 +43,35 @@
 
 @click.command()
 @click.argument("lnurl", type=str)
 def handle(lnurl):
     """
     handle a LNURL
     """
-    decoded = handle_lnurl(lnurl)
+    decoded = asyncio.run(handle_lnurl(lnurl))
     click.echo(decoded.json())
 
 
 @click.command()
 @click.argument("lnurl", type=str)
-@click.argument("amount", type=int)
-def payment_request(lnurl, amount):
+@click.argument("msat_or_login", type=str, required=False)
+def execute(lnurl, msat_or_login):
     """
-    make a payment_request
+    execute a LNURL request
     """
-    res = handle_lnurl(lnurl)
-    decoded = res.dict()
-
-    if decoded["tag"] and decoded["tag"] == "payRequest":
-        if decoded["minSendable"] <= amount <= decoded["maxSendable"]:
-            res = requests.get(decoded["callback"] + "?amount=" + str(amount))
-            res.raise_for_status()
-            return click.echo(json.dumps(res.json()))
-        else:
-            click.echo("Amount not in range.")
-    else:
-        click.echo("Not a payRequest:")
+    if not msat_or_login:
+        raise ValueError("You must provide either an amount_msat or a login_id.")
+    res = asyncio.run(execute_lnurl(lnurl, msat_or_login))
     click.echo(res.json())
 
 
 def main():
     """main function"""
     command_group.add_command(encode)
     command_group.add_command(decode)
     command_group.add_command(handle)
-    command_group.add_command(payment_request)
+    command_group.add_command(execute)
     command_group()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `lnurl-0.4.2/lnurl/models.py` & `lnurl-0.5.0/lnurl/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import math
 from typing import List, Literal, Optional, Union
 
+from bolt11 import MilliSatoshi
 from pydantic import BaseModel, Field, validator
 
 from .exceptions import LnurlResponseException
 from .types import (
     ClearnetUrl,
     DebugUrl,
     InitializationVector,
     LightningInvoice,
     LightningNodeUri,
     LnurlPayMetadata,
     Max144Str,
-    MilliSatoshi,
     OnionUrl,
 )
 
 
 class LnurlPayRouteHop(BaseModel):
     node_id: str = Field(..., alias="nodeId")
     channel_update: str = Field(..., alias="channelUpdate")
@@ -41,14 +41,15 @@
 class UrlAction(LnurlPaySuccessAction):
     tag: Literal["url"] = "url"
     url: Union[ClearnetUrl, OnionUrl, DebugUrl]
     description: Max144Str
 
 
 class LnurlResponseModel(BaseModel):
+
     class Config:
         allow_population_by_field_name = True
 
     def dict(self, **kwargs):
         kwargs.setdefault("by_alias", True)
         return super().dict(**kwargs)
 
@@ -97,16 +98,16 @@
     k1: str
     alias: Optional[str]
 
 
 class LnurlPayResponse(LnurlResponseModel):
     tag: Literal["payRequest"] = "payRequest"
     callback: Union[ClearnetUrl, OnionUrl, DebugUrl]
-    min_sendable: MilliSatoshi = Field(..., alias="minSendable")
-    max_sendable: MilliSatoshi = Field(..., alias="maxSendable")
+    min_sendable: MilliSatoshi = Field(..., alias="minSendable", gt=0)
+    max_sendable: MilliSatoshi = Field(..., alias="maxSendable", gt=0)
     metadata: LnurlPayMetadata
 
     @validator("max_sendable")
     def max_less_than_min(cls, value, values, **kwargs):  # noqa
         if "min_sendable" in values and value < values["min_sendable"]:
             raise ValueError("`max_sendable` cannot be less than `min_sendable`.")
         return value
@@ -139,16 +140,16 @@
     routes: List[List[LnurlPayRouteHop]] = []
 
 
 class LnurlWithdrawResponse(LnurlResponseModel):
     tag: Literal["withdrawRequest"] = "withdrawRequest"
     callback: Union[ClearnetUrl, OnionUrl, DebugUrl]
     k1: str
-    min_withdrawable: MilliSatoshi = Field(..., alias="minWithdrawable")
-    max_withdrawable: MilliSatoshi = Field(..., alias="maxWithdrawable")
+    min_withdrawable: MilliSatoshi = Field(..., alias="minWithdrawable", gt=0)
+    max_withdrawable: MilliSatoshi = Field(..., alias="maxWithdrawable", gt=0)
     default_description: str = Field("", alias="defaultDescription")
 
     @validator("max_withdrawable")
     def max_less_than_min(cls, value, values, **kwargs):  # noqa
         if "min_withdrawable" in values and value < values["min_withdrawable"]:
             raise ValueError("`max_withdrawable` cannot be less than `min_withdrawable`.")
         return value
```

### Comparing `lnurl-0.4.2/lnurl/types.py` & `lnurl-0.5.0/lnurl/types.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 from typing import List, Optional, Tuple, Union
 from urllib.parse import parse_qs
 
 from pydantic import (
     ConstrainedStr,
     HttpUrl,
     Json,
-    PositiveInt,
     ValidationError,
     parse_obj_as,
+    validator,
 )
 from pydantic.errors import UrlHostTldError, UrlSchemeError
 from pydantic.networks import Parts
 from pydantic.validators import str_validator
 
 from .exceptions import InvalidLnurlPayMetadata
-from .helpers import _bech32_decode, _lnurl_clean, _lnurl_decode
+from .helpers import _bech32_decode, _lnurl_clean, lnurl_decode
 
 
 def ctrl_characters_validator(value: str) -> str:
     """Checks for control characters (unicode blocks C0 and C1, plus DEL)."""
     if re.compile(r"[\u0000-\u001f\u007f-\u009f]").search(value):
         raise ValueError
     return value
@@ -126,26 +126,14 @@
             raise UrlHostTldError()
         return host, tld, host_type, rebuild
 
 
 class LightningInvoice(Bech32):
     """Bech32 Lightning invoice."""
 
-    @property
-    def amount(self) -> int:
-        raise NotImplementedError
-
-    @property
-    def prefix(self) -> str:
-        raise NotImplementedError
-
-    @property
-    def h(self):
-        raise NotImplementedError
-
 
 class LightningNodeUri(ReprMixin, str):
     """Remote node address of form `node_key@ip_address:port_number`."""
 
     __slots__ = ("key", "ip", "port")
 
     def __new__(cls, uri: str, **kwargs) -> "LightningNodeUri":
@@ -183,15 +171,15 @@
         bech32 = _lnurl_clean(lightning)
         str.__init__(bech32)
         self.bech32 = Bech32(bech32)
         self.url = url if url else self.__get_url__(bech32)
 
     @classmethod
     def __get_url__(cls, bech32: str) -> Union[OnionUrl, ClearnetUrl, DebugUrl]:
-        url: str = _lnurl_decode(bech32)
+        url: str = lnurl_decode(bech32)
         return parse_obj_as(Union[OnionUrl, ClearnetUrl, DebugUrl], url)  # type: ignore
 
     @classmethod
     def __get_validators__(cls):
         yield str_validator
         yield cls.validate
 
@@ -200,14 +188,37 @@
         return cls(value, url=cls.__get_url__(value))
 
     @property
     def is_login(self) -> bool:
         return "tag" in self.url.query_params and self.url.query_params["tag"] == "login"
 
 
+class LnAddress(ReprMixin, str):
+    """Lightning address of form `user@host`"""
+
+    def __new__(cls, address: str, **_) -> "LnAddress":
+        return str.__new__(cls, address)
+
+    def __init__(self, address: str):
+        str.__init__(address)
+        self.address = address
+        self.url = self.__get_url__(address)
+
+    @validator("address")
+    def is_valid_email_address(cls, email: str) -> bool:
+        email_regex = r"[A-Za-z0-9\._%+-]+@[A-Za-z0-9\.-]+\.[A-Za-z]{2,63}"
+        return re.fullmatch(email_regex, email) is not None
+
+    @classmethod
+    def __get_url__(cls, address: str) -> Union[OnionUrl, ClearnetUrl, DebugUrl]:
+        name, domain = address.split("@")
+        url = ("http://" if domain.endswith(".onion") else "https://") + domain + "/.well-known/lnurlp/" + name
+        return parse_obj_as(Union[OnionUrl, ClearnetUrl, DebugUrl], url)  # type: ignore
+
+
 class LnurlPayMetadata(ReprMixin, str):
     valid_metadata_mime_types = {"text/plain", "image/png;base64", "image/jpeg;base64"}
 
     __slots__ = ("_list",)
 
     def __new__(cls, json_str: str, **kwargs) -> "LnurlPayMetadata":
         return str.__new__(cls, json_str)
@@ -268,11 +279,7 @@
 class InitializationVector(ConstrainedStr):
     min_length = 24
     max_length = 24
 
 
 class Max144Str(ConstrainedStr):
     max_length = 144
-
-
-class MilliSatoshi(PositiveInt):
-    """A thousandth of a satoshi."""
```

### Comparing `lnurl-0.4.2/pyproject.toml` & `lnurl-0.5.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 [tool.poetry]
 name = "lnurl"
-version = "0.4.2"
+version = "0.5.0"
 description = "LNURL implementation for Python."
 authors = ["Alan Bits <alan@lnbits.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
   {include = "lnurl"},
   {include = "lnurl/py.typed"},
 ]
 
 [tool.poetry.scripts]
 lnurl = "lnurl.cli:main"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-requests = "^2.31.0"
 pydantic = "^1"
 bech32 = "^1.2.0"
+ecdsa = "^0.19.0"
+bolt11 = "^2.0.5"
+httpx = "^0.27.0"
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.7.0"
+black = "^24.3.0"
 pytest = "^7.4.0"
 pytest-cov = "^4.1.0"
 types-requests = "^2.31.0.2"
 mypy = "^1.5.1"
 ruff = "^0.0.284"
 pre-commit = "^3.3.3"
+pytest-asyncio = "^0.23.6"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 ignore_missing_imports = "True"
```

### Comparing `lnurl-0.4.2/PKG-INFO` & `lnurl-0.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: lnurl
-Version: 0.4.2
+Version: 0.5.0
 Summary: LNURL implementation for Python.
 License: MIT
 Author: Alan Bits
 Author-email: alan@lnbits.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: bech32 (>=1.2.0,<2.0.0)
+Requires-Dist: bolt11 (>=2.0.5,<3.0.0)
+Requires-Dist: ecdsa (>=0.19.0,<0.20.0)
+Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: pydantic (>=1,<2)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 LNURL implementation for Python
 ===============================
 
 [![github-tests-badge]][github-tests]
 [![github-mypy-badge]][github-mypy]
@@ -68,42 +70,50 @@
 -----------------------
 
 You can use a `LnurlResponse` to wrap responses you get from a LNURL.
 The different types of responses defined in the [LNURL spec][lnurl-spec] have a different model
 with different properties (see `models.py`):
 
 ```python
-import requests
+import httpx
 
 from lnurl import Lnurl, LnurlResponse
 
 lnurl = Lnurl('LNURL1DP68GURN8GHJ7MRWW4EXCTNZD9NHXATW9EU8J730D3H82UNV94MKJARGV3EXZAELWDJHXUMFDAHR6WFHXQERSVPCA649RV')
+try:
+  async with httpx.AsyncClient() as client:
+    r = await client.get(lnurl.url)
+    res = LnurlResponse.from_dict(r.json())  # LnurlPayResponse
+    res.ok  # bool
+    res.max_sendable  # int
+    res.max_sats  # int
+    res.callback.base  # str
+    res.callback.query_params # dict
+    res.metadata  # str
+    res.metadata.list()  # list
+    res.metadata.text  # str
+    res.metadata.images  # list
 r = requests.get(lnurl.url)
-
-res = LnurlResponse.from_dict(r.json())  # LnurlPayResponse
-res.ok  # bool
-res.max_sendable  # int
-res.max_sats  # int
-res.callback.base  # str
-res.callback.query_params # dict
-res.metadata  # str
-res.metadata.list()  # list
-res.metadata.text  # str
-res.metadata.images  # list
 ```
 
-If you have already `requests` installed, you can also use the `.handle()` function directly.
+If you have already `httpx` installed, you can also use the `.handle()` function directly.
 It will return the appropriate response for a LNURL.
 
 ```python
 >>> import lnurl
 >>> lnurl.handle('lightning:LNURL1DP68GURN8GHJ7MRWW4EXCTNZD9NHXATW9EU8J730D3H82UNV94CXZ7FLWDJHXUMFDAHR6V33XCUNSVE38QV6UF')
 LnurlPayResponse(tag='payRequest', callback=WebUrl('https://lnurl.bigsun.xyz/lnurl-pay/callback/2169831', scheme='https', host='lnurl.bigsun.xyz', tld='xyz', host_type='domain', path='/lnurl-pay/callback/2169831'), min_sendable=10000, max_sendable=10000, metadata=LnurlPayMetadata('[["text/plain","NgHaEyaZNDnW iI DsFYdkI"],["image/png;base64","iVBOR...uQmCC"]]'))
 ```
 
+You can execute and LNURL with either payRequest, withdrawRequest or login tag using the `execute` function.
+```python
+>>> import lnurl
+>>> lnurl.execute('lightning:LNURL1DP68GURN8GHJ7MRWW4EXCTNZD9NHXATW9EU8J730D3H82UNV94CXZ7FLWDJHXUMFDAHR6V33XCUNSVE38QV6UF', 100000)
+```
+
 Building your own LNURL responses
 ---------------------------------
 
 For LNURL services, the `lnurl` package can be used to build **valid** responses.
 
 ```python
 from lnurl import LnurlWithdrawResponse
@@ -157,10 +167,10 @@
 Options:
   --help  Show this message and exit.
 
 Commands:
   decode           decode a LNURL
   encode           encode a URL
   handle           handle a LNURL
-  payment-request  make a payment_request
+  execute          execute a LNURL
 ```
```

