# Comparing `tmp/enkanetworkv2.py-2.0.5.tar.gz` & `tmp/enkanetworkv2.py-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enkanetworkv2.py-2.0.5.tar", last modified: Thu Apr 25 10:00:21 2024, max compression
+gzip compressed data, was "enkanetworkv2.py-2.0.6.tar", last modified: Thu Apr 25 10:07:30 2024, max compression
```

## Comparing `enkanetworkv2.py-2.0.5.tar` & `enkanetworkv2.py-2.0.6.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 10:00:21.918044 enkanetworkv2.py-2.0.5/
--rw-rw-rw-   0        0        0     1070 2024-02-24 18:53:52.000000 enkanetworkv2.py-2.0.5/LICENSE
--rw-rw-rw-   0        0        0       36 2024-02-24 18:58:13.000000 enkanetworkv2.py-2.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0    19341 2024-04-25 10:00:21.918044 enkanetworkv2.py-2.0.5/PKG-INFO
--rw-rw-rw-   0        0        0    18242 2024-02-24 19:02:02.000000 enkanetworkv2.py-2.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 10:00:21.874043 enkanetworkv2.py-2.0.5/enkanetwork/
--rw-rw-rw-   0        0        0     1462 2024-04-25 09:57:55.000000 enkanetworkv2.py-2.0.5/enkanetwork/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 10:00:21.857995 enkanetworkv2.py-2.0.5/enkanetwork/assets/
-drwxrwxrwx   0        0        0        0 2024-04-25 10:00:21.882044 enkanetworkv2.py-2.0.5/enkanetwork/assets/data/
--rw-rw-rw-   0        0        0    54223 2024-04-25 09:53:04.000000 enkanetworkv2.py-2.0.5/enkanetwork/assets/data/artifact_props.json
--rw-rw-rw-   0        0        0  1095132 2024-04-25 09:53:03.000000 enkanetworkv2.py-2.0.5/enkanetwork/assets/data/artifacts.json
--rw-rw-rw-   0        0        0    43649 2024-04-25 09:53:04.000000 enkanetworkv2.py-2.0.5/enkanetwork/assets/data/characters.json
--rw-rw-rw-   0        0        0    52516 2024-04-25 09:53:04.000000 enkanetworkv2.py-2.0.5/enkanetwork/assets/data/constellations.json
--rw-rw-rw-   0        0        0    12831 2024-04-25 09:53:03.000000 enkanetworkv2.py-2.0.5/enkanetwork/assets/data/costumes.json
--rw-rw-rw-   0        0        0  1316924 2024-04-25 09:53:04.000000 enkanetworkv2.py-2.0.5/enkanetwork/assets/data/fight_props.json
--rw-rw-rw-   0        0        0    57396 2024-04-25 09:53:02.000000 enkanetworkv2.py-2.0.5/enkanetwork/assets/data/namecards.json
--rw-rw-rw-   0        0        0     6321 2024-04-06 16:43:28.000000 enkanetworkv2.py-2.0.5/enkanetwork/assets/data/pfps.json
--rw-rw-rw-   0        0        0    87635 2024-04-25 09:53:04.000000 enkanetworkv2.py-2.0.5/enkanetwork/assets/data/skills.json
--rw-rw-rw-   0        0        0    41728 2024-04-25 09:53:02.000000 enkanetworkv2.py-2.0.5/enkanetwork/assets/data/weapons.json
-drwxrwxrwx   0        0        0        0 2024-04-25 10:00:21.891044 enkanetworkv2.py-2.0.5/enkanetwork/assets/langs/
--rw-rw-rw-   0        0        0   554994 2024-04-25 09:54:12.000000 enkanetworkv2.py-2.0.5/enkanetwork/assets/langs/artifact_sets.json
--rw-rw-rw-   0        0        0  2431947 2024-04-25 09:54:14.000000 enkanetworkv2.py-2.0.5/enkanetwork/assets/langs/artifacts.json
--rw-rw-rw-   0        0        0    33337 2024-04-25 09:54:14.000000 enkanetworkv2.py-2.0.5/enkanetwork/assets/langs/characters.json
--rw-rw-rw-   0        0        0   310851 2024-04-25 09:54:14.000000 enkanetworkv2.py-2.0.5/enkanetwork/assets/langs/constellations.json
--rw-rw-rw-   0        0        0    30562 2024-02-24 19:12:22.000000 enkanetworkv2.py-2.0.5/enkanetwork/assets/langs/fight_props.json
--rw-rw-rw-   0        0        0   122404 2024-04-25 09:54:14.000000 enkanetworkv2.py-2.0.5/enkanetwork/assets/langs/namecards.json
--rw-rw-rw-   0        0        0   309249 2024-04-25 09:54:15.000000 enkanetworkv2.py-2.0.5/enkanetwork/assets/langs/skills.json
--rw-rw-rw-   0        0        0   113312 2024-04-25 09:54:15.000000 enkanetworkv2.py-2.0.5/enkanetwork/assets/langs/weapons.json
--rw-rw-rw-   0        0        0     8270 2024-04-06 17:04:36.000000 enkanetworkv2.py-2.0.5/enkanetwork/assets.py
--rw-rw-rw-   0        0        0      645 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.5/enkanetwork/cache.py
--rw-rw-rw-   0        0        0    12474 2024-04-07 20:58:35.000000 enkanetworkv2.py-2.0.5/enkanetwork/client.py
--rw-rw-rw-   0        0        0      798 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.5/enkanetwork/config.py
--rw-rw-rw-   0        0        0     1099 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.5/enkanetwork/enum.py
--rw-rw-rw-   0        0        0     1925 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.5/enkanetwork/exception.py
--rw-rw-rw-   0        0        0     7345 2024-02-24 18:56:30.000000 enkanetworkv2.py-2.0.5/enkanetwork/http.py
-drwxrwxrwx   0        0        0        0 2024-04-25 10:00:21.898044 enkanetworkv2.py-2.0.5/enkanetwork/model/
--rw-rw-rw-   0        0        0      137 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.5/enkanetwork/model/__init__.py
--rw-rw-rw-   0        0        0     5029 2024-04-06 17:00:40.000000 enkanetworkv2.py-2.0.5/enkanetwork/model/assets.py
--rw-rw-rw-   0        0        0     1935 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.5/enkanetwork/model/base.py
--rw-rw-rw-   0        0        0     1403 2024-02-24 18:46:53.000000 enkanetworkv2.py-2.0.5/enkanetwork/model/build.py
--rw-rw-rw-   0        0        0     5183 2024-02-24 18:47:25.000000 enkanetworkv2.py-2.0.5/enkanetwork/model/character.py
--rw-rw-rw-   0        0        0     5634 2024-02-24 18:35:48.000000 enkanetworkv2.py-2.0.5/enkanetwork/model/equipments.py
--rw-rw-rw-   0        0        0      307 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.5/enkanetwork/model/hoyos.py
--rw-rw-rw-   0        0        0     4063 2024-04-06 17:07:07.000000 enkanetworkv2.py-2.0.5/enkanetwork/model/players.py
--rw-rw-rw-   0        0        0      346 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.5/enkanetwork/model/profile.py
--rw-rw-rw-   0        0        0     7763 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.5/enkanetwork/model/stats.py
--rw-rw-rw-   0        0        0      293 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.5/enkanetwork/model/utils.py
--rw-rw-rw-   0        0        0     1313 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.5/enkanetwork/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-25 10:00:21.899044 enkanetworkv2.py-2.0.5/enkanetwork/types/
--rw-rw-rw-   0        0        0      157 2024-02-24 18:56:57.000000 enkanetworkv2.py-2.0.5/enkanetwork/types/__init__.py
--rw-rw-rw-   0        0        0     1157 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.5/enkanetwork/types/enkanetwork.py
--rw-rw-rw-   0        0        0     3445 2024-04-25 09:57:20.000000 enkanetworkv2.py-2.0.5/enkanetwork/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-25 10:00:21.917045 enkanetworkv2.py-2.0.5/enkanetworkv2.py.egg-info/
--rw-rw-rw-   0        0        0    19341 2024-04-25 10:00:21.000000 enkanetworkv2.py-2.0.5/enkanetworkv2.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1550 2024-04-25 10:00:21.000000 enkanetworkv2.py-2.0.5/enkanetworkv2.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 10:00:21.000000 enkanetworkv2.py-2.0.5/enkanetworkv2.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-04-25 10:00:21.000000 enkanetworkv2.py-2.0.5/enkanetworkv2.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-25 10:00:21.000000 enkanetworkv2.py-2.0.5/enkanetworkv2.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 10:00:21.919043 enkanetworkv2.py-2.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1105 2024-04-06 17:09:00.000000 enkanetworkv2.py-2.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 10:07:30.467036 enkanetworkv2.py-2.0.6/
+-rw-rw-rw-   0        0        0     1070 2024-02-24 18:53:52.000000 enkanetworkv2.py-2.0.6/LICENSE
+-rw-rw-rw-   0        0        0       36 2024-02-24 18:58:13.000000 enkanetworkv2.py-2.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0    19341 2024-04-25 10:07:30.467036 enkanetworkv2.py-2.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0    18242 2024-02-24 19:02:02.000000 enkanetworkv2.py-2.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 10:07:30.420036 enkanetworkv2.py-2.0.6/enkanetwork/
+-rw-rw-rw-   0        0        0     1462 2024-04-25 10:06:56.000000 enkanetworkv2.py-2.0.6/enkanetwork/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 10:07:30.409038 enkanetworkv2.py-2.0.6/enkanetwork/assets/
+drwxrwxrwx   0        0        0        0 2024-04-25 10:07:30.429037 enkanetworkv2.py-2.0.6/enkanetwork/assets/data/
+-rw-rw-rw-   0        0        0    54223 2024-04-25 09:53:04.000000 enkanetworkv2.py-2.0.6/enkanetwork/assets/data/artifact_props.json
+-rw-rw-rw-   0        0        0  1095132 2024-04-25 09:53:03.000000 enkanetworkv2.py-2.0.6/enkanetwork/assets/data/artifacts.json
+-rw-rw-rw-   0        0        0    43649 2024-04-25 09:53:04.000000 enkanetworkv2.py-2.0.6/enkanetwork/assets/data/characters.json
+-rw-rw-rw-   0        0        0    52516 2024-04-25 09:53:04.000000 enkanetworkv2.py-2.0.6/enkanetwork/assets/data/constellations.json
+-rw-rw-rw-   0        0        0    12831 2024-04-25 09:53:03.000000 enkanetworkv2.py-2.0.6/enkanetwork/assets/data/costumes.json
+-rw-rw-rw-   0        0        0  1316924 2024-04-25 09:53:04.000000 enkanetworkv2.py-2.0.6/enkanetwork/assets/data/fight_props.json
+-rw-rw-rw-   0        0        0    57396 2024-04-25 09:53:02.000000 enkanetworkv2.py-2.0.6/enkanetwork/assets/data/namecards.json
+-rw-rw-rw-   0        0        0     6321 2024-04-06 16:43:28.000000 enkanetworkv2.py-2.0.6/enkanetwork/assets/data/pfps.json
+-rw-rw-rw-   0        0        0    87635 2024-04-25 09:53:04.000000 enkanetworkv2.py-2.0.6/enkanetwork/assets/data/skills.json
+-rw-rw-rw-   0        0        0    41728 2024-04-25 09:53:02.000000 enkanetworkv2.py-2.0.6/enkanetwork/assets/data/weapons.json
+drwxrwxrwx   0        0        0        0 2024-04-25 10:07:30.438036 enkanetworkv2.py-2.0.6/enkanetwork/assets/langs/
+-rw-rw-rw-   0        0        0   554994 2024-04-25 09:54:12.000000 enkanetworkv2.py-2.0.6/enkanetwork/assets/langs/artifact_sets.json
+-rw-rw-rw-   0        0        0  2431947 2024-04-25 09:54:14.000000 enkanetworkv2.py-2.0.6/enkanetwork/assets/langs/artifacts.json
+-rw-rw-rw-   0        0        0    33337 2024-04-25 09:54:14.000000 enkanetworkv2.py-2.0.6/enkanetwork/assets/langs/characters.json
+-rw-rw-rw-   0        0        0   310851 2024-04-25 09:54:14.000000 enkanetworkv2.py-2.0.6/enkanetwork/assets/langs/constellations.json
+-rw-rw-rw-   0        0        0    30562 2024-02-24 19:12:22.000000 enkanetworkv2.py-2.0.6/enkanetwork/assets/langs/fight_props.json
+-rw-rw-rw-   0        0        0   122404 2024-04-25 09:54:14.000000 enkanetworkv2.py-2.0.6/enkanetwork/assets/langs/namecards.json
+-rw-rw-rw-   0        0        0   309249 2024-04-25 09:54:15.000000 enkanetworkv2.py-2.0.6/enkanetwork/assets/langs/skills.json
+-rw-rw-rw-   0        0        0   113312 2024-04-25 09:54:15.000000 enkanetworkv2.py-2.0.6/enkanetwork/assets/langs/weapons.json
+-rw-rw-rw-   0        0        0     8270 2024-04-06 17:04:36.000000 enkanetworkv2.py-2.0.6/enkanetwork/assets.py
+-rw-rw-rw-   0        0        0      645 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.6/enkanetwork/cache.py
+-rw-rw-rw-   0        0        0    12474 2024-04-07 20:58:35.000000 enkanetworkv2.py-2.0.6/enkanetwork/client.py
+-rw-rw-rw-   0        0        0      798 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.6/enkanetwork/config.py
+-rw-rw-rw-   0        0        0     1099 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.6/enkanetwork/enum.py
+-rw-rw-rw-   0        0        0     1925 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.6/enkanetwork/exception.py
+-rw-rw-rw-   0        0        0     7345 2024-02-24 18:56:30.000000 enkanetworkv2.py-2.0.6/enkanetwork/http.py
+drwxrwxrwx   0        0        0        0 2024-04-25 10:07:30.446036 enkanetworkv2.py-2.0.6/enkanetwork/model/
+-rw-rw-rw-   0        0        0      137 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.6/enkanetwork/model/__init__.py
+-rw-rw-rw-   0        0        0     5029 2024-04-06 17:00:40.000000 enkanetworkv2.py-2.0.6/enkanetwork/model/assets.py
+-rw-rw-rw-   0        0        0     1935 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.6/enkanetwork/model/base.py
+-rw-rw-rw-   0        0        0     1403 2024-02-24 18:46:53.000000 enkanetworkv2.py-2.0.6/enkanetwork/model/build.py
+-rw-rw-rw-   0        0        0     5183 2024-02-24 18:47:25.000000 enkanetworkv2.py-2.0.6/enkanetwork/model/character.py
+-rw-rw-rw-   0        0        0     5634 2024-02-24 18:35:48.000000 enkanetworkv2.py-2.0.6/enkanetwork/model/equipments.py
+-rw-rw-rw-   0        0        0      307 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.6/enkanetwork/model/hoyos.py
+-rw-rw-rw-   0        0        0     4063 2024-04-06 17:07:07.000000 enkanetworkv2.py-2.0.6/enkanetwork/model/players.py
+-rw-rw-rw-   0        0        0      346 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.6/enkanetwork/model/profile.py
+-rw-rw-rw-   0        0        0     7763 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.6/enkanetwork/model/stats.py
+-rw-rw-rw-   0        0        0      293 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.6/enkanetwork/model/utils.py
+-rw-rw-rw-   0        0        0     1313 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.6/enkanetwork/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-25 10:07:30.448036 enkanetworkv2.py-2.0.6/enkanetwork/types/
+-rw-rw-rw-   0        0        0      157 2024-02-24 18:56:57.000000 enkanetworkv2.py-2.0.6/enkanetwork/types/__init__.py
+-rw-rw-rw-   0        0        0     1157 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.6/enkanetwork/types/enkanetwork.py
+-rw-rw-rw-   0        0        0     3445 2024-04-25 09:57:20.000000 enkanetworkv2.py-2.0.6/enkanetwork/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-25 10:07:30.466037 enkanetworkv2.py-2.0.6/enkanetworkv2.py.egg-info/
+-rw-rw-rw-   0        0        0    19341 2024-04-25 10:07:30.000000 enkanetworkv2.py-2.0.6/enkanetworkv2.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1550 2024-04-25 10:07:30.000000 enkanetworkv2.py-2.0.6/enkanetworkv2.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 10:07:30.000000 enkanetworkv2.py-2.0.6/enkanetworkv2.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-04-25 10:07:30.000000 enkanetworkv2.py-2.0.6/enkanetworkv2.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-25 10:07:30.000000 enkanetworkv2.py-2.0.6/enkanetworkv2.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 10:07:30.467036 enkanetworkv2.py-2.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1105 2024-04-06 17:09:00.000000 enkanetworkv2.py-2.0.6/setup.py
```

### Comparing `enkanetworkv2.py-2.0.5/LICENSE` & `enkanetworkv2.py-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.5/PKG-INFO` & `enkanetworkv2.py-2.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enkanetworkv2.py
-Version: 2.0.5
+Version: 2.0.6
 Summary: Library for fetching JSON data from site https://enka.network/
 Home-page: https://github.com/DEViantUA/EnkaNetworkV2.py
 Author: DeviantUa
 Author-email: deviantapi@gmail.com
 Keywords: enkanetwork.py,enkanetwork,enka.network,genshinapi,enkanetworkV2,enkanetworkV2.py
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `enkanetworkv2.py-2.0.5/README.md` & `enkanetworkv2.py-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.5/enkanetwork/__init__.py` & `enkanetworkv2.py-2.0.6/enkanetwork/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE."""
 
 __title__ = 'enkanetworkV2.py'
 __author__ = 'DeviantUa'
-__version__ = '2.0.5'
+__version__ = '2.0.6'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2024-present DeviantUa'
 
 
 from .client import *
 from .exception import *
 from .model import *
```

### Comparing `enkanetworkv2.py-2.0.5/enkanetwork/assets/data/artifact_props.json` & `enkanetworkv2.py-2.0.6/enkanetwork/assets/data/artifact_props.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.5/enkanetwork/assets/data/artifacts.json` & `enkanetworkv2.py-2.0.6/enkanetwork/assets/data/artifacts.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.5/enkanetwork/assets/data/characters.json` & `enkanetworkv2.py-2.0.6/enkanetwork/assets/data/characters.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.5/enkanetwork/assets/data/constellations.json` & `enkanetworkv2.py-2.0.6/enkanetwork/assets/data/constellations.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.5/enkanetwork/assets/data/costumes.json` & `enkanetworkv2.py-2.0.6/enkanetwork/assets/data/costumes.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.5/enkanetwork/assets/data/fight_props.json` & `enkanetworkv2.py-2.0.6/enkanetwork/assets/data/fight_props.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.5/enkanetwork/assets/data/namecards.json` & `enkanetworkv2.py-2.0.6/enkanetwork/assets/data/namecards.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.5/enkanetwork/assets/data/pfps.json` & `enkanetworkv2.py-2.0.6/enkanetwork/assets/data/pfps.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.5/enkanetwork/assets/data/skills.json` & `enkanetworkv2.py-2.0.6/enkanetwork/assets/data/skills.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.5/enkanetwork/assets/data/weapons.json` & `enkanetworkv2.py-2.0.6/enkanetwork/assets/data/weapons.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.5/enkanetwork/assets/langs/artifact_sets.json` & `enkanetworkv2.py-2.0.6/enkanetwork/assets/langs/artifact_sets.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.5/enkanetwork/assets/langs/artifacts.json` & `enkanetworkv2.py-2.0.6/enkanetwork/assets/langs/artifacts.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.5/enkanetwork/assets/langs/characters.json` & `enkanetworkv2.py-2.0.6/enkanetwork/assets/langs/characters.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.5/enkanetwork/assets/langs/constellations.json` & `enkanetworkv2.py-2.0.6/enkanetwork/assets/langs/constellations.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.5/enkanetwork/assets/langs/fight_props.json` & `enkanetworkv2.py-2.0.6/enkanetwork/assets/langs/fight_props.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.5/enkanetwork/assets/langs/namecards.json` & `enkanetworkv2.py-2.0.6/enkanetwork/assets/langs/namecards.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.5/enkanetwork/assets/langs/skills.json` & `enkanetworkv2.py-2.0.6/enkanetwork/assets/langs/skills.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.5/enkanetwork/assets/langs/weapons.json` & `enkanetworkv2.py-2.0.6/enkanetwork/assets/langs/weapons.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.5/enkanetwork/assets.py` & `enkanetworkv2.py-2.0.6/enkanetwork/assets.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.5/enkanetwork/cache.py` & `enkanetworkv2.py-2.0.6/enkanetwork/cache.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.5/enkanetwork/client.py` & `enkanetworkv2.py-2.0.6/enkanetwork/client.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.5/enkanetwork/config.py` & `enkanetworkv2.py-2.0.6/enkanetwork/config.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.5/enkanetwork/enum.py` & `enkanetworkv2.py-2.0.6/enkanetwork/enum.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.5/enkanetwork/exception.py` & `enkanetworkv2.py-2.0.6/enkanetwork/exception.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.5/enkanetwork/http.py` & `enkanetworkv2.py-2.0.6/enkanetwork/http.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.5/enkanetwork/model/assets.py` & `enkanetworkv2.py-2.0.6/enkanetwork/model/assets.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.5/enkanetwork/model/base.py` & `enkanetworkv2.py-2.0.6/enkanetwork/model/base.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.5/enkanetwork/model/build.py` & `enkanetworkv2.py-2.0.6/enkanetwork/model/build.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.5/enkanetwork/model/character.py` & `enkanetworkv2.py-2.0.6/enkanetwork/model/character.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.5/enkanetwork/model/equipments.py` & `enkanetworkv2.py-2.0.6/enkanetwork/model/equipments.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.5/enkanetwork/model/players.py` & `enkanetworkv2.py-2.0.6/enkanetwork/model/players.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.5/enkanetwork/model/stats.py` & `enkanetworkv2.py-2.0.6/enkanetwork/model/stats.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.5/enkanetwork/tools.py` & `enkanetworkv2.py-2.0.6/enkanetwork/tools.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.5/enkanetwork/types/enkanetwork.py` & `enkanetworkv2.py-2.0.6/enkanetwork/types/enkanetwork.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.5/enkanetwork/utils.py` & `enkanetworkv2.py-2.0.6/enkanetwork/utils.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.5/enkanetworkv2.py.egg-info/PKG-INFO` & `enkanetworkv2.py-2.0.6/enkanetworkv2.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enkanetworkv2.py
-Version: 2.0.5
+Version: 2.0.6
 Summary: Library for fetching JSON data from site https://enka.network/
 Home-page: https://github.com/DEViantUA/EnkaNetworkV2.py
 Author: DeviantUa
 Author-email: deviantapi@gmail.com
 Keywords: enkanetwork.py,enkanetwork,enka.network,genshinapi,enkanetworkV2,enkanetworkV2.py
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `enkanetworkv2.py-2.0.5/enkanetworkv2.py.egg-info/SOURCES.txt` & `enkanetworkv2.py-2.0.6/enkanetworkv2.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.5/setup.py` & `enkanetworkv2.py-2.0.6/setup.py`

 * *Files identical despite different names*

