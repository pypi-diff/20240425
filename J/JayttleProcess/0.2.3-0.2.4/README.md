# Comparing `tmp/JayttleProcess-0.2.3-py3-none-any.whl.zip` & `tmp/JayttleProcess-0.2.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 53835 bytes, number of entries: 13
+Zip file size: 54637 bytes, number of entries: 13
 -rw-rw-rw-  2.0 fat     2978 b- defN 24-Apr-24 02:33 JayttleProcess/CommonDecorator.py
--rw-rw-rw-  2.0 fat    10691 b- defN 24-Apr-24 02:33 JayttleProcess/ComputerControl.py
+-rw-rw-rw-  2.0 fat    10765 b- defN 24-Apr-24 06:24 JayttleProcess/ComputerControl.py
 -rw-rw-rw-  2.0 fat      613 b- defN 24-Apr-08 05:57 JayttleProcess/EntertainmentCode.py
 -rw-rw-rw-  2.0 fat     6780 b- defN 24-Apr-23 15:04 JayttleProcess/FTPCommonUse.py
 -rw-rw-rw-  2.0 fat     5650 b- defN 24-Apr-24 02:33 JayttleProcess/JsonCommonManage.py
--rw-rw-rw-  2.0 fat    36633 b- defN 24-Apr-23 07:39 JayttleProcess/RinexCommonManage.py
--rw-rw-rw-  2.0 fat    32805 b- defN 24-Apr-24 02:33 JayttleProcess/SQLCommonUse.py
+-rw-rw-rw-  2.0 fat    39588 b- defN 24-Apr-24 06:24 JayttleProcess/RinexCommonManage.py
+-rw-rw-rw-  2.0 fat    32805 b- defN 24-Apr-24 06:24 JayttleProcess/SQLCommonUse.py
 -rw-rw-rw-  2.0 fat   117788 b- defN 24-Apr-24 02:34 JayttleProcess/TimeSeriesDataMethod.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-14 14:39 JayttleProcess/__init__.py
--rw-rw-rw-  2.0 fat      554 b- defN 24-Apr-24 02:34 JayttleProcess-0.2.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-24 02:34 JayttleProcess-0.2.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 24-Apr-24 02:34 JayttleProcess-0.2.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1133 b- defN 24-Apr-24 02:34 JayttleProcess-0.2.3.dist-info/RECORD
-13 files, 215732 bytes uncompressed, 51925 bytes compressed:  75.9%
+-rw-rw-rw-  2.0 fat      554 b- defN 24-Apr-24 06:25 JayttleProcess-0.2.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-24 06:25 JayttleProcess-0.2.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 24-Apr-24 06:25 JayttleProcess-0.2.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1133 b- defN 24-Apr-24 06:25 JayttleProcess-0.2.4.dist-info/RECORD
+13 files, 218761 bytes uncompressed, 52727 bytes compressed:  75.9%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: JayttleProcess/TimeSeriesDataMethod.py
 Comment: 
 
 Filename: JayttleProcess/__init__.py
 Comment: 
 
-Filename: JayttleProcess-0.2.3.dist-info/METADATA
+Filename: JayttleProcess-0.2.4.dist-info/METADATA
 Comment: 
 
-Filename: JayttleProcess-0.2.3.dist-info/WHEEL
+Filename: JayttleProcess-0.2.4.dist-info/WHEEL
 Comment: 
 
-Filename: JayttleProcess-0.2.3.dist-info/top_level.txt
+Filename: JayttleProcess-0.2.4.dist-info/top_level.txt
 Comment: 
 
-Filename: JayttleProcess-0.2.3.dist-info/RECORD
+Filename: JayttleProcess-0.2.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## JayttleProcess/ComputerControl.py

```diff
@@ -112,33 +112,32 @@
 
 def get_mouse_position():
     """获取鼠标位置"""
     x, y = pyautogui.position()
     # 返回鼠标位置
     return x, y
 
-def list_folders(directory):
+def list_folders(directory: str) -> list[str]:
     """获取目标文件夹下的所有文件夹folder名字"""
     folder_names = []
     for root, dirs, files in os.walk(directory):
         for folder in dirs:
             folder_names.append(os.path.join(root, folder))
     return folder_names
 
-def list_files_in_folders(folder_names):
+def list_files_in_folders(folder_names: list[str]) -> list[str]:
     """获取目标文件夹下的所有文件file名字"""
     file_paths = []
     for folder in folder_names:
         for root, dirs, files in os.walk(folder):
             for file in files:
                 file_paths.append(os.path.join(root, file))
     return file_paths
 
-
-def read_text_from_window(window_region):
+def read_text_from_window(window_region: tuple[int, int, int, int]) -> str:
     """
     从指定的窗口区域中读取文本
     Args:
         window_region: 窗口区域的坐标 (x, y, width, height)
     Returns:
         识别到的文本
     """
```

## JayttleProcess/RinexCommonManage.py

```diff
@@ -817,30 +817,30 @@
                 os.remove(rnx_info.file_info)
         else:
             print("CRX to RNX conversion failed with error:", process.stderr.read())
 
 
 
 
-def merge_files_threadpool(file_groups: list[list[RinexFileInfo]], merge_path: str) -> None:
+def merge_files_threadpool(file_groups: list[list[RinexFileInfo]], merge_path: str, merge_file_num: int) -> None:
     """
     使用线程池将 RinexFileInfo 对象列表合并到指定路径。
 
     参数：
         file_groups (list[list[RinexFileInfo]]): RinexFileInfo 对象列表的列表。
         merge_path (str): 合并后的文件存储路径。
+        merge_file_num (int): 每个 RinexFileInfo 对象列表中所需的文件数量。
     """
-    # 使用 ThreadPoolExecutor 来管理线程池
     with concurrent.futures.ThreadPoolExecutor(max_workers=8) as executor:
-        # 创建一个将 future 对象映射到 RinexFileInfo 对象列表的字典
-        futures = {executor.submit(MergeFiles.merge_files, rinex_files, merge_path): i for i, rinex_files in enumerate(file_groups)}
-        # 遍历 future 对象，直到它们完成
-        for future in concurrent.futures.as_completed(futures):
+        for rinex_files in file_groups:
+            if len(rinex_files) != merge_file_num:
+                print(f"文件数量不符合要求，跳过合并操作：{rinex_files}")
+                continue
+            future = executor.submit(MergeFiles.merge_files, rinex_files, merge_path)
             try:
-                # 尝试获取 future 的结果，如果出现异常则捕获并打印
                 future.result()
             except Exception as e:
                 print(f"发生异常：{e}")
 
 
 def process_file(file_path: str, file_name: str) -> None:
     """
@@ -890,7 +890,64 @@
         # 等待所有任务完成
         for future in concurrent.futures.as_completed(futures):
             try:
                 future.result()
             except Exception as e:
                 print(f"An exception occurred: {e}")
 
+#TODO: 实现toDownload与实际下载与解压后的文件还差哪些
+
+def count_lines_in_each_txt_file(folder_path: str) -> dict[str, int]:
+    file_lines_mapping = {}
+    for root, dirs, files in os.walk(folder_path):
+        for file_name in files:
+            if file_name.endswith('.txt'):
+                file_path = os.path.join(root, file_name)
+                with open(file_path, 'r', encoding='utf-8') as file:
+                    lines = file.readlines()
+                    num_lines = len(lines)
+                    file_lines_mapping[file_name[:4]] = num_lines
+    return file_lines_mapping
+
+
+def count_files_in_folders(root_folder: str) -> dict:
+    folder_file_count = {}
+    small_file_count = 0  # 记录文件大小小于 250KB 的个数
+    for root, dirs, files in os.walk(root_folder):
+        folder_name = os.path.relpath(root, root_folder)  # 获取相对于根文件夹的文件夹名称
+        crx_count = sum(1 for file in files if file.endswith('.crx'))  # 统计当前文件夹下的 crx 文件数量
+        rnx_count = sum(1 for file in files if file.endswith('.rnx'))  # 统计当前文件夹下的 rnx 文件数量
+        for file in files:
+            file_path = os.path.join(root, file)
+            file_size_kb = os.path.getsize(file_path) / 1024  # 将文件大小转换为 KB
+            if file_size_kb < 250:  # 如果文件大小小于 250KB
+                small_file_count += 1
+        folder_file_count[folder_name] = {'crx': crx_count, 'rnx': rnx_count, 'small_files': small_file_count}  # 将文件夹名称及其文件数量添加到字典中
+    return folder_file_count
+
+def count_files_in_folders_version2(root_folder: str) -> dict:
+    start_time_count = {}  # 在循环外部定义 start_time_count
+    for root, _, files in os.walk(root_folder):
+        directory_path = os.path.relpath(root, root_folder)
+        for file_name in files:
+            if file_name.endswith(".rnx"):
+                file_path = os.path.join(directory_path, file_name)
+                rnx_file = RinexFileInfo(file_path, ftp_file=False)
+                start_time = rnx_file.start_gps_time_str
+                if start_time in start_time_count:
+                    start_time_count[start_time].append(file_name)
+                else:
+                    start_time_count[start_time] = [file_name]
+        
+    # 检查是否存在相同的 start_gps_time_str
+    for start_time, files in start_time_count.items():
+        if len(files) < 6:
+            print(f"For start_gps_time_str: {start_time}, there is <6 file ")
+
+
+def delete_small_files(directory_path: str, threshold_size: float) -> None:
+    for file_name in os.listdir(directory_path):
+        file_path = os.path.join(directory_path, file_name)
+        file_size_bytes = os.path.getsize(file_path)
+        file_size_kb = file_size_bytes / 1024  # 将文件大小转换为 KB
+        if file_size_kb < threshold_size:
+            os.remove(file_path)  # 删除文件
```

## Comparing `JayttleProcess-0.2.3.dist-info/METADATA` & `JayttleProcess-0.2.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: JayttleProcess
-Version: 0.2.3
-Summary: modifty time:2024-04-24 10:35
+Version: 0.2.4
+Summary: modifty time:2024-04-24 14:25
  en: Data Process;
  zh_CN:数据处理的方法
 Home-page: UNKNOWN
 Author: Jayttle
 Author-email: 294448068@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
```

## Comparing `JayttleProcess-0.2.3.dist-info/RECORD` & `JayttleProcess-0.2.4.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 JayttleProcess/CommonDecorator.py,sha256=ES7hIDpAL3zhzpJYEXlgG4_LGvDsBoJqgIcruJiIr9A,2978
-JayttleProcess/ComputerControl.py,sha256=kUsJJmW2U_rY2SXiHGZ1_baRFfSL40F5PoWpmawofPE,10691
+JayttleProcess/ComputerControl.py,sha256=G-MGLHPKLXxTC1uv6KSqL2A3BjcSSUt7t5DbsoZaYgc,10765
 JayttleProcess/EntertainmentCode.py,sha256=KR-nFHjwIjfl8E_IMuRl44p2Xwkw6UMZYuvkdL9NFck,613
 JayttleProcess/FTPCommonUse.py,sha256=gpniZo2IAqyOWsuqh3NIsZ0ON6vfAHJBcIR3tVLX7zs,6780
 JayttleProcess/JsonCommonManage.py,sha256=KJtfAxPUGktFMocoFKFd8E_VtGW-vyhAMPPz--34mkA,5650
-JayttleProcess/RinexCommonManage.py,sha256=4LxiF_DKccS01OkQidPgDwRkgJukjU2VyIlekHvMifo,36633
+JayttleProcess/RinexCommonManage.py,sha256=aVh91byZDlpmc0q8WKjTT-qxjYTvEHMU2ItfpRMB9NE,39588
 JayttleProcess/SQLCommonUse.py,sha256=w7mOwUQ81MyXjg8NP_vYs7trLTF0_3H5B-CXL4AqPhw,32805
 JayttleProcess/TimeSeriesDataMethod.py,sha256=HUmf2RjkcNRAcjS4XkTwDqQNc-6mGhVcufjGo82D4rk,117788
 JayttleProcess/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-JayttleProcess-0.2.3.dist-info/METADATA,sha256=2l7g2m24U4dF--J2gKXSBFs3Lneqg1xmYIBDQbnt3Hc,554
-JayttleProcess-0.2.3.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-JayttleProcess-0.2.3.dist-info/top_level.txt,sha256=0wohZ9zSz5j0d_abN3JTtoTUIvlCsfp-LHIP_NcoOlw,15
-JayttleProcess-0.2.3.dist-info/RECORD,,
+JayttleProcess-0.2.4.dist-info/METADATA,sha256=RWHMqFuuwkiHQIehvYQMo4kBMT7_G7URXI8CVO6tQPg,554
+JayttleProcess-0.2.4.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+JayttleProcess-0.2.4.dist-info/top_level.txt,sha256=0wohZ9zSz5j0d_abN3JTtoTUIvlCsfp-LHIP_NcoOlw,15
+JayttleProcess-0.2.4.dist-info/RECORD,,
```

