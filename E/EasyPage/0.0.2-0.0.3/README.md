# Comparing `tmp/EasyPage-0.0.2.tar.gz` & `tmp/EasyPage-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EasyPage-0.0.2.tar", last modified: Thu Apr 25 08:07:19 2024, max compression
+gzip compressed data, was "EasyPage-0.0.3.tar", last modified: Thu Apr 25 08:40:18 2024, max compression
```

## Comparing `EasyPage-0.0.2.tar` & `EasyPage-0.0.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 08:07:19.214280 EasyPage-0.0.2/
-drwxrwxrwx   0        0        0        0 2024-04-25 08:07:19.183277 EasyPage-0.0.2/EasyPage.egg-info/
--rw-rw-rw-   0        0        0      286 2024-04-25 08:07:19.000000 EasyPage-0.0.2/EasyPage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      918 2024-04-25 08:07:19.000000 EasyPage-0.0.2/EasyPage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 08:07:19.000000 EasyPage-0.0.2/EasyPage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2024-04-25 08:07:19.000000 EasyPage-0.0.2/EasyPage.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-25 08:07:19.000000 EasyPage-0.0.2/EasyPage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      286 2024-04-25 08:07:19.214280 EasyPage-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-25 08:07:19.193277 EasyPage-0.0.2/easypage/
--rw-rw-rw-   0        0        0       81 2024-04-22 09:13:20.000000 EasyPage-0.0.2/easypage/__init__.py
--rw-rw-rw-   0        0        0     3243 2024-04-22 08:15:25.000000 EasyPage-0.0.2/easypage/cdp.py
-drwxrwxrwx   0        0        0        0 2024-04-25 08:07:19.205277 EasyPage-0.0.2/easypage/cdp_method/
--rw-rw-rw-   0        0        0        0 2024-04-17 12:56:48.000000 EasyPage-0.0.2/easypage/cdp_method/__init__.py
--rw-rw-rw-   0        0        0     1536 2024-04-24 09:10:40.000000 EasyPage-0.0.2/easypage/cdp_method/browser.py
--rw-rw-rw-   0        0        0    12414 2024-04-24 09:08:35.000000 EasyPage-0.0.2/easypage/cdp_method/dom.py
--rw-rw-rw-   0        0        0     1049 2024-04-24 08:57:22.000000 EasyPage-0.0.2/easypage/cdp_method/emulation.py
--rw-rw-rw-   0        0        0     9545 2024-04-24 14:05:55.000000 EasyPage-0.0.2/easypage/cdp_method/fetch.py
--rw-rw-rw-   0        0        0     2654 2024-04-24 09:06:00.000000 EasyPage-0.0.2/easypage/cdp_method/input.py
--rw-rw-rw-   0        0        0     3598 2024-04-24 11:46:26.000000 EasyPage-0.0.2/easypage/cdp_method/network.py
--rw-rw-rw-   0        0        0     5659 2024-04-24 09:12:45.000000 EasyPage-0.0.2/easypage/cdp_method/page.py
--rw-rw-rw-   0        0        0     3667 2024-04-24 09:16:01.000000 EasyPage-0.0.2/easypage/cdp_method/runtime.py
--rw-rw-rw-   0        0        0     2354 2024-04-24 09:16:01.000000 EasyPage-0.0.2/easypage/cdp_method/security.py
--rw-rw-rw-   0        0        0     1322 2024-04-24 09:16:01.000000 EasyPage-0.0.2/easypage/cdp_method/storage.py
--rw-rw-rw-   0        0        0     5884 2024-04-24 13:35:04.000000 EasyPage-0.0.2/easypage/cdp_method/target.py
--rw-rw-rw-   0        0        0    15945 2024-04-24 13:42:44.000000 EasyPage-0.0.2/easypage/conn.py
--rw-rw-rw-   0        0        0      391 2024-04-25 02:28:17.000000 EasyPage-0.0.2/easypage/definition.py
-drwxrwxrwx   0        0        0        0 2024-04-25 08:07:19.209277 EasyPage-0.0.2/easypage/driver/
--rw-rw-rw-   0        0        0        0 2024-04-09 06:15:36.000000 EasyPage-0.0.2/easypage/driver/__init__.py
--rw-rw-rw-   0        0        0     6188 2024-04-24 14:23:36.000000 EasyPage-0.0.2/easypage/driver/browser.py
--rw-rw-rw-   0        0        0     1587 2024-04-24 02:49:07.000000 EasyPage-0.0.2/easypage/driver/driver.py
--rw-rw-rw-   0        0        0    21191 2024-04-25 07:47:13.000000 EasyPage-0.0.2/easypage/driver/page.py
--rw-rw-rw-   0        0        0     1462 2024-04-24 08:29:43.000000 EasyPage-0.0.2/easypage/errors.py
--rw-rw-rw-   0        0        0     2074 2024-04-22 08:51:10.000000 EasyPage-0.0.2/easypage/logger.py
--rw-rw-rw-   0        0        0     4086 2024-04-25 02:12:39.000000 EasyPage-0.0.2/easypage/main.py
--rw-rw-rw-   0        0        0     4108 2024-04-25 01:40:28.000000 EasyPage-0.0.2/easypage/operate.py
--rw-rw-rw-   0        0        0    10944 2024-04-24 08:39:28.000000 EasyPage-0.0.2/easypage/options.py
--rw-rw-rw-   0        0        0     2787 2024-04-22 08:05:28.000000 EasyPage-0.0.2/easypage/settings.py
-drwxrwxrwx   0        0        0        0 2024-04-25 08:07:19.212278 EasyPage-0.0.2/easypage/utils/
--rw-rw-rw-   0        0        0        0 2024-04-09 06:15:42.000000 EasyPage-0.0.2/easypage/utils/__init__.py
--rw-rw-rw-   0        0        0     3708 2024-04-10 01:27:44.000000 EasyPage-0.0.2/easypage/utils/browser_utils.py
--rw-rw-rw-   0        0        0     1134 2024-04-24 06:28:10.000000 EasyPage-0.0.2/easypage/utils/other_utils.py
--rw-rw-rw-   0        0        0       42 2024-04-25 08:07:19.215278 EasyPage-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      599 2024-04-25 08:07:16.000000 EasyPage-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 08:40:18.158640 EasyPage-0.0.3/
+drwxrwxrwx   0        0        0        0 2024-04-25 08:40:17.900632 EasyPage-0.0.3/EasyPage.egg-info/
+-rw-rw-rw-   0        0        0      286 2024-04-25 08:40:17.000000 EasyPage-0.0.3/EasyPage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      918 2024-04-25 08:40:17.000000 EasyPage-0.0.3/EasyPage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 08:40:17.000000 EasyPage-0.0.3/EasyPage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2024-04-25 08:40:17.000000 EasyPage-0.0.3/EasyPage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-25 08:40:17.000000 EasyPage-0.0.3/EasyPage.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      286 2024-04-25 08:40:18.157640 EasyPage-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-25 08:40:17.998918 EasyPage-0.0.3/easypage/
+-rw-rw-rw-   0        0        0       81 2024-04-22 09:13:20.000000 EasyPage-0.0.3/easypage/__init__.py
+-rw-rw-rw-   0        0        0     3243 2024-04-22 08:15:25.000000 EasyPage-0.0.3/easypage/cdp.py
+drwxrwxrwx   0        0        0        0 2024-04-25 08:40:18.106638 EasyPage-0.0.3/easypage/cdp_method/
+-rw-rw-rw-   0        0        0        0 2024-04-17 12:56:48.000000 EasyPage-0.0.3/easypage/cdp_method/__init__.py
+-rw-rw-rw-   0        0        0     1536 2024-04-24 09:10:40.000000 EasyPage-0.0.3/easypage/cdp_method/browser.py
+-rw-rw-rw-   0        0        0    12414 2024-04-24 09:08:35.000000 EasyPage-0.0.3/easypage/cdp_method/dom.py
+-rw-rw-rw-   0        0        0     1049 2024-04-24 08:57:22.000000 EasyPage-0.0.3/easypage/cdp_method/emulation.py
+-rw-rw-rw-   0        0        0     9545 2024-04-24 14:05:55.000000 EasyPage-0.0.3/easypage/cdp_method/fetch.py
+-rw-rw-rw-   0        0        0     2654 2024-04-24 09:06:00.000000 EasyPage-0.0.3/easypage/cdp_method/input.py
+-rw-rw-rw-   0        0        0     3598 2024-04-24 11:46:26.000000 EasyPage-0.0.3/easypage/cdp_method/network.py
+-rw-rw-rw-   0        0        0     5659 2024-04-24 09:12:45.000000 EasyPage-0.0.3/easypage/cdp_method/page.py
+-rw-rw-rw-   0        0        0     3667 2024-04-24 09:16:01.000000 EasyPage-0.0.3/easypage/cdp_method/runtime.py
+-rw-rw-rw-   0        0        0     2354 2024-04-24 09:16:01.000000 EasyPage-0.0.3/easypage/cdp_method/security.py
+-rw-rw-rw-   0        0        0     1322 2024-04-24 09:16:01.000000 EasyPage-0.0.3/easypage/cdp_method/storage.py
+-rw-rw-rw-   0        0        0     5884 2024-04-24 13:35:04.000000 EasyPage-0.0.3/easypage/cdp_method/target.py
+-rw-rw-rw-   0        0        0    15945 2024-04-24 13:42:44.000000 EasyPage-0.0.3/easypage/conn.py
+-rw-rw-rw-   0        0        0      391 2024-04-25 02:28:17.000000 EasyPage-0.0.3/easypage/definition.py
+drwxrwxrwx   0        0        0        0 2024-04-25 08:40:18.137642 EasyPage-0.0.3/easypage/driver/
+-rw-rw-rw-   0        0        0        0 2024-04-09 06:15:36.000000 EasyPage-0.0.3/easypage/driver/__init__.py
+-rw-rw-rw-   0        0        0     6188 2024-04-24 14:23:36.000000 EasyPage-0.0.3/easypage/driver/browser.py
+-rw-rw-rw-   0        0        0     1587 2024-04-24 02:49:07.000000 EasyPage-0.0.3/easypage/driver/driver.py
+-rw-rw-rw-   0        0        0    25480 2024-04-25 08:40:04.000000 EasyPage-0.0.3/easypage/driver/page.py
+-rw-rw-rw-   0        0        0     1462 2024-04-24 08:29:43.000000 EasyPage-0.0.3/easypage/errors.py
+-rw-rw-rw-   0        0        0     2074 2024-04-22 08:51:10.000000 EasyPage-0.0.3/easypage/logger.py
+-rw-rw-rw-   0        0        0     4095 2024-04-25 08:18:53.000000 EasyPage-0.0.3/easypage/main.py
+-rw-rw-rw-   0        0        0     4106 2024-04-25 08:20:54.000000 EasyPage-0.0.3/easypage/operate.py
+-rw-rw-rw-   0        0        0    10944 2024-04-24 08:39:28.000000 EasyPage-0.0.3/easypage/options.py
+-rw-rw-rw-   0        0        0     2787 2024-04-22 08:05:28.000000 EasyPage-0.0.3/easypage/settings.py
+drwxrwxrwx   0        0        0        0 2024-04-25 08:40:18.146641 EasyPage-0.0.3/easypage/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-09 06:15:42.000000 EasyPage-0.0.3/easypage/utils/__init__.py
+-rw-rw-rw-   0        0        0     3708 2024-04-10 01:27:44.000000 EasyPage-0.0.3/easypage/utils/browser_utils.py
+-rw-rw-rw-   0        0        0     1134 2024-04-24 06:28:10.000000 EasyPage-0.0.3/easypage/utils/other_utils.py
+-rw-rw-rw-   0        0        0       42 2024-04-25 08:40:18.158640 EasyPage-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      599 2024-04-25 08:40:11.000000 EasyPage-0.0.3/setup.py
```

### Comparing `EasyPage-0.0.2/EasyPage.egg-info/SOURCES.txt` & `EasyPage-0.0.3/EasyPage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.2/easypage/cdp.py` & `EasyPage-0.0.3/easypage/cdp.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.2/easypage/cdp_method/browser.py` & `EasyPage-0.0.3/easypage/cdp_method/browser.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.2/easypage/cdp_method/dom.py` & `EasyPage-0.0.3/easypage/cdp_method/dom.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.2/easypage/cdp_method/emulation.py` & `EasyPage-0.0.3/easypage/cdp_method/emulation.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.2/easypage/cdp_method/fetch.py` & `EasyPage-0.0.3/easypage/cdp_method/fetch.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.2/easypage/cdp_method/input.py` & `EasyPage-0.0.3/easypage/cdp_method/input.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.2/easypage/cdp_method/network.py` & `EasyPage-0.0.3/easypage/cdp_method/network.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.2/easypage/cdp_method/page.py` & `EasyPage-0.0.3/easypage/cdp_method/page.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.2/easypage/cdp_method/runtime.py` & `EasyPage-0.0.3/easypage/cdp_method/runtime.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.2/easypage/cdp_method/security.py` & `EasyPage-0.0.3/easypage/cdp_method/security.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.2/easypage/cdp_method/storage.py` & `EasyPage-0.0.3/easypage/cdp_method/storage.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.2/easypage/cdp_method/target.py` & `EasyPage-0.0.3/easypage/cdp_method/target.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.2/easypage/conn.py` & `EasyPage-0.0.3/easypage/conn.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.2/easypage/driver/browser.py` & `EasyPage-0.0.3/easypage/driver/browser.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.2/easypage/driver/driver.py` & `EasyPage-0.0.3/easypage/driver/driver.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.2/easypage/driver/page.py` & `EasyPage-0.0.3/easypage/driver/page.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 """
     页面 driver
 """
 import time
+import base64
+import websocket
+from pathlib import Path
 from parsel import Selector
 from bs4 import BeautifulSoup
 from easypage.logger import logger
 from typing import Tuple, Union, List
 from easypage import definition, errors
 from easypage.driver.driver import Driver
 from easypage.options import BrowserOptions
@@ -133,14 +136,129 @@
             return status, result
 
         if 'value' in result['result']:
             return True, result['result']['value']
         else:
             return False, result['result']['description']
 
+    def frames(self) -> List['IframeElement']:
+        """
+        获取所有的 iframe
+
+        :return:
+        """
+        self.cdp.target.get_targets()
+
+        elements = []
+
+        status, new_node_ids = self.cdp.dom.query_selector_all(
+            selector="iframe",
+        )
+        if not new_node_ids or not status:
+            return elements
+
+        for node_id in new_node_ids['nodeIds']:
+            status, frame_id = self.cdp.dom.describe_node(nodeId=node_id)
+            if not frame_id or not status:
+                continue
+
+            frame_id = frame_id['node']['frameId']
+
+            try:
+                elements.append(IframeElement(opts=self._opts, driver_type=TYPE_PAGE, driver_id=frame_id))
+            except websocket.WebSocketBadStatusException:
+                logger.warning("当前 iframe 可能已不在页面上：{}", frame_id)
+
+        return elements
+
+    def cookies(self, only_key_val: bool = True, domain: str = None) -> Union[List[dict], dict]:
+        """
+        获取 cookie
+
+        :param only_key_val: 是否仅返回 {name:'',value:''} 形式
+        :param domain: 指定域名
+        :return: [{'name': '', 'value': '', 'domain': '', 'path': '', 'expires': -1, 'size': 161, 'httpOnly': True, 'secure': True, 'session': True, 'sameSite': 'Strict', 'priority': 'Medium', 'sameParty': False, 'sourceScheme': 'Secure', 'sourcePort': 443}]
+        """
+        status, cookies = self.cdp.storage.get_cookies(context_id=self._context_id)
+        if not status:
+            return []
+
+        cookies = cookies['cookies']
+
+        if only_key_val:
+            cookie_dict = {}
+            for c in cookies:
+                if domain:
+                    if c['domain'] == domain:
+                        cookie_dict[c['name']] = c['value']
+                else:
+                    cookie_dict[c['name']] = c['value']
+
+            return cookie_dict
+        else:
+            if domain:
+                return list(filter(lambda x: x['domain'] == domain, cookies))
+            return cookies
+
+    def screenshot(
+            self,
+            save_path: str = None,
+            format_type: str = "png",
+            quality: int = None,
+            clip: dict = None,
+            from_surface: bool = True,
+            capture_beyond_viewport: bool = False,
+            optimize_for_speed: bool = False,
+    ) -> bytes:
+        """
+        截图
+
+        https://chromedevtools.github.io/devtools-protocol/tot/Page/#method-captureScreenshot
+
+        clip 参考：https://chromedevtools.github.io/devtools-protocol/tot/Page/#type-Viewport
+
+        :param save_path: 保存本地的路径
+        :param format_type: jpeg, png, webp，默认值为 png
+        :param quality: 压缩质量范围为 [0..100]（仅限 jpeg）
+        :param clip: 仅捕获给定区域的屏幕截图（{x:1,y:1,width:1,height:1,scale:1}）
+        :param from_surface: 从表面捕获屏幕截图，而不是从视图捕获屏幕截图，默认值为 true
+        :param capture_beyond_viewport: 捕获视口之外的屏幕截图，默认值为 false
+        :param optimize_for_speed: 优化图像编码以提高速度，而不是优化结果大小（默认为 false）
+        :return: {"data":""}
+        """
+        # 等待页面加载
+        self.wait_loaded()
+
+        # 截图
+        status, data = self.cdp.page.capture_screenshot(
+            format_type=format_type,
+            quality=quality,
+            clip=clip,
+            from_surface=from_surface,
+            capture_beyond_viewport=capture_beyond_viewport,
+            optimize_for_speed=optimize_for_speed
+        )
+
+        if not status or not data:
+            return b""
+
+        data_bytes = base64.b64decode(data["data"])
+
+        # 保存本地
+        if save_path:
+            save_path = Path(save_path).absolute().resolve()
+            save_path.parent.mkdir(parents=True, exist_ok=True)
+            if not save_path.suffix:
+                save_path = save_path.with_suffix(".png")
+
+            with open(save_path, "wb") as f:
+                f.write(data_bytes)
+
+        return data_bytes
+
     def close(self):
         """
         关闭当前页面
 
         :return:
         """
         self.cdp.page.close()
```

### Comparing `EasyPage-0.0.2/easypage/errors.py` & `EasyPage-0.0.3/easypage/errors.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.2/easypage/logger.py` & `EasyPage-0.0.3/easypage/logger.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.2/easypage/main.py` & `EasyPage-0.0.3/easypage/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         :param log_level: 日志等级（如：logging 模块的 logging.WARNING）
         :param reuse: 是否复用已经存在的浏览器（根据 opts 内的端口判断复用，无法复用则创建新端口）
         :param reuse_close: 复用浏览器时，是否在结束时关闭浏览器并清理资源（默认关闭）
         """
         # 配置日志等级
         log_level = log_level or settings.LOGGER_LEVEL
         # TODO: 临时处理，为了通过 loguru，后续需要修改
-        if settings.SYSTEM_TYPE == "windows":
+        if not settings.SYSTEM_TYPE.startswith("win"):
             logger.logger.setLevel(log_level)
 
         self._opts = opts or BrowserOptions()
         self._reuse = reuse
         self._reuse_close = reuse_close
 
         self._proc: "Popen" = None  # type: ignore
```

### Comparing `EasyPage-0.0.2/easypage/operate.py` & `EasyPage-0.0.3/easypage/operate.py`

 * *Files 7% similar despite different names*

```diff
@@ -80,15 +80,15 @@
             port = browser_utils.find_free_port()
             opts.set_address(ip=opts.ip or settings.BROWSER_START_IP, port=port)
             logger.warning("当前端口被占用，已启用随机端口：{}", port)
 
     # 判断用户文件夹（不创建的话，会和已有的混在一起导致异常：）
     if not opts.user_data_dir:
         opts.set_user_data_dir(path=settings.USER_DATA_DIR + str(opts.port), delete_if_exists=True)
-        logger.warning("未设置用户文件夹，已使用默认路径：{}", opts.user_data_dir)
+        logger.debug("未设置用户文件夹，已使用默认路径：{}", opts.user_data_dir)
 
     # 加入插件
     if opts.extensions:
         opts.add(f"--load-extension={','.join(opts.extensions)}")
 
     # headless 判断（隐私模式没加 ua 的话，会导致部分网站通过 ua 检测出来：Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) HeadlessChrome/125.0.0.0 Safari/537.36）
     if opts.headless and not opts.user_agent:
```

### Comparing `EasyPage-0.0.2/easypage/options.py` & `EasyPage-0.0.3/easypage/options.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.2/easypage/settings.py` & `EasyPage-0.0.3/easypage/settings.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.2/easypage/utils/browser_utils.py` & `EasyPage-0.0.3/easypage/utils/browser_utils.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.2/easypage/utils/other_utils.py` & `EasyPage-0.0.3/easypage/utils/other_utils.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.2/setup.py` & `EasyPage-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='EasyPage',
-    version='0.0.2',
+    version='0.0.3',
     author='leviathangk',
     author_email='1015295213@qq.com',
     description='基于 CDP 协议，简洁快速的浏览器控制 API',
     keywords=['EasyPage', 'page', 'browser'],
     packages=find_packages(),
     install_requires=[
         "lxml",
```

