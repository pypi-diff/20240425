# Comparing `tmp/enkanetworkv2.py-2.0.4.tar.gz` & `tmp/enkanetworkv2.py-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enkanetworkv2.py-2.0.4.tar", last modified: Sun Apr  7 21:51:00 2024, max compression
+gzip compressed data, was "enkanetworkv2.py-2.0.5.tar", last modified: Thu Apr 25 10:00:21 2024, max compression
```

## Comparing `enkanetworkv2.py-2.0.4.tar` & `enkanetworkv2.py-2.0.5.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 21:51:00.799888 enkanetworkv2.py-2.0.4/
--rw-rw-rw-   0        0        0     1070 2024-02-24 18:53:52.000000 enkanetworkv2.py-2.0.4/LICENSE
--rw-rw-rw-   0        0        0       36 2024-02-24 18:58:13.000000 enkanetworkv2.py-2.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0    19341 2024-04-07 21:51:00.798889 enkanetworkv2.py-2.0.4/PKG-INFO
--rw-rw-rw-   0        0        0    18242 2024-02-24 19:02:02.000000 enkanetworkv2.py-2.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-07 21:51:00.700102 enkanetworkv2.py-2.0.4/enkanetwork/
--rw-rw-rw-   0        0        0     1462 2024-04-07 21:50:47.000000 enkanetworkv2.py-2.0.4/enkanetwork/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 21:51:00.677694 enkanetworkv2.py-2.0.4/enkanetwork/assets/
-drwxrwxrwx   0        0        0        0 2024-04-07 21:51:00.721178 enkanetworkv2.py-2.0.4/enkanetwork/assets/data/
--rw-rw-rw-   0        0        0    54227 2024-04-06 16:12:07.000000 enkanetworkv2.py-2.0.4/enkanetwork/assets/data/artifact_props.json
--rw-rw-rw-   0        0        0  1078669 2024-04-06 16:12:05.000000 enkanetworkv2.py-2.0.4/enkanetwork/assets/data/artifacts.json
--rw-rw-rw-   0        0        0    43169 2024-04-06 16:12:07.000000 enkanetworkv2.py-2.0.4/enkanetwork/assets/data/characters.json
--rw-rw-rw-   0        0        0    51875 2024-04-06 16:12:07.000000 enkanetworkv2.py-2.0.4/enkanetwork/assets/data/constellations.json
--rw-rw-rw-   0        0        0    12713 2024-04-06 16:12:05.000000 enkanetworkv2.py-2.0.4/enkanetwork/assets/data/costumes.json
--rw-rw-rw-   0        0        0  1313515 2024-04-06 16:12:07.000000 enkanetworkv2.py-2.0.4/enkanetwork/assets/data/fight_props.json
--rw-rw-rw-   0        0        0    55882 2024-04-06 16:12:04.000000 enkanetworkv2.py-2.0.4/enkanetwork/assets/data/namecards.json
--rw-rw-rw-   0        0        0     6321 2024-04-06 16:43:28.000000 enkanetworkv2.py-2.0.4/enkanetwork/assets/data/pfps.json
--rw-rw-rw-   0        0        0    85057 2024-04-06 16:12:07.000000 enkanetworkv2.py-2.0.4/enkanetwork/assets/data/skills.json
--rw-rw-rw-   0        0        0    41531 2024-04-06 16:12:04.000000 enkanetworkv2.py-2.0.4/enkanetwork/assets/data/weapons.json
-drwxrwxrwx   0        0        0        0 2024-04-07 21:51:00.742897 enkanetworkv2.py-2.0.4/enkanetwork/assets/langs/
--rw-rw-rw-   0        0        0   549230 2024-04-06 16:14:44.000000 enkanetworkv2.py-2.0.4/enkanetwork/assets/langs/artifact_sets.json
--rw-rw-rw-   0        0        0  2391484 2024-04-06 16:14:46.000000 enkanetworkv2.py-2.0.4/enkanetwork/assets/langs/artifacts.json
--rw-rw-rw-   0        0        0    32879 2024-04-06 16:14:46.000000 enkanetworkv2.py-2.0.4/enkanetwork/assets/langs/characters.json
--rw-rw-rw-   0        0        0   304646 2024-04-06 16:14:47.000000 enkanetworkv2.py-2.0.4/enkanetwork/assets/langs/constellations.json
--rw-rw-rw-   0        0        0    30562 2024-02-24 19:12:22.000000 enkanetworkv2.py-2.0.4/enkanetwork/assets/langs/fight_props.json
--rw-rw-rw-   0        0        0   119245 2024-04-06 16:14:47.000000 enkanetworkv2.py-2.0.4/enkanetwork/assets/langs/namecards.json
--rw-rw-rw-   0        0        0   301093 2024-04-06 16:14:47.000000 enkanetworkv2.py-2.0.4/enkanetwork/assets/langs/skills.json
--rw-rw-rw-   0        0        0   112669 2024-04-06 16:14:47.000000 enkanetworkv2.py-2.0.4/enkanetwork/assets/langs/weapons.json
--rw-rw-rw-   0        0        0     8270 2024-04-06 17:04:36.000000 enkanetworkv2.py-2.0.4/enkanetwork/assets.py
--rw-rw-rw-   0        0        0      645 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.4/enkanetwork/cache.py
--rw-rw-rw-   0        0        0    12474 2024-04-07 20:58:35.000000 enkanetworkv2.py-2.0.4/enkanetwork/client.py
--rw-rw-rw-   0        0        0      798 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.4/enkanetwork/config.py
--rw-rw-rw-   0        0        0     1099 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.4/enkanetwork/enum.py
--rw-rw-rw-   0        0        0     1925 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.4/enkanetwork/exception.py
--rw-rw-rw-   0        0        0     7345 2024-02-24 18:56:30.000000 enkanetworkv2.py-2.0.4/enkanetwork/http.py
-drwxrwxrwx   0        0        0        0 2024-04-07 21:51:00.761435 enkanetworkv2.py-2.0.4/enkanetwork/model/
--rw-rw-rw-   0        0        0      137 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.4/enkanetwork/model/__init__.py
--rw-rw-rw-   0        0        0     5029 2024-04-06 17:00:40.000000 enkanetworkv2.py-2.0.4/enkanetwork/model/assets.py
--rw-rw-rw-   0        0        0     1935 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.4/enkanetwork/model/base.py
--rw-rw-rw-   0        0        0     1403 2024-02-24 18:46:53.000000 enkanetworkv2.py-2.0.4/enkanetwork/model/build.py
--rw-rw-rw-   0        0        0     5183 2024-02-24 18:47:25.000000 enkanetworkv2.py-2.0.4/enkanetwork/model/character.py
--rw-rw-rw-   0        0        0     5634 2024-02-24 18:35:48.000000 enkanetworkv2.py-2.0.4/enkanetwork/model/equipments.py
--rw-rw-rw-   0        0        0      307 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.4/enkanetwork/model/hoyos.py
--rw-rw-rw-   0        0        0     4063 2024-04-06 17:07:07.000000 enkanetworkv2.py-2.0.4/enkanetwork/model/players.py
--rw-rw-rw-   0        0        0      346 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.4/enkanetwork/model/profile.py
--rw-rw-rw-   0        0        0     7763 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.4/enkanetwork/model/stats.py
--rw-rw-rw-   0        0        0      293 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.4/enkanetwork/model/utils.py
--rw-rw-rw-   0        0        0     1313 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.4/enkanetwork/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-07 21:51:00.763442 enkanetworkv2.py-2.0.4/enkanetwork/types/
--rw-rw-rw-   0        0        0      157 2024-02-24 18:56:57.000000 enkanetworkv2.py-2.0.4/enkanetwork/types/__init__.py
--rw-rw-rw-   0        0        0     1157 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.4/enkanetwork/types/enkanetwork.py
--rw-rw-rw-   0        0        0     3439 2024-04-07 21:50:42.000000 enkanetworkv2.py-2.0.4/enkanetwork/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-07 21:51:00.796890 enkanetworkv2.py-2.0.4/enkanetworkv2.py.egg-info/
--rw-rw-rw-   0        0        0    19341 2024-04-07 21:51:00.000000 enkanetworkv2.py-2.0.4/enkanetworkv2.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1550 2024-04-07 21:51:00.000000 enkanetworkv2.py-2.0.4/enkanetworkv2.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 21:51:00.000000 enkanetworkv2.py-2.0.4/enkanetworkv2.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-04-07 21:51:00.000000 enkanetworkv2.py-2.0.4/enkanetworkv2.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-07 21:51:00.000000 enkanetworkv2.py-2.0.4/enkanetworkv2.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-07 21:51:00.799888 enkanetworkv2.py-2.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1105 2024-04-06 17:09:00.000000 enkanetworkv2.py-2.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 10:00:21.918044 enkanetworkv2.py-2.0.5/
+-rw-rw-rw-   0        0        0     1070 2024-02-24 18:53:52.000000 enkanetworkv2.py-2.0.5/LICENSE
+-rw-rw-rw-   0        0        0       36 2024-02-24 18:58:13.000000 enkanetworkv2.py-2.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0    19341 2024-04-25 10:00:21.918044 enkanetworkv2.py-2.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0    18242 2024-02-24 19:02:02.000000 enkanetworkv2.py-2.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 10:00:21.874043 enkanetworkv2.py-2.0.5/enkanetwork/
+-rw-rw-rw-   0        0        0     1462 2024-04-25 09:57:55.000000 enkanetworkv2.py-2.0.5/enkanetwork/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 10:00:21.857995 enkanetworkv2.py-2.0.5/enkanetwork/assets/
+drwxrwxrwx   0        0        0        0 2024-04-25 10:00:21.882044 enkanetworkv2.py-2.0.5/enkanetwork/assets/data/
+-rw-rw-rw-   0        0        0    54223 2024-04-25 09:53:04.000000 enkanetworkv2.py-2.0.5/enkanetwork/assets/data/artifact_props.json
+-rw-rw-rw-   0        0        0  1095132 2024-04-25 09:53:03.000000 enkanetworkv2.py-2.0.5/enkanetwork/assets/data/artifacts.json
+-rw-rw-rw-   0        0        0    43649 2024-04-25 09:53:04.000000 enkanetworkv2.py-2.0.5/enkanetwork/assets/data/characters.json
+-rw-rw-rw-   0        0        0    52516 2024-04-25 09:53:04.000000 enkanetworkv2.py-2.0.5/enkanetwork/assets/data/constellations.json
+-rw-rw-rw-   0        0        0    12831 2024-04-25 09:53:03.000000 enkanetworkv2.py-2.0.5/enkanetwork/assets/data/costumes.json
+-rw-rw-rw-   0        0        0  1316924 2024-04-25 09:53:04.000000 enkanetworkv2.py-2.0.5/enkanetwork/assets/data/fight_props.json
+-rw-rw-rw-   0        0        0    57396 2024-04-25 09:53:02.000000 enkanetworkv2.py-2.0.5/enkanetwork/assets/data/namecards.json
+-rw-rw-rw-   0        0        0     6321 2024-04-06 16:43:28.000000 enkanetworkv2.py-2.0.5/enkanetwork/assets/data/pfps.json
+-rw-rw-rw-   0        0        0    87635 2024-04-25 09:53:04.000000 enkanetworkv2.py-2.0.5/enkanetwork/assets/data/skills.json
+-rw-rw-rw-   0        0        0    41728 2024-04-25 09:53:02.000000 enkanetworkv2.py-2.0.5/enkanetwork/assets/data/weapons.json
+drwxrwxrwx   0        0        0        0 2024-04-25 10:00:21.891044 enkanetworkv2.py-2.0.5/enkanetwork/assets/langs/
+-rw-rw-rw-   0        0        0   554994 2024-04-25 09:54:12.000000 enkanetworkv2.py-2.0.5/enkanetwork/assets/langs/artifact_sets.json
+-rw-rw-rw-   0        0        0  2431947 2024-04-25 09:54:14.000000 enkanetworkv2.py-2.0.5/enkanetwork/assets/langs/artifacts.json
+-rw-rw-rw-   0        0        0    33337 2024-04-25 09:54:14.000000 enkanetworkv2.py-2.0.5/enkanetwork/assets/langs/characters.json
+-rw-rw-rw-   0        0        0   310851 2024-04-25 09:54:14.000000 enkanetworkv2.py-2.0.5/enkanetwork/assets/langs/constellations.json
+-rw-rw-rw-   0        0        0    30562 2024-02-24 19:12:22.000000 enkanetworkv2.py-2.0.5/enkanetwork/assets/langs/fight_props.json
+-rw-rw-rw-   0        0        0   122404 2024-04-25 09:54:14.000000 enkanetworkv2.py-2.0.5/enkanetwork/assets/langs/namecards.json
+-rw-rw-rw-   0        0        0   309249 2024-04-25 09:54:15.000000 enkanetworkv2.py-2.0.5/enkanetwork/assets/langs/skills.json
+-rw-rw-rw-   0        0        0   113312 2024-04-25 09:54:15.000000 enkanetworkv2.py-2.0.5/enkanetwork/assets/langs/weapons.json
+-rw-rw-rw-   0        0        0     8270 2024-04-06 17:04:36.000000 enkanetworkv2.py-2.0.5/enkanetwork/assets.py
+-rw-rw-rw-   0        0        0      645 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.5/enkanetwork/cache.py
+-rw-rw-rw-   0        0        0    12474 2024-04-07 20:58:35.000000 enkanetworkv2.py-2.0.5/enkanetwork/client.py
+-rw-rw-rw-   0        0        0      798 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.5/enkanetwork/config.py
+-rw-rw-rw-   0        0        0     1099 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.5/enkanetwork/enum.py
+-rw-rw-rw-   0        0        0     1925 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.5/enkanetwork/exception.py
+-rw-rw-rw-   0        0        0     7345 2024-02-24 18:56:30.000000 enkanetworkv2.py-2.0.5/enkanetwork/http.py
+drwxrwxrwx   0        0        0        0 2024-04-25 10:00:21.898044 enkanetworkv2.py-2.0.5/enkanetwork/model/
+-rw-rw-rw-   0        0        0      137 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.5/enkanetwork/model/__init__.py
+-rw-rw-rw-   0        0        0     5029 2024-04-06 17:00:40.000000 enkanetworkv2.py-2.0.5/enkanetwork/model/assets.py
+-rw-rw-rw-   0        0        0     1935 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.5/enkanetwork/model/base.py
+-rw-rw-rw-   0        0        0     1403 2024-02-24 18:46:53.000000 enkanetworkv2.py-2.0.5/enkanetwork/model/build.py
+-rw-rw-rw-   0        0        0     5183 2024-02-24 18:47:25.000000 enkanetworkv2.py-2.0.5/enkanetwork/model/character.py
+-rw-rw-rw-   0        0        0     5634 2024-02-24 18:35:48.000000 enkanetworkv2.py-2.0.5/enkanetwork/model/equipments.py
+-rw-rw-rw-   0        0        0      307 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.5/enkanetwork/model/hoyos.py
+-rw-rw-rw-   0        0        0     4063 2024-04-06 17:07:07.000000 enkanetworkv2.py-2.0.5/enkanetwork/model/players.py
+-rw-rw-rw-   0        0        0      346 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.5/enkanetwork/model/profile.py
+-rw-rw-rw-   0        0        0     7763 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.5/enkanetwork/model/stats.py
+-rw-rw-rw-   0        0        0      293 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.5/enkanetwork/model/utils.py
+-rw-rw-rw-   0        0        0     1313 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.5/enkanetwork/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-25 10:00:21.899044 enkanetworkv2.py-2.0.5/enkanetwork/types/
+-rw-rw-rw-   0        0        0      157 2024-02-24 18:56:57.000000 enkanetworkv2.py-2.0.5/enkanetwork/types/__init__.py
+-rw-rw-rw-   0        0        0     1157 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.5/enkanetwork/types/enkanetwork.py
+-rw-rw-rw-   0        0        0     3445 2024-04-25 09:57:20.000000 enkanetworkv2.py-2.0.5/enkanetwork/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-25 10:00:21.917045 enkanetworkv2.py-2.0.5/enkanetworkv2.py.egg-info/
+-rw-rw-rw-   0        0        0    19341 2024-04-25 10:00:21.000000 enkanetworkv2.py-2.0.5/enkanetworkv2.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1550 2024-04-25 10:00:21.000000 enkanetworkv2.py-2.0.5/enkanetworkv2.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 10:00:21.000000 enkanetworkv2.py-2.0.5/enkanetworkv2.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-04-25 10:00:21.000000 enkanetworkv2.py-2.0.5/enkanetworkv2.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-25 10:00:21.000000 enkanetworkv2.py-2.0.5/enkanetworkv2.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 10:00:21.919043 enkanetworkv2.py-2.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1105 2024-04-06 17:09:00.000000 enkanetworkv2.py-2.0.5/setup.py
```

### Comparing `enkanetworkv2.py-2.0.4/LICENSE` & `enkanetworkv2.py-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.4/PKG-INFO` & `enkanetworkv2.py-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enkanetworkv2.py
-Version: 2.0.4
+Version: 2.0.5
 Summary: Library for fetching JSON data from site https://enka.network/
 Home-page: https://github.com/DEViantUA/EnkaNetworkV2.py
 Author: DeviantUa
 Author-email: deviantapi@gmail.com
 Keywords: enkanetwork.py,enkanetwork,enka.network,genshinapi,enkanetworkV2,enkanetworkV2.py
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `enkanetworkv2.py-2.0.4/README.md` & `enkanetworkv2.py-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.4/enkanetwork/__init__.py` & `enkanetworkv2.py-2.0.5/enkanetwork/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE."""
 
 __title__ = 'enkanetworkV2.py'
 __author__ = 'DeviantUa'
-__version__ = '2.0.4'
+__version__ = '2.0.5'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2024-present DeviantUa'
 
 
 from .client import *
 from .exception import *
 from .model import *
```

### Comparing `enkanetworkv2.py-2.0.4/enkanetwork/assets/data/artifact_props.json` & `enkanetworkv2.py-2.0.5/enkanetwork/assets/data/artifact_props.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985977564102565%*

 * *Differences: {"'101221'": "{'propValue': 1.6}",*

 * * "'201203'": "{'propValue': 1.6}",*

 * * "'301031'": "{'propValue': 2.5}",*

 * * "'301033'": "{'propValue': 3.1}",*

 * * "'301061'": "{'propValue': 2.5}",*

 * * "'301063'": "{'propValue': 3.1}",*

 * * "'947003'": "{'propValue': 5.0}"}*

```diff
@@ -143,15 +143,15 @@
         "propDigit": "PERCENT",
         "propType": "FIGHT_PROP_CRITICAL",
         "propValue": 1.0
     },
     "101221": {
         "propDigit": "PERCENT",
         "propType": "FIGHT_PROP_CRITICAL_HURT",
-        "propValue": 1.5
+        "propValue": 1.6
     },
     "101222": {
         "propDigit": "PERCENT",
         "propType": "FIGHT_PROP_CRITICAL_HURT",
         "propValue": 1.9
     },
     "101231": {
@@ -433,15 +433,15 @@
         "propDigit": "PERCENT",
         "propType": "FIGHT_PROP_CRITICAL",
         "propValue": 1.3
     },
     "201203": {
         "propDigit": "PERCENT",
         "propType": "FIGHT_PROP_CRITICAL",
-        "propValue": 1.5
+        "propValue": 1.6
     },
     "201221": {
         "propDigit": "PERCENT",
         "propType": "FIGHT_PROP_CRITICAL_HURT",
         "propValue": 2.2
     },
     "201222": {
@@ -503,25 +503,25 @@
         "propDigit": "DIGIT",
         "propType": "FIGHT_PROP_HP",
         "propValue": 143
     },
     "301031": {
         "propDigit": "PERCENT",
         "propType": "FIGHT_PROP_HP_PERCENT",
-        "propValue": 2.4
+        "propValue": 2.5
     },
     "301032": {
         "propDigit": "PERCENT",
         "propType": "FIGHT_PROP_HP_PERCENT",
         "propValue": 2.8
     },
     "301033": {
         "propDigit": "PERCENT",
         "propType": "FIGHT_PROP_HP_PERCENT",
-        "propValue": 3.2
+        "propValue": 3.1
     },
     "301034": {
         "propDigit": "PERCENT",
         "propType": "FIGHT_PROP_HP_PERCENT",
         "propValue": 3.5
     },
     "301051": {
@@ -543,25 +543,25 @@
         "propDigit": "DIGIT",
         "propType": "FIGHT_PROP_ATTACK",
         "propValue": 9
     },
     "301061": {
         "propDigit": "PERCENT",
         "propType": "FIGHT_PROP_ATTACK_PERCENT",
-        "propValue": 2.4
+        "propValue": 2.5
     },
     "301062": {
         "propDigit": "PERCENT",
         "propType": "FIGHT_PROP_ATTACK_PERCENT",
         "propValue": 2.8
     },
     "301063": {
         "propDigit": "PERCENT",
         "propType": "FIGHT_PROP_ATTACK_PERCENT",
-        "propValue": 3.2
+        "propValue": 3.1
     },
     "301064": {
         "propDigit": "PERCENT",
         "propType": "FIGHT_PROP_ATTACK_PERCENT",
         "propValue": 3.5
     },
     "301081": {
@@ -1328,15 +1328,15 @@
         "propDigit": "PERCENT",
         "propType": "FIGHT_PROP_ATTACK_PERCENT",
         "propValue": 4.0
     },
     "947003": {
         "propDigit": "PERCENT",
         "propType": "FIGHT_PROP_DEFENSE_PERCENT",
-        "propValue": 4.9
+        "propValue": 5.0
     },
     "947004": {
         "propDigit": "PERCENT",
         "propType": "FIGHT_PROP_CRITICAL",
         "propValue": 2.6
     },
     "947005": {
@@ -1763,15 +1763,15 @@
         "propDigit": "DIGIT",
         "propType": "FIGHT_PROP_ELEMENT_MASTERY",
         "propValue": 300
     },
     "967001": {
         "propDigit": "PERCENT",
         "propType": "FIGHT_PROP_CRITICAL",
-        "propValue": 100.0
+        "propValue": 100
     },
     "968001": {
         "propDigit": "DIGIT",
         "propType": "FIGHT_PROP_ELEMENT_MASTERY",
         "propValue": -300
     },
     "969001": {
@@ -2063,15 +2063,15 @@
         "propDigit": "PERCENT",
         "propType": "FIGHT_PROP_CRITICAL_HURT",
         "propValue": 350.0
     },
     "999002": {
         "propDigit": "PERCENT",
         "propType": "FIGHT_PROP_CRITICAL",
-        "propValue": 100.0
+        "propValue": 100
     },
     "999003": {
         "propDigit": "DIGIT",
         "propType": "FIGHT_PROP_ATTACK",
         "propValue": 233333
     },
     "999004": {
```

### Comparing `enkanetworkv2.py-2.0.4/enkanetwork/assets/data/artifacts.json` & `enkanetworkv2.py-2.0.5/enkanetwork/assets/data/artifacts.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9849699398797596%*

 * *Differences: {"'23721'": "OrderedDict([('nameTextMapHash', 1829870716), ('itemType', 'ITEM_RELIQUARY'), "*

 * *            "('equipType', 'EQUIP_RING'), ('icon', 'UI_RelicIcon_15035_1'), ('rankLevel', 5), "*

 * *            "('mainPropDepotId', 5096), ('appendPropDepotId', 964)])",*

 * * "'23722'": "OrderedDict([('nameTextMapHash', 4114993540), ('itemType', 'ITEM_RELIQUARY'), "*

 * *            "('equipType', 'EQUIP_NECKLACE'), ('icon', 'UI_RelicIcon_15035_2'), ('rankLevel', 5), "*

 * *            "('mainPropDepotId', 2000), ('appendPropDepotId […]*

```diff
@@ -4063,14 +4063,194 @@
         "equipType": "EQUIP_SHOES",
         "icon": "UI_RelicIcon_15034_5",
         "itemType": "ITEM_RELIQUARY",
         "mainPropDepotId": 1099,
         "nameTextMapHash": 206791868,
         "rankLevel": 4
     },
+    "23721": {
+        "appendPropDepotId": 964,
+        "equipType": "EQUIP_RING",
+        "icon": "UI_RelicIcon_15035_1",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 5096,
+        "nameTextMapHash": 1829870716,
+        "rankLevel": 5
+    },
+    "23722": {
+        "appendPropDepotId": 961,
+        "equipType": "EQUIP_NECKLACE",
+        "icon": "UI_RelicIcon_15035_2",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 2000,
+        "nameTextMapHash": 4114993540,
+        "rankLevel": 5
+    },
+    "23723": {
+        "appendPropDepotId": 965,
+        "equipType": "EQUIP_DRESS",
+        "icon": "UI_RelicIcon_15035_3",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 3096,
+        "nameTextMapHash": 3902182396,
+        "rankLevel": 5
+    },
+    "23724": {
+        "appendPropDepotId": 962,
+        "equipType": "EQUIP_BRACER",
+        "icon": "UI_RelicIcon_15035_4",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 4000,
+        "nameTextMapHash": 3666732564,
+        "rankLevel": 5
+    },
+    "23725": {
+        "appendPropDepotId": 963,
+        "equipType": "EQUIP_SHOES",
+        "icon": "UI_RelicIcon_15035_5",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 1099,
+        "nameTextMapHash": 2256184652,
+        "rankLevel": 5
+    },
+    "23726": {
+        "appendPropDepotId": 964,
+        "equipType": "EQUIP_RING",
+        "icon": "UI_RelicIcon_15035_1",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 5095,
+        "nameTextMapHash": 4253652668,
+        "rankLevel": 5
+    },
+    "23727": {
+        "appendPropDepotId": 961,
+        "equipType": "EQUIP_NECKLACE",
+        "icon": "UI_RelicIcon_15035_2",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 2000,
+        "nameTextMapHash": 2638728292,
+        "rankLevel": 4
+    },
+    "23728": {
+        "appendPropDepotId": 965,
+        "equipType": "EQUIP_DRESS",
+        "icon": "UI_RelicIcon_15035_3",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 3093,
+        "nameTextMapHash": 4071524972,
+        "rankLevel": 4
+    },
+    "23729": {
+        "appendPropDepotId": 962,
+        "equipType": "EQUIP_BRACER",
+        "icon": "UI_RelicIcon_15035_4",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 4000,
+        "nameTextMapHash": 2551385844,
+        "rankLevel": 4
+    },
+    "23730": {
+        "appendPropDepotId": 963,
+        "equipType": "EQUIP_SHOES",
+        "icon": "UI_RelicIcon_15035_5",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 1095,
+        "nameTextMapHash": 1827685724,
+        "rankLevel": 4
+    },
+    "23731": {
+        "appendPropDepotId": 964,
+        "equipType": "EQUIP_RING",
+        "icon": "UI_RelicIcon_15036_1",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 5090,
+        "nameTextMapHash": 133613868,
+        "rankLevel": 5
+    },
+    "23732": {
+        "appendPropDepotId": 961,
+        "equipType": "EQUIP_NECKLACE",
+        "icon": "UI_RelicIcon_15036_2",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 2000,
+        "nameTextMapHash": 3675718628,
+        "rankLevel": 5
+    },
+    "23733": {
+        "appendPropDepotId": 965,
+        "equipType": "EQUIP_DRESS",
+        "icon": "UI_RelicIcon_15036_3",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 3096,
+        "nameTextMapHash": 1917296060,
+        "rankLevel": 5
+    },
+    "23734": {
+        "appendPropDepotId": 962,
+        "equipType": "EQUIP_BRACER",
+        "icon": "UI_RelicIcon_15036_4",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 4000,
+        "nameTextMapHash": 257567548,
+        "rankLevel": 5
+    },
+    "23735": {
+        "appendPropDepotId": 963,
+        "equipType": "EQUIP_SHOES",
+        "icon": "UI_RelicIcon_15036_5",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 1099,
+        "nameTextMapHash": 1255108572,
+        "rankLevel": 5
+    },
+    "23736": {
+        "appendPropDepotId": 964,
+        "equipType": "EQUIP_RING",
+        "icon": "UI_RelicIcon_15036_1",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 5096,
+        "nameTextMapHash": 632659124,
+        "rankLevel": 5
+    },
+    "23737": {
+        "appendPropDepotId": 961,
+        "equipType": "EQUIP_NECKLACE",
+        "icon": "UI_RelicIcon_15036_2",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 2000,
+        "nameTextMapHash": 1990912852,
+        "rankLevel": 4
+    },
+    "23738": {
+        "appendPropDepotId": 965,
+        "equipType": "EQUIP_DRESS",
+        "icon": "UI_RelicIcon_15036_3",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 3093,
+        "nameTextMapHash": 4023011412,
+        "rankLevel": 4
+    },
+    "23739": {
+        "appendPropDepotId": 962,
+        "equipType": "EQUIP_BRACER",
+        "icon": "UI_RelicIcon_15036_4",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 4000,
+        "nameTextMapHash": 1584886164,
+        "rankLevel": 4
+    },
+    "23740": {
+        "appendPropDepotId": 963,
+        "equipType": "EQUIP_SHOES",
+        "icon": "UI_RelicIcon_15036_5",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 1095,
+        "nameTextMapHash": 3407812284,
+        "rankLevel": 4
+    },
     "24101": {
         "appendPropDepotId": 964,
         "equipType": "EQUIP_RING",
         "icon": "UI_RelicIcon_15001_1",
         "itemType": "ITEM_RELIQUARY",
         "mainPropDepotId": 5099,
         "nameTextMapHash": 2936766364,
@@ -7753,14 +7933,374 @@
         "equipType": "EQUIP_SHOES",
         "icon": "UI_RelicIcon_15034_5",
         "itemType": "ITEM_RELIQUARY",
         "mainPropDepotId": 1000,
         "nameTextMapHash": 487940916,
         "rankLevel": 5
     },
+    "35412": {
+        "appendPropDepotId": 401,
+        "equipType": "EQUIP_RING",
+        "icon": "UI_RelicIcon_15035_1",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 5000,
+        "nameTextMapHash": 1691105380,
+        "rankLevel": 4
+    },
+    "35413": {
+        "appendPropDepotId": 401,
+        "equipType": "EQUIP_RING",
+        "icon": "UI_RelicIcon_15035_1",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 5000,
+        "nameTextMapHash": 680620692,
+        "rankLevel": 4
+    },
+    "35422": {
+        "appendPropDepotId": 401,
+        "equipType": "EQUIP_NECKLACE",
+        "icon": "UI_RelicIcon_15035_2",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 2000,
+        "nameTextMapHash": 3081478772,
+        "rankLevel": 4
+    },
+    "35423": {
+        "appendPropDepotId": 401,
+        "equipType": "EQUIP_NECKLACE",
+        "icon": "UI_RelicIcon_15035_2",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 2000,
+        "nameTextMapHash": 2117798972,
+        "rankLevel": 4
+    },
+    "35432": {
+        "appendPropDepotId": 401,
+        "equipType": "EQUIP_DRESS",
+        "icon": "UI_RelicIcon_15035_3",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 3000,
+        "nameTextMapHash": 3246653860,
+        "rankLevel": 4
+    },
+    "35433": {
+        "appendPropDepotId": 401,
+        "equipType": "EQUIP_DRESS",
+        "icon": "UI_RelicIcon_15035_3",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 3000,
+        "nameTextMapHash": 3824907452,
+        "rankLevel": 4
+    },
+    "35442": {
+        "appendPropDepotId": 401,
+        "equipType": "EQUIP_BRACER",
+        "icon": "UI_RelicIcon_15035_4",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 4000,
+        "nameTextMapHash": 1809415524,
+        "rankLevel": 4
+    },
+    "35443": {
+        "appendPropDepotId": 401,
+        "equipType": "EQUIP_BRACER",
+        "icon": "UI_RelicIcon_15035_4",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 4000,
+        "nameTextMapHash": 1364940700,
+        "rankLevel": 4
+    },
+    "35452": {
+        "appendPropDepotId": 401,
+        "equipType": "EQUIP_SHOES",
+        "icon": "UI_RelicIcon_15035_5",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 1000,
+        "nameTextMapHash": 3134129324,
+        "rankLevel": 4
+    },
+    "35453": {
+        "appendPropDepotId": 401,
+        "equipType": "EQUIP_SHOES",
+        "icon": "UI_RelicIcon_15035_5",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 1000,
+        "nameTextMapHash": 29786276,
+        "rankLevel": 4
+    },
+    "35513": {
+        "appendPropDepotId": 501,
+        "equipType": "EQUIP_RING",
+        "icon": "UI_RelicIcon_15035_1",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 5000,
+        "nameTextMapHash": 1422096748,
+        "rankLevel": 5
+    },
+    "35514": {
+        "appendPropDepotId": 501,
+        "equipType": "EQUIP_RING",
+        "icon": "UI_RelicIcon_15035_1",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 5000,
+        "nameTextMapHash": 1867205412,
+        "rankLevel": 5
+    },
+    "35523": {
+        "appendPropDepotId": 501,
+        "equipType": "EQUIP_NECKLACE",
+        "icon": "UI_RelicIcon_15035_2",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 2000,
+        "nameTextMapHash": 575540884,
+        "rankLevel": 5
+    },
+    "35524": {
+        "appendPropDepotId": 501,
+        "equipType": "EQUIP_NECKLACE",
+        "icon": "UI_RelicIcon_15035_2",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 2000,
+        "nameTextMapHash": 1854618132,
+        "rankLevel": 5
+    },
+    "35533": {
+        "appendPropDepotId": 501,
+        "equipType": "EQUIP_DRESS",
+        "icon": "UI_RelicIcon_15035_3",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 3000,
+        "nameTextMapHash": 1150905740,
+        "rankLevel": 5
+    },
+    "35534": {
+        "appendPropDepotId": 501,
+        "equipType": "EQUIP_DRESS",
+        "icon": "UI_RelicIcon_15035_3",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 3000,
+        "nameTextMapHash": 2649107356,
+        "rankLevel": 5
+    },
+    "35543": {
+        "appendPropDepotId": 501,
+        "equipType": "EQUIP_BRACER",
+        "icon": "UI_RelicIcon_15035_4",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 4000,
+        "nameTextMapHash": 832863868,
+        "rankLevel": 5
+    },
+    "35544": {
+        "appendPropDepotId": 501,
+        "equipType": "EQUIP_BRACER",
+        "icon": "UI_RelicIcon_15035_4",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 4000,
+        "nameTextMapHash": 2942495796,
+        "rankLevel": 5
+    },
+    "35553": {
+        "appendPropDepotId": 501,
+        "equipType": "EQUIP_SHOES",
+        "icon": "UI_RelicIcon_15035_5",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 1000,
+        "nameTextMapHash": 2919065596,
+        "rankLevel": 5
+    },
+    "35554": {
+        "appendPropDepotId": 501,
+        "equipType": "EQUIP_SHOES",
+        "icon": "UI_RelicIcon_15035_5",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 1000,
+        "nameTextMapHash": 2328442068,
+        "rankLevel": 5
+    },
+    "36412": {
+        "appendPropDepotId": 401,
+        "equipType": "EQUIP_RING",
+        "icon": "UI_RelicIcon_15036_1",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 5000,
+        "nameTextMapHash": 3749124492,
+        "rankLevel": 4
+    },
+    "36413": {
+        "appendPropDepotId": 401,
+        "equipType": "EQUIP_RING",
+        "icon": "UI_RelicIcon_15036_1",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 5000,
+        "nameTextMapHash": 3617555484,
+        "rankLevel": 4
+    },
+    "36422": {
+        "appendPropDepotId": 401,
+        "equipType": "EQUIP_NECKLACE",
+        "icon": "UI_RelicIcon_15036_2",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 2000,
+        "nameTextMapHash": 777741588,
+        "rankLevel": 4
+    },
+    "36423": {
+        "appendPropDepotId": 401,
+        "equipType": "EQUIP_NECKLACE",
+        "icon": "UI_RelicIcon_15036_2",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 2000,
+        "nameTextMapHash": 2712149308,
+        "rankLevel": 4
+    },
+    "36432": {
+        "appendPropDepotId": 401,
+        "equipType": "EQUIP_DRESS",
+        "icon": "UI_RelicIcon_15036_3",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 3000,
+        "nameTextMapHash": 700967596,
+        "rankLevel": 4
+    },
+    "36433": {
+        "appendPropDepotId": 401,
+        "equipType": "EQUIP_DRESS",
+        "icon": "UI_RelicIcon_15036_3",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 3000,
+        "nameTextMapHash": 3480233164,
+        "rankLevel": 4
+    },
+    "36442": {
+        "appendPropDepotId": 401,
+        "equipType": "EQUIP_BRACER",
+        "icon": "UI_RelicIcon_15036_4",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 4000,
+        "nameTextMapHash": 1794117964,
+        "rankLevel": 4
+    },
+    "36443": {
+        "appendPropDepotId": 401,
+        "equipType": "EQUIP_BRACER",
+        "icon": "UI_RelicIcon_15036_4",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 4000,
+        "nameTextMapHash": 1840057148,
+        "rankLevel": 4
+    },
+    "36452": {
+        "appendPropDepotId": 401,
+        "equipType": "EQUIP_SHOES",
+        "icon": "UI_RelicIcon_15036_5",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 1000,
+        "nameTextMapHash": 329286804,
+        "rankLevel": 4
+    },
+    "36453": {
+        "appendPropDepotId": 401,
+        "equipType": "EQUIP_SHOES",
+        "icon": "UI_RelicIcon_15036_5",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 1000,
+        "nameTextMapHash": 2995813268,
+        "rankLevel": 4
+    },
+    "36513": {
+        "appendPropDepotId": 501,
+        "equipType": "EQUIP_RING",
+        "icon": "UI_RelicIcon_15036_1",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 5000,
+        "nameTextMapHash": 3969402636,
+        "rankLevel": 5
+    },
+    "36514": {
+        "appendPropDepotId": 501,
+        "equipType": "EQUIP_RING",
+        "icon": "UI_RelicIcon_15036_1",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 5000,
+        "nameTextMapHash": 1674295492,
+        "rankLevel": 5
+    },
+    "36523": {
+        "appendPropDepotId": 501,
+        "equipType": "EQUIP_NECKLACE",
+        "icon": "UI_RelicIcon_15036_2",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 2000,
+        "nameTextMapHash": 3572708764,
+        "rankLevel": 5
+    },
+    "36524": {
+        "appendPropDepotId": 501,
+        "equipType": "EQUIP_NECKLACE",
+        "icon": "UI_RelicIcon_15036_2",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 2000,
+        "nameTextMapHash": 3777616700,
+        "rankLevel": 5
+    },
+    "36533": {
+        "appendPropDepotId": 501,
+        "equipType": "EQUIP_DRESS",
+        "icon": "UI_RelicIcon_15036_3",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 3000,
+        "nameTextMapHash": 474006692,
+        "rankLevel": 5
+    },
+    "36534": {
+        "appendPropDepotId": 501,
+        "equipType": "EQUIP_DRESS",
+        "icon": "UI_RelicIcon_15036_3",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 3000,
+        "nameTextMapHash": 3941298052,
+        "rankLevel": 5
+    },
+    "36543": {
+        "appendPropDepotId": 501,
+        "equipType": "EQUIP_BRACER",
+        "icon": "UI_RelicIcon_15036_4",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 4000,
+        "nameTextMapHash": 3704215748,
+        "rankLevel": 5
+    },
+    "36544": {
+        "appendPropDepotId": 501,
+        "equipType": "EQUIP_BRACER",
+        "icon": "UI_RelicIcon_15036_4",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 4000,
+        "nameTextMapHash": 814298500,
+        "rankLevel": 5
+    },
+    "36553": {
+        "appendPropDepotId": 501,
+        "equipType": "EQUIP_SHOES",
+        "icon": "UI_RelicIcon_15036_5",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 1000,
+        "nameTextMapHash": 1896095676,
+        "rankLevel": 5
+    },
+    "36554": {
+        "appendPropDepotId": 501,
+        "equipType": "EQUIP_SHOES",
+        "icon": "UI_RelicIcon_15036_5",
+        "itemType": "ITEM_RELIQUARY",
+        "mainPropDepotId": 1000,
+        "nameTextMapHash": 1056891388,
+        "rankLevel": 5
+    },
     "51110": {
         "appendPropDepotId": 101,
         "equipType": "EQUIP_RING",
         "icon": "UI_RelicIcon_10001_1",
         "itemType": "ITEM_RELIQUARY",
         "mainPropDepotId": 5000,
         "nameTextMapHash": 3492048612,
```

### Comparing `enkanetworkv2.py-2.0.4/enkanetwork/assets/data/characters.json` & `enkanetworkv2.py-2.0.5/enkanetwork/assets/data/characters.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9891304347826086%*

 * *Differences: {"'10000096'": "OrderedDict([('nameTextMapHash', 167199474), ('iconName', "*

 * *               "'UI_AvatarIcon_Arlecchino'), ('sideIconName', 'UI_AvatarIcon_Side_Arlecchino'), "*

 * *               "('qualityType', 'QUALITY_ORANGE'), ('costElemType', 'Fire'), ('skills', [10961, "*

 * *               "10962, 10965]), ('talents', [961, 962, 963, 964, 965, 966])])"}*

```diff
@@ -1814,9 +1814,29 @@
             941,
             942,
             943,
             944,
             945,
             946
         ]
+    },
+    "10000096": {
+        "costElemType": "Fire",
+        "iconName": "UI_AvatarIcon_Arlecchino",
+        "nameTextMapHash": 167199474,
+        "qualityType": "QUALITY_ORANGE",
+        "sideIconName": "UI_AvatarIcon_Side_Arlecchino",
+        "skills": [
+            10961,
+            10962,
+            10965
+        ],
+        "talents": [
+            961,
+            962,
+            963,
+            964,
+            965,
+            966
+        ]
     }
 }
```

### Comparing `enkanetworkv2.py-2.0.4/enkanetwork/assets/data/constellations.json` & `enkanetworkv2.py-2.0.5/enkanetwork/assets/data/constellations.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9882352941176471%*

 * *Differences: {"'961'": "OrderedDict([('nameTextMapHash', 1931573609), ('icon', 'UI_Talent_S_Arlecchino_01')])",*

 * * "'962'": "OrderedDict([('nameTextMapHash', 2743280569), ('icon', 'UI_Talent_S_Arlecchino_02')])",*

 * * "'963'": "OrderedDict([('nameTextMapHash', 1222541609), ('icon', 'UI_Talent_U_Arlecchino_01')])",*

 * * "'964'": "OrderedDict([('nameTextMapHash', 2103473001), ('icon', 'UI_Talent_S_Arlecchino_03')])",*

 * * "'965'": "OrderedDict([('nameTextMapHash', 3475324945), ('icon', 'UI_Talent_U_Arlecchino_02')])",*

 * * "'966'": "Ordere […]*

```diff
@@ -2010,9 +2010,33 @@
     "95": {
         "icon": "UI_Talent_U_PlayerRock_01",
         "nameTextMapHash": 4177873769
     },
     "96": {
         "icon": "UI_Talent_S_PlayerRock_04",
         "nameTextMapHash": 4065853553
+    },
+    "961": {
+        "icon": "UI_Talent_S_Arlecchino_01",
+        "nameTextMapHash": 1931573609
+    },
+    "962": {
+        "icon": "UI_Talent_S_Arlecchino_02",
+        "nameTextMapHash": 2743280569
+    },
+    "963": {
+        "icon": "UI_Talent_U_Arlecchino_01",
+        "nameTextMapHash": 1222541609
+    },
+    "964": {
+        "icon": "UI_Talent_S_Arlecchino_03",
+        "nameTextMapHash": 2103473001
+    },
+    "965": {
+        "icon": "UI_Talent_U_Arlecchino_02",
+        "nameTextMapHash": 3475324945
+    },
+    "966": {
+        "icon": "UI_Talent_S_Arlecchino_04",
+        "nameTextMapHash": 585561937
     }
 }
```

### Comparing `enkanetworkv2.py-2.0.4/enkanetwork/assets/data/costumes.json` & `enkanetworkv2.py-2.0.5/enkanetwork/assets/data/costumes.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.98989898989899%*

 * *Differences: {"'209600'": "OrderedDict([('iconName', ''), ('sideIconName', ''), ('nameTextMapHash', "*

 * *             '2341898930)])'}*

```diff
@@ -484,9 +484,14 @@
         "nameTextMapHash": 2283589170,
         "sideIconName": ""
     },
     "209400": {
         "iconName": "",
         "nameTextMapHash": 4268512138,
         "sideIconName": ""
+    },
+    "209600": {
+        "iconName": "",
+        "nameTextMapHash": 2341898930,
+        "sideIconName": ""
     }
 }
```

### Comparing `enkanetworkv2.py-2.0.4/enkanetwork/assets/data/fight_props.json` & `enkanetworkv2.py-2.0.5/enkanetwork/assets/data/fight_props.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9318556048131729%*

 * *Differences: {"'CONTROL_TO_AVATAR_TRIGGER_SKILL_KEY2'": "OrderedDict([('nameTextMapHash', 1972892841)])",*

 * * "'CUTSCENE_Arlecchino_DESC'": "OrderedDict([('nameTextMapHash', 1137779934)])",*

 * * "'CUTSCENE_Arlecchino_LABEL_01'": "OrderedDict([('nameTextMapHash', 1431364199)])",*

 * * "'CUTSCENE_Arlecchino_SUBTITLE_01'": "OrderedDict([('nameTextMapHash', 3067010108)])",*

 * * "'CUTSCENE_Arlecchino_SUBTITLE_02'": "OrderedDict([('nameTextMapHash', 890887692)])",*

 * * "'CUTSCENE_Arlecchino_TITLE'": "OrderedDict([('nameTextMapHash', 3880368046)] […]*

```diff
@@ -427,14 +427,17 @@
     },
     "CONTROL_TO_AVATAR_TRIGGER_SKILL": {
         "nameTextMapHash": 2832871221
     },
     "CONTROL_TO_AVATAR_TRIGGER_SKILL_KEY": {
         "nameTextMapHash": 951641977
     },
+    "CONTROL_TO_AVATAR_TRIGGER_SKILL_KEY2": {
+        "nameTextMapHash": 1972892841
+    },
     "CONTROL_TRACK_QUEST": {
         "nameTextMapHash": 4273100090
     },
     "CONTROL_VIEW": {
         "nameTextMapHash": 1314821797
     },
     "CONTROL_WIDGET_QUICK_SWITCH": {
@@ -775,14 +778,29 @@
     },
     "CUTSCENE_AMURTA_SUBTITLE_02": {
         "nameTextMapHash": 2080667100
     },
     "CUTSCENE_AMURTA_TITLE": {
         "nameTextMapHash": 1034909079
     },
+    "CUTSCENE_Arlecchino_DESC": {
+        "nameTextMapHash": 1137779934
+    },
+    "CUTSCENE_Arlecchino_LABEL_01": {
+        "nameTextMapHash": 1431364199
+    },
+    "CUTSCENE_Arlecchino_SUBTITLE_01": {
+        "nameTextMapHash": 3067010108
+    },
+    "CUTSCENE_Arlecchino_SUBTITLE_02": {
+        "nameTextMapHash": 890887692
+    },
+    "CUTSCENE_Arlecchino_TITLE": {
+        "nameTextMapHash": 3880368046
+    },
     "CUTSCENE_BALLADEER_DESC": {
         "nameTextMapHash": 1632147722
     },
     "CUTSCENE_BALLADEER_LABEL_01": {
         "nameTextMapHash": 2196839731
     },
     "CUTSCENE_BALLADEER_SUBTITLE_01": {
@@ -3604,17 +3622,23 @@
     },
     "INVESTIGATION_CURRENT_TARGET_FINISHED": {
         "nameTextMapHash": 758686523
     },
     "INVESTIGATION_ELITE_MONSTER": {
         "nameTextMapHash": 1565613092
     },
+    "INVESTIGATION_JUMP_SCENE": {
+        "nameTextMapHash": 3060428773
+    },
     "INVESTIGATION_NOT_DISCOVER": {
         "nameTextMapHash": 3041090276
     },
+    "INVESTIGATION_REST_MAP_LOCKED": {
+        "nameTextMapHash": 1904453897
+    },
     "ITEM_AVATAR": {
         "nameTextMapHash": 2023598722
     },
     "ITEM_CITY_REPUTATION": {
         "nameTextMapHash": 311147040
     },
     "ITEM_CONSUME": {
@@ -3925,14 +3949,17 @@
     },
     "LEVEL_CYG_DAOBAODONG": {
         "nameTextMapHash": 2892208424
     },
     "LEVEL_CYG_XIANBEISHAN": {
         "nameTextMapHash": 3425661936
     },
+    "LEVEL_REMUSARENA_BUFF": {
+        "nameTextMapHash": 1049143135
+    },
     "LEVEL_Seal_Comehome": {
         "nameTextMapHash": 1207867181
     },
     "LEVEL_Waterwayship_refresh": {
         "nameTextMapHash": 1148486019
     },
     "LEVEL_YDG_Followme": {
@@ -4054,14 +4081,17 @@
     },
     "NO_TASK_ONGOING_TIPS_UP": {
         "nameTextMapHash": 2787758591
     },
     "NPC_EXPNAME_1072": {
         "nameTextMapHash": 2265986372
     },
+    "NPC_EXPNAME_1085": {
+        "nameTextMapHash": 2626237420
+    },
     "NPC_EXPNAME_12530": {
         "nameTextMapHash": 3776981284
     },
     "NPC_EXPNAME_12589": {
         "nameTextMapHash": 3995966164
     },
     "NPC_EXPNAME_12589_1": {
@@ -4588,23 +4618,101 @@
     },
     "NPC_EXPNAME_21307_1": {
         "nameTextMapHash": 998349382
     },
     "NPC_EXPNAME_21307_2": {
         "nameTextMapHash": 288134286
     },
+    "NPC_EXPNAME_21338": {
+        "nameTextMapHash": 812721180
+    },
+    "NPC_EXPNAME_21338_1": {
+        "nameTextMapHash": 266985805
+    },
+    "NPC_EXPNAME_21355": {
+        "nameTextMapHash": 2314549444
+    },
+    "NPC_EXPNAME_21394": {
+        "nameTextMapHash": 1657562724
+    },
+    "NPC_EXPNAME_21398": {
+        "nameTextMapHash": 742844236
+    },
+    "NPC_EXPNAME_21399": {
+        "nameTextMapHash": 1705323268
+    },
+    "NPC_EXPNAME_21400": {
+        "nameTextMapHash": 4039321604
+    },
+    "NPC_EXPNAME_21401": {
+        "nameTextMapHash": 2035427884
+    },
+    "NPC_EXPNAME_21402": {
+        "nameTextMapHash": 1436289668
+    },
+    "NPC_EXPNAME_21403": {
+        "nameTextMapHash": 2560530388
+    },
+    "NPC_EXPNAME_21404": {
+        "nameTextMapHash": 4232986068
+    },
+    "NPC_EXPNAME_21419": {
+        "nameTextMapHash": 1543986668
+    },
+    "NPC_EXPNAME_21420": {
+        "nameTextMapHash": 262205236
+    },
+    "NPC_EXPNAME_21421": {
+        "nameTextMapHash": 4001550332
+    },
+    "NPC_EXPNAME_21422": {
+        "nameTextMapHash": 2552119004
+    },
+    "NPC_EXPNAME_21423": {
+        "nameTextMapHash": 130515524
+    },
+    "NPC_EXPNAME_21424": {
+        "nameTextMapHash": 358535340
+    },
+    "NPC_EXPNAME_21425": {
+        "nameTextMapHash": 2025038156
+    },
+    "NPC_EXPNAME_21426": {
+        "nameTextMapHash": 3311911468
+    },
+    "NPC_EXPNAME_21431": {
+        "nameTextMapHash": 4107064540
+    },
+    "NPC_EXPNAME_21432": {
+        "nameTextMapHash": 974747412
+    },
+    "NPC_EXPNAME_21435": {
+        "nameTextMapHash": 341816916
+    },
+    "NPC_EXPNAME_21482": {
+        "nameTextMapHash": 1759017852
+    },
+    "NPC_EXPNAME_21483": {
+        "nameTextMapHash": 1288854716
+    },
+    "NPC_EXPNAME_21484": {
+        "nameTextMapHash": 3426936708
+    },
     "NPC_EXPNAME_30226": {
         "nameTextMapHash": 355090748
     },
     "NPC_EXPNAME_30320": {
         "nameTextMapHash": 44642924
     },
     "NPC_EXPNAME_30322": {
         "nameTextMapHash": 81065996
     },
+    "NPC_EXPNAME_30322_1": {
+        "nameTextMapHash": 523058794
+    },
     "NPC_EXPNAME_30404": {
         "nameTextMapHash": 2766396404
     },
     "NPC_EXPNAME_30407": {
         "nameTextMapHash": 4260062612
     },
     "NPC_EXPNAME_30416": {
@@ -4672,14 +4780,23 @@
     },
     "NPC_EXPNAME_5290": {
         "nameTextMapHash": 3871071212
     },
     "NPC_EXPNAME_5291": {
         "nameTextMapHash": 3917546724
     },
+    "NPC_EXPNAME_5300": {
+        "nameTextMapHash": 3999987660
+    },
+    "NPC_EXPNAME_5300_1": {
+        "nameTextMapHash": 2346538906
+    },
+    "NPC_EXPNAME_5300_2": {
+        "nameTextMapHash": 1665209882
+    },
     "NPC_EXPNAME_5301": {
         "nameTextMapHash": 17843708
     },
     "NPC_EXPNAME_5311": {
         "nameTextMapHash": 2428877732
     },
     "NPC_NAME_Empty": {
@@ -5464,23 +5581,35 @@
     },
     "NPC_TITLE_13980": {
         "nameTextMapHash": 3452341617
     },
     "NPC_TITLE_13981": {
         "nameTextMapHash": 4033678769
     },
+    "NPC_TITLE_13993": {
+        "nameTextMapHash": 893896489
+    },
     "NPC_TITLE_14016": {
         "nameTextMapHash": 3615369441
     },
     "NPC_TITLE_14028": {
         "nameTextMapHash": 569623201
     },
     "NPC_TITLE_1405_TEST": {
         "nameTextMapHash": 1431829271
     },
+    "NPC_TITLE_14065": {
+        "nameTextMapHash": 1672189353
+    },
+    "NPC_TITLE_14066": {
+        "nameTextMapHash": 312527593
+    },
+    "NPC_TITLE_14067": {
+        "nameTextMapHash": 560802865
+    },
     "NPC_TITLE_1409": {
         "nameTextMapHash": 1519934793
     },
     "NPC_TITLE_140901": {
         "nameTextMapHash": 4077459193
     },
     "NPC_TITLE_1411": {
@@ -6397,14 +6526,23 @@
     },
     "NPC_TITLE_21293": {
         "nameTextMapHash": 2761873609
     },
     "NPC_TITLE_21293_1": {
         "nameTextMapHash": 1828379830
     },
+    "NPC_TITLE_21338": {
+        "nameTextMapHash": 2042919849
+    },
+    "NPC_TITLE_21338_1": {
+        "nameTextMapHash": 3317781269
+    },
+    "NPC_TITLE_21338_2": {
+        "nameTextMapHash": 190664901
+    },
     "NPC_TITLE_2134": {
         "nameTextMapHash": 3618571273
     },
     "NPC_TITLE_2138": {
         "nameTextMapHash": 2522584393
     },
     "NPC_TITLE_2139": {
@@ -6424,14 +6562,17 @@
     },
     "NPC_TITLE_214201": {
         "nameTextMapHash": 4216827521
     },
     "NPC_TITLE_2143": {
         "nameTextMapHash": 3459602641
     },
+    "NPC_TITLE_21430": {
+        "nameTextMapHash": 2506606073
+    },
     "NPC_TITLE_214301": {
         "nameTextMapHash": 2596527449
     },
     "NPC_TITLE_2145": {
         "nameTextMapHash": 1575968745
     },
     "NPC_TITLE_2146": {
@@ -7201,14 +7342,17 @@
     },
     "NPC_TITLE_30539": {
         "nameTextMapHash": 611722297
     },
     "NPC_TITLE_3054": {
         "nameTextMapHash": 3390889657
     },
+    "NPC_TITLE_30544": {
+        "nameTextMapHash": 1110428881
+    },
     "NPC_TITLE_3056": {
         "nameTextMapHash": 3790168681
     },
     "NPC_TITLE_3057": {
         "nameTextMapHash": 532830657
     },
     "NPC_TITLE_3058": {
@@ -7441,14 +7585,17 @@
     },
     "NPC_TITLE_3172": {
         "nameTextMapHash": 516524153
     },
     "NPC_TITLE_3173": {
         "nameTextMapHash": 1354552625
     },
+    "NPC_TITLE_3173_1": {
+        "nameTextMapHash": 786047889
+    },
     "NPC_TITLE_3175": {
         "nameTextMapHash": 4119833249
     },
     "NPC_TITLE_3176": {
         "nameTextMapHash": 2609701529
     },
     "NPC_TITLE_3177": {
@@ -8221,14 +8368,41 @@
     },
     "NPC_TITLE_4429": {
         "nameTextMapHash": 3136026577
     },
     "NPC_TITLE_4430": {
         "nameTextMapHash": 3753014033
     },
+    "NPC_TITLE_4465": {
+        "nameTextMapHash": 3921305465
+    },
+    "NPC_TITLE_4467": {
+        "nameTextMapHash": 1751351761
+    },
+    "NPC_TITLE_4470": {
+        "nameTextMapHash": 71476345
+    },
+    "NPC_TITLE_4472": {
+        "nameTextMapHash": 4133925265
+    },
+    "NPC_TITLE_4473": {
+        "nameTextMapHash": 2526655465
+    },
+    "NPC_TITLE_4474": {
+        "nameTextMapHash": 2035077257
+    },
+    "NPC_TITLE_4475": {
+        "nameTextMapHash": 468554513
+    },
+    "NPC_TITLE_4476": {
+        "nameTextMapHash": 2222718689
+    },
+    "NPC_TITLE_4477": {
+        "nameTextMapHash": 2116807097
+    },
     "NPC_TITLE_5001": {
         "nameTextMapHash": 1689404409
     },
     "NPC_TITLE_5002": {
         "nameTextMapHash": 2479238681
     },
     "NPC_TITLE_5003": {
@@ -8614,14 +8788,32 @@
     },
     "NPC_TITLE_5285": {
         "nameTextMapHash": 2663806745
     },
     "NPC_TITLE_5286": {
         "nameTextMapHash": 3451487537
     },
+    "NPC_TITLE_5344": {
+        "nameTextMapHash": 3810916569
+    },
+    "NPC_TITLE_5345": {
+        "nameTextMapHash": 1901685273
+    },
+    "NPC_TITLE_5346": {
+        "nameTextMapHash": 4029169033
+    },
+    "NPC_TITLE_5352": {
+        "nameTextMapHash": 2131859665
+    },
+    "NPC_TITLE_5353": {
+        "nameTextMapHash": 2776489841
+    },
+    "NPC_TITLE_5354": {
+        "nameTextMapHash": 1127394609
+    },
     "NPC_TITLE_WAGNER_DAY": {
         "nameTextMapHash": 2579169492
     },
     "NPC_TITLE_WAGNER_NIGHT": {
         "nameTextMapHash": 2633631620
     },
     "None": {
@@ -8956,32 +9148,38 @@
     },
     "PENUMBRA_SWITCH_MESSAGE": {
         "nameTextMapHash": 75961651
     },
     "PERSONAL_LINE_ACTIVITY_OPEN_MONA": {
         "nameTextMapHash": 3906161786
     },
+    "PERSONAL_LINE_ARLECCHINO": {
+        "nameTextMapHash": 573476439
+    },
+    "PERSONAL_LINE_ARLECCHINO_LINE_START": {
+        "nameTextMapHash": 2444161054
+    },
     "PERSONAL_LINE_AYAKA": {
         "nameTextMapHash": 2778483999
     },
     "PERSONAL_LINE_AYAKA_LINE_START": {
         "nameTextMapHash": 1264643668
     },
-    "PERSONAL_LINE_CHIORI": {
-        "nameTextMapHash": 728395351
-    },
-    "PERSONAL_LINE_CHIORI_LINE_START": {
-        "nameTextMapHash": 52878078
-    },
     "PERSONAL_LINE_COMPLAINMENT": {
         "nameTextMapHash": 1029528935
     },
     "PERSONAL_LINE_COMPLAINMENT_TITLE": {
         "nameTextMapHash": 1904417612
     },
+    "PERSONAL_LINE_CYNO": {
+        "nameTextMapHash": 1415789359
+    },
+    "PERSONAL_LINE_CYNO_LINE_START": {
+        "nameTextMapHash": 2767624292
+    },
     "PERSONAL_LINE_EMPTY": {
         "nameTextMapHash": 176741455
     },
     "PERSONAL_LINE_EULA": {
         "nameTextMapHash": 1881592783
     },
     "PERSONAL_LINE_EULA_LINE_START": {
@@ -9946,14 +10144,17 @@
     },
     "QUEST_DIALOG_DETAIL_NPC_IS_BUSY": {
         "nameTextMapHash": 2900849852
     },
     "QUEST_DIALOG_DETAIL_NPC_IS_BUSY_WITH_QUEST": {
         "nameTextMapHash": 3354273527
     },
+    "QUEST_DIALOG_DETAIL_NPC_OCCUPIED": {
+        "nameTextMapHash": 1299490581
+    },
     "QUEST_DIALOG_DETAIL_PLACE_OCCUPIED": {
         "nameTextMapHash": 2160139607
     },
     "QUEST_DIALOG_DETAIL_PLACE_OCCUPIED_DETAIL": {
         "nameTextMapHash": 948508387
     },
     "QUEST_DIALOG_DETAIL_PLAYERLEVEL_NEED": {
@@ -11179,14 +11380,41 @@
     },
     "QUEST_Message_Q7405002": {
         "nameTextMapHash": 2507306824
     },
     "QUEST_Message_Q7405802": {
         "nameTextMapHash": 2060369936
     },
+    "QUEST_Message_Q7418306": {
+        "nameTextMapHash": 253592216
+    },
+    "QUEST_Message_Q7418403": {
+        "nameTextMapHash": 2144315400
+    },
+    "QUEST_Message_Q7418407": {
+        "nameTextMapHash": 2613659424
+    },
+    "QUEST_Message_Q7419412": {
+        "nameTextMapHash": 1571075616
+    },
+    "QUEST_Message_Q7419413": {
+        "nameTextMapHash": 1611954816
+    },
+    "QUEST_Message_Q7420205": {
+        "nameTextMapHash": 2555981208
+    },
+    "QUEST_Message_Q7420605": {
+        "nameTextMapHash": 452301984
+    },
+    "QUEST_Message_Q7420607": {
+        "nameTextMapHash": 1737352632
+    },
+    "QUEST_Message_Q7420609": {
+        "nameTextMapHash": 4292795000
+    },
     "QUEST_Message_Q7900403": {
         "nameTextMapHash": 1129099176
     },
     "QUEST_Message_Q7900404": {
         "nameTextMapHash": 1327810824
     },
     "QUEST_Message_Q7900504": {
@@ -11419,14 +11647,17 @@
     },
     "QUEST_UI_NOTSTARTED_TIPS03": {
         "nameTextMapHash": 648701071
     },
     "QUEST_UNSTART_NPC_CONFLICT": {
         "nameTextMapHash": 314137808
     },
+    "QUEST_UNSTART_PLACE_CONFLICT": {
+        "nameTextMapHash": 2252633983
+    },
     "QUEST_UNSTART_PLAYER_LEVEL_NEED": {
         "nameTextMapHash": 1214953529
     },
     "Quest_Black_Q1401708": {
         "nameTextMapHash": 1709444158
     },
     "Quest_Black_Q1401709": {
@@ -11467,14 +11698,47 @@
     },
     "Quest_Black_Q7323301": {
         "nameTextMapHash": 3644724822
     },
     "Quest_Black_Q7365001": {
         "nameTextMapHash": 4025136454
     },
+    "Quest_Black_Q7419101": {
+        "nameTextMapHash": 1322613246
+    },
+    "Quest_Black_Q7419102": {
+        "nameTextMapHash": 3363564822
+    },
+    "Quest_Black_Q7419602": {
+        "nameTextMapHash": 3622705942
+    },
+    "Quest_Black_Q7419604": {
+        "nameTextMapHash": 879566222
+    },
+    "Quest_Black_Q7419609": {
+        "nameTextMapHash": 2786809998
+    },
+    "Quest_Black_Q7419610": {
+        "nameTextMapHash": 2504613654
+    },
+    "Quest_Black_Q7419612": {
+        "nameTextMapHash": 408588054
+    },
+    "Quest_Black_Q7419615": {
+        "nameTextMapHash": 1333545806
+    },
+    "Quest_Black_Q7419619": {
+        "nameTextMapHash": 4237042814
+    },
+    "Quest_Black_Q7419620": {
+        "nameTextMapHash": 1094114118
+    },
+    "Quest_Black_Q7421604": {
+        "nameTextMapHash": 818671342
+    },
     "Quest_Black_Q7902207": {
         "nameTextMapHash": 291547870
     },
     "Quest_Black_Q7902208": {
         "nameTextMapHash": 2900074638
     },
     "Quest_Black_Q7902209": {
@@ -12277,14 +12541,20 @@
     },
     "RET_PERSONAL_LINE_PRE_QUEST_NOT_FINISH": {
         "nameTextMapHash": 2200920392
     },
     "REWARD_ITEM_GOT_TIP": {
         "nameTextMapHash": 3284409760
     },
+    "RemusCat_Interaction_Level": {
+        "nameTextMapHash": 2416172919
+    },
+    "RemusCat_Interaction_LevelShow": {
+        "nameTextMapHash": 2696226031
+    },
     "RetAccountFreeze": {
         "nameTextMapHash": 2463305349
     },
     "RetAccountNotExist": {
         "nameTextMapHash": 1417413629
     },
     "RetAccountVeirfyError": {
@@ -12295,17 +12565,14 @@
     },
     "RetActivityContentClosed": {
         "nameTextMapHash": 3572402933
     },
     "RetActivityFriendHaveGiftLimit": {
         "nameTextMapHash": 168194605
     },
-    "RetAlchemySimCropExceedLimit": {
-        "nameTextMapHash": 589832955
-    },
     "RetAlchemySimInvalidRoundState": {
         "nameTextMapHash": 3547912525
     },
     "RetAllBonfireExceedMaxCount": {
         "nameTextMapHash": 1107085557
     },
     "RetAllTargetSatiationFull": {
@@ -12409,14 +12676,17 @@
     },
     "RetBackupTeamIdNotValid": {
         "nameTextMapHash": 3384539253
     },
     "RetBackupTeamIsCurTeam": {
         "nameTextMapHash": 3606279877
     },
+    "RetBanOpearateFocus": {
+        "nameTextMapHash": 1738230013
+    },
     "RetBattlePassProductExpired": {
         "nameTextMapHash": 1674927501
     },
     "RetBigTalentPointNotEnough": {
         "nameTextMapHash": 1615464853
     },
     "RetBirthdayCannotBeSetTwice": {
@@ -12760,14 +13030,17 @@
     },
     "RetDungeonReviveFail": {
         "nameTextMapHash": 956560461
     },
     "RetDuplicateAvatar": {
         "nameTextMapHash": 2595365269
     },
+    "RetEffigyChallengeV5InCombat": {
+        "nameTextMapHash": 1606334965
+    },
     "RetEnterOtherWorldNotEnough": {
         "nameTextMapHash": 2986878029
     },
     "RetEnterSceneFail": {
         "nameTextMapHash": 902161917
     },
     "RetEnterSceneTokenInvalid": {
@@ -13117,14 +13390,17 @@
     },
     "RetGoodsNotExist": {
         "nameTextMapHash": 1957145045
     },
     "RetGoodsNotInTime": {
         "nameTextMapHash": 1920657541
     },
+    "RetGoodsPreconditionNotSatisfied": {
+        "nameTextMapHash": 3989145277
+    },
     "RetGotAllOneoffGahter": {
         "nameTextMapHash": 728737597
     },
     "RetHachiDungeonStageNotOpen": {
         "nameTextMapHash": 1285466405
     },
     "RetHachiDungeonTeammateNotPass": {
@@ -13339,14 +13615,17 @@
     },
     "RetInvalidWidgetMaterialId": {
         "nameTextMapHash": 514737429
     },
     "RetIsInDungeon": {
         "nameTextMapHash": 959681525
     },
+    "RetIsInLockAvatar": {
+        "nameTextMapHash": 2400672317
+    },
     "RetIsInLockAvatarQuest": {
         "nameTextMapHash": 831879869
     },
     "RetIsNotInStandby": {
         "nameTextMapHash": 235747205
     },
     "RetIsUsingTrialAvatar": {
@@ -13678,14 +13957,17 @@
     },
     "RetNotFoundConfig": {
         "nameTextMapHash": 36342437
     },
     "RetNotFriend": {
         "nameTextMapHash": 686213653
     },
+    "RetNotInPlayerScene": {
+        "nameTextMapHash": 1654075309
+    },
     "RetNotInPlayerWorld": {
         "nameTextMapHash": 3483694149
     },
     "RetNotInSelfScene": {
         "nameTextMapHash": 882133133
     },
     "RetNotInWorldScene": {
@@ -13729,14 +14011,20 @@
     },
     "RetOpenStateNotOpen": {
         "nameTextMapHash": 3782842317
     },
     "RetPackExceedMaxWeight": {
         "nameTextMapHash": 460706373
     },
+    "RetParentQuestCannotStartFocus": {
+        "nameTextMapHash": 2907201181
+    },
+    "RetParentQuestNotExist": {
+        "nameTextMapHash": 3665930173
+    },
     "RetPlantFlowerFriendHaveFlowerLimit": {
         "nameTextMapHash": 3366853189
     },
     "RetPlayerAlreadyIsFriend": {
         "nameTextMapHash": 3123092573
     },
     "RetPlayerBlacklistFull": {
@@ -13756,14 +14044,17 @@
     },
     "RetPlayerNotInBlacklist": {
         "nameTextMapHash": 464044653
     },
     "RetPlayerNotOnline": {
         "nameTextMapHash": 289413917
     },
+    "RetPlayerTimeLocked": {
+        "nameTextMapHash": 940524909
+    },
     "RetPointAlreayUnlocked": {
         "nameTextMapHash": 1897590317
     },
     "RetPointNotUnlocked": {
         "nameTextMapHash": 1341768941
     },
     "RetPointTooFar": {
@@ -13804,20 +14095,38 @@
     },
     "RetPushTipsNotFound": {
         "nameTextMapHash": 3219729677
     },
     "RetQuestContentError": {
         "nameTextMapHash": 3484445741
     },
+    "RetQuestFocusAnyGalleryStarted": {
+        "nameTextMapHash": 4134912245
+    },
+    "RetQuestFocusModeInCd": {
+        "nameTextMapHash": 4245849469
+    },
+    "RetQuestFocusOpenstateOff": {
+        "nameTextMapHash": 1682461
+    },
+    "RetQuestFocusUsingInformalAvatar": {
+        "nameTextMapHash": 2796421733
+    },
+    "RetQuestInFocusMode": {
+        "nameTextMapHash": 2262317429
+    },
     "RetQuestIsFail": {
         "nameTextMapHash": 4148812549
     },
     "RetQuestNotExist": {
         "nameTextMapHash": 476363653
     },
+    "RetQuestNotInFocusMode": {
+        "nameTextMapHash": 3563458293
+    },
     "RetQuestOccupiedNotAvailable": {
         "nameTextMapHash": 351555157
     },
     "RetQuickHitTreeEmptyTrees": {
         "nameTextMapHash": 3555430845
     },
     "RetRecipeLocked": {
@@ -14230,14 +14539,17 @@
     },
     "RetVintageStoreAttrTooLarge": {
         "nameTextMapHash": 427360637
     },
     "RetWaitOtherLogin": {
         "nameTextMapHash": 3858232069
     },
+    "RetWeatherIsLocked": {
+        "nameTextMapHash": 2331469557
+    },
     "RetWidgetAlreadyWithinNearbyRadius": {
         "nameTextMapHash": 849427421
     },
     "RetWidgetAnchorPointFull": {
         "nameTextMapHash": 3389364565
     },
     "RetWidgetAnchorPointNotFound": {
@@ -15199,1163 +15511,14 @@
     },
     "UI_ACTIVITY_ADVERTISEMENT_GO_TO_MISSON_BUTTON": {
         "nameTextMapHash": 3231116544
     },
     "UI_ACTIVITY_ADVERTISEMENT_INVESTIGATE_BUTTON": {
         "nameTextMapHash": 3510170761
     },
-    "UI_ACTIVITY_ALCHEMYSIM_ALCHEMY": {
-        "nameTextMapHash": 3134607896
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_ALCHEMY_NO_LIMIT": {
-        "nameTextMapHash": 3819496261
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_BAG": {
-        "nameTextMapHash": 2439381488
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_BAG_CROP_INFO": {
-        "nameTextMapHash": 349790828
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_BAG_FILTER": {
-        "nameTextMapHash": 3791057152
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_BAG_FILTER_ALL": {
-        "nameTextMapHash": 3377620651
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_BAG_NO_ITEM": {
-        "nameTextMapHash": 1205441471
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_BAG_POTION_INFO": {
-        "nameTextMapHash": 1943522205
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_BAG_UPGRADE_INFO": {
-        "nameTextMapHash": 1629456710
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CANCEL_UPGRADE": {
-        "nameTextMapHash": 4278013127
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CASH": {
-        "nameTextMapHash": 901035128
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CHAIR": {
-        "nameTextMapHash": 3220802392
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CHOOSE_GOODS": {
-        "nameTextMapHash": 872541786
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_COINS_NOT_ENOUGH": {
-        "nameTextMapHash": 2761980655
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CONFIRM_ADDED": {
-        "nameTextMapHash": 2652615786
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CONFIRM_UPGRADE": {
-        "nameTextMapHash": 1135465914
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_COST_NUMBER": {
-        "nameTextMapHash": 4206718581
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CRITICAL": {
-        "nameTextMapHash": 928722448
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP": {
-        "nameTextMapHash": 2267501104
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROPS_HARVEST_TIPS": {
-        "nameTextMapHash": 2167873314
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_ACCELERATE_ALL": {
-        "nameTextMapHash": 115337413
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_ACCELERATE_ALL_HINT": {
-        "nameTextMapHash": 3062264217
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_ACCELERATE_COIN_LACK": {
-        "nameTextMapHash": 1431897193
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_ACCELERATE_DENY": {
-        "nameTextMapHash": 1410785765
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_ADD_PS": {
-        "nameTextMapHash": 2016246831
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_CANCEL_PS": {
-        "nameTextMapHash": 3199297745
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_CHANGE_BUTTON": {
-        "nameTextMapHash": 2417739209
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_CHANGE_CONFIRM_BUTTON": {
-        "nameTextMapHash": 2583420090
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_CHANGE_DENY_SAME": {
-        "nameTextMapHash": 3074326636
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_CHANGE_HINT": {
-        "nameTextMapHash": 1076426513
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_CHANGE_TITLE": {
-        "nameTextMapHash": 1903088489
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_CLICK_HINT": {
-        "nameTextMapHash": 3941414025
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_DETAIL_ACCELERATE_ONCE": {
-        "nameTextMapHash": 61418156
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_DETAIL_GET_ONCE": {
-        "nameTextMapHash": 577590355
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_DETAIL_INFO_MATURE": {
-        "nameTextMapHash": 3215242155
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_DETAIL_INFO_NUM": {
-        "nameTextMapHash": 1144536627
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_DETAIL_INFO_PRODUCTION": {
-        "nameTextMapHash": 3200514923
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_DETAIL_INFO_TIME": {
-        "nameTextMapHash": 3092004531
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_DETAIL_PS": {
-        "nameTextMapHash": 2604867826
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_DETAIL_TITLE": {
-        "nameTextMapHash": 720302490
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_GET_ALL": {
-        "nameTextMapHash": 1737218676
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_GET_DENY": {
-        "nameTextMapHash": 2617960324
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_GET_FULL": {
-        "nameTextMapHash": 3348335508
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_GET_RESULT_EXTRA": {
-        "nameTextMapHash": 4020525449
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_GET_RESULT_TITLE": {
-        "nameTextMapHash": 4203888713
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_GUIDE_ADD": {
-        "nameTextMapHash": 2220090266
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_GUIDE_CONFIRM_PS": {
-        "nameTextMapHash": 3221696647
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_GUIDE_GET": {
-        "nameTextMapHash": 305082602
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_GUIDE_PLANT": {
-        "nameTextMapHash": 4030535618
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_GUIDE_SELECT": {
-        "nameTextMapHash": 3711740906
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_GUIDE_SWITCH": {
-        "nameTextMapHash": 3509704994
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_HANDBOOK": {
-        "nameTextMapHash": 3826048254
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_LAND": {
-        "nameTextMapHash": 140959662
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_MAX": {
-        "nameTextMapHash": 2509421262
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_NEW_REMINDER": {
-        "nameTextMapHash": 1434514131
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_PLANT_CONFIRM_BUTTON": {
-        "nameTextMapHash": 2431642612
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_PLANT_INFO_NULL": {
-        "nameTextMapHash": 2263877997
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_PLANT_INFO_NUM": {
-        "nameTextMapHash": 1959544773
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_PLANT_INFO_PRODUCTION": {
-        "nameTextMapHash": 4068475453
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_PLANT_INFO_TIME": {
-        "nameTextMapHash": 1409197253
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_PLANT_LIST": {
-        "nameTextMapHash": 3499366211
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_PUZZLE_TITLE": {
-        "nameTextMapHash": 1164945941
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_REFINE": {
-        "nameTextMapHash": 3165600870
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_REFINE_CONFIRM": {
-        "nameTextMapHash": 457646230
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_REFINE_COST": {
-        "nameTextMapHash": 879243246
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_REFINE_EMPTY_HINT": {
-        "nameTextMapHash": 892720849
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_REFINE_FULL": {
-        "nameTextMapHash": 1915079070
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_REFINE_LEVELUP_HINT": {
-        "nameTextMapHash": 2527655792
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_REFINE_LIST": {
-        "nameTextMapHash": 1109419398
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_REFINE_LV": {
-        "nameTextMapHash": 525862022
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_REFINE_NEXT_01": {
-        "nameTextMapHash": 3148634681
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_REFINE_NEXT_02": {
-        "nameTextMapHash": 2945057249
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_REFINE_NEXT_PREVIEW": {
-        "nameTextMapHash": 3128016425
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_REFINE_NULL": {
-        "nameTextMapHash": 3577571342
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_REFINE_PRESS_HINT": {
-        "nameTextMapHash": 3722527312
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_REFINE_SELECT": {
-        "nameTextMapHash": 2049845350
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_REFINE_TECH_HINT": {
-        "nameTextMapHash": 2014867353
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_SELECT_PS": {
-        "nameTextMapHash": 3549833228
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_SWITCH_PS": {
-        "nameTextMapHash": 3073623065
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CROP_UPGRADE_TIPS": {
-        "nameTextMapHash": 2932826325
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_CURRENT_ROUND": {
-        "nameTextMapHash": 2335724395
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_DEALER": {
-        "nameTextMapHash": 3255049768
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_DEALER_CHOOSE_STRATEGIES": {
-        "nameTextMapHash": 1552502322
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_DEALER_COMING_TIPS": {
-        "nameTextMapHash": 3291950179
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_DEALER_CONFIRM_TRADE": {
-        "nameTextMapHash": 147539766
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_DEALER_DEMAND": {
-        "nameTextMapHash": 2865248228
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_DEALER_PHASE": {
-        "nameTextMapHash": 3864318012
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_DEALER_POTION_NOT_ENOUGH_TIPS": {
-        "nameTextMapHash": 3154371292
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_DEALER_REPORT": {
-        "nameTextMapHash": 1450795460
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_DEALER_RESELECT_GOODS": {
-        "nameTextMapHash": 2333750257
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_DEALER_STRATEGIES_EXCEED_TIPS": {
-        "nameTextMapHash": 760392771
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_DEALER_STRATEGIES_LAST_TIME": {
-        "nameTextMapHash": 1716876418
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_DEALER_STRATEGIES_NOT_ENOUGH_TIPS": {
-        "nameTextMapHash": 3806717142
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_DEALER_STRATEGIES_PROCESS": {
-        "nameTextMapHash": 1265892505
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_DEALER_STRATEGY_FEEDBACK": {
-        "nameTextMapHash": 2864966597
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_DEALER_STRATEGY_GOOD": {
-        "nameTextMapHash": 3937080797
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_DEALER_STRATEGY_INCREASE": {
-        "nameTextMapHash": 96686469
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_DEALER_STRATEGY_NAME": {
-        "nameTextMapHash": 3923519965
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_DEALER_STRATEGY_NORMAL": {
-        "nameTextMapHash": 2826257381
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_DEALER_STRATEGY_RESULT": {
-        "nameTextMapHash": 2076882197
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_DETAIL": {
-        "nameTextMapHash": 3359130232
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_END_ROUND": {
-        "nameTextMapHash": 2956363186
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_END_ROUND_TIPS": {
-        "nameTextMapHash": 4004383408
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_EXAM": {
-        "nameTextMapHash": 1489049872
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_EXAM_AUTO_SUMBIT": {
-        "nameTextMapHash": 1860831001
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_EXAM_BEST_RESULT": {
-        "nameTextMapHash": 1892615315
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_EXAM_END": {
-        "nameTextMapHash": 2190725191
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_EXAM_EXIT": {
-        "nameTextMapHash": 3368876455
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_EXAM_FAIL": {
-        "nameTextMapHash": 42311719
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_EXAM_FINISH_HINT": {
-        "nameTextMapHash": 3444308813
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_EXAM_GET_TECH_REWARD": {
-        "nameTextMapHash": 3921170044
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_EXAM_GOAL": {
-        "nameTextMapHash": 2459701479
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_EXAM_NO_RESULT": {
-        "nameTextMapHash": 3958329889
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_EXAM_PASS_TIPS": {
-        "nameTextMapHash": 1415089042
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_EXAM_POTION_HINT": {
-        "nameTextMapHash": 2030579735
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_EXAM_REMAINING": {
-        "nameTextMapHash": 2161529207
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_EXAM_REMIND": {
-        "nameTextMapHash": 265180103
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_EXAM_RESULT": {
-        "nameTextMapHash": 4072348335
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_EXAM_RESULT_A": {
-        "nameTextMapHash": 4228174836
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_EXAM_RESULT_B": {
-        "nameTextMapHash": 998804732
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_EXAM_RESULT_C": {
-        "nameTextMapHash": 1170346052
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_EXAM_RESULT_RULE": {
-        "nameTextMapHash": 3275548036
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_EXAM_RESULT_S": {
-        "nameTextMapHash": 2860802956
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_EXAM_RETRY": {
-        "nameTextMapHash": 1813669831
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_EXAM_START": {
-        "nameTextMapHash": 2776004447
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_EXAM_START_TIPS": {
-        "nameTextMapHash": 411412398
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_EXAM_SUBMIT": {
-        "nameTextMapHash": 372456407
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_EXAM_SUCCESS": {
-        "nameTextMapHash": 467056263
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_EXAM_SUMBIT_HINT": {
-        "nameTextMapHash": 241646308
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_EXAM_TECH_BRANCH_LOCK_TIPS": {
-        "nameTextMapHash": 192054441
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_EXAM_TECH_REWARD_TIPS": {
-        "nameTextMapHash": 2353592830
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_EXIT": {
-        "nameTextMapHash": 206560576
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_EXIT_SELL_HINT": {
-        "nameTextMapHash": 268512874
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_EXTRA_TECH_BRANCH_LOCK_TIPS": {
-        "nameTextMapHash": 3642691247
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_FILTER_FAILED": {
-        "nameTextMapHash": 1564044491
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_FILTER_TIPS": {
-        "nameTextMapHash": 4083996483
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_FILTER_TITLE": {
-        "nameTextMapHash": 2950146595
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_FULLY_UPGRADE_TIPS": {
-        "nameTextMapHash": 3631102143
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_GOODS_CHANGED_TIPS": {
-        "nameTextMapHash": 1873612768
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_GOODS_COST": {
-        "nameTextMapHash": 2700845471
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_GOODS_LIMIT": {
-        "nameTextMapHash": 742519359
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_GOODS_OVERAGE": {
-        "nameTextMapHash": 3046547647
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_GOODS_RENEW": {
-        "nameTextMapHash": 2511938679
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_GOTO_FAIL": {
-        "nameTextMapHash": 3490945069
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_GOTO_START": {
-        "nameTextMapHash": 1666156597
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_GUIDE_HANDBOOK": {
-        "nameTextMapHash": 3959957694
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_HANDBOOK": {
-        "nameTextMapHash": 570630968
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_HANDBOOK_BLANK": {
-        "nameTextMapHash": 771501009
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_HANDBOOK_CASH_DESC": {
-        "nameTextMapHash": 2064421352
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_HANDBOOK_CASH_TITLE": {
-        "nameTextMapHash": 3504690048
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_HANDBOOK_COMPLETION": {
-        "nameTextMapHash": 1974352049
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_HANDBOOK_CONSUMPTION_TIPS": {
-        "nameTextMapHash": 3882944814
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_HANDBOOK_DEALER_COMING": {
-        "nameTextMapHash": 4086860917
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_HANDBOOK_DESC": {
-        "nameTextMapHash": 877106425
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_HANDBOOK_EVENT": {
-        "nameTextMapHash": 3987140081
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_HANDBOOK_FIXED_TASKS": {
-        "nameTextMapHash": 2886859136
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_HANDBOOK_GOAL_DESC": {
-        "nameTextMapHash": 1957695752
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_HANDBOOK_GOAL_TITLE": {
-        "nameTextMapHash": 720319984
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_HANDBOOK_LEVEL_DESC": {
-        "nameTextMapHash": 253681748
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_HANDBOOK_LEVEL_TITLE": {
-        "nameTextMapHash": 134930284
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_HANDBOOK_OVERVIEW": {
-        "nameTextMapHash": 838637073
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_HANDBOOK_REPORT": {
-        "nameTextMapHash": 3927094049
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_HANDBOOK_SHOP_TIPS": {
-        "nameTextMapHash": 2048656217
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_HANDBOOK_TECHTREE_TIPS": {
-        "nameTextMapHash": 2064685279
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_HANDBOOK_TITLE": {
-        "nameTextMapHash": 1804012113
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_INCOME": {
-        "nameTextMapHash": 1714191144
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_LAST_ROUND": {
-        "nameTextMapHash": 1770624946
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_LETTER": {
-        "nameTextMapHash": 2701171664
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_MARK_DESC": {
-        "nameTextMapHash": 69515334
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_MARK_TITLE": {
-        "nameTextMapHash": 1466883022
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_MONEY_LIMIT_TIPS": {
-        "nameTextMapHash": 3489785899
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_NETWORK_DELAY": {
-        "nameTextMapHash": 1842511743
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_NEWS": {
-        "nameTextMapHash": 2822277408
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_NEWS_REFRESH_TIPS": {
-        "nameTextMapHash": 1293673642
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_NEWS_TITLE_01": {
-        "nameTextMapHash": 1179269823
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_NEWS_TITLE_02": {
-        "nameTextMapHash": 864701983
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_NEWS_TITLE_03": {
-        "nameTextMapHash": 3915482759
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_NO_GOODS_REPORT": {
-        "nameTextMapHash": 2070337323
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_NO_RECORD_TIPS": {
-        "nameTextMapHash": 3684601830
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_OPEN_HINT": {
-        "nameTextMapHash": 2663035169
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_ORDER": {
-        "nameTextMapHash": 3833116960
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_ORDER_BREAK_TIPS": {
-        "nameTextMapHash": 2620447979
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_ORDER_DELIVER": {
-        "nameTextMapHash": 4247664708
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_ORDER_NO_GOODS_TIPS": {
-        "nameTextMapHash": 3763775677
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_ORDER_POTION_NOT_ENOUGH_TIPS": {
-        "nameTextMapHash": 1518725925
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_ORDER_REMIND": {
-        "nameTextMapHash": 2075006004
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_ORDER_START_TIPS": {
-        "nameTextMapHash": 517911730
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_PHASE_REWARD_TITLE": {
-        "nameTextMapHash": 2100017299
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_PLANT": {
-        "nameTextMapHash": 2710041112
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_PLANT_HARVESTABLE": {
-        "nameTextMapHash": 3362799500
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_PLAYER_LEVEL": {
-        "nameTextMapHash": 1007061820
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_PLAYER_LEVEL_LV": {
-        "nameTextMapHash": 2415299030
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_PLAYER_LEVEL_PREVIEW_REWARD": {
-        "nameTextMapHash": 872272043
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_PLAYER_LEVEL_PREVIEW_TITLE": {
-        "nameTextMapHash": 3148920187
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_PLAYER_LEVEL_TITLE": {
-        "nameTextMapHash": 1408865462
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_PLAYER_LEVEL_UNLOCK_TIPS": {
-        "nameTextMapHash": 1535061702
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_PLAYER_LEVEL_UP": {
-        "nameTextMapHash": 3620871358
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION": {
-        "nameTextMapHash": 447909936
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_CANCEL_ALL_BUTTON": {
-        "nameTextMapHash": 4079748027
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_CANCEL_ALL_HINT": {
-        "nameTextMapHash": 525558803
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_CANCEL_BUTTON": {
-        "nameTextMapHash": 749318691
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_CONFIRM_BUTTON": {
-        "nameTextMapHash": 472499042
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_DENY": {
-        "nameTextMapHash": 2055168299
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_DETAIL_CLOSE_PS": {
-        "nameTextMapHash": 419438004
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_DETAIL_OPEN_PS": {
-        "nameTextMapHash": 3835748974
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_DIY": {
-        "nameTextMapHash": 3842102075
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_DIY_BOTTLE": {
-        "nameTextMapHash": 1640814649
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_DIY_CANCEL": {
-        "nameTextMapHash": 1846190417
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_DIY_DECORATION": {
-        "nameTextMapHash": 189398009
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_DIY_DECORATION_UNSELECT": {
-        "nameTextMapHash": 2263621212
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_DIY_FINISH_BUTTON": {
-        "nameTextMapHash": 633774831
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_DIY_SELECT": {
-        "nameTextMapHash": 2958631497
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_DROP_BUTTON": {
-        "nameTextMapHash": 393120248
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_DROP_DESC": {
-        "nameTextMapHash": 3398214424
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_DROP_NEW_TITLE": {
-        "nameTextMapHash": 1789624271
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_DROP_OLD_TITLE": {
-        "nameTextMapHash": 3582173295
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_DROP_ONSALE": {
-        "nameTextMapHash": 2762213128
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_DROP_ONSALE_HINT": {
-        "nameTextMapHash": 1567713157
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_DROP_TITLE": {
-        "nameTextMapHash": 4208779544
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_DROP_UNSELECT": {
-        "nameTextMapHash": 1627540872
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_EXAM_DETAIL": {
-        "nameTextMapHash": 224915786
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_EXAM_HINT": {
-        "nameTextMapHash": 1008671994
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_EXAM_MAIN": {
-        "nameTextMapHash": 1211384498
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_EXAM_SUB": {
-        "nameTextMapHash": 3582962242
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_EXIT_HINT": {
-        "nameTextMapHash": 924322210
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_FAST_BUTTON": {
-        "nameTextMapHash": 440184632
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_FAST_CANCEL_PS": {
-        "nameTextMapHash": 2950351602
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_FAST_CLOSE_PS": {
-        "nameTextMapHash": 1076593406
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_FAST_LACK": {
-        "nameTextMapHash": 336298272
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_FAST_RETURN_PS": {
-        "nameTextMapHash": 4048617206
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_FAST_SELECT_PS": {
-        "nameTextMapHash": 1640309246
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_FAST_TIPS": {
-        "nameTextMapHash": 3183767176
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_FAST_UNSELECT": {
-        "nameTextMapHash": 1467721280
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_FINISH_BUTTON": {
-        "nameTextMapHash": 2433712096
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_FINISH_DENY": {
-        "nameTextMapHash": 634755296
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_FINISH_HINT": {
-        "nameTextMapHash": 3501538696
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_GUIDE_INFO": {
-        "nameTextMapHash": 1582478381
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_GUIDE_PUT": {
-        "nameTextMapHash": 1175889901
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_GUIDE_ROTATE": {
-        "nameTextMapHash": 910035949
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_GUIDE_SELECT": {
-        "nameTextMapHash": 285431381
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_GUIDE_SELECT_PS": {
-        "nameTextMapHash": 2152673139
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_MATERIAL": {
-        "nameTextMapHash": 1475721635
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_NAME_01": {
-        "nameTextMapHash": 2830500012
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_NAME_02": {
-        "nameTextMapHash": 3961146284
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_NAME_03": {
-        "nameTextMapHash": 27808028
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_NAME_04": {
-        "nameTextMapHash": 2690255596
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_NAME_05": {
-        "nameTextMapHash": 4024965420
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_NAME_06": {
-        "nameTextMapHash": 2511419844
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_NAME_DEFAULT": {
-        "nameTextMapHash": 1720178364
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_NAME_DUAL_PROP": {
-        "nameTextMapHash": 2344868076
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_NAME_PLUS": {
-        "nameTextMapHash": 1338492332
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_NUM_FORMAT": {
-        "nameTextMapHash": 1316866658
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_OVERLAP_NUMBER": {
-        "nameTextMapHash": 2881035403
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_OVERLAP_TITLE": {
-        "nameTextMapHash": 2387902675
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_POT_FAST": {
-        "nameTextMapHash": 3075591664
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_POT_LIMIT": {
-        "nameTextMapHash": 2007284400
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_POT_NORMAL": {
-        "nameTextMapHash": 2493022544
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_PRICE": {
-        "nameTextMapHash": 767464803
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_PROP_CLOSE_PS": {
-        "nameTextMapHash": 1988142246
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_PROP_DETAIL": {
-        "nameTextMapHash": 3746493585
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_PROP_TITLE": {
-        "nameTextMapHash": 3513057881
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_PS_EDIT": {
-        "nameTextMapHash": 2964225862
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_PS_REGION_SWITCH": {
-        "nameTextMapHash": 322565970
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_RATE_FORMAT": {
-        "nameTextMapHash": 596971908
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_RATE_TITLE": {
-        "nameTextMapHash": 1560593844
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_RESULT": {
-        "nameTextMapHash": 3687991235
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_RESULT_BUFF_01": {
-        "nameTextMapHash": 2882278626
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_RESULT_BUFF_02": {
-        "nameTextMapHash": 1172118562
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_RESULT_BUFF_03": {
-        "nameTextMapHash": 1511707130
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_RESULT_BUFF_04": {
-        "nameTextMapHash": 3535212778
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_RESULT_BUFF_05": {
-        "nameTextMapHash": 476466738
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_RESULT_BUFF_TITLE": {
-        "nameTextMapHash": 2415349850
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_RESULT_CROP_LEVEL_MAX": {
-        "nameTextMapHash": 2296055327
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_RESULT_CROP_LEVEL_TITLE": {
-        "nameTextMapHash": 3904180919
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_RESULT_CROP_NEW_HINT": {
-        "nameTextMapHash": 1601802646
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_RESULT_CROP_NEW_TITLE": {
-        "nameTextMapHash": 417296102
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_RESULT_EFFICIENCY_NEW_HINT": {
-        "nameTextMapHash": 70358347
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_RESULT_GET_BUTTON": {
-        "nameTextMapHash": 3695074862
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_RESULT_LEVEL": {
-        "nameTextMapHash": 3737730609
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_RESULT_OVERLAP_NEW_HINT": {
-        "nameTextMapHash": 4071250869
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_RESULT_POTION_TWICE_HINT": {
-        "nameTextMapHash": 676684738
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_RESULT_POT_NEW_HINT": {
-        "nameTextMapHash": 872995415
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_RESULT_SHOP_HINT": {
-        "nameTextMapHash": 1943562094
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_ROTATE_BUTTON": {
-        "nameTextMapHash": 907336942
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_TAG_CONNECT": {
-        "nameTextMapHash": 2217375106
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_UPGRADE": {
-        "nameTextMapHash": 561717907
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_UPGRADE_NONE": {
-        "nameTextMapHash": 710146989
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_POTION_UPGRADE_TIPS": {
-        "nameTextMapHash": 1395982909
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_PROFIT": {
-        "nameTextMapHash": 1008304944
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_PROFIT_TREND": {
-        "nameTextMapHash": 2244650763
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_REVENUE": {
-        "nameTextMapHash": 3212714024
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_REVENUE_DETAIL": {
-        "nameTextMapHash": 2581133676
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_REVENUE_STRUCTURE": {
-        "nameTextMapHash": 3368000028
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_REWARD_TITLE": {
-        "nameTextMapHash": 2272915512
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_ROUND": {
-        "nameTextMapHash": 1313001512
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_ROUND_DETAIL": {
-        "nameTextMapHash": 2803436546
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_ROUND_INTERVAL": {
-        "nameTextMapHash": 391144602
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_ROUND_REVENUE": {
-        "nameTextMapHash": 4210170850
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SALES_VOLUME": {
-        "nameTextMapHash": 3943910858
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SAVE_AND_EXIT": {
-        "nameTextMapHash": 1232609571
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SELECTED_GOODS": {
-        "nameTextMapHash": 3598429310
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SELL": {
-        "nameTextMapHash": 4735656
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SELLING_REPORT": {
-        "nameTextMapHash": 492526849
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SHELF": {
-        "nameTextMapHash": 3675317720
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SHOP_COST": {
-        "nameTextMapHash": 1880211474
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SHOP_GOODS_LOCK_01": {
-        "nameTextMapHash": 997220477
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SHOP_GOODS_LOCK_02": {
-        "nameTextMapHash": 2731785765
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SHOP_GOODS_UNLOCK": {
-        "nameTextMapHash": 1574109973
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_STAGE_BREAK": {
-        "nameTextMapHash": 4158156572
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_STAGE_BREAK_TIPS": {
-        "nameTextMapHash": 3966199568
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_STAGE_GOAL": {
-        "nameTextMapHash": 398566652
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_STAGE_GOAL_NO_TITLE": {
-        "nameTextMapHash": 3769819083
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_STAGE_GOAL_PERCENTAGE": {
-        "nameTextMapHash": 1672542260
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_STAGE_LAST_ROUND": {
-        "nameTextMapHash": 222021070
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_STAGE_LOCK_TIPS": {
-        "nameTextMapHash": 3682890513
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_STAGE_LOCK_TIPS_01": {
-        "nameTextMapHash": 2492805329
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_STAGE_REWARD": {
-        "nameTextMapHash": 3362433252
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_STAGE_TASK_TIPS": {
-        "nameTextMapHash": 4259781509
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_STAGE_TIPS": {
-        "nameTextMapHash": 3274191132
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY": {
-        "nameTextMapHash": 745584040
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P1_DESC1": {
-        "nameTextMapHash": 2008955883
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P1_DESC2": {
-        "nameTextMapHash": 1088689867
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P1_DESC3": {
-        "nameTextMapHash": 2643554843
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P1_DESC4": {
-        "nameTextMapHash": 1092531099
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P1_DESC5": {
-        "nameTextMapHash": 3397610147
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P1_PARM1": {
-        "nameTextMapHash": 1684147851
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P1_PARM2": {
-        "nameTextMapHash": 713505259
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P1_PARM3": {
-        "nameTextMapHash": 2022157355
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P1_PARM4": {
-        "nameTextMapHash": 648713187
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P1_PARM5": {
-        "nameTextMapHash": 3545579395
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P2_DESC1": {
-        "nameTextMapHash": 1030065665
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P2_DESC2": {
-        "nameTextMapHash": 1560583585
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P2_DESC3": {
-        "nameTextMapHash": 2729727593
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P2_DESC4": {
-        "nameTextMapHash": 111738681
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P2_DESC5": {
-        "nameTextMapHash": 126655801
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P2_PARM1": {
-        "nameTextMapHash": 3252526905
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P2_PARM2": {
-        "nameTextMapHash": 4127593785
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P2_PARM3": {
-        "nameTextMapHash": 1225289801
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P2_PARM4": {
-        "nameTextMapHash": 2091939337
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P2_PARM5": {
-        "nameTextMapHash": 1925051361
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P3_DESC1": {
-        "nameTextMapHash": 547748127
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P3_DESC2": {
-        "nameTextMapHash": 1762530087
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P3_DESC3": {
-        "nameTextMapHash": 602357767
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P3_DESC4": {
-        "nameTextMapHash": 1914013111
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P3_DESC5": {
-        "nameTextMapHash": 2526635311
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P3_PARM1": {
-        "nameTextMapHash": 2824964847
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P3_PARM2": {
-        "nameTextMapHash": 1660515759
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P3_PARM3": {
-        "nameTextMapHash": 639497479
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P3_PARM4": {
-        "nameTextMapHash": 431265415
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P3_PARM5": {
-        "nameTextMapHash": 1094503487
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P4_DESC1": {
-        "nameTextMapHash": 2278648236
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P4_DESC2": {
-        "nameTextMapHash": 1969932468
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P4_DESC3": {
-        "nameTextMapHash": 2359385860
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P4_DESC4": {
-        "nameTextMapHash": 2316047156
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P4_DESC5": {
-        "nameTextMapHash": 442403268
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P4_PARM1": {
-        "nameTextMapHash": 3379185172
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P4_PARM2": {
-        "nameTextMapHash": 4067807044
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P4_PARM3": {
-        "nameTextMapHash": 1407939252
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P4_PARM4": {
-        "nameTextMapHash": 196161084
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P4_PARM5": {
-        "nameTextMapHash": 3005412876
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_TITLE": {
-        "nameTextMapHash": 4184142263
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_TAG_NAME": {
-        "nameTextMapHash": 3876860324
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_TAG_TITLE": {
-        "nameTextMapHash": 4061151388
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_TASK_NOT_FINISH": {
-        "nameTextMapHash": 2039395681
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_TECH_BRANCH_FINISH": {
-        "nameTextMapHash": 4289561557
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_TECH_BRANCH_LEVEL_DETAIL": {
-        "nameTextMapHash": 424028999
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_TECH_BRANCH_UNLOCK": {
-        "nameTextMapHash": 3225681365
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_TECH_BRANCH_UNLOCK_TIPS": {
-        "nameTextMapHash": 3124018265
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_TECH_BRANCH_UPGRADE": {
-        "nameTextMapHash": 2242764437
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_TECH_BRANCH_UPGRADE_TIPS": {
-        "nameTextMapHash": 2136479449
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_TECH_TREE_ALCHEMY_TITLE": {
-        "nameTextMapHash": 3528541260
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_TECH_TREE_EXAM_TITLE": {
-        "nameTextMapHash": 3135623612
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_TECH_TREE_PLANT_TITLE": {
-        "nameTextMapHash": 3966241995
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_TECH_TREE_SELL_TITLE": {
-        "nameTextMapHash": 311730520
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_TECH_TREE_TITLE": {
-        "nameTextMapHash": 1844405521
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_TUTORIAL_NOT_RECORD": {
-        "nameTextMapHash": 3258793305
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_TUTORIAL_TITLE": {
-        "nameTextMapHash": 3956948558
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_TYPE_NAME": {
-        "nameTextMapHash": 3827195457
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_TYPE_TITLE": {
-        "nameTextMapHash": 778662985
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_UPGRADE_CONSUME": {
-        "nameTextMapHash": 1294297115
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_UPGRADE_SUCCESS": {
-        "nameTextMapHash": 245671115
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_WEAPON_REDEEM": {
-        "nameTextMapHash": 1449494223
-    },
-    "UI_ACTIVITY_ALCHEMYSIM_WEAPON_REDEEM_TIPS": {
-        "nameTextMapHash": 1470624583
-    },
     "UI_ACTIVITY_AREA_QUESTTIPS": {
         "nameTextMapHash": 896037515
     },
     "UI_ACTIVITY_ARENACHALLENGE3_REWARD_DESC": {
         "nameTextMapHash": 3591115396
     },
     "UI_ACTIVITY_ARENACHALLENGE4_CHALLENGE_FACTOR": {
@@ -16627,74 +15790,14 @@
     },
     "UI_ACTIVITY_ASTROLABLE_PROGRESS": {
         "nameTextMapHash": 3285814292
     },
     "UI_ACTIVITY_AUTO_QUIT": {
         "nameTextMapHash": 4213771873
     },
-    "UI_ACTIVITY_AUTO_TIME_STOP_ACTION_TIPS": {
-        "nameTextMapHash": 1577242564
-    },
-    "UI_ACTIVITY_AUTO_TIME_STOP_CAMERA_TIPS": {
-        "nameTextMapHash": 2736393882
-    },
-    "UI_ACTIVITY_AUTO_TIME_STOP_CHAR_CHANGE_TIPS": {
-        "nameTextMapHash": 2130506856
-    },
-    "UI_ACTIVITY_AUTO_TIME_STOP_CHAR_NOT_FULL_TIPS": {
-        "nameTextMapHash": 1126526848
-    },
-    "UI_ACTIVITY_AUTO_TIME_STOP_DUNGEON_ENTRY_INTERACTION": {
-        "nameTextMapHash": 567694789
-    },
-    "UI_ACTIVITY_AUTO_TIME_STOP_DUNGEON_TITLE": {
-        "nameTextMapHash": 1720579352
-    },
-    "UI_ACTIVITY_AUTO_TIME_STOP_END_QUEST_BUTTON": {
-        "nameTextMapHash": 3541305859
-    },
-    "UI_ACTIVITY_AUTO_TIME_STOP_EXIT_DUNGEON_TIPS": {
-        "nameTextMapHash": 1646682641
-    },
-    "UI_ACTIVITY_AUTO_TIME_STOP_EXIT_TIPS": {
-        "nameTextMapHash": 467104758
-    },
-    "UI_ACTIVITY_AUTO_TIME_STOP_GUIDE_TIPS": {
-        "nameTextMapHash": 1921672378
-    },
-    "UI_ACTIVITY_AUTO_TIME_STOP_GUIDE_TIPS_1": {
-        "nameTextMapHash": 2333823033
-    },
-    "UI_ACTIVITY_AUTO_TIME_STOP_LEVEL_BUFF_TITLE": {
-        "nameTextMapHash": 1758507918
-    },
-    "UI_ACTIVITY_AUTO_TIME_STOP_LEVEL_DESC": {
-        "nameTextMapHash": 1514102142
-    },
-    "UI_ACTIVITY_AUTO_TIME_STOP_MAIN_PROGRESS": {
-        "nameTextMapHash": 1468022043
-    },
-    "UI_ACTIVITY_AUTO_TIME_STOP_PRE_LEVEL_LOCKED": {
-        "nameTextMapHash": 1089988484
-    },
-    "UI_ACTIVITY_AUTO_TIME_STOP_SUCCEED_DATA_TITLE": {
-        "nameTextMapHash": 4044858431
-    },
-    "UI_ACTIVITY_AUTO_TIME_STOP_TARGET_1": {
-        "nameTextMapHash": 3025440236
-    },
-    "UI_ACTIVITY_AUTO_TIME_STOP_TARGET_2": {
-        "nameTextMapHash": 776780460
-    },
-    "UI_ACTIVITY_AUTO_TIME_STOP_TEAM_TITLE": {
-        "nameTextMapHash": 463757385
-    },
-    "UI_ACTIVITY_AUTO_TIME_STOP_TITLE": {
-        "nameTextMapHash": 3295518470
-    },
     "UI_ACTIVITY_AVARTARTRIAL_INDUNGEON_FINISHPANEL_CHANGE": {
         "nameTextMapHash": 575427936
     },
     "UI_ACTIVITY_AVARTARTRIAL_INDUNGEON_FINISHPANEL_CONTINUE": {
         "nameTextMapHash": 1536442424
     },
     "UI_ACTIVITY_AVARTARTRIAL_INDUNGEON_FINISHPANEL_LEAVE": {
@@ -16729,14 +15832,20 @@
     },
     "UI_ACTIVITY_AVARTARTRIAL_RULE_TITLE": {
         "nameTextMapHash": 3897589619
     },
     "UI_ACTIVITY_AVATAR_PROGRESS_UNMET": {
         "nameTextMapHash": 3508067920
     },
+    "UI_ACTIVITY_AVATAR_SCREEN": {
+        "nameTextMapHash": 1420803628
+    },
+    "UI_ACTIVITY_AVATAR_SCREEN_NO_RESULT": {
+        "nameTextMapHash": 609392589
+    },
     "UI_ACTIVITY_AWARDPAGE": {
         "nameTextMapHash": 2525653840
     },
     "UI_ACTIVITY_BEGINTIME": {
         "nameTextMapHash": 3502714504
     },
     "UI_ACTIVITY_BESTSCORE_CRUCIBLE": {
@@ -17179,200 +16288,14 @@
     },
     "UI_ACTIVITY_BounceConjuring_DESC": {
         "nameTextMapHash": 3387641929
     },
     "UI_ACTIVITY_CANNOT_ONLINE_TIPS": {
         "nameTextMapHash": 1348315470
     },
-    "UI_ACTIVITY_CATCAFE_ABANDON": {
-        "nameTextMapHash": 1801579372
-    },
-    "UI_ACTIVITY_CATCAFE_ACTIVITYNAME": {
-        "nameTextMapHash": 815897364
-    },
-    "UI_ACTIVITY_CATCAFE_AFFECTION": {
-        "nameTextMapHash": 724136372
-    },
-    "UI_ACTIVITY_CATCAFE_AFFECTION_HINT": {
-        "nameTextMapHash": 4200307400
-    },
-    "UI_ACTIVITY_CATCAFE_AUTOSAVED_FINISHHINT": {
-        "nameTextMapHash": 1106471958
-    },
-    "UI_ACTIVITY_CATCAFE_BLACKSCREEN_CAT1COME": {
-        "nameTextMapHash": 3761692188
-    },
-    "UI_ACTIVITY_CATCAFE_BLACKSCREEN_CAT2COME": {
-        "nameTextMapHash": 1667709068
-    },
-    "UI_ACTIVITY_CATCAFE_BLACKSCREEN_CAT3COME": {
-        "nameTextMapHash": 2198233332
-    },
-    "UI_ACTIVITY_CATCAFE_BLACKSCREEN_CAT4COME": {
-        "nameTextMapHash": 3654060124
-    },
-    "UI_ACTIVITY_CATCAFE_BLACKSCREEN_CAT5COME": {
-        "nameTextMapHash": 974941804
-    },
-    "UI_ACTIVITY_CATCAFE_BOSSDES": {
-        "nameTextMapHash": 2058173052
-    },
-    "UI_ACTIVITY_CATCAFE_BOSSLEAVING": {
-        "nameTextMapHash": 1648213932
-    },
-    "UI_ACTIVITY_CATCAFE_BOSSLOCKED_HINT": {
-        "nameTextMapHash": 2928441111
-    },
-    "UI_ACTIVITY_CATCAFE_BOSSLOCKED_TITLE": {
-        "nameTextMapHash": 4193531119
-    },
-    "UI_ACTIVITY_CATCAFE_BOSSQUESTHINT": {
-        "nameTextMapHash": 315165860
-    },
-    "UI_ACTIVITY_CATCAFE_CATBALCONY": {
-        "nameTextMapHash": 1288757860
-    },
-    "UI_ACTIVITY_CATCAFE_CATBOSSQUEST_UNFINISHED": {
-        "nameTextMapHash": 3723515963
-    },
-    "UI_ACTIVITY_CATCAFE_CATNAME_TITLE": {
-        "nameTextMapHash": 1646487394
-    },
-    "UI_ACTIVITY_CATCAFE_CATREPUTATION": {
-        "nameTextMapHash": 32804988
-    },
-    "UI_ACTIVITY_CATCAFE_CATREPUTATION_FULL": {
-        "nameTextMapHash": 2399116886
-    },
-    "UI_ACTIVITY_CATCAFE_DECOFINISHED": {
-        "nameTextMapHash": 1467273508
-    },
-    "UI_ACTIVITY_CATCAFE_DECOFINISHED_CANTCHANGE": {
-        "nameTextMapHash": 1501870942
-    },
-    "UI_ACTIVITY_CATCAFE_DECOHINT": {
-        "nameTextMapHash": 607725564
-    },
-    "UI_ACTIVITY_CATCAFE_DECOQUIT_DESC": {
-        "nameTextMapHash": 455062617
-    },
-    "UI_ACTIVITY_CATCAFE_DECOQUIT_TITLE": {
-        "nameTextMapHash": 2014152769
-    },
-    "UI_ACTIVITY_CATCAFE_DECOSAVED": {
-        "nameTextMapHash": 178431740
-    },
-    "UI_ACTIVITY_CATCAFE_DECO_INTERACTNAME": {
-        "nameTextMapHash": 1195515751
-    },
-    "UI_ACTIVITY_CATCAFE_DECO_SCOREA": {
-        "nameTextMapHash": 2143870343
-    },
-    "UI_ACTIVITY_CATCAFE_DECO_SCOREB": {
-        "nameTextMapHash": 4006811063
-    },
-    "UI_ACTIVITY_CATCAFE_DECO_SCOREC": {
-        "nameTextMapHash": 475719719
-    },
-    "UI_ACTIVITY_CATCAFE_ENDINGQUEST": {
-        "nameTextMapHash": 201099028
-    },
-    "UI_ACTIVITY_CATCAFE_FAMILIAR": {
-        "nameTextMapHash": 2172787612
-    },
-    "UI_ACTIVITY_CATCAFE_FAMILIARHINT": {
-        "nameTextMapHash": 2372560476
-    },
-    "UI_ACTIVITY_CATCAFE_FAVORDROP": {
-        "nameTextMapHash": 3504299852
-    },
-    "UI_ACTIVITY_CATCAFE_FAVORSTOP": {
-        "nameTextMapHash": 88708364
-    },
-    "UI_ACTIVITY_CATCAFE_FAVOR_MINUS": {
-        "nameTextMapHash": 4095771853
-    },
-    "UI_ACTIVITY_CATCAFE_FAVOR_PLUS": {
-        "nameTextMapHash": 2847654109
-    },
-    "UI_ACTIVITY_CATCAFE_FEEDDESC": {
-        "nameTextMapHash": 481817724
-    },
-    "UI_ACTIVITY_CATCAFE_FEEDFINISHED": {
-        "nameTextMapHash": 295185188
-    },
-    "UI_ACTIVITY_CATCAFE_FEEDHINT": {
-        "nameTextMapHash": 1765445700
-    },
-    "UI_ACTIVITY_CATCAFE_FEEDTITLE": {
-        "nameTextMapHash": 800625676
-    },
-    "UI_ACTIVITY_CATCAFE_FEED_INTERACTNAME": {
-        "nameTextMapHash": 1554941298
-    },
-    "UI_ACTIVITY_CATCAFE_GOTO_DECO": {
-        "nameTextMapHash": 3537672899
-    },
-    "UI_ACTIVITY_CATCAFE_GOTO_FEED": {
-        "nameTextMapHash": 3531406491
-    },
-    "UI_ACTIVITY_CATCAFE_GOTO_PLAY": {
-        "nameTextMapHash": 2371412483
-    },
-    "UI_ACTIVITY_CATCAFE_HINT_COUNTDOWN": {
-        "nameTextMapHash": 2362168758
-    },
-    "UI_ACTIVITY_CATCAFE_HINT_LOCKED": {
-        "nameTextMapHash": 966928398
-    },
-    "UI_ACTIVITY_CATCAFE_MARK_DESC": {
-        "nameTextMapHash": 139343108
-    },
-    "UI_ACTIVITY_CATCAFE_MARK_TITLE": {
-        "nameTextMapHash": 2381868588
-    },
-    "UI_ACTIVITY_CATCAFE_PLAYQUIT_BLACK": {
-        "nameTextMapHash": 1455294909
-    },
-    "UI_ACTIVITY_CATCAFE_PLAYQUIT_DESC": {
-        "nameTextMapHash": 527884565
-    },
-    "UI_ACTIVITY_CATCAFE_PLAYQUIT_TITLE": {
-        "nameTextMapHash": 329069509
-    },
-    "UI_ACTIVITY_CATCAFE_PLAYUNLOCKHINT": {
-        "nameTextMapHash": 401580276
-    },
-    "UI_ACTIVITY_CATCAFE_PLAY_INTERACTNAME": {
-        "nameTextMapHash": 3205506787
-    },
-    "UI_ACTIVITY_CATCAFE_REPUTATION_NUM1": {
-        "nameTextMapHash": 2858381703
-    },
-    "UI_ACTIVITY_CATCAFE_REPUTATION_NUM2": {
-        "nameTextMapHash": 3107502759
-    },
-    "UI_ACTIVITY_CATCAFE_SAVEANDQUIT": {
-        "nameTextMapHash": 4129811156
-    },
-    "UI_ACTIVITY_CATCAFE_STATE": {
-        "nameTextMapHash": 2409443652
-    },
-    "UI_ACTIVITY_CATCAFE_UNDECOED": {
-        "nameTextMapHash": 283514756
-    },
-    "UI_ACTIVITY_CATCAFE_UNFARMILIAR": {
-        "nameTextMapHash": 3917719972
-    },
-    "UI_ACTIVITY_CATCAFE_UNLOCKHINT": {
-        "nameTextMapHash": 3389278892
-    },
-    "UI_ACTIVITY_CATCAFE_UNSUMMON": {
-        "nameTextMapHash": 3523262276
-    },
     "UI_ACTIVITY_CHALLENGE_BEGIN": {
         "nameTextMapHash": 678714236
     },
     "UI_ACTIVITY_CHALLENGE_DETAIL": {
         "nameTextMapHash": 3121683592
     },
     "UI_ACTIVITY_CHALLENGE_GOTO_BUTTON": {
@@ -18160,20 +17083,179 @@
     },
     "UI_ACTIVITY_CRUCIBLE_TIMELAST": {
         "nameTextMapHash": 3023562393
     },
     "UI_ACTIVITY_CRUCIBLE_TIMESPEND": {
         "nameTextMapHash": 3472811009
     },
+    "UI_ACTIVITY_CRYSTALLINK_ARRANGE_AVATAR": {
+        "nameTextMapHash": 3875187014
+    },
+    "UI_ACTIVITY_CRYSTALLINK_ARRANGE_AVATAR_FULL_TIPS": {
+        "nameTextMapHash": 3506236691
+    },
+    "UI_ACTIVITY_CRYSTALLINK_ARRANGE_AVATAR_OTHER_TEAM_TIPS": {
+        "nameTextMapHash": 1427264689
+    },
+    "UI_ACTIVITY_CRYSTALLINK_ARRANGE_AVATAR_TRY_TIPS": {
+        "nameTextMapHash": 816795481
+    },
+    "UI_ACTIVITY_CRYSTALLINK_ARRANGE_BUFF": {
+        "nameTextMapHash": 3160485742
+    },
+    "UI_ACTIVITY_CRYSTALLINK_ARRANGE_LEVEL_DETAIL_INFO": {
+        "nameTextMapHash": 2007473574
+    },
+    "UI_ACTIVITY_CRYSTALLINK_AVATAR_NUM_TIPS": {
+        "nameTextMapHash": 822553351
+    },
+    "UI_ACTIVITY_CRYSTALLINK_BUTTON_CHARACTER_PREVIEW": {
+        "nameTextMapHash": 1518856316
+    },
+    "UI_ACTIVITY_CRYSTALLINK_CONDITION_CD": {
+        "nameTextMapHash": 2521853801
+    },
+    "UI_ACTIVITY_CRYSTALLINK_CONDITION_CD_DESC": {
+        "nameTextMapHash": 462592910
+    },
+    "UI_ACTIVITY_CRYSTALLINK_CONDITION_CRYSTAL": {
+        "nameTextMapHash": 2978649633
+    },
+    "UI_ACTIVITY_CRYSTALLINK_DETIL_INFO": {
+        "nameTextMapHash": 210580015
+    },
+    "UI_ACTIVITY_CRYSTALLINK_DUNGEON_INFO": {
+        "nameTextMapHash": 110066853
+    },
+    "UI_ACTIVITY_CRYSTALLINK_EFFECT_CRYSTAL": {
+        "nameTextMapHash": 2576164750
+    },
+    "UI_ACTIVITY_CRYSTALLINK_EFFECT_TIME_DESC": {
+        "nameTextMapHash": 854091146
+    },
+    "UI_ACTIVITY_CRYSTALLINK_END_BOSS_NUM": {
+        "nameTextMapHash": 1882027011
+    },
+    "UI_ACTIVITY_CRYSTALLINK_END_NORMAL_NUM": {
+        "nameTextMapHash": 1535135607
+    },
+    "UI_ACTIVITY_CRYSTALLINK_END_SCORE_NAME": {
+        "nameTextMapHash": 3709860741
+    },
+    "UI_ACTIVITY_CRYSTALLINK_END_SUCCESS_TITLE": {
+        "nameTextMapHash": 2351996853
+    },
+    "UI_ACTIVITY_CRYSTALLINK_ENVIRONMENT_TITLE": {
+        "nameTextMapHash": 531752313
+    },
+    "UI_ACTIVITY_CRYSTALLINK_HANDLE_RESONANCE": {
+        "nameTextMapHash": 3338859555
+    },
+    "UI_ACTIVITY_CRYSTALLINK_HANDLE_RESONANCE_CANCEL": {
+        "nameTextMapHash": 650202241
+    },
+    "UI_ACTIVITY_CRYSTALLINK_INSIDE_CRYSTAL_RESULT": {
+        "nameTextMapHash": 998929404
+    },
+    "UI_ACTIVITY_CRYSTALLINK_INSIDE_ENTHUSIASM_MATH_DESC": {
+        "nameTextMapHash": 2107788816
+    },
+    "UI_ACTIVITY_CRYSTALLINK_INSIDE_ENTHUSIASM_RESULT": {
+        "nameTextMapHash": 2706982773
+    },
+    "UI_ACTIVITY_CRYSTALLINK_INSIDE_EXIT_DESC": {
+        "nameTextMapHash": 3775808563
+    },
+    "UI_ACTIVITY_CRYSTALLINK_INSIDE_EXIT_NO": {
+        "nameTextMapHash": 3025957731
+    },
+    "UI_ACTIVITY_CRYSTALLINK_INSIDE_EXIT_YES": {
+        "nameTextMapHash": 3528193923
+    },
+    "UI_ACTIVITY_CRYSTALLINK_INSIDE_REMINDER_TIPS": {
+        "nameTextMapHash": 3132367730
+    },
+    "UI_ACTIVITY_CRYSTALLINK_INSIDE_ROOM1_TITLE": {
+        "nameTextMapHash": 1900667360
+    },
+    "UI_ACTIVITY_CRYSTALLINK_INSIDE_ROOM2_TITLE": {
+        "nameTextMapHash": 587029432
+    },
+    "UI_ACTIVITY_CRYSTALLINK_INSIDE_ROOM_SHOW": {
+        "nameTextMapHash": 172531491
+    },
+    "UI_ACTIVITY_CRYSTALLINK_INSIDE_SCORE_SHOW": {
+        "nameTextMapHash": 930945167
+    },
+    "UI_ACTIVITY_CRYSTALLINK_INSIDE_SWITCH_ROOM": {
+        "nameTextMapHash": 1883784210
+    },
+    "UI_ACTIVITY_CRYSTALLINK_LEVEL_RECORD": {
+        "nameTextMapHash": 1692120587
+    },
+    "UI_ACTIVITY_CRYSTALLINK_LEVEL_RESONANCE_NULL": {
+        "nameTextMapHash": 1804452012
+    },
+    "UI_ACTIVITY_CRYSTALLINK_MONSTER_DETAIL_DESC": {
+        "nameTextMapHash": 831704488
+    },
+    "UI_ACTIVITY_CRYSTALLINK_MONSTER_DETAIL_SCORE": {
+        "nameTextMapHash": 1323328808
+    },
+    "UI_ACTIVITY_CRYSTALLINK_MONSTER_LEVEL": {
+        "nameTextMapHash": 3558864929
+    },
+    "UI_ACTIVITY_CRYSTALLINK_MONSTER_PREVIEW": {
+        "nameTextMapHash": 1586724161
+    },
+    "UI_ACTIVITY_CRYSTALLINK_NO_FULL_RESONANCE_TIPS": {
+        "nameTextMapHash": 2534537982
+    },
+    "UI_ACTIVITY_CRYSTALLINK_NO_RESONANCE": {
+        "nameTextMapHash": 1118752309
+    },
+    "UI_ACTIVITY_CRYSTALLINK_OVERLAY_RULE": {
+        "nameTextMapHash": 3135508902
+    },
+    "UI_ACTIVITY_CRYSTALLINK_RESET": {
+        "nameTextMapHash": 2822995477
+    },
+    "UI_ACTIVITY_CRYSTALLINK_RESET_CONFIRM_TIPS": {
+        "nameTextMapHash": 4236779698
+    },
+    "UI_ACTIVITY_CRYSTALLINK_RESONANCE": {
+        "nameTextMapHash": 2533337909
+    },
+    "UI_ACTIVITY_CRYSTALLINK_RESONANCE_NUMBER": {
+        "nameTextMapHash": 4266099049
+    },
+    "UI_ACTIVITY_CRYSTALLINK_RESONANCE_PAGE_TITLE": {
+        "nameTextMapHash": 1760196219
+    },
+    "UI_ACTIVITY_CRYSTALLINK_REWARD_HINT": {
+        "nameTextMapHash": 2198329975
+    },
+    "UI_ACTIVITY_CRYSTALLINK_ROOM_1": {
+        "nameTextMapHash": 1326899507
+    },
+    "UI_ACTIVITY_CRYSTALLINK_ROOM_2": {
+        "nameTextMapHash": 2637925555
+    },
     "UI_ACTIVITY_CURRENT_SCORE": {
         "nameTextMapHash": 2770843472
     },
     "UI_ACTIVITY_CWSM_GOTO": {
         "nameTextMapHash": 2989725311
     },
+    "UI_ACTIVITY_DEEP_DESC": {
+        "nameTextMapHash": 4181180086
+    },
+    "UI_ACTIVITY_DEEP_TITLE": {
+        "nameTextMapHash": 3206340166
+    },
     "UI_ACTIVITY_DELIVERY_ATTENTION": {
         "nameTextMapHash": 2852939631
     },
     "UI_ACTIVITY_DELIVERY_BUTTON_DELIVERY": {
         "nameTextMapHash": 3779337452
     },
     "UI_ACTIVITY_DELIVERY_BUTTON_GOTO_DELIVERY": {
@@ -18499,14 +17581,176 @@
     },
     "UI_ACTIVITY_ECHOSHELL_TITLE": {
         "nameTextMapHash": 3500844362
     },
     "UI_ACTIVITY_EFFIGYV4_PREQUEST": {
         "nameTextMapHash": 2982573029
     },
+    "UI_ACTIVITY_EFFIGYV5_AREA_HINT": {
+        "nameTextMapHash": 1997644367
+    },
+    "UI_ACTIVITY_EFFIGYV5_BESTRECORD": {
+        "nameTextMapHash": 655134155
+    },
+    "UI_ACTIVITY_EFFIGYV5_BOSSDESC": {
+        "nameTextMapHash": 1637933987
+    },
+    "UI_ACTIVITY_EFFIGYV5_BOSS_EFFECT": {
+        "nameTextMapHash": 1524949313
+    },
+    "UI_ACTIVITY_EFFIGYV5_CHALLENGE_INFO": {
+        "nameTextMapHash": 3148888654
+    },
+    "UI_ACTIVITY_EFFIGYV5_CHALLENGE_START": {
+        "nameTextMapHash": 2843462126
+    },
+    "UI_ACTIVITY_EFFIGYV5_CHARA_HINT": {
+        "nameTextMapHash": 1548780482
+    },
+    "UI_ACTIVITY_EFFIGYV5_CONFIRM_SUPPORTCHANGE": {
+        "nameTextMapHash": 1487210656
+    },
+    "UI_ACTIVITY_EFFIGYV5_COPPER": {
+        "nameTextMapHash": 1552973347
+    },
+    "UI_ACTIVITY_EFFIGYV5_EASY": {
+        "nameTextMapHash": 43077667
+    },
+    "UI_ACTIVITY_EFFIGYV5_END_QUEST": {
+        "nameTextMapHash": 2068307348
+    },
+    "UI_ACTIVITY_EFFIGYV5_END_QUEST_FINISHED": {
+        "nameTextMapHash": 2761303944
+    },
+    "UI_ACTIVITY_EFFIGYV5_ENTER_MULTI": {
+        "nameTextMapHash": 2299542729
+    },
+    "UI_ACTIVITY_EFFIGYV5_ENTER_SINGLE": {
+        "nameTextMapHash": 776364145
+    },
+    "UI_ACTIVITY_EFFIGYV5_GIVEUP_TIPS": {
+        "nameTextMapHash": 773293453
+    },
+    "UI_ACTIVITY_EFFIGYV5_GOLD": {
+        "nameTextMapHash": 1513405619
+    },
+    "UI_ACTIVITY_EFFIGYV5_HARD": {
+        "nameTextMapHash": 1019380603
+    },
+    "UI_ACTIVITY_EFFIGYV5_LEVELDESC": {
+        "nameTextMapHash": 3749390475
+    },
+    "UI_ACTIVITY_EFFIGYV5_LOSE_HINT": {
+        "nameTextMapHash": 2195862450
+    },
+    "UI_ACTIVITY_EFFIGYV5_MAP_BANNED": {
+        "nameTextMapHash": 3857459532
+    },
+    "UI_ACTIVITY_EFFIGYV5_MONSTERHP": {
+        "nameTextMapHash": 4119393555
+    },
+    "UI_ACTIVITY_EFFIGYV5_MONSTERLEVEL": {
+        "nameTextMapHash": 3931949707
+    },
+    "UI_ACTIVITY_EFFIGYV5_NEXTSTEP": {
+        "nameTextMapHash": 2114419
+    },
+    "UI_ACTIVITY_EFFIGYV5_NORECORD": {
+        "nameTextMapHash": 3166859539
+    },
+    "UI_ACTIVITY_EFFIGYV5_NORMAL": {
+        "nameTextMapHash": 1303489603
+    },
+    "UI_ACTIVITY_EFFIGYV5_NUMLIMIT": {
+        "nameTextMapHash": 1835762803
+    },
+    "UI_ACTIVITY_EFFIGYV5_ONLINE_EXIT_BAN": {
+        "nameTextMapHash": 2127289915
+    },
+    "UI_ACTIVITY_EFFIGYV5_PLATIUM": {
+        "nameTextMapHash": 2269257411
+    },
+    "UI_ACTIVITY_EFFIGYV5_QUESTLIMIT": {
+        "nameTextMapHash": 926566171
+    },
+    "UI_ACTIVITY_EFFIGYV5_QUIT_HINT": {
+        "nameTextMapHash": 2597989991
+    },
+    "UI_ACTIVITY_EFFIGYV5_REVIVE_TIMELIMIT": {
+        "nameTextMapHash": 1605948836
+    },
+    "UI_ACTIVITY_EFFIGYV5_REVIVE_TIPS": {
+        "nameTextMapHash": 3612706052
+    },
+    "UI_ACTIVITY_EFFIGYV5_REWARDLIST": {
+        "nameTextMapHash": 512382291
+    },
+    "UI_ACTIVITY_EFFIGYV5_REWARD_HINT": {
+        "nameTextMapHash": 1395901105
+    },
+    "UI_ACTIVITY_EFFIGYV5_SILVER": {
+        "nameTextMapHash": 3734548515
+    },
+    "UI_ACTIVITY_EFFIGYV5_SUPPORTCHANGE": {
+        "nameTextMapHash": 2115805243
+    },
+    "UI_ACTIVITY_EFFIGYV5_SUPPORTHINT": {
+        "nameTextMapHash": 2745979675
+    },
+    "UI_ACTIVITY_EFFIGYV5_SUPPORTINFO": {
+        "nameTextMapHash": 2632695555
+    },
+    "UI_ACTIVITY_EFFIGYV5_SUPPORTNUM": {
+        "nameTextMapHash": 1282726475
+    },
+    "UI_ACTIVITY_EFFIGYV5_SUPPORT_EMPTY": {
+        "nameTextMapHash": 1201241815
+    },
+    "UI_ACTIVITY_EFFIGYV5_SUPPORT_LIMIT": {
+        "nameTextMapHash": 2994160167
+    },
+    "UI_ACTIVITY_EFFIGYV5_SUPPORT_SAVE": {
+        "nameTextMapHash": 741345775
+    },
+    "UI_ACTIVITY_EFFIGYV5_SUPPORT_SELECTED": {
+        "nameTextMapHash": 2096744895
+    },
+    "UI_ACTIVITY_EFFIGYV5_TALK_GEAR": {
+        "nameTextMapHash": 1908068882
+    },
+    "UI_ACTIVITY_EFFIGYV5_TARGETDESC": {
+        "nameTextMapHash": 2415215203
+    },
+    "UI_ACTIVITY_EFFIGYV5_TARGET_EASY": {
+        "nameTextMapHash": 2400584901
+    },
+    "UI_ACTIVITY_EFFIGYV5_TARGET_HARD": {
+        "nameTextMapHash": 4148050621
+    },
+    "UI_ACTIVITY_EFFIGYV5_TARGET_NORMAL": {
+        "nameTextMapHash": 49171573
+    },
+    "UI_ACTIVITY_EFFIGYV5_TEAMCHANGE": {
+        "nameTextMapHash": 2753007267
+    },
+    "UI_ACTIVITY_EFFIGYV5_TIMECOST": {
+        "nameTextMapHash": 3707378979
+    },
+    "UI_ACTIVITY_EFFIGYV5_TIPS_DESC": {
+        "nameTextMapHash": 1500137524
+    },
+    "UI_ACTIVITY_EFFIGYV5_TIPS_TITLE": {
+        "nameTextMapHash": 3481265204
+    },
+    "UI_ACTIVITY_EFFIGYV5_TITLE": {
+        "nameTextMapHash": 2267164819
+    },
+    "UI_ACTIVITY_EFFIGYV5_UNLOCK_LEVEL": {
+        "nameTextMapHash": 4099483087
+    },
     "UI_ACTIVITY_EFFIGY_FIRE_DESC": {
         "nameTextMapHash": 784557494
     },
     "UI_ACTIVITY_EFFIGY_FIRE_GO_TO_CHALLENGE": {
         "nameTextMapHash": 1451064100
     },
     "UI_ACTIVITY_EFFIGY_FIRE_GO_TO_MISSON": {
@@ -19414,20 +18658,221 @@
     },
     "UI_ACTIVITY_FORBID_CHAT_IN_GAME": {
         "nameTextMapHash": 183103
     },
     "UI_ACTIVITY_GET_RWARD": {
         "nameTextMapHash": 355572134
     },
+    "UI_ACTIVITY_GOLEM_CENTAUR_DESC": {
+        "nameTextMapHash": 4168448535
+    },
+    "UI_ACTIVITY_GOLEM_CENTAUR_REDBAR": {
+        "nameTextMapHash": 3931272639
+    },
+    "UI_ACTIVITY_GOLEM_CENTAUR_TITLE": {
+        "nameTextMapHash": 4035945679
+    },
+    "UI_ACTIVITY_GOLEM_CENTAUR_YELLOWBAR": {
+        "nameTextMapHash": 1419871295
+    },
     "UI_ACTIVITY_GOTO": {
         "nameTextMapHash": 705208720
     },
     "UI_ACTIVITY_GOTO_EXCHANGE": {
         "nameTextMapHash": 1583668540
     },
+    "UI_ACTIVITY_GREATFESV2_AVATAR": {
+        "nameTextMapHash": 3783261426
+    },
+    "UI_ACTIVITY_GREATFESV2_DECOCOLLECT_COLLECT_PROGRESS": {
+        "nameTextMapHash": 3332697343
+    },
+    "UI_ACTIVITY_GREATFESV2_DECOCOLLECT_COLLECT_PROGRESS_NUM": {
+        "nameTextMapHash": 3094990545
+    },
+    "UI_ACTIVITY_GREATFESV2_DECOCOLLECT_DEFEAT_PROGRESS": {
+        "nameTextMapHash": 2709612509
+    },
+    "UI_ACTIVITY_GREATFESV2_DECOCOLLECT_HINT": {
+        "nameTextMapHash": 2628019182
+    },
+    "UI_ACTIVITY_GREATFESV2_DECOCOLLECT_MAP": {
+        "nameTextMapHash": 957073710
+    },
+    "UI_ACTIVITY_GREATFESV2_DECOCOLLECT_PHOTO_NAME": {
+        "nameTextMapHash": 1742020
+    },
+    "UI_ACTIVITY_GREATFESV2_DECOCOLLECT_PHOTO_PROGRESS": {
+        "nameTextMapHash": 3994692484
+    },
+    "UI_ACTIVITY_GREATFESV2_INVITATION_CONTENT": {
+        "nameTextMapHash": 2405184571
+    },
+    "UI_ACTIVITY_GREATFESV2_INVITATION_CONTENT_ADD": {
+        "nameTextMapHash": 2096816195
+    },
+    "UI_ACTIVITY_GREATFESV2_INVITATION_CONTENT_BIG": {
+        "nameTextMapHash": 1180772971
+    },
+    "UI_ACTIVITY_GREATFESV2_INVITATION_TITLE": {
+        "nameTextMapHash": 2814404699
+    },
+    "UI_ACTIVITY_GREATFESV2_MAINPAGE_COMMUNITY": {
+        "nameTextMapHash": 390926471
+    },
+    "UI_ACTIVITY_GREATFESV2_MAINPAGE_EVENT": {
+        "nameTextMapHash": 3602408895
+    },
+    "UI_ACTIVITY_GREATFESV2_MAINPAGE_EVENT_DECOCOLLECT": {
+        "nameTextMapHash": 1584036252
+    },
+    "UI_ACTIVITY_GREATFESV2_MAINPAGE_EVENT_MUSICGAME": {
+        "nameTextMapHash": 2999184532
+    },
+    "UI_ACTIVITY_GREATFESV2_MAINPAGE_EVENT_PROGRESS": {
+        "nameTextMapHash": 2137018332
+    },
+    "UI_ACTIVITY_GREATFESV2_MAINPAGE_EVENT_QUESTLOCK": {
+        "nameTextMapHash": 3598194516
+    },
+    "UI_ACTIVITY_GREATFESV2_MAINPAGE_EVENT_SHEETRES": {
+        "nameTextMapHash": 799563764
+    },
+    "UI_ACTIVITY_GREATFESV2_MAINPAGE_EVENT_STAGEUPGRADE": {
+        "nameTextMapHash": 3391769804
+    },
+    "UI_ACTIVITY_GREATFESV2_MAINPAGE_EVENT_UPGRADEHINT": {
+        "nameTextMapHash": 1025364380
+    },
+    "UI_ACTIVITY_GREATFESV2_MAINPAGE_INVITATION": {
+        "nameTextMapHash": 1306142519
+    },
+    "UI_ACTIVITY_GREATFESV2_MAINPAGE_STORY": {
+        "nameTextMapHash": 3403545487
+    },
+    "UI_ACTIVITY_GREATFESV2_MAINPAGE_TOKEN": {
+        "nameTextMapHash": 528344887
+    },
+    "UI_ACTIVITY_GREATFESV2_MAPSMARK_DES": {
+        "nameTextMapHash": 4257648998
+    },
+    "UI_ACTIVITY_GREATFESV2_MAPSMARK_TITLE": {
+        "nameTextMapHash": 612264934
+    },
+    "UI_ACTIVITY_GREATFESV2_QUEST_LOCKED": {
+        "nameTextMapHash": 1233179423
+    },
+    "UI_ACTIVITY_GREATFESV2_SHEETRES_CHOOSE_JS": {
+        "nameTextMapHash": 3134117801
+    },
+    "UI_ACTIVITY_GREATFESV2_SHEETRES_COMPLETE": {
+        "nameTextMapHash": 2554445362
+    },
+    "UI_ACTIVITY_GREATFESV2_SHEETRES_COMPLETE_TIME": {
+        "nameTextMapHash": 217458509
+    },
+    "UI_ACTIVITY_GREATFESV2_SHEETRES_DES": {
+        "nameTextMapHash": 4148857266
+    },
+    "UI_ACTIVITY_GREATFESV2_SHEETRES_EXCHANGE_JS": {
+        "nameTextMapHash": 112134735
+    },
+    "UI_ACTIVITY_GREATFESV2_SHEETRES_FAIL": {
+        "nameTextMapHash": 1056269498
+    },
+    "UI_ACTIVITY_GREATFESV2_SHEETRES_ORIGINAL": {
+        "nameTextMapHash": 1954957602
+    },
+    "UI_ACTIVITY_GREATFESV2_SHEETRES_ORIGINAL_ING": {
+        "nameTextMapHash": 1581411515
+    },
+    "UI_ACTIVITY_GREATFESV2_SHEETRES_PLAY_JS": {
+        "nameTextMapHash": 2458911315
+    },
+    "UI_ACTIVITY_GREATFESV2_SHEETRES_QUITHINT": {
+        "nameTextMapHash": 3669739266
+    },
+    "UI_ACTIVITY_GREATFESV2_SHEETRES_RECOMMAND": {
+        "nameTextMapHash": 4062582746
+    },
+    "UI_ACTIVITY_GREATFESV2_SHEETRES_RESTORE": {
+        "nameTextMapHash": 3669791938
+    },
+    "UI_ACTIVITY_GREATFESV2_SHEETRES_RESTOREING": {
+        "nameTextMapHash": 1333103066
+    },
+    "UI_ACTIVITY_GREATFESV2_SHEETRES_TITLE": {
+        "nameTextMapHash": 1563336210
+    },
+    "UI_ACTIVITY_GREATFESV2_SHEETRES_TRYING": {
+        "nameTextMapHash": 1202592170
+    },
+    "UI_ACTIVITY_GREATFESV2_SHEETRES_TRYSECTION": {
+        "nameTextMapHash": 533931386
+    },
+    "UI_ACTIVITY_GREATFESV2_STAGE_BAN_GOTO": {
+        "nameTextMapHash": 491069038
+    },
+    "UI_ACTIVITY_GREATFESV2_STAGE_COMPLETENESS": {
+        "nameTextMapHash": 4212947261
+    },
+    "UI_ACTIVITY_GREATFESV2_STAGE_DESC": {
+        "nameTextMapHash": 450522989
+    },
+    "UI_ACTIVITY_GREATFESV2_STAGE_EVENTLOCKED": {
+        "nameTextMapHash": 2309764869
+    },
+    "UI_ACTIVITY_GREATFESV2_STAGE_GONPC": {
+        "nameTextMapHash": 3453567621
+    },
+    "UI_ACTIVITY_GREATFESV2_STAGE_LIGHTS_SWITCHCOLOR": {
+        "nameTextMapHash": 1674999079
+    },
+    "UI_ACTIVITY_GREATFESV2_STAGE_LIGHTS_SWITCHPOS": {
+        "nameTextMapHash": 3034062447
+    },
+    "UI_ACTIVITY_GREATFESV2_STAGE_REWARDREVIEW": {
+        "nameTextMapHash": 593797837
+    },
+    "UI_ACTIVITY_GREATFESV2_STAGE_TITLE": {
+        "nameTextMapHash": 2126810805
+    },
+    "UI_ACTIVITY_GREATFESV2_STAGE_UPGRADE": {
+        "nameTextMapHash": 2305197029
+    },
+    "UI_ACTIVITY_GREATFESV2_STAGE_UPGRADE_AVAILABLE": {
+        "nameTextMapHash": 4233103355
+    },
+    "UI_ACTIVITY_GREATFESV2_TOKEN": {
+        "nameTextMapHash": 4176035394
+    },
+    "UI_ACTIVITY_GREATFESV2_TOKEN_TIPS": {
+        "nameTextMapHash": 3109767181
+    },
+    "UI_ACTIVITY_GUIDE_SHEETRESTORE_CHOOSE": {
+        "nameTextMapHash": 2890119978
+    },
+    "UI_ACTIVITY_GUIDE_SHEETRESTORE_EXCHANGENOTE": {
+        "nameTextMapHash": 4196141298
+    },
+    "UI_ACTIVITY_GUIDE_SHEETRESTORE_HELP": {
+        "nameTextMapHash": 618798050
+    },
+    "UI_ACTIVITY_GUIDE_SHEETRESTORE_HELP_COMFIRM": {
+        "nameTextMapHash": 3841068393
+    },
+    "UI_ACTIVITY_GUIDE_SHEETRESTORE_HELP_COMPLETE": {
+        "nameTextMapHash": 2391011745
+    },
+    "UI_ACTIVITY_GUIDE_SHEETRESTORE_HELP_HOLD": {
+        "nameTextMapHash": 3352404121
+    },
+    "UI_ACTIVITY_GUIDE_SHEETRESTORE_MODE2": {
+        "nameTextMapHash": 3870443674
+    },
     "UI_ACTIVITY_Gargoyle_Fafnir_GOTO": {
         "nameTextMapHash": 76895914
     },
     "UI_ACTIVITY_HACHI_BATTLE_TITLE": {
         "nameTextMapHash": 2912670669
     },
     "UI_ACTIVITY_HACHI_ITEM_NAME": {
@@ -19603,14 +19048,104 @@
     },
     "UI_ACTIVITY_HIDE_AND_SEEK_TIPS": {
         "nameTextMapHash": 2439437960
     },
     "UI_ACTIVITY_HIDE_AND_SEEK_TUTORIAL": {
         "nameTextMapHash": 2013613696
     },
+    "UI_ACTIVITY_HIDE_AND_SEEK_V4_CATCH": {
+        "nameTextMapHash": 1589891405
+    },
+    "UI_ACTIVITY_HIDE_AND_SEEK_V4_CONTENT": {
+        "nameTextMapHash": 1234637869
+    },
+    "UI_ACTIVITY_HIDE_AND_SEEK_V4_CONTINUE": {
+        "nameTextMapHash": 990806725
+    },
+    "UI_ACTIVITY_HIDE_AND_SEEK_V4_DESC": {
+        "nameTextMapHash": 3560884389
+    },
+    "UI_ACTIVITY_HIDE_AND_SEEK_V4_DRAFTPLAY": {
+        "nameTextMapHash": 3885508845
+    },
+    "UI_ACTIVITY_HIDE_AND_SEEK_V4_DRAFT_TIPS": {
+        "nameTextMapHash": 1118047072
+    },
+    "UI_ACTIVITY_HIDE_AND_SEEK_V4_GHOST_REMINDER_DESC": {
+        "nameTextMapHash": 3062637048
+    },
+    "UI_ACTIVITY_HIDE_AND_SEEK_V4_GHOST_REMINDER_TITLE": {
+        "nameTextMapHash": 3646377960
+    },
+    "UI_ACTIVITY_HIDE_AND_SEEK_V4_INVITE_CONFIRM": {
+        "nameTextMapHash": 533838751
+    },
+    "UI_ACTIVITY_HIDE_AND_SEEK_V4_KILL": {
+        "nameTextMapHash": 4179979189
+    },
+    "UI_ACTIVITY_HIDE_AND_SEEK_V4_LIMIT_WARNING": {
+        "nameTextMapHash": 575812642
+    },
+    "UI_ACTIVITY_HIDE_AND_SEEK_V4_MULTIPLAY": {
+        "nameTextMapHash": 4117973477
+    },
+    "UI_ACTIVITY_HIDE_AND_SEEK_V4_MULTIPLAYER": {
+        "nameTextMapHash": 3590449925
+    },
+    "UI_ACTIVITY_HIDE_AND_SEEK_V4_MULTIPLAY_TIPS": {
+        "nameTextMapHash": 1901631007
+    },
+    "UI_ACTIVITY_HIDE_AND_SEEK_V4_MULTI_WARNING": {
+        "nameTextMapHash": 1571584354
+    },
+    "UI_ACTIVITY_HIDE_AND_SEEK_V4_NPC_TITLE": {
+        "nameTextMapHash": 3205305980
+    },
+    "UI_ACTIVITY_HIDE_AND_SEEK_V4_QUIT_DRAFT_DESC": {
+        "nameTextMapHash": 153300281
+    },
+    "UI_ACTIVITY_HIDE_AND_SEEK_V4_QUIT_DRAFT_TITLE": {
+        "nameTextMapHash": 1475428193
+    },
+    "UI_ACTIVITY_HIDE_AND_SEEK_V4_QUIT_MATCH_DESC": {
+        "nameTextMapHash": 202674240
+    },
+    "UI_ACTIVITY_HIDE_AND_SEEK_V4_QUIT_MATCH_TITLE": {
+        "nameTextMapHash": 617316032
+    },
+    "UI_ACTIVITY_HIDE_AND_SEEK_V4_RELEASE_TIME": {
+        "nameTextMapHash": 541126264
+    },
+    "UI_ACTIVITY_HIDE_AND_SEEK_V4_REPAIR": {
+        "nameTextMapHash": 3391895989
+    },
+    "UI_ACTIVITY_HIDE_AND_SEEK_V4_REPAIR_PROGRESS": {
+        "nameTextMapHash": 1134352072
+    },
+    "UI_ACTIVITY_HIDE_AND_SEEK_V4_RESCURE": {
+        "nameTextMapHash": 3832916573
+    },
+    "UI_ACTIVITY_HIDE_AND_SEEK_V4_REWARD_ACHIEVEMENT": {
+        "nameTextMapHash": 302255513
+    },
+    "UI_ACTIVITY_HIDE_AND_SEEK_V4_REWARD_SCORE": {
+        "nameTextMapHash": 1159253257
+    },
+    "UI_ACTIVITY_HIDE_AND_SEEK_V4_SCORELIMIT_TIPS": {
+        "nameTextMapHash": 3099842063
+    },
+    "UI_ACTIVITY_HIDE_AND_SEEK_V4_SCORELIMIT_WARNING": {
+        "nameTextMapHash": 916027791
+    },
+    "UI_ACTIVITY_HIDE_AND_SEEK_V4_SCORE_ACHIEVED": {
+        "nameTextMapHash": 1547830727
+    },
+    "UI_ACTIVITY_HIDE_AND_SEEK_V4_TITLE": {
+        "nameTextMapHash": 242044349
+    },
     "UI_ACTIVITY_HIDE_AND_SEEK_WARNING_PREPARED": {
         "nameTextMapHash": 4283446890
     },
     "UI_ACTIVITY_HIDE_AND_SEEK_WINNER_HIDER": {
         "nameTextMapHash": 2907954290
     },
     "UI_ACTIVITY_HIDE_AND_SEEK_WINNER_SEEKER": {
@@ -22135,122 +21670,14 @@
     },
     "UI_ACTIVITY_SIGNIN_TABNAME_1001": {
         "nameTextMapHash": 643898299
     },
     "UI_ACTIVITY_SIGNIN_TABNAME_1002": {
         "nameTextMapHash": 86487771
     },
-    "UI_ACTIVITY_SLIMECANNON_COMBO": {
-        "nameTextMapHash": 1917326769
-    },
-    "UI_ACTIVITY_SLIMECANNON_CONTINUE": {
-        "nameTextMapHash": 1673071713
-    },
-    "UI_ACTIVITY_SLIMECANNON_COUNTDOWN": {
-        "nameTextMapHash": 3125845753
-    },
-    "UI_ACTIVITY_SLIMECANNON_ENDEXIT": {
-        "nameTextMapHash": 216410281
-    },
-    "UI_ACTIVITY_SLIMECANNON_ENDQUEST": {
-        "nameTextMapHash": 2506457577
-    },
-    "UI_ACTIVITY_SLIMECANNON_ENDRESTART": {
-        "nameTextMapHash": 44684953
-    },
-    "UI_ACTIVITY_SLIMECANNON_ENDSCORE": {
-        "nameTextMapHash": 484651073
-    },
-    "UI_ACTIVITY_SLIMECANNON_ENDSELECT": {
-        "nameTextMapHash": 522717649
-    },
-    "UI_ACTIVITY_SLIMECANNON_EXIT": {
-        "nameTextMapHash": 2164402529
-    },
-    "UI_ACTIVITY_SLIMECANNON_EXITTIPS": {
-        "nameTextMapHash": 429458449
-    },
-    "UI_ACTIVITY_SLIMECANNON_INGAMESCORE": {
-        "nameTextMapHash": 4196138145
-    },
-    "UI_ACTIVITY_SLIMECANNON_LOCK_TIPS": {
-        "nameTextMapHash": 918540446
-    },
-    "UI_ACTIVITY_SLIMECANNON_MELT": {
-        "nameTextMapHash": 4143020625
-    },
-    "UI_ACTIVITY_SLIMECANNON_NEXTBULLET": {
-        "nameTextMapHash": 2738566633
-    },
-    "UI_ACTIVITY_SLIMECANNON_NOTOPSCORE": {
-        "nameTextMapHash": 3837132673
-    },
-    "UI_ACTIVITY_SLIMECANNON_OBJTITLE": {
-        "nameTextMapHash": 1275247689
-    },
-    "UI_ACTIVITY_SLIMECANNON_OVERLOAD": {
-        "nameTextMapHash": 1149045881
-    },
-    "UI_ACTIVITY_SLIMECANNON_QUESTDONETIPS": {
-        "nameTextMapHash": 3178182753
-    },
-    "UI_ACTIVITY_SLIMECANNON_RECORD01": {
-        "nameTextMapHash": 1056482113
-    },
-    "UI_ACTIVITY_SLIMECANNON_RECORD02": {
-        "nameTextMapHash": 3483724633
-    },
-    "UI_ACTIVITY_SLIMECANNON_RECORD03": {
-        "nameTextMapHash": 1072425737
-    },
-    "UI_ACTIVITY_SLIMECANNON_RESTART": {
-        "nameTextMapHash": 1382055993
-    },
-    "UI_ACTIVITY_SLIMECANNON_REWARDTITLE": {
-        "nameTextMapHash": 3353278849
-    },
-    "UI_ACTIVITY_SLIMECANNON_SCORELEVEL": {
-        "nameTextMapHash": 1098266305
-    },
-    "UI_ACTIVITY_SLIMECANNON_STAGELEVEL": {
-        "nameTextMapHash": 1516664113
-    },
-    "UI_ACTIVITY_SLIMECANNON_STAGELOCK": {
-        "nameTextMapHash": 3109245937
-    },
-    "UI_ACTIVITY_SLIMECANNON_START": {
-        "nameTextMapHash": 25343361
-    },
-    "UI_ACTIVITY_SLIMECANNON_STARTTIPS": {
-        "nameTextMapHash": 2923980185
-    },
-    "UI_ACTIVITY_SLIMECANNON_SUCCEED": {
-        "nameTextMapHash": 2686730433
-    },
-    "UI_ACTIVITY_SLIMECANNON_SUPERCONDUCT": {
-        "nameTextMapHash": 1548535665
-    },
-    "UI_ACTIVITY_SLIMECANNON_TITLE": {
-        "nameTextMapHash": 1740925465
-    },
-    "UI_ACTIVITY_SLIMECANNON_TOPSCORE": {
-        "nameTextMapHash": 1211108505
-    },
-    "UI_ACTIVITY_SLIMECANNON_TUTORIAL1": {
-        "nameTextMapHash": 2822265537
-    },
-    "UI_ACTIVITY_SLIMECANNON_TUTORIAL2": {
-        "nameTextMapHash": 1152467785
-    },
-    "UI_ACTIVITY_SLIMECANNON_TUTORIAL3": {
-        "nameTextMapHash": 1331950273
-    },
-    "UI_ACTIVITY_SLIMECANNON_TUTORIALTITLE": {
-        "nameTextMapHash": 1243599433
-    },
     "UI_ACTIVITY_STAGE_LOCK": {
         "nameTextMapHash": 2117355951
     },
     "UI_ACTIVITY_STAGE_UNLOCK_TIPS": {
         "nameTextMapHash": 4057832592
     },
     "UI_ACTIVITY_STARTFAILED_ENDED": {
@@ -24751,14 +24178,17 @@
     },
     "UI_ADVENTURE_INVESTIGATION_PROBABILITY_REWARD": {
         "nameTextMapHash": 2800108873
     },
     "UI_ADVENTURE_INVESTIGATION_PROGRESS": {
         "nameTextMapHash": 877088907
     },
+    "UI_ADVENTURE_INVESTIGATION_RANK_UNLOCK": {
+        "nameTextMapHash": 3521339862
+    },
     "UI_ADVENTURE_INVESTIGATION_REBORN": {
         "nameTextMapHash": 1392318267
     },
     "UI_ADVENTURE_INVESTIGATION_REBORN_TIME": {
         "nameTextMapHash": 3573739655
     },
     "UI_ADVENTURE_INVESTIGATION_REWARD": {
@@ -24940,14 +24370,74 @@
     },
     "UI_AVATAR_TITLE": {
         "nameTextMapHash": 2022941172
     },
     "UI_AVATAR_WINGS": {
         "nameTextMapHash": 257286060
     },
+    "UI_Activity_CrystalLinkThird_Arrange_Avartar_NotFull": {
+        "nameTextMapHash": 1631429349
+    },
+    "UI_Activity_CrystalLinkThird_Arrange_Avartar_Room1": {
+        "nameTextMapHash": 3607263333
+    },
+    "UI_Activity_CrystalLinkThird_Arrange_Avartar_Room2": {
+        "nameTextMapHash": 2643095981
+    },
+    "UI_Activity_CrystalLinkThird_Continue_Arrange": {
+        "nameTextMapHash": 2158080433
+    },
+    "UI_Activity_CrystalLinkThird_DungeonEntry": {
+        "nameTextMapHash": 25952426
+    },
+    "UI_Activity_CrystalLinkThird_Exit_Confirm": {
+        "nameTextMapHash": 3368011605
+    },
+    "UI_Activity_CrystalLinkThird_Mark_Desc": {
+        "nameTextMapHash": 2290734633
+    },
+    "UI_Activity_CrystalLinkThird_Mark_Title": {
+        "nameTextMapHash": 1657683729
+    },
+    "UI_Activity_CrystalLinkThird_MaxScore": {
+        "nameTextMapHash": 3015217826
+    },
+    "UI_Activity_CrystalLinkThird_ModifyLink": {
+        "nameTextMapHash": 1450595098
+    },
+    "UI_Activity_CrystalLinkThird_MoreDamage": {
+        "nameTextMapHash": 2793886018
+    },
+    "UI_Activity_CrystalLinkThird_MuchMoreDamage": {
+        "nameTextMapHash": 315935970
+    },
+    "UI_Activity_CrystalLinkThird_OnlineBan_Fight_Hint": {
+        "nameTextMapHash": 2194024494
+    },
+    "UI_Activity_CrystalLinkThird_OnlineBan_GoTo_Hint": {
+        "nameTextMapHash": 3059908984
+    },
+    "UI_Activity_CrystalLinkThird_ResetLink_Hint": {
+        "nameTextMapHash": 2631448997
+    },
+    "UI_Activity_CrystalLinkThird_SomeDamage": {
+        "nameTextMapHash": 4237801778
+    },
+    "UI_Activity_CrystalLinkThird_TimeOut_Hint": {
+        "nameTextMapHash": 3663731689
+    },
+    "UI_Activity_CrystalLinkThird_UnlockQuestButton": {
+        "nameTextMapHash": 1061051922
+    },
+    "UI_Activity_CrystalLinkThird_WatcherList": {
+        "nameTextMapHash": 3478349538
+    },
+    "UI_BAN_APPEAL": {
+        "nameTextMapHash": 2303801132
+    },
     "UI_BAN_MAP_TIPS": {
         "nameTextMapHash": 3349593108
     },
     "UI_BATTLEPASS_PAY_TIME_COUNT_DOWN": {
         "nameTextMapHash": 1464495449
     },
     "UI_BATTLEPASS_PAY_TIME_END": {
@@ -25867,14 +25357,17 @@
     },
     "UI_BUTTON_CHANGE": {
         "nameTextMapHash": 2309567037
     },
     "UI_BUTTON_CHECK": {
         "nameTextMapHash": 4095226093
     },
+    "UI_BUTTON_CHECKDETAIL": {
+        "nameTextMapHash": 1387616997
+    },
     "UI_BUTTON_CLEAR": {
         "nameTextMapHash": 2895639485
     },
     "UI_BUTTON_CONFIRM_SCREEN": {
         "nameTextMapHash": 1518533022
     },
     "UI_BUTTON_CONVERSION": {
@@ -26110,14 +25603,23 @@
     },
     "UI_Bargain_Warn_02": {
         "nameTextMapHash": 3289724551
     },
     "UI_Bargain_Warn_03": {
         "nameTextMapHash": 1872180647
     },
+    "UI_Blackscreen_RemusArena": {
+        "nameTextMapHash": 2710579089
+    },
+    "UI_Blackscreen_RestCat": {
+        "nameTextMapHash": 1029066617
+    },
+    "UI_Blackscreen_RestStone": {
+        "nameTextMapHash": 2204759137
+    },
     "UI_CATALOG_ARANARA_MUSICGET": {
         "nameTextMapHash": 223139789
     },
     "UI_CATALOG_ARANARA_QUEST_GOTO": {
         "nameTextMapHash": 1054070017
     },
     "UI_CATALOG_ARANARA_QUEST_GROUPBATTLE": {
@@ -26431,14 +25933,17 @@
     },
     "UI_CODEX_ANIMAL_ROTATE": {
         "nameTextMapHash": 2300880334
     },
     "UI_CODEX_ANIMAL_ZOOM": {
         "nameTextMapHash": 512236110
     },
+    "UI_CODEX_AREAPUAHTIPS": {
+        "nameTextMapHash": 3821249644
+    },
     "UI_CODEX_BIOS": {
         "nameTextMapHash": 1897268740
     },
     "UI_CODEX_BOOKS": {
         "nameTextMapHash": 3560796780
     },
     "UI_CODEX_BOOK_ALL_COLLECTED": {
@@ -27331,20 +26836,26 @@
     },
     "UI_DUNGEONENTRY_RECOMMEND_TIPS_032": {
         "nameTextMapHash": 2878144290
     },
     "UI_DUNGEONENTRY_RECOMMEND_TIPS_033": {
         "nameTextMapHash": 1108716986
     },
+    "UI_DUNGEONENTRY_RECOMMEND_TIPS_034": {
+        "nameTextMapHash": 1479498490
+    },
     "UI_DUNGEONENTRY_RECOMMEND_TIPS_TITLE": {
         "nameTextMapHash": 31128490
     },
     "UI_DUNGEONENTRY_REWARD_KEY_COUNT": {
         "nameTextMapHash": 3189212404
     },
+    "UI_DUNGEONENTRY_REWARD_KEY_COUNT_SPECIAL": {
+        "nameTextMapHash": 3954932562
+    },
     "UI_DUNGEONENTRY_SINGLE_MULTIPLAYER": {
         "nameTextMapHash": 857795135
     },
     "UI_DUNGEONENTRY_SINGLE_PLAYER_ONLY": {
         "nameTextMapHash": 2862110381
     },
     "UI_DUNGEONENTRY_START_MULTIPLAYER": {
@@ -27406,20 +26917,29 @@
     },
     "UI_DUNGEON_ENTRY_1109": {
         "nameTextMapHash": 1111225651
     },
     "UI_DUNGEON_ENTRY_1142": {
         "nameTextMapHash": 1525986819
     },
+    "UI_DUNGEON_ENTRY_1151": {
+        "nameTextMapHash": 2072441131
+    },
     "UI_DUNGEON_ENTRY_1202": {
         "nameTextMapHash": 3024443467
     },
     "UI_DUNGEON_ENTRY_1207": {
         "nameTextMapHash": 4122575003
     },
+    "UI_DUNGEON_ENTRY_1209": {
+        "nameTextMapHash": 1117995683
+    },
+    "UI_DUNGEON_ENTRY_1241": {
+        "nameTextMapHash": 1746819179
+    },
     "UI_DUNGEON_ENTRY_20": {
         "nameTextMapHash": 1177628219
     },
     "UI_DUNGEON_ENTRY_22": {
         "nameTextMapHash": 3585043443
     },
     "UI_DUNGEON_ENTRY_221": {
@@ -27691,14 +27211,17 @@
     },
     "UI_DUNGEON_ENTRY_Baizhu": {
         "nameTextMapHash": 2647746467
     },
     "UI_DUNGEON_ENTRY_BlitzRush_Dungeon": {
         "nameTextMapHash": 2773855912
     },
+    "UI_DUNGEON_ENTRY_CRYSTALLINK": {
+        "nameTextMapHash": 1910987920
+    },
     "UI_DUNGEON_ENTRY_ChannellerSlab_Loop": {
         "nameTextMapHash": 3734572481
     },
     "UI_DUNGEON_ENTRY_ChannellerSlab_Loop2": {
         "nameTextMapHash": 258691977
     },
     "UI_DUNGEON_ENTRY_ChannellerSlab_Loop_V2": {
@@ -29242,14 +28765,17 @@
     },
     "UI_GACHA_SHOW_PANEL_A017_UP1_TITLE2": {
         "nameTextMapHash": 383635418
     },
     "UI_GACHA_SHOW_PANEL_A017_UP2_NAME": {
         "nameTextMapHash": 183836432
     },
+    "UI_GACHA_SHOW_PANEL_A0181_TITLE": {
+        "nameTextMapHash": 3265361806
+    },
     "UI_GACHA_SHOW_PANEL_A018_SUBTITLE": {
         "nameTextMapHash": 739651495
     },
     "UI_GACHA_SHOW_PANEL_A018_TITLE": {
         "nameTextMapHash": 937696679
     },
     "UI_GACHA_SHOW_PANEL_A018_UP1_NAME1": {
@@ -30919,14 +30445,20 @@
     },
     "UI_GCG_HISTORY_EFFECT_DAMAGE_KO": {
         "nameTextMapHash": 3655547037
     },
     "UI_GCG_HISTORY_EFFECT_DAMAGE_REACTION": {
         "nameTextMapHash": 1773441381
     },
+    "UI_GCG_HISTORY_EFFECT_DECKADDCARD_OPPO": {
+        "nameTextMapHash": 1276075529
+    },
+    "UI_GCG_HISTORY_EFFECT_DECKADDCARD_SELF": {
+        "nameTextMapHash": 2788994937
+    },
     "UI_GCG_HISTORY_EFFECT_DICE_OPPO": {
         "nameTextMapHash": 2185436139
     },
     "UI_GCG_HISTORY_EFFECT_DICE_RANDOM": {
         "nameTextMapHash": 3244476843
     },
     "UI_GCG_HISTORY_EFFECT_DICE_SELF": {
@@ -31009,14 +30541,20 @@
     },
     "UI_GCG_HISTORY_EFFECT_RETURNHAND_OPPO": {
         "nameTextMapHash": 3433629770
     },
     "UI_GCG_HISTORY_EFFECT_RETURNHAND_SELF": {
         "nameTextMapHash": 638384930
     },
+    "UI_GCG_HISTORY_EFFECT_SHUFFLE_OPPO": {
+        "nameTextMapHash": 337248541
+    },
+    "UI_GCG_HISTORY_EFFECT_SHUFFLE_SELF": {
+        "nameTextMapHash": 2220988941
+    },
     "UI_GCG_HISTORY_EFFECT_SPRITE_TAG": {
         "nameTextMapHash": 3215036734
     },
     "UI_GCG_HISTORY_EFFECT_STAGE": {
         "nameTextMapHash": 1527094397
     },
     "UI_GCG_HISTORY_EFFECT_SUMMON_OPPO": {
@@ -32590,23 +32128,38 @@
     },
     "UI_GENERALREWARD_TITLE_ASTERMID": {
         "nameTextMapHash": 3783476731
     },
     "UI_GENERALREWARD_UNCLAIMED": {
         "nameTextMapHash": 793620898
     },
+    "UI_GHOST_PAINTING_BOTH_CORRECT_HINT": {
+        "nameTextMapHash": 1334631149
+    },
+    "UI_GHOST_PAINTING_BOTH_WRONG": {
+        "nameTextMapHash": 981057553
+    },
+    "UI_GHOST_PAINTING_CAMERA_WRONG": {
+        "nameTextMapHash": 249063728
+    },
+    "UI_GHOST_PAINTING_PAINTING_WRONG": {
+        "nameTextMapHash": 455643689
+    },
     "UI_GODDESS_AREA_ELEMENT_ENHANCE": {
         "nameTextMapHash": 374461147
     },
     "UI_GODDESS_ENTRY_UNLOCK_CONDITION": {
         "nameTextMapHash": 3461060887
     },
     "UI_GODDESS_NO_ITEM": {
         "nameTextMapHash": 4137541427
     },
+    "UI_GOLDEN_HALL_EXIT_CONFIRM_DESC": {
+        "nameTextMapHash": 2209681226
+    },
     "UI_GUIDERATING_FAVOUR": {
         "nameTextMapHash": 4028093950
     },
     "UI_GUIDERATING_FEEDBACK": {
         "nameTextMapHash": 2593757710
     },
     "UI_GUIDERATING_MAINCONTENT": {
@@ -33721,14 +33274,32 @@
     },
     "UI_GadgetUI_70292014": {
         "nameTextMapHash": 3088685974
     },
     "UI_GadgetUI_70292059": {
         "nameTextMapHash": 3378535238
     },
+    "UI_GadgetUI_70330923": {
+        "nameTextMapHash": 405414134
+    },
+    "UI_GadgetUI_70330927": {
+        "nameTextMapHash": 2341196862
+    },
+    "UI_GadgetUI_70330968": {
+        "nameTextMapHash": 4168825518
+    },
+    "UI_GadgetUI_70330983": {
+        "nameTextMapHash": 177497390
+    },
+    "UI_GadgetUI_70330985": {
+        "nameTextMapHash": 367828510
+    },
+    "UI_GadgetUI_70330998": {
+        "nameTextMapHash": 3595509286
+    },
     "UI_H5_ACTIVITY_NAME": {
         "nameTextMapHash": 1612739398
     },
     "UI_H5_ACTIVITY_NONE": {
         "nameTextMapHash": 4039720118
     },
     "UI_HDR_SCREEN_SETUP_UI_TIPS": {
@@ -34531,14 +34102,20 @@
     },
     "UI_HOMEWORLD_CHANGEBGM_USE_CITY_BGM": {
         "nameTextMapHash": 860340951
     },
     "UI_HOMEWORLD_CHANGEBGM_USE_DESC": {
         "nameTextMapHash": 1976587481
     },
+    "UI_HOMEWORLD_CHANGEBGM_USE_ITEM_DESC": {
+        "nameTextMapHash": 2199112152
+    },
+    "UI_HOMEWORLD_CHANGEBGM_USE_ITEM_NUM": {
+        "nameTextMapHash": 879307112
+    },
     "UI_HOMEWORLD_CHANGE_MOUNTAIN_BUTTON": {
         "nameTextMapHash": 570266807
     },
     "UI_HOMEWORLD_CLEAR_ROOM": {
         "nameTextMapHash": 1188304269
     },
     "UI_HOMEWORLD_CLEAR_ROOM_DESC": {
@@ -35053,14 +34630,20 @@
     },
     "UI_HOMEWORLD_FASTGET_NEED": {
         "nameTextMapHash": 125869395
     },
     "UI_HOMEWORLD_FILTER_FURNITURE_CONFIRM_BUTTON": {
         "nameTextMapHash": 4216463320
     },
+    "UI_HOMEWORLD_FILTER_FURNITURE_DISCOUNT": {
+        "nameTextMapHash": 2952887528
+    },
+    "UI_HOMEWORLD_FILTER_FURNITURE_DISCOUNT_ABBR": {
+        "nameTextMapHash": 1203329554
+    },
     "UI_HOMEWORLD_FILTER_FURNITURE_NO_MAKE": {
         "nameTextMapHash": 2681697883
     },
     "UI_HOMEWORLD_FILTER_FURNITURE_NO_MAKE_ABBR": {
         "nameTextMapHash": 158760381
     },
     "UI_HOMEWORLD_FILTER_FURNITURE_NULL_TIPS": {
@@ -35152,14 +34735,38 @@
     },
     "UI_HOMEWORLD_FURNITURE_FREEZE": {
         "nameTextMapHash": 1893367406
     },
     "UI_HOMEWORLD_FURNITURE_FREEZE_SUITE": {
         "nameTextMapHash": 2677317121
     },
+    "UI_HOMEWORLD_FURNITURE_TIPS_EXANDIN": {
+        "nameTextMapHash": 1637488352
+    },
+    "UI_HOMEWORLD_FURNITURE_TIPS_EXTERIOR": {
+        "nameTextMapHash": 1262782192
+    },
+    "UI_HOMEWORLD_FURNITURE_TIPS_EXTERIOR_DRAWING": {
+        "nameTextMapHash": 665043929
+    },
+    "UI_HOMEWORLD_FURNITURE_TIPS_EXTERIOR_SUIT_DRAWING": {
+        "nameTextMapHash": 4130662510
+    },
+    "UI_HOMEWORLD_FURNITURE_TIPS_INTERIOR": {
+        "nameTextMapHash": 2098426096
+    },
+    "UI_HOMEWORLD_FURNITURE_TIPS_INTERIOR_DRAWING": {
+        "nameTextMapHash": 23822054
+    },
+    "UI_HOMEWORLD_FURNITURE_TIPS_INTERIOR_SUIT_DRAWING": {
+        "nameTextMapHash": 3894456772
+    },
+    "UI_HOMEWORLD_FURNITURE_TIPS_LEVEL_TYPE": {
+        "nameTextMapHash": 413503741
+    },
     "UI_HOMEWORLD_GIFT_A": {
         "nameTextMapHash": 760098185
     },
     "UI_HOMEWORLD_GIFT_B": {
         "nameTextMapHash": 2395384137
     },
     "UI_HOMEWORLD_GIFT_C": {
@@ -35338,14 +34945,17 @@
     },
     "UI_HOMEWORLD_MACHFISH_BUTTON": {
         "nameTextMapHash": 534950721
     },
     "UI_HOMEWORLD_MAGNET": {
         "nameTextMapHash": 3847607546
     },
+    "UI_HOMEWORLD_MAKE_FURNITURE_LIST_NUM_UP": {
+        "nameTextMapHash": 3890609969
+    },
     "UI_HOMEWORLD_MISC": {
         "nameTextMapHash": 4228014370
     },
     "UI_HOMEWORLD_MODULECHOOSE_CHANGE_BUTTON": {
         "nameTextMapHash": 2411476546
     },
     "UI_HOMEWORLD_MODULECHOOSE_CHANGE_DESC": {
@@ -35626,14 +35236,164 @@
     },
     "UI_HOMEWORLD_PS_EDIT_MODE_ROTATE": {
         "nameTextMapHash": 555560317
     },
     "UI_HOMEWORLD_PS_EDIT_MODE_ZOOM_OUT": {
         "nameTextMapHash": 3809640451
     },
+    "UI_HOMEWORLD_QUICK_BUY": {
+        "nameTextMapHash": 281521346
+    },
+    "UI_HOMEWORLD_QUICK_BUY_DESC": {
+        "nameTextMapHash": 2332357644
+    },
+    "UI_HOMEWORLD_QUICK_BUY_DESC1": {
+        "nameTextMapHash": 1242660532
+    },
+    "UI_HOMEWORLD_QUICK_BUY_FAIL_REMIND1": {
+        "nameTextMapHash": 1848004558
+    },
+    "UI_HOMEWORLD_QUICK_BUY_FAIL_REMIND2": {
+        "nameTextMapHash": 2737999694
+    },
+    "UI_HOMEWORLD_QUICK_BUY_PRICE": {
+        "nameTextMapHash": 615793348
+    },
+    "UI_HOMEWORLD_QUICK_BUY_TITLE": {
+        "nameTextMapHash": 2566156212
+    },
+    "UI_HOMEWORLD_QUICK_GETALL_DESC": {
+        "nameTextMapHash": 3887552827
+    },
+    "UI_HOMEWORLD_QUICK_GET_BLUEPRINT_DESC": {
+        "nameTextMapHash": 2620445093
+    },
+    "UI_HOMEWORLD_QUICK_GET_BLUEPRINT_TIPS": {
+        "nameTextMapHash": 2540533237
+    },
+    "UI_HOMEWORLD_QUICK_GET_BUTTON": {
+        "nameTextMapHash": 1577539724
+    },
+    "UI_HOMEWORLD_QUICK_GET_SUIT_DESC": {
+        "nameTextMapHash": 96111940
+    },
+    "UI_HOMEWORLD_QUICK_GET_SUIT_TIPS": {
+        "nameTextMapHash": 25816236
+    },
+    "UI_HOMEWORLD_QUICK_GET_TITLE": {
+        "nameTextMapHash": 3850595460
+    },
+    "UI_HOMEWORLD_QUICK_MAKE": {
+        "nameTextMapHash": 3081384338
+    },
+    "UI_HOMEWORLD_QUICK_MAKE_ADD_LIST": {
+        "nameTextMapHash": 1474670742
+    },
+    "UI_HOMEWORLD_QUICK_MAKE_ADD_LIST_DESC1": {
+        "nameTextMapHash": 2991245678
+    },
+    "UI_HOMEWORLD_QUICK_MAKE_ADD_LIST_DESC2": {
+        "nameTextMapHash": 4056607294
+    },
+    "UI_HOMEWORLD_QUICK_MAKE_ADD_LIST_DESC3": {
+        "nameTextMapHash": 3142890758
+    },
+    "UI_HOMEWORLD_QUICK_MAKE_ADD_LIST_EMPTY_REMIND": {
+        "nameTextMapHash": 162140270
+    },
+    "UI_HOMEWORLD_QUICK_MAKE_ADD_LIST_REMIND": {
+        "nameTextMapHash": 1160096182
+    },
+    "UI_HOMEWORLD_QUICK_MAKE_BLUEPRINT_DELETE_DESC": {
+        "nameTextMapHash": 3570582325
+    },
+    "UI_HOMEWORLD_QUICK_MAKE_BLUEPRINT_NAME": {
+        "nameTextMapHash": 2921259029
+    },
+    "UI_HOMEWORLD_QUICK_MAKE_BUY_EMPTY_DESC": {
+        "nameTextMapHash": 2626799417
+    },
+    "UI_HOMEWORLD_QUICK_MAKE_DELETE_LIST": {
+        "nameTextMapHash": 4074719982
+    },
+    "UI_HOMEWORLD_QUICK_MAKE_DELETE_LIST_DESC": {
+        "nameTextMapHash": 865716643
+    },
+    "UI_HOMEWORLD_QUICK_MAKE_DELETE_LIST_REMIND": {
+        "nameTextMapHash": 1504111835
+    },
+    "UI_HOMEWORLD_QUICK_MAKE_EMPTY_DESC": {
+        "nameTextMapHash": 3694141394
+    },
+    "UI_HOMEWORLD_QUICK_MAKE_EMPTY_DESC1": {
+        "nameTextMapHash": 1027298986
+    },
+    "UI_HOMEWORLD_QUICK_MAKE_GETALL_DESC": {
+        "nameTextMapHash": 729323274
+    },
+    "UI_HOMEWORLD_QUICK_MAKE_GET_ALL_BUTTON": {
+        "nameTextMapHash": 2796699810
+    },
+    "UI_HOMEWORLD_QUICK_MAKE_GET_ALL_REMIND": {
+        "nameTextMapHash": 302333770
+    },
+    "UI_HOMEWORLD_QUICK_MAKE_GET_ONE_BUTTON": {
+        "nameTextMapHash": 4004828467
+    },
+    "UI_HOMEWORLD_QUICK_MAKE_GET_ONE_DESC": {
+        "nameTextMapHash": 3383598803
+    },
+    "UI_HOMEWORLD_QUICK_MAKE_GET_ONE_PART_DESC": {
+        "nameTextMapHash": 3933252141
+    },
+    "UI_HOMEWORLD_QUICK_MAKE_GET_ONE_TITLE": {
+        "nameTextMapHash": 2777111427
+    },
+    "UI_HOMEWORLD_QUICK_MAKE_GET_PART_BUTTON": {
+        "nameTextMapHash": 3228573392
+    },
+    "UI_HOMEWORLD_QUICK_MAKE_LIST": {
+        "nameTextMapHash": 800487778
+    },
+    "UI_HOMEWORLD_QUICK_MAKE_LIST_ADDTO_BUTTON": {
+        "nameTextMapHash": 292014377
+    },
+    "UI_HOMEWORLD_QUICK_MAKE_LIST_ADDTO_DESC": {
+        "nameTextMapHash": 2874657113
+    },
+    "UI_HOMEWORLD_QUICK_MAKE_LIST_DELETE_BUTTON": {
+        "nameTextMapHash": 2916828088
+    },
+    "UI_HOMEWORLD_QUICK_MAKE_LIST_FURNITURE": {
+        "nameTextMapHash": 4101302002
+    },
+    "UI_HOMEWORLD_QUICK_MAKE_LIST_NEW": {
+        "nameTextMapHash": 2955232570
+    },
+    "UI_HOMEWORLD_QUICK_MAKE_QUEUE": {
+        "nameTextMapHash": 1570720634
+    },
+    "UI_HOMEWORLD_QUICK_MAKE_SUIT_NAME": {
+        "nameTextMapHash": 2988492682
+    },
+    "UI_HOMEWORLD_QUICK_MAKE_UNABLE_GET": {
+        "nameTextMapHash": 1565390934
+    },
+    "UI_HOMEWORLD_QUICK_MAKE_UNABLE_GET_DESC": {
+        "nameTextMapHash": 2869377394
+    },
+    "UI_HOMEWORLD_QUICK_MAKE_UNABLE_GET_NUM": {
+        "nameTextMapHash": 4068062698
+    },
+    "UI_HOMEWORLD_QUICK_MAKE_UNABLE_GET_TITLE": {
+        "nameTextMapHash": 137381034
+    },
+    "UI_HOMEWORLD_QUICK_MAKE_UNABLE_RECOVERY_DESC": {
+        "nameTextMapHash": 2455671614
+    },
     "UI_HOMEWORLD_RESET_CAMERA": {
         "nameTextMapHash": 3672773189
     },
     "UI_HOMEWORLD_ROCKERY_TIP": {
         "nameTextMapHash": 2424025919
     },
     "UI_HOMEWORLD_ROTATE": {
@@ -36064,14 +35824,20 @@
     },
     "UI_LONG_PRESS": {
         "nameTextMapHash": 4178599025
     },
     "UI_LUMEN_STONE_MANUAL_TITLE": {
         "nameTextMapHash": 164201649
     },
+    "UI_Level_RemusMural_Fail": {
+        "nameTextMapHash": 2178122189
+    },
+    "UI_Level_RemusMural_Success": {
+        "nameTextMapHash": 1845852445
+    },
     "UI_MAIL_CANCEL_STAR": {
         "nameTextMapHash": 1721229724
     },
     "UI_MAIL_DELETE_ALL_DESC": {
         "nameTextMapHash": 819015792
     },
     "UI_MAIL_DELETE_ALL_TITLE": {
@@ -36880,14 +36646,20 @@
     },
     "UI_MAPMARK_MarkTalk_DESC": {
         "nameTextMapHash": 941341683
     },
     "UI_MAPMARK_MarkTalk_TITLE": {
         "nameTextMapHash": 3427883915
     },
+    "UI_MAPMARK_MarkTempleOfSilence_Sumeru_DESC": {
+        "nameTextMapHash": 2258455746
+    },
+    "UI_MAPMARK_MarkTempleOfSilence_Sumeru_TITLE": {
+        "nameTextMapHash": 617560842
+    },
     "UI_MAPMARK_MarkTransPointLocked_DESC": {
         "nameTextMapHash": 214180711
     },
     "UI_MAPMARK_MarkTransPointLocked_TITLE": {
         "nameTextMapHash": 2520270535
     },
     "UI_MAPMARK_MarkTransPoint_DESC": {
@@ -37219,14 +36991,17 @@
     },
     "UI_MAP_AREA20_TITLE_2": {
         "nameTextMapHash": 2129188214
     },
     "UI_MAP_AREA20_TITLE_3": {
         "nameTextMapHash": 3459657686
     },
+    "UI_MAP_AREA20_TITLE_4": {
+        "nameTextMapHash": 4020953414
+    },
     "UI_MAP_AREA21_TITLE_1": {
         "nameTextMapHash": 1936055401
     },
     "UI_MAP_AREA21_TITLE_2": {
         "nameTextMapHash": 2813616473
     },
     "UI_MAP_AREA21_TITLE_3": {
@@ -37585,14 +37360,20 @@
     },
     "UI_MAP_AREA41_TITLE_8": {
         "nameTextMapHash": 135856925
     },
     "UI_MAP_AREA41_TITLE_9": {
         "nameTextMapHash": 3320238701
     },
+    "UI_MAP_AREA42_TITLE_1": {
+        "nameTextMapHash": 3121729972
+    },
+    "UI_MAP_AREA42_TITLE_2": {
+        "nameTextMapHash": 1477110460
+    },
     "UI_MAP_AREA47_TITLE_1": {
         "nameTextMapHash": 1162265720
     },
     "UI_MAP_AREA47_TITLE_2": {
         "nameTextMapHash": 3624137928
     },
     "UI_MAP_AREA4_TITLE_1": {
@@ -37627,14 +37408,41 @@
     },
     "UI_MAP_AREA5_TITLE_8": {
         "nameTextMapHash": 403584449
     },
     "UI_MAP_AREA5_TITLE_9": {
         "nameTextMapHash": 3589918329
     },
+    "UI_MAP_AREA600_TITLE_1": {
+        "nameTextMapHash": 3914501004
+    },
+    "UI_MAP_AREA600_TITLE_2": {
+        "nameTextMapHash": 2212562884
+    },
+    "UI_MAP_AREA600_TITLE_3": {
+        "nameTextMapHash": 2913691580
+    },
+    "UI_MAP_AREA600_TITLE_4": {
+        "nameTextMapHash": 2133249316
+    },
+    "UI_MAP_AREA600_TITLE_5": {
+        "nameTextMapHash": 1061088820
+    },
+    "UI_MAP_AREA600_TITLE_6": {
+        "nameTextMapHash": 3756117404
+    },
+    "UI_MAP_AREA600_TITLE_7": {
+        "nameTextMapHash": 3404393588
+    },
+    "UI_MAP_AREA600_TITLE_8": {
+        "nameTextMapHash": 1487171940
+    },
+    "UI_MAP_AREA600_TITLE_9": {
+        "nameTextMapHash": 14944484
+    },
     "UI_MAP_AREA6_TITLE_1": {
         "nameTextMapHash": 2582135861
     },
     "UI_MAP_AREA6_TITLE_2": {
         "nameTextMapHash": 47848653
     },
     "UI_MAP_AREA6_TITLE_3": {
@@ -37831,14 +37639,29 @@
     },
     "UI_MAP_City5_TITLE_38": {
         "nameTextMapHash": 1300722553
     },
     "UI_MAP_City5_TITLE_39": {
         "nameTextMapHash": 23191433
     },
+    "UI_MAP_City5_TITLE_42": {
+        "nameTextMapHash": 456094057
+    },
+    "UI_MAP_City5_TITLE_600": {
+        "nameTextMapHash": 1755242177
+    },
+    "UI_MAP_DAYEVENT_TIPNEW": {
+        "nameTextMapHash": 3539751821
+    },
+    "UI_MAP_DAYEVENT_TIPNEW2": {
+        "nameTextMapHash": 3994752885
+    },
+    "UI_MAP_DEEPSE_UNLOCKTIPS": {
+        "nameTextMapHash": 320480990
+    },
     "UI_MAP_DUNGEON)RECOMMEND_PARTY_LEVEL": {
         "nameTextMapHash": 359569047
     },
     "UI_MAP_DUNGEON_LEVEL": {
         "nameTextMapHash": 3614476560
     },
     "UI_MAP_DUNGEON_LEVEL_UNLOCK": {
@@ -37945,14 +37768,50 @@
     },
     "UI_MAP_REWARD_VANASARA_GATHER": {
         "nameTextMapHash": 1142861439
     },
     "UI_MAP_REWARD_WISHINGPOND_GATHER": {
         "nameTextMapHash": 3912626916
     },
+    "UI_MAP_SETTING_CARDSERCHOPENTIPS": {
+        "nameTextMapHash": 1196564808
+    },
+    "UI_MAP_SETTING_CONTROLLER": {
+        "nameTextMapHash": 1624704608
+    },
+    "UI_MAP_SETTING_CONTROLLER_ATTRACTION": {
+        "nameTextMapHash": 1835716037
+    },
+    "UI_MAP_SETTING_CONTROLLER_SENSITIVITY": {
+        "nameTextMapHash": 636760349
+    },
+    "UI_MAP_SETTING_MARKOPENTIPS": {
+        "nameTextMapHash": 2534800424
+    },
+    "UI_MAP_SETTING_MARKOPENTIPS_CONTENT": {
+        "nameTextMapHash": 293794820
+    },
+    "UI_MAP_SETTING_SHOWCONTENT1": {
+        "nameTextMapHash": 1662853856
+    },
+    "UI_MAP_SETTING_SHOWCONTENT2": {
+        "nameTextMapHash": 1811169768
+    },
+    "UI_MAP_SETTING_SHOWCONTENT_MARK": {
+        "nameTextMapHash": 3321151326
+    },
+    "UI_MAP_SETTING_SWITCH_OFF": {
+        "nameTextMapHash": 4069971357
+    },
+    "UI_MAP_SETTING_SWITCH_ON": {
+        "nameTextMapHash": 2801311613
+    },
+    "UI_MAP_SETTING_TITLE": {
+        "nameTextMapHash": 1743113480
+    },
     "UI_MAP_SWITCH_TO_INFO_LIST": {
         "nameTextMapHash": 964672017
     },
     "UI_MAP_SWITCH_TO_MAP": {
         "nameTextMapHash": 3462199510
     },
     "UI_MAP_SWITCH_TO_REWARD_TIPS": {
@@ -38554,14 +38413,17 @@
     },
     "UI_MUSIC_GAME_DRUM_ADJUST_BUTTON": {
         "nameTextMapHash": 2801071526
     },
     "UI_MUSIC_GAME_DRUM_ADJUST_DELAY": {
         "nameTextMapHash": 663486238
     },
+    "UI_MUSIC_GAME_DRUM_BACK_TO_SELECT": {
+        "nameTextMapHash": 3013490074
+    },
     "UI_MUSIC_GAME_DRUM_BACK_TO_SHARE": {
         "nameTextMapHash": 1770732050
     },
     "UI_MUSIC_GAME_DRUM_BEST_RECORD": {
         "nameTextMapHash": 1019251665
     },
     "UI_MUSIC_GAME_DRUM_BUTTION_APPEAR": {
@@ -39019,14 +38881,161 @@
     },
     "UI_MUSIC_GAME_DRUM_UGC_TUTORIAL": {
         "nameTextMapHash": 3413017847
     },
     "UI_MUSIC_GAME_DRUM_UNPLAYED": {
         "nameTextMapHash": 3246581590
     },
+    "UI_MUSIC_GAME_GREATFESV2_CHANGE_RECOMMEND": {
+        "nameTextMapHash": 3960987524
+    },
+    "UI_MUSIC_GAME_GREATFESV2_COLLECT_SONG": {
+        "nameTextMapHash": 3389819050
+    },
+    "UI_MUSIC_GAME_GREATFESV2_COLLECT_SONG_DEFAULT": {
+        "nameTextMapHash": 3484967480
+    },
+    "UI_MUSIC_GAME_GREATFESV2_COLLECT_SONG_SORT_01": {
+        "nameTextMapHash": 3491997823
+    },
+    "UI_MUSIC_GAME_GREATFESV2_COLLECT_SONG_SORT_02": {
+        "nameTextMapHash": 1360318423
+    },
+    "UI_MUSIC_GAME_GREATFESV2_CONNECT_HINT": {
+        "nameTextMapHash": 3860157272
+    },
+    "UI_MUSIC_GAME_GREATFESV2_GOTO_SETTING": {
+        "nameTextMapHash": 302892336
+    },
+    "UI_MUSIC_GAME_GREATFESV2_HOT_RECOMMEND": {
+        "nameTextMapHash": 862598532
+    },
+    "UI_MUSIC_GAME_GREATFESV2_IMPORT_ERROR": {
+        "nameTextMapHash": 3818725320
+    },
+    "UI_MUSIC_GAME_GREATFESV2_IMPORT_SETTING": {
+        "nameTextMapHash": 134292768
+    },
+    "UI_MUSIC_GAME_GREATFESV2_INSANE": {
+        "nameTextMapHash": 3141383739
+    },
+    "UI_MUSIC_GAME_GREATFESV2_INSANE_LEVEL": {
+        "nameTextMapHash": 2153473310
+    },
+    "UI_MUSIC_GAME_GREATFESV2_INSANE_LEVEL_LOCKED": {
+        "nameTextMapHash": 538083933
+    },
+    "UI_MUSIC_GAME_GREATFESV2_INSTRUMENT_DEFAULT": {
+        "nameTextMapHash": 1545245293
+    },
+    "UI_MUSIC_GAME_GREATFESV2_INSTRUMENT_STATE": {
+        "nameTextMapHash": 1479165133
+    },
+    "UI_MUSIC_GAME_GREATFESV2_NEW_RECOMMEND": {
+        "nameTextMapHash": 4017685426
+    },
+    "UI_MUSIC_GAME_GREATFESV2_NOTE_NUM_01": {
+        "nameTextMapHash": 3084100726
+    },
+    "UI_MUSIC_GAME_GREATFESV2_NOTE_NUM_02": {
+        "nameTextMapHash": 941337878
+    },
+    "UI_MUSIC_GAME_GREATFESV2_NOTE_TYPE_01": {
+        "nameTextMapHash": 3591299553
+    },
+    "UI_MUSIC_GAME_GREATFESV2_NOTE_TYPE_02": {
+        "nameTextMapHash": 3415583489
+    },
+    "UI_MUSIC_GAME_GREATFESV2_OPEN_HINT": {
+        "nameTextMapHash": 4242606202
+    },
+    "UI_MUSIC_GAME_GREATFESV2_OTHER_SONGS": {
+        "nameTextMapHash": 4230002769
+    },
+    "UI_MUSIC_GAME_GREATFESV2_PREFERENCE": {
+        "nameTextMapHash": 2069546659
+    },
+    "UI_MUSIC_GAME_GREATFESV2_PREFERENCE_CHECK": {
+        "nameTextMapHash": 408788007
+    },
+    "UI_MUSIC_GAME_GREATFESV2_PREFERENCE_CHECK_TIPS": {
+        "nameTextMapHash": 1643188657
+    },
+    "UI_MUSIC_GAME_GREATFESV2_PREFERENCE_CONFIRM": {
+        "nameTextMapHash": 3795573895
+    },
+    "UI_MUSIC_GAME_GREATFESV2_PREFERENCE_CURRENT_SONG": {
+        "nameTextMapHash": 2564751118
+    },
+    "UI_MUSIC_GAME_GREATFESV2_PREFERENCE_DEFAULT": {
+        "nameTextMapHash": 467535327
+    },
+    "UI_MUSIC_GAME_GREATFESV2_PREFERENCE_GUIDE": {
+        "nameTextMapHash": 2533499831
+    },
+    "UI_MUSIC_GAME_GREATFESV2_PREFERENCE_LIMIT": {
+        "nameTextMapHash": 252047991
+    },
+    "UI_MUSIC_GAME_GREATFESV2_PREFERENCE_NOTE_NUM": {
+        "nameTextMapHash": 3242897008
+    },
+    "UI_MUSIC_GAME_GREATFESV2_PREFERENCE_NOTE_TYPE": {
+        "nameTextMapHash": 3238229056
+    },
+    "UI_MUSIC_GAME_GREATFESV2_PREFERENCE_NOTE_TYPE_01": {
+        "nameTextMapHash": 838194966
+    },
+    "UI_MUSIC_GAME_GREATFESV2_PREFERENCE_NOTE_TYPE_02": {
+        "nameTextMapHash": 103558262
+    },
+    "UI_MUSIC_GAME_GREATFESV2_PREFERENCE_PAST_SONG": {
+        "nameTextMapHash": 2119204221
+    },
+    "UI_MUSIC_GAME_GREATFESV2_PREFERENCE_SET": {
+        "nameTextMapHash": 1355218823
+    },
+    "UI_MUSIC_GAME_GREATFESV2_PREFERENCE_SONG_NAME": {
+        "nameTextMapHash": 3200557677
+    },
+    "UI_MUSIC_GAME_GREATFESV2_PREFERENCE_TIPS": {
+        "nameTextMapHash": 2522324863
+    },
+    "UI_MUSIC_GAME_GREATFESV2_PS_CLOSE_SETTING": {
+        "nameTextMapHash": 681250443
+    },
+    "UI_MUSIC_GAME_GREATFESV2_PS_OPEN_SETTING": {
+        "nameTextMapHash": 91917507
+    },
+    "UI_MUSIC_GAME_GREATFESV2_RECOMMEND_SONG": {
+        "nameTextMapHash": 1276017186
+    },
+    "UI_MUSIC_GAME_GREATFESV2_SEARCH_SONG": {
+        "nameTextMapHash": 1032669837
+    },
+    "UI_MUSIC_GAME_GREATFESV2_SOUND_SETTING": {
+        "nameTextMapHash": 3433541723
+    },
+    "UI_MUSIC_GAME_GREATFESV2_THEME_DEFAULT": {
+        "nameTextMapHash": 3014886766
+    },
+    "UI_MUSIC_GAME_GREATFESV2_THEME_NORMAL": {
+        "nameTextMapHash": 4288251518
+    },
+    "UI_MUSIC_GAME_GREATFESV2_THEME_SELECT": {
+        "nameTextMapHash": 3058698790
+    },
+    "UI_MUSIC_GAME_GREATFESV2_TITLE": {
+        "nameTextMapHash": 1095822723
+    },
+    "UI_MUSIC_GAME_GREATFESV2_UI_SETTING": {
+        "nameTextMapHash": 162812705
+    },
+    "UI_MUSIC_GAME_GREATFESV2_UNRELEASED": {
+        "nameTextMapHash": 2686892643
+    },
     "UI_MUSIC_GAME_KEY_AUDIO_TIPS": {
         "nameTextMapHash": 2715618962
     },
     "UI_MUSIC_WIDGET_CANNOT_PLAY_TIPS": {
         "nameTextMapHash": 2141834040
     },
     "UI_MovedBattery_01": {
@@ -39955,14 +39964,17 @@
     },
     "UI_PRISONRANKING_TEAMNAME_04": {
         "nameTextMapHash": 2775353243
     },
     "UI_PRISONRANKING_TITLE": {
         "nameTextMapHash": 656646736
     },
+    "UI_PROFILEICON_UNLOCK_TITLE": {
+        "nameTextMapHash": 700220686
+    },
     "UI_PROMOTE_BUTTON": {
         "nameTextMapHash": 3614149475
     },
     "UI_PROUD_SKILL_UNLOCK": {
         "nameTextMapHash": 2875876030
     },
     "UI_PS4_ONLINE_EXCLUSIVE": {
@@ -40081,17 +40093,23 @@
     },
     "UI_QUEST_FINISHED": {
         "nameTextMapHash": 269100490
     },
     "UI_QUEST_FINISHWQ": {
         "nameTextMapHash": 1900071618
     },
+    "UI_QUEST_FOCUSOCCUPIED": {
+        "nameTextMapHash": 1927331578
+    },
     "UI_QUEST_GODDESSLOCKED": {
         "nameTextMapHash": 1161309330
     },
+    "UI_QUEST_GuideQuestItem": {
+        "nameTextMapHash": 2072950682
+    },
     "UI_QUEST_Guide_To_Layer": {
         "nameTextMapHash": 4262858181
     },
     "UI_QUEST_Guide_To_Layer_Hint": {
         "nameTextMapHash": 3759187128
     },
     "UI_QUEST_IN_AREA": {
@@ -40195,14 +40213,125 @@
     },
     "UI_QuestCheck_RuleExplain": {
         "nameTextMapHash": 1838487678
     },
     "UI_QuestCheck_SuccessTips": {
         "nameTextMapHash": 797606734
     },
+    "UI_QuestFocus_Button_CD_Hint": {
+        "nameTextMapHash": 296803323
+    },
+    "UI_QuestFocus_Close_Hint": {
+        "nameTextMapHash": 944683674
+    },
+    "UI_QuestFocus_Close_Tips": {
+        "nameTextMapHash": 3832405514
+    },
+    "UI_QuestFocus_GameMainPage_Focus_Occupied": {
+        "nameTextMapHash": 3230906186
+    },
+    "UI_QuestFocus_GameMainPage_Hint": {
+        "nameTextMapHash": 2470427005
+    },
+    "UI_QuestFocus_GameMainPage_Pasue": {
+        "nameTextMapHash": 3202567117
+    },
+    "UI_QuestFocus_GameMainPage_Title": {
+        "nameTextMapHash": 3560258549
+    },
+    "UI_QuestFocus_GuideText": {
+        "nameTextMapHash": 4282114733
+    },
+    "UI_QuestFocus_MUTUALEXCLUSION_Tips_Detial": {
+        "nameTextMapHash": 3828820932
+    },
+    "UI_QuestFocus_MUTUALEXCLUSION_Tips_Title": {
+        "nameTextMapHash": 256033748
+    },
+    "UI_QuestFocus_Mutual_Close_Hint": {
+        "nameTextMapHash": 122504137
+    },
+    "UI_QuestFocus_Pasue_Hint": {
+        "nameTextMapHash": 4126162943
+    },
+    "UI_QuestFocus_QuestPage_BanSwitch_Hint": {
+        "nameTextMapHash": 1347022554
+    },
+    "UI_QuestFocus_QuestPage_Focus_Occupied": {
+        "nameTextMapHash": 1711273617
+    },
+    "UI_QuestFocus_QuestPage_Focus_Occupied_Brief": {
+        "nameTextMapHash": 1108921574
+    },
+    "UI_QuestFocus_QuestPage_Npc_Occupied": {
+        "nameTextMapHash": 778263839
+    },
+    "UI_QuestFocus_QuestPage_Place_Occupied": {
+        "nameTextMapHash": 633352972
+    },
+    "UI_QuestFocus_Swich_LoadingHint": {
+        "nameTextMapHash": 1620546369
+    },
+    "UI_QuestFocus_Swich_Name": {
+        "nameTextMapHash": 757693281
+    },
+    "UI_QuestFocus_Swich_Tips_Button_Cancle": {
+        "nameTextMapHash": 3714925631
+    },
+    "UI_QuestFocus_Swich_Tips_Button_Confirm": {
+        "nameTextMapHash": 3616602055
+    },
+    "UI_QuestFocus_Swich_Tips_Detial_1": {
+        "nameTextMapHash": 3106822492
+    },
+    "UI_QuestFocus_Swich_Tips_Detial_3": {
+        "nameTextMapHash": 1998865500
+    },
+    "UI_QuestFocus_Swich_Tips_QustHint_Coop": {
+        "nameTextMapHash": 571626416
+    },
+    "UI_QuestFocus_Swich_Tips_QustHint_DisableSwitch": {
+        "nameTextMapHash": 4150388152
+    },
+    "UI_QuestFocus_Swich_Tips_QustHint_EnableSwitch": {
+        "nameTextMapHash": 598644384
+    },
+    "UI_QuestFocus_Swich_Tips_QustHint_IQ": {
+        "nameTextMapHash": 463094696
+    },
+    "UI_QuestFocus_Swich_Tips_QustHint_InFocus": {
+        "nameTextMapHash": 1896127648
+    },
+    "UI_QuestFocus_Swich_Tips_QustHint_RandomQuest": {
+        "nameTextMapHash": 1527396104
+    },
+    "UI_QuestFocus_Swich_Tips_Rule_Detail": {
+        "nameTextMapHash": 2846163768
+    },
+    "UI_QuestFocus_Swich_Tips_Rule_Name": {
+        "nameTextMapHash": 462484944
+    },
+    "UI_QuestFocus_Swich_Tips_Rule_Title": {
+        "nameTextMapHash": 3225961136
+    },
+    "UI_QuestFocus_Swich_Tips_Title": {
+        "nameTextMapHash": 772666436
+    },
+    "UI_QuestFocus_Switch_Off": {
+        "nameTextMapHash": 840050337
+    },
+    "UI_QuestFocus_Switch_On": {
+        "nameTextMapHash": 723957809
+    },
+    "UI_QuestFocus_Switch_ReadyHint": {
+        "nameTextMapHash": 3609163433
+    },
+    "UI_QuestFocus_Switch_TypeAndState": {
+        "nameTextMapHash": 225405793
+    },
     "UI_RACING_NEWRECORD": {
         "nameTextMapHash": 1727146555
     },
     "UI_RACING_TIMESPENT": {
         "nameTextMapHash": 4063423715
     },
     "UI_RANDOM_FACTOR": {
@@ -40360,14 +40489,17 @@
     },
     "UI_REMARK_SET_TITLE": {
         "nameTextMapHash": 1901358930
     },
     "UI_REMARK_TITLE": {
         "nameTextMapHash": 3977494001
     },
+    "UI_REMUS_DASH_QTE_SWITCH": {
+        "nameTextMapHash": 2460833207
+    },
     "UI_REPAIR_SKYHARP_PAGE_COMPLETE_BUTTON": {
         "nameTextMapHash": 3985473604
     },
     "UI_REPAIR_SKYHARP_PAGE_INREPAIR_BUTTON": {
         "nameTextMapHash": 4273685542
     },
     "UI_REPAIR_SKYHARP_PAGE_REPAIR_BUTTON": {
@@ -41242,14 +41374,44 @@
     },
     "UI_RelicIterations_Unlock_Hint": {
         "nameTextMapHash": 3333575510
     },
     "UI_RelicIterations_Unlock_Title": {
         "nameTextMapHash": 1881569846
     },
+    "UI_RemusArena_Talk": {
+        "nameTextMapHash": 2004378246
+    },
+    "UI_RemusArena_Talk_Permanent": {
+        "nameTextMapHash": 2145492938
+    },
+    "UI_RemusCat_Talk_01": {
+        "nameTextMapHash": 3563196009
+    },
+    "UI_RemusCat_Talk_02": {
+        "nameTextMapHash": 1277749617
+    },
+    "UI_RemusMusicBox_BUTTON_01": {
+        "nameTextMapHash": 4060380388
+    },
+    "UI_RemusMusicBox_BUTTON_02": {
+        "nameTextMapHash": 2904257820
+    },
+    "UI_RemusMusicBox_PICTURE_01": {
+        "nameTextMapHash": 2561882384
+    },
+    "UI_RemusMusicBox_TITLE_01": {
+        "nameTextMapHash": 3518090126
+    },
+    "UI_RemusMusicBox_TITLE_02": {
+        "nameTextMapHash": 3105437862
+    },
+    "UI_RemusMusicBox_TITLE_03": {
+        "nameTextMapHash": 2728117302
+    },
     "UI_Request_Fail": {
         "nameTextMapHash": 2171710347
     },
     "UI_RogueLikeRechallenge_Desc": {
         "nameTextMapHash": 86134926
     },
     "UI_RogueLikeRechallenge_Remark": {
@@ -41950,14 +42112,23 @@
     },
     "UI_SCENE_ENTRY_ENTER_Shuixian_Tower_2": {
         "nameTextMapHash": 3763644728
     },
     "UI_SCENE_ENTRY_ENTER_SumeruHome": {
         "nameTextMapHash": 2918111560
     },
+    "UI_SCENE_ENTRY_ENTER_TempleOfSilence01": {
+        "nameTextMapHash": 2514149352
+    },
+    "UI_SCENE_ENTRY_ENTER_TempleOfSilence02": {
+        "nameTextMapHash": 1588492608
+    },
+    "UI_SCENE_ENTRY_ENTER_TempleOfSilence03": {
+        "nameTextMapHash": 1081302192
+    },
     "UI_SCENE_ENTRY_ENTER_TenryuBugyo": {
         "nameTextMapHash": 2938935600
     },
     "UI_SCENE_ENTRY_ENTER_UYUTEI": {
         "nameTextMapHash": 1815094752
     },
     "UI_SCENE_ENTRY_ENTER_WardenOffice": {
@@ -42058,14 +42229,17 @@
     },
     "UI_SCENE_ENTRY_EXIT_Shuixian_Tower_2": {
         "nameTextMapHash": 2257069314
     },
     "UI_SCENE_ENTRY_EXIT_SumeruHome": {
         "nameTextMapHash": 3825636565
     },
+    "UI_SCENE_ENTRY_EXIT_TempleOfSilence": {
+        "nameTextMapHash": 99844997
+    },
     "UI_SCENE_ENTRY_EXIT_TenryuBugyo": {
         "nameTextMapHash": 2851729317
     },
     "UI_SCENE_ENTRY_EXIT_UYUTEI": {
         "nameTextMapHash": 3062503781
     },
     "UI_SCENE_ENTRY_EXIT_WardenOffice": {
@@ -42877,23 +43051,29 @@
     },
     "UI_SETUP_OTHER_5STAR": {
         "nameTextMapHash": 3189880098
     },
     "UI_SETUP_OTHER_BACKGROUND": {
         "nameTextMapHash": 2999653010
     },
+    "UI_SETUP_OTHER_MANAGE_ADS": {
+        "nameTextMapHash": 311713845
+    },
     "UI_SETUP_OTHER_TITLE_A": {
         "nameTextMapHash": 417241556
     },
     "UI_SHARE": {
         "nameTextMapHash": 1277702795
     },
     "UI_SHARE_REWARD": {
         "nameTextMapHash": 1130242878
     },
+    "UI_SHEET_RESTORE_NPC_QUEST_OCCUPY": {
+        "nameTextMapHash": 1803331021
+    },
     "UI_SHIELD_MIRROREDBIGWORLD_ITEM": {
         "nameTextMapHash": 81636433
     },
     "UI_SHOP_FORGE_WEAPON_TEXT": {
         "nameTextMapHash": 661447068
     },
     "UI_SILONG_MAPMARK_DESC": {
@@ -44299,14 +44479,17 @@
     },
     "UI_TRAININGGUIDE_BLUETIP_MENU_FIRSTTIME": {
         "nameTextMapHash": 748511507
     },
     "UI_TRAININGGUIDE_EMPTY": {
         "nameTextMapHash": 3269668098
     },
+    "UI_TRAININGGUIDE_ENTRY_BANNED": {
+        "nameTextMapHash": 861106503
+    },
     "UI_TRAININGGUIDE_ENTRY_TIP": {
         "nameTextMapHash": 1809660311
     },
     "UI_TRAININGGUIDE_FAIL_TIP": {
         "nameTextMapHash": 1505664154
     },
     "UI_TRAININGGUIDE_MATERIAL_LACK_TIP": {
@@ -44905,14 +45088,26 @@
     },
     "UI_WEATHER_SANDSTORM_DESC": {
         "nameTextMapHash": 2291579468
     },
     "UI_WEATHER_SANDSTORM_TITLE": {
         "nameTextMapHash": 3276881788
     },
+    "UI_WHALEINTERACT_CANNON": {
+        "nameTextMapHash": 2013963264
+    },
+    "UI_WHALEINTERACT_TALK": {
+        "nameTextMapHash": 3613076232
+    },
+    "UI_WHALETRENCH_ENTRY_BLACKSCREEN": {
+        "nameTextMapHash": 3668195063
+    },
+    "UI_WHALETRENCH_EXIT_COMFIRM_DESC": {
+        "nameTextMapHash": 714583823
+    },
     "UI_WIDGET_ACTIONPANEL_NUM": {
         "nameTextMapHash": 680340328
     },
     "UI_WIDGET_ANCHOR_FORBIDDEN_IN_BATTLE": {
         "nameTextMapHash": 1863424275
     },
     "UI_WIDGET_ANCHOR_FORBIDDEN_IN_FOCUS": {
@@ -44959,14 +45154,23 @@
     },
     "UI_WIDGET_CREATE_GADGET_RECYCLE": {
         "nameTextMapHash": 1193517177
     },
     "UI_WIDGET_DETECTOR_FAILED": {
         "nameTextMapHash": 381105203
     },
+    "UI_WIDGET_DETECTOR_NO_RESULT": {
+        "nameTextMapHash": 2475224632
+    },
+    "UI_WIDGET_DETECTOR_TAB_DESC": {
+        "nameTextMapHash": 2976221719
+    },
+    "UI_WIDGET_DETECTOR_TAB_TITLE": {
+        "nameTextMapHash": 3435000207
+    },
     "UI_WIDGET_EQUIP_SUCCESS": {
         "nameTextMapHash": 4106910055
     },
     "UI_WIDGET_FIREWORKS_IN_QUEUE_HINT": {
         "nameTextMapHash": 1976347353
     },
     "UI_WIDGET_FIREWORKS_LAUNCH": {
```

### Comparing `enkanetworkv2.py-2.0.4/enkanetwork/assets/data/namecards.json` & `enkanetworkv2.py-2.0.5/enkanetwork/assets/data/namecards.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9743589743589743%*

 * *Differences: {"'210195'": "OrderedDict([('nameTextMapHash', 89079668), ('icon', 'UI_NameCardIcon_Arlecchino'), "*

 * *             "('picPath', ['UI_NameCardPic_Arlecchino_Alpha', 'UI_NameCardPic_Arlecchino_P']), "*

 * *             "('rankLevel', 4), ('materialType', 'MATERIAL_NAMECARD')])",*

 * * "'210196'": "OrderedDict([('nameTextMapHash', 3853344316), ('icon', 'UI_NameCardIcon_Deep'), "*

 * *             "('picPath', ['UI_NameCardPic_Deep_Alpha', 'UI_NameCardPic_Deep_P']), ('rankLevel', "*

 * *             "4), ('materialType', 'MATERIAL_N […]*

```diff
@@ -1894,9 +1894,59 @@
         "materialType": "MATERIAL_NAMECARD",
         "nameTextMapHash": 882758588,
         "picPath": [
             "UI_NameCardPic_Bp31_Alpha",
             "UI_NameCardPic_Bp31_P"
         ],
         "rankLevel": 4
+    },
+    "210195": {
+        "icon": "UI_NameCardIcon_Arlecchino",
+        "materialType": "MATERIAL_NAMECARD",
+        "nameTextMapHash": 89079668,
+        "picPath": [
+            "UI_NameCardPic_Arlecchino_Alpha",
+            "UI_NameCardPic_Arlecchino_P"
+        ],
+        "rankLevel": 4
+    },
+    "210196": {
+        "icon": "UI_NameCardIcon_Deep",
+        "materialType": "MATERIAL_NAMECARD",
+        "nameTextMapHash": 3853344316,
+        "picPath": [
+            "UI_NameCardPic_Deep_Alpha",
+            "UI_NameCardPic_Deep_P"
+        ],
+        "rankLevel": 4
+    },
+    "210197": {
+        "icon": "UI_NameCardIcon_Tzz9",
+        "materialType": "MATERIAL_NAMECARD",
+        "nameTextMapHash": 1686874332,
+        "picPath": [
+            "UI_NameCardPic_Tzz9_Alpha",
+            "UI_NameCardPic_Tzz9_P"
+        ],
+        "rankLevel": 4
+    },
+    "210198": {
+        "icon": "UI_NameCardIcon_WishingPond",
+        "materialType": "MATERIAL_NAMECARD",
+        "nameTextMapHash": 328422540,
+        "picPath": [
+            "UI_NameCardPic_WishingPond_Alpha",
+            "UI_NameCardPic_WishingPond_P"
+        ],
+        "rankLevel": 4
+    },
+    "210199": {
+        "icon": "UI_NameCardIcon_GreatFestivalV2",
+        "materialType": "MATERIAL_NAMECARD",
+        "nameTextMapHash": 1744889084,
+        "picPath": [
+            "UI_NameCardPic_GreatFestivalV2_Alpha",
+            "UI_NameCardPic_GreatFestivalV2_P"
+        ],
+        "rankLevel": 4
     }
 }
```

### Comparing `enkanetworkv2.py-2.0.4/enkanetwork/assets/data/pfps.json` & `enkanetworkv2.py-2.0.5/enkanetwork/assets/data/pfps.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.4/enkanetwork/assets/data/skills.json` & `enkanetworkv2.py-2.0.5/enkanetwork/assets/data/skills.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9712918660287081%*

 * *Differences: {"'10961'": "OrderedDict([('nameTextMapHash', 3395884205), ('skillIcon', 'Skill_A_03'), "*

 * *            "('proudSkillGroupId', 9631)])",*

 * * "'10962'": "OrderedDict([('nameTextMapHash', 88213301), ('skillIcon', 'Skill_S_Arlecchino_01'), "*

 * *            "('proudSkillGroupId', 9632)])",*

 * * "'10963'": "OrderedDict([('nameTextMapHash', 1398698245), ('skillIcon', 'Skill_S_Arlecchino_01'), "*

 * *            "('proudSkillGroupId', '')])",*

 * * "'10965'": "OrderedDict([('nameTextMapHash', 2156811133), ('skillIcon', 'Skill_E_Arlecch […]*

```diff
@@ -1955,14 +1955,44 @@
         "skillIcon": "Skill_S_Chiori_03"
     },
     "10945": {
         "nameTextMapHash": 373425821,
         "proudSkillGroupId": 9439,
         "skillIcon": "Skill_E_Chiori_01"
     },
+    "10961": {
+        "nameTextMapHash": 3395884205,
+        "proudSkillGroupId": 9631,
+        "skillIcon": "Skill_A_03"
+    },
+    "10962": {
+        "nameTextMapHash": 88213301,
+        "proudSkillGroupId": 9632,
+        "skillIcon": "Skill_S_Arlecchino_01"
+    },
+    "10963": {
+        "nameTextMapHash": 1398698245,
+        "proudSkillGroupId": "",
+        "skillIcon": "Skill_S_Arlecchino_01"
+    },
+    "10965": {
+        "nameTextMapHash": 2156811133,
+        "proudSkillGroupId": 9639,
+        "skillIcon": "Skill_E_Arlecchino_01"
+    },
+    "10966": {
+        "nameTextMapHash": 3589496853,
+        "proudSkillGroupId": "",
+        "skillIcon": "Skill_A_03"
+    },
+    "10967": {
+        "nameTextMapHash": 4257022253,
+        "proudSkillGroupId": "",
+        "skillIcon": "Skill_A_03"
+    },
     "11301": {
         "nameTextMapHash": 3802462781,
         "proudSkillGroupId": "",
         "skillIcon": "Skill_A_02"
     },
     "11302": {
         "nameTextMapHash": 2467360621,
@@ -2205,24 +2235,34 @@
         "skillIcon": "Skill_LanV4PartyLion_01"
     },
     "20080": {
         "nameTextMapHash": 3018374477,
         "proudSkillGroupId": "",
         "skillIcon": "QuesteventSkillIcon_01"
     },
+    "20081": {
+        "nameTextMapHash": 845866237,
+        "proudSkillGroupId": "",
+        "skillIcon": "Skill_Music"
+    },
     "20083": {
         "nameTextMapHash": 4248326901,
         "proudSkillGroupId": "",
         "skillIcon": "Skill_LanV4PartyLion_01"
     },
     "20084": {
         "nameTextMapHash": 682415765,
         "proudSkillGroupId": "",
         "skillIcon": "Skill_LanV4PartyLion_01"
     },
+    "20086": {
+        "nameTextMapHash": 4251923773,
+        "proudSkillGroupId": "",
+        "skillIcon": "Skill_Music"
+    },
     "20093": {
         "nameTextMapHash": 3906587141,
         "proudSkillGroupId": "",
         "skillIcon": "Btn_SlimeCannon_Fire_01"
     },
     "20094": {
         "nameTextMapHash": 2428119293,
@@ -2395,14 +2435,19 @@
         "skillIcon": "Skill_LanV3_Icon05"
     },
     "20345": {
         "nameTextMapHash": 1316655253,
         "proudSkillGroupId": "",
         "skillIcon": "Btn_PacMan"
     },
+    "20346": {
+        "nameTextMapHash": 840915861,
+        "proudSkillGroupId": "",
+        "skillIcon": "Btn_Whale_Interrupt"
+    },
     "20350": {
         "nameTextMapHash": 3206240077,
         "proudSkillGroupId": "",
         "skillIcon": "Skill_E_Klee_01"
     },
     "20351": {
         "nameTextMapHash": 2174036525,
@@ -2565,14 +2610,54 @@
         "skillIcon": "Skill_CarpJump_01"
     },
     "20531": {
         "nameTextMapHash": 1873021445,
         "proudSkillGroupId": "",
         "skillIcon": "Btn_Fishing_Exit"
     },
+    "20532": {
+        "nameTextMapHash": 1819872509,
+        "proudSkillGroupId": "",
+        "skillIcon": "Btn_HideAndSeekV4_Seeker_A_03"
+    },
+    "20533": {
+        "nameTextMapHash": 4151065125,
+        "proudSkillGroupId": "",
+        "skillIcon": "Btn_HideAndSeekV4_Seeker_E_03"
+    },
+    "20534": {
+        "nameTextMapHash": 1658286853,
+        "proudSkillGroupId": "",
+        "skillIcon": "Btn_HideAndSeekV4_Hider_S"
+    },
+    "20535": {
+        "nameTextMapHash": 164728021,
+        "proudSkillGroupId": "",
+        "skillIcon": "Btn_HideAndSeekV4_Hider_S"
+    },
+    "20538": {
+        "nameTextMapHash": 2797265765,
+        "proudSkillGroupId": "",
+        "skillIcon": "Btn_HideAndSeekV4_Seeker_E_01"
+    },
+    "20539": {
+        "nameTextMapHash": 351406893,
+        "proudSkillGroupId": "",
+        "skillIcon": "Btn_HideAndSeekV4_Seeker_S"
+    },
+    "20540": {
+        "nameTextMapHash": 1185389325,
+        "proudSkillGroupId": "",
+        "skillIcon": "Btn_HideAndSeekV4_Seeker_S"
+    },
+    "20541": {
+        "nameTextMapHash": 3465751389,
+        "proudSkillGroupId": "",
+        "skillIcon": "Btn_HideAndSeekV4_Seeker_A_01"
+    },
     "5002010": {
         "nameTextMapHash": 1113979477,
         "proudSkillGroupId": "",
         "skillIcon": "Skill_A_01"
     },
     "5003010": {
         "nameTextMapHash": 2743040301,
@@ -3039,9 +3124,14 @@
         "proudSkillGroupId": "",
         "skillIcon": "Skill_A_Catalyst_MD"
     },
     "5094010": {
         "nameTextMapHash": 331992085,
         "proudSkillGroupId": "",
         "skillIcon": "Skill_A_01"
+    },
+    "5096010": {
+        "nameTextMapHash": 2699549653,
+        "proudSkillGroupId": "",
+        "skillIcon": "Skill_A_03"
     }
 }
```

### Comparing `enkanetworkv2.py-2.0.4/enkanetwork/assets/data/weapons.json` & `enkanetworkv2.py-2.0.5/enkanetwork/assets/data/weapons.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9953051643192489%*

 * *Differences: {"'13512'": "OrderedDict([('nameTextMapHash', 2944936683), ('icon', "*

 * *            "'UI_EquipIcon_Pole_BloodMoon'), ('awakenIcon', 'UI_EquipIcon_Pole_BloodMoon_Awaken'), "*

 * *            "('rankLevel', 5)])"}*

```diff
@@ -769,14 +769,20 @@
     },
     "13511": {
         "awakenIcon": "UI_EquipIcon_Pole_Deshret_Awaken",
         "icon": "UI_EquipIcon_Pole_Deshret",
         "nameTextMapHash": 4238339131,
         "rankLevel": 5
     },
+    "13512": {
+        "awakenIcon": "UI_EquipIcon_Pole_BloodMoon_Awaken",
+        "icon": "UI_EquipIcon_Pole_BloodMoon",
+        "nameTextMapHash": 2944936683,
+        "rankLevel": 5
+    },
     "14101": {
         "awakenIcon": "UI_EquipIcon_Catalyst_Apprentice_Awaken",
         "icon": "UI_EquipIcon_Catalyst_Apprentice",
         "nameTextMapHash": 3584825427,
         "rankLevel": 1
     },
     "14201": {
```

### Comparing `enkanetworkv2.py-2.0.4/enkanetwork/assets/langs/artifact_sets.json` & `enkanetworkv2.py-2.0.5/enkanetwork/assets/langs/artifact_sets.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9911591355599214%*

 * *Differences: {"'1230304555'": "OrderedDict([('CHS', '烬日之影'), ('DE', 'Schatten der äschernen Sonne'), ('EN', "*

 * *                 '"Ashen Sun\'s Shadow"), (\'ES\', \'Sombra del sol cenizo\'), (\'FR\', \'Ombre du '*

 * *                 'soleil cendré\'), (\'ID\', "Ashen Sun\'s Shadow"), (\'IT\', \'Ombra del sole '*

 * *                 "cinereo'), ('JP', '燃え尽きる日の影'), ('KR', '잿빛 태양의 그림자'), ('PT', 'Sombra do Sol de "*

 * *                 'Cinzas\'), (\'RU\', \'Тень пепельного солнца\'), (\'TH\', "Ashen Sun\'s '*

 * *                 'Shadow"), […]*

```diff
@@ -955,14 +955,30 @@
         "KR": "\ub9c8\ub825\uc758 \uac08\uc99d",
         "PT": "Viciado em Magia",
         "RU": "\u0412\u043b\u0435\u0447\u0435\u043d\u0438\u0435 \u043c\u0430\u0433\u0438\u0438",
         "TH": "Magic Affinity",
         "TR": "B\u00fcy\u00fc Ba\u011f\u0131ml\u0131s\u0131",
         "VI": "Th\u1ecb Ma"
     },
+    "1230304555": {
+        "CHS": "\u70ec\u65e5\u4e4b\u5f71",
+        "DE": "Schatten der \u00e4schernen Sonne",
+        "EN": "Ashen Sun's Shadow",
+        "ES": "Sombra del sol cenizo",
+        "FR": "Ombre du soleil cendr\u00e9",
+        "ID": "Ashen Sun's Shadow",
+        "IT": "Ombra del sole cinereo",
+        "JP": "\u71c3\u3048\u5c3d\u304d\u308b\u65e5\u306e\u5f71",
+        "KR": "\uc7bf\ube5b \ud0dc\uc591\uc758 \uadf8\ub9bc\uc790",
+        "PT": "Sombra do Sol de Cinzas",
+        "RU": "\u0422\u0435\u043d\u044c \u043f\u0435\u043f\u0435\u043b\u044c\u043d\u043e\u0433\u043e \u0441\u043e\u043b\u043d\u0446\u0430",
+        "TH": "Ashen Sun's Shadow",
+        "TR": "Solgun G\u00fcne\u015fin G\u00f6lgesi",
+        "VI": "B\u00f3ng T\u1ed1i M\u1eb7t Tr\u1eddi T\u00e0n"
+    },
     "1234331811": {
         "CHS": "\u91d1\u748b\u7687\u6781",
         "DE": "Majest\u00e4tische Gr\u00f6\u00dfe",
         "EN": "Golden Majesty",
         "ES": "Majestad dorada",
         "FR": "Majest\u00e9 dor\u00e9e",
         "ID": "Golden Majesty",
@@ -1803,14 +1819,30 @@
         "KR": "\uacb0",
         "PT": "Determina\u00e7\u00e3o",
         "RU": "\u0420\u0435\u0448\u0438\u0442\u0435\u043b\u044c\u043d\u044b\u0439",
         "TH": "Gash",
         "TR": "Derin Yara",
         "VI": "Quy\u1ebft"
     },
+    "1407869611": {
+        "CHS": "\u672a\u7adf\u7684\u9050\u601d",
+        "DE": "Unvollendete Tr\u00e4umerei",
+        "EN": "Unfinished Reverie",
+        "ES": "Enso\u00f1aci\u00f3n Inacabada",
+        "FR": "R\u00eaverie incompl\u00e8te",
+        "ID": "Unfinished Reverie",
+        "IT": "Fantasmagoria incompiuta",
+        "JP": "\u9042\u3052\u3089\u308c\u306a\u304b\u3063\u305f\u60f3\u3044",
+        "KR": "\ubbf8\uc644\uc758 \ubabd\uc0c1",
+        "PT": "Reminisc\u00eancia Incompleta",
+        "RU": "\u041d\u0435\u0437\u0430\u043a\u043e\u043d\u0447\u0435\u043d\u043d\u044b\u0435 \u0433\u0440\u0451\u0437\u044b",
+        "TH": "Unfinished Reverie",
+        "TR": "Yar\u0131m Kalan R\u00fcya",
+        "VI": "\u1ea2o M\u1ed9ng Ch\u01b0a Ho\u00e0n Th\u00e0nh"
+    },
     "141119323": {
         "CHS": "\u98ce\u4e0e\u82b1\u7684\u5bc6\u8bed",
         "DE": "Fl\u00fcstern von Wind und Blumen",
         "EN": "Whispers of Wind and Flower",
         "ES": "C\u00f3digo vientoflorido",
         "FR": "Murmure des vents et des fleurs",
         "ID": "Whispers of Wind and Flower",
@@ -2107,14 +2139,30 @@
         "KR": "\uc5d0\ub108\uc9c0 \uc8fc\uc785 \uac00\uc2dc",
         "PT": "Ferr\u00e3o Energ\u00e9tico",
         "RU": "\u0417\u0430\u0440\u044f\u0436\u0435\u043d\u043d\u043e\u0435 \u0436\u0430\u043b\u043e",
         "TH": "Infusion Stinger",
         "TR": "Tesirli Me\u00e7",
         "VI": "K\u00edch N\u0103ng L\u01b0\u1ee3ng"
     },
+    "1492570003": {
+        "CHS": "\u8c10\u5f8b\u5f02\u60f3\u65ad\u7ae0",
+        "DE": "Fragment harmonischer Launen",
+        "EN": "Fragment of Harmonic Whimsy",
+        "ES": "Fragmento de la Armon\u00eda Fantasiosa",
+        "FR": "Fragment d'harmonie divergente",
+        "ID": "Fragment of Harmonic Whimsy",
+        "IT": "Scheggia di estro armonico",
+        "JP": "\u8ae7\u5f8b\u5947\u60f3\u306e\u65ad\u7ae0",
+        "KR": "\uc870\ud654\ub85c\uc6b4 \uacf5\uc0c1\uc758 \ub2e8\ud3b8",
+        "PT": "Fragmento da Harmonia Fant\u00e1stica",
+        "RU": "\u0424\u0440\u0430\u0433\u043c\u0435\u043d\u0442 \u0433\u0430\u0440\u043c\u043e\u043d\u0438\u0447\u0435\u0441\u043a\u043e\u0439 \u0444\u0430\u043d\u0442\u0430\u0437\u0438\u0438",
+        "TH": "Fragment of Harmonic Whimsy",
+        "TR": "Armonik \u0130lham Par\u00e7as\u0131",
+        "VI": "M\u1ea3nh H\u00e0i H\u00f2a B\u1ea5t Th\u01b0\u1eddng"
+    },
     "1492752155": {
         "CHS": "\u6c14\u5b9a\u795e\u95f2",
         "DE": "G\u00f6ttliche F\u00fcgung",
         "EN": "Composed",
         "ES": "Serenidad",
         "FR": "Sang-froid",
         "ID": "Composed",
@@ -2603,14 +2651,30 @@
         "KR": "",
         "PT": "",
         "RU": "",
         "TH": "",
         "TR": "",
         "VI": ""
     },
+    "1607784379": {
+        "CHS": "\u70ec\u65e5\u4e4b\u5f71",
+        "DE": "Schatten der \u00e4schernen Sonne",
+        "EN": "Ashen Sun's Shadow",
+        "ES": "Sombra del sol cenizo",
+        "FR": "Ombre du soleil cendr\u00e9",
+        "ID": "Ashen Sun's Shadow",
+        "IT": "Ombra del sole cinereo",
+        "JP": "\u71c3\u3048\u5c3d\u304d\u308b\u65e5\u306e\u5f71",
+        "KR": "\uc7bf\ube5b \ud0dc\uc591\uc758 \uadf8\ub9bc\uc790",
+        "PT": "Sombra do Sol de Cinzas",
+        "RU": "\u0422\u0435\u043d\u044c \u043f\u0435\u043f\u0435\u043b\u044c\u043d\u043e\u0433\u043e \u0441\u043e\u043b\u043d\u0446\u0430",
+        "TH": "Ashen Sun's Shadow",
+        "TR": "Solgun G\u00fcne\u015fin G\u00f6lgesi",
+        "VI": "B\u00f3ng T\u1ed1i M\u1eb7t Tr\u1eddi T\u00e0n"
+    },
     "1610242915": {
         "CHS": "\u4f20\u627f",
         "DE": "\u00dcberlieferung",
         "EN": "Heritage",
         "ES": "Legado",
         "FR": "H\u00e9ritage",
         "ID": "Heritage",
@@ -8459,14 +8523,30 @@
         "KR": "\uc774\ucc29\ubd88\uadc0",
         "PT": "Sem Retorno",
         "RU": "\u041d\u0435\u0432\u043e\u0437\u0432\u0440\u0430\u0442\u043d\u044b\u0439",
         "TH": "Unreturning",
         "TR": "D\u00f6n\u00fc\u015fs\u00fcz",
         "VI": "R\u1eddi Kh\u1ecfi B\u1ea7y \u0110\u00e0n"
     },
+    "3029495379": {
+        "CHS": "\u8c10\u5f8b\u5f02\u60f3\u65ad\u7ae0",
+        "DE": "Fragment harmonischer Launen",
+        "EN": "Fragment of Harmonic Whimsy",
+        "ES": "Fragmento de la Armon\u00eda Fantasiosa",
+        "FR": "Fragment d'harmonie divergente",
+        "ID": "Fragment of Harmonic Whimsy",
+        "IT": "Scheggia di estro armonico",
+        "JP": "\u8ae7\u5f8b\u5947\u60f3\u306e\u65ad\u7ae0",
+        "KR": "\uc870\ud654\ub85c\uc6b4 \uacf5\uc0c1\uc758 \ub2e8\ud3b8",
+        "PT": "Fragmento da Harmonia Fant\u00e1stica",
+        "RU": "\u0424\u0440\u0430\u0433\u043c\u0435\u043d\u0442 \u0433\u0430\u0440\u043c\u043e\u043d\u0438\u0447\u0435\u0441\u043a\u043e\u0439 \u0444\u0430\u043d\u0442\u0430\u0437\u0438\u0438",
+        "TH": "Fragment of Harmonic Whimsy",
+        "TR": "Armonik \u0130lham Par\u00e7as\u0131",
+        "VI": "M\u1ea3nh H\u00e0i H\u00f2a B\u1ea5t Th\u01b0\u1eddng"
+    },
     "303155515": {
         "CHS": "\u79bb\u7c07\u4e0d\u5f52",
         "DE": "Ohne Wiederkehr",
         "EN": "Unreturning",
         "ES": "Sin retorno",
         "FR": "Sans retour",
         "ID": "Unreturning",
@@ -10555,14 +10635,30 @@
         "KR": "\uae09\ub958",
         "PT": "Corrente Torrencial",
         "RU": "\u0412\u043e\u0440\u043e\u043d\u043a\u0430",
         "TH": "Rapids",
         "TR": "Ak\u0131nt\u0131lar",
         "VI": "K\u00edch L\u01b0u"
     },
+    "352459163": {
+        "CHS": "\u672a\u7adf\u7684\u9050\u601d",
+        "DE": "Unvollendete Tr\u00e4umerei",
+        "EN": "Unfinished Reverie",
+        "ES": "Enso\u00f1aci\u00f3n Inacabada",
+        "FR": "R\u00eaverie incompl\u00e8te",
+        "ID": "Unfinished Reverie",
+        "IT": "Fantasmagoria incompiuta",
+        "JP": "\u9042\u3052\u3089\u308c\u306a\u304b\u3063\u305f\u60f3\u3044",
+        "KR": "\ubbf8\uc644\uc758 \ubabd\uc0c1",
+        "PT": "Reminisc\u00eancia Incompleta",
+        "RU": "\u041d\u0435\u0437\u0430\u043a\u043e\u043d\u0447\u0435\u043d\u043d\u044b\u0435 \u0433\u0440\u0451\u0437\u044b",
+        "TH": "Unfinished Reverie",
+        "TR": "Yar\u0131m Kalan R\u00fcya",
+        "VI": "\u1ea2o M\u1ed9ng Ch\u01b0a Ho\u00e0n Th\u00e0nh"
+    },
     "3533218187": {
         "CHS": "\u5343\u5ca9\u8bc0\u00b7\u540c\u5fc3",
         "DE": "Axiom der Millelithen \u2013 Einigkeit",
         "EN": "Lithic Axiom: Unity",
         "ES": "Axioma de la roca: Unidad",
         "FR": "Axiome de la roche : Unit\u00e9",
         "ID": "Lithic Axiom: Unity",
@@ -10875,14 +10971,30 @@
         "KR": "\uc5d0\ub108\uc9c0 \uc0e4\uc6cc",
         "PT": "Imers\u00e3o de Energia",
         "RU": "\u0414\u043e\u0436\u0434\u044c \u044d\u043d\u0435\u0440\u0433\u0438\u0438",
         "TH": "Energy Shower",
         "TR": "Enerji Ya\u011fmuru",
         "VI": "T\u1eafm N\u0103ng L\u01b0\u1ee3ng"
     },
+    "3624979763": {
+        "CHS": "\u70ec\u65e5\u4e4b\u5f71",
+        "DE": "Schatten der \u00e4schernen Sonne",
+        "EN": "Ashen Sun's Shadow",
+        "ES": "Sombra del sol cenizo",
+        "FR": "Ombre du soleil cendr\u00e9",
+        "ID": "Ashen Sun's Shadow",
+        "IT": "Ombra del sole cinereo",
+        "JP": "\u71c3\u3048\u5c3d\u304d\u308b\u65e5\u306e\u5f71",
+        "KR": "\uc7bf\ube5b \ud0dc\uc591\uc758 \uadf8\ub9bc\uc790",
+        "PT": "Sombra do Sol de Cinzas",
+        "RU": "\u0422\u0435\u043d\u044c \u043f\u0435\u043f\u0435\u043b\u044c\u043d\u043e\u0433\u043e \u0441\u043e\u043b\u043d\u0446\u0430",
+        "TH": "Ashen Sun's Shadow",
+        "TR": "Solgun G\u00fcne\u015fin G\u00f6lgesi",
+        "VI": "B\u00f3ng T\u1ed1i M\u1eb7t Tr\u1eddi T\u00e0n"
+    },
     "3626268211": {
         "CHS": "\u6765\u6b46\u4f59\u54cd",
         "DE": "Echo des Opferfests",
         "EN": "Echoes of an Offering",
         "ES": "Eco del Sacrificio",
         "FR": "\u00c9chos d'une offrande",
         "ID": "Echoes of an Offering",
@@ -15067,14 +15179,30 @@
         "KR": "\uae08\ube5b\uc758 \uc625\u00b7\uc81c\uad70\uc758 \uae38",
         "PT": "Majestade Dourada",
         "RU": "\u0417\u043e\u043b\u043e\u0447\u0451\u043d\u043e\u0435 \u0432\u0435\u043b\u0438\u0447\u0435\u0441\u0442\u0432\u043e",
         "TH": "Golden Majesty",
         "TR": "Alt\u0131n \u0130hti\u015fam",
         "VI": "Ho\u00e0ng C\u1ef1c Ch\u01b0\u01a1ng V\u00e0ng"
     },
+    "742248595": {
+        "CHS": "\u70ec\u65e5\u4e4b\u5f71",
+        "DE": "Schatten der \u00e4schernen Sonne",
+        "EN": "Ashen Sun's Shadow",
+        "ES": "Sombra del sol cenizo",
+        "FR": "Ombre du soleil cendr\u00e9",
+        "ID": "Ashen Sun's Shadow",
+        "IT": "Ombra del sole cinereo",
+        "JP": "\u71c3\u3048\u5c3d\u304d\u308b\u65e5\u306e\u5f71",
+        "KR": "\uc7bf\ube5b \ud0dc\uc591\uc758 \uadf8\ub9bc\uc790",
+        "PT": "Sombra do Sol de Cinzas",
+        "RU": "\u0422\u0435\u043d\u044c \u043f\u0435\u043f\u0435\u043b\u044c\u043d\u043e\u0433\u043e \u0441\u043e\u043b\u043d\u0446\u0430",
+        "TH": "Ashen Sun's Shadow",
+        "TR": "Solgun G\u00fcne\u015fin G\u00f6lgesi",
+        "VI": "B\u00f3ng T\u1ed1i M\u1eb7t Tr\u1eddi T\u00e0n"
+    },
     "744390051": {
         "CHS": "\u4e13\u6ce8",
         "DE": "Konzentration",
         "EN": "Focus",
         "ES": "Concentraci\u00f3n",
         "FR": "Focus",
         "ID": "Focus",
@@ -15339,14 +15467,30 @@
         "KR": "\uc2e0\uae30\ub8e8 \ub05d\uc758 \ub728\uac70\uc6b4 \uafc8",
         "PT": "Sonho Ardente no Fim do Horizonte",
         "RU": "\u041c\u0430\u0440\u0435\u0432\u043e \u043d\u0430 \u0433\u043e\u0440\u0438\u0437\u043e\u043d\u0442\u0435",
         "TH": "Heat Haze at Horizon's End",
         "TR": "Ufuk Serab\u0131",
         "VI": "Gi\u1ea5c M\u1ed9ng Cu\u1ed1i Ch\u00e2n Tr\u1eddi"
     },
+    "813291827": {
+        "CHS": "\u70ec\u65e5\u4e4b\u5f71",
+        "DE": "Schatten der \u00e4schernen Sonne",
+        "EN": "Ashen Sun's Shadow",
+        "ES": "Sombra del sol cenizo",
+        "FR": "Ombre du soleil cendr\u00e9",
+        "ID": "Ashen Sun's Shadow",
+        "IT": "Ombra del sole cinereo",
+        "JP": "\u71c3\u3048\u5c3d\u304d\u308b\u65e5\u306e\u5f71",
+        "KR": "\uc7bf\ube5b \ud0dc\uc591\uc758 \uadf8\ub9bc\uc790",
+        "PT": "Sombra do Sol de Cinzas",
+        "RU": "\u0422\u0435\u043d\u044c \u043f\u0435\u043f\u0435\u043b\u044c\u043d\u043e\u0433\u043e \u0441\u043e\u043b\u043d\u0446\u0430",
+        "TH": "Ashen Sun's Shadow",
+        "TR": "Solgun G\u00fcne\u015fin G\u00f6lgesi",
+        "VI": "B\u00f3ng T\u1ed1i M\u1eb7t Tr\u1eddi T\u00e0n"
+    },
     "813820979": {
         "CHS": "\u80fd\u91cf\u6c90\u6d74",
         "DE": "Energiebad",
         "EN": "Energy Shower",
         "ES": "Inmersi\u00f3n energ\u00e9tica",
         "FR": "Immersion \u00e9nerg\u00e9tique",
         "ID": "Energy Shower",
```

### Comparing `enkanetworkv2.py-2.0.4/enkanetwork/assets/langs/artifacts.json` & `enkanetworkv2.py-2.0.5/enkanetwork/assets/langs/artifacts.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9849699398797596%*

 * *Differences: {"'1056891388'": "OrderedDict([('CHS', '举业的识刻'), ('DE', 'Augenblick des Erfolgs'), ('EN', 'Moment "*

 * *                 "of Attainment'), ('ES', 'Momento de Aprehensión'), ('FR', 'Instant de "*

 * *                 "réalisation'), ('ID', 'Moment of Attainment'), ('IT', 'Momento di conquista'), "*

 * *                 "('JP', '大業を成す刻'), ('KR', '대업의 시간'), ('PT', 'Momento de Conquista'), ('RU', "*

 * *                 "'Момент обретения'), ('TH', 'Moment of Attainment'), ('TR', 'Zafer Anı'), ('VI', "*

 * *                 "'Thời Khắ […]*

```diff
@@ -1003,14 +1003,30 @@
         "KR": "\uc0ac\ub0e5\uafbc\uc758 \ube0c\ub85c\uce58",
         "PT": "Flor de Lapela do Ca\u00e7ador",
         "RU": "\u0411\u0440\u043e\u0448\u044c \u043e\u0445\u043e\u0442\u043d\u0438\u043a\u0430",
         "TH": "Hunter's Brooch",
         "TR": "Avc\u0131n\u0131n Bro\u015fu",
         "VI": "\u0110\u00f3a Hoa C\u1ee7a Th\u1ee3 S\u0103n"
     },
+    "1056891388": {
+        "CHS": "\u4e3e\u4e1a\u7684\u8bc6\u523b",
+        "DE": "Augenblick des Erfolgs",
+        "EN": "Moment of Attainment",
+        "ES": "Momento de Aprehensi\u00f3n",
+        "FR": "Instant de r\u00e9alisation",
+        "ID": "Moment of Attainment",
+        "IT": "Momento di conquista",
+        "JP": "\u5927\u696d\u3092\u6210\u3059\u523b",
+        "KR": "\ub300\uc5c5\uc758 \uc2dc\uac04",
+        "PT": "Momento de Conquista",
+        "RU": "\u041c\u043e\u043c\u0435\u043d\u0442 \u043e\u0431\u0440\u0435\u0442\u0435\u043d\u0438\u044f",
+        "TH": "Moment of Attainment",
+        "TR": "Zafer An\u0131",
+        "VI": "Th\u1eddi Kh\u1eafc C\u1ee7a \u0110\u1ea1t Th\u00e0nh"
+    },
     "1057543844": {
         "CHS": "\u541f\u6e38\u8005\u4e4b\u58f6",
         "DE": "Bardenflasche",
         "EN": "Wanderer's String-Kettle",
         "ES": "Cantimplora del Errante",
         "FR": "Gourde \u00e0 cordes du m\u00e9nestrel",
         "ID": "Wanderer's String-Kettle",
@@ -2523,14 +2539,30 @@
         "KR": "\uc228\uaca8\uc9c4 \ube5b\uc758 \uae43\ud138",
         "PT": "Pena do Esplendor",
         "RU": "\u041f\u0435\u0440\u043e \u0441\u043a\u0440\u044b\u0442\u043e\u0433\u043e \u0441\u0438\u044f\u043d\u0438\u044f",
         "TH": "Feather of Nascent Light",
         "TR": "Sakl\u0131 I\u015f\u0131\u011f\u0131n T\u00fcy\u00fc",
         "VI": "L\u00f4ng V\u0169 L\u1ea5p L\u00e1nh"
     },
+    "1150905740": {
+        "CHS": "\u5f02\u60f3\u96f6\u843d\u7684\u5706\u821e",
+        "DE": "Reigen vereinzelter Launen",
+        "EN": "Whimsical Dance of the Withered",
+        "ES": "Vals Fantasioso de la Ruina",
+        "FR": "Ronde des pens\u00e9es fan\u00e9es",
+        "ID": "Whimsical Dance of the Withered",
+        "IT": "Danza estrosa dei caduti",
+        "JP": "\u7570\u60f3\u304c\u67af\u308c\u843d\u3061\u308b\u5186\u821e",
+        "KR": "\uc601\ub77d\ud55c \uacf5\uc0c1\uc758 \uc648\uce20",
+        "PT": "Valsa Divergente dos Ca\u00eddos",
+        "RU": "\u0412\u0430\u043b\u044c\u0441 \u0443\u0432\u044f\u0434\u0448\u0438\u0445 \u0444\u0430\u043d\u0442\u0430\u0437\u0438\u0439",
+        "TH": "Whimsical Dance of the Withered",
+        "TR": "Solup Gidenin Tuhaf Dans\u0131",
+        "VI": "V\u0169 \u0110i\u1ec7u C\u1ee7a T\u00e0n Phai"
+    },
     "115138260": {
         "CHS": "\u9ad8\u5929\u7684\u98ce\u4e4b\u4e3b\u51a0",
         "DE": "Krone der himmlischen Winde",
         "EN": "Lord of Wind over Firmament's Crown",
         "ES": "Corona del Se\u00f1or de los Vientos Celestiales",
         "FR": "Couronne des Vents c\u00e9lestes",
         "ID": "Lord of Wind over Firmament's Crown",
@@ -4363,14 +4395,30 @@
         "KR": "\uc6a9\uc0ac\uc758 \ud6c8\uc7a5",
         "PT": "Medalha do Valente",
         "RU": "\u0411\u0440\u043e\u0448\u044c \u0445\u0440\u0430\u0431\u0440\u0435\u0446\u0430",
         "TH": "Medal of The Brave",
         "TR": "Cesurlar\u0131n Madalyas\u0131",
         "VI": "Huy Ch\u01b0\u01a1ng D\u0169ng S\u0129"
     },
+    "1255108572": {
+        "CHS": "\u4e3e\u4e1a\u7684\u8bc6\u523b",
+        "DE": "Augenblick des Erfolgs",
+        "EN": "Moment of Attainment",
+        "ES": "Momento de Aprehensi\u00f3n",
+        "FR": "Instant de r\u00e9alisation",
+        "ID": "Moment of Attainment",
+        "IT": "Momento di conquista",
+        "JP": "\u5927\u696d\u3092\u6210\u3059\u523b",
+        "KR": "\ub300\uc5c5\uc758 \uc2dc\uac04",
+        "PT": "Momento de Conquista",
+        "RU": "\u041c\u043e\u043c\u0435\u043d\u0442 \u043e\u0431\u0440\u0435\u0442\u0435\u043d\u0438\u044f",
+        "TH": "Moment of Attainment",
+        "TR": "Zafer An\u0131",
+        "VI": "Th\u1eddi Kh\u1eafc C\u1ee7a \u0110\u1ea1t Th\u00e0nh"
+    },
     "1255686932": {
         "CHS": "\u6c34\u4ed9\u7684\u65f6\u65f6\u523b\u523b",
         "DE": "Best\u00e4ndigkeit der Narzisse",
         "EN": "Nymph's Constancy",
         "ES": "Asiduidad de las Ninfas",
         "FR": "Constance de la nymphe",
         "ID": "Nymph's Constancy",
@@ -5627,14 +5675,30 @@
         "KR": "\uc2ec\ud310\uc758 \uc2dc\uac04",
         "PT": "Momento do Julgamento",
         "RU": "\u041c\u0433\u043d\u043e\u0432\u0435\u043d\u0438\u0435 \u043f\u0440\u0430\u0432\u043e\u0441\u0443\u0434\u0438\u044f",
         "TH": "Moment of Judgment",
         "TR": "Yarg\u0131 An\u0131",
         "VI": "Th\u1eddi Kh\u1eafc C\u1ee7a Ph\u00e1n Quy\u1ebft"
     },
+    "133613868": {
+        "CHS": "\u7b79\u8c0b\u7684\u5171\u6a3d",
+        "DE": "Weinflasche der Planung",
+        "EN": "The Wine-Flask Over Which the Plan Was Hatched",
+        "ES": "Jarra del Gran Plan",
+        "FR": "Coupe commune de strat\u00e9gie",
+        "ID": "The Wine-Flask Over Which the Plan Was Hatched",
+        "IT": "Calice dell'escogitativa",
+        "JP": "\u8a08\u7565\u306e\u76c3",
+        "KR": "\uacf5\ubaa8\uc758 \uc220\uc794",
+        "PT": "A Garrafa de Vinho Sobre a Qual o Plano Foi Concebido",
+        "RU": "\u0427\u0430\u0448\u0430 \u0437\u0430\u043c\u044b\u0441\u043b\u0430",
+        "TH": "The Wine-Flask Over Which the Plan Was Hatched",
+        "TR": "Plan\u0131n Haz\u0131rland\u0131\u011f\u0131 \u015earap Kadehi",
+        "VI": "Ly R\u01b0\u1ee3u C\u00f9ng B\u00e0y M\u01b0u"
+    },
     "1336456300": {
         "CHS": "\u8d24\u533b\u4e4b\u7fbd",
         "DE": "Feder der Genesung",
         "EN": "Wise Doctor's Pinion",
         "ES": "Pluma del Doctor Sabio",
         "FR": "Plume du sage docteur",
         "ID": "Wise Doctor's Pinion",
@@ -6267,14 +6331,30 @@
         "KR": "\ud559\uc0ac\uc758 \uba39\uc794",
         "PT": "C\u00e1lice de Tinta do Estudioso",
         "RU": "\u0427\u0435\u0440\u043d\u0438\u043b\u044c\u043d\u0438\u0446\u0430 \u0443\u0447\u0451\u043d\u043e\u0433\u043e",
         "TH": "Scholar's Ink Bottle",
         "TR": "Alimin M\u00fcrekkep Hokkas\u0131",
         "VI": "Ly M\u1ef1c H\u1ecdc S\u0129"
     },
+    "1364940700": {
+        "CHS": "\u8c10\u5f8b\u4ea4\u54cd\u7684\u524d\u594f",
+        "DE": "Vorspiel der harmonischen Sinfonie",
+        "EN": "Harmonious Symphony Prelude",
+        "ES": "Preludio de la Sinfon\u00eda Arm\u00f3nica",
+        "FR": "Pr\u00e9lude des symphonies harmoniques",
+        "ID": "Harmonious Symphony Prelude",
+        "IT": "Preludio della Sinfonia armonica",
+        "JP": "\u97ff\u304d\u5408\u3046\u8ae7\u5f8b\u306e\u524d\u594f",
+        "KR": "\uc870\ud654\ub85c\uc6b4 \uc804\uc8fc\uace1",
+        "PT": "Prel\u00fadio da Sinfonia Harmoniosa",
+        "RU": "\u0423\u0432\u0435\u0440\u0442\u044e\u0440\u0430 \u0441\u0442\u0440\u043e\u0439\u043d\u043e\u0439 \u0441\u0438\u043c\u0444\u043e\u043d\u0438\u0438",
+        "TH": "Harmonious Symphony Prelude",
+        "TR": "Ahenkli Senfoninin Ba\u015flang\u0131c\u0131",
+        "VI": "D\u1ea1o \u0110\u1ea7u C\u1ee7a Giao H\u01b0\u1edfng"
+    },
     "1365224652": {
         "CHS": "\u6559\u5b98\u7684\u7fbd\u9970",
         "DE": "Ausbilderfederschmuck",
         "EN": "Instructor's Feather Accessory",
         "ES": "Pluma del Instructor",
         "FR": "Plume de l'Instructeur",
         "ID": "Instructor's Feathered Accessory",
@@ -7099,14 +7179,30 @@
         "KR": "\ubc88\uac1c \uc7ac\uc559\uc758 \uc0dd\uc874\uc790",
         "PT": "Sobreviventes da Cat\u00e1strofe",
         "RU": "\u041f\u0435\u0440\u0435\u0436\u0438\u0432\u0448\u0438\u0439 \u043a\u0430\u0442\u0430\u0441\u0442\u0440\u043e\u0444\u0443",
         "TH": "Survivor of Catastrophe",
         "TR": "Felaketten Kurtulan",
         "VI": "Tai H\u1ecda C\u1ee7a S\u00e9t"
     },
+    "1422096748": {
+        "CHS": "\u7075\u9732\u503e\u6d12\u7684\u72c2\u8bd7",
+        "DE": "Rhapsodie des sprudelnden Ichors",
+        "EN": "Ichor Shower Rhapsody",
+        "ES": "Rapsodia del Icor Derramado",
+        "FR": "Rhapsodie de l'ichor d\u00e9vers\u00e9",
+        "ID": "Ichor Shower Rhapsody",
+        "IT": "Rapsodia di pioggia dell'Icore",
+        "JP": "\u964d\u308a\u6ce8\u3050\u30a4\u30b3\u30eb\u306e\u72c2\u8a69",
+        "KR": "\uc601\ud63c \uc774\uc2ac\uc758 \uad11\uc2dc\uace1",
+        "PT": "Raps\u00f3dia da Chuva de Icor",
+        "RU": "\u041d\u0435\u0438\u0441\u0442\u043e\u0432\u0430\u044f \u0440\u0430\u043f\u0441\u043e\u0434\u0438\u044f \u0438\u0445\u043e\u0440\u0430",
+        "TH": "Ichor Shower Rhapsody",
+        "TR": "\u0130khor Ya\u011fmuru Rapsodisi",
+        "VI": "\u00c1ng Th\u01a1 C\u1ee7a Linh L\u1ed9"
+    },
     "1422661004": {
         "CHS": "\u89d2\u6597\u58eb\u7684\u5e0c\u5180",
         "DE": "Zuversicht des Gladiators",
         "EN": "Gladiator's Longing",
         "ES": "Esperanza del Gladiador",
         "FR": "Espoir du Gladiateur",
         "ID": "Gladiator's Longing",
@@ -9803,14 +9899,30 @@
         "KR": "\uc131\ub77c\uaddc\ubcbd\uc758 \uc2dc\uacc4",
         "PT": "Rel\u00f3gio de Sol de Jade Duradouro",
         "RU": "\u0427\u0430\u0441\u044b \u0438\u0437 \u043f\u0440\u043e\u0447\u043d\u043e\u0433\u043e \u043d\u0435\u0444\u0440\u0438\u0442\u0430",
         "TH": "Sundial of Enduring Jade",
         "TR": "Dayan\u0131kl\u0131 Ye\u015fim G\u00fcne\u015f Saati",
         "VI": "C\u00e1t Tinh \u0110\u00e0"
     },
+    "1584886164": {
+        "CHS": "\u6697\u7ed3\u7684\u660e\u82b1",
+        "DE": "Helle Bl\u00fcte dunkler Fr\u00fcchte",
+        "EN": "Dark Fruit of Bright Flowers",
+        "ES": "Flor Secreta Rutilante",
+        "FR": "Fleur de n\u0153uds dissimul\u00e9s",
+        "ID": "Dark Fruit of Bright Flowers",
+        "IT": "Frutto fosco di fiori limpidi",
+        "JP": "\u9670\u306b\u54b2\u304f\u5149\u306e\u82b1",
+        "KR": "\uc5b4\ub460 \uc18d\uc758 \ubc1d\uc740 \uaf43",
+        "PT": "Fruto Sombrio de Flores Brilhantes",
+        "RU": "\u0422\u0451\u043c\u043d\u044b\u0439 \u043f\u043b\u043e\u0434 \u044f\u0440\u043a\u0438\u0445 \u0446\u0432\u0435\u0442\u043e\u0432",
+        "TH": "Dark Fruit of Bright Flowers",
+        "TR": "Parlak \u00c7i\u00e7eklerin Koyu Meyvesi",
+        "VI": "Hoa S\u00e1ng C\u1ee7a Qu\u1ea3 \u0110en"
+    },
     "1587172172": {
         "CHS": "\u91ce\u82b1\u8bb0\u5fc6\u7684\u7eff\u91ce",
         "DE": "Feldj\u00e4gerblume",
         "EN": "In Remembrance of Viridescent Fields",
         "ES": "Recuerdo de Flores Silvestres",
         "FR": "Souvenir de fleur des champs",
         "ID": "In Rememberance of Viridescent Field",
@@ -11339,14 +11451,30 @@
         "KR": "\ub3c4\uae08 \ube0c\ub85c\uce58",
         "PT": "Broche Dourado",
         "RU": "\u041f\u043e\u0437\u043e\u043b\u043e\u0447\u0435\u043d\u043d\u0430\u044f \u0431\u0440\u043e\u0448\u044c",
         "TH": "Gilded Corsage",
         "TR": "Yald\u0131zl\u0131 Bro\u015f",
         "VI": "Hoa C\u00e0i V\u00e0ng"
     },
+    "1674295492": {
+        "CHS": "\u7b79\u8c0b\u7684\u5171\u6a3d",
+        "DE": "Weinflasche der Planung",
+        "EN": "The Wine-Flask Over Which the Plan Was Hatched",
+        "ES": "Jarra del Gran Plan",
+        "FR": "Coupe commune de strat\u00e9gie",
+        "ID": "The Wine-Flask Over Which the Plan Was Hatched",
+        "IT": "Calice dell'escogitativa",
+        "JP": "\u8a08\u7565\u306e\u76c3",
+        "KR": "\uacf5\ubaa8\uc758 \uc220\uc794",
+        "PT": "A Garrafa de Vinho Sobre a Qual o Plano Foi Concebido",
+        "RU": "\u0427\u0430\u0448\u0430 \u0437\u0430\u043c\u044b\u0441\u043b\u0430",
+        "TH": "The Wine-Flask Over Which the Plan Was Hatched",
+        "TR": "Plan\u0131n Haz\u0131rland\u0131\u011f\u0131 \u015earap Kadehi",
+        "VI": "Ly R\u01b0\u1ee3u C\u00f9ng B\u00e0y M\u01b0u"
+    },
     "1676197220": {
         "CHS": "\u8ff7\u8bef\u8005\u4e4b\u706f",
         "DE": "Lampe des Verirrten",
         "EN": "Lamp of the Lost",
         "ES": "L\u00e1mpara del Exilio",
         "FR": "Lampe des perdus",
         "ID": "Lamp of the Lost",
@@ -11547,14 +11675,30 @@
         "KR": "\uc6a9\uc0ac\uc758 \uae30\ub300",
         "PT": "Esperan\u00e7a do Valente",
         "RU": "\u041d\u0430\u0434\u0435\u0436\u0434\u044b \u0445\u0440\u0430\u0431\u0440\u0435\u0446\u0430",
         "TH": "Prospect of the Brave",
         "TR": "Cesurlar\u0131n Aray\u0131\u015f\u0131",
         "VI": "S\u1ef1 Mong \u0110\u1ee3i C\u1ee7a D\u0169ng S\u0129"
     },
+    "1691105380": {
+        "CHS": "\u7075\u9732\u503e\u6d12\u7684\u72c2\u8bd7",
+        "DE": "Rhapsodie des sprudelnden Ichors",
+        "EN": "Ichor Shower Rhapsody",
+        "ES": "Rapsodia del Icor Derramado",
+        "FR": "Rhapsodie de l'ichor d\u00e9vers\u00e9",
+        "ID": "Ichor Shower Rhapsody",
+        "IT": "Rapsodia di pioggia dell'Icore",
+        "JP": "\u964d\u308a\u6ce8\u3050\u30a4\u30b3\u30eb\u306e\u72c2\u8a69",
+        "KR": "\uc601\ud63c \uc774\uc2ac\uc758 \uad11\uc2dc\uace1",
+        "PT": "Raps\u00f3dia da Chuva de Icor",
+        "RU": "\u041d\u0435\u0438\u0441\u0442\u043e\u0432\u0430\u044f \u0440\u0430\u043f\u0441\u043e\u0434\u0438\u044f \u0438\u0445\u043e\u0440\u0430",
+        "TH": "Ichor Shower Rhapsody",
+        "TR": "\u0130khor Ya\u011fmuru Rapsodisi",
+        "VI": "\u00c1ng Th\u01a1 C\u1ee7a Linh L\u1ed9"
+    },
     "1691841340": {
         "CHS": "\u6467\u51b0\u800c\u884c\u7684\u6267\u671b",
         "DE": "Resolution des Schneestapfers",
         "EN": "Icebreaker's Resolve",
         "ES": "Obstinaci\u00f3n Perforahielos",
         "FR": "R\u00e9solution du Briseur de glace",
         "ID": "Icebreaker's Resolve",
@@ -13067,14 +13211,30 @@
         "KR": "\uae30\uc801\uc758 \uc794",
         "PT": "C\u00e1lice do Milagre",
         "RU": "\u0427\u0430\u0448\u043a\u0430 \u043c\u0430\u043b\u0435\u043d\u044c\u043a\u043e\u0433\u043e \u0447\u0443\u0434\u0430",
         "TH": "Tiny Miracle's Goblet",
         "TR": "K\u00fc\u00e7\u00fck Mucizenin Kadehi",
         "VI": "Ly K\u1ef3 T\u00edch"
     },
+    "1794117964": {
+        "CHS": "\u6697\u7ed3\u7684\u660e\u82b1",
+        "DE": "Helle Bl\u00fcte dunkler Fr\u00fcchte",
+        "EN": "Dark Fruit of Bright Flowers",
+        "ES": "Flor Secreta Rutilante",
+        "FR": "Fleur de n\u0153uds dissimul\u00e9s",
+        "ID": "Dark Fruit of Bright Flowers",
+        "IT": "Frutto fosco di fiori limpidi",
+        "JP": "\u9670\u306b\u54b2\u304f\u5149\u306e\u82b1",
+        "KR": "\uc5b4\ub460 \uc18d\uc758 \ubc1d\uc740 \uaf43",
+        "PT": "Fruto Sombrio de Flores Brilhantes",
+        "RU": "\u0422\u0451\u043c\u043d\u044b\u0439 \u043f\u043b\u043e\u0434 \u044f\u0440\u043a\u0438\u0445 \u0446\u0432\u0435\u0442\u043e\u0432",
+        "TH": "Dark Fruit of Bright Flowers",
+        "TR": "Parlak \u00c7i\u00e7eklerin Koyu Meyvesi",
+        "VI": "Hoa S\u00e1ng C\u1ee7a Qu\u1ea3 \u0110en"
+    },
     "1794180868": {
         "CHS": "\u6218\u72c2\u7684\u9b3c\u9762",
         "DE": "Furchteinfl\u00f6\u00dfende Berserkermaske",
         "EN": "Berserker's Battle Mask",
         "ES": "M\u00e1scara de Batalla del Berserker",
         "FR": "Masque du Berserker",
         "ID": "Berserker's Battle Mask",
@@ -13355,14 +13515,30 @@
         "KR": "\ubaa8\ud5d8\uac00\uc758 \uba38\ub9ac\ub760",
         "PT": "Bandana de Aventureiro",
         "RU": "\u041f\u043e\u0432\u044f\u0437\u043a\u0430 \u0438\u0441\u043a\u0430\u0442\u0435\u043b\u044f \u043f\u0440\u0438\u043a\u043b\u044e\u0447\u0435\u043d\u0438\u0439",
         "TH": "Adventurer's Bandana",
         "TR": "Macerac\u0131n\u0131n Bandanas\u0131",
         "VI": "Kh\u0103n Nh\u00e0 M\u1ea1o Hi\u1ec3m"
     },
+    "1809415524": {
+        "CHS": "\u8c10\u5f8b\u4ea4\u54cd\u7684\u524d\u594f",
+        "DE": "Vorspiel der harmonischen Sinfonie",
+        "EN": "Harmonious Symphony Prelude",
+        "ES": "Preludio de la Sinfon\u00eda Arm\u00f3nica",
+        "FR": "Pr\u00e9lude des symphonies harmoniques",
+        "ID": "Harmonious Symphony Prelude",
+        "IT": "Preludio della Sinfonia armonica",
+        "JP": "\u97ff\u304d\u5408\u3046\u8ae7\u5f8b\u306e\u524d\u594f",
+        "KR": "\uc870\ud654\ub85c\uc6b4 \uc804\uc8fc\uace1",
+        "PT": "Prel\u00fadio da Sinfonia Harmoniosa",
+        "RU": "\u0423\u0432\u0435\u0440\u0442\u044e\u0440\u0430 \u0441\u0442\u0440\u043e\u0439\u043d\u043e\u0439 \u0441\u0438\u043c\u0444\u043e\u043d\u0438\u0438",
+        "TH": "Harmonious Symphony Prelude",
+        "TR": "Ahenkli Senfoninin Ba\u015flang\u0131c\u0131",
+        "VI": "D\u1ea1o \u0110\u1ea7u C\u1ee7a Giao H\u01b0\u1edfng"
+    },
     "1809600972": {
         "CHS": "\u5c11\u5973\u6613\u901d\u7684\u82b3\u989c",
         "DE": "Verg\u00e4nglichkeit der Maid",
         "EN": "Maiden's Fading Beauty",
         "ES": "Belleza Desvanecida de la Doncella",
         "FR": "Beaut\u00e9 fugace de la Demoiselle",
         "ID": "Maiden's Fading Beauty",
@@ -13659,14 +13835,30 @@
         "KR": "\ubc14\ub78c \uad70\uc8fc\uc758 \uae43\ud138",
         "PT": "Pluma dos Ventos Celestiais",
         "RU": "\u041f\u0435\u0440\u043e \u0445\u043e\u0437\u044f\u0438\u043d\u0430 \u0432\u0435\u0442\u0440\u043e\u0432",
         "TH": "Lord of Wind over Firmament's Feather",
         "TR": "G\u00f6kkubbe R\u00fczgar\u0131 Efendisinin T\u00fcy\u00fc",
         "VI": "L\u00f4ng V\u0169 Ng\u1ecdn Gi\u00f3 Tr\u1eddi Cao"
     },
+    "1827685724": {
+        "CHS": "\u547d\u9014\u8f6e\u8f6c\u7684\u8c10\u8c11",
+        "DE": "R\u00e4tsel der Wendung des Schicksals",
+        "EN": "The Grand Jape of the Turning of Fate",
+        "ES": "Gran Burla del Giro del Destino",
+        "FR": "Farce des changements du destin",
+        "ID": "The Grand Jape of the Turning of Fate",
+        "IT": "Grande scherzo del destino",
+        "JP": "\u904b\u547d\u3068\u8f2a\u5efb\u306e\u8ae7\u8b14",
+        "KR": "\uad6c\ub974\ub294 \uc6b4\uba85\uc758 \ud574\ud559\uace1",
+        "PT": "A Grande Farsa da Volta do Destino",
+        "RU": "\u0421\u043a\u0435\u0440\u0446\u043e \u043f\u043e\u0432\u043e\u0440\u043e\u0442\u043e\u0432 \u0441\u0443\u0434\u044c\u0431\u044b",
+        "TH": "The Grand Jape of the Turning of Fate",
+        "TR": "Kader D\u00f6ng\u00fcs\u00fcn\u00fcn B\u00fcy\u00fck Oyunu",
+        "VI": "Tr\u00eau Ng\u01b0\u01a1i C\u1ee7a V\u1eadn M\u1ec7nh"
+    },
     "1828983796": {
         "CHS": "\u5b66\u58eb\u7684\u4e66\u7b7e",
         "DE": "Gelehrtenlesezeichen",
         "EN": "Scholar's Bookmark",
         "ES": "Marcap\u00e1ginas de la Erudita",
         "FR": "Marque-page de l'\u00c9rudit",
         "ID": "Scholar's Bookmark",
@@ -13675,14 +13867,30 @@
         "KR": "\ud559\uc0ac\uc758 \ucc45\uac08\ud53c",
         "PT": "Marca-p\u00e1ginas de Estudioso",
         "RU": "\u0417\u0430\u043a\u043b\u0430\u0434\u043a\u0430 \u0443\u0447\u0451\u043d\u043e\u0433\u043e",
         "TH": "Scholar's Bookmark",
         "TR": "Alimin Kitap Ayrac\u0131",
         "VI": "K\u1eb9p S\u00e1ch H\u1ecdc S\u0129"
     },
+    "1829870716": {
+        "CHS": "\u7075\u9732\u503e\u6d12\u7684\u72c2\u8bd7",
+        "DE": "Rhapsodie des sprudelnden Ichors",
+        "EN": "Ichor Shower Rhapsody",
+        "ES": "Rapsodia del Icor Derramado",
+        "FR": "Rhapsodie de l'ichor d\u00e9vers\u00e9",
+        "ID": "Ichor Shower Rhapsody",
+        "IT": "Rapsodia di pioggia dell'Icore",
+        "JP": "\u964d\u308a\u6ce8\u3050\u30a4\u30b3\u30eb\u306e\u72c2\u8a69",
+        "KR": "\uc601\ud63c \uc774\uc2ac\uc758 \uad11\uc2dc\uace1",
+        "PT": "Raps\u00f3dia da Chuva de Icor",
+        "RU": "\u041d\u0435\u0438\u0441\u0442\u043e\u0432\u0430\u044f \u0440\u0430\u043f\u0441\u043e\u0434\u0438\u044f \u0438\u0445\u043e\u0440\u0430",
+        "TH": "Ichor Shower Rhapsody",
+        "TR": "\u0130khor Ya\u011fmuru Rapsodisi",
+        "VI": "\u00c1ng Th\u01a1 C\u1ee7a Linh L\u1ed9"
+    },
     "1830201900": {
         "CHS": "\u5dc9\u5ca9\u7422\u5851\u4e4b\u6a3d",
         "DE": "Krug aus Felsgestein",
         "EN": "Goblet of Chiseled Crag",
         "ES": "C\u00e1liz del Escultor de Monta\u00f1as",
         "FR": "Coupe en roche escarp\u00e9e",
         "ID": "Goblet of Chiseled Crag",
@@ -13787,14 +13995,30 @@
         "KR": "\uae30\uc801\uc758 \uadc0\uac78\uc774",
         "PT": "Brincos do Milagre",
         "RU": "\u0421\u0435\u0440\u0451\u0436\u043a\u0438 \u043c\u0430\u043b\u0435\u043d\u044c\u043a\u043e\u0433\u043e \u0447\u0443\u0434\u0430",
         "TH": "Tiny Miracle's Earrings",
         "TR": "K\u00fc\u00e7\u00fck Mucizenin K\u00fcpeleri",
         "VI": "B\u00f4ng Tai K\u1ef3 T\u00edch"
     },
+    "1840057148": {
+        "CHS": "\u6697\u7ed3\u7684\u660e\u82b1",
+        "DE": "Helle Bl\u00fcte dunkler Fr\u00fcchte",
+        "EN": "Dark Fruit of Bright Flowers",
+        "ES": "Flor Secreta Rutilante",
+        "FR": "Fleur de n\u0153uds dissimul\u00e9s",
+        "ID": "Dark Fruit of Bright Flowers",
+        "IT": "Frutto fosco di fiori limpidi",
+        "JP": "\u9670\u306b\u54b2\u304f\u5149\u306e\u82b1",
+        "KR": "\uc5b4\ub460 \uc18d\uc758 \ubc1d\uc740 \uaf43",
+        "PT": "Fruto Sombrio de Flores Brilhantes",
+        "RU": "\u0422\u0451\u043c\u043d\u044b\u0439 \u043f\u043b\u043e\u0434 \u044f\u0440\u043a\u0438\u0445 \u0446\u0432\u0435\u0442\u043e\u0432",
+        "TH": "Dark Fruit of Bright Flowers",
+        "TR": "Parlak \u00c7i\u00e7eklerin Koyu Meyvesi",
+        "VI": "Hoa S\u00e1ng C\u1ee7a Qu\u1ea3 \u0110en"
+    },
     "1840901268": {
         "CHS": "\u5b97\u5ba4\u94f6\u74ee",
         "DE": "K\u00f6niglicher Silberkrug",
         "EN": "Royal Silver Urn",
         "ES": "Urna Plateada Real",
         "FR": "Urne d'argent du Noble",
         "ID": "Royal Silver Urn",
@@ -13995,14 +14219,30 @@
         "KR": "\ub9c8\ub140\uc758 \uc5fc\ud654 \uaf43",
         "PT": "Flor de Labareda da Bruxa",
         "RU": "\u0412\u0435\u0434\u044c\u043c\u0438\u043d \u043e\u0433\u043d\u0435\u043d\u043d\u044b\u0439 \u0446\u0432\u0435\u0442\u043e\u043a",
         "TH": "Witch's Flower of Blaze",
         "TR": "Cad\u0131n\u0131n Alev \u00c7i\u00e7e\u011fi",
         "VI": "Hoa L\u1eeda C\u1ee7a Ma N\u1eef"
     },
+    "1854618132": {
+        "CHS": "\u53e4\u6d77\u7384\u5e7d\u7684\u591c\u60f3",
+        "DE": "N\u00e4chtliches Gr\u00fcbeln der uralten See",
+        "EN": "Ancient Sea's Nocturnal Musing",
+        "ES": "Nocturno del Mar de Anta\u00f1o",
+        "FR": "R\u00eaverie des eaux antiques",
+        "ID": "Ancient Sea's Nocturnal Musing",
+        "IT": "Riflessione notturna del Mare Antico",
+        "JP": "\u53e4\u6d77\u306e\u5e7d\u6df1\u306a\u308b\u591c\u60f3",
+        "KR": "\uace0\ub300 \ubc14\ub2e4\uc758 \uc57c\uc0c1\uace1",
+        "PT": "Reflex\u00e3o Noturna do Mar Antigo",
+        "RU": "\u041d\u043e\u0447\u043d\u044b\u0435 \u0440\u0430\u0437\u0434\u0443\u043c\u044c\u044f \u0434\u0440\u0435\u0432\u043d\u0435\u0433\u043e \u043c\u043e\u0440\u044f",
+        "TH": "Ancient Sea's Nocturnal Musing",
+        "TR": "Kadim Deniz'in Gece D\u00fc\u015f\u00fcnceleri",
+        "VI": "D\u1ea1 T\u1ea5u C\u1ee7a Bi\u1ec3n X\u01b0a"
+    },
     "1854905796": {
         "CHS": "\u8363\u82b1\u4e4b\u671f",
         "DE": "Bl\u00fcte der Glorie",
         "EN": "Bloom Times",
         "ES": "Era del Esplendor",
         "FR": "P\u00e9riode de floraison",
         "ID": "Bloom Times",
@@ -14251,14 +14491,30 @@
         "KR": "\ub178\ub984\uafbc\uc758 \uadc0\uac78\uc774",
         "PT": "Brincos de Apostador",
         "RU": "\u0421\u0435\u0440\u0451\u0436\u043a\u0438 \u0430\u0437\u0430\u0440\u0442\u043d\u043e\u0433\u043e \u0438\u0433\u0440\u043e\u043a\u0430",
         "TH": "Gambler's Earrings",
         "TR": "Kumarbaz\u0131n K\u00fcpeleri",
         "VI": "Hoa Tai Con B\u1ea1c"
     },
+    "1867205412": {
+        "CHS": "\u7075\u9732\u503e\u6d12\u7684\u72c2\u8bd7",
+        "DE": "Rhapsodie des sprudelnden Ichors",
+        "EN": "Ichor Shower Rhapsody",
+        "ES": "Rapsodia del Icor Derramado",
+        "FR": "Rhapsodie de l'ichor d\u00e9vers\u00e9",
+        "ID": "Ichor Shower Rhapsody",
+        "IT": "Rapsodia di pioggia dell'Icore",
+        "JP": "\u964d\u308a\u6ce8\u3050\u30a4\u30b3\u30eb\u306e\u72c2\u8a69",
+        "KR": "\uc601\ud63c \uc774\uc2ac\uc758 \uad11\uc2dc\uace1",
+        "PT": "Raps\u00f3dia da Chuva de Icor",
+        "RU": "\u041d\u0435\u0438\u0441\u0442\u043e\u0432\u0430\u044f \u0440\u0430\u043f\u0441\u043e\u0434\u0438\u044f \u0438\u0445\u043e\u0440\u0430",
+        "TH": "Ichor Shower Rhapsody",
+        "TR": "\u0130khor Ya\u011fmuru Rapsodisi",
+        "VI": "\u00c1ng Th\u01a1 C\u1ee7a Linh L\u1ed9"
+    },
     "1868002956": {
         "CHS": "\u5b66\u58eb\u7684\u955c\u7247",
         "DE": "Gelehrtenmonokel",
         "EN": "Scholar's Lens",
         "ES": "Mon\u00f3culo de la Erudita",
         "FR": "Lunettes de l'\u00c9rudit",
         "ID": "Scholar's Glasses",
@@ -14795,14 +15051,30 @@
         "KR": "\ubaa8\ud5d8\uac00\uc758 \uba38\ub9ac\ub760",
         "PT": "Bandana de Aventureiro",
         "RU": "\u041f\u043e\u0432\u044f\u0437\u043a\u0430 \u0438\u0441\u043a\u0430\u0442\u0435\u043b\u044f \u043f\u0440\u0438\u043a\u043b\u044e\u0447\u0435\u043d\u0438\u0439",
         "TH": "Adventurer's Bandana",
         "TR": "Macerac\u0131n\u0131n Bandanas\u0131",
         "VI": "Kh\u0103n Nh\u00e0 M\u1ea1o Hi\u1ec3m"
     },
+    "1896095676": {
+        "CHS": "\u4e3e\u4e1a\u7684\u8bc6\u523b",
+        "DE": "Augenblick des Erfolgs",
+        "EN": "Moment of Attainment",
+        "ES": "Momento de Aprehensi\u00f3n",
+        "FR": "Instant de r\u00e9alisation",
+        "ID": "Moment of Attainment",
+        "IT": "Momento di conquista",
+        "JP": "\u5927\u696d\u3092\u6210\u3059\u523b",
+        "KR": "\ub300\uc5c5\uc758 \uc2dc\uac04",
+        "PT": "Momento de Conquista",
+        "RU": "\u041c\u043e\u043c\u0435\u043d\u0442 \u043e\u0431\u0440\u0435\u0442\u0435\u043d\u0438\u044f",
+        "TH": "Moment of Attainment",
+        "TR": "Zafer An\u0131",
+        "VI": "Th\u1eddi Kh\u1eafc C\u1ee7a \u0110\u1ea1t Th\u00e0nh"
+    },
     "189946132": {
         "CHS": "\u5e73\u96f7\u4e4b\u7fbd",
         "DE": "Feder des Donnerb\u00e4ndigers",
         "EN": "Thundersoother's Plume",
         "ES": "Pluma del Domador de Truenos",
         "FR": "Plume du Dompteur de foudre",
         "ID": "Thundersoother's Plume",
@@ -15259,14 +15531,30 @@
         "KR": "\uc218\ud638\uc758 \uaf43",
         "PT": "Flor do Guarda",
         "RU": "\u0426\u0432\u0435\u0442\u043e\u043a \u0437\u0430\u0449\u0438\u0442\u043d\u0438\u043a\u0430",
         "TH": "Guardian's Flower",
         "TR": "Muhaf\u0131z \u00c7i\u00e7e\u011fi",
         "VI": "Hoa Th\u1ee7 H\u1ed9"
     },
+    "1917296060": {
+        "CHS": "\u5931\u5195\u7684\u5b9d\u51a0",
+        "DE": "Kronenlose Krone",
+        "EN": "Crownless Crown",
+        "ES": "Corona Descoronada",
+        "FR": "Couronne sans couronne",
+        "ID": "Crownless Crown",
+        "IT": "Corona senza corona",
+        "JP": "\u4e3b\u306a\u304d\u51a0",
+        "KR": "\uc8fc\uc778 \uc783\uc740 \uc655\uad00",
+        "PT": "Coroa Descoroada",
+        "RU": "\u041d\u0435\u0432\u0435\u043d\u0447\u0430\u043d\u043d\u0430\u044f \u043a\u043e\u0440\u043e\u043d\u0430",
+        "TH": "Crownless Crown",
+        "TR": "Sahipsiz Ta\u00e7",
+        "VI": "V\u01b0\u01a1ng Mi\u1ec7n Qu\u00fd Kh\u00f4ng Ngai"
+    },
     "1918993596": {
         "CHS": "\u5f52\u4e61\u4e4b\u7fbd",
         "DE": "Feder der Heimkehr",
         "EN": "Feather of Homecoming",
         "ES": "Pluma del Retorno",
         "FR": "Plume du Voyageur",
         "ID": "Feather of Homecoming",
@@ -16411,14 +16699,30 @@
         "KR": "\ubd88 \uc704\ub97c \uac77\ub294 \uc790\uc758 \uae68\ub2ec\uc74c",
         "PT": "Despertamento do Corredor de Lava",
         "RU": "\u041f\u0440\u043e\u0441\u0432\u0435\u0442\u043b\u0435\u043d\u0438\u0435 \u0441\u0442\u0443\u043f\u0430\u044e\u0449\u0435\u0433\u043e \u043f\u043e \u043b\u0430\u0432\u0435",
         "TH": "Epiphany of Lavawalker",
         "TR": "Lavdagezenin Uyan\u0131\u015f\u0131",
         "VI": "S\u1ef1 T\u1ec9nh Ng\u1ed9 C\u1ee7a Ng\u01b0\u1eddi V\u01b0\u1ee3t L\u1eeda"
     },
+    "1990912852": {
+        "CHS": "\u892a\u5149\u7684\u7fe0\u5c3e",
+        "DE": "Verblasste Smaragdschwanzfeder",
+        "EN": "Faded Emerald Tail",
+        "ES": "Cola Esmeralda Descolorida",
+        "FR": "Queue \u00e9meraude de fanaison",
+        "ID": "Faded Emerald Tail",
+        "IT": "Coda smeraldina scolorita",
+        "JP": "\u5149\u892a\u305b\u305f\u7fe0\u5c3e",
+        "KR": "\ube5b\ubc14\ub79c \ud478\ub978 \uaf41\uc9c0",
+        "PT": "Cauda de Esmeralda Desbotada",
+        "RU": "\u0411\u043b\u0451\u043a\u043b\u044b\u0439 \u0438\u0437\u0443\u043c\u0440\u0443\u0434\u043d\u044b\u0439 \u0445\u0432\u043e\u0441\u0442",
+        "TH": "Faded Emerald Tail",
+        "TR": "Solmu\u015f Z\u00fcmr\u00fct Kuyruk",
+        "VI": "\u0110u\u00f4i Ph\u1ec9 Th\u00fay Phai M\u00e0u"
+    },
     "199095372": {
         "CHS": "\u51db\u51ac\u971c\u5fc3",
         "DE": "Herz des Frosts",
         "EN": "Heart of Frost",
         "ES": "Coraz\u00f3n de Escarcha",
         "FR": "C\u0153ur givreux de l'hiver",
         "ID": "Heart of Frost",
@@ -18427,14 +18731,30 @@
         "KR": "\uc2ec\ud310\uc758 \ub0a0\uac1c",
         "PT": "Pluma do Julgamento",
         "RU": "\u041f\u0435\u0440\u043e \u0441\u0443\u0436\u0434\u0435\u043d\u0438\u044f",
         "TH": "Feather of Judgment",
         "TR": "Yarg\u0131 T\u00fcy\u00fc",
         "VI": "L\u00f4ng V\u0169 Ph\u00e1n Quy\u1ebft"
     },
+    "2117798972": {
+        "CHS": "\u53e4\u6d77\u7384\u5e7d\u7684\u591c\u60f3",
+        "DE": "N\u00e4chtliches Gr\u00fcbeln der uralten See",
+        "EN": "Ancient Sea's Nocturnal Musing",
+        "ES": "Nocturno del Mar de Anta\u00f1o",
+        "FR": "R\u00eaverie des eaux antiques",
+        "ID": "Ancient Sea's Nocturnal Musing",
+        "IT": "Riflessione notturna del Mare Antico",
+        "JP": "\u53e4\u6d77\u306e\u5e7d\u6df1\u306a\u308b\u591c\u60f3",
+        "KR": "\uace0\ub300 \ubc14\ub2e4\uc758 \uc57c\uc0c1\uace1",
+        "PT": "Reflex\u00e3o Noturna do Mar Antigo",
+        "RU": "\u041d\u043e\u0447\u043d\u044b\u0435 \u0440\u0430\u0437\u0434\u0443\u043c\u044c\u044f \u0434\u0440\u0435\u0432\u043d\u0435\u0433\u043e \u043c\u043e\u0440\u044f",
+        "TH": "Ancient Sea's Nocturnal Musing",
+        "TR": "Kadim Deniz'in Gece D\u00fc\u015f\u00fcnceleri",
+        "VI": "D\u1ea1 T\u1ea5u C\u1ee7a Bi\u1ec3n X\u01b0a"
+    },
     "2118496724": {
         "CHS": "\u76df\u8a93\u91d1\u7235",
         "DE": "Edler Schwurkrug",
         "EN": "Noble's Pledging Vessel",
         "ES": "Copa del Juramento",
         "FR": "Coupe du serment",
         "ID": "Noble's Pledging Vessel",
@@ -20427,14 +20747,30 @@
         "KR": "\uae30\uc801\uc758 \ubaa8\ub798",
         "PT": "Ampulheta do Milagre",
         "RU": "\u041f\u0435\u0441\u043e\u0447\u043d\u044b\u0435 \u0447\u0430\u0441\u044b \u043c\u0430\u043b\u0435\u043d\u044c\u043a\u043e\u0433\u043e \u0447\u0443\u0434\u0430",
         "TH": "Tiny Miracle's Hourglass",
         "TR": "K\u00fc\u00e7\u00fck Mucizenin Kum Saati",
         "VI": "C\u00e1t K\u1ef3 T\u00edch"
     },
+    "2256184652": {
+        "CHS": "\u547d\u9014\u8f6e\u8f6c\u7684\u8c10\u8c11",
+        "DE": "R\u00e4tsel der Wendung des Schicksals",
+        "EN": "The Grand Jape of the Turning of Fate",
+        "ES": "Gran Burla del Giro del Destino",
+        "FR": "Farce des changements du destin",
+        "ID": "The Grand Jape of the Turning of Fate",
+        "IT": "Grande scherzo del destino",
+        "JP": "\u904b\u547d\u3068\u8f2a\u5efb\u306e\u8ae7\u8b14",
+        "KR": "\uad6c\ub974\ub294 \uc6b4\uba85\uc758 \ud574\ud559\uace1",
+        "PT": "A Grande Farsa da Volta do Destino",
+        "RU": "\u0421\u043a\u0435\u0440\u0446\u043e \u043f\u043e\u0432\u043e\u0440\u043e\u0442\u043e\u0432 \u0441\u0443\u0434\u044c\u0431\u044b",
+        "TH": "The Grand Jape of the Turning of Fate",
+        "TR": "Kader D\u00f6ng\u00fcs\u00fcn\u00fcn B\u00fcy\u00fck Oyunu",
+        "VI": "Tr\u00eau Ng\u01b0\u01a1i C\u1ee7a V\u1eadn M\u1ec7nh"
+    },
     "2258251212": {
         "CHS": "\u6b66\u4eba\u7684\u7ea2\u82b1",
         "DE": "Rote Kampfk\u00fcnstlerblume",
         "EN": "Martial Artist's Red Flower",
         "ES": "Flor Roja del Artista Marcial",
         "FR": "Fleur \u00e9carlate de l'Artiste martial",
         "ID": "Martial Artist's Red Flower",
@@ -21451,14 +21787,30 @@
         "KR": "\uc81c\uc218\uc758 \uad00",
         "PT": "Coroa do Ritual Hydro",
         "RU": "\u0422\u0438\u0430\u0440\u0430 \u0432\u043e\u0434\u044b",
         "TH": "Tiara of Torrents",
         "TR": "Sa\u011fanak Tac\u0131",
         "VI": "N\u00f3n T\u1ebf Th\u1ee7y"
     },
+    "2328442068": {
+        "CHS": "\u547d\u9014\u8f6e\u8f6c\u7684\u8c10\u8c11",
+        "DE": "R\u00e4tsel der Wendung des Schicksals",
+        "EN": "The Grand Jape of the Turning of Fate",
+        "ES": "Gran Burla del Giro del Destino",
+        "FR": "Farce des changements du destin",
+        "ID": "The Grand Jape of the Turning of Fate",
+        "IT": "Grande scherzo del destino",
+        "JP": "\u904b\u547d\u3068\u8f2a\u5efb\u306e\u8ae7\u8b14",
+        "KR": "\uad6c\ub974\ub294 \uc6b4\uba85\uc758 \ud574\ud559\uace1",
+        "PT": "A Grande Farsa da Volta do Destino",
+        "RU": "\u0421\u043a\u0435\u0440\u0446\u043e \u043f\u043e\u0432\u043e\u0440\u043e\u0442\u043e\u0432 \u0441\u0443\u0434\u044c\u0431\u044b",
+        "TH": "The Grand Jape of the Turning of Fate",
+        "TR": "Kader D\u00f6ng\u00fcs\u00fcn\u00fcn B\u00fcy\u00fck Oyunu",
+        "VI": "Tr\u00eau Ng\u01b0\u01a1i C\u1ee7a V\u1eadn M\u1ec7nh"
+    },
     "2328804548": {
         "CHS": "\u6e38\u533b\u7684\u94f6\u83b2",
         "DE": "Wanderarztanemone",
         "EN": "Traveling Doctor's Silver Lotus",
         "ES": "Loto de Plata de la M\u00e9dica Itinerante",
         "FR": "An\u00e9mone du M\u00e9decin itin\u00e9rant",
         "ID": "Traveling Doctor's Silver Lotus",
@@ -25083,14 +25435,30 @@
         "KR": "\uc790\uc218\uc815 \ud654\uad00",
         "PT": "Coroa Ametista",
         "RU": "\u0410\u043c\u0435\u0442\u0438\u0441\u0442\u043e\u0432\u044b\u0439 \u0432\u0435\u043d\u0435\u0446",
         "TH": "Amethyst Crown",
         "TR": "Ametist Ta\u00e7",
         "VI": "V\u01b0\u01a1ng Mi\u1ec7n T\u1eed Tinh"
     },
+    "2551385844": {
+        "CHS": "\u8c10\u5f8b\u4ea4\u54cd\u7684\u524d\u594f",
+        "DE": "Vorspiel der harmonischen Sinfonie",
+        "EN": "Harmonious Symphony Prelude",
+        "ES": "Preludio de la Sinfon\u00eda Arm\u00f3nica",
+        "FR": "Pr\u00e9lude des symphonies harmoniques",
+        "ID": "Harmonious Symphony Prelude",
+        "IT": "Preludio della Sinfonia armonica",
+        "JP": "\u97ff\u304d\u5408\u3046\u8ae7\u5f8b\u306e\u524d\u594f",
+        "KR": "\uc870\ud654\ub85c\uc6b4 \uc804\uc8fc\uace1",
+        "PT": "Prel\u00fadio da Sinfonia Harmoniosa",
+        "RU": "\u0423\u0432\u0435\u0440\u0442\u044e\u0440\u0430 \u0441\u0442\u0440\u043e\u0439\u043d\u043e\u0439 \u0441\u0438\u043c\u0444\u043e\u043d\u0438\u0438",
+        "TH": "Harmonious Symphony Prelude",
+        "TR": "Ahenkli Senfoninin Ba\u015flang\u0131c\u0131",
+        "VI": "D\u1ea1o \u0110\u1ea7u C\u1ee7a Giao H\u01b0\u1edfng"
+    },
     "2551406228": {
         "CHS": "\u5b66\u58eb\u7684\u4e66\u7b7e",
         "DE": "Gelehrtenlesezeichen",
         "EN": "Scholar's Bookmark",
         "ES": "Marcap\u00e1ginas de la Erudita",
         "FR": "Marque-page de l'\u00c9rudit",
         "ID": "Scholar's Bookmark",
@@ -25531,14 +25899,30 @@
         "KR": "\ubc14\ub78c \uad70\uc8fc\uc758 \uc794",
         "PT": "C\u00e1lice dos Ventos Celestiais",
         "RU": "\u0427\u0430\u0448\u0430 \u0445\u043e\u0437\u044f\u0438\u043d\u0430 \u0432\u0435\u0442\u0440\u043e\u0432",
         "TH": "Lord of Wind over Firmament's Cup",
         "TR": "G\u00f6kkubbe R\u00fczgar\u0131 Efendisinin Kadehi",
         "VI": "Ly Ng\u1ecdn Gi\u00f3 Tr\u1eddi Cao"
     },
+    "257567548": {
+        "CHS": "\u6697\u7ed3\u7684\u660e\u82b1",
+        "DE": "Helle Bl\u00fcte dunkler Fr\u00fcchte",
+        "EN": "Dark Fruit of Bright Flowers",
+        "ES": "Flor Secreta Rutilante",
+        "FR": "Fleur de n\u0153uds dissimul\u00e9s",
+        "ID": "Dark Fruit of Bright Flowers",
+        "IT": "Frutto fosco di fiori limpidi",
+        "JP": "\u9670\u306b\u54b2\u304f\u5149\u306e\u82b1",
+        "KR": "\uc5b4\ub460 \uc18d\uc758 \ubc1d\uc740 \uaf43",
+        "PT": "Fruto Sombrio de Flores Brilhantes",
+        "RU": "\u0422\u0451\u043c\u043d\u044b\u0439 \u043f\u043b\u043e\u0434 \u044f\u0440\u043a\u0438\u0445 \u0446\u0432\u0435\u0442\u043e\u0432",
+        "TH": "Dark Fruit of Bright Flowers",
+        "TR": "Parlak \u00c7i\u00e7eklerin Koyu Meyvesi",
+        "VI": "Hoa S\u00e1ng C\u1ee7a Qu\u1ea3 \u0110en"
+    },
     "2578477676": {
         "CHS": "\u5e78\u8fd0\u513f\u94f6\u51a0",
         "DE": "Silberner Gl\u00fcckshaarreif",
         "EN": "Lucky Dog's Silver Circlet",
         "ES": "Tiara de Plata del Afortunado",
         "FR": "Diad\u00e8me d'argent du Chanceux",
         "ID": "Lucky Dog's Silver Circlet",
@@ -26523,14 +26907,30 @@
         "KR": "\ubc88\uac1c\uc758 \uc790\ud0dc",
         "PT": "Postura Eletrizante",
         "RU": "\u0413\u0440\u043e\u043c\u043e\u0433\u043b\u0430\u0441\u043d\u044b\u0439 \u043e\u0431\u043b\u0438\u043a",
         "TH": "Thundering Poise",
         "TR": "Y\u0131ld\u0131r\u0131m Duru\u015fu",
         "VI": "Di\u1ec7n M\u1ea1o S\u1ea5m S\u00e9t"
     },
+    "2638728292": {
+        "CHS": "\u53e4\u6d77\u7384\u5e7d\u7684\u591c\u60f3",
+        "DE": "N\u00e4chtliches Gr\u00fcbeln der uralten See",
+        "EN": "Ancient Sea's Nocturnal Musing",
+        "ES": "Nocturno del Mar de Anta\u00f1o",
+        "FR": "R\u00eaverie des eaux antiques",
+        "ID": "Ancient Sea's Nocturnal Musing",
+        "IT": "Riflessione notturna del Mare Antico",
+        "JP": "\u53e4\u6d77\u306e\u5e7d\u6df1\u306a\u308b\u591c\u60f3",
+        "KR": "\uace0\ub300 \ubc14\ub2e4\uc758 \uc57c\uc0c1\uace1",
+        "PT": "Reflex\u00e3o Noturna do Mar Antigo",
+        "RU": "\u041d\u043e\u0447\u043d\u044b\u0435 \u0440\u0430\u0437\u0434\u0443\u043c\u044c\u044f \u0434\u0440\u0435\u0432\u043d\u0435\u0433\u043e \u043c\u043e\u0440\u044f",
+        "TH": "Ancient Sea's Nocturnal Musing",
+        "TR": "Kadim Deniz'in Gece D\u00fc\u015f\u00fcnceleri",
+        "VI": "D\u1ea1 T\u1ea5u C\u1ee7a Bi\u1ec3n X\u01b0a"
+    },
     "2639957116": {
         "CHS": "\u5317\u98ce\u4e4b\u76cf",
         "DE": "Kelch des Aquilo",
         "EN": "Goblet of Aquilo",
         "ES": "C\u00e1liz de Aquilo",
         "FR": "Coupe aquilon",
         "ID": "Goblet of Aquilo",
@@ -26667,14 +27067,30 @@
         "KR": "\ubc14\ub78c \uad70\uc8fc\uc758 \uaf43",
         "PT": "Flor dos Ventos Celestiais",
         "RU": "\u0426\u0432\u0435\u0442\u043e\u043a \u0445\u043e\u0437\u044f\u0438\u043d\u0430 \u0432\u0435\u0442\u0440\u043e\u0432",
         "TH": "Lord of Wind over Firmament's Flower",
         "TR": "G\u00f6kkubbe R\u00fczgar\u0131 Efendisinin \u00c7i\u00e7e\u011fi",
         "VI": "Hoa Ng\u1ecdn Gi\u00f3 Tr\u1eddi Cao"
     },
+    "2649107356": {
+        "CHS": "\u5f02\u60f3\u96f6\u843d\u7684\u5706\u821e",
+        "DE": "Reigen vereinzelter Launen",
+        "EN": "Whimsical Dance of the Withered",
+        "ES": "Vals Fantasioso de la Ruina",
+        "FR": "Ronde des pens\u00e9es fan\u00e9es",
+        "ID": "Whimsical Dance of the Withered",
+        "IT": "Danza estrosa dei caduti",
+        "JP": "\u7570\u60f3\u304c\u67af\u308c\u843d\u3061\u308b\u5186\u821e",
+        "KR": "\uc601\ub77d\ud55c \uacf5\uc0c1\uc758 \uc648\uce20",
+        "PT": "Valsa Divergente dos Ca\u00eddos",
+        "RU": "\u0412\u0430\u043b\u044c\u0441 \u0443\u0432\u044f\u0434\u0448\u0438\u0445 \u0444\u0430\u043d\u0442\u0430\u0437\u0438\u0439",
+        "TH": "Whimsical Dance of the Withered",
+        "TR": "Solup Gidenin Tuhaf Dans\u0131",
+        "VI": "V\u0169 \u0110i\u1ec7u C\u1ee7a T\u00e0n Phai"
+    },
     "2650209148": {
         "CHS": "\u65e0\u5e38\u4e4b\u9762",
         "DE": "Wechselhafte Maske",
         "EN": "Capricious Visage",
         "ES": "M\u00e1scara de la Mutabilidad",
         "FR": "Visage capricieux",
         "ID": "Capricious Visage",
@@ -27563,14 +27979,30 @@
         "KR": "\ube5b\uc744 \uc887\ub294 \ub3cc",
         "PT": "Pedra do Ca\u00e7ador da Luz",
         "RU": "\u0421\u043e\u043b\u043d\u0435\u0447\u043d\u044b\u0435 \u0447\u0430\u0441\u044b \u0432\u0440\u0435\u043c\u0435\u043d\u0449\u0438\u043a\u0430",
         "TH": "Sundial of the Sojourner",
         "TR": "Yolcunun Saati",
         "VI": "H\u00f2n \u0110\u00e1 Ph\u00e1t S\u00e1ng"
     },
+    "2712149308": {
+        "CHS": "\u892a\u5149\u7684\u7fe0\u5c3e",
+        "DE": "Verblasste Smaragdschwanzfeder",
+        "EN": "Faded Emerald Tail",
+        "ES": "Cola Esmeralda Descolorida",
+        "FR": "Queue \u00e9meraude de fanaison",
+        "ID": "Faded Emerald Tail",
+        "IT": "Coda smeraldina scolorita",
+        "JP": "\u5149\u892a\u305b\u305f\u7fe0\u5c3e",
+        "KR": "\ube5b\ubc14\ub79c \ud478\ub978 \uaf41\uc9c0",
+        "PT": "Cauda de Esmeralda Desbotada",
+        "RU": "\u0411\u043b\u0451\u043a\u043b\u044b\u0439 \u0438\u0437\u0443\u043c\u0440\u0443\u0434\u043d\u044b\u0439 \u0445\u0432\u043e\u0441\u0442",
+        "TH": "Faded Emerald Tail",
+        "TR": "Solmu\u015f Z\u00fcmr\u00fct Kuyruk",
+        "VI": "\u0110u\u00f4i Ph\u1ec9 Th\u00fay Phai M\u00e0u"
+    },
     "2713166956": {
         "CHS": "\u590f\u796d\u4e4b\u9762",
         "DE": "Sommerfestmaske",
         "EN": "Summer Night's Mask",
         "ES": "M\u00e1scara de la Noche de Verano",
         "FR": "Masque de la nuit d'\u00e9t\u00e9",
         "ID": "Summer Night's Mask",
@@ -31019,14 +31451,30 @@
         "KR": "",
         "PT": "",
         "RU": "",
         "TH": "",
         "TR": "",
         "VI": ""
     },
+    "2919065596": {
+        "CHS": "\u547d\u9014\u8f6e\u8f6c\u7684\u8c10\u8c11",
+        "DE": "R\u00e4tsel der Wendung des Schicksals",
+        "EN": "The Grand Jape of the Turning of Fate",
+        "ES": "Gran Burla del Giro del Destino",
+        "FR": "Farce des changements du destin",
+        "ID": "The Grand Jape of the Turning of Fate",
+        "IT": "Grande scherzo del destino",
+        "JP": "\u904b\u547d\u3068\u8f2a\u5efb\u306e\u8ae7\u8b14",
+        "KR": "\uad6c\ub974\ub294 \uc6b4\uba85\uc758 \ud574\ud559\uace1",
+        "PT": "A Grande Farsa da Volta do Destino",
+        "RU": "\u0421\u043a\u0435\u0440\u0446\u043e \u043f\u043e\u0432\u043e\u0440\u043e\u0442\u043e\u0432 \u0441\u0443\u0434\u044c\u0431\u044b",
+        "TH": "The Grand Jape of the Turning of Fate",
+        "TR": "Kader D\u00f6ng\u00fcs\u00fcn\u00fcn B\u00fcy\u00fck Oyunu",
+        "VI": "Tr\u00eau Ng\u01b0\u01a1i C\u1ee7a V\u1eadn M\u1ec7nh"
+    },
     "2919362316": {
         "CHS": "\u6559\u5b98\u7684\u80f8\u82b1",
         "DE": "Ausbilderbrosche",
         "EN": "Instructor's Brooch",
         "ES": "Broche del Instructor",
         "FR": "Broche de l'Instructeur",
         "ID": "Instructor's Brooch",
@@ -31339,14 +31787,30 @@
         "KR": "\uc804\ud22c\uad11\uc758 \uc7a5\ubbf8",
         "PT": "Rosa de Berserker",
         "RU": "\u0420\u043e\u0437\u0430 \u0431\u0435\u0440\u0441\u0435\u0440\u043a\u0430",
         "TH": "Berserker's Rose",
         "TR": "Vah\u015fi Sava\u015f\u00e7\u0131 G\u00fcl\u00fc",
         "VI": "T\u01b0\u1eddng Vi Cu\u1ed3ng Chi\u1ebfn"
     },
+    "2942495796": {
+        "CHS": "\u8c10\u5f8b\u4ea4\u54cd\u7684\u524d\u594f",
+        "DE": "Vorspiel der harmonischen Sinfonie",
+        "EN": "Harmonious Symphony Prelude",
+        "ES": "Preludio de la Sinfon\u00eda Arm\u00f3nica",
+        "FR": "Pr\u00e9lude des symphonies harmoniques",
+        "ID": "Harmonious Symphony Prelude",
+        "IT": "Preludio della Sinfonia armonica",
+        "JP": "\u97ff\u304d\u5408\u3046\u8ae7\u5f8b\u306e\u524d\u594f",
+        "KR": "\uc870\ud654\ub85c\uc6b4 \uc804\uc8fc\uace1",
+        "PT": "Prel\u00fadio da Sinfonia Harmoniosa",
+        "RU": "\u0423\u0432\u0435\u0440\u0442\u044e\u0440\u0430 \u0441\u0442\u0440\u043e\u0439\u043d\u043e\u0439 \u0441\u0438\u043c\u0444\u043e\u043d\u0438\u0438",
+        "TH": "Harmonious Symphony Prelude",
+        "TR": "Ahenkli Senfoninin Ba\u015flang\u0131c\u0131",
+        "VI": "D\u1ea1o \u0110\u1ea7u C\u1ee7a Giao H\u01b0\u1edfng"
+    },
     "2942754732": {
         "CHS": "\u5c11\u5973\u7247\u523b\u7684\u95f2\u6687",
         "DE": "Mu\u00dfe der Maid",
         "EN": "Maiden's Fleeting Leisure",
         "ES": "Pasatiempo de la Doncella",
         "FR": "Loisir de la Demoiselle",
         "ID": "Maiden's Fleeting Leisure",
@@ -31867,14 +32331,30 @@
         "KR": "\ud53c\uc5d0 \ubb3c\ub4e0 \uae30\uc0ac\uc758 \uc2dc\uacc4",
         "PT": "Rel\u00f3gio do Cavaleiro Sanguin\u00e1rio",
         "RU": "\u0427\u0430\u0441 \u0434\u043e\u043b\u0433\u0430 \u0440\u044b\u0446\u0430\u0440\u044f \u043a\u0440\u043e\u0432\u0438",
         "TH": "Bloodstained Final Hour",
         "TR": "Kanl\u0131 \u015e\u00f6valyenin Saati",
         "VI": "\u0110\u1ed3ng H\u1ed3 K\u1ef5 S\u0129 Nhu\u1ed1m M\u00e1u"
     },
+    "29786276": {
+        "CHS": "\u547d\u9014\u8f6e\u8f6c\u7684\u8c10\u8c11",
+        "DE": "R\u00e4tsel der Wendung des Schicksals",
+        "EN": "The Grand Jape of the Turning of Fate",
+        "ES": "Gran Burla del Giro del Destino",
+        "FR": "Farce des changements du destin",
+        "ID": "The Grand Jape of the Turning of Fate",
+        "IT": "Grande scherzo del destino",
+        "JP": "\u904b\u547d\u3068\u8f2a\u5efb\u306e\u8ae7\u8b14",
+        "KR": "\uad6c\ub974\ub294 \uc6b4\uba85\uc758 \ud574\ud559\uace1",
+        "PT": "A Grande Farsa da Volta do Destino",
+        "RU": "\u0421\u043a\u0435\u0440\u0446\u043e \u043f\u043e\u0432\u043e\u0440\u043e\u0442\u043e\u0432 \u0441\u0443\u0434\u044c\u0431\u044b",
+        "TH": "The Grand Jape of the Turning of Fate",
+        "TR": "Kader D\u00f6ng\u00fcs\u00fcn\u00fcn B\u00fcy\u00fck Oyunu",
+        "VI": "Tr\u00eau Ng\u01b0\u01a1i C\u1ee7a V\u1eadn M\u1ec7nh"
+    },
     "2979692732": {
         "CHS": "\u4f17\u751f\u4e4b\u8c23",
         "DE": "Lied der Verg\u00e4nglichkeit",
         "EN": "Song of Life",
         "ES": "Canto de la Vida",
         "FR": "Chant de vie",
         "ID": "Song of Life",
@@ -32171,14 +32651,30 @@
         "KR": "\ubc88\uac1c\ub97c \ubd80\ub974\ub294 \ubaa8\uc790",
         "PT": "Coroa do Invocador do Trov\u00e3o",
         "RU": "\u041a\u043e\u0440\u043e\u043d\u0430 \u043f\u0440\u0438\u0437\u044b\u0432\u0430\u0442\u0435\u043b\u044f \u0433\u0440\u043e\u043c\u0430",
         "TH": "Thunder Summoner's Crown",
         "TR": "Y\u0131ld\u0131r\u0131m Sihirdar\u0131 Tac\u0131",
         "VI": "V\u01b0\u01a1ng Mi\u1ec7n G\u1ecdi S\u00e9t"
     },
+    "2995813268": {
+        "CHS": "\u4e3e\u4e1a\u7684\u8bc6\u523b",
+        "DE": "Augenblick des Erfolgs",
+        "EN": "Moment of Attainment",
+        "ES": "Momento de Aprehensi\u00f3n",
+        "FR": "Instant de r\u00e9alisation",
+        "ID": "Moment of Attainment",
+        "IT": "Momento di conquista",
+        "JP": "\u5927\u696d\u3092\u6210\u3059\u523b",
+        "KR": "\ub300\uc5c5\uc758 \uc2dc\uac04",
+        "PT": "Momento de Conquista",
+        "RU": "\u041c\u043e\u043c\u0435\u043d\u0442 \u043e\u0431\u0440\u0435\u0442\u0435\u043d\u0438\u044f",
+        "TH": "Moment of Attainment",
+        "TR": "Zafer An\u0131",
+        "VI": "Th\u1eddi Kh\u1eafc C\u1ee7a \u0110\u1ea1t Th\u00e0nh"
+    },
     "2996035980": {
         "CHS": "\u5192\u9669\u5bb6\u5934\u5e26",
         "DE": "Kopftuch eines Abenteurers",
         "EN": "Adventurer's Bandana",
         "ES": "Bandana del Aventurero",
         "FR": "Bandeau de l'Aventurier",
         "ID": "Adventurer's Bandana",
@@ -33435,14 +33931,30 @@
         "KR": "\uc18c\ub140\uc758 \ud754\ub4e4\ub9ac\ub294 \uadf8\ub9ac\uc6c0",
         "PT": "Lembran\u00e7as da Donzela",
         "RU": "\u0422\u043e\u0441\u043a\u0430 \u044e\u043d\u043e\u0439 \u0434\u0435\u0432\u044b",
         "TH": "Maiden's Heart-stricken Infatuation",
         "TR": "Han\u0131m\u0131n Kara Sevdas\u0131",
         "VI": "\u00dd Ngh\u0129 C\u1ee7a Thi\u1ebfu N\u1eef"
     },
+    "3081478772": {
+        "CHS": "\u53e4\u6d77\u7384\u5e7d\u7684\u591c\u60f3",
+        "DE": "N\u00e4chtliches Gr\u00fcbeln der uralten See",
+        "EN": "Ancient Sea's Nocturnal Musing",
+        "ES": "Nocturno del Mar de Anta\u00f1o",
+        "FR": "R\u00eaverie des eaux antiques",
+        "ID": "Ancient Sea's Nocturnal Musing",
+        "IT": "Riflessione notturna del Mare Antico",
+        "JP": "\u53e4\u6d77\u306e\u5e7d\u6df1\u306a\u308b\u591c\u60f3",
+        "KR": "\uace0\ub300 \ubc14\ub2e4\uc758 \uc57c\uc0c1\uace1",
+        "PT": "Reflex\u00e3o Noturna do Mar Antigo",
+        "RU": "\u041d\u043e\u0447\u043d\u044b\u0435 \u0440\u0430\u0437\u0434\u0443\u043c\u044c\u044f \u0434\u0440\u0435\u0432\u043d\u0435\u0433\u043e \u043c\u043e\u0440\u044f",
+        "TH": "Ancient Sea's Nocturnal Musing",
+        "TR": "Kadim Deniz'in Gece D\u00fc\u015f\u00fcnceleri",
+        "VI": "D\u1ea1 T\u1ea5u C\u1ee7a Bi\u1ec3n X\u01b0a"
+    },
     "3081896228": {
         "CHS": "\u796d\u96f7\u793c\u51a0",
         "DE": "Blitzopferdiadem",
         "EN": "Tiara of Thunder",
         "ES": "Diadema del Trueno",
         "FR": "Couronne rituelle \u00c9lectro",
         "ID": "Tiara of Thunder",
@@ -34219,14 +34731,30 @@
         "KR": "\ubb34\uc778\uc758 \ubd89\uc740 \uaf43",
         "PT": "Flor Vermelha de Artista Marcial",
         "RU": "\u0410\u043b\u044b\u0439 \u0446\u0432\u0435\u0442\u043e\u043a \u0432\u043e\u0438\u043d\u0430",
         "TH": "Martial Artist's Red Flower",
         "TR": "D\u00f6v\u00fc\u015f Ustas\u0131n\u0131n K\u0131rm\u0131z\u0131 \u00c7i\u00e7e\u011fi",
         "VI": "Hoa V\u00f5 Nh\u00e2n"
     },
+    "3134129324": {
+        "CHS": "\u547d\u9014\u8f6e\u8f6c\u7684\u8c10\u8c11",
+        "DE": "R\u00e4tsel der Wendung des Schicksals",
+        "EN": "The Grand Jape of the Turning of Fate",
+        "ES": "Gran Burla del Giro del Destino",
+        "FR": "Farce des changements du destin",
+        "ID": "The Grand Jape of the Turning of Fate",
+        "IT": "Grande scherzo del destino",
+        "JP": "\u904b\u547d\u3068\u8f2a\u5efb\u306e\u8ae7\u8b14",
+        "KR": "\uad6c\ub974\ub294 \uc6b4\uba85\uc758 \ud574\ud559\uace1",
+        "PT": "A Grande Farsa da Volta do Destino",
+        "RU": "\u0421\u043a\u0435\u0440\u0446\u043e \u043f\u043e\u0432\u043e\u0440\u043e\u0442\u043e\u0432 \u0441\u0443\u0434\u044c\u0431\u044b",
+        "TH": "The Grand Jape of the Turning of Fate",
+        "TR": "Kader D\u00f6ng\u00fcs\u00fcn\u00fcn B\u00fcy\u00fck Oyunu",
+        "VI": "Tr\u00eau Ng\u01b0\u01a1i C\u1ee7a V\u1eadn M\u1ec7nh"
+    },
     "3134842684": {
         "CHS": "\u9057\u5fd8\u7684\u5bb9\u5668",
         "DE": "Vergessenes Gef\u00e4\u00df",
         "EN": "Forgotten Vessel",
         "ES": "Licorera del Olvido",
         "FR": "R\u00e9ceptacle oubli\u00e9",
         "ID": "Forgotten Vessel",
@@ -36059,14 +36587,30 @@
         "KR": "\uc11c\ub9ac\ub97c \uac10\uc2fc \uae30\uace8",
         "PT": "Orgulho da Geada",
         "RU": "\u041c\u043e\u0440\u043e\u0437\u043d\u0430\u044f \u0433\u043e\u0440\u0434\u043e\u0441\u0442\u044c",
         "TH": "Frost-Weaved Dignity",
         "TR": "Buzul Nak\u0131\u015fl\u0131 Asalet",
         "VI": "Ni\u1ec1m Ki\u00eau H\u00e3nh B\u0103ng Gi\u00e1"
     },
+    "3246653860": {
+        "CHS": "\u5f02\u60f3\u96f6\u843d\u7684\u5706\u821e",
+        "DE": "Reigen vereinzelter Launen",
+        "EN": "Whimsical Dance of the Withered",
+        "ES": "Vals Fantasioso de la Ruina",
+        "FR": "Ronde des pens\u00e9es fan\u00e9es",
+        "ID": "Whimsical Dance of the Withered",
+        "IT": "Danza estrosa dei caduti",
+        "JP": "\u7570\u60f3\u304c\u67af\u308c\u843d\u3061\u308b\u5186\u821e",
+        "KR": "\uc601\ub77d\ud55c \uacf5\uc0c1\uc758 \uc648\uce20",
+        "PT": "Valsa Divergente dos Ca\u00eddos",
+        "RU": "\u0412\u0430\u043b\u044c\u0441 \u0443\u0432\u044f\u0434\u0448\u0438\u0445 \u0444\u0430\u043d\u0442\u0430\u0437\u0438\u0439",
+        "TH": "Whimsical Dance of the Withered",
+        "TR": "Solup Gidenin Tuhaf Dans\u0131",
+        "VI": "V\u0169 \u0110i\u1ec7u C\u1ee7a T\u00e0n Phai"
+    },
     "3247223020": {
         "CHS": "\u5b88\u62a4\u5fbd\u5370",
         "DE": "W\u00e4chterabzeichen",
         "EN": "Guardian's Sigil",
         "ES": "Insignia del Guardi\u00e1n",
         "FR": "Plume du Gardien",
         "ID": "Guardian's Sigil",
@@ -36683,14 +37227,30 @@
         "KR": "\uc218\ud638\uc758 \ub760",
         "PT": "Cinto do Guarda",
         "RU": "\u041f\u043e\u0432\u044f\u0437\u043a\u0430 \u0437\u0430\u0449\u0438\u0442\u043d\u0438\u043a\u0430",
         "TH": "Guardian's Band",
         "TR": "Muhaf\u0131z Band\u0131",
         "VI": "N\u00f3n Th\u1ee7 H\u1ed9"
     },
+    "329286804": {
+        "CHS": "\u4e3e\u4e1a\u7684\u8bc6\u523b",
+        "DE": "Augenblick des Erfolgs",
+        "EN": "Moment of Attainment",
+        "ES": "Momento de Aprehensi\u00f3n",
+        "FR": "Instant de r\u00e9alisation",
+        "ID": "Moment of Attainment",
+        "IT": "Momento di conquista",
+        "JP": "\u5927\u696d\u3092\u6210\u3059\u523b",
+        "KR": "\ub300\uc5c5\uc758 \uc2dc\uac04",
+        "PT": "Momento de Conquista",
+        "RU": "\u041c\u043e\u043c\u0435\u043d\u0442 \u043e\u0431\u0440\u0435\u0442\u0435\u043d\u0438\u044f",
+        "TH": "Moment of Attainment",
+        "TR": "Zafer An\u0131",
+        "VI": "Th\u1eddi Kh\u1eafc C\u1ee7a \u0110\u1ea1t Th\u00e0nh"
+    },
     "3293065964": {
         "CHS": "\u9010\u5149\u4e4b\u77f3",
         "DE": "Stein der Lichtjagd",
         "EN": "Sundial of the Sojourner",
         "ES": "Piedra Atrapaluz",
         "FR": "Montre du Voyageur",
         "ID": "Sundial of the Sojourner",
@@ -38443,14 +39003,30 @@
         "KR": "\uc720\ubc30\uc790\uc758 \uba38\ub9ac\uc7a5\uc2dd",
         "PT": "Grinalda do Exilado",
         "RU": "\u041a\u043e\u0440\u043e\u043d\u0430 \u0438\u0437\u0433\u043d\u0430\u043d\u043d\u0438\u043a\u0430",
         "TH": "Exile's Circlet",
         "TR": "S\u00fcrg\u00fcn\u00fcn Tac\u0131",
         "VI": "V\u01b0\u01a1ng Mi\u1ec7n K\u1ebb L\u01b0u \u0110\u00e0y"
     },
+    "3407812284": {
+        "CHS": "\u4e3e\u4e1a\u7684\u8bc6\u523b",
+        "DE": "Augenblick des Erfolgs",
+        "EN": "Moment of Attainment",
+        "ES": "Momento de Aprehensi\u00f3n",
+        "FR": "Instant de r\u00e9alisation",
+        "ID": "Moment of Attainment",
+        "IT": "Momento di conquista",
+        "JP": "\u5927\u696d\u3092\u6210\u3059\u523b",
+        "KR": "\ub300\uc5c5\uc758 \uc2dc\uac04",
+        "PT": "Momento de Conquista",
+        "RU": "\u041c\u043e\u043c\u0435\u043d\u0442 \u043e\u0431\u0440\u0435\u0442\u0435\u043d\u0438\u044f",
+        "TH": "Moment of Attainment",
+        "TR": "Zafer An\u0131",
+        "VI": "Th\u1eddi Kh\u1eafc C\u1ee7a \u0110\u1ea1t Th\u00e0nh"
+    },
     "3407812548": {
         "CHS": "\u6d41\u653e\u8005\u4e4b\u7fbd",
         "DE": "Feder des Verbannten",
         "EN": "Exile's Feather",
         "ES": "Pluma del Exiliado",
         "FR": "Plume de l'Exil\u00e9",
         "ID": "Exile's Feather",
@@ -39787,14 +40363,30 @@
         "KR": "\uc81c\ud48d\uc758 \uad00",
         "PT": "Coroa do Ritual Anemo",
         "RU": "\u0422\u0438\u0430\u0440\u0430 \u0432\u0435\u0442\u0440\u0430",
         "TH": "Tiara of Gales",
         "TR": "Bora Tac\u0131",
         "VI": "N\u00f3n T\u1ebf Phong"
     },
+    "3480233164": {
+        "CHS": "\u5931\u5195\u7684\u5b9d\u51a0",
+        "DE": "Kronenlose Krone",
+        "EN": "Crownless Crown",
+        "ES": "Corona Descoronada",
+        "FR": "Couronne sans couronne",
+        "ID": "Crownless Crown",
+        "IT": "Corona senza corona",
+        "JP": "\u4e3b\u306a\u304d\u51a0",
+        "KR": "\uc8fc\uc778 \uc783\uc740 \uc655\uad00",
+        "PT": "Coroa Descoroada",
+        "RU": "\u041d\u0435\u0432\u0435\u043d\u0447\u0430\u043d\u043d\u0430\u044f \u043a\u043e\u0440\u043e\u043d\u0430",
+        "TH": "Crownless Crown",
+        "TR": "Sahipsiz Ta\u00e7",
+        "VI": "V\u01b0\u01a1ng Mi\u1ec7n Qu\u00fd Kh\u00f4ng Ngai"
+    },
     "3480828772": {
         "CHS": "\u6559\u5b98\u7684\u7fbd\u9970",
         "DE": "Ausbilderfederschmuck",
         "EN": "Instructor's Feather Accessory",
         "ES": "Pluma del Instructor",
         "FR": "Plume de l'Instructeur",
         "ID": "Instructor's Feathered Accessory",
@@ -41483,14 +42075,30 @@
         "KR": "\uc218\ud638\uc758 \uaf43",
         "PT": "Flor do Guarda",
         "RU": "\u0426\u0432\u0435\u0442\u043e\u043a \u0437\u0430\u0449\u0438\u0442\u043d\u0438\u043a\u0430",
         "TH": "Guardian's Flower",
         "TR": "Muhaf\u0131z \u00c7i\u00e7e\u011fi",
         "VI": "Hoa Th\u1ee7 H\u1ed9"
     },
+    "3572708764": {
+        "CHS": "\u892a\u5149\u7684\u7fe0\u5c3e",
+        "DE": "Verblasste Smaragdschwanzfeder",
+        "EN": "Faded Emerald Tail",
+        "ES": "Cola Esmeralda Descolorida",
+        "FR": "Queue \u00e9meraude de fanaison",
+        "ID": "Faded Emerald Tail",
+        "IT": "Coda smeraldina scolorita",
+        "JP": "\u5149\u892a\u305b\u305f\u7fe0\u5c3e",
+        "KR": "\ube5b\ubc14\ub79c \ud478\ub978 \uaf41\uc9c0",
+        "PT": "Cauda de Esmeralda Desbotada",
+        "RU": "\u0411\u043b\u0451\u043a\u043b\u044b\u0439 \u0438\u0437\u0443\u043c\u0440\u0443\u0434\u043d\u044b\u0439 \u0445\u0432\u043e\u0441\u0442",
+        "TH": "Faded Emerald Tail",
+        "TR": "Solmu\u015f Z\u00fcmr\u00fct Kuyruk",
+        "VI": "\u0110u\u00f4i Ph\u1ec9 Th\u00fay Phai M\u00e0u"
+    },
     "3573789380": {
         "CHS": "\u51b7\u5374\u7f29\u51cf",
         "DE": "",
         "EN": "",
         "ES": "",
         "FR": "",
         "ID": "",
@@ -42075,14 +42683,30 @@
         "KR": "\ubb34\uc778\uc758 \uae43\ud138\uc7a5\uc2dd",
         "PT": "Acess\u00f3rio de Penas de Artista Marcial",
         "RU": "\u041f\u0435\u0440\u043e \u0432\u043e\u0438\u043d\u0430",
         "TH": "Martial Artist's Feathered Accessory",
         "TR": "D\u00f6v\u00fc\u015f Ustas\u0131n\u0131n T\u00fcyl\u00fc Aksesuar\u0131",
         "VI": "L\u00f4ng V\u0169 V\u00f5 Nh\u00e2n"
     },
+    "3617555484": {
+        "CHS": "\u7b79\u8c0b\u7684\u5171\u6a3d",
+        "DE": "Weinflasche der Planung",
+        "EN": "The Wine-Flask Over Which the Plan Was Hatched",
+        "ES": "Jarra del Gran Plan",
+        "FR": "Coupe commune de strat\u00e9gie",
+        "ID": "The Wine-Flask Over Which the Plan Was Hatched",
+        "IT": "Calice dell'escogitativa",
+        "JP": "\u8a08\u7565\u306e\u76c3",
+        "KR": "\uacf5\ubaa8\uc758 \uc220\uc794",
+        "PT": "A Garrafa de Vinho Sobre a Qual o Plano Foi Concebido",
+        "RU": "\u0427\u0430\u0448\u0430 \u0437\u0430\u043c\u044b\u0441\u043b\u0430",
+        "TH": "The Wine-Flask Over Which the Plan Was Hatched",
+        "TR": "Plan\u0131n Haz\u0131rland\u0131\u011f\u0131 \u015earap Kadehi",
+        "VI": "Ly R\u01b0\u1ee3u C\u00f9ng B\u00e0y M\u01b0u"
+    },
     "3619882004": {
         "CHS": "\u6d41\u653e\u8005\u4e4b\u676f",
         "DE": "Kelch des Verbannten",
         "EN": "Exile's Goblet",
         "ES": "C\u00e1liz del Exiliado",
         "FR": "Coupe de l'Exil\u00e9",
         "ID": "Exile's Goblet",
@@ -42827,14 +43451,30 @@
         "KR": "\uc6a9\uc0ac\uc758 \ud658\uc1a1",
         "PT": "Despedida do Valente",
         "RU": "\u041f\u0440\u043e\u0432\u043e\u0434\u044b \u0445\u0440\u0430\u0431\u0440\u0435\u0446\u0430",
         "TH": "Outset of the Brave",
         "TR": "Cesurlar\u0131n Yolculu\u011fu",
         "VI": "H\u00e0nh Tr\u00ecnh C\u1ee7a D\u0169ng S\u0129"
     },
+    "3666732564": {
+        "CHS": "\u8c10\u5f8b\u4ea4\u54cd\u7684\u524d\u594f",
+        "DE": "Vorspiel der harmonischen Sinfonie",
+        "EN": "Harmonious Symphony Prelude",
+        "ES": "Preludio de la Sinfon\u00eda Arm\u00f3nica",
+        "FR": "Pr\u00e9lude des symphonies harmoniques",
+        "ID": "Harmonious Symphony Prelude",
+        "IT": "Preludio della Sinfonia armonica",
+        "JP": "\u97ff\u304d\u5408\u3046\u8ae7\u5f8b\u306e\u524d\u594f",
+        "KR": "\uc870\ud654\ub85c\uc6b4 \uc804\uc8fc\uace1",
+        "PT": "Prel\u00fadio da Sinfonia Harmoniosa",
+        "RU": "\u0423\u0432\u0435\u0440\u0442\u044e\u0440\u0430 \u0441\u0442\u0440\u043e\u0439\u043d\u043e\u0439 \u0441\u0438\u043c\u0444\u043e\u043d\u0438\u0438",
+        "TH": "Harmonious Symphony Prelude",
+        "TR": "Ahenkli Senfoninin Ba\u015flang\u0131c\u0131",
+        "VI": "D\u1ea1o \u0110\u1ea7u C\u1ee7a Giao H\u01b0\u1edfng"
+    },
     "3670729252": {
         "CHS": "\u4f24\u5bb3\u589e\u52a0",
         "DE": "",
         "EN": "",
         "ES": "",
         "FR": "",
         "ID": "",
@@ -42923,14 +43563,30 @@
         "KR": "\uc804\ud22c\uad11\uc758 \uadc0\uba74",
         "PT": "M\u00e1scara de Batalha de Berserker",
         "RU": "\u0411\u043e\u0435\u0432\u0430\u044f \u043c\u0430\u0441\u043a\u0430 \u0431\u0435\u0440\u0441\u0435\u0440\u043a\u0430",
         "TH": "Berserker's Battle Mask",
         "TR": "Vah\u015fi Sava\u015f\u00e7\u0131 Sava\u015f Maskesi",
         "VI": "M\u1eb7t Qu\u1ef7 Cu\u1ed3ng Chi\u1ebfn"
     },
+    "3675718628": {
+        "CHS": "\u892a\u5149\u7684\u7fe0\u5c3e",
+        "DE": "Verblasste Smaragdschwanzfeder",
+        "EN": "Faded Emerald Tail",
+        "ES": "Cola Esmeralda Descolorida",
+        "FR": "Queue \u00e9meraude de fanaison",
+        "ID": "Faded Emerald Tail",
+        "IT": "Coda smeraldina scolorita",
+        "JP": "\u5149\u892a\u305b\u305f\u7fe0\u5c3e",
+        "KR": "\ube5b\ubc14\ub79c \ud478\ub978 \uaf41\uc9c0",
+        "PT": "Cauda de Esmeralda Desbotada",
+        "RU": "\u0411\u043b\u0451\u043a\u043b\u044b\u0439 \u0438\u0437\u0443\u043c\u0440\u0443\u0434\u043d\u044b\u0439 \u0445\u0432\u043e\u0441\u0442",
+        "TH": "Faded Emerald Tail",
+        "TR": "Solmu\u015f Z\u00fcmr\u00fct Kuyruk",
+        "VI": "\u0110u\u00f4i Ph\u1ec9 Th\u00fay Phai M\u00e0u"
+    },
     "3677436260": {
         "CHS": "\u7834\u51b0\u8e0f\u96ea\u7684\u56de\u97f3",
         "DE": "Echo des Eisbrechers",
         "EN": "Broken Rime's Echo",
         "ES": "Eco de la Escarcha",
         "FR": "\u00c9cho de l'hiver",
         "ID": "Broken Rime's Echo",
@@ -43387,14 +44043,30 @@
         "KR": "\uc228\uaca8\uc9c4 \ube5b\uc758 \uae43\ud138",
         "PT": "Pena do Esplendor",
         "RU": "\u041f\u0435\u0440\u043e \u0441\u043a\u0440\u044b\u0442\u043e\u0433\u043e \u0441\u0438\u044f\u043d\u0438\u044f",
         "TH": "Feather of Nascent Light",
         "TR": "Sakl\u0131 I\u015f\u0131\u011f\u0131n T\u00fcy\u00fc",
         "VI": "L\u00f4ng V\u0169 L\u1ea5p L\u00e1nh"
     },
+    "3704215748": {
+        "CHS": "\u6697\u7ed3\u7684\u660e\u82b1",
+        "DE": "Helle Bl\u00fcte dunkler Fr\u00fcchte",
+        "EN": "Dark Fruit of Bright Flowers",
+        "ES": "Flor Secreta Rutilante",
+        "FR": "Fleur de n\u0153uds dissimul\u00e9s",
+        "ID": "Dark Fruit of Bright Flowers",
+        "IT": "Frutto fosco di fiori limpidi",
+        "JP": "\u9670\u306b\u54b2\u304f\u5149\u306e\u82b1",
+        "KR": "\uc5b4\ub460 \uc18d\uc758 \ubc1d\uc740 \uaf43",
+        "PT": "Fruto Sombrio de Flores Brilhantes",
+        "RU": "\u0422\u0451\u043c\u043d\u044b\u0439 \u043f\u043b\u043e\u0434 \u044f\u0440\u043a\u0438\u0445 \u0446\u0432\u0435\u0442\u043e\u0432",
+        "TH": "Dark Fruit of Bright Flowers",
+        "TR": "Parlak \u00c7i\u00e7eklerin Koyu Meyvesi",
+        "VI": "Hoa S\u00e1ng C\u1ee7a Qu\u1ea3 \u0110en"
+    },
     "3705988300": {
         "CHS": "\u5dc9\u5ca9\u7422\u5851\u4e4b\u6a3d",
         "DE": "Krug aus Felsgestein",
         "EN": "Goblet of Chiseled Crag",
         "ES": "C\u00e1liz del Escultor de Monta\u00f1as",
         "FR": "Coupe en roche escarp\u00e9e",
         "ID": "Goblet of Chiseled Crag",
@@ -43963,14 +44635,30 @@
         "KR": "\uc720\ubc30\uc790\uc758 \uaf43",
         "PT": "Flor do Exilado",
         "RU": "\u0426\u0432\u0435\u0442\u043e\u043a \u0438\u0437\u0433\u043d\u0430\u043d\u043d\u0438\u043a\u0430",
         "TH": "Exile's Flower",
         "TR": "S\u00fcrg\u00fcn\u00fcn \u00c7i\u00e7e\u011fi",
         "VI": "Hoa K\u1ebb L\u01b0u \u0110\u00e0y"
     },
+    "3749124492": {
+        "CHS": "\u7b79\u8c0b\u7684\u5171\u6a3d",
+        "DE": "Weinflasche der Planung",
+        "EN": "The Wine-Flask Over Which the Plan Was Hatched",
+        "ES": "Jarra del Gran Plan",
+        "FR": "Coupe commune de strat\u00e9gie",
+        "ID": "The Wine-Flask Over Which the Plan Was Hatched",
+        "IT": "Calice dell'escogitativa",
+        "JP": "\u8a08\u7565\u306e\u76c3",
+        "KR": "\uacf5\ubaa8\uc758 \uc220\uc794",
+        "PT": "A Garrafa de Vinho Sobre a Qual o Plano Foi Concebido",
+        "RU": "\u0427\u0430\u0448\u0430 \u0437\u0430\u043c\u044b\u0441\u043b\u0430",
+        "TH": "The Wine-Flask Over Which the Plan Was Hatched",
+        "TR": "Plan\u0131n Haz\u0131rland\u0131\u011f\u0131 \u015earap Kadehi",
+        "VI": "Ly R\u01b0\u1ee3u C\u00f9ng B\u00e0y M\u01b0u"
+    },
     "3749570204": {
         "CHS": "\u9ec4\u91d1\u98de\u9e1f\u7684\u843d\u7fbd",
         "DE": "Des Goldvogels fallende Feder",
         "EN": "Golden Bird's Shedding",
         "ES": "Pluma del Ave Dorada",
         "FR": "Mue de l'oiseau d'or",
         "ID": "Golden Bird's Shedding",
@@ -44427,14 +45115,30 @@
         "KR": "\uac80\ud22c\uc0ac\uc758 \uadc0\uacb0",
         "PT": "Destino do Gladiador",
         "RU": "\u0421\u0443\u0434\u044c\u0431\u0430 \u0433\u043b\u0430\u0434\u0438\u0430\u0442\u043e\u0440\u0430",
         "TH": "Gladiator's Destiny",
         "TR": "Gladyat\u00f6r\u00fcn Kaderi",
         "VI": "Gi\u00e1c \u0110\u1ea5u S\u0129 Tr\u1edf V\u1ec1"
     },
+    "3777616700": {
+        "CHS": "\u892a\u5149\u7684\u7fe0\u5c3e",
+        "DE": "Verblasste Smaragdschwanzfeder",
+        "EN": "Faded Emerald Tail",
+        "ES": "Cola Esmeralda Descolorida",
+        "FR": "Queue \u00e9meraude de fanaison",
+        "ID": "Faded Emerald Tail",
+        "IT": "Coda smeraldina scolorita",
+        "JP": "\u5149\u892a\u305b\u305f\u7fe0\u5c3e",
+        "KR": "\ube5b\ubc14\ub79c \ud478\ub978 \uaf41\uc9c0",
+        "PT": "Cauda de Esmeralda Desbotada",
+        "RU": "\u0411\u043b\u0451\u043a\u043b\u044b\u0439 \u0438\u0437\u0443\u043c\u0440\u0443\u0434\u043d\u044b\u0439 \u0445\u0432\u043e\u0441\u0442",
+        "TH": "Faded Emerald Tail",
+        "TR": "Solmu\u015f Z\u00fcmr\u00fct Kuyruk",
+        "VI": "\u0110u\u00f4i Ph\u1ec9 Th\u00fay Phai M\u00e0u"
+    },
     "3777926628": {
         "CHS": "\u52c7\u58eb\u7684\u52cb\u7ae0",
         "DE": "Reckenmedaille",
         "EN": "Medal of the Brave",
         "ES": "Medalla del Guerrero",
         "FR": "Embl\u00e8me du Brave",
         "ID": "Medal of the Brave",
@@ -45227,14 +45931,30 @@
         "KR": "\uad50\uad00\uc758 \uae43\ud138\uc7a5\uc2dd",
         "PT": "Acess\u00f3rio de Penas de Instrutor",
         "RU": "\u041f\u0435\u0440\u043e \u0438\u043d\u0441\u0442\u0440\u0443\u043a\u0442\u043e\u0440\u0430",
         "TH": "Instructor's Feather Accessory",
         "TR": "E\u011fitmenin T\u00fcyl\u00fc Aksesuar\u0131",
         "VI": "L\u00f4ng V\u0169 Gi\u00e1o Quan"
     },
+    "3824907452": {
+        "CHS": "\u5f02\u60f3\u96f6\u843d\u7684\u5706\u821e",
+        "DE": "Reigen vereinzelter Launen",
+        "EN": "Whimsical Dance of the Withered",
+        "ES": "Vals Fantasioso de la Ruina",
+        "FR": "Ronde des pens\u00e9es fan\u00e9es",
+        "ID": "Whimsical Dance of the Withered",
+        "IT": "Danza estrosa dei caduti",
+        "JP": "\u7570\u60f3\u304c\u67af\u308c\u843d\u3061\u308b\u5186\u821e",
+        "KR": "\uc601\ub77d\ud55c \uacf5\uc0c1\uc758 \uc648\uce20",
+        "PT": "Valsa Divergente dos Ca\u00eddos",
+        "RU": "\u0412\u0430\u043b\u044c\u0441 \u0443\u0432\u044f\u0434\u0448\u0438\u0445 \u0444\u0430\u043d\u0442\u0430\u0437\u0438\u0439",
+        "TH": "Whimsical Dance of the Withered",
+        "TR": "Solup Gidenin Tuhaf Dans\u0131",
+        "VI": "V\u0169 \u0110i\u1ec7u C\u1ee7a T\u00e0n Phai"
+    },
     "3826661628": {
         "CHS": "\u52c7\u58eb\u7684\u51a0\u5195",
         "DE": "Reckenhaarreif",
         "EN": "Crown of the Brave",
         "ES": "Corona del Guerrero",
         "FR": "Couronne du Brave",
         "ID": "Crown of the Brave",
@@ -46587,14 +47307,30 @@
         "KR": "\uc6d4\uacc4\uc218 \uc655\uad00",
         "PT": "Diadema L\u00e1urea",
         "RU": "\u041b\u0430\u0432\u0440\u043e\u0432\u044b\u0439 \u0432\u0435\u043d\u0435\u0446",
         "TH": "Laurel Coronet",
         "TR": "Defne Tac\u0131",
         "VI": "V\u01b0\u01a1ng Mi\u1ec7n C\u1ee7a Nguy\u1ec7t Qu\u1ebf"
     },
+    "3902182396": {
+        "CHS": "\u5f02\u60f3\u96f6\u843d\u7684\u5706\u821e",
+        "DE": "Reigen vereinzelter Launen",
+        "EN": "Whimsical Dance of the Withered",
+        "ES": "Vals Fantasioso de la Ruina",
+        "FR": "Ronde des pens\u00e9es fan\u00e9es",
+        "ID": "Whimsical Dance of the Withered",
+        "IT": "Danza estrosa dei caduti",
+        "JP": "\u7570\u60f3\u304c\u67af\u308c\u843d\u3061\u308b\u5186\u821e",
+        "KR": "\uc601\ub77d\ud55c \uacf5\uc0c1\uc758 \uc648\uce20",
+        "PT": "Valsa Divergente dos Ca\u00eddos",
+        "RU": "\u0412\u0430\u043b\u044c\u0441 \u0443\u0432\u044f\u0434\u0448\u0438\u0445 \u0444\u0430\u043d\u0442\u0430\u0437\u0438\u0439",
+        "TH": "Whimsical Dance of the Withered",
+        "TR": "Solup Gidenin Tuhaf Dans\u0131",
+        "VI": "V\u0169 \u0110i\u1ec7u C\u1ee7a T\u00e0n Phai"
+    },
     "3903117612": {
         "CHS": "\u6218\u72c2\u7684\u8537\u8587",
         "DE": "Berserkerrose",
         "EN": "Berserker's Rose",
         "ES": "Rosa del Berserker",
         "FR": "Rose du Berserker",
         "ID": "Berserker's Rose",
@@ -47131,14 +47867,30 @@
         "KR": "\ubaa8\ud5d8\uac00\uc758 \uaf41\uc9c0 \uae43\ud138",
         "PT": "Pena de Cauda de Aventureiro",
         "RU": "\u041f\u0435\u0440\u043e \u0438\u0441\u043a\u0430\u0442\u0435\u043b\u044f \u043f\u0440\u0438\u043a\u043b\u044e\u0447\u0435\u043d\u0438\u0439",
         "TH": "Adventurer's Tail Feather",
         "TR": "Macerac\u0131n\u0131n Kuyruk T\u00fcy\u00fc",
         "VI": "L\u00f4ng V\u0169 Nh\u00e0 M\u1ea1o Hi\u1ec3m"
     },
+    "3941298052": {
+        "CHS": "\u5931\u5195\u7684\u5b9d\u51a0",
+        "DE": "Kronenlose Krone",
+        "EN": "Crownless Crown",
+        "ES": "Corona Descoronada",
+        "FR": "Couronne sans couronne",
+        "ID": "Crownless Crown",
+        "IT": "Corona senza corona",
+        "JP": "\u4e3b\u306a\u304d\u51a0",
+        "KR": "\uc8fc\uc778 \uc783\uc740 \uc655\uad00",
+        "PT": "Coroa Descoroada",
+        "RU": "\u041d\u0435\u0432\u0435\u043d\u0447\u0430\u043d\u043d\u0430\u044f \u043a\u043e\u0440\u043e\u043d\u0430",
+        "TH": "Crownless Crown",
+        "TR": "Sahipsiz Ta\u00e7",
+        "VI": "V\u01b0\u01a1ng Mi\u1ec7n Qu\u00fd Kh\u00f4ng Ngai"
+    },
     "3941697284": {
         "CHS": "\u4e45\u8fdc\u82b1\u843d\u4e4b\u65f6",
         "DE": "Uralter Abschied",
         "EN": "Ancient Abscission",
         "ES": "Marchitamiento de Anta\u00f1o",
         "FR": "Abscission ancienne",
         "ID": "Ancient Abscission",
@@ -47627,14 +48379,30 @@
         "KR": "\ubc88\uac1c\ub97c \ubd80\ub974\ub294 \ubaa8\uc790",
         "PT": "Coroa do Invocador do Trov\u00e3o",
         "RU": "\u041a\u043e\u0440\u043e\u043d\u0430 \u043f\u0440\u0438\u0437\u044b\u0432\u0430\u0442\u0435\u043b\u044f \u0433\u0440\u043e\u043c\u0430",
         "TH": "Thunder Summoner's Crown",
         "TR": "Y\u0131ld\u0131r\u0131m Sihirdar\u0131 Tac\u0131",
         "VI": "V\u01b0\u01a1ng Mi\u1ec7n G\u1ecdi S\u00e9t"
     },
+    "3969402636": {
+        "CHS": "\u7b79\u8c0b\u7684\u5171\u6a3d",
+        "DE": "Weinflasche der Planung",
+        "EN": "The Wine-Flask Over Which the Plan Was Hatched",
+        "ES": "Jarra del Gran Plan",
+        "FR": "Coupe commune de strat\u00e9gie",
+        "ID": "The Wine-Flask Over Which the Plan Was Hatched",
+        "IT": "Calice dell'escogitativa",
+        "JP": "\u8a08\u7565\u306e\u76c3",
+        "KR": "\uacf5\ubaa8\uc758 \uc220\uc794",
+        "PT": "A Garrafa de Vinho Sobre a Qual o Plano Foi Concebido",
+        "RU": "\u0427\u0430\u0448\u0430 \u0437\u0430\u043c\u044b\u0441\u043b\u0430",
+        "TH": "The Wine-Flask Over Which the Plan Was Hatched",
+        "TR": "Plan\u0131n Haz\u0131rland\u0131\u011f\u0131 \u015earap Kadehi",
+        "VI": "Ly R\u01b0\u1ee3u C\u00f9ng B\u00e0y M\u01b0u"
+    },
     "3970228692": {
         "CHS": "\u6545\u4eba\u4e4b\u5fc3",
         "DE": "Sinn der Kameradschaft",
         "EN": "Heart of Comradeship",
         "ES": "Coraz\u00f3n de la Amistad",
         "FR": "Fleur du Voyageur",
         "ID": "Heart of Comradeship",
@@ -48523,14 +49291,30 @@
         "KR": "\uc81c\uc218\uc758 \uad00",
         "PT": "Coroa do Ritual Hydro",
         "RU": "\u0422\u0438\u0430\u0440\u0430 \u0432\u043e\u0434\u044b",
         "TH": "Tiara of Torrents",
         "TR": "Sa\u011fanak Tac\u0131",
         "VI": "N\u00f3n T\u1ebf Th\u1ee7y"
     },
+    "4023011412": {
+        "CHS": "\u5931\u5195\u7684\u5b9d\u51a0",
+        "DE": "Kronenlose Krone",
+        "EN": "Crownless Crown",
+        "ES": "Corona Descoronada",
+        "FR": "Couronne sans couronne",
+        "ID": "Crownless Crown",
+        "IT": "Corona senza corona",
+        "JP": "\u4e3b\u306a\u304d\u51a0",
+        "KR": "\uc8fc\uc778 \uc783\uc740 \uc655\uad00",
+        "PT": "Coroa Descoroada",
+        "RU": "\u041d\u0435\u0432\u0435\u043d\u0447\u0430\u043d\u043d\u0430\u044f \u043a\u043e\u0440\u043e\u043d\u0430",
+        "TH": "Crownless Crown",
+        "TR": "Sahipsiz Ta\u00e7",
+        "VI": "V\u01b0\u01a1ng Mi\u1ec7n Qu\u00fd Kh\u00f4ng Ngai"
+    },
     "4023236604": {
         "CHS": "\u964d\u96f7\u7684\u51f6\u5146",
         "DE": "Omen des Blitzes",
         "EN": "Omen of Thunderstorm",
         "ES": "Presagio de la Tormenta",
         "FR": "Pr\u00e9sage de tomb\u00e9e du tonnerre",
         "ID": "Omen of Thunderstorm",
@@ -49275,14 +50059,30 @@
         "KR": "\uba85\uc758\uc758 \uae43\ud138",
         "PT": "Pena do M\u00e9dico Virtuoso",
         "RU": "\u041f\u0435\u0440\u043e \u043c\u0443\u0434\u0440\u043e\u0433\u043e \u043b\u0435\u043a\u0430\u0440\u044f",
         "TH": "Wise Doctor's Pinion",
         "TR": "Bilge Doktorun T\u00fcy\u00fc",
         "VI": "L\u00f4ng V\u0169 Hi\u1ec1n Y"
     },
+    "4071524972": {
+        "CHS": "\u5f02\u60f3\u96f6\u843d\u7684\u5706\u821e",
+        "DE": "Reigen vereinzelter Launen",
+        "EN": "Whimsical Dance of the Withered",
+        "ES": "Vals Fantasioso de la Ruina",
+        "FR": "Ronde des pens\u00e9es fan\u00e9es",
+        "ID": "Whimsical Dance of the Withered",
+        "IT": "Danza estrosa dei caduti",
+        "JP": "\u7570\u60f3\u304c\u67af\u308c\u843d\u3061\u308b\u5186\u821e",
+        "KR": "\uc601\ub77d\ud55c \uacf5\uc0c1\uc758 \uc648\uce20",
+        "PT": "Valsa Divergente dos Ca\u00eddos",
+        "RU": "\u0412\u0430\u043b\u044c\u0441 \u0443\u0432\u044f\u0434\u0448\u0438\u0445 \u0444\u0430\u043d\u0442\u0430\u0437\u0438\u0439",
+        "TH": "Whimsical Dance of the Withered",
+        "TR": "Solup Gidenin Tuhaf Dans\u0131",
+        "VI": "V\u0169 \u0110i\u1ec7u C\u1ee7a T\u00e0n Phai"
+    },
     "4072756124": {
         "CHS": "\u6b66\u4eba\u7684\u5934\u5dfe",
         "DE": "Kampfk\u00fcnstler-Kopftuch",
         "EN": "Martial Artist's Bandana",
         "ES": "Bandana del Artista Marcial",
         "FR": "Bandeau de l'Artiste martial",
         "ID": "Martial Artist's Bandana",
@@ -49931,14 +50731,30 @@
         "KR": "\ud06c\ubc14\ub808\ub098\uc758 \ub208\ubd80\uc2e0 \uc2ec\uc7a5",
         "PT": "Cora\u00e7\u00e3o do Brilho de Khvarena",
         "RU": "\u0421\u0435\u0440\u0434\u0446\u0435 \u0441\u0432\u0435\u0442\u043e\u0437\u0430\u0440\u043d\u043e\u0441\u0442\u0438 \u0425\u0432\u0430\u0440\u043d\u044b",
         "TH": "Heart of Khvarena's Brilliance",
         "TR": "Khvarena'n\u0131n \u0130hti\u015fam\u0131n\u0131n Kalbi",
         "VI": "Tr\u00e1i Tim Khvarena Huy Ho\u00e0ng"
     },
+    "4114993540": {
+        "CHS": "\u53e4\u6d77\u7384\u5e7d\u7684\u591c\u60f3",
+        "DE": "N\u00e4chtliches Gr\u00fcbeln der uralten See",
+        "EN": "Ancient Sea's Nocturnal Musing",
+        "ES": "Nocturno del Mar de Anta\u00f1o",
+        "FR": "R\u00eaverie des eaux antiques",
+        "ID": "Ancient Sea's Nocturnal Musing",
+        "IT": "Riflessione notturna del Mare Antico",
+        "JP": "\u53e4\u6d77\u306e\u5e7d\u6df1\u306a\u308b\u591c\u60f3",
+        "KR": "\uace0\ub300 \ubc14\ub2e4\uc758 \uc57c\uc0c1\uace1",
+        "PT": "Reflex\u00e3o Noturna do Mar Antigo",
+        "RU": "\u041d\u043e\u0447\u043d\u044b\u0435 \u0440\u0430\u0437\u0434\u0443\u043c\u044c\u044f \u0434\u0440\u0435\u0432\u043d\u0435\u0433\u043e \u043c\u043e\u0440\u044f",
+        "TH": "Ancient Sea's Nocturnal Musing",
+        "TR": "Kadim Deniz'in Gece D\u00fc\u015f\u00fcnceleri",
+        "VI": "D\u1ea1 T\u1ea5u C\u1ee7a Bi\u1ec3n X\u01b0a"
+    },
     "4116721580": {
         "CHS": "\u6218\u72c2\u7684\u9aa8\u676f",
         "DE": "Berserkertrinkhorn",
         "EN": "Berserker's Bone Goblet",
         "ES": "C\u00e1liz de Hueso del Berserker",
         "FR": "Coupe du Berserker",
         "ID": "Berserker's Bone Goblet",
@@ -52395,14 +53211,30 @@
         "KR": "\ub2e8\ub2e8\ud55c \uad6c\ub9ac \ub098\uce68\ubc18",
         "PT": "B\u00fassola de Cobre",
         "RU": "\u041c\u0435\u0434\u043d\u044b\u0439 \u043a\u043e\u043c\u043f\u0430\u0441",
         "TH": "Copper Compass",
         "TR": "Bak\u0131r Pusula",
         "VI": "La B\u00e0n \u0110\u1ed3ng"
     },
+    "4253652668": {
+        "CHS": "\u7075\u9732\u503e\u6d12\u7684\u72c2\u8bd7",
+        "DE": "Rhapsodie des sprudelnden Ichors",
+        "EN": "Ichor Shower Rhapsody",
+        "ES": "Rapsodia del Icor Derramado",
+        "FR": "Rhapsodie de l'ichor d\u00e9vers\u00e9",
+        "ID": "Ichor Shower Rhapsody",
+        "IT": "Rapsodia di pioggia dell'Icore",
+        "JP": "\u964d\u308a\u6ce8\u3050\u30a4\u30b3\u30eb\u306e\u72c2\u8a69",
+        "KR": "\uc601\ud63c \uc774\uc2ac\uc758 \uad11\uc2dc\uace1",
+        "PT": "Raps\u00f3dia da Chuva de Icor",
+        "RU": "\u041d\u0435\u0438\u0441\u0442\u043e\u0432\u0430\u044f \u0440\u0430\u043f\u0441\u043e\u0434\u0438\u044f \u0438\u0445\u043e\u0440\u0430",
+        "TH": "Ichor Shower Rhapsody",
+        "TR": "\u0130khor Ya\u011fmuru Rapsodisi",
+        "VI": "\u00c1ng Th\u01a1 C\u1ee7a Linh L\u1ed9"
+    },
     "4253759884": {
         "CHS": "\u6d41\u653e\u8005\u6000\u8868",
         "DE": "Taschenuhr des Verbannten",
         "EN": "Exile's Pocket Watch",
         "ES": "Reloj de Bolsillo del Exiliado",
         "FR": "Montre de poche de l'Exil\u00e9",
         "ID": "Exile's Pocket Watch",
@@ -53659,14 +54491,30 @@
         "KR": "\uc704\uc554 \ubc18\uc11d\uc758 \uc220\uc794",
         "PT": "Ta\u00e7a do Escultor de Pedra",
         "RU": "\u041a\u0443\u0431\u043e\u043a \u0438\u0437 \u0440\u0435\u0437\u043d\u043e\u0433\u043e \u043a\u0430\u043c\u043d\u044f",
         "TH": "Goblet of Chiseled Crag",
         "TR": "Yal\u00e7\u0131n Kayal\u0131k Kadehi",
         "VI": "Ly Ng\u1ecdc B\u00e0n Th\u1ea1ch"
     },
+    "474006692": {
+        "CHS": "\u5931\u5195\u7684\u5b9d\u51a0",
+        "DE": "Kronenlose Krone",
+        "EN": "Crownless Crown",
+        "ES": "Corona Descoronada",
+        "FR": "Couronne sans couronne",
+        "ID": "Crownless Crown",
+        "IT": "Corona senza corona",
+        "JP": "\u4e3b\u306a\u304d\u51a0",
+        "KR": "\uc8fc\uc778 \uc783\uc740 \uc655\uad00",
+        "PT": "Coroa Descoroada",
+        "RU": "\u041d\u0435\u0432\u0435\u043d\u0447\u0430\u043d\u043d\u0430\u044f \u043a\u043e\u0440\u043e\u043d\u0430",
+        "TH": "Crownless Crown",
+        "TR": "Sahipsiz Ta\u00e7",
+        "VI": "V\u01b0\u01a1ng Mi\u1ec7n Qu\u00fd Kh\u00f4ng Ngai"
+    },
     "476129404": {
         "CHS": "\u5b88\u62a4\u4e4b\u82b1",
         "DE": "W\u00e4chterblume",
         "EN": "Guardian's Flower",
         "ES": "Flor del Guardi\u00e1n",
         "FR": "Fleur du Gardien",
         "ID": "Guardian's Flower",
@@ -55403,14 +56251,30 @@
         "KR": "\uc720\ubc30\uc790\uc758 \uaf43",
         "PT": "Flor do Exilado",
         "RU": "\u0426\u0432\u0435\u0442\u043e\u043a \u0438\u0437\u0433\u043d\u0430\u043d\u043d\u0438\u043a\u0430",
         "TH": "Exile's Flower",
         "TR": "S\u00fcrg\u00fcn\u00fcn \u00c7i\u00e7e\u011fi",
         "VI": "Hoa K\u1ebb L\u01b0u \u0110\u00e0y"
     },
+    "575540884": {
+        "CHS": "\u53e4\u6d77\u7384\u5e7d\u7684\u591c\u60f3",
+        "DE": "N\u00e4chtliches Gr\u00fcbeln der uralten See",
+        "EN": "Ancient Sea's Nocturnal Musing",
+        "ES": "Nocturno del Mar de Anta\u00f1o",
+        "FR": "R\u00eaverie des eaux antiques",
+        "ID": "Ancient Sea's Nocturnal Musing",
+        "IT": "Riflessione notturna del Mare Antico",
+        "JP": "\u53e4\u6d77\u306e\u5e7d\u6df1\u306a\u308b\u591c\u60f3",
+        "KR": "\uace0\ub300 \ubc14\ub2e4\uc758 \uc57c\uc0c1\uace1",
+        "PT": "Reflex\u00e3o Noturna do Mar Antigo",
+        "RU": "\u041d\u043e\u0447\u043d\u044b\u0435 \u0440\u0430\u0437\u0434\u0443\u043c\u044c\u044f \u0434\u0440\u0435\u0432\u043d\u0435\u0433\u043e \u043c\u043e\u0440\u044f",
+        "TH": "Ancient Sea's Nocturnal Musing",
+        "TR": "Kadim Deniz'in Gece D\u00fc\u015f\u00fcnceleri",
+        "VI": "D\u1ea1 T\u1ea5u C\u1ee7a Bi\u1ec3n X\u01b0a"
+    },
     "575973620": {
         "CHS": "\u5386\u7ecf\u98ce\u96ea\u7684\u601d\u5ff5",
         "DE": "Gedenken des Schneetreibens",
         "EN": "Snowswept Memory",
         "ES": "Anhelo de la Ventisca",
         "FR": "M\u00e9moires du froid",
         "ID": "Snowswept Memory",
@@ -56571,14 +57435,30 @@
         "KR": "\ub2d8\ud504\uc758 \uc2dc\uc2dc\uac01\uac01",
         "PT": "Ninfas Eternas",
         "RU": "\u041f\u043e\u0441\u0442\u043e\u044f\u043d\u0441\u0442\u0432\u043e \u043d\u0438\u043c\u0444\u044b",
         "TH": "Nymph's Constancy",
         "TR": "Nergisin Daimiyeti",
         "VI": "Th\u1eddi Kh\u1eafc C\u1ee7a Th\u1ee7y Ti\u00ean"
     },
+    "632659124": {
+        "CHS": "\u7b79\u8c0b\u7684\u5171\u6a3d",
+        "DE": "Weinflasche der Planung",
+        "EN": "The Wine-Flask Over Which the Plan Was Hatched",
+        "ES": "Jarra del Gran Plan",
+        "FR": "Coupe commune de strat\u00e9gie",
+        "ID": "The Wine-Flask Over Which the Plan Was Hatched",
+        "IT": "Calice dell'escogitativa",
+        "JP": "\u8a08\u7565\u306e\u76c3",
+        "KR": "\uacf5\ubaa8\uc758 \uc220\uc794",
+        "PT": "A Garrafa de Vinho Sobre a Qual o Plano Foi Concebido",
+        "RU": "\u0427\u0430\u0448\u0430 \u0437\u0430\u043c\u044b\u0441\u043b\u0430",
+        "TH": "The Wine-Flask Over Which the Plan Was Hatched",
+        "TR": "Plan\u0131n Haz\u0131rland\u0131\u011f\u0131 \u015earap Kadehi",
+        "VI": "Ly R\u01b0\u1ee3u C\u00f9ng B\u00e0y M\u01b0u"
+    },
     "633132620": {
         "CHS": "\u6b66\u4eba\u7684\u6c34\u6f0f",
         "DE": "Kampfk\u00fcnstler-Wasseruhr",
         "EN": "Martial Artist's Water Hourglass",
         "ES": "Reloj de Agua del Artista Marcial",
         "FR": "Sablier d'eau de l'Artiste martial",
         "ID": "Martial Artist's Water Hourglass",
@@ -57531,14 +58411,30 @@
         "KR": "\ud574\uc5f0\uc758 \uc794",
         "PT": "C\u00e1lice das Profundezas",
         "RU": "\u041a\u0443\u0431\u043e\u043a \u043e\u0433\u043b\u0443\u0448\u0430\u044e\u0449\u0438\u0445 \u0433\u043b\u0443\u0431\u0438\u043d",
         "TH": "Goblet of Thundering Deep",
         "TR": "U\u011fultulu Derinliklerin Kadehi",
         "VI": "Ly G\u1ee3n S\u00f3ng"
     },
+    "680620692": {
+        "CHS": "\u7075\u9732\u503e\u6d12\u7684\u72c2\u8bd7",
+        "DE": "Rhapsodie des sprudelnden Ichors",
+        "EN": "Ichor Shower Rhapsody",
+        "ES": "Rapsodia del Icor Derramado",
+        "FR": "Rhapsodie de l'ichor d\u00e9vers\u00e9",
+        "ID": "Ichor Shower Rhapsody",
+        "IT": "Rapsodia di pioggia dell'Icore",
+        "JP": "\u964d\u308a\u6ce8\u3050\u30a4\u30b3\u30eb\u306e\u72c2\u8a69",
+        "KR": "\uc601\ud63c \uc774\uc2ac\uc758 \uad11\uc2dc\uace1",
+        "PT": "Raps\u00f3dia da Chuva de Icor",
+        "RU": "\u041d\u0435\u0438\u0441\u0442\u043e\u0432\u0430\u044f \u0440\u0430\u043f\u0441\u043e\u0434\u0438\u044f \u0438\u0445\u043e\u0440\u0430",
+        "TH": "Ichor Shower Rhapsody",
+        "TR": "\u0130khor Ya\u011fmuru Rapsodisi",
+        "VI": "\u00c1ng Th\u01a1 C\u1ee7a Linh L\u1ed9"
+    },
     "680641668": {
         "CHS": "\u6e21\u706b\u8005\u7684\u51b3\u7edd",
         "DE": "Entschlossenheit des Laval\u00e4ufers",
         "EN": "Lavawalker's Resolution",
         "ES": "Determinaci\u00f3n del Corredor de Lava",
         "FR": "D\u00e9termination du Marcheur du feu",
         "ID": "Lavawalker's Resolution",
@@ -57979,14 +58875,30 @@
         "KR": "\uc18c\ub140\uc758 \ud754\ub4e4\ub9ac\ub294 \uadf8\ub9ac\uc6c0",
         "PT": "Lembran\u00e7as da Donzela",
         "RU": "\u0422\u043e\u0441\u043a\u0430 \u044e\u043d\u043e\u0439 \u0434\u0435\u0432\u044b",
         "TH": "Maiden's Heart-Stricken Infatuation",
         "TR": "Han\u0131m\u0131n Kara Sevdas\u0131",
         "VI": "\u00dd Ngh\u0129 C\u1ee7a Thi\u1ebfu N\u1eef"
     },
+    "700967596": {
+        "CHS": "\u5931\u5195\u7684\u5b9d\u51a0",
+        "DE": "Kronenlose Krone",
+        "EN": "Crownless Crown",
+        "ES": "Corona Descoronada",
+        "FR": "Couronne sans couronne",
+        "ID": "Crownless Crown",
+        "IT": "Corona senza corona",
+        "JP": "\u4e3b\u306a\u304d\u51a0",
+        "KR": "\uc8fc\uc778 \uc783\uc740 \uc655\uad00",
+        "PT": "Coroa Descoroada",
+        "RU": "\u041d\u0435\u0432\u0435\u043d\u0447\u0430\u043d\u043d\u0430\u044f \u043a\u043e\u0440\u043e\u043d\u0430",
+        "TH": "Crownless Crown",
+        "TR": "Sahipsiz Ta\u00e7",
+        "VI": "V\u01b0\u01a1ng Mi\u1ec7n Qu\u00fd Kh\u00f4ng Ngai"
+    },
     "701624180": {
         "CHS": "\u68a6\u9192\u4e4b\u74e2",
         "DE": "Kalebasse des Erwachens",
         "EN": "Calabash of Awakening",
         "ES": "Calabaza del Despertar",
         "FR": "Calebasse d'\u00e9veil",
         "ID": "Calabash of Awakening",
@@ -59355,14 +60267,30 @@
         "KR": "\uc18c\ub140\uc758 \uc9e7\uc740 \ud589\ubcf5",
         "PT": "Juventude Passageira da Donzela",
         "RU": "\u0423\u0445\u043e\u0434\u044f\u0449\u0430\u044f \u043c\u043e\u043b\u043e\u0434\u043e\u0441\u0442\u044c \u044e\u043d\u043e\u0439 \u0434\u0435\u0432\u044b",
         "TH": "Maiden's Passing Youth",
         "TR": "Han\u0131m\u0131n Kaybolan Gen\u00e7li\u011fi",
         "VI": "Th\u1eddi Gian Ch\u1edd \u0110\u1ee3i C\u1ee7a Thi\u1ebfu N\u1eef"
     },
+    "777741588": {
+        "CHS": "\u892a\u5149\u7684\u7fe0\u5c3e",
+        "DE": "Verblasste Smaragdschwanzfeder",
+        "EN": "Faded Emerald Tail",
+        "ES": "Cola Esmeralda Descolorida",
+        "FR": "Queue \u00e9meraude de fanaison",
+        "ID": "Faded Emerald Tail",
+        "IT": "Coda smeraldina scolorita",
+        "JP": "\u5149\u892a\u305b\u305f\u7fe0\u5c3e",
+        "KR": "\ube5b\ubc14\ub79c \ud478\ub978 \uaf41\uc9c0",
+        "PT": "Cauda de Esmeralda Desbotada",
+        "RU": "\u0411\u043b\u0451\u043a\u043b\u044b\u0439 \u0438\u0437\u0443\u043c\u0440\u0443\u0434\u043d\u044b\u0439 \u0445\u0432\u043e\u0441\u0442",
+        "TH": "Faded Emerald Tail",
+        "TR": "Solmu\u015f Z\u00fcmr\u00fct Kuyruk",
+        "VI": "\u0110u\u00f4i Ph\u1ec9 Th\u00fay Phai M\u00e0u"
+    },
     "777899188": {
         "CHS": "\u4e0d\u52a8\u7384\u77f3\u4e4b\u76f8",
         "DE": "Maske des starren Gesteins",
         "EN": "Mask of Solitude Basalt",
         "ES": "M\u00e1scara de Basalto Inerte",
         "FR": "Masque en basalte inerte",
         "ID": "Mask of Solitude Basalt",
@@ -59995,14 +60923,30 @@
         "KR": "\uc774\uad6d\uc758 \uc220\uc794",
         "PT": "C\u00e1lice de Uma Terra Desconhecida",
         "RU": "\u041a\u0443\u0431\u043e\u043a \u0432\u0440\u0435\u043c\u0435\u043d\u0449\u0438\u043a\u0430",
         "TH": "Goblet of the Sojourner",
         "TR": "Yolcunun Kadehi",
         "VI": "Chi\u1ebfc Ly D\u1ecb Qu\u1ed1c"
     },
+    "814298500": {
+        "CHS": "\u6697\u7ed3\u7684\u660e\u82b1",
+        "DE": "Helle Bl\u00fcte dunkler Fr\u00fcchte",
+        "EN": "Dark Fruit of Bright Flowers",
+        "ES": "Flor Secreta Rutilante",
+        "FR": "Fleur de n\u0153uds dissimul\u00e9s",
+        "ID": "Dark Fruit of Bright Flowers",
+        "IT": "Frutto fosco di fiori limpidi",
+        "JP": "\u9670\u306b\u54b2\u304f\u5149\u306e\u82b1",
+        "KR": "\uc5b4\ub460 \uc18d\uc758 \ubc1d\uc740 \uaf43",
+        "PT": "Fruto Sombrio de Flores Brilhantes",
+        "RU": "\u0422\u0451\u043c\u043d\u044b\u0439 \u043f\u043b\u043e\u0434 \u044f\u0440\u043a\u0438\u0445 \u0446\u0432\u0435\u0442\u043e\u0432",
+        "TH": "Dark Fruit of Bright Flowers",
+        "TR": "Parlak \u00c7i\u00e7eklerin Koyu Meyvesi",
+        "VI": "Hoa S\u00e1ng C\u1ee7a Qu\u1ea3 \u0110en"
+    },
     "815154916": {
         "CHS": "\u5b97\u5ba4\u4e4b\u7fce",
         "DE": "K\u00f6nigliche Feder",
         "EN": "Royal Plume",
         "ES": "Pluma Real",
         "FR": "Plume du Noble",
         "ID": "Royal Plume",
@@ -60235,14 +61179,30 @@
         "KR": "\uad50\uad00\uc758 \ud68c\uc911\uc2dc\uacc4",
         "PT": "Rel\u00f3gio de Bolso de Instrutor",
         "RU": "\u041a\u0430\u0440\u043c\u0430\u043d\u043d\u044b\u0435 \u0447\u0430\u0441\u044b \u0438\u043d\u0441\u0442\u0440\u0443\u043a\u0442\u043e\u0440\u0430",
         "TH": "Instructor's Pocket Watch",
         "TR": "E\u011fitmenin Cep Saati",
         "VI": "\u0110\u1ed3ng H\u1ed3 Gi\u00e1o Quan"
     },
+    "832863868": {
+        "CHS": "\u8c10\u5f8b\u4ea4\u54cd\u7684\u524d\u594f",
+        "DE": "Vorspiel der harmonischen Sinfonie",
+        "EN": "Harmonious Symphony Prelude",
+        "ES": "Preludio de la Sinfon\u00eda Arm\u00f3nica",
+        "FR": "Pr\u00e9lude des symphonies harmoniques",
+        "ID": "Harmonious Symphony Prelude",
+        "IT": "Preludio della Sinfonia armonica",
+        "JP": "\u97ff\u304d\u5408\u3046\u8ae7\u5f8b\u306e\u524d\u594f",
+        "KR": "\uc870\ud654\ub85c\uc6b4 \uc804\uc8fc\uace1",
+        "PT": "Prel\u00fadio da Sinfonia Harmoniosa",
+        "RU": "\u0423\u0432\u0435\u0440\u0442\u044e\u0440\u0430 \u0441\u0442\u0440\u043e\u0439\u043d\u043e\u0439 \u0441\u0438\u043c\u0444\u043e\u043d\u0438\u0438",
+        "TH": "Harmonious Symphony Prelude",
+        "TR": "Ahenkli Senfoninin Ba\u015flang\u0131c\u0131",
+        "VI": "D\u1ea1o \u0110\u1ea7u C\u1ee7a Giao H\u01b0\u1edfng"
+    },
     "834707436": {
         "CHS": "\u6d41\u653e\u8005\u4e4b\u82b1",
         "DE": "Blume des Verbannten",
         "EN": "Exile's Flower",
         "ES": "Flor del Exiliado",
         "FR": "Fleur de l'Exil\u00e9",
         "ID": "Exile's Flower",
```

### Comparing `enkanetworkv2.py-2.0.4/enkanetwork/assets/langs/characters.json` & `enkanetworkv2.py-2.0.5/enkanetwork/assets/langs/characters.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9878048780487805%*

 * *Differences: {"'167199474'": "OrderedDict([('CHS', '阿蕾奇诺'), ('DE', 'Arlecchino'), ('EN', 'Arlecchino'), ('ES', "*

 * *                "'Arlecchino'), ('FR', 'Arlecchino'), ('ID', 'Arlecchino'), ('IT', 'Arlecchino'), "*

 * *                "('JP', 'アルレッキーノ'), ('KR', '아를레키노'), ('PT', 'Arlecchino'), ('RU', 'Арлекино'), "*

 * *                "('TH', 'Arlecchino'), ('TR', 'Arlecchino'), ('VI', 'Arlecchino')])"}*

```diff
@@ -203,14 +203,30 @@
         "KR": "\uce74\ubbf8\uc0ac\ud1a0 \uc544\uc57c\ud1a0",
         "PT": "Kamisato Ayato",
         "RU": "\u0410\u044f\u0442\u043e",
         "TH": "Kamisato Ayato",
         "TR": "Kamisato Ayato",
         "VI": "Kamisato Ayato"
     },
+    "167199474": {
+        "CHS": "\u963f\u857e\u5947\u8bfa",
+        "DE": "Arlecchino",
+        "EN": "Arlecchino",
+        "ES": "Arlecchino",
+        "FR": "Arlecchino",
+        "ID": "Arlecchino",
+        "IT": "Arlecchino",
+        "JP": "\u30a2\u30eb\u30ec\u30c3\u30ad\u30fc\u30ce",
+        "KR": "\uc544\ub97c\ub808\ud0a4\ub178",
+        "PT": "Arlecchino",
+        "RU": "\u0410\u0440\u043b\u0435\u043a\u0438\u043d\u043e",
+        "TH": "Arlecchino",
+        "TR": "Arlecchino",
+        "VI": "Arlecchino"
+    },
     "168956722": {
         "CHS": "\u4e03\u4e03",
         "DE": "Qiqi",
         "EN": "Qiqi",
         "ES": "Qiqi",
         "FR": "Qiqi",
         "ID": "Qiqi",
```

### Comparing `enkanetworkv2.py-2.0.4/enkanetwork/assets/langs/constellations.json` & `enkanetworkv2.py-2.0.5/enkanetwork/assets/langs/constellations.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9882352941176471%*

 * *Differences: {"'1222541609'": "OrderedDict([('CHS', '「你将成为我们新的家人…」'), ('DE', '„Du wirst Teil unserer Familie "*

 * *                 'werden ...“\'), (\'EN\', \'"You Shall Become a New Member of Our Family..."\'), '*

 * *                 "('ES', 'Tú serás el nuevo miembro de nuestra familia'), ('FR', '« Vous "*

 * *                 'deviendrez notre nouvelle famille... »\'), (\'ID\', \'"You Shall Become a New '*

 * *                 'Member of Our Family ..."\'), (\'IT\', \'"Diventerai un nuovo membro della '*

 * *                 'nostra famig […]*

```diff
@@ -427,14 +427,30 @@
         "KR": "\uac15\uc544\uc9c0 \ub3cc\uc9c4\u00b7\uc6c0\uc9c1\uc784\uc740 \ubc88\uac1c\ucc98\ub7fc",
         "PT": "Pegureiro Atacante: For\u00e7a Trovejante",
         "RU": "\u0423\u0434\u0430\u0440 \u0441\u043e\u0431\u0430\u043a\u0438: \u0421\u0438\u043b\u0430 \u0433\u0440\u043e\u043c\u0430",
         "TH": "Striking Hound: Thunderous Force",
         "TR": "G\u00fc\u00e7l\u00fc Taz\u0131: Y\u0131ld\u0131r\u0131m Gibi \u015eiddetli",
         "VI": "C\u1eafn: Kinh \u0110\u1ed9ng Nh\u01b0 S\u1ea5m"
     },
+    "1222541609": {
+        "CHS": "\u300c\u4f60\u5c06\u6210\u4e3a\u6211\u4eec\u65b0\u7684\u5bb6\u4eba\u2026\u300d",
+        "DE": "\u201eDu wirst Teil unserer Familie werden ...\u201c",
+        "EN": "\"You Shall Become a New Member of Our Family...\"",
+        "ES": "T\u00fa ser\u00e1s el nuevo miembro de nuestra familia",
+        "FR": "\u00ab Vous deviendrez notre nouvelle famille... \u00bb",
+        "ID": "\"You Shall Become a New Member of Our Family ...\"",
+        "IT": "\"Diventerai un nuovo membro della nostra famiglia...\"",
+        "JP": "\u300c\u541b\u306f\u79c1\u305f\u3061\u306e \u65b0\u3057\u3044\u5bb6\u65cf\u306b\u306a\u308b\u3093\u3060\u2026\u300d",
+        "KR": "\u300c\uc6b0\ub9ac\uc758 \uc0c8 \uac00\uc871\uc774 \ub418\uc5c8\uc73c\ub2c8\u2026\u300d",
+        "PT": "\"Voc\u00ea se Tornar\u00e1 um Novo Membro da Nossa Fam\u00edlia...\"",
+        "RU": "\u00ab\u0422\u044b \u0441\u0442\u0430\u043d\u0435\u0448\u044c \u043d\u043e\u0432\u044b\u043c \u0447\u043b\u0435\u043d\u043e\u043c \u043d\u0430\u0448\u0435\u0439 \u0441\u0435\u043c\u044c\u0438...\u00bb",
+        "TH": "\"You Shall Become a New Member of Our Family...\"",
+        "TR": "\"Ailemizin Yeni \u00dcyesi Olacaks\u0131n...\"",
+        "VI": "\"Ng\u01b0\u01a1i S\u1ebd Tr\u1edf Th\u00e0nh Th\u00e0nh Vi\u00ean M\u1edbi C\u1ee7a Gia \u0110\u00ecnh Ta...\""
+    },
     "1235684201": {
         "CHS": "\u7a7a\u53d6\u5947\u601d\u7684\u624b\u827a",
         "DE": "Bizarre Wunder",
         "EN": "Whimsical Wonders",
         "ES": "Truco telequin\u00e9tico",
         "FR": "Art de mysticit\u00e9",
         "ID": "Whimsical Wonders",
@@ -1803,14 +1819,30 @@
         "KR": "\uae30\ub9cc\uc790\uc5d0\uac8c \ucc98\ubc8c\uc744",
         "PT": "Punindo as Fraudes",
         "RU": "\u041d\u0430\u043a\u0430\u0437\u0430\u0442\u044c \u0430\u043b\u0447\u043d\u044b\u0445 \u0438 \u0431\u0435\u0441\u0447\u0435\u0441\u0442\u043d\u044b\u0445",
         "TH": "Punishment for the Frauds",
         "TR": "Sahtekarlara Ukubet",
         "VI": "Khi\u1ec3n Tr\u00e1ch K\u1ebb D\u1ed1i Gian"
     },
+    "1931573609": {
+        "CHS": "\u300c\u6240\u6709\u7684\u4ec7\u4e0e\u503a\u7686\u7531\u6211\u507f\u2026\u300d",
+        "DE": "\u201eJeden Groll und alle Schulden werde ich begleichen ...\u201c",
+        "EN": "\"All Reprisals and Arrears, Mine to Bear...\"",
+        "ES": "Yo cargar\u00e9 con todas las deudas y el odio",
+        "FR": "\u00ab \u00c0 moi de supporter toute haine et toute dette... \u00bb",
+        "ID": "\"All Reprisals and Arrears, Mine to Bear...\"",
+        "IT": "\"Sono io a sopportare ogni interesse o rappresaglia...\"",
+        "JP": "\u300c\u3042\u3089\u3086\u308b\u6028\u307f\u3068\u501f\u308a\u306f \u79c1\u304c\u6e05\u7b97\u3057\u3088\u3046\u2026\u300d",
+        "KR": "\u300c\ubaa8\ub4e0 \uc6d0\ud55c\uacfc \ube5a\uc740 \ub0b4\uac00 \uac1a\uace0\u2026\u300d",
+        "PT": "\"Todas as Vingan\u00e7as e D\u00edvidas s\u00e3o Minhas...\"",
+        "RU": "\u00ab\u0412\u0441\u0435 \u0432\u043e\u0437\u043c\u0435\u0437\u0434\u0438\u044f \u0438 \u043f\u043e\u0432\u0438\u043d\u043d\u043e\u0441\u0442\u0438 \u043f\u043e\u043d\u0435\u0441\u0443 \u044f...\u00bb",
+        "TH": "\"All Reprisals and Arrears, Mine to Bear...\"",
+        "TR": "\"T\u00fcm \u0130ntikamlar ve Bor\u00e7lar Bana Aittir...\"",
+        "VI": "\"T\u1ea5t C\u1ea3 Th\u00f9 V\u00e0 N\u1ee3 Do Ta T\u1ef1 Tr\u1ea3...\""
+    },
     "1939010113": {
         "CHS": "\u56de\u8f6c\u7684\u6012\u98ce",
         "DE": "Wirbelnder Wind",
         "EN": "Raging Vortex",
         "ES": "Torbellino furioso",
         "FR": "Vortex d\u00e9cha\u00een\u00e9",
         "ID": "Raging Vortex",
@@ -2251,14 +2283,30 @@
         "KR": "\ub178\ub825\uc774 \uace7 \ub9c8\ubc95",
         "PT": "A Aten\u00e7\u00e3o \u00e9 o Meu Poder",
         "RU": "\u041c\u0430\u0433\u0438\u044f \u0443\u0441\u0435\u0440\u0434\u0438\u044f",
         "TH": "Attentiveness be My Power",
         "TR": "\u00c7al\u0131\u015fkanl\u0131\u011f\u0131n B\u00fcy\u00fcs\u00fc",
         "VI": "N\u1ed7 L\u1ef1c L\u00e0 Ma Thu\u1eadt"
     },
+    "2103473001": {
+        "CHS": "\u300c\u6b64\u540e\uff0c\u4f60\u4eec\u987b\u76f8\u7231\u76f8\u62a4\u2026\u300d",
+        "DE": "\u201eVon nun an m\u00fcsst ihr euch gegenseitig lieben und besch\u00fctzen ...\u201c",
+        "EN": "\"You Shall Love and Protect Each Other Henceforth...\"",
+        "ES": "Entonces, se amar\u00e1n y se proteger\u00e1n",
+        "FR": "\u00ab D\u00e9sormais, vous devez vous aimer et vous prot\u00e9ger... \u00bb",
+        "ID": "\"You Shall Love and Protect Each Other Henceforth ...\"",
+        "IT": "\"D'ora in avanti, amatevi e proteggetevi l'un l'altro...\"",
+        "JP": "\u300c\u3053\u308c\u304b\u3089\u306f\u4e92\u3044\u3092\u6148\u3057\u307f \u624b\u3092\u53d6\u308a\u5408\u3046\u3068\u3057\u3088\u3046\u2026\u300d",
+        "KR": "\u300c\uc55e\uc73c\ub85c \uc0ac\uc774\uc88b\uac8c \uc9c0\ub0b4\uac70\ub77c\u2026\u300d",
+        "PT": "\"De Hoje em Diante, Amor e Prote\u00e7\u00e3o M\u00fatua...\"",
+        "RU": "\u00ab\u0412\u043f\u0440\u0435\u0434\u044c \u043b\u044e\u0431\u0438\u0442\u0435 \u0438 \u0437\u0430\u0449\u0438\u0449\u0430\u0439\u0442\u0435 \u0434\u0440\u0443\u0433 \u0434\u0440\u0443\u0433\u0430...\u00bb",
+        "TH": "\"You Shall Love and Protect Each Other Henceforth...\"",
+        "TR": "\"Bundan B\u00f6yle Birbirinizi Sevip Koruyun...\"",
+        "VI": "\"Sau N\u00e0y, C\u00e1c Ng\u01b0\u01a1i Y\u00eau Th\u01b0\u01a1ng T\u01b0\u01a1ng Tr\u1ee3 Nhau...\""
+    },
     "2112971153": {
         "CHS": "\u843d\u67d3\u4e94\u8272",
         "DE": "F\u00fcnffarbige F\u00e4rbung",
         "EN": "In Five Colors Dyed",
         "ES": "Tintura pol\u00edcroma",
         "FR": "Cinq couleurs de la teinture",
         "ID": "In Five Colors Dyed",
@@ -3659,14 +3707,30 @@
         "KR": "\uc870\ub958\ubc1c\uc804",
         "PT": "Invocadora da Tempestade",
         "RU": "\u041f\u0440\u0438\u0437\u044b\u0432 \u0431\u0443\u0440\u0438",
         "TH": "Summoner of Storm",
         "TR": "F\u0131rt\u0131na Sihirdar\u0131",
         "VI": "Th\u1ee7y Tri\u1ec1u D\u1eabn \u0110i\u1ec7n"
     },
+    "2743280569": {
+        "CHS": "\u300c\u6240\u6709\u7684\u8d4f\u4e0e\u7f5a\u7686\u81ea\u6211\u51fa\u2026\u300d",
+        "DE": "\u201eJede Belohnung und Vergeltung wird von mir vergeben ...\u201c",
+        "EN": "\"All Rewards and Retribution, Mine to Bestow...\"",
+        "ES": "Yo otorgar\u00e9 toda recompensa y castigo",
+        "FR": "\u00ab \u00c0 moi d'accorder toute r\u00e9compense et toute punition... \u00bb",
+        "ID": "\"All Rewards and Retribution, Mine to Bestow...\"",
+        "IT": "\"Sono io a conferire ogni punizione o ricompensa...\"",
+        "JP": "\u300c\u3042\u3089\u3086\u308b\u8912\u8cde\u3068\u7f70\u306f \u3053\u306e\u624b\u306b\u3088\u308b\u3082\u306e\u2026\u300d",
+        "KR": "\u300c\ubaa8\ub4e0 \uc0c1\ubc8c\uc740 \ub0b4\uac00 \ub0b4\ub9b4 \uac83\uc774\ub2e4\u2026\u300d",
+        "PT": "\"Todas as Recompensas e Retribui\u00e7\u00f5es s\u00e3o Minhas para Dar...\"",
+        "RU": "\u00ab\u0417\u0430 \u0434\u043e\u0431\u0440\u044b\u0435 \u0434\u0435\u044f\u043d\u0438\u044f \u0438 \u043f\u0440\u0435\u0433\u0440\u0435\u0448\u0435\u043d\u0438\u044f \u0432\u043e\u0437\u0434\u0430\u043c \u044f...\u00bb",
+        "TH": "\"All Rewards and Retribution, Mine to Bestow...\"",
+        "TR": "\"T\u00fcm \u00d6d\u00fcller ve Cezalar Bendendir...\"",
+        "VI": "\"T\u1ea5t C\u1ea3 Th\u01b0\u1edfng V\u00e0 Ph\u1ea1t Do Ta T\u1ef1 Ra...\""
+    },
     "2746616153": {
         "CHS": "\u793a\u8fa8\u771f\u610f\u7684\u773c",
         "DE": "Enth\u00fcllende Einsicht",
         "EN": "Watchful Eye",
         "ES": "El ojo de la verdad",
         "FR": "\u0152il perspicace",
         "ID": "Watchful Eye",
@@ -5003,14 +5067,30 @@
         "KR": "\uc5b8\ub355\uacfc \uc0b0\ub9bc\uc744 \uc9c0\ub098",
         "PT": "Pelas Colinas e Bosques",
         "RU": "\u041f\u043e \u0433\u043e\u0440\u0430\u043c \u0438 \u043b\u0435\u0441\u0430\u043c",
         "TH": "Through Hill and Copse",
         "TR": "Tepe ve \u00c7al\u0131l\u0131k Boyunca",
         "VI": "D\u1ea1o B\u01b0\u1edbc \u0110\u1ed3i C\u1ecf"
     },
+    "3475324945": {
+        "CHS": "\u300c\u6211\u4eec\u5df2\u5b51\u7136\u4e00\u8eab\uff0c\u4e0e\u6b7b\u65e0\u5f02\u2026\u300d",
+        "DE": "\u201eAllein sind wir so gut wie tot ...\u201c",
+        "EN": "\"For Alone, We Are as Good as Dead...\"",
+        "ES": "Nuestra soledad se equipara a la muerte",
+        "FR": "\u00ab Car seuls, c'est la mort qui nous attend... \u00bb",
+        "ID": "\"For Alone, We Are as Good as Dead ...\"",
+        "IT": "\"Nella solitudine, siamo come spoglie esanimi...\"",
+        "JP": "\u300c\u79c1\u305f\u3061\u306f\u307f\u306a\u72ec\u6cd5\u5e2b\u3060 \u6211\u3089\u304c\u8eab\u306f\u5c4d\u3082\u540c\u7136\u2026\u300d",
+        "KR": "\u300c\uace0\ub3c5\ud55c \uc6b0\ub9ac\ub294 \ub9dd\uc790\uc640 \ub2e4\ub984\uc5c6\uc73c\ub098\u2026\u300d",
+        "PT": "\"Sozinhos, Estamos Mortos...\"",
+        "RU": "\u00ab\u041f\u043e \u043e\u0434\u0438\u043d\u043e\u0447\u043a\u0435 \u043c\u044b \u0432\u0441\u0451 \u0440\u0430\u0432\u043d\u043e \u0447\u0442\u043e \u043c\u0435\u0440\u0442\u0432\u044b...\u00bb",
+        "TH": "\"For Alone, We Are as Good as Dead...\"",
+        "TR": "\"Yaln\u0131zl\u0131\u011f\u0131m\u0131z \u00d6l\u00fcmle Birdir...\"",
+        "VI": "\"V\u00ec M\u1ed9t M\u00ecnh Kh\u00e1c G\u00ec V\u1edbi \u0110\u00e3 Ch\u1ebft...\""
+    },
     "3475888113": {
         "CHS": "\u5374\u6708\u7684\u8f7b\u821e",
         "DE": "Tanz des abnehmenden Mondes",
         "EN": "Dance of the Waning Moon",
         "ES": "Danza de la luna menguante",
         "FR": "Danse de la lune d\u00e9croissante",
         "ID": "Dance of the Waning Moon",
@@ -7083,14 +7163,30 @@
         "KR": "\uc625\ud640\u00b7\ubd80\uc11c\uc838\ub3c4 \uac74\uc7ac\ud55c \uacac\uace0\ud568",
         "PT": "Top\u00e1zio, Inquebr\u00e1vel e Destemido",
         "RU": "\u0422\u043e\u043f\u0430\u0437, \u043d\u0435\u0441\u043b\u043e\u043c\u043b\u0435\u043d\u043d\u044b\u0439 \u0438 \u0431\u0435\u0441\u0441\u0442\u0440\u0430\u0448\u043d\u044b\u0439",
         "TH": "Topaz, Unbreakable and Fearless",
         "TR": "Sars\u0131lmaz ve Korkusuz Topaz",
         "VI": "Ho\u00e0ng T\u00f4ng, Ph\u00e1 Nh\u01b0ng Kh\u00f4ng M\u1ea5t Ki\u00ean C\u01b0\u1eddng"
     },
+    "585561937": {
+        "CHS": "\u300c\u81ea\u6b64\u4ee5\u540e\uff0c\u6211\u4eec\u5c06\u5171\u98e8\u65b0\u751f\u3002\u300d",
+        "DE": "\u201eVon nun an werden wir gemeinsam ein neues Leben f\u00fchren.\u201c",
+        "EN": "\"From This Day On, We Shall Delight in New Life Together.\"",
+        "ES": "As\u00ed pues, disfrutemos de una nueva vida",
+        "FR": "\u00ab D\u00e9sormais, nous vivrons ensemble une nouvelle vie. \u00bb",
+        "ID": "\"From This Day On, We Shall Delight in New Life Together.\"",
+        "IT": "\"Da oggi in poi, potremo gioire insieme di una nuova vita.\"",
+        "JP": "\u300c\u3053\u306e\u5148\u3001\u6211\u3005\u306f \u2014\u2014\u65b0\u3057\u304d\u751f\u306b\u8208\u3058\u308b\u300d",
+        "KR": "\u300c\uc55e\uc73c\ub85c \uc6b0\ub9ac\ub294 \uc0c8 \uc0dd\uba85\uc744 \ub204\ub9ac\ub9ac\ub77c\u300d",
+        "PT": "\"De Hoje em Diante, Nos Deliciaremos numa Nova Vida.\"",
+        "RU": "\u00ab\u0412\u043e\u0437\u0440\u0430\u0434\u0443\u0435\u043c\u0441\u044f \u043d\u043e\u0432\u043e\u0439 \u0436\u0438\u0437\u043d\u0438 \u0432\u043c\u0435\u0441\u0442\u0435\u00bb",
+        "TH": "\"From This Day On, We Shall Delight in New Life Together\"",
+        "TR": "\"Bug\u00fcnden \u0130tibaren Yeni Bir Hayat\u0131n Tad\u0131n\u0131 \u00c7\u0131karal\u0131m.\"",
+        "VI": "\"T\u1eeb Nay V\u1ec1 Sau, Ch\u00fang Ta S\u1ebd C\u00f9ng \u0110\u00f3n Cu\u1ed9c S\u1ed1ng M\u1edbi.\""
+    },
     "600240137": {
         "CHS": "\u8fde\u73af\u8f70\u9686",
         "DE": "Kettenreaktion",
         "EN": "Chained Reactions",
         "ES": "Explosi\u00f3n en cadena",
         "FR": "Bombardement continu",
         "ID": "Chained Reaction",
```

### Comparing `enkanetworkv2.py-2.0.4/enkanetwork/assets/langs/fight_props.json` & `enkanetworkv2.py-2.0.5/enkanetwork/assets/langs/fight_props.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.4/enkanetwork/assets/langs/namecards.json` & `enkanetworkv2.py-2.0.5/enkanetwork/assets/langs/namecards.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9743589743589743%*

 * *Differences: {"'1686874332'": "OrderedDict([('CHS', '成就·掣鲸'), ('DE', 'Errungenschaft – Walbändiger'), ('EN', "*

 * *                 "'Achievement: Whalewrangler'), ('ES', 'Logro - Cazanarvales'), ('FR', 'Succès - "*

 * *                 "Baleinier'), ('ID', 'Achievement: Penjinak Paus'), ('IT', 'Obiettivo: "*

 * *                 "Cacciabalene'), ('JP', 'アチーブメント·掣鯨'), ('KR', '업적·포경'), ('PT', 'Conquista: "*

 * *                 "Destruidor de Baleias'), ('RU', 'Укротитель китов'), ('TH', 'ความสำเร็จ - "*

 * *                 "ล่าวาฬ'), ('TR', ' […]*

```diff
@@ -603,14 +603,30 @@
         "KR": "\ub9ac\ub137\u00b7\uc9c4\uc2ec",
         "PT": "Lynette - Seriedade",
         "RU": "\u0421\u0435\u0440\u044c\u0451\u0437\u043d\u043e\u0441\u0442\u044c",
         "TH": "Lynette - \u0e01\u0e25\u0e32\u0e22\u0e40\u0e1b\u0e47\u0e19\u0e08\u0e23\u0e34\u0e07",
         "TR": "Lynette: \u0130\u00e7tenlik",
         "VI": "Lynette - Th\u00e0nh Th\u1eadt"
     },
+    "1686874332": {
+        "CHS": "\u6210\u5c31\u00b7\u63a3\u9cb8",
+        "DE": "Errungenschaft \u2013 Walb\u00e4ndiger",
+        "EN": "Achievement: Whalewrangler",
+        "ES": "Logro - Cazanarvales",
+        "FR": "Succ\u00e8s - Baleinier",
+        "ID": "Achievement: Penjinak Paus",
+        "IT": "Obiettivo: Cacciabalene",
+        "JP": "\u30a2\u30c1\u30fc\u30d6\u30e1\u30f3\u30c8\u00b7\u63a3\u9be8",
+        "KR": "\uc5c5\uc801\u00b7\ud3ec\uacbd",
+        "PT": "Conquista: Destruidor de Baleias",
+        "RU": "\u0423\u043a\u0440\u043e\u0442\u0438\u0442\u0435\u043b\u044c \u043a\u0438\u0442\u043e\u0432",
+        "TH": "\u0e04\u0e27\u0e32\u0e21\u0e2a\u0e33\u0e40\u0e23\u0e47\u0e08 - \u0e25\u0e48\u0e32\u0e27\u0e32\u0e2c",
+        "TR": "Ba\u015far\u0131m: Balina Terbiyecisi",
+        "VI": "Th\u00e0nh T\u1ef1u - S\u0103n C\u00e1 Voi"
+    },
     "1688417908": {
         "CHS": "\u9e7f\u91ce\u9662\u5e73\u85cf\u00b7\u97a0\u6bec",
         "DE": "Shikanoin Heizou \u2013 Temari",
         "EN": "Shikanoin Heizou: Temari",
         "ES": "Shikanoin Heizou - Temari",
         "FR": "Shikanoin Heizou - Temari",
         "ID": "Shikanoin Heizou: Temari",
@@ -683,14 +699,30 @@
         "KR": "\uc5c5\uc801\u00b7\ud3b8\uc720",
         "PT": "Conquista - Explorador",
         "RU": "\u0418\u0441\u0441\u043b\u0435\u0434\u043e\u0432\u0430\u0442\u0435\u043b\u044c",
         "TH": "\u0e04\u0e27\u0e32\u0e21\u0e2a\u0e33\u0e40\u0e23\u0e47\u0e08 - \u0e19\u0e31\u0e01\u0e2a\u0e33\u0e23\u0e27\u0e08",
         "TR": "Ba\u015far\u0131m: Ka\u015fif",
         "VI": "Th\u00e0nh t\u1ef1u - \u0110i kh\u1eafp n\u01a1i"
     },
+    "1744889084": {
+        "CHS": "\u7eaa\u884c\u00b7\u90a6\u6447",
+        "DE": "Erlebnispass \u2013 Rock \u2019n\u2019 Roll",
+        "EN": "Travel Notes: The Realms Rocked",
+        "ES": "PB - Tierra del rock",
+        "FR": "PB - Rock-athon",
+        "ID": "Catatan Perjalanan: Alam Bergetar",
+        "IT": "Appunti di viaggio: Regni del rock",
+        "JP": "\u7d00\u884c\u00b7\u90a6\u9b42",
+        "KR": "\uae30\ud589\u00b7\ub85c\ud070\ub864",
+        "PT": "Passe de Batalha: Rock Pauleira",
+        "RU": "\u0420\u043e\u043a-\u043a\u043e\u0440\u043e\u043b\u0435\u0432\u0441\u0442\u0432\u0430",
+        "TH": "\u0e1a\u0e31\u0e19\u0e17\u0e36\u0e01 - \u0e2a\u0e31\u0e48\u0e19\u0e2a\u0e30\u0e17\u0e49\u0e32\u0e19",
+        "TR": "Gezi Notlar\u0131: Rock 'N' Roll Diyarlar",
+        "VI": "Nh\u1eadt K\u00fd H\u00e0nh Tr\u00ecnh - Rung Chuy\u1ec3n"
+    },
     "1763845860": {
         "CHS": "\u6210\u5c31\u00b7\u65c5\u5c45",
         "DE": "Errungenschaft \u2013 Feriendomizil",
         "EN": "Achievement: Vacation Home",
         "ES": "Logro - Estancia vacacional",
         "FR": "Succ\u00e8s - Maison de vacances",
         "ID": "Achievement: Rumah Liburan",
@@ -1755,14 +1787,30 @@
         "KR": "\ubaac\ub4dc\u00b7\ucd95\ubcf5",
         "PT": "Mondstadt - B\u00ean\u00e7\u00e3o",
         "RU": "\u041c\u043e\u043b\u0438\u0442\u0432\u0430",
         "TH": "Mondstadt - Blessing",
         "TR": "Mondstadt: L\u00fctuf",
         "VI": "Mondstadt - Ch\u00fac Ph\u00fac"
     },
+    "328422540": {
+        "CHS": "\u67ab\u4e39\u00b7\u9732\u6cc9",
+        "DE": "Fontaine \u2013 Tauwasserbrunnen",
+        "EN": "Fontaine: Lucine",
+        "ES": "Fontaine - Lucine",
+        "FR": "Fontaine - Lucine",
+        "ID": "Fontaine: Air Mancur Embun",
+        "IT": "Fontaine: Lucine",
+        "JP": "\u30d5\u30a9\u30f3\u30c6\u30fc\u30cc\u00b7\u30eb\u30ad\u30ca",
+        "KR": "\ud3f0\ud0c0\uc778\u00b7\ub8e8\ud0a4\ub098 \ubd84\uc218",
+        "PT": "Fontaine: Nascente do Orvalho",
+        "RU": "\u041b\u044e\u0441\u0438\u043d",
+        "TH": "Fontaine - \u0e2a\u0e23\u0e30\u0e19\u0e49\u0e33\u0e1e\u0e38",
+        "TR": "Fontaine: Lucine",
+        "VI": "Fontaine - Su\u1ed1i S\u01b0\u01a1ng"
+    },
     "3292114052": {
         "CHS": "\u5343\u7ec7\u00b7\u5c55\u8896",
         "DE": "Chiori \u2013 Spektakul\u00e4re \u00c4rmel",
         "EN": "Chiori: Spectacular Sleeves",
         "ES": "Chiori - Tamoto",
         "FR": "Chiori - Manches spectaculaires",
         "ID": "Chiori: Spectacular Sleeves",
@@ -2219,14 +2267,30 @@
         "KR": "\uae30\ud589\u00b7\ubc31\uc601(\u767d\u82f1)",
         "PT": "Passe Batalha - Lyratum",
         "RU": "\u041f\u0430\u0441\u043b\u0451\u043d",
         "TH": "\u0e1a\u0e31\u0e19\u0e17\u0e36\u0e01 - \u0e01\u0e25\u0e35\u0e1a\u0e14\u0e2d\u0e01\u0e44\u0e21\u0e49\u0e02\u0e32\u0e27",
         "TR": "Gezi Notlar\u0131: Beyaz Yaprak",
         "VI": "Nh\u1eadt K\u00fd H\u00e0nh Tr\u00ecnh - Lyratum"
     },
+    "3853344316": {
+        "CHS": "\u67ab\u4e39\u00b7\u8c03\u5f8b",
+        "DE": "Fontaine \u2013 Abstimmung",
+        "EN": "Fontaine: Attunement",
+        "ES": "Fontaine - Afinaci\u00f3n",
+        "FR": "Fontaine - Harmonisation",
+        "ID": "Fontaine: Penyelarasan",
+        "IT": "Fontaine: Armonizzazione",
+        "JP": "\u30d5\u30a9\u30f3\u30c6\u30fc\u30cc\u00b7\u8abf\u5f8b",
+        "KR": "\ud3f0\ud0c0\uc778\u00b7\uc870\uc728",
+        "PT": "Fontaine: Sintonia",
+        "RU": "\u041d\u0430\u0441\u0442\u0440\u043e\u0439\u043a\u0430 \u0438\u043d\u0441\u0442\u0440\u0443\u043c\u0435\u043d\u0442\u0430",
+        "TH": "Fontaine - \u0e1b\u0e23\u0e31\u0e1a\u0e08\u0e39\u0e19",
+        "TR": "Fontaine: Uyumluluk",
+        "VI": "Fontaine - Ch\u1ec9nh \u00c2m"
+    },
     "3868762092": {
         "CHS": "\u83ab\u5a1c\u00b7\u5929\u661f",
         "DE": "Mona \u2013 Einst\u00fcrzender Himmel",
         "EN": "Mona: Starry Sky",
         "ES": "Mona - Cielo estrellado",
         "FR": "Mona - Astromancie",
         "ID": "Mona: Starry Sky",
@@ -2907,14 +2971,30 @@
         "KR": "\uc694\uc774\ubbf8\uc57c\u00b7\uc720\uae08\ubd88\uaf43",
         "PT": "Yoimiya: Fa\u00edsca de Auratus",
         "RU": "\u0418\u0441\u043a\u0440\u044b \u0437\u043e\u043b\u043e\u0442\u043e\u0439 \u0440\u044b\u0431\u043a\u0438",
         "TH": "Yoimiya - \u0e1b\u0e23\u0e30\u0e01\u0e32\u0e22\u0e40\u0e1e\u0e25\u0e34\u0e07\u0e40\u0e23\u0e34\u0e07\u0e23\u0e30\u0e1a\u0e33",
         "TR": "Yoimiya: Alt\u0131n K\u0131v\u0131lc\u0131m",
         "VI": "Yoimiya - Hoa L\u1eeda Kim L\u01b0u"
     },
+    "89079668": {
+        "CHS": "\u963f\u857e\u5947\u8bfa\u00b7\u6cd5\u5ea6",
+        "DE": "Arlecchino \u2013 Edikt",
+        "EN": "Arlecchino: Edict",
+        "ES": "Arlecchino - Ley",
+        "FR": "Arlecchino - \u00c9dit",
+        "ID": "Arlecchino: Edict",
+        "IT": "Arlecchino: Editto",
+        "JP": "\u30a2\u30eb\u30ec\u30c3\u30ad\u30fc\u30ce\u00b7\u898f\u5247",
+        "KR": "\uc544\ub97c\ub808\ud0a4\ub178\u00b7\uaddc\uce59",
+        "PT": "Arlecchino: \u00c9dito",
+        "RU": "\u041f\u0440\u0430\u0432\u0438\u043b\u0430",
+        "TH": "Arlecchino - \u0e01\u0e0e\u0e40\u0e01\u0e13\u0e11\u0e4c",
+        "TR": "Arlecchino: Ferman",
+        "VI": "Arlecchino - S\u1eafc L\u1ec7nh"
+    },
     "893197700": {
         "CHS": "\u7eaa\u884c\u00b7\u610f\u5de7",
         "DE": "Erlebnispass \u2013 Zuneigung",
         "EN": "Travel Notes: Artful Intent",
         "ES": "PB - Pretensi\u00f3n artesanal",
         "FR": "PB - D\u00e9brouillardise",
         "ID": "Catatan Perjalanan: Tekad Pengrajin",
```

### Comparing `enkanetworkv2.py-2.0.4/enkanetwork/assets/langs/skills.json` & `enkanetworkv2.py-2.0.5/enkanetwork/assets/langs/skills.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9712918660287081%*

 * *Differences: {"'1185389325'": "OrderedDict([('CHS', '捕获！'), ('DE', 'Gefangen!'), ('EN', 'Capture!'), ('ES', "*

 * *                 '\'¡Captura!\'), (\'FR\', "Je t\'ai eu !"), (\'ID\', \'Capture!\'), (\'IT\', '*

 * *                 "'Cattura!'), ('JP', '捕獲！'), ('KR', '포획!'), ('PT', 'Capturar!'), ('RU', "*

 * *                 "'Попался!'), ('TH', 'Capture!'), ('TR', 'Yakala!'), ('VI', 'Bắt Lấy!')])",*

 * * "'1398698245'": "OrderedDict([('CHS', '元素战技替换技能'), ('DE', ''), ('EN', ''), ('ES', ''), ('FR', "*

 * *                 "''), ('ID', ''), ('I […]*

```diff
@@ -475,14 +475,30 @@
         "KR": "",
         "PT": "",
         "RU": "",
         "TH": "",
         "TR": "",
         "VI": ""
     },
+    "1185389325": {
+        "CHS": "\u6355\u83b7\uff01",
+        "DE": "Gefangen!",
+        "EN": "Capture!",
+        "ES": "\u00a1Captura!",
+        "FR": "Je t'ai eu !",
+        "ID": "Capture!",
+        "IT": "Cattura!",
+        "JP": "\u6355\u7372\uff01",
+        "KR": "\ud3ec\ud68d!",
+        "PT": "Capturar!",
+        "RU": "\u041f\u043e\u043f\u0430\u043b\u0441\u044f!",
+        "TH": "Capture!",
+        "TR": "Yakala!",
+        "VI": "B\u1eaft L\u1ea5y!"
+    },
     "1185804085": {
         "CHS": "4.0\u4eba\u95f4\u5927\u70ae-\u53d1\u5c04\u952e",
         "DE": "",
         "EN": "",
         "ES": "",
         "FR": "",
         "ID": "",
@@ -1019,14 +1035,30 @@
         "KR": "\uc77c\ubc18 \uacf5\uaca9\u00b7\ud604\uc6d4\uc758 \ucda4",
         "PT": "Ataque Normal: Dan\u00e7a da Meia-Lua",
         "RU": "\u0422\u0430\u043d\u0435\u0446 \u0448\u0430\u043c\u0448\u0438\u0440\u0430",
         "TH": "\u0e42\u0e08\u0e21\u0e15\u0e35\u0e1b\u0e01\u0e15\u0e34: Dance of Samser",
         "TR": "Normal Sald\u0131r\u0131: Samser Dans\u0131",
         "VI": "T\u1ea5n C\u00f4ng Th\u01b0\u1eddng - V\u0169 \u0110i\u1ec7u Samser"
     },
+    "1398698245": {
+        "CHS": "\u5143\u7d20\u6218\u6280\u66ff\u6362\u6280\u80fd",
+        "DE": "",
+        "EN": "",
+        "ES": "",
+        "FR": "",
+        "ID": "",
+        "IT": "",
+        "JP": "",
+        "KR": "",
+        "PT": "",
+        "RU": "",
+        "TH": "",
+        "TR": "",
+        "VI": ""
+    },
     "1422444957": {
         "CHS": "\u666e\u901a\u653b\u51fb\u00b7\u795e\u5c04\u624b",
         "DE": "Standardangriff: Scharfsch\u00fctze",
         "EN": "Normal Attack: Sharpshooter",
         "ES": "Ataque Normal: As de la arquer\u00eda",
         "FR": "Attaque normale : Archerie revisit\u00e9e",
         "ID": "Normal Attack: Sharpshooter",
@@ -1595,14 +1627,30 @@
         "KR": "",
         "PT": "",
         "RU": "",
         "TH": "",
         "TR": "",
         "VI": ""
     },
+    "164728021": {
+        "CHS": "\u4f2a\u88c5",
+        "DE": "Tarnung",
+        "EN": "Disguise",
+        "ES": "Camuflaje",
+        "FR": "Camouflage",
+        "ID": "Disguise",
+        "IT": "Camuffamento",
+        "JP": "\u507d\u88c5",
+        "KR": "\uc704\uc7a5",
+        "PT": "Disfarce",
+        "RU": "\u041c\u0430\u0441\u043a\u0438\u0440\u043e\u0432\u043a\u0430",
+        "TH": "Disguise",
+        "TR": "K\u0131l\u0131k De\u011fi\u015ftirme",
+        "VI": "Ng\u1ee5y Trang"
+    },
     "1656473773": {
         "CHS": "\u4f2a\u88c5",
         "DE": "Tarnung",
         "EN": "Disguise",
         "ES": "Camuflaje",
         "FR": "Camouflage",
         "ID": "Disguise",
@@ -1611,14 +1659,30 @@
         "KR": "\uc704\uc7a5",
         "PT": "Disfarce",
         "RU": "\u041c\u0430\u0441\u043a\u0438\u0440\u043e\u0432\u043a\u0430",
         "TH": "Disguise",
         "TR": "K\u0131l\u0131k De\u011fi\u015ftirme",
         "VI": "Ng\u1ee5y Trang"
     },
+    "1658286853": {
+        "CHS": "\u4f2a\u88c5",
+        "DE": "Tarnung",
+        "EN": "Disguise",
+        "ES": "Camuflaje",
+        "FR": "Camouflage",
+        "ID": "Disguise",
+        "IT": "Camuffamento",
+        "JP": "\u507d\u88c5",
+        "KR": "\uc704\uc7a5",
+        "PT": "Disfarce",
+        "RU": "\u041c\u0430\u0441\u043a\u0438\u0440\u043e\u0432\u043a\u0430",
+        "TH": "Disguise",
+        "TR": "K\u0131l\u0131k De\u011fi\u015ftirme",
+        "VI": "Ng\u1ee5y Trang"
+    },
     "1660121349": {
         "CHS": "\u666e\u901a\u653b\u51fb\u00b7\u5f02\u90a6\u60ca\u96f7",
         "DE": "Standardangriff: Gewitter aus der Fremde",
         "EN": "Normal Attack: Foreign Thundershock",
         "ES": "Ataque Normal: Rel\u00e1mpago extranjero",
         "FR": "Attaque normale : Tonnerre venu d'ailleurs",
         "ID": "Normal Attack: Foreign Thundershock",
@@ -2059,14 +2123,30 @@
         "KR": "\uc0b0\uacfc \uac15\uc758 \uae30\ub9b0 \ud754\uc801",
         "PT": "Rastros de Qilin",
         "RU": "\u0421\u043b\u0435\u0434 \u0446\u0438\u043b\u0438\u043d\u044f",
         "TH": "Trail of the Qilin",
         "TR": "Qilin'in \u0130zi",
         "VI": "S\u01a1n Tr\u1ea1ch L\u00e2n T\u00edch"
     },
+    "1819872509": {
+        "CHS": "\u6355\u5f71\u4fe1\u6807",
+        "DE": "Schattenf\u00e4ngerbake",
+        "EN": "Shadecatcher Beacon",
+        "ES": "Baliza atrapasombras",
+        "FR": "Balise photosensible",
+        "ID": "Shadecatcher Beacon",
+        "IT": "Faro acchiappaombre",
+        "JP": "\u6349\u5f71\u30d3\u30fc\u30b3\u30f3",
+        "KR": "\uadf8\ub9bc\uc790 \ud3ec\ucc29 \ube44\ucf58",
+        "PT": "Sinal de Captura",
+        "RU": "\u041c\u0430\u044f\u0447\u043e\u043a \u043f\u043e\u0438\u043c\u043a\u0438 \u0442\u0435\u043d\u0435\u0439",
+        "TH": "Shadecatcher Beacon",
+        "TR": "G\u00f6lge Kapan\u0131 \u0130\u015faret\u00e7isi",
+        "VI": "T\u00edn Hi\u1ec7u Ch\u1ee5p B\u00f3ng"
+    },
     "1821490277": {
         "CHS": "\u8bf1\u9975\u6218\u672f",
         "DE": "K\u00f6dertaktik",
         "EN": "Lay Bait",
         "ES": "Se\u00f1uelo",
         "FR": "Leurre",
         "ID": "Lay Bait",
@@ -2731,14 +2811,30 @@
         "KR": "\uc131\uc2e0 \ud68c\uadc0",
         "PT": "Restaura\u00e7\u00e3o Estelar",
         "RU": "\u0412\u043e\u0437\u0432\u0440\u0430\u0449\u0435\u043d\u0438\u0435 \u0437\u0432\u0435\u0437\u0434\u044b",
         "TH": "Stellar Restoration",
         "TR": "Y\u0131ld\u0131zlar\u0131n D\u00fczeni",
         "VI": "Tinh \u0110\u1ea9u Quy V\u1ecb"
     },
+    "2156811133": {
+        "CHS": "\u5384\u6708\u5c06\u5347",
+        "DE": "Aufgehen des Mondes des Verderbens",
+        "EN": "Balemoon Rising",
+        "ES": "Ascenso lunaciago",
+        "FR": "Ascension lunatique",
+        "ID": "Balemoon Rising",
+        "IT": "Ascesa della Luna cruenta",
+        "JP": "\u6607\u308a\u3086\u304f\u51f6\u6708",
+        "KR": "\ub5a0\uc624\ub974\ub294 \uc7ac\uc561\uc758 \ub2ec",
+        "PT": "Ascens\u00e3o da Lua Ominosa",
+        "RU": "\u0412\u043e\u0441\u0445\u043e\u0436\u0434\u0435\u043d\u0438\u0435 \u0440\u043e\u043a\u043e\u0432\u043e\u0439 \u043b\u0443\u043d\u044b",
+        "TH": "Balemoon Rising",
+        "TR": "U\u011fursuz Ay\u0131n Do\u011fu\u015fu",
+        "VI": "\u00c1ch Nguy\u1ec7t Tr\u1ed7i D\u1eady"
+    },
     "2160740245": {
         "CHS": "\u5723\u4eea\u00b7\u82cd\u9e6d\u5e87\u536b",
         "DE": "Heiliger Ritus \u2013 Heiligtum des Reihers",
         "EN": "Sacred Rite: Heron's Sanctum",
         "ES": "Rito sagrado: Garza guardiana",
         "FR": "Liturgie : Sanctuaire de la h\u00e9ronne",
         "ID": "Sacred Rite: Heron's Sanctum",
@@ -4155,14 +4251,30 @@
         "KR": "\uc77c\ubc18 \uacf5\uaca9\u00b7\uc194\uc9c1\ud55c \uac70\uc808",
         "PT": "Ataque Normal: Desist\u00eancia Franca",
         "RU": "\u041f\u0440\u044f\u043c\u043e\u0435 \u043d\u0435\u043f\u0440\u0438\u044f\u0442\u0438\u0435",
         "TH": "\u0e42\u0e08\u0e21\u0e15\u0e35\u0e1b\u0e01\u0e15\u0e34: Blunt Refusal",
         "TR": "Normal Sald\u0131r\u0131: A\u00e7\u0131k \u0130nkar",
         "VI": "T\u1ea5n C\u00f4ng Th\u01b0\u1eddng - T\u1eeb Ch\u1ed1i Th\u1eb3ng"
     },
+    "2699549653": {
+        "CHS": "\u963f\u857e\u5947\u8bfa\u7a7a\u4e2d\u653b\u51fb",
+        "DE": "",
+        "EN": "",
+        "ES": "",
+        "FR": "",
+        "ID": "",
+        "IT": "",
+        "JP": "",
+        "KR": "",
+        "PT": "",
+        "RU": "",
+        "TH": "",
+        "TR": "",
+        "VI": ""
+    },
     "2706644389": {
         "CHS": "\u8fea\u5e0c\u96c5\u5143\u7d20\u6218\u6280-\u4e8c\u6bb5\u6536\u5200",
         "DE": "",
         "EN": "",
         "ES": "",
         "FR": "",
         "ID": "",
@@ -4507,14 +4619,30 @@
         "KR": "",
         "PT": "",
         "RU": "",
         "TH": "",
         "TR": "",
         "VI": ""
     },
+    "2797265765": {
+        "CHS": "\u7981\u9522\u8bc5\u5492",
+        "DE": "Fluchtloser Fluch",
+        "EN": "Imprisoning Curse",
+        "ES": "Confinamiento",
+        "FR": "Confinement",
+        "ID": "Imprisoning Curse",
+        "IT": "Trappola maledetta",
+        "JP": "\u7981\u932e\u306e\u546a\u3044",
+        "KR": "\uac10\uae08\uc758 \uc800\uc8fc",
+        "PT": "Maldi\u00e7\u00e3o do Aprisionamento",
+        "RU": "\u041e\u043a\u043e\u0432\u044b",
+        "TH": "Imprisoning Curse",
+        "TR": "Hapseden Lanet",
+        "VI": "L\u1eddi Nguy\u1ec1n Giam C\u1ea7m"
+    },
     "2798026229": {
         "CHS": "\u4e94\u90ce\u7784\u51c6\u6a21\u5f0f",
         "DE": "",
         "EN": "",
         "ES": "",
         "FR": "",
         "ID": "",
@@ -6027,14 +6155,30 @@
         "KR": "\uc77c\ubc18 \uacf5\uaca9\u00b7\uac15\ucca0 \ub9c8\ub8e8",
         "PT": "Ataque Normal: Presa de A\u00e7o",
         "RU": "\u0421\u0442\u0430\u043b\u044c\u043d\u043e\u0439 \u043a\u043b\u044b\u043a",
         "TH": "\u0e42\u0e08\u0e21\u0e15\u0e35\u0e1b\u0e01\u0e15\u0e34: Steel Fang",
         "TR": "Normal Sald\u0131r\u0131: \u00c7elik Di\u015f",
         "VI": "T\u1ea5n C\u00f4ng Th\u01b0\u1eddng: Nanh Th\u00e9p"
     },
+    "3395884205": {
+        "CHS": "\u666e\u901a\u653b\u51fb\u00b7\u65a9\u9996\u4e4b\u9080",
+        "DE": "Standardangriff: Einladung zur Enthauptung",
+        "EN": "Normal Attack: Invitation to a Beheading",
+        "ES": "Ataque Normal: Invitaci\u00f3n a una decapitaci\u00f3n",
+        "FR": "Attaque normale : Invitation au supplice",
+        "ID": "Normal Attack: Invitation to a Beheading",
+        "IT": "Attacco normale: Invito alla decapitazione",
+        "JP": "\u901a\u5e38\u653b\u6483\u00b7\u65ac\u9996\u3078\u306e\u62db\u5f85\u72b6",
+        "KR": "\uc77c\ubc18 \uacf5\uaca9\u00b7\uc0ac\ud615\uc7a5\uc73c\ub85c\uc758 \ucd08\ub300",
+        "PT": "Ataque Normal: Convite para Decapita\u00e7\u00e3o",
+        "RU": "\u041f\u0440\u0438\u0433\u043b\u0430\u0448\u0435\u043d\u0438\u0435 \u043d\u0430 \u043a\u0430\u0437\u043d\u044c",
+        "TH": "\u0e42\u0e08\u0e21\u0e15\u0e35\u0e1b\u0e01\u0e15\u0e34: Invitation to a Beheading",
+        "TR": "Normal Sald\u0131r\u0131: \u0130nfaza \u00c7a\u011fr\u0131",
+        "VI": "T\u1ea5n C\u00f4ng Th\u01b0\u1eddng - L\u1eddi M\u1eddi Tr\u1ea3m Th\u1ee7"
+    },
     "3398003357": {
         "CHS": "\u5143\u7d20\u7206\u53d1",
         "DE": "",
         "EN": "",
         "ES": "",
         "FR": "",
         "ID": "",
@@ -6155,14 +6299,30 @@
         "KR": "",
         "PT": "",
         "RU": "",
         "TH": "",
         "TR": "",
         "VI": ""
     },
+    "3465751389": {
+        "CHS": "\u795e\u79d8\u9884\u611f",
+        "DE": "Mysteri\u00f6se Vorahnung",
+        "EN": "Mysterious Hunch",
+        "ES": "Sexto sentido",
+        "FR": "Sixi\u00e8me sens",
+        "ID": "Mysterious Hunch",
+        "IT": "Presagio misterioso",
+        "JP": "\u4e0d\u601d\u8b70\u306a\u4e88\u611f",
+        "KR": "\uc2e0\ube44\ud55c \uc608\uac10",
+        "PT": "Pressentimento Misterioso",
+        "RU": "\u0428\u0435\u0441\u0442\u043e\u0435 \u0447\u0443\u0432\u0441\u0442\u0432\u043e",
+        "TH": "Mysterious Hunch",
+        "TR": "Gizemli \u0130\u00e7g\u00fcd\u00fc",
+        "VI": "D\u1ef1 C\u1ea3m Th\u1ea7n B\u00ed"
+    },
     "3471617741": {
         "CHS": "Rx\u767d\u76d2\u6d4b\u8bd5\u666e\u653b",
         "DE": "",
         "EN": "",
         "ES": "",
         "FR": "",
         "ID": "",
@@ -6267,14 +6427,30 @@
         "KR": "\ub0e5\ub0e5 \uace8\ubaa9 \ub204\ube44\uae30",
         "PT": "Chute Miauteoro",
         "RU": "\u041c\u044f\u0443\u0442\u0435\u043e\u0440\u0438\u0442\u043d\u044b\u0439 \u0443\u0434\u0430\u0440",
         "TH": "Meow-teor Kick",
         "TR": "Miyav Jitsu",
         "VI": "M\u00e8o Tung C\u01b0\u1edbc"
     },
+    "351406893": {
+        "CHS": "\u6355\u83b7\uff01",
+        "DE": "Gefangen!",
+        "EN": "Capture!",
+        "ES": "\u00a1Captura!",
+        "FR": "Je t'ai eu !",
+        "ID": "Capture!",
+        "IT": "Cattura!",
+        "JP": "\u6355\u7372\uff01",
+        "KR": "\ud3ec\ud68d!",
+        "PT": "Capturar!",
+        "RU": "\u041f\u043e\u043f\u0430\u043b\u0441\u044f!",
+        "TH": "Capture!",
+        "TR": "Yakala!",
+        "VI": "B\u1eaft L\u1ea5y!"
+    },
     "3521320029": {
         "CHS": "\u51dd\u6d6a\u4e4b\u5149\u5251",
         "DE": "Schwert der Brandung",
         "EN": "Glacial Illumination",
         "ES": "Fulgor glacial",
         "FR": "Lame de fond",
         "ID": "Glacial Illumination",
@@ -6475,14 +6651,30 @@
         "KR": "",
         "PT": "",
         "RU": "",
         "TH": "",
         "TR": "",
         "VI": ""
     },
+    "3589496853": {
+        "CHS": "\u963f\u857e\u5947\u8bfa\u91cd\u51fb\u8fdc\u8ddd\u79bb\u7d22\u654c",
+        "DE": "",
+        "EN": "",
+        "ES": "",
+        "FR": "",
+        "ID": "",
+        "IT": "",
+        "JP": "",
+        "KR": "",
+        "PT": "",
+        "RU": "",
+        "TH": "",
+        "TR": "",
+        "VI": ""
+    },
     "3592193965": {
         "CHS": "\u6240\u95fb\u904d\u8ba1",
         "DE": "Kennerin aller Tricks",
         "EN": "All Schemes to Know",
         "ES": "Omnisciencia",
         "FR": "Omniscience des plans",
         "ID": "All Schemes to Know",
@@ -7835,14 +8027,30 @@
         "KR": "\uacf5\uc911 \ud22c\ud558",
         "PT": "",
         "RU": "",
         "TH": "",
         "TR": "",
         "VI": ""
     },
+    "4151065125": {
+        "CHS": "\u65e0\u5f62\u8ffd\u8ff9",
+        "DE": "Unbemerkte Verfolgung",
+        "EN": "Unseen Pursuit",
+        "ES": "Rastreo invisible",
+        "FR": "Trace invisible",
+        "ID": "Unseen Pursuit",
+        "IT": "Inseguitore invisibile",
+        "JP": "\u5f62\u306a\u304d\u8ffd\u8de1",
+        "KR": "\uc740\ubc00\ud55c \ucd94\uc801",
+        "PT": "Rastros Invis\u00edveis",
+        "RU": "\u041d\u0435\u0432\u0438\u0434\u0438\u043c\u0430\u044f \u043f\u043e\u0433\u043e\u043d\u044f",
+        "TH": "Unseen Pursuit",
+        "TR": "Gizli Takip",
+        "VI": "D\u1ea5u V\u1ebft V\u00f4 H\u00ecnh"
+    },
     "4155943733": {
         "CHS": "\u5361\u8428\u624e\u83b1\u5bab\u7684\u65e0\u5fae\u4e0d\u81f3",
         "DE": "Zuneigung von Alcazarzaray",
         "EN": "Alcazarzaray's Exactitude",
         "ES": "Meticulosidad de Alcazarzaray",
         "FR": "M\u00e9ticulosit\u00e9 d'Alcazarzaray",
         "ID": "Alcazarzaray's Exactitude",
@@ -8171,14 +8379,46 @@
         "KR": "\uc720\uae08 \uc6b4\uac04\ucd08",
         "PT": "Saxifraga Ryuukin",
         "RU": "\u041a\u0430\u043c\u043d\u0435\u043b\u043e\u043c\u043a\u0430 \u0420\u044e\u043a\u0438\u043d",
         "TH": "Ryuukin Saxifrage",
         "TR": "Ta\u015fk\u0131ran Ryuukin",
         "VI": "C\u1ecf Ryuukin"
     },
+    "4251923773": {
+        "CHS": "4.6\u97f3\u4e50\u673a\u5236\u6c34\u4e0b",
+        "DE": "",
+        "EN": "",
+        "ES": "",
+        "FR": "",
+        "ID": "",
+        "IT": "",
+        "JP": "",
+        "KR": "",
+        "PT": "",
+        "RU": "",
+        "TH": "",
+        "TR": "",
+        "VI": ""
+    },
+    "4257022253": {
+        "CHS": "\u963f\u857e\u5947\u8bfa\u62b5\u6b7b\u56de\u8840",
+        "DE": "",
+        "EN": "",
+        "ES": "",
+        "FR": "",
+        "ID": "",
+        "IT": "",
+        "JP": "",
+        "KR": "",
+        "PT": "",
+        "RU": "",
+        "TH": "",
+        "TR": "",
+        "VI": ""
+    },
     "4260508917": {
         "CHS": "\u753b\u5219\u5de7\u65bd",
         "DE": "K\u00fcnstlerische Genialit\u00e4t",
         "EN": "Artistic Ingenuity",
         "ES": "Genio de la arquitectura",
         "FR": "Ing\u00e9niosit\u00e9 artistique",
         "ID": "Artistic Ingenuity",
@@ -9435,14 +9675,46 @@
         "KR": "\ud48d\ub9c8\ud3ec",
         "PT": "",
         "RU": "",
         "TH": "",
         "TR": "",
         "VI": ""
     },
+    "840915861": {
+        "CHS": "4.6\u9cb8\u9c7c\u94a9\u722a\u9000\u51fa",
+        "DE": "",
+        "EN": "",
+        "ES": "",
+        "FR": "",
+        "ID": "",
+        "IT": "",
+        "JP": "",
+        "KR": "",
+        "PT": "",
+        "RU": "",
+        "TH": "",
+        "TR": "",
+        "VI": ""
+    },
+    "845866237": {
+        "CHS": "4.6\u97f3\u4e50\u673a\u5236",
+        "DE": "",
+        "EN": "",
+        "ES": "",
+        "FR": "",
+        "ID": "",
+        "IT": "",
+        "JP": "",
+        "KR": "",
+        "PT": "",
+        "RU": "",
+        "TH": "",
+        "TR": "",
+        "VI": ""
+    },
     "856237685": {
         "CHS": "\u795e\u91cc\u6d41\u00b7\u955c\u82b1",
         "DE": "Kamisato-Stil \u2013 Kyouka",
         "EN": "Kamisato Art: Kyouka",
         "ES": "Estilo Kamisato: Belleza reflejada",
         "FR": "\u00c9cole Kamisato : Beaut\u00e9 r\u00e9fl\u00e9chie",
         "ID": "Kamisato Art: Kyouka",
@@ -9483,14 +9755,30 @@
         "KR": "\uc720\ud6c4\ub958\u00b7\ud48d\uc740 \ub3cc\uc9c4",
         "PT": "Arte Yoohoo: Ataque Fuuin",
         "RU": "\u0418\u0441\u043a\u0443\u0441\u0441\u0442\u0432\u043e \u042e\u0445\u0443: \u0420\u044b\u0432\u043e\u043a \u0424\u0443\u0438\u043d",
         "TH": "Yoohoo Art: Fuuin Dash",
         "TR": "Yoohoo Sanat\u0131: Fuuin Ko\u015fusu",
         "VI": "Tr\u01b0\u1eddng Ph\u00e1i Yoohoo - Fuuin L\u0103n Tr\u00f2n"
     },
+    "88213301": {
+        "CHS": "\u4e07\u76f8\u5316\u7070",
+        "DE": "Alles wird zu Staub",
+        "EN": "All Is Ash",
+        "ES": "Que todo sea cenizas",
+        "FR": "Pulv\u00e9risation totale",
+        "ID": "All is Ash",
+        "IT": "Cenere alla cenere",
+        "JP": "\u4e07\u8c61\u3001\u7070\u306b\u5e30\u3059",
+        "KR": "\uc7ac\uac00 \ub41c \ub9cc\uc0c1",
+        "PT": "Tudo s\u00e3o Cinzas",
+        "RU": "\u0412\u0441\u0451 \u043f\u0440\u0435\u0432\u0440\u0430\u0449\u0430\u0435\u0442\u0441\u044f \u0432 \u043f\u0440\u0430\u0445",
+        "TH": "All Is Ash",
+        "TR": "Hepsi K\u00fcl Oldu",
+        "VI": "V\u1ea1n V\u1eadt H\u00f3a Tro"
+    },
     "886703661": {
         "CHS": "\u7c73\u5361\u7a7a\u4e2d\u653b\u51fb",
         "DE": "",
         "EN": "",
         "ES": "",
         "FR": "",
         "ID": "",
```

### Comparing `enkanetworkv2.py-2.0.4/enkanetwork/assets/langs/weapons.json` & `enkanetworkv2.py-2.0.5/enkanetwork/assets/langs/weapons.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9953051643192489%*

 * *Differences: {"'2944936683'": "OrderedDict([('CHS', '赤月之形'), ('DE', 'Form des scharlachroten Mondes'), ('EN', "*

 * *                 '"Crimson Moon\'s Semblance"), (\'ES\', \'Semblante de la Luna Carmesí\'), '*

 * *                 '(\'FR\', \'Semblance de la lune écarlate\'), (\'ID\', "Crimson Moon\'s '*

 * *                 'Semblance"), (\'IT\', \'Forma della Luna cremisi\'), (\'JP\', \'赤月のシルエット\'), '*

 * *                 "('KR', '붉은 달의 형상'), ('PT', 'Semblante da Lua Carmesim'), ('RU', 'Очертания алой "*

 * *                 'луны\'), (\'T […]*

```diff
@@ -1531,14 +1531,30 @@
         "KR": "\uc655\uc2e4\uc758 \uc7a5\ucc3d",
         "PT": "Lan\u00e7a de Ca\u00e7a Real",
         "RU": "\u041a\u043e\u0440\u043e\u043b\u0435\u0432\u0441\u043a\u043e\u0435 \u043a\u043e\u043f\u044c\u0451",
         "TH": "Royal Spear",
         "TR": "Kraliyet M\u0131zra\u011f\u0131",
         "VI": "Th\u01b0\u01a1ng S\u0103n T\u00f4ng Th\u1ea5t"
     },
+    "2944936683": {
+        "CHS": "\u8d64\u6708\u4e4b\u5f62",
+        "DE": "Form des scharlachroten Mondes",
+        "EN": "Crimson Moon's Semblance",
+        "ES": "Semblante de la Luna Carmes\u00ed",
+        "FR": "Semblance de la lune \u00e9carlate",
+        "ID": "Crimson Moon's Semblance",
+        "IT": "Forma della Luna cremisi",
+        "JP": "\u8d64\u6708\u306e\u30b7\u30eb\u30a8\u30c3\u30c8",
+        "KR": "\ubd89\uc740 \ub2ec\uc758 \ud615\uc0c1",
+        "PT": "Semblante da Lua Carmesim",
+        "RU": "\u041e\u0447\u0435\u0440\u0442\u0430\u043d\u0438\u044f \u0430\u043b\u043e\u0439 \u043b\u0443\u043d\u044b",
+        "TH": "Crimson Moon's Semblance",
+        "TR": "K\u0131z\u0131l Ay\u0131n Sureti",
+        "VI": "H\u00ecnh Th\u00e1i X\u00edch Nguy\u1ec7t"
+    },
     "2947140987": {
         "CHS": "\u6697\u5df7\u95ea\u5149",
         "DE": "Gassenleuchte",
         "EN": "The Alley Flash",
         "ES": "Destello en la Oscuridad",
         "FR": "\u00c9clair des impasses",
         "ID": "The Alley Flash",
```

### Comparing `enkanetworkv2.py-2.0.4/enkanetwork/assets.py` & `enkanetworkv2.py-2.0.5/enkanetwork/assets.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.4/enkanetwork/cache.py` & `enkanetworkv2.py-2.0.5/enkanetwork/cache.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.4/enkanetwork/client.py` & `enkanetworkv2.py-2.0.5/enkanetwork/client.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.4/enkanetwork/config.py` & `enkanetworkv2.py-2.0.5/enkanetwork/config.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.4/enkanetwork/enum.py` & `enkanetworkv2.py-2.0.5/enkanetwork/enum.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.4/enkanetwork/exception.py` & `enkanetworkv2.py-2.0.5/enkanetwork/exception.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.4/enkanetwork/http.py` & `enkanetworkv2.py-2.0.5/enkanetwork/http.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.4/enkanetwork/model/assets.py` & `enkanetworkv2.py-2.0.5/enkanetwork/model/assets.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.4/enkanetwork/model/base.py` & `enkanetworkv2.py-2.0.5/enkanetwork/model/base.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.4/enkanetwork/model/build.py` & `enkanetworkv2.py-2.0.5/enkanetwork/model/build.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.4/enkanetwork/model/character.py` & `enkanetworkv2.py-2.0.5/enkanetwork/model/character.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.4/enkanetwork/model/equipments.py` & `enkanetworkv2.py-2.0.5/enkanetwork/model/equipments.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.4/enkanetwork/model/players.py` & `enkanetworkv2.py-2.0.5/enkanetwork/model/players.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.4/enkanetwork/model/stats.py` & `enkanetworkv2.py-2.0.5/enkanetwork/model/stats.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.4/enkanetwork/tools.py` & `enkanetworkv2.py-2.0.5/enkanetwork/tools.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.4/enkanetwork/types/enkanetwork.py` & `enkanetworkv2.py-2.0.5/enkanetwork/types/enkanetwork.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.4/enkanetwork/utils.py` & `enkanetworkv2.py-2.0.5/enkanetwork/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,13 +125,13 @@
     }
     return content
 
 
 async def update_pfps(path):
     async with aiohttp.ClientSession() as session:
         async with session.get("https://raw.githubusercontent.com/EnkaNetwork/API-docs/master/store/pfps.json") as response:
-            data = response.read()
+            data = await response.read()
             
     data = json.loads(data)
     
     with open(os.path.join(path, "pfps.json"), 'w',  encoding='utf-8') as file:
         json.dump(data, file, indent=4)
```

### Comparing `enkanetworkv2.py-2.0.4/enkanetworkv2.py.egg-info/PKG-INFO` & `enkanetworkv2.py-2.0.5/enkanetworkv2.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enkanetworkv2.py
-Version: 2.0.4
+Version: 2.0.5
 Summary: Library for fetching JSON data from site https://enka.network/
 Home-page: https://github.com/DEViantUA/EnkaNetworkV2.py
 Author: DeviantUa
 Author-email: deviantapi@gmail.com
 Keywords: enkanetwork.py,enkanetwork,enka.network,genshinapi,enkanetworkV2,enkanetworkV2.py
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `enkanetworkv2.py-2.0.4/enkanetworkv2.py.egg-info/SOURCES.txt` & `enkanetworkv2.py-2.0.5/enkanetworkv2.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.4/setup.py` & `enkanetworkv2.py-2.0.5/setup.py`

 * *Files identical despite different names*

