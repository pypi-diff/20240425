# Comparing `tmp/CTkMenuBar-0.4.tar.gz` & `tmp/ctkmenubar-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CTkMenuBar-0.4.tar", last modified: Mon Mar 25 11:33:45 2024, max compression
+gzip compressed data, was "ctkmenubar-0.5.tar", last modified: Thu Apr 25 09:56:52 2024, max compression
```

## Comparing `CTkMenuBar-0.4.tar` & `ctkmenubar-0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-03-25 11:33:45.196370 CTkMenuBar-0.4/
-drwxrwxrwx   0        0        0        0 2024-03-25 11:33:45.174370 CTkMenuBar-0.4/CTkMenuBar/
--rw-rw-rw-   0        0        0      269 2024-03-25 11:07:02.000000 CTkMenuBar-0.4/CTkMenuBar/__init__.py
--rw-rw-rw-   0        0        0    11371 2024-03-25 11:17:30.000000 CTkMenuBar-0.4/CTkMenuBar/dropdown_menu.py
--rw-rw-rw-   0        0        0     2184 2024-03-25 11:25:04.000000 CTkMenuBar-0.4/CTkMenuBar/menu_bar.py
--rw-rw-rw-   0        0        0     4474 2024-03-25 11:33:03.000000 CTkMenuBar-0.4/CTkMenuBar/title_menu_win.py
-drwxrwxrwx   0        0        0        0 2024-03-25 11:33:45.193368 CTkMenuBar-0.4/CTkMenuBar.egg-info/
--rw-rw-rw-   0        0        0     4491 2024-03-25 11:33:45.000000 CTkMenuBar-0.4/CTkMenuBar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2024-03-25 11:33:45.000000 CTkMenuBar-0.4/CTkMenuBar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       40 2024-03-25 11:33:45.000000 CTkMenuBar-0.4/CTkMenuBar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-03-25 11:33:45.000000 CTkMenuBar-0.4/CTkMenuBar.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-25 11:33:45.000000 CTkMenuBar-0.4/CTkMenuBar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7048 2022-11-20 16:16:56.000000 CTkMenuBar-0.4/LICENSE
--rw-rw-rw-   0        0        0     4491 2024-03-25 11:33:45.195368 CTkMenuBar-0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3769 2024-03-25 11:15:27.000000 CTkMenuBar-0.4/README.md
--rw-rw-rw-   0        0        0      582 2024-03-25 11:33:45.198371 CTkMenuBar-0.4/setup.cfg
--rw-rw-rw-   0        0        0     1129 2024-03-25 11:15:40.000000 CTkMenuBar-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 09:56:52.307766 ctkmenubar-0.5/
+drwxrwxrwx   0        0        0        0 2024-04-25 09:56:52.279204 ctkmenubar-0.5/CTkMenuBar/
+-rw-rw-rw-   0        0        0      269 2024-04-25 09:51:53.000000 ctkmenubar-0.5/CTkMenuBar/__init__.py
+-rw-rw-rw-   0        0        0    11782 2024-04-25 09:55:15.000000 ctkmenubar-0.5/CTkMenuBar/dropdown_menu.py
+-rw-rw-rw-   0        0        0     2184 2024-03-25 11:25:04.000000 ctkmenubar-0.5/CTkMenuBar/menu_bar.py
+-rw-rw-rw-   0        0        0     4474 2024-03-25 11:33:03.000000 ctkmenubar-0.5/CTkMenuBar/title_menu_win.py
+drwxrwxrwx   0        0        0        0 2024-04-25 09:56:52.305244 ctkmenubar-0.5/CTkMenuBar.egg-info/
+-rw-rw-rw-   0        0        0     4491 2024-04-25 09:56:52.000000 ctkmenubar-0.5/CTkMenuBar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      308 2024-04-25 09:56:52.000000 ctkmenubar-0.5/CTkMenuBar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       40 2024-04-25 09:56:52.000000 ctkmenubar-0.5/CTkMenuBar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-25 09:56:52.000000 ctkmenubar-0.5/CTkMenuBar.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-25 09:56:52.000000 ctkmenubar-0.5/CTkMenuBar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7048 2022-11-20 16:16:56.000000 ctkmenubar-0.5/LICENSE
+-rw-rw-rw-   0        0        0     4491 2024-04-25 09:56:52.306752 ctkmenubar-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3769 2024-03-25 11:15:27.000000 ctkmenubar-0.5/README.md
+-rw-rw-rw-   0        0        0      582 2024-04-25 09:56:52.310761 ctkmenubar-0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1129 2024-04-25 09:52:12.000000 ctkmenubar-0.5/setup.py
```

### Comparing `CTkMenuBar-0.4/CTkMenuBar/dropdown_menu.py` & `ctkmenubar-0.5/CTkMenuBar/dropdown_menu.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,15 +98,15 @@
             width = self.width,
             height = self.height,
             text=option,
             anchor="w",
             text_color=self.text_color,
             command=partial(self.selectOption, command), **kwargs)
         optionButton.configure(cursor=self.cursor)
-        
+                          
         optionButton.setParentMenu(self)
         self._options_list.append(optionButton)
         self._configureButton(optionButton)
 
         optionButton.pack(
             side="top",
             fill="both", 
@@ -137,35 +137,46 @@
             separator_color=self.separator_color,
             text_color=self.text_color,
             font=self.font)
         
         submenuButtonSeed.setSubmenu(submenu=submenu)
         submenuButtonSeed.configure(command=submenu.toggleShow)
         submenu.bind("<Enter>", lambda e: submenu._show_submenu(self, hovered=True))
+        
+        self.after(300, self.update)
+            
         submenuButtonSeed.bind("<Enter>", lambda e: self.after(500, lambda: submenu._show_submenu(self)))
-        submenuButtonSeed.bind("<Leave>", lambda e: self.after(500, lambda: submenu._left(self)))
+        submenuButtonSeed.bind("<Leave>", lambda e: self.after(500, lambda: submenu._left(self)), add="+")
         submenuButtonSeed.configure(cursor=self.cursor)
         
         submenuButtonSeed.pack(
             side="top",
             fill="both", 
             expand=True,
             padx=3+(self.corner_radius/5),
             pady=3+(self.corner_radius/5))
         return submenu
-
+    
+    def update(self):
+        subMenus = self._getSubMenus()
+        for submenu in subMenus:
+            for widget in submenu.winfo_children():
+                widget.bind("<Enter>", lambda e, submenu=submenu: submenu._show_submenu(self, hovered=True))
+            
     def _left(self, parent):
         if parent.hovered:
             return
+        
         subMenus = parent._getSubMenus()
         
         for i in subMenus:
             i._hide()
 
     def _show_submenu(self, parent, hovered=False) ->None:
+    
         parent.hovered = hovered
         
         subMenus = parent._getSubMenus()
         
         for i in subMenus:
             i._hide()
 
@@ -223,26 +234,28 @@
     def _collapseSiblingSubmenus(self, button: _CDMOptionButton | _CDMSubmenuButton, *args, **kwargs) -> None:
         for option in self._options_list:
             if option != button and isinstance(option, _CDMSubmenuButton):
                 option.submenu._hideChildrenMenus()
                 option.submenu._hide()
 
     def toggleShow(self, *args, **kwargs) -> None:
+    
         widget_base = self.menu_seed_object.master.winfo_name()
         if widget_base.startswith("!ctktitlemenu") or widget_base.startswith("!ctkmenubar"):
             for i in self.menu_seed_object.master.menu:
-                i._hide()
-            
-        if not self.winfo_manager():
+                if i!=self:
+                    i._hide()
+    
+        if not self.winfo_viewable():
             self._show()
             self.lift()
         else:
             self._hideChildrenMenus()
             self._hide()
-                
+            
     def _configureButton(self, button: customtkinter.CTkButton) -> None:
         button.configure(fg_color="transparent")
         if self.fg_color:
             button.configure(fg_color=self.fg_color)
         if self.hover_color:
             button.configure(hover_color=self.hover_color)
         if self.font:
```

### Comparing `CTkMenuBar-0.4/CTkMenuBar/menu_bar.py` & `ctkmenubar-0.5/CTkMenuBar/menu_bar.py`

 * *Files identical despite different names*

### Comparing `CTkMenuBar-0.4/CTkMenuBar/title_menu_win.py` & `ctkmenubar-0.5/CTkMenuBar/title_menu_win.py`

 * *Files identical despite different names*

### Comparing `CTkMenuBar-0.4/CTkMenuBar.egg-info/PKG-INFO` & `ctkmenubar-0.5/CTkMenuBar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTkMenuBar
-Version: 0.4
+Version: 0.5
 Summary: Customtkinter Menu Widget
 Home-page: https://github.com/Akascape/CTkMenuBar
 Author: Akash Bora
 License: Creative Commons Zero v1.0 Universal
 Keywords: customtkinter,customtkinter-menu,ctkmenubar,titlemenu,menubar,tkinter,menu-widget,tkinter-gui
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CTkMenuBar-0.4/LICENSE` & `ctkmenubar-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `CTkMenuBar-0.4/PKG-INFO` & `ctkmenubar-0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTkMenuBar
-Version: 0.4
+Version: 0.5
 Summary: Customtkinter Menu Widget
 Home-page: https://github.com/Akascape/CTkMenuBar
 Author: Akash Bora
 License: Creative Commons Zero v1.0 Universal
 Keywords: customtkinter,customtkinter-menu,ctkmenubar,titlemenu,menubar,tkinter,menu-widget,tkinter-gui
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CTkMenuBar-0.4/README.md` & `ctkmenubar-0.5/README.md`

 * *Files identical despite different names*

### Comparing `CTkMenuBar-0.4/setup.cfg` & `ctkmenubar-0.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2043 546b 4d65 6e75 4261 720d 0a76   = CTkMenuBar..v
-00000020: 6572 7369 6f6e 203d 2030 2e34 0d0a 6465  ersion = 0.4..de
+00000020: 6572 7369 6f6e 203d 2030 2e35 0d0a 6465  ersion = 0.5..de
 00000030: 7363 7269 7074 696f 6e20 3d20 4375 7374  scription = Cust
 00000040: 6f6d 746b 696e 7465 7220 4d65 6e75 2057  omtkinter Menu W
 00000050: 6964 6765 740d 0a6c 6f6e 675f 6465 7363  idget..long_desc
 00000060: 7269 7074 696f 6e20 3d20 6669 6c65 3a20  ription = file: 
 00000070: 5245 4144 4d45 2e6d 640d 0a6c 6f6e 675f  README.md..long_
 00000080: 6465 7363 7269 7074 696f 6e5f 636f 6e74  description_cont
 00000090: 656e 745f 7479 7065 203d 2074 6578 742f  ent_type = text/
```

### Comparing `CTkMenuBar-0.4/setup.py` & `ctkmenubar-0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     """Opens and fetches text of long descrition file."""
     with open(path, 'r') as f:
         text = f.read()
     return text
 
 setup(
     name = 'CTkMenuBar',
-    version = '0.4',
+    version = '0.5',
     description = "Customtkinter Menu Widget",
     license = "Creative Commons Zero v1.0 Universal",
     readme = "README.md",
     long_description = get_long_description('README.md'),
     long_description_content_type = "text/markdown",
     author = 'Akash Bora',
     url = "https://github.com/Akascape/CTkMenuBar",
```

