# Comparing `tmp/smp-0.3.3.tar.gz` & `tmp/smp-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smp-0.3.3.tar", max compression
+gzip compressed data, was "smp-0.3.4.tar", max compression
```

## Comparing `smp-0.3.3.tar` & `smp-0.3.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11365 2024-03-18 22:52:13.210248 smp-0.3.3/LICENSE
--rw-r--r--   0        0        0     2243 2024-03-18 22:52:13.210248 smp-0.3.3/README.md
--rw-r--r--   0        0        0      953 2024-03-18 22:52:13.210248 smp-0.3.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-18 22:52:13.210248 smp-0.3.3/smp/__init__.py
--rw-r--r--   0        0        0      659 2024-03-18 22:52:13.210248 smp-0.3.3/smp/error.py
--rw-r--r--   0        0        0      471 2024-03-18 22:52:13.210248 smp-0.3.3/smp/exceptions.py
--rw-r--r--   0        0        0     4229 2024-03-18 22:52:13.210248 smp-0.3.3/smp/header.py
--rw-r--r--   0        0        0     6129 2024-03-18 22:52:13.210248 smp-0.3.3/smp/image_management.py
--rw-r--r--   0        0        0     5068 2024-03-18 22:52:13.210248 smp-0.3.3/smp/message.py
--rw-r--r--   0        0        0     6741 2024-03-18 22:52:13.210248 smp-0.3.3/smp/os_management.py
--rw-r--r--   0        0        0     3135 2024-03-18 22:52:13.210248 smp-0.3.3/smp/packet.py
--rw-r--r--   0        0        0        0 2024-03-18 22:52:13.210248 smp-0.3.3/smp/py.typed
--rw-r--r--   0        0        0     1051 2024-03-18 22:52:13.210248 smp-0.3.3/smp/shell_management.py
--rw-r--r--   0        0        0        0 2024-03-18 22:52:13.210248 smp-0.3.3/smp/user/__init__.py
--rw-r--r--   0        0        0     1321 2024-03-18 22:52:13.210248 smp-0.3.3/smp/user/intercreate.py
--rw-r--r--   0        0        0     2894 1970-01-01 00:00:00.000000 smp-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0    11365 2024-04-24 23:26:42.128815 smp-0.3.4/LICENSE
+-rw-r--r--   0        0        0     2243 2024-04-24 23:26:42.128815 smp-0.3.4/README.md
+-rw-r--r--   0        0        0      953 2024-04-24 23:26:42.128815 smp-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-24 23:26:42.128815 smp-0.3.4/smp/__init__.py
+-rw-r--r--   0        0        0      659 2024-04-24 23:26:42.128815 smp-0.3.4/smp/error.py
+-rw-r--r--   0        0        0      471 2024-04-24 23:26:42.128815 smp-0.3.4/smp/exceptions.py
+-rw-r--r--   0        0        0     4905 2024-04-24 23:26:42.128815 smp-0.3.4/smp/header.py
+-rw-r--r--   0        0        0     6149 2024-04-24 23:26:42.128815 smp-0.3.4/smp/image_management.py
+-rw-r--r--   0        0        0     4822 2024-04-24 23:26:42.128815 smp-0.3.4/smp/message.py
+-rw-r--r--   0        0        0     6761 2024-04-24 23:26:42.128815 smp-0.3.4/smp/os_management.py
+-rw-r--r--   0        0        0     3135 2024-04-24 23:26:42.128815 smp-0.3.4/smp/packet.py
+-rw-r--r--   0        0        0        0 2024-04-24 23:26:42.128815 smp-0.3.4/smp/py.typed
+-rw-r--r--   0        0        0     1071 2024-04-24 23:26:42.128815 smp-0.3.4/smp/shell_management.py
+-rw-r--r--   0        0        0        0 2024-04-24 23:26:42.128815 smp-0.3.4/smp/user/__init__.py
+-rw-r--r--   0        0        0     1359 2024-04-24 23:26:42.128815 smp-0.3.4/smp/user/intercreate.py
+-rw-r--r--   0        0        0     2894 1970-01-01 00:00:00.000000 smp-0.3.4/PKG-INFO
```

### Comparing `smp-0.3.3/LICENSE` & `smp-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `smp-0.3.3/README.md` & `smp-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `smp-0.3.3/pyproject.toml` & `smp-0.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `smp-0.3.3/smp/error.py` & `smp-0.3.4/smp/error.py`

 * *Files identical despite different names*

### Comparing `smp-0.3.3/smp/header.py` & `smp-0.3.4/smp/header.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """The Simple Management Protocol (SMP) header."""
 
 import struct
 from dataclasses import dataclass
 from enum import IntEnum, IntFlag, auto, unique
-from typing import TypeVar
+from typing import ClassVar, Dict, Type, TypeAlias
 
 
 class CommandId:
     @unique
     class OSManagement(IntEnum):
         ECHO = 0
         ECHO_CONTROL = 1
@@ -33,15 +33,15 @@
         EXECUTE = 0
 
     @unique
     class Intercreate(IntEnum):
         UPLOAD = 1
 
 
-AnyCommandId = TypeVar("AnyCommandId", bound=IntEnum)
+AnyCommandId: TypeAlias = IntEnum | int
 
 
 class GroupId(IntEnum):
     OS_MANAGEMENT = 0
     IMAGE_MANAGEMENT = 1
     STATISTICS_MANAGEMENT = 2
     SETTINGS_MANAGEMENT = 3
@@ -52,14 +52,17 @@
     FILE_MANAGEMENT = 8
     SHELL_MANAGEMENT = 9
     ZEPHYR = 63
     _APPLICATIION_CUSTOM_MIN = 64
     INTERCREATE = 64
 
 
+AnyGroupId: TypeAlias = IntEnum | int
+
+
 @unique
 class OP(IntEnum):
     READ = 0
     READ_RSP = 1
     WRITE = 2
     WRITE_RSP = 3
 
@@ -87,28 +90,32 @@
 
 @dataclass(frozen=True)
 class Header:
     op: OP
     version: Version
     flags: Flag
     length: int
-    group_id: GroupId
+    group_id: AnyGroupId | GroupId
     sequence: int
     command_id: (
-        CommandId.OSManagement | CommandId.ImageManagement | CommandId.ShellManagement | IntEnum
+        AnyCommandId
+        | CommandId.OSManagement
+        | CommandId.ImageManagement
+        | CommandId.ShellManagement
+        | CommandId.Intercreate
     )
 
-    _MAP_GROUP_ID_TO_COMMAND_ID_ENUM = {
+    _MAP_GROUP_ID_TO_COMMAND_ID_ENUM: ClassVar[Dict[int, Type[IntEnum]]] = {
         GroupId.OS_MANAGEMENT: CommandId.OSManagement,
         GroupId.IMAGE_MANAGEMENT: CommandId.ImageManagement,
         GroupId.SHELL_MANAGEMENT: CommandId.ShellManagement,
         GroupId.INTERCREATE: CommandId.Intercreate,
     }
-    _STRUCT = struct.Struct("!BBHHBB")
-    SIZE = _STRUCT.size
+    _STRUCT: ClassVar = struct.Struct("!BBHHBB")
+    SIZE: ClassVar = _STRUCT.size
 
     @staticmethod
     def _pack_op(op: OP) -> int:
         """The value to be packed into the byte."""
         return op << _OP_BIT.SHIFT
 
     @staticmethod
@@ -127,25 +134,40 @@
         return Version((res_ver_op_byte >> _VERSION_BIT.SHIFT) & _VERSION_BIT.MASK)
 
     @staticmethod
     def _pack_op_and_version(op: OP, version: Version) -> int:
         """The op and version packed into one byte."""
         return Header._pack_op(op) | Header._pack_version(version)
 
+    @staticmethod
+    def _validate_command_id(group_id: int, command_id: int) -> None:
+        """Validate the command_id if the GroupId is known."""
+
+        if command_id_t := Header._MAP_GROUP_ID_TO_COMMAND_ID_ENUM.get(group_id):
+            try:
+                command_id_t(command_id)
+            except ValueError:
+                raise ValueError(
+                    f"Command ID {command_id} is not valid for Group ID {group_id}"
+                    f" ({GroupId(group_id).name})"
+                )
+
     def __post_init__(self) -> None:
+        Header._validate_command_id(self.group_id, self.command_id)
+
         object.__setattr__(
             self,
             '_bytes',
             self._STRUCT.pack(
                 self._pack_op_and_version(self.op, self.version),
                 Flag(self.flags),
                 self.length,
-                GroupId(self.group_id),
+                self.group_id,
                 self.sequence,
-                Header._MAP_GROUP_ID_TO_COMMAND_ID_ENUM[GroupId(self.group_id)](self.command_id),
+                self.command_id,
             ),
         )
 
     def __bytes__(self) -> bytes:
         return self._bytes  # type: ignore
 
     @property
@@ -157,16 +179,18 @@
         """Deserialize the header bytes to a `Header`."""
         assert len(header) == 8, "The header is specified as 8 bytes"
 
         res_ver_op_byte, flags, length, group_id, sequence, command_id = Header._STRUCT.unpack(
             header
         )
 
+        Header._validate_command_id(group_id, command_id)
+
         return Header(
             Header._unpack_op(res_ver_op_byte),
             Header._unpack_version(res_ver_op_byte),
             Flag(flags),
             length,
-            GroupId(group_id),
+            group_id,
             sequence,
-            Header._MAP_GROUP_ID_TO_COMMAND_ID_ENUM[GroupId(group_id)](command_id),
+            command_id,
         )
```

### Comparing `smp-0.3.3/smp/image_management.py` & `smp-0.3.4/smp/image_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """The Simple Management Protocol (SMP) Image Management group."""
 
 from enum import IntEnum, auto, unique
-from typing import Generator, List
+from typing import ClassVar, Generator, List
 
 from pydantic import BaseModel, ConfigDict, ValidationInfo, field_validator
 
 from smp import error, header, message
 
 
 class _ImageManagementGroup:
-    _GROUP_ID = header.GroupId.IMAGE_MANAGEMENT
+    _GROUP_ID: ClassVar = header.GroupId.IMAGE_MANAGEMENT
 
 
 class HashBytes(bytes):  # pragma: no cover
     """Only to print something useful to the console."""
 
     def __rich_repr__(self) -> Generator[str, None, None]:
         yield self.hex().upper()
```

### Comparing `smp-0.3.3/smp/message.py` & `smp-0.3.4/smp/message.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,17 +19,18 @@
 
 class _MessageBase(ABC, BaseModel):
     model_config = ConfigDict(extra="forbid", frozen=True)
 
     _OP: ClassVar[smpheader.OP]
     _VERSION: ClassVar[smpheader.Version] = smpheader.Version.V0
     _FLAGS: ClassVar[smpheader.Flag] = smpheader.Flag(0)
-    _GROUP_ID: ClassVar[smpheader.GroupId]
+    _GROUP_ID: ClassVar[smpheader.GroupId | smpheader.AnyGroupId]
     _COMMAND_ID: ClassVar[
-        smpheader.CommandId.ImageManagement
+        smpheader.AnyCommandId
+        | smpheader.CommandId.ImageManagement
         | smpheader.CommandId.OSManagement
         | smpheader.CommandId.ShellManagement
         | smpheader.CommandId.Intercreate
     ]
 
     header: smpheader.Header | None = None
 
@@ -75,19 +76,17 @@
                 self,
                 'header',
                 smpheader.Header(
                     op=self._OP,
                     version=self._VERSION,
                     flags=smpheader.Flag(self._FLAGS),
                     length=len(data_bytes),
-                    group_id=smpheader.GroupId(self._GROUP_ID),
+                    group_id=self._GROUP_ID,
                     sequence=next(_counter) % 0xFF,
-                    command_id=smpheader.Header._MAP_GROUP_ID_TO_COMMAND_ID_ENUM[
-                        smpheader.GroupId(self._GROUP_ID)
-                    ](self._COMMAND_ID),
+                    command_id=self._COMMAND_ID,
                 ),
             )
         elif self.header.length != len(data_bytes):
             raise SMPMalformed(
                 f"header.length {self.header.length} != len(data_bytes) {len(data_bytes)}"
             )
         self._bytes = cast(smpheader.Header, self.header).BYTES + data_bytes
@@ -116,19 +115,17 @@
                 self,
                 'header',
                 smpheader.Header(
                     op=self._OP,
                     version=self._VERSION,
                     flags=smpheader.Flag(self._FLAGS),
                     length=len(data_bytes),
-                    group_id=smpheader.GroupId(self._GROUP_ID),
+                    group_id=self._GROUP_ID,
                     sequence=self.sequence,
-                    command_id=smpheader.Header._MAP_GROUP_ID_TO_COMMAND_ID_ENUM[
-                        smpheader.GroupId(self._GROUP_ID)
-                    ](self._COMMAND_ID),
+                    command_id=self._COMMAND_ID,
                 ),
             )
         self._bytes = cast(smpheader.Header, self.header).BYTES + data_bytes
 
 
 class ReadRequest(Request, ABC):
     """A read request from an SMP client to an SMP server."""
```

### Comparing `smp-0.3.3/smp/os_management.py` & `smp-0.3.4/smp/os_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """The Simple Management Protocol (SMP) OS Management group."""
 
 
 from enum import IntEnum, auto, unique
-from typing import Any, Dict
+from typing import Any, ClassVar, Dict
 
 from pydantic import BaseModel, ConfigDict, Field
 
 from smp import error, header, message
 
 
 class _OSManagementGroup:
-    _GROUP_ID = header.GroupId.OS_MANAGEMENT
+    _GROUP_ID: ClassVar = header.GroupId.OS_MANAGEMENT
 
 
 class EchoWriteRequest(_OSManagementGroup, message.WriteRequest):
     _COMMAND_ID = header.CommandId.OSManagement.ECHO
 
     d: str
```

### Comparing `smp-0.3.3/smp/packet.py` & `smp-0.3.4/smp/packet.py`

 * *Files identical despite different names*

### Comparing `smp-0.3.3/smp/shell_management.py` & `smp-0.3.4/smp/shell_management.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """The Simple Management Protocol (SMP) Shell Management group."""
 
 
 from enum import IntEnum, auto, unique
-from typing import List
+from typing import ClassVar, List
 
 from smp import error, header, message
 
 
 class _ShellManagementGroup:
-    _GROUP_ID = header.GroupId.SHELL_MANAGEMENT
+    _GROUP_ID: ClassVar = header.GroupId.SHELL_MANAGEMENT
 
 
 class ExecuteRequest(_ShellManagementGroup, message.WriteRequest):
     _COMMAND_ID = header.CommandId.ShellManagement.EXECUTE
 
     argv: List[str]
```

### Comparing `smp-0.3.3/smp/user/intercreate.py` & `smp-0.3.4/smp/user/intercreate.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """The Simple Management Protocol (SMP) Intercreate Management group."""
 
 from enum import IntEnum, auto, unique
+from typing import ClassVar
 
 from smp import error, header, message
 
 
 class _IntercreateManagementGroup:
-    _GROUP_ID = header.GroupId.INTERCREATE
+    _GROUP_ID: ClassVar = header.GroupId.INTERCREATE
 
 
 class ImageUploadWriteRequest(_IntercreateManagementGroup, message.WriteRequest):
     _COMMAND_ID = header.CommandId.Intercreate.UPLOAD
 
     off: int
     """The offset in the image to write to."""
```

### Comparing `smp-0.3.3/PKG-INFO` & `smp-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smp
-Version: 0.3.3
+Version: 0.3.4
 Summary: Simple Management Protocol (SMP) for remotely managing MCU firmware
 License: Apache-2.0
 Author: J.P. Hutchins
 Author-email: jphutchins@gmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

