# Comparing `tmp/limoon-0.0.5.tar.gz` & `tmp/limoon-0.0.7.tar.gz`

## Comparing `limoon-0.0.5.tar` & `limoon-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     5554 2020-02-02 00:00:00.000000 limoon-0.0.5/DOCUMENTATION.md
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 limoon-0.0.5/README.md
--rw-r--r--   0        0        0    31396 2020-02-02 00:00:00.000000 limoon-0.0.5/limoon-logo.png
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 limoon-0.0.5/.github/workflows/doc.yml
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 limoon-0.0.5/.github/workflows/publish.yml
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 limoon-0.0.5/.github/workflows/test.yml
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 limoon-0.0.5/src/limoon/__init__.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 limoon-0.0.5/src/limoon/constant.py
--rw-r--r--   0        0        0     5351 2020-02-02 00:00:00.000000 limoon-0.0.5/src/limoon/core.py
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 limoon-0.0.5/src/limoon/exception.py
--rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 limoon-0.0.5/src/limoon/model.py
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 limoon-0.0.5/src/limoon/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 limoon-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 limoon-0.0.5/tests/test.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 limoon-0.0.5/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 limoon-0.0.5/LICENSE.txt
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 limoon-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 limoon-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     5805 2020-02-02 00:00:00.000000 limoon-0.0.7/DOCUMENTATION.md
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 limoon-0.0.7/README.md
+-rw-r--r--   0        0        0    31396 2020-02-02 00:00:00.000000 limoon-0.0.7/limoon-logo.png
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 limoon-0.0.7/.github/workflows/doc.yml
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 limoon-0.0.7/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 limoon-0.0.7/.github/workflows/test.yml
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 limoon-0.0.7/src/limoon/__init__.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 limoon-0.0.7/src/limoon/constant.py
+-rw-r--r--   0        0        0     5506 2020-02-02 00:00:00.000000 limoon-0.0.7/src/limoon/core.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 limoon-0.0.7/src/limoon/exception.py
+-rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 limoon-0.0.7/src/limoon/model.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 limoon-0.0.7/src/limoon/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 limoon-0.0.7/tests/__init__.py
+-rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 limoon-0.0.7/tests/test.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 limoon-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 limoon-0.0.7/LICENSE.txt
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 limoon-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 limoon-0.0.7/PKG-INFO
```

### Comparing `limoon-0.0.5/DOCUMENTATION.md` & `limoon-0.0.7/DOCUMENTATION.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,87 +1,56 @@
 # Table of Contents
 
 * [limoon](#limoon)
-* [limoon.exception](#limoon.exception)
-  * [TopicNotFound](#limoon.exception.TopicNotFound)
-  * [EntryNotFound](#limoon.exception.EntryNotFound)
-  * [AuthorNotFound](#limoon.exception.AuthorNotFound)
 * [limoon.core](#limoon.core)
   * [get\_topic](#limoon.core.get_topic)
   * [get\_entry](#limoon.core.get_entry)
   * [get\_author](#limoon.core.get_author)
   * [get\_author\_rank](#limoon.core.get_author_rank)
   * [get\_author\_topic](#limoon.core.get_author_topic)
   * [get\_agenda](#limoon.core.get_agenda)
   * [get\_debe](#limoon.core.get_debe)
+* [limoon.utils](#limoon.utils)
+* [limoon.constant](#limoon.constant)
 * [limoon.model](#limoon.model)
   * [Rank](#limoon.model.Rank)
   * [Entry](#limoon.model.Entry)
   * [Topic](#limoon.model.Topic)
   * [Author](#limoon.model.Author)
-* [limoon.constant](#limoon.constant)
-* [limoon.utils](#limoon.utils)
+* [limoon.exception](#limoon.exception)
+  * [TopicNotFound](#limoon.exception.TopicNotFound)
+  * [EntryNotFound](#limoon.exception.EntryNotFound)
+  * [AuthorNotFound](#limoon.exception.AuthorNotFound)
+  * [PageNotFound](#limoon.exception.PageNotFound)
 
 <a id="limoon"></a>
 
 # limoon
 
-<a id="limoon.exception"></a>
-
-# limoon.exception
-
-<a id="limoon.exception.TopicNotFound"></a>
-
-## TopicNotFound Objects
-
-```python
-class TopicNotFound(Exception)
-```
-
-The topic record is not available.
-
-<a id="limoon.exception.EntryNotFound"></a>
-
-## EntryNotFound Objects
-
-```python
-class EntryNotFound(Exception)
-```
-
-The entry record is not available.
-
-<a id="limoon.exception.AuthorNotFound"></a>
-
-## AuthorNotFound Objects
-
-```python
-class AuthorNotFound(Exception)
-```
-
-The author record is not available.
-
 <a id="limoon.core"></a>
 
 # limoon.core
 
 <a id="limoon.core.get_topic"></a>
 
 #### get\_topic
 
 ```python
 def get_topic(topic_keywords: TopicKeywords,
-              max_entry: int = None) -> model.Topic
+              max_entry: int = None,
+              page: int = 1) -> model.Topic
 ```
 
 This function get Ekşi Sözlük topic.
 
 **Arguments**:
 
 - `topic_keywords` _str_ - Keywords (or path) of topic to be get.
-- `max_entry` _int=None_ - Maximum number of entrys to be get from page.
+- `max_entry` _int=None_ - Maximum number of entrys get from per page.
+- `page` _int=1_ - Specific topic page.
   
 
 **Returns**:
 
 - `model.Topic` _class_ - Topic data class.
 
 <a id="limoon.core.get_entry"></a>
@@ -150,15 +119,15 @@
 ```
 
 This function get Ekşi Sözlük author topic.
 
 **Arguments**:
 
 - `nickname` _str_ - Unique author nickname.
-- `max_entry` _int=None_ - Maximum number of entrys to be get from page.
+- `max_entry` _int=None_ - Maximum number of entrys get from per page.
   
 
 **Returns**:
 
 - `model.Topic` _class_ - Topic data class.
 
 <a id="limoon.core.get_agenda"></a>
@@ -170,16 +139,16 @@
                max_entry: int = None) -> Iterator[model.Topic]
 ```
 
 This function get Ekşi Sözlük agenda (gündem) page.
 
 **Arguments**:
 
-- `max_topic` _int=None_ - Maximum number of topics to be get from agenda.
-- `max_entry` _int=None_ - Maximum number of entrys to be get from topic.
+- `max_topic` _int=None_ - Maximum number of topics get from agenda.
+- `max_entry` _int=None_ - Maximum number of entrys get from topic.
   
 
 **Returns**:
 
 - `Iterator[model.Topic]` - Topic data classes.
 
 <a id="limoon.core.get_debe"></a>
@@ -190,21 +159,29 @@
 def get_debe(max_entry: int = None) -> Iterator[model.Entry]
 ```
 
 This function get Ekşi Sözlük debe page.
 
 **Arguments**:
 
-- `max_entry` _int=None_ - Maximum number of entrys to be get page.
+- `max_entry` _int=None_ - Maximum number of entrys get per page.
   
 
 **Returns**:
 
 - `Iterator[model.Topic]` - Entry data classes.
 
+<a id="limoon.utils"></a>
+
+# limoon.utils
+
+<a id="limoon.constant"></a>
+
+# limoon.constant
+
 <a id="limoon.model"></a>
 
 # limoon.model
 
 <a id="limoon.model.Rank"></a>
 
 ## Rank Objects
@@ -280,15 +257,51 @@
 - `total_entry` _int_ - Author total entry count.
 - `follower_count` _int_ - Author total follower count.
 - `following_count` _int_ - Author total following count.
 - `avatar_url` _str_ - Author avatar HTTP link.
 - `rank` _class_ - Author rank.
 - `url` _str_ - Author HTTP link.
 
-<a id="limoon.constant"></a>
+<a id="limoon.exception"></a>
 
-# limoon.constant
+# limoon.exception
 
-<a id="limoon.utils"></a>
+<a id="limoon.exception.TopicNotFound"></a>
 
-# limoon.utils
+## TopicNotFound Objects
+
+```python
+class TopicNotFound(Exception)
+```
+
+The topic record is not available.
+
+<a id="limoon.exception.EntryNotFound"></a>
+
+## EntryNotFound Objects
+
+```python
+class EntryNotFound(Exception)
+```
+
+The entry record is not available.
+
+<a id="limoon.exception.AuthorNotFound"></a>
+
+## AuthorNotFound Objects
+
+```python
+class AuthorNotFound(Exception)
+```
+
+The author record is not available.
+
+<a id="limoon.exception.PageNotFound"></a>
+
+## PageNotFound Objects
+
+```python
+class PageNotFound(Exception)
+```
+
+The page record is not available.
```

### Comparing `limoon-0.0.5/README.md` & `limoon-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `limoon-0.0.5/limoon-logo.png` & `limoon-0.0.7/limoon-logo.png`

 * *Files identical despite different names*

### Comparing `limoon-0.0.5/.github/workflows/doc.yml` & `limoon-0.0.7/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `limoon-0.0.5/.github/workflows/publish.yml` & `limoon-0.0.7/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `limoon-0.0.5/.github/workflows/test.yml` & `limoon-0.0.7/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `limoon-0.0.5/src/limoon/core.py` & `limoon-0.0.7/src/limoon/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,47 @@
 from http import HTTPStatus
-from typing import TypeVar, Iterator, Callable
+from typing import Callable, Iterator, TypeVar, Union
 from urllib.parse import urlparse
 
 from requests_html import HTMLResponse, HTMLSession
 
 from limoon import constant, exception, model, utils
 
-
 # Typings
 EntryID = TypeVar("EntryID", Callable, int)
 TopicKeywords = TypeVar("TopicKeywords", Callable, str)
 Nickname = TypeVar("Nickname", Callable, str)
 SearchKeywords = TypeVar("SearchKeywords", Callable, str)
 
 # Session
 session = HTMLSession()
 
 
-def request(endpoint: str) -> HTMLResponse:
-    return session.get(constant.BASE_URL + endpoint)
+def request(endpoint: str, params: dict = {}) -> HTMLResponse:
+    return session.get(constant.BASE_URL + endpoint, params=params)
 
 
-def get_topic(topic_keywords: TopicKeywords, max_entry: int = None) -> model.Topic:
+def get_topic(
+    topic_keywords: TopicKeywords, max_entry: int = None, page: int = 1
+) -> model.Topic:
     """This function get Ekşi Sözlük topic.
 
     Arguments:
     topic_keywords (str): Keywords (or path) of topic to be get.
-    max_entry (int=None): Maximum number of entrys to be get from page.
+    max_entry (int=None): Maximum number of entrys get from per page.
+    page (int=1): Specific topic page.
 
     Returns:
     model.Topic (class): Topic data class.
     """
 
-    r = request(constant.TOPIC_ROUTE.format(topic_keywords))
+    if not isinstance(page, int):
+        raise TypeError
+
+    r = request(constant.TOPIC_ROUTE.format(topic_keywords), params={"p": page})
 
     if r.status_code == HTTPStatus.NOT_FOUND:
         raise exception.TopicNotFound()
 
     h1 = r.html.find("h1#title", first=True)
     path = h1.find("a", first=True).attrs["href"]
     page_count = r.html.find("div.pager", first=True)
@@ -50,15 +55,15 @@
     )
 
 
 def get_entry(entry_id: EntryID) -> model.Entry:
     """This function get Ekşi Sözlük entry.
 
     Arguments:
-    entry_id (int): Unique entry identity. 
+    entry_id (int): Unique entry identity.
 
     Returns:
     model.Entry (class): Entry data class.
     """
 
     if not isinstance(entry_id, int):
         raise TypeError
@@ -73,15 +78,15 @@
     return next(utils.entry_parser(r.html))
 
 
 def get_author(nickname: Nickname) -> model.Author:
     """This function get Ekşi Sözlük author.
 
     Arguments:
-    nickname (str): Unique author nickname. 
+    nickname (str): Unique author nickname.
 
     Returns:
     model.Author (class): Author data class.
     """
 
     r = request(constant.AUTHOR_ROUTE.format(nickname))
 
@@ -107,15 +112,15 @@
     )
 
 
 def get_author_rank(nickname: Nickname) -> model.Rank:
     """This function get Ekşi Sözlük author rank.
 
     Arguments:
-    nickname (str): Unique author nickname. 
+    nickname (str): Unique author nickname.
 
     Returns:
     model.Rank (class): Rank data class.
     """
 
     author = get_author(nickname)
 
@@ -123,30 +128,31 @@
 
 
 def get_author_topic(nickname: Nickname, max_entry: int = None) -> model.Topic:
     """This function get Ekşi Sözlük author topic.
 
     Arguments:
     nickname (str): Unique author nickname.
-    max_entry (int=None): Maximum number of entrys to be get from page.
+    max_entry (int=None): Maximum number of entrys get from per page.
 
     Returns:
     model.Topic (class): Topic data class.
     """
 
     r = request(constant.AUTHOR_TOPIC_ROUTE.format(nickname))
-    
+
     return get_topic(urlparse(r.url).path[1:], max_entry=max_entry)
 
+
 def get_agenda(max_topic: int = None, max_entry: int = None) -> Iterator[model.Topic]:
     """This function get Ekşi Sözlük agenda (gündem) page.
 
     Arguments:
-    max_topic (int=None): Maximum number of topics to be get from agenda.
-    max_entry (int=None): Maximum number of entrys to be get from topic.
+    max_topic (int=None): Maximum number of topics get from agenda.
+    max_entry (int=None): Maximum number of entrys get from topic.
 
     Returns:
     Iterator[model.Topic]: Topic data classes.
     """
 
     r = request(constant.AGENDA_ROUTE)
 
@@ -162,15 +168,15 @@
         )
 
 
 def get_debe(max_entry: int = None) -> Iterator[model.Entry]:
     """This function get Ekşi Sözlük debe page.
 
     Arguments:
-    max_entry (int=None): Maximum number of entrys to be get page.
+    max_entry (int=None): Maximum number of entrys get per page.
 
     Returns:
     Iterator[model.Topic]: Entry data classes.
     """
 
     r = request(constant.DEBE_ROUTE)
```

### Comparing `limoon-0.0.5/src/limoon/model.py` & `limoon-0.0.7/src/limoon/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import re
 from dataclasses import dataclass, field
-from typing import Iterator, Union, TypeVar, Callable
+from typing import Callable, Iterator, TypeVar, Union
 
 from limoon import constant
 
 # Typings
 URL = TypeError("URL", Callable, str)
 
 
 @dataclass
 class Rank:
     """Rank data class.
-    
+
     Arguments:
     name (str): Custom rank name.
     karma (int): Rank karma number.
     """
 
     name: str
     karma: int
@@ -23,15 +23,15 @@
     def __repr__(self):
         return "Rank()"
 
 
 @dataclass
 class Entry:
     """Entry data class.
-    
+
     Arguments:
     id (int): Unique entry identity.
     author_nickname (str): Author who created entry.
     content (str): Entry content (with HTML tags).
     favorite_count (int): Entry favorite count.
     created (str): Datetime of create entry.
     edited (str|bool): Datetime of edit entry.
```

### Comparing `limoon-0.0.5/src/limoon/utils.py` & `limoon-0.0.7/src/limoon/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 from typing import Iterator
 
-from requests_html import HTML, Element
+from requests_html import HTML
 
 from limoon import model
 
 
-def extract_entry_data(element: Element) -> list:
-    author = element.find("a.entry-author", first=True)
-    content = element.find("div.content", first=True)
-    favorite_count = element.attrs["data-favorite-count"]
-    created = element.find("a.entry-date", first=True)
-
-    return [
-        int(element.attrs["data-id"]),
-        author.text,
-        content.text,
-        int(favorite_count),
-        created.text,
-    ]
-
-
 def entry_parser(html: HTML, max_entry: int = None) -> Iterator[model.Entry]:
     entry_items = html.find("ul#entry-item-list", first=True).find("li#entry-item")
 
     for item in entry_items[:max_entry]:
-        entry_data = extract_entry_data(item)
-        yield model.Entry(*entry_data)
+        author = item.find("a.entry-author", first=True)
+        content = item.find("div.content", first=True)
+        favorite_count = item.attrs["data-favorite-count"]
+        created = item.find("a.entry-date", first=True)
+
+        yield model.Entry(
+            int(item.attrs["data-id"]),
+            author.text,
+            content.text,
+            int(favorite_count),
+            created.text,
+        )
```

### Comparing `limoon-0.0.5/tests/test.py` & `limoon-0.0.7/tests/test.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,14 +13,24 @@
         assert topic.title == "linux"
         assert topic.path == "linux--32084"
         assert len(list(topic.entrys)) > 1
         assert type(list(topic.entrys)) is list
         assert topic.page_count > 1
         assert topic.url == "https://eksisozluk.com/linux--32084"
 
+    def test_get_topic_page(self):
+        topic = limoon.get_topic("linux--32084", page=42)
+        entrys = list(topic.entrys)
+
+        assert len(entrys) == 10
+        assert type(entrys) is list
+        assert topic.page_count > 1
+        assert entrys[7].author_nickname == "hooker with a penis"
+        assert "sene olmus 2012, ve hala linux sadece çekirdektir." in entrys[7].content
+
     def test_get_entry(self):
         entry = limoon.get_entry(1)
 
         assert type(entry) is limoon.Entry
         assert entry.id == 1
         assert entry.author_nickname == "ssg"
         assert type(entry.content) is str
@@ -46,15 +56,15 @@
 
     def test_get_author_rank(self):
         author_rank = limoon.get_author_rank("ssg")
 
         assert type(author_rank) is limoon.Rank
         assert type(author_rank.name) is str
         assert type(author_rank.karma) is int
-        assert author_rank.karma > 1 
+        assert author_rank.karma > 1
 
     def test_get_author_topic(self):
         author_topic = limoon.get_author_topic("ssg")
 
         assert type(author_topic) is limoon.Topic
         assert author_topic.id == 31795
         assert author_topic.title == "ssg"
@@ -66,14 +76,18 @@
 
 
 class TestException:
     def test_topic_not_found(self):
         with pytest.raises(exception.TopicNotFound):
             limoon.get_topic("böylebirbaslikyok")
 
+    def test_topic_page_not_found(self):
+        with pytest.raises(exception.TopicNotFound):
+            limoon.get_topic("linux--32084", page=123456789)
+
     def test_entry_not_found(self):
         with pytest.raises(exception.EntryNotFound):
             limoon.get_entry(123456789)
 
     def test_author_not_found(self):
         with pytest.raises(exception.AuthorNotFound):
             limoon.get_author("böylebirkullanıcıyok")
```

### Comparing `limoon-0.0.5/.gitignore` & `limoon-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `limoon-0.0.5/LICENSE.txt` & `limoon-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `limoon-0.0.5/pyproject.toml` & `limoon-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `limoon-0.0.5/PKG-INFO` & `limoon-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: limoon
-Version: 0.0.5
+Version: 0.0.7
 Summary: Web scraper base Pythonic API for Ekşi Sözlük
 Project-URL: Source, https://github.com/beucismis/limoon
 Project-URL: Issues, https://github.com/beucismis/limoon/issues
 Project-URL: Documentation, https://github.com/beucismis/limoon/DOCUMENTATION.md
 Author-email: beucismis <beucismis@tutamail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

