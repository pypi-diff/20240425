# Comparing `tmp/CTkListbox-1.3.tar.gz` & `tmp/ctklistbox-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CTkListbox-1.3.tar", last modified: Mon Feb 12 11:35:39 2024, max compression
+gzip compressed data, was "ctklistbox-1.4.tar", last modified: Thu Apr 25 13:06:15 2024, max compression
```

## Comparing `CTkListbox-1.3.tar` & `ctklistbox-1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-02-12 11:35:39.294264 CTkListbox-1.3/
-drwxrwxrwx   0        0        0        0 2024-02-12 11:35:39.267554 CTkListbox-1.3/CTkListbox/
--rw-rw-rw-   0        0        0      190 2024-01-08 14:53:43.000000 CTkListbox-1.3/CTkListbox/__init__.py
--rw-rw-rw-   0        0        0    15064 2024-02-12 11:13:16.000000 CTkListbox-1.3/CTkListbox/ctk_listbox.py
-drwxrwxrwx   0        0        0        0 2024-02-12 11:35:39.290861 CTkListbox-1.3/CTkListbox.egg-info/
--rw-rw-rw-   0        0        0     3206 2024-02-12 11:35:39.000000 CTkListbox-1.3/CTkListbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2024-02-12 11:35:39.000000 CTkListbox-1.3/CTkListbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       40 2024-02-12 11:35:39.000000 CTkListbox-1.3/CTkListbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-02-12 11:35:39.000000 CTkListbox-1.3/CTkListbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-02-12 11:35:39.000000 CTkListbox-1.3/CTkListbox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1067 2024-01-08 14:34:16.000000 CTkListbox-1.3/LICENSE
--rw-rw-rw-   0        0        0     3206 2024-02-12 11:35:39.290861 CTkListbox-1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2577 2024-02-12 11:34:37.000000 CTkListbox-1.3/README.md
--rw-rw-rw-   0        0        0      527 2024-02-12 11:35:39.294264 CTkListbox-1.3/setup.cfg
--rw-rw-rw-   0        0        0     1056 2024-02-12 10:45:48.000000 CTkListbox-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:06:15.629718 ctklistbox-1.4/
+drwxrwxrwx   0        0        0        0 2024-04-25 13:06:15.598470 ctklistbox-1.4/CTkListbox/
+-rw-rw-rw-   0        0        0      190 2024-04-25 12:48:05.000000 ctklistbox-1.4/CTkListbox/__init__.py
+-rw-rw-rw-   0        0        0    15541 2024-04-25 13:05:19.000000 ctklistbox-1.4/CTkListbox/ctk_listbox.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:06:15.614094 ctklistbox-1.4/CTkListbox.egg-info/
+-rw-rw-rw-   0        0        0     3206 2024-04-25 13:06:15.000000 ctklistbox-1.4/CTkListbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2024-04-25 13:06:15.000000 ctklistbox-1.4/CTkListbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       40 2024-04-25 13:06:15.000000 ctklistbox-1.4/CTkListbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-25 13:06:15.000000 ctklistbox-1.4/CTkListbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-25 13:06:15.000000 ctklistbox-1.4/CTkListbox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1067 2024-01-08 14:34:16.000000 ctklistbox-1.4/LICENSE
+-rw-rw-rw-   0        0        0     3206 2024-04-25 13:06:15.629718 ctklistbox-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2578 2024-04-25 12:48:50.000000 ctklistbox-1.4/README.md
+-rw-rw-rw-   0        0        0      527 2024-04-25 13:06:15.629718 ctklistbox-1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1056 2024-04-25 12:50:54.000000 ctklistbox-1.4/setup.py
```

### Comparing `CTkListbox-1.3/CTkListbox/ctk_listbox.py` & `ctklistbox-1.4/CTkListbox/ctk_listbox.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
         self.select_color = (
             customtkinter.ThemeManager.theme["CTkButton"]["fg_color"]
             if highlight_color == "default"
             else highlight_color
         )
         self.text_color = (
-            customtkinter.ThemeManager.theme["CTkButton"]["text_color"]
+            customtkinter.ThemeManager.theme["CTkLabel"]["text_color"]
             if text_color == "default"
             else text_color
         )
         self.hover_color = (
             customtkinter.ThemeManager.theme["CTkButton"]["hover_color"]
             if hover_color == "default"
             else hover_color
@@ -79,14 +79,15 @@
         self.multiple = multiple_selection
         self.selected = None
         self.hover = hover
         self.end_num = 0
         self.selections = []
         self.selected_index = 0
         self._scrollbar.configure(height=height)
+        self.columnconfigure(0, weight=1)
         
         if listvariable:
             self.listvariable = listvariable
             self.listvariable.trace_add("write", lambda a, b, c: self.update_listvar())
             self.update_listvar()
 
     def update_listvar(self):
@@ -166,34 +167,38 @@
     def unbind(self, key):
         super().unbind(key)
         self._parent_frame.unbind(key)
         self._parent_canvas.unbind(key)
         
     def deselect(self, index):
         if not self.multiple:
-            self.selected.configure(fg_color=self.button_fg_color)
-            self.selected = None
-            return
+            if self.selected:
+                self.selected.configure(fg_color=self.button_fg_color)
+                self.selected = None
+                return
         if self.buttons[index] in self.selections:
             self.selections.remove(self.buttons[index])
             self.buttons[index].configure(fg_color=self.button_fg_color)
 
     def deactivate(self, index):
         if str(index).lower() == "all":
-            for i in self.buttons:
-                self.deselect(i)
+            if self.multiple:
+                for i in self.buttons:
+                    self.deselect(i)
+            else:
+                self.deselect(0)
             return
-
+        
         if str(index).lower() == "end":
             index = -1
 
         selected = list(self.buttons.keys())[index]
         self.deselect(selected)
 
-    def insert(self, index, option, **args):
+    def insert(self, index, option, update=True, **args):
         """add new option in the listbox"""
 
         if str(index).lower() == "end":
             index = f"END{self.end_num}"
             self.end_num += 1
 
         if index in self.buttons:
@@ -206,24 +211,30 @@
             anchor=self.justify,
             text_color=self.text_color,
             font=self.font,
             hover_color=self.hover_color,
             **args,
         )
         self.buttons[index].configure(command=lambda num=index: self.select(num))
-        self.buttons[index].pack(padx=0, pady=(0, 5), fill="x", expand=True)
-        self.update()
+        
+        if type(index) is int:
+            self.buttons[index].grid(padx=0, pady=(0, 5), sticky="nsew", column=0, row=index)
+        else:
+            self.buttons[index].grid(padx=0, pady=(0, 5), sticky="nsew", column=0)
+            
+        if update:
+            self.update()
 
         if self.multiple:
             self.buttons[index].bind(
                 "<Shift-1>", lambda e: self.select_multiple(self.buttons[index])
             )
 
         return self.buttons[index]
-
+        
     def select_multiple(self, button):
         selections = list(self.buttons.values())
         if len(self.selections) > 0:
             last = selections.index(self.selections[-1])
             to = selections.index(button)
 
             if last < to:
@@ -242,16 +253,18 @@
         
         self._parent_frame.destroy()
         self._parent_canvas.destroy()
         
     def delete(self, index, last=None):
         """delete options from the listbox"""
         if str(index).lower() == "all":
+            self.deactivate("all")
             for i in self.buttons:
                 self.buttons[i].destroy()
+                self.update()
             self.buttons = {}
             self.end_num = 0
             return
 
         if str(index).lower() == "end":
             self.end_num -= 1
             if len(self.buttons.keys())>0:
@@ -279,15 +292,15 @@
                 del self.buttons[i]
         else:
             self.buttons[index].destroy()
             if self.multiple:
                 if self.buttons[index] in self.selections:
                     self.selections.remove(self.buttons[index])
             del self.buttons[index]
-
+        
     def size(self):
         """return total number of items in the listbox"""
         return len(self.buttons.keys())
 
     def get(self, index=None):
         """get the selected value"""
         if index is not None:
```

### Comparing `CTkListbox-1.3/CTkListbox.egg-info/PKG-INFO` & `ctklistbox-1.4/CTkListbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTkListbox
-Version: 1.3
+Version: 1.4
 Summary: Customtkinter Listbox widget
 Home-page: https://github.com/Akascape/CTkListbox
 Author: Akash Bora
 License: MIT
 Keywords: customtkinter,tkinter,listbox-widget,listbox,modern-listbox,option menu,list-box,ctklistbox
 Classifier: License :: OSI Approved :: MIT License 
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CTkListbox-1.3/LICENSE` & `ctklistbox-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `CTkListbox-1.3/PKG-INFO` & `ctklistbox-1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTkListbox
-Version: 1.3
+Version: 1.4
 Summary: Customtkinter Listbox widget
 Home-page: https://github.com/Akascape/CTkListbox
 Author: Akash Bora
 License: MIT
 Keywords: customtkinter,tkinter,listbox-widget,listbox,modern-listbox,option menu,list-box,ctklistbox
 Classifier: License :: OSI Approved :: MIT License 
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CTkListbox-1.3/README.md` & `ctklistbox-1.4/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -69,8 +69,8 @@
 - **.curselection()**
   returns indexes of selected options
 - **.configure()**
    change some parameters for the listbox.
 - **.move_up(index)/.move_down(index)**
    Reorder options in the listbox
   
-### Thanks for visiting! Hope it will help :)
+### Thanks for visiting! Hope it will help :)
```

### Comparing `CTkListbox-1.3/setup.cfg` & `ctklistbox-1.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2043 546b 4c69 7374 626f 780d 0a76   = CTkListbox..v
-00000020: 6572 7369 6f6e 203d 2031 2e33 0d0a 6465  ersion = 1.3..de
+00000020: 6572 7369 6f6e 203d 2031 2e34 0d0a 6465  ersion = 1.4..de
 00000030: 7363 7269 7074 696f 6e20 3d20 4375 7374  scription = Cust
 00000040: 6f6d 746b 696e 7465 7220 4c69 7374 626f  omtkinter Listbo
 00000050: 7820 7769 6467 6574 0d0a 6c6f 6e67 5f64  x widget..long_d
 00000060: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
 00000070: 653a 2052 4541 444d 452e 6d64 0d0a 6c6f  e: README.md..lo
 00000080: 6e67 5f64 6573 6372 6970 7469 6f6e 5f63  ng_description_c
 00000090: 6f6e 7465 6e74 5f74 7970 6520 3d20 7465  ontent_type = te
```

### Comparing `CTkListbox-1.3/setup.py` & `ctklistbox-1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     """Opens and fetches text of long descrition file."""
     with open(path, 'r') as f:
         text = f.read()
     return text
 
 setup(
     name = 'CTkListbox',
-    version = '1.3',
+    version = '1.4',
     description = "Customtkinter Listbox widget",
     license = "MIT",
     readme = "README.md",
     long_description = get_long_description('README.md'),
     long_description_content_type = "text/markdown",
     author = 'Akash Bora',
     url = "https://github.com/Akascape/CTkListbox",
```

