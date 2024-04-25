# Comparing `tmp/x12306-0.2.1.tar.gz` & `tmp/x12306-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "x12306-0.2.1.tar", last modified: Mon Feb  5 13:13:01 2024, max compression
+gzip compressed data, was "x12306-0.3.0.tar", last modified: Thu Apr 25 13:45:49 2024, max compression
```

## Comparing `x12306-0.2.1.tar` & `x12306-0.3.0.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxr-xr-x   0 null       (501) staff       (20)        0 2024-02-05 13:13:01.468082 x12306-0.2.1/
--rw-r--r--   0 null       (501) staff       (20)     1060 2024-02-05 11:55:36.000000 x12306-0.2.1/LICENSE
--rw-r--r--   0 null       (501) staff       (20)       25 2024-02-05 12:01:34.000000 x12306-0.2.1/MANIFEST.in
--rw-r--r--   0 null       (501) staff       (20)     3397 2024-02-05 13:13:01.467680 x12306-0.2.1/PKG-INFO
--rw-r--r--   0 null       (501) staff       (20)     2175 2024-02-05 12:39:30.000000 x12306-0.2.1/README.md
--rw-r--r--   0 null       (501) staff       (20)       38 2024-02-05 13:13:01.468201 x12306-0.2.1/setup.cfg
--rw-r--r--   0 null       (501) staff       (20)     2168 2024-02-05 12:50:06.000000 x12306-0.2.1/setup.py
-drwxr-xr-x   0 null       (501) staff       (20)        0 2024-02-05 13:13:01.463292 x12306-0.2.1/x12306/
--rw-r--r--   0 null       (501) staff       (20)     2280 2024-02-05 12:38:36.000000 x12306-0.2.1/x12306/__init__.py
--rw-r--r--   0 null       (501) staff       (20)      456 2024-02-05 13:12:53.000000 x12306-0.2.1/x12306/__version__.py
--rw-r--r--   0 null       (501) staff       (20)     2876 2024-02-05 11:55:36.000000 x12306-0.2.1/x12306/config.py
-drwxr-xr-x   0 null       (501) staff       (20)        0 2024-02-05 13:13:01.466898 x12306-0.2.1/x12306/data/
--rw-r--r--   0 null       (501) staff       (20)    31811 2024-02-05 11:55:36.000000 x12306-0.2.1/x12306/data/cdn.txt
--rw-r--r--   0 null       (501) staff       (20)        0 2024-02-05 11:55:36.000000 x12306-0.2.1/x12306/data/proxies.txt
--rw-r--r--   0 null       (501) staff       (20)    95846 2024-02-05 11:55:36.000000 x12306-0.2.1/x12306/data/stations.txt
--rw-r--r--   0 null       (501) staff       (20)      105 2024-02-05 11:55:36.000000 x12306-0.2.1/x12306/exceptions.py
--rw-r--r--   0 null       (501) staff       (20)     3643 2024-02-05 12:21:21.000000 x12306-0.2.1/x12306/glovar.py
--rw-r--r--   0 null       (501) staff       (20)     1529 2024-02-05 11:55:36.000000 x12306-0.2.1/x12306/request.py
--rw-r--r--   0 null       (501) staff       (20)     9687 2024-02-05 11:55:36.000000 x12306-0.2.1/x12306/train.py
--rw-r--r--   0 null       (501) staff       (20)      975 2024-02-05 11:55:36.000000 x12306-0.2.1/x12306/utils.py
-drwxr-xr-x   0 null       (501) staff       (20)        0 2024-02-05 13:13:01.465710 x12306-0.2.1/x12306.egg-info/
--rw-r--r--   0 null       (501) staff       (20)     3397 2024-02-05 13:13:01.000000 x12306-0.2.1/x12306.egg-info/PKG-INFO
--rw-r--r--   0 null       (501) staff       (20)      435 2024-02-05 13:13:01.000000 x12306-0.2.1/x12306.egg-info/SOURCES.txt
--rw-r--r--   0 null       (501) staff       (20)        1 2024-02-05 13:13:01.000000 x12306-0.2.1/x12306.egg-info/dependency_links.txt
--rw-r--r--   0 null       (501) staff       (20)       48 2024-02-05 13:13:01.000000 x12306-0.2.1/x12306.egg-info/entry_points.txt
--rw-r--r--   0 null       (501) staff       (20)       27 2024-02-05 13:13:01.000000 x12306-0.2.1/x12306.egg-info/requires.txt
--rw-r--r--   0 null       (501) staff       (20)        7 2024-02-05 13:13:01.000000 x12306-0.2.1/x12306.egg-info/top_level.txt
+drwxr-xr-x   0 null       (501) staff       (20)        0 2024-04-25 13:45:49.268462 x12306-0.3.0/
+-rw-r--r--   0 null       (501) staff       (20)     1060 2024-02-05 11:55:36.000000 x12306-0.3.0/LICENSE
+-rw-r--r--   0 null       (501) staff       (20)       25 2024-02-05 12:01:34.000000 x12306-0.3.0/MANIFEST.in
+-rw-r--r--   0 null       (501) staff       (20)     4342 2024-04-25 13:45:49.268100 x12306-0.3.0/PKG-INFO
+-rw-r--r--   0 null       (501) staff       (20)     3137 2024-04-25 13:43:34.000000 x12306-0.3.0/README.md
+-rw-r--r--   0 null       (501) staff       (20)       38 2024-04-25 13:45:49.268571 x12306-0.3.0/setup.cfg
+-rw-r--r--   0 null       (501) staff       (20)     2168 2024-02-05 12:50:06.000000 x12306-0.3.0/setup.py
+drwxr-xr-x   0 null       (501) staff       (20)        0 2024-04-25 13:45:49.263953 x12306-0.3.0/x12306/
+-rw-r--r--   0 null       (501) staff       (20)     2226 2024-04-25 13:33:32.000000 x12306-0.3.0/x12306/__init__.py
+-rw-r--r--   0 null       (501) staff       (20)      440 2024-04-25 13:21:17.000000 x12306-0.3.0/x12306/__version__.py
+drwxr-xr-x   0 null       (501) staff       (20)        0 2024-04-25 13:45:49.267481 x12306-0.3.0/x12306/data/
+-rw-r--r--   0 null       (501) staff       (20)    31811 2024-02-05 11:55:36.000000 x12306-0.3.0/x12306/data/cdn.txt
+-rw-r--r--   0 null       (501) staff       (20)        0 2024-02-05 11:55:36.000000 x12306-0.3.0/x12306/data/proxies.txt
+-rw-r--r--   0 null       (501) staff       (20)    95846 2024-02-05 11:55:36.000000 x12306-0.3.0/x12306/data/stations.2019.txt
+-rw-r--r--   0 null       (501) staff       (20)   164536 2024-04-25 12:28:49.000000 x12306-0.3.0/x12306/data/stations.txt
+-rw-r--r--   0 null       (501) staff       (20)      105 2024-02-05 11:55:36.000000 x12306-0.3.0/x12306/exceptions.py
+-rw-r--r--   0 null       (501) staff       (20)     7241 2024-04-25 13:15:35.000000 x12306-0.3.0/x12306/settings.py
+-rw-r--r--   0 null       (501) staff       (20)     9557 2024-04-25 13:19:32.000000 x12306-0.3.0/x12306/train.py
+-rw-r--r--   0 null       (501) staff       (20)      716 2024-04-25 12:52:51.000000 x12306-0.3.0/x12306/utils.py
+drwxr-xr-x   0 null       (501) staff       (20)        0 2024-04-25 13:45:49.265512 x12306-0.3.0/x12306.egg-info/
+-rw-r--r--   0 null       (501) staff       (20)     4342 2024-04-25 13:45:49.000000 x12306-0.3.0/x12306.egg-info/PKG-INFO
+-rw-r--r--   0 null       (501) staff       (20)      432 2024-04-25 13:45:49.000000 x12306-0.3.0/x12306.egg-info/SOURCES.txt
+-rw-r--r--   0 null       (501) staff       (20)        1 2024-04-25 13:45:49.000000 x12306-0.3.0/x12306.egg-info/dependency_links.txt
+-rw-r--r--   0 null       (501) staff       (20)       48 2024-04-25 13:45:49.000000 x12306-0.3.0/x12306.egg-info/entry_points.txt
+-rw-r--r--   0 null       (501) staff       (20)       27 2024-04-25 13:45:49.000000 x12306-0.3.0/x12306.egg-info/requires.txt
+-rw-r--r--   0 null       (501) staff       (20)        7 2024-04-25 13:45:49.000000 x12306-0.3.0/x12306.egg-info/top_level.txt
```

### Comparing `x12306-0.2.1/LICENSE` & `x12306-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `x12306-0.2.1/setup.py` & `x12306-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `x12306-0.2.1/x12306/__init__.py` & `x12306-0.3.0/x12306/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,75 +4,71 @@
 @author: HJK
 @file: __init__.py
 @time: 2019-02-08
 """
 
 import click
 
-from .config import Options
-from .glovar import Glovar
+from .settings import settings
 from .train import TrainTable
 
 
 @click.command()
 @click.version_option()
 @click.option("-f", "--from-station", prompt="请输入出发地", help="出发地")
 @click.option("-t", "--to-station", prompt="请输入目的地", help="目的地")
 @click.option("-d", "--date", prompt="请输入日期（YYYY-MM-DD）", help="日期")
-@click.option("-s", "--seats", help="限制座位")
-@click.option("-n", "--train-no", help="限制车次")
+@click.option("-s", "--seats", help="限制座位，如：一等座 二等座 无座")
+@click.option("-n", "--trains-no", help="限制车次，如：G1 G2 G3")
 @click.option("-z", "--zmode", default=False, is_flag=True, help="高级模式，查询中间站点")
 @click.option("-zz", "--zzmode", default=False, is_flag=True, help="终极模式，查询所有中间站点")
 @click.option("-r", "--remaining", default=False, is_flag=True, help="只看有票")
+@click.option("-v", "--verbose", default=False, is_flag=True, help="调试模式")
 @click.option("--gcd", default=False, is_flag=True, help="只看高铁动车城际")
 @click.option("--ktz", default=False, is_flag=True, help="只看普快特快直达等")
 @click.option("--proxies-file", help="代理列表文件")
 @click.option("--stations-file", help="站点信息文件")
 @click.option("--cdn-file", help="CDN文件")
 def main(
     from_station,
     to_station,
     date,
     seats,
-    train_no,
+    trains_no,
     zmode,
     zzmode,
     remaining,
+    verbose,
     gcd,
     ktz,
     proxies_file,
     stations_file,
     cdn_file,
 ):
     """
     12306查票助手 https://github.com/0xHJK/x12306
 
-    Example：python x12306.py -f 上海 -t 北京 -d "2019-03-01" -n "G16 G18 G22" -r
-
-    如果查询失败的话，请修改glovar.py中的QUERY_URL和JSESSIONID
+    Example: python3 x12306.py -f 上海 -t 北京 -d "2024-05-01"
     """
-    opts = Options()
-    opts.fs = from_station
-    opts.ts = to_station
-    if date:
-        opts.date = date
-    if seats:
-        opts.seats = seats
-    if train_no:
-        opts.train_no = train_no
-    opts.zmode = zmode
-    opts.zzmode = zzmode
-    opts.gcd = gcd
-    opts.ktz = ktz
-    opts.remaining = remaining
-    if proxies_file:
-        opts.proxies_file = proxies_file
-    if stations_file:
-        opts.stations_file = stations_file
-    if cdn_file:
-        opts.cdn_file = cdn_file
+    settings.update(
+        fs=from_station,
+        ts=to_station,
+        date=date,
+        seats=seats,
+        trains_no=trains_no,
+        zmode=zmode,
+        zzmode=zzmode,
+        remaining=remaining,
+        verbose=verbose,
+        gcd=gcd,
+        ktz=ktz,
+        proxies_file=proxies_file,
+        stations_file=stations_file,
+        cdn_file=cdn_file,
+    )
 
     print("\n-----------------------")
-    print(opts)
+    print(settings)
+    print("查询中...请稍等... :)\n")
     tt = TrainTable()
-    tt.update_trains()
+    tt.update()
     tt.echo()
```

### Comparing `x12306-0.2.1/x12306/data/cdn.txt` & `x12306-0.3.0/x12306/data/cdn.txt`

 * *Files identical despite different names*

### Comparing `x12306-0.2.1/x12306/data/stations.txt` & `x12306-0.3.0/x12306/data/stations.2019.txt`

 * *Files identical despite different names*

### Comparing `x12306-0.2.1/x12306/train.py` & `x12306-0.3.0/x12306/train.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 """
 """
     搜索结果中的班次信息
 """
 
 import time
 import re
+import requests
 import prettytable as pt
 
-from .glovar import Glovar, QUERY_URL
-from .request import Request
-from .utils import code_to_station, station_to_code, colorize
+from .settings import settings
+from .utils import colorize
 
 
 class Train:
     """
     搜索结果中的班次信息，包括车次号、余票、时间等信息
     """
 
@@ -30,16 +30,14 @@
         self._ts_code = ""
         self._fs = ""
         self._ts = ""
         self.start_time = ""
         self.end_time = ""
         self.duration = ""
         self.remaining = []
-        # 途经的车站（站编码，站名，到达时间）元组
-        self.stations = []
 
     def __str__(self):
         colored_remaining = [
             colorize(s, "green") if s != "无" and s != "--" else s
             for s in self.remaining
         ]
         remaining_seats = "/".join(colored_remaining)
@@ -55,57 +53,57 @@
             self.end_time,
             remaining_seats,
             self.duration,
         )
         return s
 
     def __eq__(self, other):
-        """ 车次、出发站和目的地相同判断为相等 """
+        """车次、出发站和目的地相同判断为相等"""
         return (
             self.full_no == other.full_no
             and self._fs == other._fs
             and self._ts == other._ts
         )
 
     def __lt__(self, other):
-        """ 根据车次号排序 """
+        """根据车次号排序"""
         return self.start_time < other.start_time
 
     def __gt__(self, other):
-        """ 根据车次号排序 """
+        """根据车次号排序"""
         return self.start_time > other.start_time
 
     @property
     def fs_code(self):
         return self._fs_code
 
     @fs_code.setter
     def fs_code(self, fs_code):
         self._fs_code = fs_code
-        self._fs = code_to_station(fs_code)
+        self._fs = settings.reverse_stations_dict.get(fs_code, "")
 
     @property
     def ts_code(self):
         return self._ts_code
 
     @ts_code.setter
     def ts_code(self, ts_code):
         self._ts_code = ts_code
-        self._ts = code_to_station(ts_code)
+        self._ts = settings.reverse_stations_dict.get(ts_code, "")
 
     @property
     def has_remaining(self) -> bool:
         for r in self.remaining:
             if r != "无" and r != "--":
                 return True
         return False
 
     @property
     def row(self) -> list:
-        """ 关键信息列表 """
+        """关键信息列表"""
         colored_remaining = [
             colorize(s, "green") if s != "无" and s != "--" else s
             for s in self.remaining
         ]
         remaining_seats = "/".join(colored_remaining)
         if re.match("[GCD]", self.no):
             colored_no = colorize(self.no, self.no[0].lower())
@@ -117,189 +115,185 @@
             self._fs,
             self._ts,
             self.end_time,
             remaining_seats,
             self.duration,
         ]
 
-    def update_stations(self):
-        """
-            更新train对象中沿途车站的信息
-        :param train: Train对象
-        :param kwargs:
-        :return: 无返回
-        """
-        glovar = Glovar()
-        req = Request()
-        s = req.get_session()
-
-        # 准备请求参数
-        params = {
-            "train_no": self.full_no,
-            "from_station_telecode": self.fs_code,
-            "to_station_telecode": self.ts_code,
-            "depart_date": glovar.date,
-        }
-        # 发送请求
-        r = s.get(
-            "https://kyfw.12306.cn/otn/czxx/queryByTrainNo", params=params, timeout=10
-        )
-        j = r.json()
-        for item in j["data"]["data"]:
-            if not item["isEnabled"]:
-                continue
-            station_code = station_to_code(item["station_name"])
-            self.stations.append(
-                (station_code, item["station_name"], item["arrive_time"])
-            )
-
 
 class TrainTable:
     """
     搜索结果列表
     """
 
     def __init__(self):
         self.trains_list = []
+        self._session = requests.Session()
+        self._session.headers.update(settings.headers)
+
+    @property
+    def session(self):
+        # TODO: 设置代理、随机headers等
+        return self._session
 
     def echo(self):
         """
         对外调用的方法，用来打印查询结果
         """
         tb = pt.PrettyTable()
         tb.field_names = ["车次", "发车", "出发站", "到达站", "到达", "余票", "历时"]
         self.cleanup()
         for train in self.trains_list:
             tb.add_row(train.row)
         print(tb)
 
     def cleanup(self):
-        """ 处理trains_list，排序和删除无效数据 """
-        glovar = Glovar()
+        """处理trains_list，排序和删除无效数据"""
         t_list = []
-        if glovar.remaining:
+        if settings.remaining:
             for train in self.trains_list:
                 # print(train.no, train.remaining, train.has_remaining)
                 if train.has_remaining:
                     t_list.append(train)
         else:
             t_list = self.trains_list
         self.trains_list = sorted(t_list)
 
-    def update_trains(self, **kwargs):
+    def update(self):
         """
-            对外调用的方法，查询12306列车信息，把结果更新到trains_list中
-        :param kwargs:
+        对外调用的方法，查询12306列车信息，把结果更新到trains_list中
         """
-        glovar = Glovar()
-
-        fs = kwargs.get("fs", "")
-        ts = kwargs.get("ts", "")
-        if fs and ts:
-            # 优先处理fs和ts
-            fs_code = station_to_code(fs)
-            ts_code = station_to_code(ts)
+        if settings.zmode:
+            self.trains_list = self._query_trains_zmode(
+                settings.fs_code,
+                settings.ts_code,
+                settings.date,
+                settings.trains_no_list,
+            )
         else:
-            # 如果没有则再处理fs_code和ts_code
-            fs_code = kwargs.get("fs_code", glovar.fs_code)
-            ts_code = kwargs.get("ts_code", glovar.ts_code)
+            self.trains_list = self._query_trains(
+                settings.fs_code,
+                settings.ts_code,
+                settings.date,
+                settings.trains_no_list,
+            )
 
-        date = kwargs.get("date", glovar.date)
-        no_list = kwargs.get("no_list", glovar.no_list)
+    def _query(self, url, params, retries=1) -> dict:
+        """
+            查询方法，根据url和参数，返回json对象
+        :param url: 查询url
+        :param params: 查询参数
+        :param retries: 重试次数
+        :return: 返回json对象
+        """
+        s = self.session
+        # print("查询中...", " ".join([v for v in params.values()]))
+        if settings.verbose:
+            print(url, params)
+        try:
+            r = s.get(url, params=params, timeout=settings.timeout)
+            j = r.json()
+        except Exception as e:
+            print(colorize("第 %i 查询失败" % retries, "red"), e)
+            print(url, params)
+            print(s.headers)
+            if retries < settings.max_retries:
+                time.sleep(retries * settings.timeout)
+                return self._query(url, params, retries + 1)
+            else:
+                j = {}
+        return j
 
-        if kwargs.get("zmode", glovar.zmode):
-            self.trains_list = self._query_trains_zmode(fs_code, ts_code, date, no_list)
-        else:
-            self.trains_list = self._query_trains_basic(fs_code, ts_code, date, no_list)
+    def _query_stations(self, train) -> list:
+        """
+            查询沿途车站信息
+        :param train: Train对象
+        """
+        stations_list = []
+        # 准备请求参数
+        params = {
+            "train_no": train.full_no,
+            "from_station_telecode": train.fs_code,
+            "to_station_telecode": train.ts_code,
+            "depart_date": settings.date,
+        }
+        j = self._query(settings.trainno_url, params)
+        if j and j.get("data") and j["data"].get("data"):
+            for item in j["data"]["data"]:
+                if item["isEnabled"]:
+                    stations_list.append(item["station_name"])
+            stations_list = stations_list[1:-1]  # 除了出发站和目标站本身
+        return stations_list
 
-    def _query_trains_basic(self, fs_code, ts_code, date, no_list) -> list:
+    def _query_trains(self, fs_code, ts_code, date, trains_no_list) -> list:
         """
             普通查询方法，根据出发地和目的地编码、日期和限制车次，返回trains列表
             仅被内部调用，调用前处理好参数
         :param fs_code: 出发地编码
         :param ts_code: 目的地编码
         :param date: 日期
-        :param no_list: 选择车次列表
+        :param trains_no_list: 选择车次列表
         :return: 返回搜索结果列表，每一项是一个Train对象
         """
-        glovar = Glovar()
-        req = Request()
-        s = req.get_session()
         # 准备请求参数
         params = {
             "leftTicketDTO.train_date": date,
             "leftTicketDTO.from_station": fs_code,
             "leftTicketDTO.to_station": ts_code,
             "purpose_codes": "ADULT",
         }
-        try:
-            # 发送请求
-            print(params)
-            r = s.get(
-                QUERY_URL, params=params, timeout=10
-            )
-            j = r.json()
+        trains_list = []
+        j = self._query(settings.query_url, params)
+        if j and j.get("data") and j["data"].get("result"):
             raws = j["data"]["result"]
             # 处理返回结果
-            train_list = []
             for raw in raws:
                 fields = raw.split("|")
                 # 如果限制了车次，且搜索车次不在目标车次中则丢弃
-                if no_list and fields[3] not in no_list:
+                if trains_no_list and fields[3] not in trains_no_list:
                     continue
-                # 如果限制了种类
-                if glovar.gcd:
+                if settings.gcd and fields[3][0] not in "GCD":
                     # 只看高铁动车城际
-                    if fields[3][0] not in "GCD":
-                        continue
-                elif glovar.ktz:
+                    continue
+                if settings.ktz and fields[3][0] in "GCD":
                     # 只看普通列车
-                    if fields[3][0] in "GCD":
-                        continue
+                    continue
 
                 train = Train()
                 train.full_no = fields[2]  # 编号全称
                 train.no = fields[3]  # 编号简称
                 train.fs_code = fields[6]
                 train.ts_code = fields[7]
                 train.start_time = fields[8]
                 train.end_time = fields[9]
                 train.duration = fields[10]
-                for i in glovar.seats_idx_list:
+                for i in settings.seats_code_list:
                     train.remaining.append(fields[i] or "--")
-                train_list.append(train)
-        except Exception as e:
-            print(e)
-            print(r.text)
-            print(s.headers)
-            train_list = []
-        return train_list
+                trains_list.append(train)
+        return trains_list
 
-    def _query_trains_zmode(self, fs_code, ts_code, date, no_list) -> list:
+    def _query_trains_zmode(self, fs_code, ts_code, date, trains_no_list) -> list:
         """
             高级查询模式，会查询从出发站到沿途所有站的车次情况
             仅被内部调用，调用前处理好参数
         :param fs_code: 出发地编码
         :param ts_code: 目的地编码
         :param date: 日期
-        :param no_list: 限制车次
+        :param trains_no_list: 限制车次
         :return: Train对象列表
         """
-        # stations_set = set()
-        stations_dict = {}
-        trains_list = self._query_trains_basic(fs_code, ts_code, date, no_list)
-        try:
-            for train in trains_list:
-                train.update_stations()
-                for station in train.stations[1:-1]:  # 除了出发站和目标站本身
-                    # stations_set.add(station[0])
-                    if station[0] in stations_dict:
-                        stations_dict[station[0]].append(train.no)
-                    else:
-                        stations_dict[station[0]] = [train.no]
-            for station, trains in stations_dict.items():
-                time.sleep(1)
-                trains_list += self._query_trains_basic(fs_code, station, date, trains)
-        except Exception as e:
-            print(e)
-        finally:
-            return trains_list
+        trains_list = self._query_trains(fs_code, ts_code, date, trains_no_list)
+        trains_no_list = [train.no for train in trains_list]
+        stations_list = []
+
+        for train in trains_list:
+            stations_list += self._query_stations(train)
+        stations_list = list(set(stations_list))
+
+        for station in stations_list:
+            ts_code = settings.stations_dict.get(station, "")
+            if ts_code:
+                trains_list += self._query_trains(
+                    fs_code, ts_code, date, trains_no_list
+                )
+
+        return trains_list
```

