# Comparing `tmp/nepattern-0.7.1.tar.gz` & `tmp/nepattern-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nepattern-0.7.1.tar", last modified: Tue Apr 23 09:40:33 2024, max compression
+gzip compressed data, was "nepattern-0.7.2.tar", last modified: Thu Apr 25 09:56:26 2024, max compression
```

## Comparing `nepattern-0.7.1.tar` & `nepattern-0.7.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0     1091 2024-02-24 17:08:26.922234 nepattern-0.7.1/LICENSE
--rw-r--r--   0        0        0      943 2024-02-24 17:08:26.923232 nepattern-0.7.1/README.md
--rw-r--r--   0        0        0     2658 2024-04-21 14:43:28.345665 nepattern-0.7.1/nepattern/__init__.py
--rw-r--r--   0        0        0    29438 2024-04-23 09:22:22.663290 nepattern-0.7.1/nepattern/base.py
--rw-r--r--   0        0        0     4148 2024-02-24 17:08:26.923232 nepattern-0.7.1/nepattern/context.py
--rw-r--r--   0        0        0     1507 2024-04-21 13:33:39.317700 nepattern-0.7.1/nepattern/context.pyi
--rw-r--r--   0        0        0    29733 2024-04-23 09:37:19.191429 nepattern-0.7.1/nepattern/core.py
--rw-r--r--   0        0        0    31324 2024-04-23 09:33:16.089736 nepattern-0.7.1/nepattern/core.pyi
--rw-r--r--   0        0        0       63 2024-02-24 17:08:26.924232 nepattern-0.7.1/nepattern/exception.py
--rw-r--r--   0        0        0       26 2024-02-24 17:08:26.924232 nepattern-0.7.1/nepattern/i18n/.config.json
--rw-r--r--   0        0        0      481 2024-02-24 17:08:26.924232 nepattern-0.7.1/nepattern/i18n/en-US.json
--rw-r--r--   0        0        0      470 2024-02-24 17:08:26.924232 nepattern-0.7.1/nepattern/i18n/zh-CN.json
--rw-r--r--   0        0        0     5611 2024-04-23 09:38:29.355325 nepattern-0.7.1/nepattern/main.py
--rw-r--r--   0        0        0     2186 2024-04-21 13:37:01.346873 nepattern-0.7.1/nepattern/main.pyi
--rw-r--r--   0        0        0     1073 2024-02-24 18:59:34.297506 nepattern-0.7.1/nepattern/util.py
--rw-r--r--   0        0        0     2056 2024-04-23 09:40:33.481176 nepattern-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     1693 1970-01-01 00:00:00.000000 nepattern-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1091 2024-02-24 17:08:26.922234 nepattern-0.7.2/LICENSE
+-rw-r--r--   0        0        0      943 2024-02-24 17:08:26.923232 nepattern-0.7.2/README.md
+-rw-r--r--   0        0        0     3058 2024-04-25 09:22:34.763668 nepattern-0.7.2/nepattern/__init__.py
+-rw-r--r--   0        0        0    29346 2024-04-25 09:49:34.487307 nepattern-0.7.2/nepattern/base.py
+-rw-r--r--   0        0        0     4148 2024-04-25 09:22:34.747677 nepattern-0.7.2/nepattern/context.py
+-rw-r--r--   0        0        0     1525 2024-04-25 09:22:43.597720 nepattern-0.7.2/nepattern/context.pyi
+-rw-r--r--   0        0        0    30111 2024-04-25 09:28:25.729185 nepattern-0.7.2/nepattern/core.py
+-rw-r--r--   0        0        0    34323 2024-04-25 09:28:38.979141 nepattern-0.7.2/nepattern/core.pyi
+-rw-r--r--   0        0        0       63 2024-02-24 17:08:26.924232 nepattern-0.7.2/nepattern/exception.py
+-rw-r--r--   0        0        0     6761 2024-04-25 09:31:42.239930 nepattern-0.7.2/nepattern/func.py
+-rw-r--r--   0        0        0       26 2024-02-24 17:08:26.924232 nepattern-0.7.2/nepattern/i18n/.config.json
+-rw-r--r--   0        0        0      481 2024-02-24 17:08:26.924232 nepattern-0.7.2/nepattern/i18n/en-US.json
+-rw-r--r--   0        0        0      470 2024-02-24 17:08:26.924232 nepattern-0.7.2/nepattern/i18n/zh-CN.json
+-rw-r--r--   0        0        0     5611 2024-04-23 09:38:29.355325 nepattern-0.7.2/nepattern/main.py
+-rw-r--r--   0        0        0     2237 2024-04-25 09:22:43.626718 nepattern-0.7.2/nepattern/main.pyi
+-rw-r--r--   0        0        0     1071 2024-04-25 09:22:43.620721 nepattern-0.7.2/nepattern/util.py
+-rw-r--r--   0        0        0     2065 2024-04-25 09:56:26.393732 nepattern-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     1693 1970-01-01 00:00:00.000000 nepattern-0.7.2/PKG-INFO
```

### Comparing `nepattern-0.7.1/LICENSE` & `nepattern-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nepattern-0.7.1/README.md` & `nepattern-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `nepattern-0.7.1/nepattern/__init__.py` & `nepattern-0.7.2/nepattern/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from typing import Any
 from pathlib import Path
+from typing import Any
 
 from tarina import Empty as Empty  # noqa
 
 from .base import ANY as ANY
 from .base import AntiPattern as AntiPattern
 from .base import AnyString as AnyString
 from .base import BOOLEAN as BOOLEAN
 from .base import BYTES as BYTES
 from .base import DATETIME as DATETIME
-from .base import DelimiterInt as DelimiterInt
 from .base import DICT as DICT
+from .base import DelimiterInt as DelimiterInt
 from .base import DirectPattern as DirectPattern
 from .base import DirectTypePattern as DirectTypePattern
 from .base import EMAIL as EMAIL
 from .base import FLOAT as FLOAT
 from .base import HEX as HEX
 from .base import HEX_COLOR as HEX_COLOR
 from .base import INTEGER as INTEGER
@@ -43,14 +43,26 @@
 from .context import local_patterns as local_patterns
 from .context import reset_local_patterns as reset_local_patterns
 from .context import switch_local_patterns as switch_local_patterns
 from .core import BasePattern as BasePattern
 from .core import MatchMode as MatchMode
 from .core import ValidateResult as ValidateResult
 from .exception import MatchFailed as MatchFailed
+from .func import Dot as Dot
+from .func import Filter as Filter
+from .func import GetItem as GetItem
+from .func import Index as Index
+from .func import Join as Join
+from .func import Lower as Lower
+from .func import Map as Map
+from .func import Reduce as Reduce
+from .func import Slice as Slice
+from .func import Step as Step
+from .func import Sum as Sum
+from .func import Upper as Upper
 from .main import parser as parser
 from .util import RawStr as RawStr
 from .util import TPattern as TPattern
 
 type_parser = parser
 
 global_patterns().update(
```

### Comparing `nepattern-0.7.1/nepattern/base.py` & `nepattern-0.7.2/nepattern/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,141 +1,134 @@
 from __future__ import annotations
 
-from enum import Enum
 from datetime import datetime
+from enum import Enum
 from pathlib import Path
 import re
 import sys
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     ForwardRef,
+    Generic,
     Iterable,
     Literal,
     Match,
     TypeVar,
     Union,
     cast,
     final,
-    overload, Generic,
+    overload,
 )
 
 from tarina import DateParser, Empty, lang
 
-from .core import BasePattern, MatchMode, ResultFlag, ValidateResult, _MATCHES, TMM
+from .core import _MATCHES, TMM, BasePattern, MatchMode, ResultFlag, ValidateResult
 from .exception import MatchFailed
 from .util import TPattern
 
 TOrigin = TypeVar("TOrigin")
 TDefault = TypeVar("TDefault")
 _T = TypeVar("_T")
 _T1 = TypeVar("_T1")
 
 
 class DirectPattern(BasePattern[TOrigin, TOrigin, Literal[MatchMode.KEEP]]):
     """直接判断"""
 
-    __slots__ = ("target",)
-
     def __init__(self, target: TOrigin, alias: str | None = None):
         self.target = target
         super().__init__(mode=MatchMode.KEEP, origin=type(target), alias=alias or str(target))
 
     def match(self, input_: Any):
         if input_ != self.target:
             raise MatchFailed(
                 lang.require("nepattern", "content_error").format(target=input_, expected=self.target)
             )
         return input_
 
     @overload
-    def validate(self, input_: TOrigin) -> ValidateResult[TOrigin, Literal[ResultFlag.VALID]]:
-        ...
+    def validate(self, input_: TOrigin) -> ValidateResult[TOrigin, Literal[ResultFlag.VALID]]: ...
 
     @overload
-    def validate(self, input_: _T) -> ValidateResult[_T, Literal[ResultFlag.ERROR]]:
-        ...
+    def validate(self, input_: _T) -> ValidateResult[_T, Literal[ResultFlag.ERROR]]: ...
 
     @overload
-    def validate(self, input_: TOrigin, default: Any) -> ValidateResult[TOrigin, Literal[ResultFlag.VALID]]:
-        ...
+    def validate(
+        self, input_: TOrigin, default: Any
+    ) -> ValidateResult[TOrigin, Literal[ResultFlag.VALID]]: ...
 
     @overload
     def validate(
         self, input_: Any, default: TDefault
-    ) -> ValidateResult[TDefault, Literal[ResultFlag.DEFAULT]]:
-        ...
+    ) -> ValidateResult[TDefault, Literal[ResultFlag.DEFAULT]]: ...
 
     def validate(self, input_: Any, default: Union[TDefault, Empty] = Empty) -> ValidateResult[TOrigin | TDefault, ResultFlag]:  # type: ignore
-        if input_ == self.target:
-            return ValidateResult(input_, flag=ResultFlag.VALID)
-        e = MatchFailed(
-            lang.require("nepattern", "content_error").format(target=input_, expected=self.target)
-        )
-        if default is Empty:
-            return ValidateResult(error=e, flag=ResultFlag.ERROR)
-        return ValidateResult(default, flag=ResultFlag.DEFAULT)  # type: ignore
+        try:
+            return ValidateResult(self.match(input_), flag=ResultFlag.VALID)
+        except MatchFailed as e:
+            if default is Empty:
+                return ValidateResult(error=e, flag=ResultFlag.ERROR)
+            return ValidateResult(default, flag=ResultFlag.DEFAULT)  # type: ignore
 
     def __calc_eq__(self, other):  # pragma: no cover
         return isinstance(other, DirectPattern) and self.target == other.target
+    
+    def copy(self):
+        return DirectPattern(self.target, self.alias)
 
 
 class DirectTypePattern(BasePattern[TOrigin, TOrigin, Literal[MatchMode.KEEP]]):
     """直接类型判断"""
 
-    __slots__ = ("target",)
-
     def __init__(self, target: type[TOrigin], alias: str | None = None):
         self.target = target
         super().__init__(mode=MatchMode.KEEP, origin=target, alias=alias or target.__name__)
 
     def match(self, input_: Any):
         if not isinstance(input_, self.target):
             raise MatchFailed(
                 lang.require("nepattern", "type_error").format(
                     type=input_.__class__, target=input_, expected=self.target
                 )
             )
         return input_
 
     @overload
-    def validate(self, input_: TOrigin) -> ValidateResult[TOrigin, Literal[ResultFlag.VALID]]:
-        ...
+    def validate(self, input_: TOrigin) -> ValidateResult[TOrigin, Literal[ResultFlag.VALID]]: ...
 
     @overload
-    def validate(self, input_: _T) -> ValidateResult[_T, Literal[ResultFlag.ERROR]]:
-        ...
+    def validate(self, input_: _T) -> ValidateResult[_T, Literal[ResultFlag.ERROR]]: ...
 
     @overload
-    def validate(self, input_: TOrigin, default: Any) -> ValidateResult[TOrigin, Literal[ResultFlag.VALID]]:
-        ...
+    def validate(
+        self, input_: TOrigin, default: Any
+    ) -> ValidateResult[TOrigin, Literal[ResultFlag.VALID]]: ...
 
     @overload
     def validate(
         self, input_: Any, default: TDefault
-    ) -> ValidateResult[TDefault, Literal[ResultFlag.DEFAULT]]:
-        ...
+    ) -> ValidateResult[TDefault, Literal[ResultFlag.DEFAULT]]: ...
 
     def validate(self, input_: Any, default: Union[TDefault, Empty] = Empty) -> ValidateResult[TOrigin | TDefault, ResultFlag]:  # type: ignore
-        if isinstance(input_, self.target):
-            return ValidateResult(input_, flag=ResultFlag.VALID)
-        e = MatchFailed(
-            lang.require("nepattern", "type_error").format(
-                type=input_.__class__, target=input_, expected=self.target
-            )
-        )
-        if default is Empty:
-            return ValidateResult(error=e, flag=ResultFlag.ERROR)
-        return ValidateResult(default, flag=ResultFlag.DEFAULT)  # type: ignore
+        try:
+            return ValidateResult(self.match(input_), flag=ResultFlag.VALID)
+        except MatchFailed as e:
+            if default is Empty:
+                return ValidateResult(error=e, flag=ResultFlag.ERROR)
+            return ValidateResult(default, flag=ResultFlag.DEFAULT)  # type: ignore
 
     def __calc_eq__(self, other):  # pragma: no cover
         return isinstance(other, DirectTypePattern) and self.target == other.target
 
+    def copy(self):
+        return DirectTypePattern(self.target, self.alias)
+
 
 class RegexPattern(BasePattern[Match[str], str, Literal[MatchMode.REGEX_MATCH]]):
     """针对正则的特化匹配，支持正则组"""
 
     def __init__(self, pattern: str | TPattern, alias: str | None = None):
         super().__init__("", origin=Match[str], alias=alias or "regex[:group]")  # type: ignore
         self.regex_pattern = re.compile(pattern)
@@ -153,14 +146,17 @@
         raise MatchFailed(
             lang.require("nepattern", "content_error").format(target=input_, expected=self.pattern)
         )
 
     def __calc_eq__(self, other):  # pragma: no cover
         return isinstance(other, RegexPattern) and self.pattern == other.pattern
 
+    def copy(self):
+        return RegexPattern(self.pattern, self.alias)
+
 
 class UnionPattern(BasePattern[Any, _T, Literal[MatchMode.KEEP]]):
     """多类型参数的匹配"""
 
     optional: bool
     for_validate: list[BasePattern]
     for_equal: list[str | object]
@@ -191,15 +187,15 @@
             for pat in self.for_validate:
                 if (res := pat.validate(input_)).success:
                     return res.value()
             raise MatchFailed(
                 lang.require("nepattern", "content_error").format(target=input_, expected=self.alias)
             )
         return input_
-    
+
     @classmethod
     def _(cls, *types: type[_T1]) -> UnionPattern[_T1]:
         from .main import parser
 
         return cls([parser(i) for i in types])  # type: ignore
 
     def __calc_repr__(self):
@@ -220,15 +216,17 @@
     SUF = "suf"
     ALL = "all"
 
 
 TIterMode = TypeVar("TIterMode", bound=IterMode)
 
 
-class SequencePattern(BasePattern[TSeq, Union[str, TSeq], Literal[MatchMode.REGEX_CONVERT]], Generic[TSeq, TIterMode]):
+class SequencePattern(
+    BasePattern[TSeq, Union[str, TSeq], Literal[MatchMode.REGEX_CONVERT]], Generic[TSeq, TIterMode]
+):
     """匹配列表或者元组或者集合"""
 
     base: BasePattern
     itermode: TIterMode
 
     def __init__(self, form: type[TSeq], base: BasePattern, mode: TIterMode = IterMode.ALL):
         self.base = base
@@ -282,18 +280,18 @@
     """匹配字典或者映射表"""
 
     key: BasePattern[TKey, Any, Any]
     value: BasePattern[TVal, Any, Any]
     itermode: TIterMode
 
     def __init__(
-        self, 
-        arg_key: BasePattern[TKey, Any, Any], 
+        self,
+        arg_key: BasePattern[TKey, Any, Any],
         arg_value: BasePattern[TVal, Any, Any],
-        mode: TIterMode = IterMode.ALL
+        mode: TIterMode = IterMode.ALL,
     ):
         self.key = arg_key
         self.value = arg_value
         self.itermode = mode
         super().__init__(
             r"\{(.+?)\}",
             MatchMode.REGEX_CONVERT,
@@ -372,15 +370,17 @@
     def __calc_eq__(self, other):  # pragma: no cover
         return isinstance(other, SwitchPattern) and self.switch == other.switch
 
 
 class ForwardRefPattern(BasePattern[Any, Any, Literal[MatchMode.TYPE_CONVERT]]):
     def __init__(self, ref: ForwardRef):
         self.ref = ref
-        super().__init__(mode=MatchMode.TYPE_CONVERT, origin=Any, converter=lambda _, x: eval(x), alias=ref.__forward_arg__)
+        super().__init__(
+            mode=MatchMode.TYPE_CONVERT, origin=Any, converter=lambda _, x: eval(x), alias=ref.__forward_arg__
+        )
 
     def match(self, input_: Any):
         if isinstance(input_, str) and input_ == self.ref.__forward_arg__:
             return input_
         _main = sys.modules["__main__"]
         if sys.version_info < (3, 9):  # pragma: no cover
             origin = self.ref._evaluate(_main.__dict__, _main.__dict__)
@@ -400,30 +400,26 @@
 
 class AntiPattern(BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]]):
     def __init__(self, pattern: BasePattern[TOrigin, Any, Any]):
         self.base: BasePattern[TOrigin, Any, Any] = pattern
         super().__init__(mode=MatchMode.TYPE_CONVERT, origin=pattern.origin, alias=f"!{pattern}")
 
     @overload
-    def validate(self, input_: TOrigin) -> ValidateResult[Any, Literal[ResultFlag.ERROR]]:
-        ...
+    def validate(self, input_: TOrigin) -> ValidateResult[Any, Literal[ResultFlag.ERROR]]: ...
 
     @overload
-    def validate(self, input_: _T) -> ValidateResult[_T, Literal[ResultFlag.VALID]]:
-        ...
+    def validate(self, input_: _T) -> ValidateResult[_T, Literal[ResultFlag.VALID]]: ...
 
     @overload
     def validate(
         self, input_: TOrigin, default: TDefault
-    ) -> ValidateResult[TDefault, Literal[ResultFlag.DEFAULT]]:
-        ...
+    ) -> ValidateResult[TDefault, Literal[ResultFlag.DEFAULT]]: ...
 
     @overload
-    def validate(self, input_: _T, default: Any) -> ValidateResult[_T, Literal[ResultFlag.VALID]]:
-        ...
+    def validate(self, input_: _T, default: Any) -> ValidateResult[_T, Literal[ResultFlag.VALID]]: ...
 
     def validate(self, input_: _T, default: Union[TDefault, Empty] = Empty) -> ValidateResult[_T | TDefault, ResultFlag]:  # type: ignore
         """
         对传入的值进行反向验证，返回可能的匹配与转化结果。
 
         若传入默认值，验证失败会返回默认值
         """
@@ -502,37 +498,42 @@
 AnyString = AnyStrPattern()
 """匹配任意内容并转为字符串的表达式"""
 
 
 @final
 class StrPattern(BasePattern[str, Union[str, bytes, bytearray], Literal[MatchMode.TYPE_CONVERT]]):
     def __init__(self):
-        super().__init__(mode=MatchMode.TYPE_CONVERT, origin=str, accepts=Union[str, bytes, bytearray], alias="str")
+        super().__init__(
+            mode=MatchMode.TYPE_CONVERT, origin=str, accepts=Union[str, bytes, bytearray], alias="str"
+        )
 
     def match(self, input_: Any) -> str:
         if isinstance(input_, str):
             return input_.value if isinstance(input_, Enum) else input_
         elif isinstance(input_, (bytes, bytearray)):
             return input_.decode()
         raise MatchFailed(
-            lang.require("nepattern", "type_error")
-            .format(type=input_.__class__, target=input_, expected="str | bytes | bytearray")
+            lang.require("nepattern", "type_error").format(
+                type=input_.__class__, target=input_, expected="str | bytes | bytearray"
+            )
         )
 
     def __calc_eq__(self, other):  # pragma: no cover
         return other.__class__ is StrPattern
 
 
 STRING = StrPattern()
 
 
 @final
 class BytesPattern(BasePattern[bytes, Union[str, bytes, bytearray], Literal[MatchMode.TYPE_CONVERT]]):
     def __init__(self):
-        super().__init__(mode=MatchMode.TYPE_CONVERT, origin=bytes, accepts=Union[str, bytes, bytearray], alias="bytes")
+        super().__init__(
+            mode=MatchMode.TYPE_CONVERT, origin=bytes, accepts=Union[str, bytes, bytearray], alias="bytes"
+        )
 
     def match(self, input_: Any) -> bytes:
         if isinstance(input_, bytes):
             return input_
         elif isinstance(input_, bytearray):
             return bytes(input_)
         elif isinstance(input_, str):
@@ -635,33 +636,31 @@
             input_ = input_.decode()
         if isinstance(input_, str):
             input_ = input_.lower()
         if input_ == "true":
             return True
         if input_ == "false":
             return False
-        raise MatchFailed(
-            lang.require("nepattern", "content_error").format(target=input_, expected="bool")
-        )
+        raise MatchFailed(lang.require("nepattern", "content_error").format(target=input_, expected="bool"))
 
     def __calc_eq__(self, other):  # pragma: no cover
         return other.__class__ is BoolPattern
 
 
 BOOLEAN = BoolPattern()
 """布尔表达式，只能接受true或false样式的量"""
 
 
 @final
 class WideBoolPattern(BasePattern[bool, Any, Literal[MatchMode.TYPE_CONVERT]]):
     def __init__(self):
         super().__init__(mode=MatchMode.TYPE_CONVERT, origin=bool, alias="bool")
 
-    BOOL_FALSE = {0, '0', 'off', 'f', 'false', 'n', 'no'}
-    BOOL_TRUE = {1, '1', 'on', 't', 'true', 'y', 'yes'}
+    BOOL_FALSE = {0, "0", "off", "f", "false", "n", "no"}
+    BOOL_TRUE = {1, "1", "on", "t", "true", "y", "yes"}
 
     def match(self, input_: Any) -> bool:
         if input_ is True or input_ is False:
             return input_
         if isinstance(input_, bytes):  # pragma: no cover
             input_ = input_.decode()
         if isinstance(input_, str):
@@ -672,16 +671,17 @@
             if input_ in self.BOOL_FALSE:
                 return False
             raise MatchFailed(
                 lang.require("nepattern", "content_error").format(target=input_, expected="bool")
             )
         except (ValueError, TypeError) as e:
             raise MatchFailed(
-                lang.require("nepattern", "type_error")
-                .format(type=input_.__class__, target=input_, expected="bool")
+                lang.require("nepattern", "type_error").format(
+                    type=input_.__class__, target=input_, expected="bool"
+                )
             ) from e
 
     def __calc_eq__(self, other):  # pragma: no cover
         return other.__class__ is BoolPattern
 
 
 WIDE_BOOLEAN = WideBoolPattern()
@@ -724,15 +724,15 @@
             )
         try:
             return int(input_, 16)
         except ValueError as e:
             raise MatchFailed(
                 lang.require("nepattern", "content_error").format(target=input_, expected="hex")
             ) from e
-    
+
     def __calc_eq__(self, other):  # pragma: no cover
         return other.__class__ is HexPattern
 
 
 HEX = HexPattern()
 """匹配16进制数的表达式"""
 
@@ -796,15 +796,15 @@
     alias="filedata",
     converter=lambda _, x: x.read_bytes() if x.exists() and x.is_file() else None,
 )
 
 
 def combine(
     current: BasePattern[TOrigin, TInput, TMM],
-    previous: BasePattern[Any, Any, Literal[MatchMode.VALUE_OPERATE]] | None = None,
+    previous: BasePattern[TInput, Any, Any] | None = None,
     alias: str | None = None,
     validators: list[Callable[[TOrigin], bool]] | None = None,
 ) -> BasePattern[TOrigin, TInput, TMM]:
     _new = current.copy()
     if previous:
         _match = _new.match
```

### Comparing `nepattern-0.7.1/nepattern/context.py` & `nepattern-0.7.2/nepattern/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from collections import UserDict
 from contextvars import ContextVar, Token
 from typing import final
 
 from tarina import Empty
 
-from .base import UnionPattern, NONE
+from .base import NONE, UnionPattern
 
 
 @final
 class Patterns(UserDict):
     def __init__(self, name):
         self.name = name
         super().__init__({"": NONE})
```

### Comparing `nepattern-0.7.1/nepattern/context.pyi` & `nepattern-0.7.2/nepattern/context.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -3,25 +3,28 @@
 
 from .core import BasePattern
 
 @final
 class Patterns(UserDict[Any, BasePattern]):
     name: str
     def __init__(self, name: str): ...
-    def set(self, target: BasePattern[Any, Any, Any], alias: str | None = None, cover: bool = True, no_alias=False):
+    def set(
+        self, target: BasePattern[Any, Any, Any], alias: str | None = None, cover: bool = True, no_alias=False
+    ):
         """
         增加可使用的类型转换器
 
         Args:
             target: 设置的表达式
             alias: 目标类型的别名
             cover: 是否覆盖已有的转换器
             no_alias: 是否不使用目标类型自带的别名
         """
         ...
+
     def sets(self, patterns: Iterable[BasePattern[Any, Any, Any]], cover: bool = True, no_alias=False): ...
     def merge(self, patterns: dict[str, BasePattern[Any, Any, Any]], no_alias=False): ...
     def remove(self, origin_type: type, alias: str | None = None): ...
 
 def create_local_patterns(
     name: str,
     data: dict[Any, BasePattern[Any, Any, Any]] | None = None,
```

### Comparing `nepattern-0.7.1/nepattern/core.py` & `nepattern-0.7.2/nepattern/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from copy import deepcopy
 from enum import Enum, IntEnum
 import re
-from typing import Any, Callable, Generic, Literal, TypeVar, TYPE_CHECKING
+from typing import TYPE_CHECKING, Any, Callable, Generic, Literal, TypeVar
 from typing_extensions import Self, get_args, get_origin
 
 from tarina import Empty, generic_isinstance
 from tarina.lang import lang
 
 from .exception import MatchFailed
 
@@ -122,15 +122,15 @@
         )
     return input_
 
 
 def _keep_previous(self: BasePattern[Any, Any, Literal[MatchMode.KEEP]], input_: Any) -> Any:
     if TYPE_CHECKING:
         assert self.previous
-    if self.accept(input_):    
+    if self.accept(input_):
         input_ = self.previous.match(input_)
     elif not self.accept(input_ := self.previous.match(input_)):
         raise MatchFailed(
             lang.require("nepattern", "type_error").format(
                 type=input_.__class__, target=input_, expected=self.alias
             )
         )
@@ -154,15 +154,17 @@
         return mat[0]
     raise MatchFailed(lang.require("nepattern", "content_error").format(target=input_, expected=self.alias))
 
 
 def _regex_match_type(self: BasePattern[str, str, Literal[MatchMode.REGEX_MATCH]], input_: Any) -> str:
     if TYPE_CHECKING:
         assert self.previous
-    if not isinstance(input_, str) and not isinstance(input_ := self.previous.match(input_), str):  # pragma: no cover
+    if not isinstance(input_, str) and not isinstance(
+        input_ := self.previous.match(input_), str
+    ):  # pragma: no cover
         raise MatchFailed(
             lang.require("nepattern", "type_error").format(
                 type=input_.__class__, target=input_, expected=self.alias
             )
         )
     if mat := (self.regex_pattern.match(input_) or self.regex_pattern.search(input_)):
         return mat[0]
@@ -188,58 +190,66 @@
     if self.previous:
         if self.previous.mode == MatchMode.TYPE_CONVERT:
             return _regex_match_type
         return _regex_match_value
     return _regex_match_no_previous
 
 
-def _regex_convert_no_previous_any(self: BasePattern[TOrigin, str | TOrigin, Literal[MatchMode.REGEX_CONVERT]], input_: Any) -> TOrigin:
+def _regex_convert_no_previous_any(
+    self: BasePattern[TOrigin, str | TOrigin, Literal[MatchMode.REGEX_CONVERT]], input_: Any
+) -> TOrigin:
     if not isinstance(input_, str):
         raise MatchFailed(
             lang.require("nepattern", "type_error").format(
                 type=input_.__class__, target=input_, expected=self.alias
             )
         )
     if mat := (self.regex_pattern.match(input_) or self.regex_pattern.search(input_)):
         if (res := self.converter(self, mat)) is not None:
             return res
     raise MatchFailed(lang.require("nepattern", "content_error").format(target=input_, expected=self.alias))
 
 
-def _regex_convert_no_previous_other(self: BasePattern[TOrigin, str | TOrigin, Literal[MatchMode.REGEX_CONVERT]], input_: Any) -> TOrigin:
+def _regex_convert_no_previous_other(
+    self: BasePattern[TOrigin, str | TOrigin, Literal[MatchMode.REGEX_CONVERT]], input_: Any
+) -> TOrigin:
     if generic_isinstance(input_, self.origin):
         return input_  # type: ignore
     if not isinstance(input_, str):
         raise MatchFailed(
             lang.require("nepattern", "type_error").format(
                 type=input_.__class__, target=input_, expected=self.alias
             )
         )
     if mat := (self.regex_pattern.match(input_) or self.regex_pattern.search(input_)):
         if (res := self.converter(self, mat)) is not None:
             return res
     raise MatchFailed(lang.require("nepattern", "content_error").format(target=input_, expected=self.alias))
 
 
-def _regex_convert_any_type(self: BasePattern[TOrigin, str | TOrigin, Literal[MatchMode.REGEX_CONVERT]], input_: Any) -> TOrigin:
+def _regex_convert_any_type(
+    self: BasePattern[TOrigin, str | TOrigin, Literal[MatchMode.REGEX_CONVERT]], input_: Any
+) -> TOrigin:
     if TYPE_CHECKING:
         assert self.previous
     if not isinstance(input_, str) and not isinstance(input_ := self.previous.match(input_), str):
         raise MatchFailed(
             lang.require("nepattern", "type_error").format(
                 type=input_.__class__, target=input_, expected=self.alias
             )
         )
     if mat := (self.regex_pattern.match(input_) or self.regex_pattern.search(input_)):
         if (res := self.converter(self, mat)) is not None:
             return res
     raise MatchFailed(lang.require("nepattern", "content_error").format(target=input_, expected=self.alias))
 
 
-def _regex_convert_any_value(self: BasePattern[TOrigin, str | TOrigin, Literal[MatchMode.REGEX_CONVERT]], input_: Any) -> TOrigin:
+def _regex_convert_any_value(
+    self: BasePattern[TOrigin, str | TOrigin, Literal[MatchMode.REGEX_CONVERT]], input_: Any
+) -> TOrigin:
     if TYPE_CHECKING:
         assert self.previous
     if not isinstance(input_, str):
         raise MatchFailed(
             lang.require("nepattern", "type_error").format(
                 type=input_.__class__, target=input_, expected=self.alias
             )
@@ -247,15 +257,17 @@
     input_ = self.previous.match(input_)
     if mat := (self.regex_pattern.match(input_) or self.regex_pattern.search(input_)):
         if (res := self.converter(self, mat)) is not None:
             return res
     raise MatchFailed(lang.require("nepattern", "content_error").format(target=input_, expected=self.alias))
 
 
-def _regex_convert_value(self: BasePattern[TOrigin, str | TOrigin, Literal[MatchMode.REGEX_CONVERT]], input_: Any) -> TOrigin:
+def _regex_convert_value(
+    self: BasePattern[TOrigin, str | TOrigin, Literal[MatchMode.REGEX_CONVERT]], input_: Any
+) -> TOrigin:
     if TYPE_CHECKING:
         assert self.previous
     input_ = self.previous.match(input_)
     if generic_isinstance(input_, self.origin):
         return input_  # type: ignore
     if not isinstance(input_, str):
         raise MatchFailed(
@@ -265,15 +277,17 @@
         )
     if mat := (self.regex_pattern.match(input_) or self.regex_pattern.search(input_)):
         if (res := self.converter(self, mat)) is not None:
             return res
     raise MatchFailed(lang.require("nepattern", "content_error").format(target=input_, expected=self.alias))
 
 
-def _regex_convert_type(self: BasePattern[TOrigin, str | TOrigin, Literal[MatchMode.REGEX_CONVERT]], input_: Any) -> TOrigin:
+def _regex_convert_type(
+    self: BasePattern[TOrigin, str | TOrigin, Literal[MatchMode.REGEX_CONVERT]], input_: Any
+) -> TOrigin:
     if TYPE_CHECKING:
         assert self.previous
     if generic_isinstance(input_, self.origin):
         return input_  # type: ignore
     if not isinstance(input_, str) and not isinstance(input_ := self.previous.match(input_), str):
         raise MatchFailed(
             lang.require("nepattern", "type_error").format(
@@ -286,55 +300,67 @@
     raise MatchFailed(lang.require("nepattern", "content_error").format(target=input_, expected=self.alias))
 
 
 def select_regex_convert(self: BasePattern[Any, Any, Literal[MatchMode.REGEX_CONVERT]]):
     if self.origin is Any or self.origin is str:
         if not self.previous:
             return _regex_convert_no_previous_any
-        return _regex_convert_any_value if self.previous.mode == MatchMode.VALUE_OPERATE else _regex_convert_any_type
+        return (
+            _regex_convert_any_value
+            if self.previous.mode == MatchMode.VALUE_OPERATE
+            else _regex_convert_any_type
+        )
     if not self.previous:
         return _regex_convert_no_previous_other
     if self.previous.mode == MatchMode.VALUE_OPERATE:
         return _regex_convert_value
     return _regex_convert_type
 
 
-def _type_convert_no_previous_no_accepts_any(self: BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]], input_: Any) -> TOrigin:
+def _type_convert_no_previous_no_accepts_any(
+    self: BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]], input_: Any
+) -> TOrigin:
     if (res := self.converter(self, input_)) is None:
         raise MatchFailed(
             lang.require("nepattern", "content_error").format(target=input_, expected=self.alias)
         )
     return res  # type: ignore
 
 
-def _type_convert_no_previous_no_accepts_other(self: BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]], input_: Any) -> TOrigin:
+def _type_convert_no_previous_no_accepts_other(
+    self: BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]], input_: Any
+) -> TOrigin:
     if generic_isinstance(input_, self.origin):
         return input_
     if (res := self.converter(self, input_)) is None:
         raise MatchFailed(
             lang.require("nepattern", "content_error").format(target=input_, expected=self.alias)
         )
     return res  # type: ignore
 
 
-def _type_convert_no_previous_accepts_any(self: BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]], input_: Any) -> TOrigin:
+def _type_convert_no_previous_accepts_any(
+    self: BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]], input_: Any
+) -> TOrigin:
     if not self.accept(input_):
         raise MatchFailed(
             lang.require("nepattern", "type_error").format(
                 type=input_.__class__, target=input_, expected=self.alias
             )
         )
     if (res := self.converter(self, input_)) is None:
         raise MatchFailed(
             lang.require("nepattern", "content_error").format(target=input_, expected=self.alias)
         )
     return res  # type: ignore
 
 
-def _type_convert_no_previous_accepts_other(self: BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]], input_: Any) -> TOrigin:
+def _type_convert_no_previous_accepts_other(
+    self: BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]], input_: Any
+) -> TOrigin:
     if not self.accept(input_):
         raise MatchFailed(
             lang.require("nepattern", "type_error").format(
                 type=input_.__class__, target=input_, expected=self.alias
             )
         )
     if generic_isinstance(input_, self.origin):
@@ -342,95 +368,117 @@
     if (res := self.converter(self, input_)) is None:
         raise MatchFailed(
             lang.require("nepattern", "content_error").format(target=input_, expected=self.alias)
         )
     return res  # type: ignore
 
 
-def _type_convert_type_no_accepts_any(self: BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]], input_: Any) -> TOrigin:
+def _type_convert_type_no_accepts_any(
+    self: BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]], input_: Any
+) -> TOrigin:
     if TYPE_CHECKING:
         assert self.previous
-    if (res := self.converter(self, input_)) is None and (res := self.converter(self, self.previous.match(input_))) is None:
+    if (res := self.converter(self, input_)) is None and (
+        res := self.converter(self, self.previous.match(input_))
+    ) is None:
         raise MatchFailed(
             lang.require("nepattern", "content_error").format(target=input_, expected=self.alias)
         )
     return res  # type: ignore
 
 
-def _type_convert_type_no_accepts_other(self: BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]], input_: Any) -> TOrigin:
+def _type_convert_type_no_accepts_other(
+    self: BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]], input_: Any
+) -> TOrigin:
     if TYPE_CHECKING:
         assert self.previous
     if generic_isinstance(input_, self.origin):
         return input_
-    if (res := self.converter(self, input_)) is None and (res := self.converter(self, self.previous.match(input_))) is None:
+    if (res := self.converter(self, input_)) is None and (
+        res := self.converter(self, self.previous.match(input_))
+    ) is None:
         raise MatchFailed(
             lang.require("nepattern", "content_error").format(target=input_, expected=self.alias)
         )
     return res  # type: ignore
 
 
-def _type_convert_type_accepts_any(self: BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]], input_: Any) -> TOrigin:
+def _type_convert_type_accepts_any(
+    self: BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]], input_: Any
+) -> TOrigin:
     if TYPE_CHECKING:
         assert self.previous
     if not self.accept(input_) and not self.accept(input_ := self.previous.match(input_)):
         raise MatchFailed(
             lang.require("nepattern", "type_error").format(
                 type=input_.__class__, target=input_, expected=self.alias
             )
         )
-    if (res := self.converter(self, input_)) is None and (res := self.converter(self, self.previous.match(input_))) is None:
+    if (res := self.converter(self, input_)) is None and (
+        res := self.converter(self, self.previous.match(input_))
+    ) is None:
         raise MatchFailed(
             lang.require("nepattern", "content_error").format(target=input_, expected=self.alias)
         )
     return res  # type: ignore
 
 
-def _type_convert_type_accepts_other(self: BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]], input_: Any) -> TOrigin:
+def _type_convert_type_accepts_other(
+    self: BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]], input_: Any
+) -> TOrigin:
     if TYPE_CHECKING:
         assert self.previous
     if not self.accept(input_) and not self.accept(input_ := self.previous.match(input_)):
         raise MatchFailed(
             lang.require("nepattern", "type_error").format(
                 type=input_.__class__, target=input_, expected=self.alias
             )
         )
     if generic_isinstance(input_, self.origin):
         return input_
-    if (res := self.converter(self, input_)) is None and (res := self.converter(self, self.previous.match(input_))) is None:
+    if (res := self.converter(self, input_)) is None and (
+        res := self.converter(self, self.previous.match(input_))
+    ) is None:
         raise MatchFailed(
             lang.require("nepattern", "content_error").format(target=input_, expected=self.alias)
         )
     return res  # type: ignore
 
 
-def _type_convert_value_no_accepts_any(self: BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]], input_: Any) -> TOrigin:
+def _type_convert_value_no_accepts_any(
+    self: BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]], input_: Any
+) -> TOrigin:
     if TYPE_CHECKING:
         assert self.previous
     input_ = self.previous.match(input_)
     if (res := self.converter(self, input_)) is None:
         raise MatchFailed(
             lang.require("nepattern", "content_error").format(target=input_, expected=self.alias)
         )
     return res  # type: ignore
 
 
-def _type_convert_value_no_accepts_other(self: BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]], input_: Any) -> TOrigin:
+def _type_convert_value_no_accepts_other(
+    self: BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]], input_: Any
+) -> TOrigin:
     if TYPE_CHECKING:
         assert self.previous
     input_ = self.previous.match(input_)
     if generic_isinstance(input_, self.origin):
         return input_
     if (res := self.converter(self, input_)) is None:
         raise MatchFailed(
             lang.require("nepattern", "content_error").format(target=input_, expected=self.alias)
         )
     return res  # type: ignore
 
 
-def _type_convert_value_accepts_any(self: BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]], input_: Any) -> TOrigin:
+def _type_convert_value_accepts_any(
+    self: BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]], input_: Any
+) -> TOrigin:
     if TYPE_CHECKING:
         assert self.previous
     if self.accept(input_):
         input_ = self.previous.match(input_)
     elif not self.accept(input_ := self.previous.match(input_)):
         raise MatchFailed(
             lang.require("nepattern", "type_error").format(
@@ -440,15 +488,17 @@
     if (res := self.converter(self, input_)) is None:
         raise MatchFailed(
             lang.require("nepattern", "content_error").format(target=input_, expected=self.alias)
         )
     return res  # type: ignore
 
 
-def _type_convert_value_accepts_other(self: BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]], input_: Any) -> TOrigin:
+def _type_convert_value_accepts_other(
+    self: BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]], input_: Any
+) -> TOrigin:
     if TYPE_CHECKING:
         assert self.previous
     if self.accept(input_):
         input_ = self.previous.match(input_)
     elif not self.accept(input_ := self.previous.match(input_)):
         raise MatchFailed(
             lang.require("nepattern", "type_error").format(
@@ -478,45 +528,53 @@
             return _type_convert_no_previous_no_accepts_any
         return _type_convert_value_no_accepts_any if self.previous else _type_convert_type_no_accepts_any
     if not self.previous:
         return _type_convert_no_previous_no_accepts_other
     return _type_convert_value_no_accepts_other if self.previous else _type_convert_type_no_accepts_other
 
 
-def _value_operate_no_previous(self: BasePattern[TOrigin, TOrigin, Literal[MatchMode.VALUE_OPERATE]], input_: Any) -> TOrigin:
+def _value_operate_no_previous(
+    self: BasePattern[TOrigin, TOrigin, Literal[MatchMode.VALUE_OPERATE]], input_: Any
+) -> TOrigin:
     if not generic_isinstance(input_, self.origin):
         raise MatchFailed(
             lang.require("nepattern", "type_error").format(
                 type=input_.__class__, target=input_, expected=self.alias
             )
         )
     if (res := self.converter(self, input_)) is None:
         raise MatchFailed(
             lang.require("nepattern", "content_error").format(target=input_, expected=self.alias)
         )
     return res  # type: ignore
 
 
-def _value_operate_type(self: BasePattern[TOrigin, TOrigin, Literal[MatchMode.VALUE_OPERATE]], input_: Any) -> TOrigin:
+def _value_operate_type(
+    self: BasePattern[TOrigin, TOrigin, Literal[MatchMode.VALUE_OPERATE]], input_: Any
+) -> TOrigin:
     if TYPE_CHECKING:
         assert self.previous
-    if not generic_isinstance(input_, self.origin) and not generic_isinstance(input_ := self.previous.match(input_), self.origin):
+    if not generic_isinstance(input_, self.origin) and not generic_isinstance(
+        input_ := self.previous.match(input_), self.origin
+    ):
         raise MatchFailed(
             lang.require("nepattern", "type_error").format(
                 type=input_.__class__, target=input_, expected=self.alias
             )
         )
     if (res := self.converter(self, input_)) is None:
         raise MatchFailed(
             lang.require("nepattern", "content_error").format(target=input_, expected=self.alias)
         )
     return res  # type: ignore
 
 
-def _value_operate_value(self: BasePattern[TOrigin, TOrigin, Literal[MatchMode.VALUE_OPERATE]], input_: Any) -> TOrigin:
+def _value_operate_value(
+    self: BasePattern[TOrigin, TOrigin, Literal[MatchMode.VALUE_OPERATE]], input_: Any
+) -> TOrigin:
     if TYPE_CHECKING:
         assert self.previous
     if not generic_isinstance(input_, self.origin):
         raise MatchFailed(
             lang.require("nepattern", "type_error").format(
                 type=input_.__class__, target=input_, expected=self.alias
             )
@@ -532,14 +590,15 @@
 def select_value_operate(self: BasePattern[Any, Any, Literal[MatchMode.VALUE_OPERATE]]):
     if self.previous:
         if self.previous.mode == MatchMode.TYPE_CONVERT:
             return _value_operate_type
         return _value_operate_value
     return _value_operate_no_previous
 
+
 _MATCHES = {
     MatchMode.KEEP: select_keep_match,
     MatchMode.REGEX_MATCH: select_regex_match,
     MatchMode.REGEX_CONVERT: select_regex_convert,
     MatchMode.TYPE_CONVERT: select_type_convert,
     MatchMode.VALUE_OPERATE: select_value_operate,
 }
@@ -587,15 +646,17 @@
         if pattern is None:
             _origin = origin or Any
             self.mode = MatchMode(mode or MatchMode.KEEP)
             self.pattern = ""
             self.regex_pattern = re.compile("")
         else:
             if pattern.startswith("^") or pattern.endswith("$"):
-                raise ValueError(lang.require("nepattern", "pattern_head_or_tail_error").format(target=pattern))
+                raise ValueError(
+                    lang.require("nepattern", "pattern_head_or_tail_error").format(target=pattern)
+                )
             self.pattern = pattern
             self.regex_pattern = re.compile(f"^{pattern}$")
             self.mode = MatchMode(mode or MatchMode.REGEX_MATCH)
             _origin = origin or str
         self.origin: type[TOrigin] = _origin  # type: ignore
         self.alias = alias
         self.previous = previous
@@ -634,15 +695,17 @@
             self.match = _MATCHES[self.mode](self).__get__(self)  # type: ignore
 
     def refresh(self):  # pragma: no cover
         self._repr = self.__calc_repr__()
         self._hash = self.__calc_hash__()
 
     def __calc_hash__(self):
-        return hash((self._repr, self.origin, self.mode, self.alias, self.previous, self._accepts, self.pattern))
+        return hash(
+            (self._repr, self.origin, self.mode, self.alias, self.previous, self._accepts, self.pattern)
+        )
 
     def __calc_repr__(self):
         if self.mode == MatchMode.KEEP:
             if self.alias:
                 return self.alias
             return (
                 "Any"
```

### Comparing `nepattern-0.7.1/nepattern/core.pyi` & `nepattern-0.7.2/nepattern/core.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -92,20 +92,24 @@
     @overload
     def __rshift__(self, other: type[T]) -> T: ...
     @overload
     def __rshift__(self, other: Callable[[TVOrigin], T]) -> T: ...
     @overload
     def __rshift__(self, other: Any) -> Self: ...
     @overload
-    def __bool__(self: ValidateResult[TVOrigin, Literal[ResultFlag.VALID]] | ValidateResult[TVOrigin, Literal[ResultFlag.DEFAULT]]) -> Literal[True]: ...
+    def __bool__(
+        self: (
+            ValidateResult[TVOrigin, Literal[ResultFlag.VALID]]
+            | ValidateResult[TVOrigin, Literal[ResultFlag.DEFAULT]]
+        )
+    ) -> Literal[True]: ...
     @overload
     def __bool__(self: ValidateResult[TVOrigin, Literal[ResultFlag.ERROR]]) -> Literal[False]: ...
     def __repr__(self): ...
 
-
 _MATCHES: dict[MatchMode, Callable[[Any], Callable[[Any, Any], Any]]] = {}
 
 class BasePattern(Generic[TOrigin, TInput, TMM]):
     """对参数类型值的包装"""
 
     regex_pattern: TPattern  # type: ignore
     pattern: str
@@ -246,436 +250,618 @@
     ): ...
     @overload
     def __init__(
         self: BasePattern[TOrigin, str | TOrigin, Literal[MatchMode.REGEX_CONVERT]],
         pattern: str,
         mode: Literal[MatchMode.REGEX_CONVERT],
         origin: type[TOrigin],
-        converter: Callable[[BasePattern[TOrigin, str | TOrigin, Literal[MatchMode.REGEX_CONVERT]], re.Match[str]], TOrigin | None]
-        | None = None,
+        converter: (
+            Callable[
+                [BasePattern[TOrigin, str | TOrigin, Literal[MatchMode.REGEX_CONVERT]], re.Match[str]],
+                TOrigin | None,
+            ]
+            | None
+        ) = None,
         alias: str | None = None,
         previous: None = None,
         accepts: type[str] = str,
         addition_accepts: None = None,
         validators: list[Callable[[TOrigin], bool]] | None = None,
     ): ...
     @overload
     def __init__(
         self: BasePattern[TOrigin, str | TOrigin | TInput1, Literal[MatchMode.REGEX_CONVERT]],
         pattern: str,
         mode: Literal[MatchMode.REGEX_CONVERT],
         origin: type[TOrigin],
-        previous: BasePattern[str | TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]] | BasePattern[str, TInput1, Literal[MatchMode.TYPE_CONVERT]] | BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]],
-        converter: Callable[[BasePattern[TOrigin, str | TOrigin | TInput1, Literal[MatchMode.REGEX_CONVERT]], re.Match[str]], TOrigin | None]
-        | None = None,
+        previous: (
+            BasePattern[str | TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]]
+            | BasePattern[str, TInput1, Literal[MatchMode.TYPE_CONVERT]]
+            | BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]]
+        ),
+        converter: (
+            Callable[
+                [
+                    BasePattern[TOrigin, str | TOrigin | TInput1, Literal[MatchMode.REGEX_CONVERT]],
+                    re.Match[str],
+                ],
+                TOrigin | None,
+            ]
+            | None
+        ) = None,
         alias: str | None = None,
         accepts: type[str] = str,
         addition_accepts: None = None,
         validators: list[Callable[[TOrigin], bool]] | None = None,
     ): ...
     @overload
     def __init__(
         self: BasePattern[TOrigin, str | TOrigin, Literal[MatchMode.REGEX_CONVERT]],
         pattern: str,
         mode: Literal[MatchMode.REGEX_CONVERT],
         origin: type[TOrigin],
-        previous: BasePattern[str | TOrigin, str | TOrigin, Literal[MatchMode.VALUE_OPERATE]] | BasePattern[str, str, Literal[MatchMode.VALUE_OPERATE]] | BasePattern[TOrigin, TOrigin, Literal[MatchMode.VALUE_OPERATE]],
-        converter: Callable[[BasePattern[TOrigin, str | TOrigin, Literal[MatchMode.REGEX_CONVERT]], re.Match[str]], TOrigin | None]
-        | None = None,
+        previous: (
+            BasePattern[str | TOrigin, str | TOrigin, Literal[MatchMode.VALUE_OPERATE]]
+            | BasePattern[str, str, Literal[MatchMode.VALUE_OPERATE]]
+            | BasePattern[TOrigin, TOrigin, Literal[MatchMode.VALUE_OPERATE]]
+        ),
+        converter: (
+            Callable[
+                [BasePattern[TOrigin, str | TOrigin, Literal[MatchMode.REGEX_CONVERT]], re.Match[str]],
+                TOrigin | None,
+            ]
+            | None
+        ) = None,
         alias: str | None = None,
         accepts: type[str] = str,
         addition_accepts: None = None,
         validators: list[Callable[[TOrigin], bool]] | None = None,
     ): ...
     @overload
     def __init__(
         self: BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
-        converter: Callable[[BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]], Any], TOrigin | None],
-        origin:  None = None,
+        converter: Callable[
+            [BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]], Any], TOrigin | None
+        ],
+        origin: None = None,
         alias: str | None = None,
         previous: None = None,
         accepts: None = None,
         addition_accepts: None = None,
         validators: list[Callable[[TOrigin], bool]] | None = None,
     ): ...
     @overload
     def __init__(
         self: BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
         accepts: type[TInput1],
-        converter: Callable[[BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]], TInput1], TOrigin | None],
-        origin:  None = None,
+        converter: Callable[
+            [BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]], TInput1], TOrigin | None
+        ],
+        origin: None = None,
         alias: str | None = None,
         previous: None = None,
         addition_accepts: None = None,
         validators: list[Callable[[TOrigin], bool]] | None = None,
     ): ...
     @overload
     def __init__(
         self: BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
         addition_accepts: BasePattern[Any, TInput1, Any],
-        converter: Callable[[BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]], TInput1], TOrigin | None],
-        origin:  None = None,
+        converter: Callable[
+            [BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]], TInput1], TOrigin | None
+        ],
+        origin: None = None,
         alias: str | None = None,
         previous: None = None,
         accepts: None = None,
         validators: list[Callable[[TOrigin], bool]] | None = None,
     ): ...
     @overload
     def __init__(
         self: BasePattern[TOrigin, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
         accepts: type[TInput1],
         addition_accepts: BasePattern[Any, TInput2, Any],
-        converter: Callable[[BasePattern[TOrigin, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]], TInput1 | TInput2], TOrigin | None],
-        origin:  None = None,
+        converter: Callable[
+            [BasePattern[TOrigin, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]], TInput1 | TInput2],
+            TOrigin | None,
+        ],
+        origin: None = None,
         alias: str | None = None,
         previous: None = None,
         validators: list[Callable[[TOrigin], bool]] | None = None,
     ): ...
     @overload
     def __init__(
         self: BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
         origin: type[TOrigin],
-        converter: Callable[[BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]], Any], TOrigin | None] | None = None,
+        converter: (
+            Callable[[BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]], Any], TOrigin | None] | None
+        ) = None,
         alias: str | None = None,
         previous: None = None,
         accepts: None = None,
         addition_accepts: None = None,
         validators: list[Callable[[TOrigin], bool]] | None = None,
     ): ...
     @overload
     def __init__(
         self: BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
         origin: type[TOrigin],
         accepts: type[TInput1],
-        converter: Callable[[BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]], TInput1], TOrigin | None] | None = None,
+        converter: (
+            Callable[
+                [BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]], TInput1], TOrigin | None
+            ]
+            | None
+        ) = None,
         alias: str | None = None,
         previous: None = None,
         addition_accepts: None = None,
         validators: list[Callable[[TOrigin], bool]] | None = None,
     ): ...
     @overload
     def __init__(
         self: BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
         origin: type[TOrigin],
         addition_accepts: BasePattern[Any, TInput1, Any],
-        converter: Callable[[BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]], TInput1], TOrigin | None] | None = None,
+        converter: (
+            Callable[
+                [BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]], TInput1], TOrigin | None
+            ]
+            | None
+        ) = None,
         alias: str | None = None,
         previous: None = None,
         accepts: None = None,
         validators: list[Callable[[TOrigin], bool]] | None = None,
     ): ...
     @overload
     def __init__(
         self: BasePattern[TOrigin, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
         origin: type[TOrigin],
         accepts: type[TInput1],
         addition_accepts: BasePattern[Any, TInput2, Any],
-        converter: Callable[[BasePattern[TOrigin, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]], TInput1 | TInput2], TOrigin | None]
-        | None = None,
+        converter: (
+            Callable[
+                [BasePattern[TOrigin, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]], TInput1 | TInput2],
+                TOrigin | None,
+            ]
+            | None
+        ) = None,
         alias: str | None = None,
         previous: None = None,
         validators: list[Callable[[TOrigin], bool]] | None = None,
     ): ...
     @overload
     def __init__(
         self: BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
         previous: BasePattern[TInput1, Any, Literal[MatchMode.TYPE_CONVERT]],
-        converter: Callable[[BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]], TInput1 | Any], TOrigin | None],
+        converter: Callable[
+            [BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]], TInput1 | Any], TOrigin | None
+        ],
         alias: str | None = None,
         origin: None = None,
         accepts: None = None,
         addition_accepts: None = None,
         validators: list[Callable[[TOrigin], bool]] | None = None,
     ): ...
     @overload
     def __init__(
         self: BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
         origin: type[TOrigin],
         previous: BasePattern[TInput1, Any, Literal[MatchMode.TYPE_CONVERT]],
-        converter: Callable[[BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]], TInput1 | Any], TOrigin | None] | None = None,
+        converter: (
+            Callable[
+                [BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]], TInput1 | Any], TOrigin | None
+            ]
+            | None
+        ) = None,
         alias: str | None = None,
         accepts: None = None,
         addition_accepts: None = None,
         validators: list[Callable[[TOrigin], bool]] | None = None,
     ): ...
     @overload
     def __init__(
         self: BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
         previous: BasePattern[TInput1, TInput1, Literal[MatchMode.VALUE_OPERATE]],
-        converter: Callable[[BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]], TInput1], TOrigin | None],
+        converter: Callable[
+            [BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]], TInput1], TOrigin | None
+        ],
         alias: str | None = None,
         origin: None = None,
         accepts: None = None,
         addition_accepts: None = None,
         validators: list[Callable[[TOrigin], bool]] | None = None,
     ): ...
     @overload
     def __init__(
         self: BasePattern[TOrigin, TOrigin | TInput1, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
         origin: type[TOrigin],
-        previous:  BasePattern[TOrigin | TInput1, TOrigin | TInput1, Literal[MatchMode.VALUE_OPERATE]] | BasePattern[TOrigin, TOrigin, Literal[MatchMode.VALUE_OPERATE]] | BasePattern[TInput1, TInput1, Literal[MatchMode.VALUE_OPERATE]],
-        converter: Callable[[BasePattern[TOrigin, TOrigin | TInput1, Literal[MatchMode.TYPE_CONVERT]], TInput1], TOrigin | None] | None = None,
+        previous: (
+            BasePattern[TOrigin | TInput1, TOrigin | TInput1, Literal[MatchMode.VALUE_OPERATE]]
+            | BasePattern[TOrigin, TOrigin, Literal[MatchMode.VALUE_OPERATE]]
+            | BasePattern[TInput1, TInput1, Literal[MatchMode.VALUE_OPERATE]]
+        ),
+        converter: (
+            Callable[
+                [BasePattern[TOrigin, TOrigin | TInput1, Literal[MatchMode.TYPE_CONVERT]], TInput1],
+                TOrigin | None,
+            ]
+            | None
+        ) = None,
         alias: str | None = None,
         accepts: None = None,
         addition_accepts: None = None,
         validators: list[Callable[[TOrigin], bool]] | None = None,
     ): ...
     @overload
     def __init__(
         self: BasePattern[TOrigin, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
         accepts: type[TInput1],
         previous: BasePattern[TInput4 | TInput1, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]],
-        converter: Callable[[BasePattern[TOrigin, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]], TInput1 | TInput4], TOrigin | None],
+        converter: Callable[
+            [BasePattern[TOrigin, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]], TInput1 | TInput4],
+            TOrigin | None,
+        ],
         alias: str | None = None,
         origin: None = None,
         addition_accepts: None = None,
         validators: list[Callable[[TOrigin], bool]] | None = None,
     ): ...
     @overload
     def __init__(
         self: BasePattern[TOrigin, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
         origin: type[TOrigin],
         accepts: type[TInput1],
         previous: BasePattern[TInput4 | TInput1, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]],
-        converter: Callable[[BasePattern[TOrigin, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]], TInput1 | TInput4], TOrigin | None] | None = None,
+        converter: (
+            Callable[
+                [BasePattern[TOrigin, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]], TInput1 | TInput4],
+                TOrigin | None,
+            ]
+            | None
+        ) = None,
         alias: str | None = None,
         addition_accepts: None = None,
         validators: list[Callable[[TOrigin], bool]] | None = None,
     ): ...
     @overload
     def __init__(
         self: BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
         accepts: type[TInput1],
         previous: BasePattern[TInput1, TInput1, Literal[MatchMode.VALUE_OPERATE]],
-        converter: Callable[[BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]], TInput1], TOrigin | None],
+        converter: Callable[
+            [BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]], TInput1], TOrigin | None
+        ],
         alias: str | None = None,
-        origin:  None = None,
+        origin: None = None,
         addition_accepts: None = None,
         validators: list[Callable[[TOrigin], bool]] | None = None,
     ): ...
     @overload
     def __init__(
         self: BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
         origin: type[TOrigin],
         accepts: type[TInput1],
         previous: BasePattern[TInput1, TInput1, Literal[MatchMode.VALUE_OPERATE]],
-        converter: Callable[[BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]], TInput1], TOrigin | None] | None = None,
+        converter: (
+            Callable[
+                [BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]], TInput1], TOrigin | None
+            ]
+            | None
+        ) = None,
         alias: str | None = None,
         addition_accepts: None = None,
         validators: list[Callable[[TOrigin], bool]] | None = None,
     ): ...
     @overload
     def __init__(
         self: BasePattern[TOrigin, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
         addition_accepts: BasePattern[Any, TInput1, Any],
         previous: BasePattern[TInput4 | TInput1, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]],
-        converter: Callable[[BasePattern[TOrigin, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]], TInput1 | TInput4], TOrigin | None],
+        converter: Callable[
+            [BasePattern[TOrigin, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]], TInput1 | TInput4],
+            TOrigin | None,
+        ],
         alias: str | None = None,
         origin: None = None,
         accepts: None = None,
         validators: list[Callable[[TOrigin], bool]] | None = None,
     ): ...
     @overload
     def __init__(
         self: BasePattern[TOrigin, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
         origin: type[TOrigin],
         addition_accepts: BasePattern[Any, TInput1, Any],
         previous: BasePattern[TInput4 | TInput1, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]],
-        converter: Callable[[BasePattern[TOrigin, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]], TInput1 | TInput4], TOrigin | None] | None = None,
+        converter: (
+            Callable[
+                [BasePattern[TOrigin, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]], TInput1 | TInput4],
+                TOrigin | None,
+            ]
+            | None
+        ) = None,
         alias: str | None = None,
         accepts: None = None,
         validators: list[Callable[[TOrigin], bool]] | None = None,
     ): ...
     @overload
     def __init__(
         self: BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
         addition_accepts: BasePattern[Any, TInput1, Any],
         previous: BasePattern[TInput1, TInput1, Literal[MatchMode.VALUE_OPERATE]],
-        converter: Callable[[BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]], TInput1], TOrigin | None],
+        converter: Callable[
+            [BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]], TInput1], TOrigin | None
+        ],
         alias: str | None = None,
         origin: None = None,
         accepts: None = None,
         validators: list[Callable[[TOrigin], bool]] | None = None,
     ): ...
     @overload
     def __init__(
         self: BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
         origin: type[TOrigin],
         addition_accepts: BasePattern[Any, TInput1, Any],
         previous: BasePattern[TInput1, TInput1, Literal[MatchMode.VALUE_OPERATE]],
-        converter: Callable[[BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]], TInput1], TOrigin | None] | None = None,
+        converter: (
+            Callable[
+                [BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]], TInput1], TOrigin | None
+            ]
+            | None
+        ) = None,
         alias: str | None = None,
         accepts: None = None,
         validators: list[Callable[[TOrigin], bool]] | None = None,
     ): ...
     @overload
     def __init__(
         self: BasePattern[TOrigin, TInput1 | TInput2 | TInput3, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
         accepts: type[TInput1],
-        previous: BasePattern[TInput1 | TInput3, TInput2, Literal[MatchMode.TYPE_CONVERT]] | BasePattern[TInput1, TInput2, Literal[MatchMode.TYPE_CONVERT]] | BasePattern[TInput3, TInput2, Literal[MatchMode.TYPE_CONVERT]],
+        previous: (
+            BasePattern[TInput1 | TInput3, TInput2, Literal[MatchMode.TYPE_CONVERT]]
+            | BasePattern[TInput1, TInput2, Literal[MatchMode.TYPE_CONVERT]]
+            | BasePattern[TInput3, TInput2, Literal[MatchMode.TYPE_CONVERT]]
+        ),
         addition_accepts: BasePattern[Any, TInput3, Any],
-        converter: Callable[[BasePattern[TOrigin, TInput1 | TInput2 | TInput3, Literal[MatchMode.TYPE_CONVERT]], TInput1 | TInput3], TOrigin | None],
+        converter: Callable[
+            [
+                BasePattern[TOrigin, TInput1 | TInput2 | TInput3, Literal[MatchMode.TYPE_CONVERT]],
+                TInput1 | TInput3,
+            ],
+            TOrigin | None,
+        ],
         alias: str | None = None,
         origin: None = None,
         validators: list[Callable[[TOrigin], bool]] | None = None,
     ): ...
     @overload
     def __init__(
         self: BasePattern[TOrigin, TInput1 | TInput2 | TInput3, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
         origin: type[TOrigin],
         accepts: type[TInput1],
-        previous: BasePattern[TInput1 | TInput3, TInput2, Literal[MatchMode.TYPE_CONVERT]] | BasePattern[TInput1, TInput2, Literal[MatchMode.TYPE_CONVERT]] | BasePattern[TInput3, TInput2, Literal[MatchMode.TYPE_CONVERT]],
+        previous: (
+            BasePattern[TInput1 | TInput3, TInput2, Literal[MatchMode.TYPE_CONVERT]]
+            | BasePattern[TInput1, TInput2, Literal[MatchMode.TYPE_CONVERT]]
+            | BasePattern[TInput3, TInput2, Literal[MatchMode.TYPE_CONVERT]]
+        ),
         addition_accepts: BasePattern[Any, TInput3, Any],
-        converter: Callable[[BasePattern[TOrigin, TInput1 | TInput2 | TInput3, Literal[MatchMode.TYPE_CONVERT]], TInput1 | TInput3], TOrigin | None]
-        | None = None,
+        converter: (
+            Callable[
+                [
+                    BasePattern[TOrigin, TInput1 | TInput2 | TInput3, Literal[MatchMode.TYPE_CONVERT]],
+                    TInput1 | TInput3,
+                ],
+                TOrigin | None,
+            ]
+            | None
+        ) = None,
         alias: str | None = None,
         validators: list[Callable[[TOrigin], bool]] | None = None,
     ): ...
     @overload
     def __init__(
         self: BasePattern[TOrigin, TInput1 | TInput3, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
         accepts: type[TInput1],
-        previous: BasePattern[TInput1 | TInput3, TInput1 | TInput3, Literal[MatchMode.VALUE_OPERATE]] | BasePattern[TInput3, TInput3, Literal[MatchMode.VALUE_OPERATE]] | BasePattern[TInput1, TInput1, Literal[MatchMode.VALUE_OPERATE]],
+        previous: (
+            BasePattern[TInput1 | TInput3, TInput1 | TInput3, Literal[MatchMode.VALUE_OPERATE]]
+            | BasePattern[TInput3, TInput3, Literal[MatchMode.VALUE_OPERATE]]
+            | BasePattern[TInput1, TInput1, Literal[MatchMode.VALUE_OPERATE]]
+        ),
         addition_accepts: BasePattern[Any, TInput3, Any],
-        converter: Callable[[BasePattern[TOrigin, TInput1 | TInput3, Literal[MatchMode.TYPE_CONVERT]], TInput1 | TInput3], TOrigin | None],
+        converter: Callable[
+            [BasePattern[TOrigin, TInput1 | TInput3, Literal[MatchMode.TYPE_CONVERT]], TInput1 | TInput3],
+            TOrigin | None,
+        ],
         origin: None = None,
         alias: str | None = None,
         validators: list[Callable[[TOrigin], bool]] | None = None,
     ): ...
     @overload
     def __init__(
         self: BasePattern[TOrigin, TInput1 | TInput3, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
         origin: type[TOrigin],
         accepts: type[TInput1],
-        previous: BasePattern[TInput1 | TInput3, TInput1 | TInput3, Literal[MatchMode.VALUE_OPERATE]] | BasePattern[TInput3, TInput3, Literal[MatchMode.VALUE_OPERATE]] | BasePattern[TInput1, TInput1, Literal[MatchMode.VALUE_OPERATE]],
+        previous: (
+            BasePattern[TInput1 | TInput3, TInput1 | TInput3, Literal[MatchMode.VALUE_OPERATE]]
+            | BasePattern[TInput3, TInput3, Literal[MatchMode.VALUE_OPERATE]]
+            | BasePattern[TInput1, TInput1, Literal[MatchMode.VALUE_OPERATE]]
+        ),
         addition_accepts: BasePattern[Any, TInput3, Any],
-        converter: Callable[[BasePattern[TOrigin, TInput1 | TInput3, Literal[MatchMode.TYPE_CONVERT]], TInput1 | TInput3], TOrigin | None]
-        | None = None,
+        converter: (
+            Callable[
+                [BasePattern[TOrigin, TInput1 | TInput3, Literal[MatchMode.TYPE_CONVERT]], TInput1 | TInput3],
+                TOrigin | None,
+            ]
+            | None
+        ) = None,
         alias: str | None = None,
         validators: list[Callable[[TOrigin], bool]] | None = None,
     ): ...
     @overload
     def __init__(
         self: BasePattern[TOrigin, TOrigin, Literal[MatchMode.VALUE_OPERATE]],
         *,
         mode: Literal[MatchMode.VALUE_OPERATE],
         origin: type[TOrigin],
-        converter: Callable[[BasePattern[TOrigin, TOrigin, Literal[MatchMode.VALUE_OPERATE]], TOrigin], TOrigin | None],
+        converter: Callable[
+            [BasePattern[TOrigin, TOrigin, Literal[MatchMode.VALUE_OPERATE]], TOrigin], TOrigin | None
+        ],
         alias: str | None = None,
         previous: None = None,
         accepts: None = None,
         addition_accepts: None = None,
         validators: list[Callable[[TOrigin], bool]] | None = None,
     ): ...
     @overload
     def __init__(
         self: BasePattern[TOrigin, TOrigin | TInput1, Literal[MatchMode.VALUE_OPERATE]],
         *,
         mode: Literal[MatchMode.VALUE_OPERATE],
         origin: type[TOrigin],
         previous: BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]],
-        converter: Callable[[BasePattern[TOrigin, TOrigin | TInput1, Literal[MatchMode.VALUE_OPERATE]], TOrigin], TOrigin | None],
+        converter: Callable[
+            [BasePattern[TOrigin, TOrigin | TInput1, Literal[MatchMode.VALUE_OPERATE]], TOrigin],
+            TOrigin | None,
+        ],
+        alias: str | None = None,
+        accepts: None = None,
+        addition_accepts: None = None,
+        validators: list[Callable[[TOrigin], bool]] | None = None,
+    ): ...
+    @overload
+    def __init__(
+        self: BasePattern[TOrigin, TOrigin | TInput2, Literal[MatchMode.VALUE_OPERATE]],
+        *,
+        mode: Literal[MatchMode.VALUE_OPERATE],
+        origin: type[TOrigin],
+        previous: BasePattern[TOrigin, TOrigin | TInput2, Literal[MatchMode.TYPE_CONVERT]],
+        converter: Callable[
+            [BasePattern[TOrigin, TOrigin | TInput2, Literal[MatchMode.VALUE_OPERATE]], TOrigin],
+            TOrigin | None,
+        ],
         alias: str | None = None,
         accepts: None = None,
         addition_accepts: None = None,
         validators: list[Callable[[TOrigin], bool]] | None = None,
     ): ...
     @overload
     def __init__(
         self: BasePattern[TOrigin, TOrigin, Literal[MatchMode.VALUE_OPERATE]],
         *,
         mode: Literal[MatchMode.VALUE_OPERATE],
         origin: type[TOrigin],
         previous: BasePattern[TOrigin, TOrigin, Literal[MatchMode.VALUE_OPERATE]],
-        converter: Callable[[BasePattern[TOrigin, TOrigin, Literal[MatchMode.VALUE_OPERATE]], TOrigin], TOrigin | None],
+        converter: Callable[
+            [BasePattern[TOrigin, TOrigin, Literal[MatchMode.VALUE_OPERATE]], TOrigin], TOrigin | None
+        ],
         alias: str | None = None,
         accepts: None = None,
         addition_accepts: None = None,
         validators: list[Callable[[TOrigin], bool]] | None = None,
     ): ...
     def refresh(self): ...
     def __calc_hash__(self): ...
     def __calc_repr__(self): ...
     def __calc_eq__(self, other): ...
     def __repr__(self): ...
     def __str__(self): ...
     def __hash__(self): ...
     def __eq__(self, other): ...
     @staticmethod
-    def of(unit: type[TOrigin]) -> DirectTypePattern[TOrigin]:
+    def of(unit: type[TOrigin1]) -> DirectTypePattern[TOrigin1]:
         """提供 Type[DataUnit] 类型的构造方法"""
         ...
+
     @staticmethod
-    def on(obj: TOrigin) -> DirectPattern[TOrigin]:
+    def on(obj: TOrigin1) -> DirectPattern[TOrigin1]:
         """提供 DataUnit 类型的构造方法"""
         ...
+
     @staticmethod
     def to(content: Any) -> BasePattern:
         """便捷的使用 type_parser 的方法"""
         ...
+
     @overload
-    def validate(self: BasePattern[TOrigin, TInput, Literal[MatchMode.KEEP]], input_: TInput) -> ValidateResult[TOrigin, Literal[ResultFlag.VALID]]: ...
+    def validate(
+        self: BasePattern[TOrigin, TInput, Literal[MatchMode.KEEP]], input_: TInput
+    ) -> ValidateResult[TOrigin, Literal[ResultFlag.VALID]]: ...
     @overload
-    def validate(self: BasePattern[TOrigin, TInput, Literal[MatchMode.KEEP]], input_: T) -> ValidateResult[T, Literal[ResultFlag.ERROR]]: ...
+    def validate(
+        self: BasePattern[TOrigin, TInput, Literal[MatchMode.KEEP]], input_: T
+    ) -> ValidateResult[T, Literal[ResultFlag.ERROR]]: ...
     @overload
-    def validate(self: BasePattern[TOrigin, TInput, Literal[MatchMode.VALUE_OPERATE]], input_: TInput) -> ValidateResult[TOrigin, Literal[ResultFlag.VALID]]: ...
+    def validate(
+        self: BasePattern[TOrigin, TInput, Literal[MatchMode.VALUE_OPERATE]], input_: TInput
+    ) -> ValidateResult[TOrigin, Literal[ResultFlag.VALID]]: ...
     @overload
-    def validate(self: BasePattern[TOrigin, TInput, Literal[MatchMode.VALUE_OPERATE]], input_: T) -> ValidateResult[T, Literal[ResultFlag.ERROR]]: ...
+    def validate(
+        self: BasePattern[TOrigin, TInput, Literal[MatchMode.VALUE_OPERATE]], input_: T
+    ) -> ValidateResult[T, Literal[ResultFlag.ERROR]]: ...
     @overload
-    def validate(self: BasePattern[TOrigin, TInput, TMM], input_: TInput) -> ValidateResult[TOrigin, Literal[ResultFlag.VALID]] | ValidateResult[TOrigin, Literal[ResultFlag.ERROR]]: ...
+    def validate(
+        self: BasePattern[TOrigin, TInput, TMM], input_: TInput
+    ) -> (
+        ValidateResult[TOrigin, Literal[ResultFlag.VALID]]
+        | ValidateResult[TOrigin, Literal[ResultFlag.ERROR]]
+    ): ...
     @overload
-    def validate(self: BasePattern[TOrigin, TInput, TMM], input_: T) -> ValidateResult[T, Literal[ResultFlag.ERROR]]: ...
+    def validate(
+        self: BasePattern[TOrigin, TInput, TMM], input_: T
+    ) -> ValidateResult[T, Literal[ResultFlag.ERROR]]: ...
     @overload
     def validate(
         self: BasePattern[TOrigin, TInput, Literal[MatchMode.KEEP]], input_: TInput, default: Any
     ) -> ValidateResult[TOrigin, Literal[ResultFlag.VALID]]: ...
     @overload
     def validate(
         self: BasePattern[TOrigin, TInput, Literal[MatchMode.KEEP]], input_: Any, default: TDefault
@@ -687,20 +873,25 @@
     @overload
     def validate(
         self: BasePattern[TOrigin, TInput, Literal[MatchMode.VALUE_OPERATE]], input_: Any, default: TDefault
     ) -> ValidateResult[TDefault, Literal[ResultFlag.DEFAULT]]: ...
     @overload
     def validate(
         self: BasePattern[TOrigin, TInput, TMM], input_: TInput, default: Any
-    ) -> ValidateResult[TOrigin, Literal[ResultFlag.VALID]] | ValidateResult[TOrigin, Literal[ResultFlag.ERROR]]: ...
+    ) -> (
+        ValidateResult[TOrigin, Literal[ResultFlag.VALID]]
+        | ValidateResult[TOrigin, Literal[ResultFlag.ERROR]]
+    ): ...
     @overload
     def validate(
         self: BasePattern[TOrigin, TInput, TMM], input_: Any, default: TDefault
     ) -> ValidateResult[TDefault, Literal[ResultFlag.DEFAULT]]: ...
     def match(self, input_: TInput) -> TOrigin: ...
     def copy(self) -> BasePattern[TOrigin, TInput, TMM]: ...
     def __rrshift__(
         self, other: T
     ) -> ValidateResult[T, Literal[ResultFlag.VALID]] | ValidateResult[T, Literal[ResultFlag.ERROR]]: ...
     def __rmatmul__(self, other) -> Self: ...
     def __matmul__(self, other) -> Self: ...
-    def __or__(self, other: BasePattern[TOrigin1, TInput1, Any]) -> BasePattern[TOrigin1 | TOrigin, TInput1 | TInput, TMM]: ...
+    def __or__(
+        self, other: BasePattern[TOrigin1, TInput1, Any]
+    ) -> BasePattern[TOrigin1 | TOrigin, TInput1 | TInput, TMM]: ...
```

### Comparing `nepattern-0.7.1/nepattern/main.py` & `nepattern-0.7.2/nepattern/main.py`

 * *Files identical despite different names*

### Comparing `nepattern-0.7.1/nepattern/main.pyi` & `nepattern-0.7.2/nepattern/main.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,53 +1,65 @@
 from collections.abc import Mapping as ABCMap
 from collections.abc import MutableSequence as ABCMuSeq
 from collections.abc import Set as ABCSet
 from types import UnionType
-from typing import Any, Callable, ForwardRef, Iterable, TypeVar, overload, Literal
+from typing import Any, Callable, ForwardRef, Iterable, Literal, TypeVar, overload
 
 from .base import (
     DirectPattern,
     DirectTypePattern,
     ForwardRefPattern,
+    IterMode,
     MappingPattern,
     RegexPattern,
     SequencePattern,
     SwitchPattern,
     UnionPattern,
-    IterMode
 )
 from .core import BasePattern, MatchMode
 from .util import RawStr, TPattern
 
 T1 = TypeVar("T1")
 T2 = TypeVar("T2")
 
 @overload
 def parser(
     item: str, extra: str = "allow"
-) -> BasePattern[str, str, Literal[MatchMode.REGEX_MATCH]] | DirectPattern[str] | RegexPattern | UnionPattern: ...
+) -> (
+    BasePattern[str, str, Literal[MatchMode.REGEX_MATCH]] | DirectPattern[str] | RegexPattern | UnionPattern
+): ...
 @overload
 def parser(item: RawStr, extra: str = "allow") -> DirectPattern[str]: ...
 @overload
 def parser(item: TPattern, extra: str = "allow") -> RegexPattern: ...
 @overload
-def parser(item: type[ABCMap[T1, T2]], extra: str = "allow") -> MappingPattern[T1, T2, Literal[IterMode.ALL]]: ...
+def parser(
+    item: type[ABCMap[T1, T2]], extra: str = "allow"
+) -> MappingPattern[T1, T2, Literal[IterMode.ALL]]: ...
 @overload
-def parser(item: type[ABCMuSeq[T1]], extra: str = "allow") -> SequencePattern[list[T1], Literal[IterMode.ALL]]: ...
+def parser(
+    item: type[ABCMuSeq[T1]], extra: str = "allow"
+) -> SequencePattern[list[T1], Literal[IterMode.ALL]]: ...
 @overload
-def parser(item: type[tuple[T1, ...]], extra: str = "allow") -> SequencePattern[tuple[T1, ...], Literal[IterMode.ALL]]: ...
+def parser(
+    item: type[tuple[T1, ...]], extra: str = "allow"
+) -> SequencePattern[tuple[T1, ...], Literal[IterMode.ALL]]: ...
 @overload
-def parser(item: type[ABCSet[T1]], extra: str = "allow") -> SequencePattern[set[T1], Literal[IterMode.ALL]]: ...
+def parser(
+    item: type[ABCSet[T1]], extra: str = "allow"
+) -> SequencePattern[set[T1], Literal[IterMode.ALL]]: ...
 @overload
 def parser(item: type[T1], extra: str = "allow") -> BasePattern[T1, Any, Any] | DirectTypePattern[T1]: ...
 @overload
 def parser(item: ABCMap[T1, T2], extra: str = "allow") -> SwitchPattern[T2, T1]: ...
 @overload
 def parser(item: UnionType, extra: str = "allow") -> UnionPattern[Any]: ...
 @overload
 def parser(item: Iterable[T1 | type[T1]], extra: str = "allow") -> UnionPattern[T1]: ...
 @overload
 def parser(item: ForwardRef, extra: str = "allow") -> ForwardRefPattern: ...
 @overload
-def parser(item: Callable[[T1], T2], extra: str = "allow") -> BasePattern[T2, T1, Literal[MatchMode.TYPE_CONVERT]]: ...
+def parser(
+    item: Callable[[T1], T2], extra: str = "allow"
+) -> BasePattern[T2, T1, Literal[MatchMode.TYPE_CONVERT]]: ...
 @overload
 def parser(item: T1, extra: str = "allow") -> BasePattern[T1, T1, Literal[MatchMode.KEEP]]: ...
```

### Comparing `nepattern-0.7.1/nepattern/util.py` & `nepattern-0.7.2/nepattern/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 from tarina.lang import lang
 
 if sys.version_info >= (3, 9):  # pragma: no cover
     from types import GenericAlias as CGenericAlias  # noqa
 else:  # pragma: no cover
     CGenericAlias: type = type(List[int])  # noqa
 
-if sys.version_info >= (3, 10):   # pragma: no cover
+if sys.version_info >= (3, 10):  # pragma: no cover
     from types import UnionType as CUnionType  # noqa
 else:  # pragma: no cover
     CUnionType: type = type(Union[int, str])  # noqa
 
-if sys.version_info >= (3, 11):   # pragma: no cover
+if sys.version_info >= (3, 11):  # pragma: no cover
     from re._compiler import compile as re_compile  # noqa
 else:  # pragma: no cover
     from sre_compile import compile as re_compile  # noqa
 
 if TYPE_CHECKING:
     TPattern = Pattern[str]
 else:
```

### Comparing `nepattern-0.7.1/pyproject.toml` & `nepattern-0.7.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nepattern"
-version = "0.7.1"
+version = "0.7.2"
 description = "a complex pattern, support typing"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "typing-extensions>=4.5.0",
     "tarina>=0.4.1",
@@ -30,16 +30,14 @@
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 repository = "https://github.com/ArcletProject/NEPattern"
 
-[project.optional-dependencies]
-
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [tool.pdm.build]
@@ -48,14 +46,16 @@
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
     "pytest~=7.1.3",
     "coverage~=6.5.0",
     "fix-future-annotations>=0.5.0",
+    "isort>=5.13.2",
+    "black>=24.4.1",
 ]
 
 [tool.pdm.scripts.test]
 composite = [
     "coverage run -m pytest -vv",
     "coverage xml",
     "coverage report",
```

### Comparing `nepattern-0.7.1/PKG-INFO` & `nepattern-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nepattern
-Version: 0.7.1
+Version: 0.7.2
 Summary: a complex pattern, support typing
 Keywords: typing,pattern,converter,validator
 Author-Email: RF-Tar-Railt <rf_tar_railt@qq.com>
 License: MIT
 Classifier: Typing :: Typed
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

