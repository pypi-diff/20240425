# Comparing `tmp/espn_api-0.9.3.tar.gz` & `tmp/espn_api-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "espn_api-0.9.3.tar", last modified: Fri Dec 18 15:39:35 2020, max compression
+gzip compressed data, was "espn_api-0.9.4.tar", last modified: Sat Jan  2 16:35:16 2021, max compression
```

## Comparing `espn_api-0.9.3.tar` & `espn_api-0.9.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-18 15:39:35.975674 espn_api-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (116)      366 2020-12-18 15:39:35.975674 espn_api-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2777 2020-12-18 15:39:20.000000 espn_api-0.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-18 15:39:35.971674 espn_api-0.9.3/espn_api/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-18 15:39:20.000000 espn_api-0.9.3/espn_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4139 2020-12-18 15:39:20.000000 espn_api-0.9.3/espn_api/base_league.py
--rw-r--r--   0 runner    (1001) docker     (116)     1139 2020-12-18 15:39:20.000000 espn_api-0.9.3/espn_api/base_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-18 15:39:35.975674 espn_api-0.9.3/espn_api/basketball/
--rw-r--r--   0 runner    (1001) docker     (116)      204 2020-12-18 15:39:20.000000 espn_api-0.9.3/espn_api/basketball/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      991 2020-12-18 15:39:20.000000 espn_api-0.9.3/espn_api/basketball/activity.py
--rw-r--r--   0 runner    (1001) docker     (116)     1879 2020-12-18 15:39:20.000000 espn_api-0.9.3/espn_api/basketball/constant.py
--rw-r--r--   0 runner    (1001) docker     (116)     5079 2020-12-18 15:39:20.000000 espn_api-0.9.3/espn_api/basketball/league.py
--rw-r--r--   0 runner    (1001) docker     (116)     2420 2020-12-18 15:39:20.000000 espn_api-0.9.3/espn_api/basketball/matchup.py
--rw-r--r--   0 runner    (1001) docker     (116)     1772 2020-12-18 15:39:20.000000 espn_api-0.9.3/espn_api/basketball/player.py
--rw-r--r--   0 runner    (1001) docker     (116)     2213 2020-12-18 15:39:20.000000 espn_api-0.9.3/espn_api/basketball/team.py
--rw-r--r--   0 runner    (1001) docker     (116)      750 2020-12-18 15:39:20.000000 espn_api-0.9.3/espn_api/basketball/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-18 15:39:35.975674 espn_api-0.9.3/espn_api/football/
--rw-r--r--   0 runner    (1001) docker     (116)      314 2020-12-18 15:39:20.000000 espn_api-0.9.3/espn_api/football/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1210 2020-12-18 15:39:20.000000 espn_api-0.9.3/espn_api/football/activity.py
--rw-r--r--   0 runner    (1001) docker     (116)     1755 2020-12-18 15:39:20.000000 espn_api-0.9.3/espn_api/football/box_player.py
--rw-r--r--   0 runner    (1001) docker     (116)     1819 2020-12-18 15:39:20.000000 espn_api-0.9.3/espn_api/football/box_score.py
--rw-r--r--   0 runner    (1001) docker     (116)     3476 2020-12-18 15:39:20.000000 espn_api-0.9.3/espn_api/football/constant.py
--rw-r--r--   0 runner    (1001) docker     (116)    12135 2020-12-18 15:39:20.000000 espn_api-0.9.3/espn_api/football/league.py
--rw-r--r--   0 runner    (1001) docker     (116)      693 2020-12-18 15:39:20.000000 espn_api-0.9.3/espn_api/football/matchup.py
--rw-r--r--   0 runner    (1001) docker     (116)      669 2020-12-18 15:39:20.000000 espn_api-0.9.3/espn_api/football/pick.py
--rw-r--r--   0 runner    (1001) docker     (116)     2445 2020-12-18 15:39:20.000000 espn_api-0.9.3/espn_api/football/player.py
--rw-r--r--   0 runner    (1001) docker     (116)     3144 2020-12-18 15:39:20.000000 espn_api-0.9.3/espn_api/football/team.py
--rw-r--r--   0 runner    (1001) docker     (116)     2223 2020-12-18 15:39:20.000000 espn_api-0.9.3/espn_api/football/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-18 15:39:35.975674 espn_api-0.9.3/espn_api/requests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-18 15:39:20.000000 espn_api-0.9.3/espn_api/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      169 2020-12-18 15:39:20.000000 espn_api-0.9.3/espn_api/requests/constant.py
--rw-r--r--   0 runner    (1001) docker     (116)     5027 2020-12-18 15:39:20.000000 espn_api-0.9.3/espn_api/requests/espn_requests.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-18 15:39:35.975674 espn_api-0.9.3/espn_api/utils/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-18 15:39:20.000000 espn_api-0.9.3/espn_api/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1361 2020-12-18 15:39:20.000000 espn_api-0.9.3/espn_api/utils/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-18 15:39:35.971674 espn_api-0.9.3/espn_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      366 2020-12-18 15:39:35.000000 espn_api-0.9.3/espn_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      966 2020-12-18 15:39:35.000000 espn_api-0.9.3/espn_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-18 15:39:35.000000 espn_api-0.9.3/espn_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       23 2020-12-18 15:39:35.000000 espn_api-0.9.3/espn_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        9 2020-12-18 15:39:35.000000 espn_api-0.9.3/espn_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      130 2020-12-18 15:39:35.979673 espn_api-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      594 2020-12-18 15:39:20.000000 espn_api-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-02 16:35:16.480103 espn_api-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (116)      366 2021-01-02 16:35:16.480103 espn_api-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     2777 2021-01-02 16:35:06.000000 espn_api-0.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-02 16:35:16.480103 espn_api-0.9.4/espn_api/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-02 16:35:06.000000 espn_api-0.9.4/espn_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4139 2021-01-02 16:35:06.000000 espn_api-0.9.4/espn_api/base_league.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1139 2021-01-02 16:35:06.000000 espn_api-0.9.4/espn_api/base_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-02 16:35:16.480103 espn_api-0.9.4/espn_api/basketball/
+-rw-r--r--   0 runner    (1001) docker     (116)      204 2021-01-02 16:35:06.000000 espn_api-0.9.4/espn_api/basketball/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      991 2021-01-02 16:35:06.000000 espn_api-0.9.4/espn_api/basketball/activity.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1879 2021-01-02 16:35:06.000000 espn_api-0.9.4/espn_api/basketball/constant.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5079 2021-01-02 16:35:06.000000 espn_api-0.9.4/espn_api/basketball/league.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2423 2021-01-02 16:35:06.000000 espn_api-0.9.4/espn_api/basketball/matchup.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1772 2021-01-02 16:35:06.000000 espn_api-0.9.4/espn_api/basketball/player.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2213 2021-01-02 16:35:06.000000 espn_api-0.9.4/espn_api/basketball/team.py
+-rw-r--r--   0 runner    (1001) docker     (116)      750 2021-01-02 16:35:06.000000 espn_api-0.9.4/espn_api/basketball/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-02 16:35:16.480103 espn_api-0.9.4/espn_api/football/
+-rw-r--r--   0 runner    (1001) docker     (116)      314 2021-01-02 16:35:06.000000 espn_api-0.9.4/espn_api/football/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1210 2021-01-02 16:35:06.000000 espn_api-0.9.4/espn_api/football/activity.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1755 2021-01-02 16:35:06.000000 espn_api-0.9.4/espn_api/football/box_player.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1819 2021-01-02 16:35:06.000000 espn_api-0.9.4/espn_api/football/box_score.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3476 2021-01-02 16:35:06.000000 espn_api-0.9.4/espn_api/football/constant.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12135 2021-01-02 16:35:06.000000 espn_api-0.9.4/espn_api/football/league.py
+-rw-r--r--   0 runner    (1001) docker     (116)      693 2021-01-02 16:35:06.000000 espn_api-0.9.4/espn_api/football/matchup.py
+-rw-r--r--   0 runner    (1001) docker     (116)      669 2021-01-02 16:35:06.000000 espn_api-0.9.4/espn_api/football/pick.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2445 2021-01-02 16:35:06.000000 espn_api-0.9.4/espn_api/football/player.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3144 2021-01-02 16:35:06.000000 espn_api-0.9.4/espn_api/football/team.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2223 2021-01-02 16:35:06.000000 espn_api-0.9.4/espn_api/football/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-02 16:35:16.480103 espn_api-0.9.4/espn_api/requests/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-02 16:35:06.000000 espn_api-0.9.4/espn_api/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      169 2021-01-02 16:35:06.000000 espn_api-0.9.4/espn_api/requests/constant.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5027 2021-01-02 16:35:06.000000 espn_api-0.9.4/espn_api/requests/espn_requests.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-02 16:35:16.480103 espn_api-0.9.4/espn_api/utils/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-02 16:35:06.000000 espn_api-0.9.4/espn_api/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1361 2021-01-02 16:35:06.000000 espn_api-0.9.4/espn_api/utils/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-02 16:35:16.480103 espn_api-0.9.4/espn_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)      366 2021-01-02 16:35:16.000000 espn_api-0.9.4/espn_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      966 2021-01-02 16:35:16.000000 espn_api-0.9.4/espn_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-02 16:35:16.000000 espn_api-0.9.4/espn_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       23 2021-01-02 16:35:16.000000 espn_api-0.9.4/espn_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        9 2021-01-02 16:35:16.000000 espn_api-0.9.4/espn_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      130 2021-01-02 16:35:16.480103 espn_api-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)      594 2021-01-02 16:35:06.000000 espn_api-0.9.4/setup.py
```

### Comparing `espn_api-0.9.3/README.md` & `espn_api-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `espn_api-0.9.3/espn_api/base_league.py` & `espn_api-0.9.4/espn_api/base_league.py`

 * *Files identical despite different names*

### Comparing `espn_api-0.9.3/espn_api/base_settings.py` & `espn_api-0.9.4/espn_api/base_settings.py`

 * *Files identical despite different names*

### Comparing `espn_api-0.9.3/espn_api/basketball/activity.py` & `espn_api-0.9.4/espn_api/basketball/activity.py`

 * *Files identical despite different names*

### Comparing `espn_api-0.9.3/espn_api/basketball/constant.py` & `espn_api-0.9.4/espn_api/basketball/constant.py`

 * *Files identical despite different names*

### Comparing `espn_api-0.9.3/espn_api/basketball/league.py` & `espn_api-0.9.4/espn_api/basketball/league.py`

 * *Files identical despite different names*

### Comparing `espn_api-0.9.3/espn_api/basketball/matchup.py` & `espn_api-0.9.4/espn_api/basketball/matchup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 class Matchup(object):
     '''Creates Matchup instance'''
     def __init__(self, data):
         self.home_team_live_score = None
         self.away_team_live_score = None
         self._fetch_matchup_info(data)
-        
+
     def __repr__(self):
         # TODO: use final score when that's available?
         # writing this too early to see if data['home']['totalPoints'] is final score
         # it might also be used for points leagues instead of category leagues
         if not self.away_team_live_score:
             return 'Matchup(%s, %s)' % (self.home_team, self.away_team, )
         else:
@@ -26,22 +26,22 @@
         self.home_team = data['home']['teamId']
         self.home_final_score = data['home']['totalPoints']
         self.away_team = data['away']['teamId']
         self.away_final_score = data['away']['totalPoints']
         self.winner = data['winner']
         self.home_team_cats = None
         self.away_team_cats = None
-        
+
         # if stats are available
-        if 'cumulativeScore' in data['home'].keys():
+        if 'cumulativeScore' in data['home'].keys() and data['home']['cumulativeScore']['scoreByStat']:
 
             self.home_team_live_score = (data['home']['cumulativeScore']['wins'] +
                                          data['home']['cumulativeScore']['ties']/2)
             self.away_team_live_score = (data['away']['cumulativeScore']['wins'] +
                                          data['away']['cumulativeScore']['ties']/2)
-            
+
             self.home_team_cats = { STATS_MAP[i]: {'score': data['home']['cumulativeScore']['scoreByStat'][i]['score'],
                                                    'result': data['home']['cumulativeScore']['scoreByStat'][i]['result']} for i in data['home']['cumulativeScore']['scoreByStat'].keys()}
-            
+
             self.away_team_cats = { STATS_MAP[i]: {'score': data['away']['cumulativeScore']['scoreByStat'][i]['score'],
                                                    'result': data['away']['cumulativeScore']['scoreByStat'][i]['result']} for i in data['away']['cumulativeScore']['scoreByStat'].keys()}
-        
+
```

### Comparing `espn_api-0.9.3/espn_api/basketball/player.py` & `espn_api-0.9.4/espn_api/basketball/player.py`

 * *Files identical despite different names*

### Comparing `espn_api-0.9.3/espn_api/basketball/team.py` & `espn_api-0.9.4/espn_api/basketball/team.py`

 * *Files identical despite different names*

### Comparing `espn_api-0.9.3/espn_api/basketball/utils.py` & `espn_api-0.9.4/espn_api/basketball/utils.py`

 * *Files identical despite different names*

### Comparing `espn_api-0.9.3/espn_api/football/activity.py` & `espn_api-0.9.4/espn_api/football/activity.py`

 * *Files identical despite different names*

### Comparing `espn_api-0.9.3/espn_api/football/box_player.py` & `espn_api-0.9.4/espn_api/football/box_player.py`

 * *Files identical despite different names*

### Comparing `espn_api-0.9.3/espn_api/football/box_score.py` & `espn_api-0.9.4/espn_api/football/box_score.py`

 * *Files identical despite different names*

### Comparing `espn_api-0.9.3/espn_api/football/constant.py` & `espn_api-0.9.4/espn_api/football/constant.py`

 * *Files identical despite different names*

### Comparing `espn_api-0.9.3/espn_api/football/league.py` & `espn_api-0.9.4/espn_api/football/league.py`

 * *Files identical despite different names*

### Comparing `espn_api-0.9.3/espn_api/football/matchup.py` & `espn_api-0.9.4/espn_api/football/matchup.py`

 * *Files identical despite different names*

### Comparing `espn_api-0.9.3/espn_api/football/pick.py` & `espn_api-0.9.4/espn_api/football/pick.py`

 * *Files identical despite different names*

### Comparing `espn_api-0.9.3/espn_api/football/player.py` & `espn_api-0.9.4/espn_api/football/player.py`

 * *Files identical despite different names*

### Comparing `espn_api-0.9.3/espn_api/football/team.py` & `espn_api-0.9.4/espn_api/football/team.py`

 * *Files identical despite different names*

### Comparing `espn_api-0.9.3/espn_api/football/utils.py` & `espn_api-0.9.4/espn_api/football/utils.py`

 * *Files identical despite different names*

### Comparing `espn_api-0.9.3/espn_api/requests/espn_requests.py` & `espn_api-0.9.4/espn_api/requests/espn_requests.py`

 * *Files identical despite different names*

### Comparing `espn_api-0.9.3/espn_api/utils/logger.py` & `espn_api-0.9.4/espn_api/utils/logger.py`

 * *Files identical despite different names*

### Comparing `espn_api-0.9.3/espn_api.egg-info/SOURCES.txt` & `espn_api-0.9.4/espn_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `espn_api-0.9.3/setup.py` & `espn_api-0.9.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='espn_api',
     packages=find_packages(),
-    version='0.9.3',
+    version='0.9.4',
     author='Christian Wendt',
     description='ESPN API',
     install_requires=['requests>=2.0.0,<3.0.0'],
     setup_requires=['nose>=1.0'],
     test_suite='nose.collector',
     tests_require=['nose', 'requests_mock', 'coverage'],
     url='https://github.com/cwendt94/espn-api',
```

