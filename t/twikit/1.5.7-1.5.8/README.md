# Comparing `tmp/twikit-1.5.7.tar.gz` & `tmp/twikit-1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twikit-1.5.7.tar", last modified: Wed Apr 24 16:53:59 2024, max compression
+gzip compressed data, was "twikit-1.5.8.tar", last modified: Thu Apr 25 06:59:23 2024, max compression
```

## Comparing `twikit-1.5.7.tar` & `twikit-1.5.8.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 16:53:59.978966 twikit-1.5.7/
--rw-rw-rw-   0        0        0     1079 2024-04-13 12:42:36.000000 twikit-1.5.7/LICENSE
--rw-rw-rw-   0        0        0     3863 2024-04-24 16:53:59.975973 twikit-1.5.7/PKG-INFO
--rw-rw-rw-   0        0        0     3590 2024-04-13 12:42:36.000000 twikit-1.5.7/README.md
--rw-rw-rw-   0        0        0       42 2024-04-24 16:53:59.978966 twikit-1.5.7/setup.cfg
--rw-rw-rw-   0        0        0      694 2024-04-13 12:42:36.000000 twikit-1.5.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-24 16:53:59.899179 twikit-1.5.7/twikit/
--rw-rw-rw-   0        0        0      658 2024-04-24 16:49:51.000000 twikit-1.5.7/twikit/__init__.py
--rw-rw-rw-   0        0        0     1686 2024-04-23 16:10:15.000000 twikit-1.5.7/twikit/bookmark.py
--rw-rw-rw-   0        0        0   142787 2024-04-24 16:49:04.000000 twikit-1.5.7/twikit/client.py
--rw-rw-rw-   0        0        0     8639 2024-04-15 14:41:30.000000 twikit-1.5.7/twikit/community.py
--rw-rw-rw-   0        0        0     2666 2024-04-22 14:20:57.000000 twikit-1.5.7/twikit/errors.py
--rw-rw-rw-   0        0        0     7305 2024-04-13 12:42:36.000000 twikit-1.5.7/twikit/group.py
--rw-rw-rw-   0        0        0     2095 2024-04-23 16:02:50.000000 twikit-1.5.7/twikit/http.py
--rw-rw-rw-   0        0        0     7617 2024-04-13 12:42:37.000000 twikit-1.5.7/twikit/list.py
--rw-rw-rw-   0        0        0     3908 2024-04-13 12:42:37.000000 twikit-1.5.7/twikit/message.py
--rw-rw-rw-   0        0        0     1439 2024-04-13 14:30:38.000000 twikit-1.5.7/twikit/notification.py
--rw-rw-rw-   0        0        0        0 2024-04-23 16:07:38.000000 twikit-1.5.7/twikit/py.typed
--rw-rw-rw-   0        0        0     1070 2024-04-13 12:42:37.000000 twikit-1.5.7/twikit/trend.py
--rw-rw-rw-   0        0        0    22891 2024-04-24 16:28:18.000000 twikit-1.5.7/twikit/tweet.py
-drwxrwxrwx   0        0        0        0 2024-04-24 16:53:59.972981 twikit-1.5.7/twikit/twikit_async/
--rw-rw-rw-   0        0        0      610 2024-04-23 16:10:47.000000 twikit-1.5.7/twikit/twikit_async/__init__.py
--rw-rw-rw-   0        0        0     1758 2024-04-23 16:10:22.000000 twikit-1.5.7/twikit/twikit_async/bookmark.py
--rw-rw-rw-   0        0        0   145199 2024-04-24 16:49:39.000000 twikit-1.5.7/twikit/twikit_async/client.py
--rw-rw-rw-   0        0        0     8767 2024-04-15 14:48:23.000000 twikit-1.5.7/twikit/twikit_async/community.py
--rw-rw-rw-   0        0        0      875 2024-04-13 12:42:37.000000 twikit-1.5.7/twikit/twikit_async/errors.py
--rw-rw-rw-   0        0        0     7509 2024-04-13 12:42:37.000000 twikit-1.5.7/twikit/twikit_async/group.py
--rw-rw-rw-   0        0        0     2137 2024-04-14 11:11:58.000000 twikit-1.5.7/twikit/twikit_async/http.py
--rw-rw-rw-   0        0        0     7780 2024-04-13 12:42:37.000000 twikit-1.5.7/twikit/twikit_async/list.py
--rw-rw-rw-   0        0        0     3974 2024-04-13 12:42:37.000000 twikit-1.5.7/twikit/twikit_async/message.py
--rw-rw-rw-   0        0        0     1439 2024-04-13 12:42:37.000000 twikit-1.5.7/twikit/twikit_async/notification.py
--rw-rw-rw-   0        0        0     1079 2024-04-13 12:42:37.000000 twikit-1.5.7/twikit/twikit_async/trend.py
--rw-rw-rw-   0        0        0    22772 2024-04-24 16:29:28.000000 twikit-1.5.7/twikit/twikit_async/tweet.py
--rw-rw-rw-   0        0        0    14740 2024-04-16 15:30:17.000000 twikit-1.5.7/twikit/twikit_async/user.py
--rw-rw-rw-   0        0        0     3390 2024-04-13 12:42:37.000000 twikit-1.5.7/twikit/twikit_async/utils.py
--rw-rw-rw-   0        0        0    14517 2024-04-16 15:30:25.000000 twikit-1.5.7/twikit/user.py
--rw-rw-rw-   0        0        0    30253 2024-04-24 16:45:39.000000 twikit-1.5.7/twikit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-24 16:53:59.917130 twikit-1.5.7/twikit.egg-info/
--rw-rw-rw-   0        0        0     3863 2024-04-24 16:53:59.000000 twikit-1.5.7/twikit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      857 2024-04-24 16:53:59.000000 twikit-1.5.7/twikit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 16:53:59.000000 twikit-1.5.7/twikit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-04-24 16:53:59.000000 twikit-1.5.7/twikit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-24 16:53:59.000000 twikit-1.5.7/twikit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-25 06:59:23.013476 twikit-1.5.8/
+-rw-rw-rw-   0        0        0     1079 2024-04-13 12:42:36.000000 twikit-1.5.8/LICENSE
+-rw-rw-rw-   0        0        0     3863 2024-04-25 06:59:23.010478 twikit-1.5.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3590 2024-04-13 12:42:36.000000 twikit-1.5.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-25 06:59:23.013476 twikit-1.5.8/setup.cfg
+-rw-rw-rw-   0        0        0      694 2024-04-13 12:42:36.000000 twikit-1.5.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 06:59:22.933684 twikit-1.5.8/twikit/
+-rw-rw-rw-   0        0        0      658 2024-04-25 06:57:47.000000 twikit-1.5.8/twikit/__init__.py
+-rw-rw-rw-   0        0        0     1686 2024-04-23 16:10:15.000000 twikit-1.5.8/twikit/bookmark.py
+-rw-rw-rw-   0        0        0   139609 2024-04-25 06:49:11.000000 twikit-1.5.8/twikit/client.py
+-rw-rw-rw-   0        0        0     8639 2024-04-15 14:41:30.000000 twikit-1.5.8/twikit/community.py
+-rw-rw-rw-   0        0        0     2666 2024-04-22 14:20:57.000000 twikit-1.5.8/twikit/errors.py
+-rw-rw-rw-   0        0        0     7305 2024-04-13 12:42:36.000000 twikit-1.5.8/twikit/group.py
+-rw-rw-rw-   0        0        0     2095 2024-04-23 16:02:50.000000 twikit-1.5.8/twikit/http.py
+-rw-rw-rw-   0        0        0     7617 2024-04-13 12:42:37.000000 twikit-1.5.8/twikit/list.py
+-rw-rw-rw-   0        0        0     3908 2024-04-13 12:42:37.000000 twikit-1.5.8/twikit/message.py
+-rw-rw-rw-   0        0        0     1439 2024-04-13 14:30:38.000000 twikit-1.5.8/twikit/notification.py
+-rw-rw-rw-   0        0        0        0 2024-04-23 16:07:38.000000 twikit-1.5.8/twikit/py.typed
+-rw-rw-rw-   0        0        0     1070 2024-04-13 12:42:37.000000 twikit-1.5.8/twikit/trend.py
+-rw-rw-rw-   0        0        0    23612 2024-04-25 06:54:59.000000 twikit-1.5.8/twikit/tweet.py
+drwxrwxrwx   0        0        0        0 2024-04-25 06:59:23.008484 twikit-1.5.8/twikit/twikit_async/
+-rw-rw-rw-   0        0        0      610 2024-04-23 16:10:47.000000 twikit-1.5.8/twikit/twikit_async/__init__.py
+-rw-rw-rw-   0        0        0     1758 2024-04-23 16:10:22.000000 twikit-1.5.8/twikit/twikit_async/bookmark.py
+-rw-rw-rw-   0        0        0   141857 2024-04-25 06:47:26.000000 twikit-1.5.8/twikit/twikit_async/client.py
+-rw-rw-rw-   0        0        0     8767 2024-04-15 14:48:23.000000 twikit-1.5.8/twikit/twikit_async/community.py
+-rw-rw-rw-   0        0        0      875 2024-04-13 12:42:37.000000 twikit-1.5.8/twikit/twikit_async/errors.py
+-rw-rw-rw-   0        0        0     7509 2024-04-13 12:42:37.000000 twikit-1.5.8/twikit/twikit_async/group.py
+-rw-rw-rw-   0        0        0     2137 2024-04-14 11:11:58.000000 twikit-1.5.8/twikit/twikit_async/http.py
+-rw-rw-rw-   0        0        0     7780 2024-04-13 12:42:37.000000 twikit-1.5.8/twikit/twikit_async/list.py
+-rw-rw-rw-   0        0        0     3974 2024-04-13 12:42:37.000000 twikit-1.5.8/twikit/twikit_async/message.py
+-rw-rw-rw-   0        0        0     1439 2024-04-13 12:42:37.000000 twikit-1.5.8/twikit/twikit_async/notification.py
+-rw-rw-rw-   0        0        0     1079 2024-04-13 12:42:37.000000 twikit-1.5.8/twikit/twikit_async/trend.py
+-rw-rw-rw-   0        0        0    23493 2024-04-25 06:55:20.000000 twikit-1.5.8/twikit/twikit_async/tweet.py
+-rw-rw-rw-   0        0        0    14740 2024-04-25 06:56:56.000000 twikit-1.5.8/twikit/twikit_async/user.py
+-rw-rw-rw-   0        0        0     3390 2024-04-13 12:42:37.000000 twikit-1.5.8/twikit/twikit_async/utils.py
+-rw-rw-rw-   0        0        0    14517 2024-04-16 15:30:25.000000 twikit-1.5.8/twikit/user.py
+-rw-rw-rw-   0        0        0    30253 2024-04-25 02:12:28.000000 twikit-1.5.8/twikit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-25 06:59:22.951638 twikit-1.5.8/twikit.egg-info/
+-rw-rw-rw-   0        0        0     3863 2024-04-25 06:59:22.000000 twikit-1.5.8/twikit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      857 2024-04-25 06:59:22.000000 twikit-1.5.8/twikit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 06:59:22.000000 twikit-1.5.8/twikit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-04-25 06:59:22.000000 twikit-1.5.8/twikit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-25 06:59:22.000000 twikit-1.5.8/twikit.egg-info/top_level.txt
```

### Comparing `twikit-1.5.7/LICENSE` & `twikit-1.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `twikit-1.5.7/PKG-INFO` & `twikit-1.5.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twikit
-Version: 1.5.7
+Version: 1.5.8
 Summary: Twitter API wrapper for python with **no API key required**.
 Home-page: https://github.com/d60/twikit
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `twikit-1.5.7/README.md` & `twikit-1.5.8/README.md`

 * *Files identical despite different names*

### Comparing `twikit-1.5.7/setup.py` & `twikit-1.5.8/setup.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.7/twikit/__init__.py` & `twikit-1.5.8/twikit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ==========================
 Twikit Twitter API Wrapper
 ==========================
 
 A Python library for interacting with the Twitter API.
 """
 
-__version__ = '1.5.7'
+__version__ = '1.5.8'
 
 from .bookmark import BookmarkFolder
 from .client import Client
 from .community import (Community, CommunityCreator, CommunityMember,
                         CommunityRule)
 from .errors import *
 from .group import Group, GroupMessage
```

### Comparing `twikit-1.5.7/twikit/bookmark.py` & `twikit-1.5.8/twikit/bookmark.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.7/twikit/client.py` & `twikit-1.5.8/twikit/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 )
 from .group import Group, GroupMessage
 from .http import HTTPClient
 from .list import List
 from .message import Message
 from .notification import Notification
 from .trend import Trend
-from .tweet import CommunityNote, Poll, ScheduledTweet, Tweet
+from .tweet import CommunityNote, Poll, ScheduledTweet, Tweet, tweet_from_data
 from .user import User
 from .utils import (
     BOOKMARK_FOLDER_TIMELINE_FEATURES,
     COMMUNITY_TWEETS_FEATURES,
     COMMUNITY_NOTE_FEATURES,
     JOIN_COMMUNITY_FEATURES,
     LIST_FEATURES,
@@ -483,27 +483,18 @@
         for item in items:
             if item['entryId'].startswith('cursor-bottom'):
                 next_cursor = item['content']['value']
             if item['entryId'].startswith('cursor-top'):
                 previous_cursor = item['content']['value']
             if not item['entryId'].startswith(('tweet', 'search-grid')):
                 continue
-            tweet_info = find_dict(item, 'result')
-            if not tweet_info:
-                continue
-            tweet_info = tweet_info[0]
-            if 'tweet' in tweet_info:
-                tweet_info = tweet_info['tweet']
-            if 'core' not in tweet_info:
-                continue
-            if 'result' not in tweet_info['core']['user_results']:
-                continue
-            user_info = tweet_info['core']['user_results']['result']
-            if 'legacy' in tweet_info:
-                results.append(Tweet(self, tweet_info, User(self, user_info)))
+
+            tweet = tweet_from_data(self, item)
+            if tweet is not None:
+                results.append(tweet)
 
         if next_cursor is None:
             if product == 'Media':
                 entries = find_dict(
                     instructions, 'entries'
                 )[0]
                 next_cursor = entries[-1]['content']['value']
@@ -599,25 +590,26 @@
             'features': SIMILAR_POSTS_FEATURES
         })
         response = self.http.get(
             Endpoint.SIMILAR_POSTS,
             params=params,
             headers=self._base_headers
         ).json()
-
-        items = find_dict(response, 'entries')[0]
+        items_ = find_dict(response, 'entries')
         results = []
-        for item in items:
+        if not items_:
+            return results
+
+        for item in items_[0]:
             if not item['entryId'].startswith('tweet'):
                 continue
-            tweet_data = find_dict(item, 'result')[0]
-            if 'tweet' in tweet_data:
-                tweet_data = tweet_data['tweet']
-            user_data = tweet_data['core']['user_results']['result']
-            results.append(Tweet(self, tweet_data, User(self, user_data)))
+
+            tweet = tweet_from_data(self, item)
+            if tweet is not None:
+                results.append(tweet)
 
         return results
 
     def upload_media(
         self,
         source: str | bytes,
         wait_for_completion: bool = False,
@@ -1329,21 +1321,17 @@
         response = self._get_tweet_detail(tweet_id, cursor)
         entries = find_dict(response, 'entries')[0]
 
         results = []
         for entry in entries:
             if entry['entryId'].startswith(('cursor', 'label')):
                 continue
-            tweet_info = find_dict(entry, 'result')[0]
-            if tweet_info['__typename'] == 'TweetTombstone':
-                continue
-            if tweet_info['__typename'] == 'TweetWithVisibilityResults':
-                tweet_info = tweet_info['tweet']
-            user_info = tweet_info['core']['user_results']['result']
-            results.append(Tweet(self, tweet_info, User(self, user_info)))
+            tweet = tweet_from_data(self, entry)
+            if tweet is not None:
+                results.append(tweet)
 
         if entries[-1]['entryId'].startswith('cursor'):
             next_cursor = entries[-1]['content']['itemContent']['value']
             _fetch_next_result = partial(self._get_more_replies,
                                          tweet_id, next_cursor)
         else:
             next_cursor = None
@@ -1358,19 +1346,17 @@
     def _show_more_replies(self, tweet_id: str, cursor: str) -> Result[Tweet]:
         response = self._get_tweet_detail(tweet_id, cursor)
         items = find_dict(response, 'moduleItems')[0]
         results = []
         for item in items:
             if 'tweet' not in item['entryId']:
                 continue
-            tweet_data = find_dict(item, 'result')[0]
-            if 'tweet' in tweet_data:
-                tweet_data = tweet_data['tweet']
-            user_data = tweet_data['core']['user_results']['result']
-            results.append(Tweet(self, tweet_data, User(self, user_data)))
+            tweet = tweet_from_data(self, item)
+            if tweet is not None:
+                results.append(tweet)
         return Result(results)
 
     def get_tweet_by_id(
         self, tweet_id: str, cursor: str | None = None
     ) -> Tweet:
         """
         Fetches a tweet by tweet ID.
@@ -1399,59 +1385,40 @@
         replies_list = []
         related_tweets = []
         tweet = None
 
         for entry in entries:
             if entry['entryId'].startswith('cursor'):
                 continue
-            tweet_info_ = find_dict(entry, 'result')
-            if not tweet_info_:
-                continue
-            tweet_info = tweet_info_[0]
-
-            if tweet_info.get('__typename') == 'TweetTombstone':
+            tweet_object = tweet_from_data(self, entry)
+            if tweet_object is None:
                 continue
 
-            if tweet_info.get('__typename') == 'TweetWithVisibilityResults':
-                tweet_info = tweet_info['tweet']
-
-            user_info = find_dict(tweet_info, 'user_results')[0]['result']
-            tweet_object = Tweet(self, tweet_info, User(self, user_info))
-
             if entry['entryId'].startswith('tweetdetailrelatedtweets'):
                 related_tweets.append(tweet_object)
                 continue
 
             if entry['entryId'] == f'tweet-{tweet_id}':
-                if tweet_info.get('__typename') == 'TweetTombstone':
-                    raise TweetNotAvailable('This tweet is not available.')
-
                 tweet = tweet_object
             else:
                 if tweet is None:
                     reply_to.append(tweet_object)
                 else:
                     replies = []
                     sr_cursor = None
                     show_replies = None
 
                     for reply in entry['content']['items'][1:]:
                         if 'tweetcomposer' in reply['entryId']:
                             continue
-                        if 'tweet' in find_dict(reply, 'result'):
-                            reply = reply['tweet']
                         if 'tweet' in reply.get('entryId'):
-                            rpl_data = find_dict(reply, 'result')[0]
-                            if rpl_data.get('__typename') == 'TweetTombstone':
+                            rpl = tweet_from_data(self, reply)
+                            if rpl is None:
                                 continue
-                            usr_data = find_dict(
-                                rpl_data, 'user_results')[0]['result']
-                            replies.append(
-                                Tweet(self, rpl_data, User(self, usr_data))
-                            )
+                            replies.append(rpl)
                         if 'cursor' in reply.get('entryId'):
                             sr_cursor = reply['item']['itemContent']['value']
                             show_replies = partial(
                                 self._show_more_replies,
                                 tweet_id,
                                 sr_cursor
                             )
@@ -1805,35 +1772,27 @@
                 ('tweet', 'profile-conversation', 'profile-grid')
             ):
                 continue
 
             if entry_id.startswith('profile-conversation'):
                 tweets = item['content']['items']
                 replies = []
-
                 for reply in tweets[1:]:
-                    tweet_info = find_dict(reply, 'result')[0]
-                    if 'tweet' in tweet_info:
-                        tweet_info = tweet_info['tweet']
-                    user_info = find_dict(tweet_info, 'result')[0]
-                    user = User(self, user_info)
-
-                    replies.append(Tweet(self, tweet_info, user))
-
+                    tweet_object = tweet_from_data(self, reply)
+                    if tweet_object is None:
+                        continue
+                    replies.append(tweet_object)
                 item = tweets[0]
             else:
                 replies = None
 
-            tweet_info = find_dict(item, 'result')[0]
-            if 'tweet' in tweet_info:
-                tweet_info = tweet_info['tweet']
-            user_info = find_dict(tweet_info, 'result')[0]
-            tweet = Tweet(self, tweet_info, User(self, user_info))
+            tweet = tweet_from_data(self, item)
+            if tweet is None:
+                continue
             tweet.replies = replies
-
             results.append(tweet)
 
         return Result(
             results,
             partial(self.get_user_tweets,
                     user_id, tweet_type, count, next_cursor),
             next_cursor,
@@ -1908,19 +1867,18 @@
         items = find_dict(response, 'entries')[0]
         next_cursor = items[-1]['content']['value']
         results = []
 
         for item in items:
             if 'itemContent' not in item['content']:
                 continue
-            tweet_info = find_dict(item, 'result')[0]
-            if tweet_info['__typename'] == 'TweetWithVisibilityResults':
-                tweet_info = tweet_info['tweet']
-            user_info = tweet_info['core']['user_results']['result']
-            results.append(Tweet(self, tweet_info, user_info))
+            tweet = tweet_from_data(self, item)
+            if tweet is None:
+                continue
+            results.append(tweet)
 
         return Result(
             results,
             partial(self.get_timeline, count, seen_tweet_ids, next_cursor),
             next_cursor
         )
 
@@ -1990,19 +1948,18 @@
         items = find_dict(response, 'entries')[0]
         next_cursor = items[-1]['content']['value']
         results = []
 
         for item in items:
             if 'itemContent' not in item['content']:
                 continue
-            tweet_info = find_dict(item, 'result')[0]
-            if tweet_info['__typename'] == 'TweetWithVisibilityResults':
-                tweet_info = tweet_info['tweet']
-            user_info = tweet_info['core']['user_results']['result']
-            results.append(Tweet(self, tweet_info, user_info))
+            tweet = tweet_from_data(self, item)
+            if tweet is None:
+                continue
+            results.append(tweet)
 
         return Result(
             results,
             partial(self.get_latest_timeline,
                     count, seen_tweet_ids, next_cursor),
             next_cursor
         )
@@ -2291,17 +2248,18 @@
             previous_cursor = None
             fetch_previous_result = None
 
         results = []
         for item in items:
             if not item['entryId'].startswith('tweet'):
                 continue
-            tweet_info = find_dict(item, 'tweet_results')[0]['result']
-            user_info = tweet_info['core']['user_results']['result']
-            results.append(Tweet(self, tweet_info, User(self, user_info)))
+            tweet = tweet_from_data(self, item)
+            if tweet is None:
+                continue
+            results.append(tweet)
 
         return Result(
             results,
             partial(self.get_bookmarks, count, next_cursor, folder_id),
             next_cursor,
             fetch_previous_result,
             previous_cursor
@@ -3821,19 +3779,18 @@
         items = find_dict(response, 'entries')[0]
         next_cursor = items[-1]['content']['value']
 
         results = []
         for item in items:
             if not item['entryId'].startswith('tweet'):
                 continue
-            tweet_info = find_dict(item, 'result')[0]
-            if tweet_info['__typename'] == 'TweetWithVisibilityResults':
-                tweet_info = tweet_info['tweet']
-            user_info = find_dict(tweet_info, 'result')[0]
-            results.append(Tweet(self, tweet_info, User(self, user_info)))
+
+            tweet = tweet_from_data(self, item)
+            if tweet is not None:
+                results.append(tweet)
 
         return Result(
             results,
             partial(self.get_list_tweets, list_id, count, next_cursor),
             next_cursor
         )
 
@@ -4269,19 +4226,18 @@
             next_cursor = items[-1]['content']['value']
             previous_cursor = items[-2]['content']['value']
 
         tweets = []
         for item in items:
             if not item['entryId'].startswith(('tweet', 'communities-grid')):
                 continue
-            tweet_data = find_dict(item, 'result')[0]
-            if 'tweet' in tweet_data:
-                tweet_data = tweet_data['tweet']
-            user_data = tweet_data['core']['user_results']['result']
-            tweets.append(Tweet(self, tweet_data, User(self, user_data)))
+
+            tweet = tweet_from_data(self, item)
+            if tweet is not None:
+                tweets.append(tweet)
 
         return Result(
             tweets,
             partial(self.get_community_tweets, community_id,
                     tweet_type, count, next_cursor),
             next_cursor,
             partial(self.get_community_tweets, community_id,
@@ -4331,14 +4287,15 @@
             headers=self._base_headers
         ).json()
         items = find_dict(response, 'entries')[0]
         tweets = []
         for item in items:
             if not item['entryId'].startswith('tweet'):
                 continue
+            tweet = tweet_from_data(self, item)
             tweet_data = find_dict(item, 'result')[0]
             if 'tweet' in tweet_data:
                 tweet_data = tweet_data['tweet']
             user_data = tweet_data['core']['user_results']['result']
             community_data = tweet_data['community_results']['result']
             community_data['rest_id'] = community_data['id_str']
             community = Community(self, community_data)
@@ -4598,19 +4555,18 @@
         ).json()
 
         items = find_dict(response, 'entries')[0]
         tweets = []
         for item in items:
             if not item['entryId'].startswith('tweet'):
                 continue
-            tweet_data = find_dict(item, 'result')[0]
-            if 'tweet' in tweet_data:
-                tweet_data = tweet_data['tweet']
-            user_data = find_dict(tweet_data, 'result')[0]
-            tweets.append(Tweet(self, tweet_data, User(self, user_data)))
+
+            tweet = tweet_from_data(self, item)
+            if tweet is not None:
+                tweets.append(tweet)
 
         next_cursor = items[-1]['content']['value']
         previous_cursor = items[-2]['content']['value']
 
         return Result(
             tweets,
             partial(self.search_community_tweet, community_id,
```

### Comparing `twikit-1.5.7/twikit/community.py` & `twikit-1.5.8/twikit/community.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.7/twikit/errors.py` & `twikit-1.5.8/twikit/errors.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.7/twikit/group.py` & `twikit-1.5.8/twikit/group.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.7/twikit/http.py` & `twikit-1.5.8/twikit/http.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.7/twikit/list.py` & `twikit-1.5.8/twikit/list.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.7/twikit/message.py` & `twikit-1.5.8/twikit/message.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.7/twikit/notification.py` & `twikit-1.5.8/twikit/notification.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.7/twikit/trend.py` & `twikit-1.5.8/twikit/trend.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.7/twikit/tweet.py` & `twikit-1.5.8/twikit/tweet.py`

 * *Files 3% similar despite different names*

```diff
@@ -129,18 +129,19 @@
             self.retweeted_tweet: Tweet = Tweet(
                 client, retweeted_tweet, retweeted_user
             )
         else:
             self.retweeted_tweet = None
 
         note_tweet_results = find_dict(data, 'note_tweet_results')
+        self.full_text: str | None = None
         if note_tweet_results:
-            self.full_text: str = find_dict(note_tweet_results, 'text')[0]
-        else:
-            self.full_text = None
+            text_list = find_dict(note_tweet_results, 'text')
+            if text_list:
+                self.full_text = text_list[0]
 
         self.is_quote_status: bool = legacy['is_quote_status']
         self.possibly_sensitive: bool = legacy.get('possibly_sensitive')
         self.possibly_sensitive_editable: bool = legacy.get(
             'possibly_sensitive_editable')
         self.quote_count: int = legacy['quote_count']
         self.media: list = legacy['entities'].get('media')
@@ -463,14 +464,35 @@
     def __eq__(self, __value: object) -> bool:
         return isinstance(__value, Tweet) and self.id == __value.id
 
     def __ne__(self, __value: object) -> bool:
         return not self == __value
 
 
+def tweet_from_data(client: Client, data: dict) -> Tweet:
+    tweet_data_ = find_dict(data, 'result', True)
+    if not tweet_data_:
+        return None
+    tweet_data = tweet_data_[0]
+
+    if tweet_data.get('__typename') == 'TweetTombstone':
+        return None
+    if 'tweet' in tweet_data:
+        tweet_data = tweet_data['tweet']
+    if 'core' not in tweet_data:
+        return None
+    if 'result' not in tweet_data['core']['user_results']:
+        return None
+    if 'legacy' not in tweet_data:
+        return None
+
+    user_data = tweet_data['core']['user_results']['result']
+    return Tweet(client, tweet_data, User(client, user_data))
+
+
 class ScheduledTweet:
     def __init__(self, client: Client, data: dict) -> None:
         self._client = client
 
         self.id = data['rest_id']
         self.execute_at: int = data['scheduling_info']['execute_at']
         self.state: str = data['scheduling_info']['state']
```

### Comparing `twikit-1.5.7/twikit/twikit_async/__init__.py` & `twikit-1.5.8/twikit/twikit_async/__init__.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.7/twikit/twikit_async/bookmark.py` & `twikit-1.5.8/twikit/twikit_async/bookmark.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.7/twikit/twikit_async/client.py` & `twikit-1.5.8/twikit/twikit_async/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 )
 from .group import Group, GroupMessage
 from .http import HTTPClient
 from .list import List
 from .message import Message
 from .notification import Notification
 from .trend import Trend
-from .tweet import CommunityNote, Poll, ScheduledTweet, Tweet
+from .tweet import CommunityNote, Poll, ScheduledTweet, Tweet, tweet_from_data
 from .user import User
 from .utils import Flow, Result
 
 
 class Client:
     """
     A client for interacting with the Twitter API.
@@ -487,27 +487,18 @@
         for item in items:
             if item['entryId'].startswith('cursor-bottom'):
                 next_cursor = item['content']['value']
             if item['entryId'].startswith('cursor-top'):
                 previous_cursor = item['content']['value']
             if not item['entryId'].startswith(('tweet', 'search-grid')):
                 continue
-            tweet_info = find_dict(item, 'result')
-            if not tweet_info:
-                continue
-            tweet_info = tweet_info[0]
-            if 'tweet' in tweet_info:
-                tweet_info = tweet_info['tweet']
-            if 'core' not in tweet_info:
-                continue
-            if 'result' not in tweet_info['core']['user_results']:
-                continue
-            user_info = tweet_info['core']['user_results']['result']
-            if 'legacy' in tweet_info:
-                results.append(Tweet(self, tweet_info, User(self, user_info)))
+
+            tweet = tweet_from_data(self, item)
+            if tweet is not None:
+                results.append(tweet)
 
         if next_cursor is None:
             if product == 'Media':
                 entries = find_dict(
                     instructions, 'entries'
                 )[0]
                 next_cursor = entries[-1]['content']['value']
@@ -604,25 +595,26 @@
             'features': SIMILAR_POSTS_FEATURES
         })
         response = (await self.http.get(
             Endpoint.SIMILAR_POSTS,
             params=params,
             headers=self._base_headers
         )).json()
-
-        items = find_dict(response, 'entries')[0]
+        items_ = find_dict(response, 'entries')
         results = []
-        for item in items:
+        if not items_:
+            return results
+
+        for item in items_[0]:
             if not item['entryId'].startswith('tweet'):
                 continue
-            tweet_data = find_dict(item, 'result')[0]
-            if 'tweet' in tweet_data:
-                tweet_data = tweet_data['tweet']
-            user_data = tweet_data['core']['user_results']['result']
-            results.append(Tweet(self, tweet_data, User(self, user_data)))
+
+            tweet = tweet_from_data(self, item)
+            if tweet is not None:
+                results.append(tweet)
 
         return results
 
     async def upload_media(
         self,
         source: str | bytes,
         wait_for_completion: bool = False,
@@ -1344,21 +1336,17 @@
         response = await self._get_tweet_detail(tweet_id, cursor)
         entries = find_dict(response, 'entries')[0]
 
         results = []
         for entry in entries:
             if entry['entryId'].startswith(('cursor', 'label')):
                 continue
-            tweet_info = find_dict(entry, 'result')[0]
-            if tweet_info['__typename'] == 'TweetTombstone':
-                continue
-            if tweet_info['__typename'] == 'TweetWithVisibilityResults':
-                tweet_info = tweet_info['tweet']
-            user_info = tweet_info['core']['user_results']['result']
-            results.append(Tweet(self, tweet_info, User(self, user_info)))
+            tweet = tweet_from_data(self, entry)
+            if tweet is not None:
+                results.append(tweet)
 
         if entries[-1]['entryId'].startswith('cursor'):
             next_cursor = entries[-1]['content']['itemContent']['value']
             _fetch_next_result = partial(self._get_more_replies,
                                          tweet_id, next_cursor)
         else:
             next_cursor = None
@@ -1375,19 +1363,17 @@
     ) -> Result[Tweet]:
         response = await self._get_tweet_detail(tweet_id, cursor)
         items = find_dict(response, 'moduleItems')[0]
         results = []
         for item in items:
             if 'tweet' not in item['entryId']:
                 continue
-            tweet_data = find_dict(item, 'result')[0]
-            if 'tweet' in tweet_data:
-                tweet_data = tweet_data['tweet']
-            user_data = tweet_data['core']['user_results']['result']
-            results.append(Tweet(self, tweet_data, User(self, user_data)))
+            tweet = tweet_from_data(self, item)
+            if tweet is not None:
+                results.append(tweet)
         return Result(results)
 
     async def get_tweet_by_id(
         self, tweet_id: str, cursor: str | None = None
     ) -> Tweet:
         """
         Fetches a tweet by tweet ID.
@@ -1416,59 +1402,40 @@
         replies_list = []
         related_tweets = []
         tweet = None
 
         for entry in entries:
             if entry['entryId'].startswith('cursor'):
                 continue
-            tweet_info_ = find_dict(entry, 'result')
-            if not tweet_info_:
-                continue
-            tweet_info = tweet_info_[0]
-
-            if tweet_info.get('__typename') == 'TweetTombstone':
+            tweet_object = tweet_from_data(self, entry)
+            if tweet_object is None:
                 continue
 
-            if tweet_info['__typename'] == 'TweetWithVisibilityResults':
-                tweet_info = tweet_info['tweet']
-
-            user_info = find_dict(tweet_info, 'user_results')[0]['result']
-            tweet_object = Tweet(self, tweet_info, User(self, user_info))
-
             if entry['entryId'].startswith('tweetdetailrelatedtweets'):
                 related_tweets.append(tweet_object)
                 continue
 
             if entry['entryId'] == f'tweet-{tweet_id}':
-                if tweet_info.get('__typename') == 'TweetTombstone':
-                    raise TweetNotAvailable('This tweet is not available.')
-
                 tweet = tweet_object
             else:
                 if tweet is None:
                     reply_to.append(tweet_object)
                 else:
                     replies = []
                     sr_cursor = None
                     show_replies = None
-                    # Reply to reply
+
                     for reply in entry['content']['items'][1:]:
                         if 'tweetcomposer' in reply['entryId']:
                             continue
-                        if 'tweet' in find_dict(reply, 'result'):
-                            reply = reply['tweet']
                         if 'tweet' in reply.get('entryId'):
-                            rpl_data = find_dict(reply, 'result')[0]
-                            if rpl_data.get('__typename') == 'TweetTombstone':
+                            rpl = tweet_from_data(self, reply)
+                            if rpl is None:
                                 continue
-                            usr_data = find_dict(
-                                rpl_data, 'user_results')[0]['result']
-                            replies.append(
-                                Tweet(self, rpl_data, User(self, usr_data))
-                            )
+                            replies.append(rpl)
                         if 'cursor' in reply.get('entryId'):
                             sr_cursor = reply['item']['itemContent']['value']
                             show_replies = partial(
                                 self._show_more_replies,
                                 tweet_id,
                                 sr_cursor
                             )
@@ -1826,35 +1793,27 @@
                 ('tweet', 'profile-conversation', 'profile-grid')
             ):
                 continue
 
             if entry_id.startswith('profile-conversation'):
                 tweets = item['content']['items']
                 replies = []
-
                 for reply in tweets[1:]:
-                    tweet_info = find_dict(reply, 'result')[0]
-                    if 'tweet' in tweet_info:
-                        tweet_info = tweet_info['tweet']
-                    user_info = find_dict(tweet_info, 'result')[0]
-                    user = User(self, user_info)
-
-                    replies.append(Tweet(self, tweet_info, user))
-
+                    tweet_object = tweet_from_data(self, reply)
+                    if tweet_object is None:
+                        continue
+                    replies.append(tweet_object)
                 item = tweets[0]
             else:
                 replies = None
 
-            tweet_info = find_dict(item, 'result')[0]
-            if 'tweet' in tweet_info:
-                tweet_info = tweet_info['tweet']
-            user_info = find_dict(tweet_info, 'result')[0]
-            tweet = Tweet(self, tweet_info, User(self, user_info))
+            tweet = tweet_from_data(self, item)
+            if tweet is None:
+                continue
             tweet.replies = replies
-
             results.append(tweet)
 
         return Result(
             results,
             partial(self.get_user_tweets,
                     user_id, tweet_type, count, next_cursor),
             next_cursor,
@@ -1929,19 +1888,18 @@
         items = find_dict(response, 'entries')[0]
         next_cursor = items[-1]['content']['value']
         results = []
 
         for item in items:
             if 'itemContent' not in item['content']:
                 continue
-            tweet_info = find_dict(item, 'result')[0]
-            if tweet_info['__typename'] == 'TweetWithVisibilityResults':
-                tweet_info = tweet_info['tweet']
-            user_info = tweet_info['core']['user_results']['result']
-            results.append(Tweet(self, tweet_info, user_info))
+            tweet = tweet_from_data(self, item)
+            if tweet is None:
+                continue
+            results.append(tweet)
 
         return Result(
             results,
             partial(self.get_timeline, count, seen_tweet_ids, next_cursor),
             next_cursor
         )
 
@@ -2011,19 +1969,18 @@
         items = find_dict(response, 'entries')[0]
         next_cursor = items[-1]['content']['value']
         results = []
 
         for item in items:
             if 'itemContent' not in item['content']:
                 continue
-            tweet_info = find_dict(item, 'result')[0]
-            if tweet_info['__typename'] == 'TweetWithVisibilityResults':
-                tweet_info = tweet_info['tweet']
-            user_info = tweet_info['core']['user_results']['result']
-            results.append(Tweet(self, tweet_info, user_info))
+            tweet = tweet_from_data(self, item)
+            if tweet is None:
+                continue
+            results.append(tweet)
 
         return Result(
             results,
             partial(self.get_latest_timeline,
                     count, seen_tweet_ids, next_cursor),
             next_cursor
         )
@@ -2311,19 +2268,18 @@
                                             previous_cursor, folder_id)
         else:
             previous_cursor = None
             fetch_previous_result = None
 
         results = []
         for item in items:
-            if not item['entryId'].startswith('tweet'):
+            tweet = tweet_from_data(self, item)
+            if tweet is None:
                 continue
-            tweet_info = find_dict(item, 'tweet_results')[0]['result']
-            user_info = tweet_info['core']['user_results']['result']
-            results.append(Tweet(self, tweet_info, User(self, user_info)))
+            results.append(tweet)
 
         return Result(
             results,
             partial(self.get_bookmarks, count, next_cursor, folder_id),
             next_cursor,
             fetch_previous_result,
             previous_cursor
@@ -3846,19 +3802,18 @@
         items = find_dict(response, 'entries')[0]
         next_cursor = items[-1]['content']['value']
 
         results = []
         for item in items:
             if not item['entryId'].startswith('tweet'):
                 continue
-            tweet_info = find_dict(item, 'result')[0]
-            if tweet_info['__typename'] == 'TweetWithVisibilityResults':
-                tweet_info = tweet_info['tweet']
-            user_info = find_dict(tweet_info, 'result')[0]
-            results.append(Tweet(self, tweet_info, User(self, user_info)))
+
+            tweet = tweet_from_data(self, item)
+            if tweet is not None:
+                results.append(tweet)
 
         return Result(
             results,
             partial(self.get_list_tweets, list_id, count, next_cursor),
             next_cursor
         )
 
@@ -4299,19 +4254,18 @@
             next_cursor = items[-1]['content']['value']
             previous_cursor = items[-2]['content']['value']
 
         tweets = []
         for item in items:
             if not item['entryId'].startswith(('tweet', 'communities-grid')):
                 continue
-            tweet_data = find_dict(item, 'result')[0]
-            if 'tweet' in tweet_data:
-                tweet_data = tweet_data['tweet']
-            user_data = tweet_data['core']['user_results']['result']
-            tweets.append(Tweet(self, tweet_data, User(self, user_data)))
+
+            tweet = tweet_from_data(self, item)
+            if tweet is not None:
+                tweets.append(tweet)
 
         return Result(
             tweets,
             partial(self.get_community_tweets, community_id,
                     tweet_type, count, next_cursor),
             next_cursor,
             partial(self.get_community_tweets, community_id,
@@ -4628,19 +4582,18 @@
         )).json()
 
         items = find_dict(response, 'entries')[0]
         tweets = []
         for item in items:
             if not item['entryId'].startswith('tweet'):
                 continue
-            tweet_data = find_dict(item, 'result')[0]
-            if 'tweet' in tweet_data:
-                tweet_data = tweet_data['tweet']
-            user_data = find_dict(tweet_data, 'result')[0]
-            tweets.append(Tweet(self, tweet_data, User(self, user_data)))
+
+            tweet = tweet_from_data(self, item)
+            if tweet is not None:
+                tweets.append(tweet)
 
         next_cursor = items[-1]['content']['value']
         previous_cursor = items[-2]['content']['value']
 
         return Result(
             tweets,
             partial(self.search_community_tweet, community_id,
```

### Comparing `twikit-1.5.7/twikit/twikit_async/community.py` & `twikit-1.5.8/twikit/twikit_async/community.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.7/twikit/twikit_async/errors.py` & `twikit-1.5.8/twikit/twikit_async/errors.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.7/twikit/twikit_async/group.py` & `twikit-1.5.8/twikit/twikit_async/group.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.7/twikit/twikit_async/http.py` & `twikit-1.5.8/twikit/twikit_async/http.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.7/twikit/twikit_async/list.py` & `twikit-1.5.8/twikit/twikit_async/list.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.7/twikit/twikit_async/message.py` & `twikit-1.5.8/twikit/twikit_async/message.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.7/twikit/twikit_async/notification.py` & `twikit-1.5.8/twikit/twikit_async/notification.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.7/twikit/twikit_async/trend.py` & `twikit-1.5.8/twikit/twikit_async/trend.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.7/twikit/twikit_async/tweet.py` & `twikit-1.5.8/twikit/twikit_async/tweet.py`

 * *Files 3% similar despite different names*

```diff
@@ -126,18 +126,19 @@
             self.retweeted_tweet: Tweet = Tweet(
                 client, retweeted_tweet, retweeted_user
             )
         else:
             self.retweeted_tweet = None
 
         note_tweet_results = find_dict(data, 'note_tweet_results')
+        self.full_text: str | None = None
         if note_tweet_results:
-            self.full_text: str = find_dict(note_tweet_results, 'text')[0]
-        else:
-            self.full_text = None
+            text_list = find_dict(note_tweet_results, 'text')
+            if text_list:
+                self.full_text = text_list[0]
 
         self.is_quote_status: bool = legacy['is_quote_status']
         self.possibly_sensitive: bool = legacy.get('possibly_sensitive')
         self.possibly_sensitive_editable: bool = legacy.get(
             'possibly_sensitive_editable')
         self.quote_count: int = legacy['quote_count']
         self.media: list = legacy['entities'].get('media')
@@ -460,14 +461,35 @@
     def __eq__(self, __value: object) -> bool:
         return isinstance(__value, Tweet) and self.id == __value.id
 
     def __ne__(self, __value: object) -> bool:
         return not self == __value
 
 
+def tweet_from_data(client: Client, data: dict) -> Tweet:
+    tweet_data_ = find_dict(data, 'result', True)
+    if not tweet_data_:
+        return None
+    tweet_data = tweet_data_[0]
+
+    if tweet_data.get('__typename') == 'TweetTombstone':
+        return None
+    if 'tweet' in tweet_data:
+        tweet_data = tweet_data['tweet']
+    if 'core' not in tweet_data:
+        return None
+    if 'result' not in tweet_data['core']['user_results']:
+        return None
+    if 'legacy' not in tweet_data:
+        return None
+
+    user_data = tweet_data['core']['user_results']['result']
+    return Tweet(client, tweet_data, User(client, user_data))
+
+
 class ScheduledTweet:
     def __init__(self, client: Client, data: dict) -> None:
         self._client = client
 
         self.id = data['rest_id']
         self.execute_at: int = data['scheduling_info']['execute_at']
         self.state: str = data['scheduling_info']['state']
```

### Comparing `twikit-1.5.7/twikit/twikit_async/user.py` & `twikit-1.5.8/twikit/twikit_async/user.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.7/twikit/twikit_async/utils.py` & `twikit-1.5.8/twikit/twikit_async/utils.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.7/twikit/user.py` & `twikit-1.5.8/twikit/user.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.7/twikit/utils.py` & `twikit-1.5.8/twikit/utils.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.7/twikit.egg-info/PKG-INFO` & `twikit-1.5.8/twikit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twikit
-Version: 1.5.7
+Version: 1.5.8
 Summary: Twitter API wrapper for python with **no API key required**.
 Home-page: https://github.com/d60/twikit
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `twikit-1.5.7/twikit.egg-info/SOURCES.txt` & `twikit-1.5.8/twikit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

