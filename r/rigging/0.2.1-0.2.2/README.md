# Comparing `tmp/rigging-0.2.1.tar.gz` & `tmp/rigging-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rigging-0.2.1.tar", max compression
+gzip compressed data, was "rigging-0.2.2.tar", max compression
```

## Comparing `rigging-0.2.1.tar` & `rigging-0.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1066 2024-04-10 22:37:42.924340 rigging-0.2.1/LICENSE
--rw-r--r--   0        0        0     6803 2024-04-10 22:37:42.924340 rigging-0.2.1/README.md
--rw-r--r--   0        0        0     1841 2024-04-10 22:37:42.924340 rigging-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      375 2024-04-10 22:37:42.924340 rigging-0.2.1/rigging/__init__.py
--rw-r--r--   0        0        0    12752 2024-04-10 22:37:42.924340 rigging-0.2.1/rigging/chat.py
--rw-r--r--   0        0        0      457 2024-04-10 22:37:42.924340 rigging-0.2.1/rigging/error.py
--rw-r--r--   0        0        0     5068 2024-04-10 22:37:42.924340 rigging-0.2.1/rigging/generator.py
--rw-r--r--   0        0        0     1501 2024-04-10 22:37:42.924340 rigging-0.2.1/rigging/logging.py
--rw-r--r--   0        0        0     6593 2024-04-10 22:37:42.924340 rigging-0.2.1/rigging/message.py
--rw-r--r--   0        0        0     8638 2024-04-10 22:37:42.924340 rigging-0.2.1/rigging/model.py
--rw-r--r--   0        0        0     1090 2024-04-10 22:37:42.924340 rigging-0.2.1/rigging/prompt.py
--rw-r--r--   0        0        0        0 2024-04-10 22:37:42.924340 rigging-0.2.1/rigging/py.typed
--rw-r--r--   0        0        0     8455 2024-04-10 22:37:42.924340 rigging-0.2.1/rigging/tool.py
--rw-r--r--   0        0        0     7535 1970-01-01 00:00:00.000000 rigging-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-25 15:43:17.481841 rigging-0.2.2/LICENSE
+-rw-r--r--   0        0        0     6803 2024-04-25 15:43:17.481841 rigging-0.2.2/README.md
+-rw-r--r--   0        0        0     1842 2024-04-25 15:43:17.481841 rigging-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      536 2024-04-25 15:43:17.481841 rigging-0.2.2/rigging/__init__.py
+-rw-r--r--   0        0        0    14218 2024-04-25 15:43:17.485841 rigging-0.2.2/rigging/chat.py
+-rw-r--r--   0        0        0      457 2024-04-25 15:43:17.485841 rigging-0.2.2/rigging/error.py
+-rw-r--r--   0        0        0     5068 2024-04-25 15:43:17.485841 rigging-0.2.2/rigging/generator.py
+-rw-r--r--   0        0        0     1501 2024-04-25 15:43:17.485841 rigging-0.2.2/rigging/logging.py
+-rw-r--r--   0        0        0     8077 2024-04-25 15:43:17.485841 rigging-0.2.2/rigging/message.py
+-rw-r--r--   0        0        0     8682 2024-04-25 15:43:17.485841 rigging-0.2.2/rigging/model.py
+-rw-r--r--   0        0        0     1090 2024-04-25 15:43:17.485841 rigging-0.2.2/rigging/prompt.py
+-rw-r--r--   0        0        0        0 2024-04-25 15:43:17.485841 rigging-0.2.2/rigging/py.typed
+-rw-r--r--   0        0        0     8455 2024-04-25 15:43:17.485841 rigging-0.2.2/rigging/tool.py
+-rw-r--r--   0        0        0     7536 1970-01-01 00:00:00.000000 rigging-0.2.2/PKG-INFO
```

### Comparing `rigging-0.2.1/LICENSE` & `rigging-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rigging-0.2.1/README.md` & `rigging-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `rigging-0.2.1/pyproject.toml` & `rigging-0.2.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "rigging"
-version = "0.2.1"
+version = "0.2.2"
 description = "LLM Interaction Framework"
 authors = ["Nick Landers <monoxgas@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/dreadnode/rigging"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "<3.13,>=3.10"
 pydantic = "2.5.3"
 pydantic-xml = "2.7.0"
 loguru = "^0.7.2"
-litellm = "1.34.5"
+litellm = "1.35.21"
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.27.1"
 mypy = "^1.8.0"
 ruff = "^0.1.14"
 pytest = "^8.0.0"
```

### Comparing `rigging-0.2.1/rigging/chat.py` & `rigging-0.2.2/rigging/chat.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,40 +57,28 @@
         return [t.cast(MessageDict, message.model_dump()) for message in self.all]
 
     def restart(self) -> "PendingChat":
         if self.pending_chat is None:
             raise ValueError("Cannot restart chat that was not created with a PendingChat")
         return PendingChat(self.pending_chat.generator, self.messages, self.pending_chat.params)
 
-    @t.overload
-    def continue_(self, messages: t.Sequence[MessageDict]) -> "PendingChat":
-        ...
-
-    @t.overload
-    def continue_(self, messages: MessageDict) -> "PendingChat":
-        ...
+    # TODO: Why are these overloads here? I wonder if IDEs preferred them
 
-    @t.overload
-    def continue_(self, messages: t.Sequence[Message]) -> "PendingChat":
-        ...
-
-    @t.overload
-    def continue_(self, messages: Message) -> "PendingChat":
-        ...
-
-    def continue_(
-        self, messages: t.Sequence[Message] | t.Sequence[MessageDict] | Message | MessageDict
+    def fork(
+        self, messages: t.Sequence[Message] | t.Sequence[MessageDict] | Message | MessageDict | str
     ) -> "PendingChat":
         if self.pending_chat is None:
             raise ValueError("Cannot continue chat that was not created with a PendingChat")
 
-        messages_list: list[Message] = (
-            Message.fit_list(messages) if isinstance(messages, t.Sequence) else [Message.fit(messages)]
-        )
-        return PendingChat(self.pending_chat.generator, self.all + messages_list, self.pending_chat.params)
+        pending = PendingChat(self.pending_chat.generator, self.all, self.pending_chat.params)
+        pending.add(messages)
+        return pending
+
+    def continue_(self, messages: t.Sequence[Message] | t.Sequence[MessageDict] | Message | str) -> "PendingChat":
+        return self.fork(messages)
 
     def clone(self) -> "Chat":
         return Chat(
             [m.model_copy() for m in self.messages], [m.model_copy() for m in self.next_messages], self.pending_chat
         )
 
     def apply(self, **kwargs: str) -> "Chat":
@@ -147,14 +135,40 @@
         return self.with_params(GenerateParams(**kwargs))
 
     def with_params(self, params: "GenerateParams") -> "PendingChat":
         if params is not None:
             self.params = params
         return self
 
+    def add(
+        self, messages: t.Sequence[MessageDict] | t.Sequence[Message] | MessageDict | Message | str
+    ) -> "PendingChat":
+        message_list: list[Message] = (
+            [Message.fit(messages)]
+            if not isinstance(messages, t.Sequence) or isinstance(messages, str)
+            else Message.fit_list(messages)
+        )
+        # If the last message is the same role as the first new message, append to it
+        if self.chat.next_messages and self.chat.next_messages[-1].role == message_list[0].role:
+            self.chat.next_messages[-1].content += "\n" + message_list[0].content
+            message_list = message_list[1:]
+        else:
+            self.chat.next_messages += message_list
+        return self
+
+    def fork(
+        self, messages: t.Sequence[MessageDict] | t.Sequence[Message] | MessageDict | Message | str
+    ) -> "PendingChat":
+        return self.clone().add(messages)
+
+    def continue_(
+        self, messages: t.Sequence[MessageDict] | t.Sequence[Message] | MessageDict | Message | str
+    ) -> "PendingChat":
+        return self.fork(messages)
+
     def clone(self) -> "PendingChat":
         new = PendingChat(self.generator, [], self.params)
         new.chat = self.chat.clone()
         return new
 
     def apply(self, **kwargs: str) -> "PendingChat":
         new = self.clone()
@@ -331,14 +345,37 @@
                 self.chat.all + new_messages, callback, reset_between, drop_internal, max_rounds
             )
             new_messages = new_messages[:-1] + next_messages
 
         return new_messages
 
     @t.overload
+    def run_with(
+        self,
+        messages: t.Sequence[MessageDict] | t.Sequence[Message] | MessageDict | Message | str,
+        count: t.Literal[None] = None,
+    ) -> Chat:
+        ...
+
+    @t.overload
+    def run_with(
+        self,
+        messages: t.Sequence[MessageDict] | t.Sequence[Message] | MessageDict | Message | str,
+        count: int,
+    ) -> list[Chat]:
+        ...
+
+    def run_with(
+        self,
+        messages: t.Sequence[MessageDict] | t.Sequence[Message] | MessageDict | Message | str,
+        count: int | None = None,
+    ) -> Chat | list[Chat]:
+        return self.add(messages).run(count)
+
+    @t.overload
     def run(self, count: t.Literal[None] = None) -> Chat:
         ...
 
     @t.overload
     def run(self, count: int) -> list[Chat]:
         ...
```

### Comparing `rigging-0.2.1/rigging/generator.py` & `rigging-0.2.2/rigging/generator.py`

 * *Files identical despite different names*

### Comparing `rigging-0.2.1/rigging/logging.py` & `rigging-0.2.2/rigging/logging.py`

 * *Files identical despite different names*

### Comparing `rigging-0.2.1/rigging/message.py` & `rigging-0.2.2/rigging/message.py`

 * *Files 12% similar despite different names*

```diff
@@ -63,28 +63,56 @@
     def _remove_part(self, part: ParsedMessagePart) -> str:
         self._content = self._content[: part.slice_.start] + self._content[part.slice_.stop :]
         self.parts.remove(part)
         return self._content
 
     def _add_part(self, part: ParsedMessagePart) -> None:
         for existing in self.parts:
+            if part.slice_ == existing.slice_ and isinstance(part.model, type(existing.model)):
+                return  # We clearly already have this part defined
             if max(part.slice_.start, existing.slice_.start) < min(part.slice_.stop, existing.slice_.stop):
                 raise ValueError("Incoming part overlaps with an existing part")
         self.parts.append(part)
 
+    # Looks more complicated than it is. We just want to clean all the models
+    # in the message content by re-serializing them. As we do so, we'll need
+    # to watch for the total size of our message shifting and update the slices
+    # of the following parts accordingly. In other words, as A expands, B which
+    # follows will have a new start slice and end slice.
+    #
+    # TODO: We should probably just re-trigger parsing for everything
     def _sync_parts(self) -> None:
+        shift = 0
         for part in self.parts:
+            existing = self._content[part.slice_]
+
+            # Adjust for any previous shifts
+            part.slice_ = slice(part.slice_.start + shift, part.slice_.stop + shift)
+
+            # Check if the content has changed
             xml_content = part.model.to_pretty_xml()
+            if xml_content == existing:
+                continue
+
+            # Otherwise update content, add to shift, and update this slice
+            old_length = part.slice_.stop - part.slice_.start
+            new_length = len(xml_content)
+
             self._content = self._content[: part.slice_.start] + xml_content + self._content[part.slice_.stop :]
-            part.slice_ = slice(part.slice_.start, part.slice_.start + len(xml_content))
+            part.slice_ = slice(part.slice_.start, part.slice_.start + new_length)
+
+            shift += new_length - old_length
 
     @computed_field  # type: ignore[misc]
     @property
     def content(self) -> str:
-        self._sync_parts()
+        # We used to sync the models and content each time it was accessed,
+        # hence the getter. Now we just return the stored content.
+        # I'll leave it as is for now in case we want to add any
+        # logic here in the future.
         return self._content
 
     @content.setter
     def content(self, value: str) -> None:
         # TODO: Maintain any parsed parts which are
         # still in the content - our move to slices for
         # tracking parsed parts makes this more complicated
@@ -146,15 +174,15 @@
             try:
                 for model, slice_ in model_class.from_text(self.content):
                     self._add_part(ParsedMessagePart(model=model, slice_=slice_))
                     parsed.append(model)
             except MissingModelError as e:
                 if fail_on_missing:
                     raise e
-
+        self._sync_parts()
         return parsed
 
     @classmethod
     def from_model(
         cls: type["Message"], models: Model | t.Sequence[Model], role: Role = "user", suffix: str | None = None
     ) -> "Message":
         parts: list[ParsedMessagePart] = []
@@ -171,12 +199,14 @@
         return cls(role=role, content=content, parts=parts)
 
     @classmethod
     def fit_list(cls, messages: t.Sequence["Message"] | t.Sequence[MessageDict]) -> list["Message"]:
         return [cls.fit(message) for message in messages]
 
     @classmethod
-    def fit(cls, message: t.Union["Message", MessageDict]) -> "Message":
+    def fit(cls, message: t.Union["Message", MessageDict, str]) -> "Message":
+        if isinstance(message, str):
+            return cls(role="user", content=message)
         return cls(**message) if isinstance(message, dict) else message
 
 
 Messages = t.Sequence[MessageDict] | t.Sequence[Message]
```

### Comparing `rigging-0.2.1/rigging/model.py` & `rigging-0.2.2/rigging/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from xml.etree import ElementTree as ET
 
 from pydantic import ValidationError, field_validator
 from pydantic.alias_generators import to_snake
 from pydantic_xml import BaseXmlModel
 from pydantic_xml import attr as attr
 from pydantic_xml import element as element
+from pydantic_xml import wrapped as wrapped
 from pydantic_xml.element import SearchMode  # type: ignore [attr-defined]
 from pydantic_xml.typedefs import NsMap
 
 from rigging.error import MissingModelError
 
 #
 # Core XML serializable models for messages
```

### Comparing `rigging-0.2.1/rigging/prompt.py` & `rigging-0.2.2/rigging/prompt.py`

 * *Files identical despite different names*

### Comparing `rigging-0.2.1/rigging/tool.py` & `rigging-0.2.2/rigging/tool.py`

 * *Files identical despite different names*

### Comparing `rigging-0.2.1/PKG-INFO` & `rigging-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: rigging
-Version: 0.2.1
+Version: 0.2.2
 Summary: LLM Interaction Framework
 Home-page: https://github.com/dreadnode/rigging
 License: MIT
 Author: Nick Landers
 Author-email: monoxgas@gmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: litellm (==1.34.5)
+Requires-Dist: litellm (==1.35.21)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: pydantic (==2.5.3)
 Requires-Dist: pydantic-xml (==2.7.0)
 Project-URL: Repository, https://github.com/dreadnode/rigging
 Description-Content-Type: text/markdown
 
 # Rigging
```

