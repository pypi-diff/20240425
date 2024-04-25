# Comparing `tmp/FlowVisor-0.0.3.tar.gz` & `tmp/FlowVisor-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlowVisor-0.0.3.tar", last modified: Tue Apr 23 15:18:35 2024, max compression
+gzip compressed data, was "FlowVisor-0.1.0.tar", last modified: Thu Apr 25 10:37:12 2024, max compression
```

## Comparing `FlowVisor-0.0.3.tar` & `FlowVisor-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,25 @@
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-04-23 15:18:35.474054 FlowVisor-0.0.3/
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-04-23 15:18:35.474054 FlowVisor-0.0.3/FlowVisor.egg-info/
--rw-rw-r--   0 phil      (1000) phil      (1000)     2757 2024-04-23 15:18:35.000000 FlowVisor-0.0.3/FlowVisor.egg-info/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)      311 2024-04-23 15:18:35.000000 FlowVisor-0.0.3/FlowVisor.egg-info/SOURCES.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)        1 2024-04-23 15:18:35.000000 FlowVisor-0.0.3/FlowVisor.egg-info/dependency_links.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       51 2024-04-23 15:18:35.000000 FlowVisor-0.0.3/FlowVisor.egg-info/requires.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       10 2024-04-23 15:18:35.000000 FlowVisor-0.0.3/FlowVisor.egg-info/top_level.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)     1067 2024-04-22 08:55:02.000000 FlowVisor-0.0.3/LICENSE
--rw-rw-r--   0 phil      (1000) phil      (1000)     2757 2024-04-23 15:18:35.474054 FlowVisor-0.0.3/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)     2119 2024-04-23 15:17:49.000000 FlowVisor-0.0.3/README.md
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-04-23 15:18:35.474054 FlowVisor-0.0.3/flowvisor/
--rw-rw-r--   0 phil      (1000) phil      (1000)       87 2024-04-23 14:16:28.000000 FlowVisor-0.0.3/flowvisor/__init__.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     7539 2024-04-23 14:40:02.000000 FlowVisor-0.0.3/flowvisor/flowvisor.py
--rw-rw-r--   0 phil      (1000) phil      (1000)      606 2024-04-22 11:10:52.000000 FlowVisor-0.0.3/flowvisor/flowvisor_config.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     7283 2024-04-23 14:38:39.000000 FlowVisor-0.0.3/flowvisor/function_node.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2368 2024-04-22 10:26:27.000000 FlowVisor-0.0.3/flowvisor/utils.py
--rw-rw-r--   0 phil      (1000) phil      (1000)       38 2024-04-23 15:18:35.474054 FlowVisor-0.0.3/setup.cfg
--rw-rw-r--   0 phil      (1000) phil      (1000)     1002 2024-04-23 15:18:31.000000 FlowVisor-0.0.3/setup.py
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-04-25 10:37:12.300068 FlowVisor-0.1.0/
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-04-25 10:37:12.300068 FlowVisor-0.1.0/FlowVisor.egg-info/
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2800 2024-04-25 10:37:12.000000 FlowVisor-0.1.0/FlowVisor.egg-info/PKG-INFO
+-rw-rw-r--   0 phil      (1000) phil      (1000)      471 2024-04-25 10:37:12.000000 FlowVisor-0.1.0/FlowVisor.egg-info/SOURCES.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)        1 2024-04-25 10:37:12.000000 FlowVisor-0.1.0/FlowVisor.egg-info/dependency_links.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)       99 2024-04-25 10:37:12.000000 FlowVisor-0.1.0/FlowVisor.egg-info/entry_points.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)       52 2024-04-25 10:37:12.000000 FlowVisor-0.1.0/FlowVisor.egg-info/requires.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)       10 2024-04-25 10:37:12.000000 FlowVisor-0.1.0/FlowVisor.egg-info/top_level.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)     1067 2024-04-22 08:55:02.000000 FlowVisor-0.1.0/LICENSE
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2800 2024-04-25 10:37:12.300068 FlowVisor-0.1.0/PKG-INFO
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2119 2024-04-23 15:17:49.000000 FlowVisor-0.1.0/README.md
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-04-25 10:37:12.300068 FlowVisor-0.1.0/flowvisor/
+-rw-rw-r--   0 phil      (1000) phil      (1000)      170 2024-04-25 10:31:59.000000 FlowVisor-0.1.0/flowvisor/__init__.py
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-04-25 10:37:12.300068 FlowVisor-0.1.0/flowvisor/cli/
+-rw-rw-r--   0 phil      (1000) phil      (1000)        0 2024-04-25 10:31:43.000000 FlowVisor-0.1.0/flowvisor/cli/__init__.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3016 2024-04-25 10:17:04.000000 FlowVisor-0.1.0/flowvisor/cli/add_vis.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2080 2024-04-25 10:34:16.000000 FlowVisor-0.1.0/flowvisor/cli/remove_vis.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)    11506 2024-04-25 09:23:49.000000 FlowVisor-0.1.0/flowvisor/flowvisor.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)      838 2024-04-25 09:21:07.000000 FlowVisor-0.1.0/flowvisor/flowvisor_config.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     7439 2024-04-25 09:18:55.000000 FlowVisor-0.1.0/flowvisor/function_node.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2644 2024-04-23 20:23:57.000000 FlowVisor-0.1.0/flowvisor/time_tracker.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)      299 2024-04-23 18:54:33.000000 FlowVisor-0.1.0/flowvisor/timer.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     1386 2024-04-25 09:19:05.000000 FlowVisor-0.1.0/flowvisor/utils.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)       38 2024-04-25 10:37:12.300068 FlowVisor-0.1.0/setup.cfg
+-rw-rw-r--   0 phil      (1000) phil      (1000)     1533 2024-04-25 10:19:31.000000 FlowVisor-0.1.0/setup.py
```

### Comparing `FlowVisor-0.0.3/FlowVisor.egg-info/PKG-INFO` & `FlowVisor-0.1.0/FlowVisor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: FlowVisor
-Version: 0.0.3
-Summary: Visualize the flow of your python code.
+Version: 0.1.0
+Summary: Visualize and profile your python code with FlowVisor.
 Home-page: https://github.com/cophilot/FlowVisor
 Author: cophilot (Philipp B.)
 Author-email: <info@philipp-bonin.com>
 License: MIT
-Keywords: python,flow,visualize,code,flowvisor
+Keywords: python,flow,visualize,code,flowvisor,profiling,profile,decorator
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `FlowVisor-0.0.3/LICENSE` & `FlowVisor-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.0.3/PKG-INFO` & `FlowVisor-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: FlowVisor
-Version: 0.0.3
-Summary: Visualize the flow of your python code.
+Version: 0.1.0
+Summary: Visualize and profile your python code with FlowVisor.
 Home-page: https://github.com/cophilot/FlowVisor
 Author: cophilot (Philipp B.)
 Author-email: <info@philipp-bonin.com>
 License: MIT
-Keywords: python,flow,visualize,code,flowvisor
+Keywords: python,flow,visualize,code,flowvisor,profiling,profile,decorator
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `FlowVisor-0.0.3/README.md` & `FlowVisor-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.0.3/flowvisor/flowvisor.py` & `FlowVisor-0.1.0/flowvisor/flowvisor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,48 @@
 """
 The FlowVisor is a package that visualizes the flow of functions in a codebase.
 """
-import time
+import datetime
 import json
+import timeit
 from typing import List
-from inspect import getmembers, isfunction, ismodule
+#from inspect import getmembers, isfunction, ismodule
 import pickle
-from diagrams import Diagram
+from diagrams import Diagram, Cluster
 from diagrams.custom import Custom
+from flowvisor import utils
 from flowvisor.flowvisor_config import FlowVisorConfig
 from flowvisor.function_node import FunctionNode
+from flowvisor.time_tracker import TimeTracker
 from flowvisor.utils import function_to_id
 
 def vis(func):
     """
     Decorator that visualizes the function.
     """
     def wrapper(*args, **kwargs):
+        TimeTracker.stop()
+        if FlowVisor.CONFIG.reduce_overhead:
+            TimeTracker.apply(advanced=FlowVisor.get_advanced_overhead_reduction())
+            timer_id = TimeTracker.register_new_timer()
+
         FlowVisor.function_called(func)
-        start = time.time()
+
+        start = TimeTracker.start()
         result = func(*args, **kwargs)
-        end = time.time()
-        FlowVisor.function_returned(func, duration=end - start)
+        end = TimeTracker.stop()
+
+        duration = end - start
+        if FlowVisor.CONFIG.reduce_overhead:
+            TimeTracker.apply(advanced=FlowVisor.get_advanced_overhead_reduction())
+            duration = TimeTracker.get_time_and_remove_timer(timer_id)
+
+        FlowVisor.function_returned(func, duration)
+        
+        TimeTracker.start()
         return result
     return wrapper
 
 class FlowVisor:
     """
     The FlowVisor class is responsible for managing the flow of the functions 
     and generating the graph.
@@ -86,88 +103,137 @@
     def get_called_nodes_only():
         """
         Returns only the nodes that have been called.
         """
         return [node for node in FlowVisor.NODES if node.called > 0]
 
     @staticmethod
-    def generate_graph():
+    def graph():
         """
         Generates the graph.
         """
-        highest_time = 0
+        highest_time = -1
         called_nodes = FlowVisor.get_called_nodes_only()
         for node in called_nodes:
             if node.time > highest_time:
                 highest_time = node.time
 
         try:
-            FunctionNode.make_node_image_cache()
             with Diagram(FlowVisor.CONFIG.graph_title,
                          show=FlowVisor.CONFIG.show_graph,
                          filename=FlowVisor.CONFIG.output_file,
                          direction="LR"):
-                # Add logo
+
+                FunctionNode.make_node_image_cache()
+
+                if FlowVisor.CONFIG.add_timestamp:
+                    timestamp = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
+                    Custom(str(timestamp), "", width="0.001", height="0.001")
+
                 if FlowVisor.CONFIG.logo != "":
                     Custom("", FlowVisor.CONFIG.logo,
                            width=FlowVisor.CONFIG.get_node_scale(),
                            height=FlowVisor.CONFIG.get_node_scale())
 
                 # Draw nodes
-                for r in called_nodes:
-                    FlowVisor.draw_function_node(r, highest_time)
+                if FlowVisor.CONFIG.group_nodes:
+                    FlowVisor.draw_nodes_with_cluster(called_nodes, highest_time)
+                else:
+                    for n in called_nodes:
+                        FlowVisor.draw_function_node(n, highest_time)
+
         finally:
+            # Make sure to clear the cache always
             FunctionNode.clear_node_image_cache()
 
     @staticmethod
+    def draw_nodes_with_cluster(nodes: List[FunctionNode], highest_time: float):
+        """
+        Draws the nodes with cluster.
+        """
+        sorted_nodes = FlowVisor.get_node_sorted_by_filename(nodes)
+        total_times = [sum([n.time for n in row]) for row in sorted_nodes]
+        highest_time_file_time = max(total_times)
+        for index, row in enumerate(sorted_nodes):
+            cluster_title = f"{row[0].file_name} ({utils.get_time_as_string(total_times[index])})"
+            bg_color = utils.value_to_hex_color(total_times[index], highest_time_file_time,
+                                                light_color=[0xFF, 0xFF, 0xFF],
+                                                dark_color=[0xAA, 0xAA, 0xAA])
+            font_color = utils.value_to_hex_color(total_times[index], highest_time_file_time,
+                                                light_color=[0x00, 0x00, 0x00],
+                                                dark_color=[0xFF, 0xFF, 0xFF])
+            with Cluster(cluster_title, graph_attr={"bgcolor": bg_color, "fontcolor": font_color}):
+                for n in row:
+                    FlowVisor.draw_function_node(n, highest_time)
+
+    @staticmethod
+    def get_node_sorted_by_filename(nodes: List[FunctionNode]):
+        """
+        Returns the nodes sorted by filename.
+        """
+        file_names = []
+        for node in nodes:
+            if node.file_path not in file_names:
+                file_names.append(node.file_path)
+
+        result = []
+        for file_name in file_names:
+            row = []
+            for node in nodes:
+                if node.file_path == file_name:
+                    row.append(node)
+            result.append(row)
+        return result
+
+    @staticmethod
     def get_nodes_as_dict():
         """
         Returns the nodes as a dictionary.
         """
         return [node.to_dict() for node in FlowVisor.NODES]
 
     @staticmethod
-    def save_flow(file: str, type = "pickle"):
+    def export(file: str, export_type = "pickle"):
         """
         Saves the flow to a file.
         """
         nodes_dict = FlowVisor.get_nodes_as_dict()
-        if type == "json":
+        if export_type == "json":
             if not file.endswith(".json"):
                 file += ".json"
             with open(file, "w", encoding="utf-8") as f:
                 json.dump(nodes_dict, f, indent=4)
-        if type == "pickle":
+        if export_type == "pickle":
             if not file.endswith(".pickle"):
                 file += ".pickle"
             with open(file, "wb") as f:
                 pickle.dump(nodes_dict, f)
 
     @staticmethod
-    def generate_graph_from_file(file: str):
+    def generate_graph(file: str = ""):
         """
         Generates the graph from a file.
         """
         mode = "pickle"
         if file.endswith(".json"):
             mode = "json"
         if mode == "json":
             with open(file, "r", encoding="utf-8") as f:
                 raw_nodes = json.load(f)
         else:
             with open(file, "rb") as f:
                 raw_nodes = pickle.load(f)
-        
+
         for n in raw_nodes:
             node = FunctionNode.from_dict(n)
             FlowVisor.NODES.append(node)
         for node in FlowVisor.NODES:
             node.resolve_children_ids(FlowVisor.NODES)
-        
-        FlowVisor.generate_graph()
+
+        FlowVisor.graph()
 
     @staticmethod
     def draw_function_node(func_node: FunctionNode, highest_time):
         """
         Draws the function node.
         """
         node = func_node.get_as_diagram_node(highest_time, FlowVisor.CONFIG)
@@ -197,14 +263,61 @@
     def set_exclude_functions(exclude_functions: List[str]):
         """
         Sets the exclude functions.
         """
         FlowVisor.EXCLUDE_FUNCTIONS = exclude_functions
 
     @staticmethod
+    def is_stack_empty():
+        """
+        Checks if the stack is empty.
+        """
+        return len(FlowVisor.STACK) == 0
+
+    @staticmethod
+    def enable_advanced_overhead_reduction():
+        """
+        Enables advanced overhead reduction.
+        """
+        n = 50000
+        t = timeit.timeit(setup="import time", stmt="time.time()", number=n)
+        mean = t / n
+        print(f"Mean time for time.time() is: {utils.get_time_as_string(mean)}")
+        FlowVisor.CONFIG.advanced_overhead_reduction = mean
+
+    @staticmethod
+    def disable_advanced_overhead_reduction():
+        """
+        Disables advanced overhead reduction.
+        """
+        FlowVisor.CONFIG.advanced_overhead_reduction = None
+
+    @staticmethod
+    def get_advanced_overhead_reduction():
+        """
+        Gets the advanced overhead reduction.
+        """
+        return FlowVisor.CONFIG.advanced_overhead_reduction
+
+    @staticmethod
+    def enable_dev_mode():
+        """
+        Enables the dev mode.
+        """
+        FlowVisor.CONFIG.dev_mode = True
+
+    @staticmethod
+    def set_config(config: FlowVisorConfig):
+        """
+        Sets the configuration.
+        """
+        FlowVisor.CONFIG = config
+
+    '''
+    @staticmethod
     def visualize_all():
         """
         Visualizes all the functions in this project.
         """
         FlowVisor.visualize_module_by_name("__main__")
 
     @staticmethod
@@ -215,15 +328,15 @@
         module = __import__(module_name)
 
         FlowVisor.visualize_module(module)
 
     @staticmethod
     def visualize_module(module: object):
         FlowVisor.visualize_module_helper(module, [])
-    
+
     @staticmethod
     def visualize_module_helper(module: object, added_modules):
         """
         Visualizes all the functions in a module.
         """
         print("This function is still buggy and will not work as expected. Workin on it!")
         for name, obj in getmembers(module, isfunction):
@@ -239,7 +352,8 @@
         #        continue
         #    added_modules.append(sub_module.__name__)
         #    print(f"Visualizing module: {sub_module.__name__}")
         #    # write to a file
         #    with open(f"log.txt", "a") as f:
         #        f.write(f"Visualizing module: {sub_module.__name__}\n")
         #    FlowVisor.visualize_module_helper(sub_module, added_modules)
+    '''
```

### Comparing `FlowVisor-0.0.3/flowvisor/flowvisor_config.py` & `FlowVisor-0.1.0/flowvisor/flowvisor_config.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """
+Configuration class for FlowVisor
 """
 class FlowVisorConfig:
     """
     Configuration class for FlowVisor
     """
 
     def __init__(self):
@@ -11,13 +12,18 @@
         self.output_file: str = "function_flow"
         self.graph_title: str = ""
         self.node_scale: float = 2.0
         self.node_show_file: bool = True
         self.node_show_call_count: bool = True
         self.node_show_avg_time: bool = True
         self.static_font_color: str = ""
-        
+        self.reduce_overhead: bool = True
+        self.add_timestamp: bool = False
+        self.advanced_overhead_reduction = None
+        self.group_nodes: bool = False
+        self.dev_mode: bool = False
+
     def get_node_scale(self):
         """
         Get the node scale as a string
         """
         return str(self.node_scale)
```

### Comparing `FlowVisor-0.0.3/flowvisor/function_node.py` & `FlowVisor-0.1.0/flowvisor/function_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,30 +64,32 @@
             self.generate_diagram_node(highest_time, config)
         return self.diagram_node
 
     def generate_diagram_node(self,highest_time: float, config: FlowVisorConfig):
         """
         Generates the diagram node.
         """
-        circle_file = self.export_node_image(highest_time)
+        node_image = self.export_node_image(highest_time)
 
         size = self.time / highest_time
         if size < 0.1:
             size = 0.1
 
         size = 1
         size = size * config.node_scale
 
         title = self.get_node_title(config)
 
         font_color = config.static_font_color
         if font_color == "":
-            font_color = utils.font_color_to_hex_color(self.time, highest_time)
+            font_color = utils.value_to_hex_color(self.time, highest_time,
+                                                  dark_color=[0xFF, 0xC0, 0x82],
+                                                  light_color=[0x00, 0x00, 0x00])
 
-        self.diagram_node = Custom(title, circle_file,
+        self.diagram_node = Custom(title, node_image,
                                    width=str(size),
                                    height=str(size),
                                    fontcolor=font_color)
 
     def get_node_title(self, config: FlowVisorConfig):
         """
         Returns the title of the node, that is displayed in the diagram.
```

### Comparing `FlowVisor-0.0.3/flowvisor/utils.py` & `FlowVisor-0.1.0/flowvisor/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -28,54 +28,28 @@
 
     nanoseconds = int(t * 1000000000)
     if nanoseconds > 0:
         return f"{nanoseconds}ns"
 
     return "<1ns"
 
-def value_to_hex_color(value, max_value):
+def value_to_hex_color(value, max_value, light_color = [0xA9, 0xF3, 0xF9], dark_color = [0x00, 0x1F, 0x3F]):
+    """
+    Return a hexadecimal color code based on the value and max_value
+    """
     # Ensure value is within range [0, max_value]
     value = max(0, min(value, max_value))
-    
-    # Interpolate between light blue (#a9f3f9) and dark blue (#00008B)
-    light_blue = [0xA9, 0xF3, 0xF9]  # RGB values for light blue
-    dark_blue = [0x00, 0x1F, 0x3F]    # RGB values for dark blue
-    
-    # Calculate interpolation factors
-    ratio = value / max_value
-    inv_ratio = 1 - ratio
-    
-    # Interpolate RGB values
-    interpolated_color = [
-        int(light_blue[i] * inv_ratio + dark_blue[i] * ratio)
-        for i in range(3)
-    ]
-    
-    # Convert interpolated RGB values to hexadecimal color code
-    hex_color = '#{:02X}{:02X}{:02X}'.format(*interpolated_color)
-    
-    return hex_color
 
-def font_color_to_hex_color(value, max_value):
-    # Ensure value is within range [0, max_value]
-    value = max(0, min(value, max_value))
-    
-    # Interpolate between light orange (#ffc082) and dark orange (#6b3500)
-    light_orange = [0xFF, 0xFF, 0xFF]  # RGB values for light orange
-    dark_orange = [0x6B, 0x35, 0x00]    # RGB values for dark orange
-    light_orange = [0xFF, 0xC0, 0x82]  # RGB values for light orange
-    dark_orange = [0x00, 0x00, 0x00]    # RGB values for dark orange
-    
     # Calculate interpolation factors
     ratio = value / max_value
     inv_ratio = 1 - ratio
-    
+
     # Interpolate RGB values
     interpolated_color = [
-        int(dark_orange[i] * inv_ratio + light_orange[i] * ratio)
+        int(light_color[i] * inv_ratio + dark_color[i] * ratio)
         for i in range(3)
     ]
-    
+
     # Convert interpolated RGB values to hexadecimal color code
     hex_color = '#{:02X}{:02X}{:02X}'.format(*interpolated_color)
-    
-    return hex_color
+
+    return hex_color
```

