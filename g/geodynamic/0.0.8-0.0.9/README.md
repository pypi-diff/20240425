# Comparing `tmp/geodynamic-0.0.8.tar.gz` & `tmp/geodynamic-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geodynamic-0.0.8.tar", last modified: Sun Apr 21 11:52:53 2024, max compression
+gzip compressed data, was "geodynamic-0.0.9.tar", last modified: Tue Apr 23 14:09:10 2024, max compression
```

## Comparing `geodynamic-0.0.8.tar` & `geodynamic-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-21 11:52:53.938582 geodynamic-0.0.8/
--rw-r--r--   0 mac        (501) staff       (20)       18 2024-04-05 12:40:59.000000 geodynamic-0.0.8/LICENSE.txt
--rw-r--r--   0 mac        (501) staff       (20)     1099 2024-04-21 11:52:53.938467 geodynamic-0.0.8/PKG-INFO
--rw-------   0 mac        (501) staff       (20)      428 2024-04-18 12:05:16.000000 geodynamic-0.0.8/README.md
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-21 11:52:53.929474 geodynamic-0.0.8/geodynamic/
--rw-------   0 mac        (501) staff       (20)        0 2024-04-05 11:31:09.000000 geodynamic-0.0.8/geodynamic/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-21 11:52:53.933766 geodynamic-0.0.8/geodynamic/geo/
--rw-------   0 mac        (501) staff       (20)        0 2023-12-28 13:25:09.000000 geodynamic-0.0.8/geodynamic/geo/__init__.py
--rw-------   0 mac        (501) staff       (20)    10547 2024-04-13 15:38:56.000000 geodynamic-0.0.8/geodynamic/geo/construction.py
--rw-------   0 mac        (501) staff       (20)    24312 2024-04-15 15:34:01.000000 geodynamic-0.0.8/geodynamic/geo/lib_commands.py
--rw-------   0 mac        (501) staff       (20)    12974 2024-04-13 14:52:57.000000 geodynamic-0.0.8/geodynamic/geo/lib_elements.py
--rw-------   0 mac        (501) staff       (20)     1752 2024-01-22 09:44:40.000000 geodynamic-0.0.8/geodynamic/geo/lib_vars.py
--rw-------   0 mac        (501) staff       (20)    32122 2024-04-21 11:50:53.000000 geodynamic-0.0.8/geodynamic/manim_dynamic.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-21 11:52:53.936452 geodynamic-0.0.8/geodynamic/parsers/
--rw-rw-r--   0 mac        (501) staff       (20)        0 2024-04-20 15:28:40.000000 geodynamic-0.0.8/geodynamic/parsers/__init__.py
--rw-------   0 mac        (501) staff       (20)    13622 2024-04-05 11:51:36.000000 geodynamic-0.0.8/geodynamic/parsers/ggb_generator.py
--rw-------   0 mac        (501) staff       (20)     7626 2024-04-21 11:50:59.000000 geodynamic-0.0.8/geodynamic/parsers/ggb_parser.py
--rw-------   0 mac        (501) staff       (20)     3344 2024-04-05 11:52:04.000000 geodynamic-0.0.8/geodynamic/parsers/short_parser.py
--rw-rw-r--   0 mac        (501) staff       (20)     3971 2024-04-21 10:17:23.000000 geodynamic-0.0.8/geodynamic/parsers/svg_parser.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-21 11:52:53.937650 geodynamic-0.0.8/geodynamic.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)     1099 2024-04-21 11:52:53.000000 geodynamic-0.0.8/geodynamic.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      575 2024-04-21 11:52:53.000000 geodynamic-0.0.8/geodynamic.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2024-04-21 11:52:53.000000 geodynamic-0.0.8/geodynamic.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       60 2024-04-21 11:52:53.000000 geodynamic-0.0.8/geodynamic.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       11 2024-04-21 11:52:53.000000 geodynamic-0.0.8/geodynamic.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) staff       (20)       38 2024-04-21 11:52:53.939764 geodynamic-0.0.8/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      951 2024-04-21 11:52:39.000000 geodynamic-0.0.8/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-23 14:09:10.793645 geodynamic-0.0.9/
+-rw-r--r--   0 mac        (501) staff       (20)       18 2024-04-05 12:40:59.000000 geodynamic-0.0.9/LICENSE.txt
+-rw-r--r--   0 mac        (501) staff       (20)     1099 2024-04-23 14:09:10.793576 geodynamic-0.0.9/PKG-INFO
+-rw-------   0 mac        (501) staff       (20)      428 2024-04-18 12:05:16.000000 geodynamic-0.0.9/README.md
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-23 14:09:10.787358 geodynamic-0.0.9/geodynamic/
+-rw-------   0 mac        (501) staff       (20)        0 2024-04-05 11:31:09.000000 geodynamic-0.0.9/geodynamic/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-23 14:09:10.791153 geodynamic-0.0.9/geodynamic/geo/
+-rw-------   0 mac        (501) staff       (20)        0 2023-12-28 13:25:09.000000 geodynamic-0.0.9/geodynamic/geo/__init__.py
+-rw-------   0 mac        (501) staff       (20)    10547 2024-04-13 15:38:56.000000 geodynamic-0.0.9/geodynamic/geo/construction.py
+-rw-------   0 mac        (501) staff       (20)    24312 2024-04-15 15:34:01.000000 geodynamic-0.0.9/geodynamic/geo/lib_commands.py
+-rw-------   0 mac        (501) staff       (20)    12974 2024-04-13 14:52:57.000000 geodynamic-0.0.9/geodynamic/geo/lib_elements.py
+-rw-------   0 mac        (501) staff       (20)     1752 2024-01-22 09:44:40.000000 geodynamic-0.0.9/geodynamic/geo/lib_vars.py
+-rw-------   0 mac        (501) staff       (20)    37162 2024-04-23 14:01:32.000000 geodynamic-0.0.9/geodynamic/manim_dynamic.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-23 14:09:10.792715 geodynamic-0.0.9/geodynamic/parsers/
+-rw-rw-r--   0 mac        (501) staff       (20)        0 2024-04-20 15:28:40.000000 geodynamic-0.0.9/geodynamic/parsers/__init__.py
+-rw-------   0 mac        (501) staff       (20)    13622 2024-04-05 11:51:36.000000 geodynamic-0.0.9/geodynamic/parsers/ggb_generator.py
+-rw-------   0 mac        (501) staff       (20)     7381 2024-04-23 13:50:40.000000 geodynamic-0.0.9/geodynamic/parsers/ggb_parser.py
+-rw-------   0 mac        (501) staff       (20)     3344 2024-04-05 11:52:04.000000 geodynamic-0.0.9/geodynamic/parsers/short_parser.py
+-rw-rw-r--   0 mac        (501) staff       (20)     4142 2024-04-23 10:46:27.000000 geodynamic-0.0.9/geodynamic/parsers/svg_parser.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-23 14:09:10.793273 geodynamic-0.0.9/geodynamic.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)     1099 2024-04-23 14:09:10.000000 geodynamic-0.0.9/geodynamic.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      575 2024-04-23 14:09:10.000000 geodynamic-0.0.9/geodynamic.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2024-04-23 14:09:10.000000 geodynamic-0.0.9/geodynamic.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       60 2024-04-23 14:09:10.000000 geodynamic-0.0.9/geodynamic.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)       11 2024-04-23 14:09:10.000000 geodynamic-0.0.9/geodynamic.egg-info/top_level.txt
+-rw-r--r--   0 mac        (501) staff       (20)       38 2024-04-23 14:09:10.793946 geodynamic-0.0.9/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      951 2024-04-23 14:07:57.000000 geodynamic-0.0.9/setup.py
```

### Comparing `geodynamic-0.0.8/PKG-INFO` & `geodynamic-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geodynamic
-Version: 0.0.8
+Version: 0.0.9
 Summary: Geometric tools for parsing GeoGebra construction, proccess with manim animation and export to SVG
 Home-page: https://gitlab.mathem.ru/
 Author: ivaleo
 Author-email: ivaleotion@gmail.com
 Keywords: geometry dynamic geogebra manim animation svg python
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `geodynamic-0.0.8/geodynamic/geo/construction.py` & `geodynamic-0.0.9/geodynamic/geo/construction.py`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.8/geodynamic/geo/lib_commands.py` & `geodynamic-0.0.9/geodynamic/geo/lib_commands.py`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.8/geodynamic/geo/lib_elements.py` & `geodynamic-0.0.9/geodynamic/geo/lib_elements.py`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.8/geodynamic/geo/lib_vars.py` & `geodynamic-0.0.9/geodynamic/geo/lib_vars.py`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.8/geodynamic/manim_dynamic.py` & `geodynamic-0.0.9/geodynamic/manim_dynamic.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,56 @@
     if isinstance(x, (int, float)): return False
     else:
         try:
             y = float(x)
             return False
         except:
             return True
+ 
+def rgba(arr):
+    if isinstance(arr, str): arr = arr.split(' ')
+    
+    try:
+        if len(arr) == 1:
+            return ManimColor(arr[0]).to_rgb()
+        elif len(arr) == 2:
+            if arr[1] is None: return ManimColor(arr[0]).to_rgb()
+            else: return ManimColor(arr[0], arr[1]).to_rgba()
+        elif len(arr) == 3:
+            return ManimColor(arr).to_rgb()
+        elif len(arr) == 4:
+            return ManimColor(arr).to_rgba()
+    except Exception as e:
+        #print('RBGA:', arr)
+        #print('EXCEPTION:', e)
+        return None
+    return None
+
+def equal(arr1, arr2, eps = None):
+    if len(arr1) != len(arr2): return False
+
+    if eps is None:
+        for i in range(len(arr1)):
+            if arr1[i] != arr2[i]: return False
+    else:
+        for i in range(len(arr1)):
+            if np.abs(arr1[i] - arr2[i]) > eps: return False
+
+    return True
+
+def getColorFromDict(dict, col, eps = 0.01):
+    col = rgba(col)
+    if col is None: return None
+    
+    for key in dict:
+        col_value = rgba(key)
+        if equal(col, col_value, eps): 
+            return rgba(dict[key])
+    
+    return None
 
 def CorrectSVG(svg_path):
     #tree = ET.parse(svg_path)
 
     #for elem in tree.findall(f'.//{xmlns}text'):
     #    elem.set('font-style', 'italic')
 
@@ -87,14 +129,35 @@
         self.col = style['color']['main']
         self.col_light = style['color']['light']
         self.col_accent = style['color']['acc']
         self.col_accent_light = style['color']['acc_light']
         self.col_gray = '#eeeeee'
         
         self.technic = style_map['technic']
+        self.ggb_export = style_map['ggb_export']
+        
+        if 'colors' in self.ggb_export:
+            for key in self.ggb_export['colors']:
+                value = self.ggb_export['colors'][key]
+                arr = value.split(' ')
+                if arr[0] in style['color']:
+                    self.ggb_export['colors'][key] = style['color'][arr[0]]
+                    if len(arr) > 1: self.ggb_export['colors'][key] += ' ' + ' '.join(arr[1:])
+        
+        if 'dot' in self.ggb_export:
+            for key in self.ggb_export['dot']:
+                value = str(self.ggb_export['dot'][key])
+                if value in style['dot']:
+                    self.ggb_export['dot'][key] = style['dot'][value]
+        
+        if 'line' in self.ggb_export: 
+            for key in self.ggb_export['line']:
+                value = str(self.ggb_export['line'][key])
+                if value in style['line']:
+                    self.ggb_export['line'][key] = style['line'][value]
 
     def setViewByGeo(self, geoView):
         w0, h0 = self.view['width'], self.view['height']
         w, h = geoView['width'], geoView['height']
         if isnan(w0) & isnan(h0): 
             print("ERROR: width and heigth haven't been set")
             return
@@ -286,14 +349,51 @@
 
     def loadGeoGebra(self, filepath, style_json_file = None, px_size = None, debug = False):
         self.geo = ggb_parser.load(filepath, debug = debug) 
         self.geo.rebuild(debug = debug)
         
         style = GeoStyle(style_json_file = style_json_file, px_size = px_size)
         
+        if 'polygon_boundary_layer' in style.technic:
+            if style.technic['polygon_boundary_layer'] == 'top':
+                for comm in self.geo.commands:
+                    if comm.name == 'Polygon':
+                        for segm in comm.outputs[1:]:
+                            self.geo.element(segm).style['z_index'] = 10
+                            
+        if 'colors' in style.ggb_export:
+            ggb_colors = style.ggb_export['colors']
+            for elem in self.geo.elements:
+                col = getParamFromDict(elem.style, 'stroke', None)
+                col_opacity = getParamFromDict(elem.style, 'stroke_opacity', None)
+                col_new = getColorFromDict(ggb_colors, [col, col_opacity])
+                if col_new is not None: 
+                    elem.style['stroke'] = col_new
+                    if len(col_new) > 3:
+                        elem.style['stroke_opacity'] = col_new[3]
+            
+                col = getParamFromDict(elem.style, 'fill', None)
+                col_opacity = getParamFromDict(elem.style, 'fill_opacity', None)
+                col_new = getColorFromDict(ggb_colors, [col, col_opacity])
+                if col_new is not None: 
+                    elem.style['fill'] = col_new
+                    if len(col_new) > 3:
+                        elem.style['fill_opacity'] = col_new[3]
+                        
+        if 'line' in style.ggb_export:
+            ggb_line = style.ggb_export['line']
+            print(ggb_line)
+            for elem in self.geo.elements:
+                wid = getParamFromDict(elem.style, 'stroke_width', None)
+                #print(str(wid))
+                wid_new = getParamFromDict(ggb_line, str(wid), None)
+                if wid_new is not None: 
+                    print('WIDTH:', wid_new)
+                    elem.style['stroke_width'] = 2 * wid_new
+        
         bounds = self.getAllGeometryBounds(self.geo.style['view']['scale'])
         padding = style.technic['crop_padding'] if 'crop_padding' in style.technic else 10
         
         #print('BOUNDS:', bounds)
         
         self.geo.style['view']['width'] = bounds[2] - bounds[0] + 2 * padding
         self.geo.style['view']['height'] = bounds[3] - bounds[1] + 2 * padding
@@ -308,23 +408,28 @@
         view = style.view
         scale = view['scale']
         scale_export = style.technic['scale_export'] if 'scale_export' in style.technic else 1
         q = 50 * scale_export / scale
         for key in ['dot_size', 'line_width', 'ang_width', 'ang_rdefault', 'ang_right', 'ang_rshift', 'strich_width', 'strich_rshift', 'strich_len']:
             setattr(style, key, getattr(style, key) * q)
             
+        for elem in self.geo.elements:
+            wid = getParamFromDict(elem.style, 'stroke_width', None)
+            if wid is not None: 
+                elem.style['stroke_width'] = float(wid) * q
+            
         ratio = 1920/1080
         if view['width'] / view['height'] >= ratio:
             self.camera.frame.set(width = view['width'] / scale)
             dx = self.camera.frame.width / 2 - view['xZero'] / scale
             dy = view['height'] / (2 * scale) - view['yZero'] / scale      
             self.camera.frame.shift(dx * RIGHT + dy * DOWN)
         else:
             self.camera.frame.set(width = ratio * view['height'] / scale)
-            dx = view['height'] / (2 * scale) - view['xZero'] / scale
+            dx = view['width'] / (2 * scale) - view['xZero'] / scale
             dy = self.camera.frame.height / 2 - view['yZero'] / scale      
             self.camera.frame.shift(dx * RIGHT + dy * DOWN)
     
         self.setStyle(style)
         self.addAllGeometry(show = True)
 
     def updateGeoVar(self, x, var_name):
@@ -628,22 +733,29 @@
     return min(max_r, r)
 
 def CreateMObject(elem, z_auto = False, style = None, debug = False):
     try:
         if style is None: style = GeoDynamic.style_default
 
         dash = getParamFromDict(elem.style, 'stroke_dash', None)
-        cap = getParamFromDict(elem.style, 'stroke_cap', getParamFromDict(style.technic, 'line_caps', 'auto'))
+        cap = getParamFromDict(elem.style, 'stroke_cap', getParamFromDict(style.technic, 'line_caps', None))
+        ra_joint = getParamFromDict(elem.style, 'right_angle_joint', getParamFromDict(style.technic, 'right_angle_joint', 'auto'))
         #print('CAP', cap)
+        joint_map = {
+            "auto": LineJointType.AUTO,
+            "bevel": LineJointType.BEVEL,
+            "miter": LineJointType.MITER,
+            "round": LineJointType.ROUND
+        }
 
         col_s = getParamFromDict(elem.style, 'stroke', style.strong)
         col_f = getParamFromDict(elem.style, 'fill', style.background if type(elem.data) != geo.Point else style.strong)
         op_s = getParamFromDict(elem.style, 'stroke_opacity', 1)
         op_f = getParamFromDict(elem.style, 'fill_opacity', 1)
-        lw = getParamFromDict(elem.style, 'stroke_width', style.line_width, type(elem.data) == geo.Arc)
+        lw = getParamFromDict(elem.style, 'stroke_width', style.line_width) #, type(elem.data) == geo.Arc)
         col_label = getParamFromDict(elem.style, 'label_color', style.strong)
 
         zz = getParamFromDict(elem.style, 'z_index')
         zz_fill = 0.01
         zz_stroke = 5
         zz_label = 50
 
@@ -679,16 +791,17 @@
                 n1 = elem.data.v1 * (r / np.linalg.norm(elem.data.v1))
                 n2 = elem.data.v2 * (r / np.linalg.norm(elem.data.v2))
                 p1 = [p[0] + n1[0], p[1] + n1[1], 0]
                 p2 = [p1[0] + n2[0], p1[1] + n2[1], 0]
                 p3 = [p[0] + n2[0], p[1] + n2[1], 0]
                 arr.append(Polygon(p, p1, p2, p3, 
                                     color = col_f, stroke_width = 0, fill_opacity = op_f).set_z_index(zz))
-                arr.append(RightAngle(line1, line2, length = r,
-                                color = col_s, fill_opacity = 0, stroke_width = style.ang_width, stroke_opacity = op_s).set_z_index(zz + 0.1))
+                arr.append(VMobject(color = col_s, fill_opacity = 0, stroke_width = style.ang_width, stroke_opacity = op_s, joint_type = joint_map[ra_joint])
+                           .set_points_as_corners([p1, p2, p3]).set_z_index(zz + 0.1))
+                #print('RIGHT_JOINT:', joint_map[ra_joint])
             else:
                 arr.append(AnnularSector(inner_radius = 0, outer_radius = r, angle = elem.data.angle, 
                                 color = col_f, fill_opacity = op_f).set_z_index(zz)
                                 .rotate(elem.data.start_angle, about_point=ORIGIN).shift ([p[0], p[1], 0]))
                 for i in range(elem.style['lines']):
                     arr.append(Angle(line1, line2, radius = r - i * style.ang_rshift, other_angle = False, 
                                 color = col_s, fill_opacity = 0, stroke_width = style.ang_width, stroke_opacity = op_s).set_z_index(zz + 0.1))
@@ -763,25 +876,33 @@
                 tex.move_to(Arc(arc_center = c, radius = elem.data.r + 0.7, start_angle = a1, angle = a2 - a1).point_from_proportion(0.5))
                 arr.append(tex)
                 if hasParam(elem.style, 'offset'):
                     tex.shift([elem.style['offset'][0], elem.style['offset'][1], 0])
 
             return VGroup(*arr, name = elem.name)
 
-        if type(elem.data) == geo.Point:  
+        if type(elem.data) == geo.Point:
             arr = [Dot([elem.data.a[0], elem.data.a[1], 0], radius = style.dot_size / 2,
                     color = col_f, fill_opacity = op_f).set_z_index(zz)]
+            if getParamFromDict(style.technic, 'points_display', None) == 'only_labels':
+                arr[0].set_fill(opacity = 0)
+                arr[0].set_phantom(True)
+                
             if hasParam(elem.style, 'show_label'):
                 label = elem.style['label'] if hasParam(elem.style, 'label') else '$' + elem.name + '$'
                 tex = Tex(correctedLabel(label), color = col_label).set_z_index(zz_label).scale(1.12).move_to(arr[0])
                 arr.append(tex)
                 if hasParam(elem.style, 'offset'):
                     tex.shift([elem.style['offset'][0], elem.style['offset'][1], 0])
+                if getParamFromDict(style.technic, 'points_display', None) == 'only_points':
+                    arr[1].set_fill(opacity = 0)
+                    arr[1].set_phantom(True)
 
             return VGroup(*arr, name = elem.name)
+        
     except Exception as e:
         print(f'MObject for element "{elem.name}" is NONE')
-        print(e)
+        print(f'EXCEPTION: {e}')
         return None
     
     return None
```

### Comparing `geodynamic-0.0.8/geodynamic/parsers/ggb_generator.py` & `geodynamic-0.0.9/geodynamic/parsers/ggb_generator.py`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.8/geodynamic/parsers/ggb_parser.py` & `geodynamic-0.0.9/geodynamic/parsers/ggb_parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,16 +37,14 @@
 
 def parse_constr(constr: Construction, constr_xelem: XElement, debug = False):
     xelems_left_to_pass = 0
     fixed_element = False
 
     style = {}
     
-    polygon_border = {}
-    
     for xelem in constr_xelem:            
         if xelem.tag == "element":
             name = xelem.attrib['label']
             #print(f'ELEMENT {name}')
             if xelem.attrib["type"] != "numeric":
                 style[name] = {}
 
@@ -85,15 +83,15 @@
                     lineStyle = xelem.find("lineStyle")
                     if lineStyle is not None:
                         thick, tt = lineStyle.attrib['thickness'], lineStyle.attrib['type']
                         op = float(lineStyle.attrib['opacity']) if 'opacity' in lineStyle.attrib else 255
                         if xelem.attrib['type'] in ['angle', 'segment', 'arc', 'conic']:
                             style[name]['stroke'] = rgb_to_hex(r, g, b)
                             #style[name]['stroke_opacity'] = op / 255
-                            #style[name]['stroke_width'] = thick
+                            style[name]['stroke_width'] = thick
                             if int(tt) > 0: style[name]['stroke_dash'] = 0.65
                         
         if xelems_left_to_pass:
             xelems_left_to_pass -= 1
             continue
 
         if xelem.tag == "expression":
@@ -103,25 +101,22 @@
         if xelem.tag == "command":
             comm_name = xelem.attrib["name"]
             input_xelem, output_xelem = xelem.find("input"), xelem.find("output")
             inputs, outputs = list(input_xelem.attrib.values()), list(output_xelem.attrib.values())
             
             if comm_name == "Point":
                 if len(inputs) == 1:
-                    print('Point FIXED')
+                    if debug: print('Point FIXED')
                     fixed_element = True
                 else:
                     xelems_left_to_pass = 1
                 continue
             if comm_name == "PointIn":
                 xelems_left_to_pass = 1
                 continue
-            if comm_name == "Polygon":
-                for segm in outputs[1:]:
-                    polygon_border[segm] = True
 
             constr.add(Command(comm_name, inputs, outputs))
             xelems_left_to_pass = len(output_xelem.attrib)
             continue
         
         # Here xelem has to be a commandless point or numeric (Var)
         
@@ -141,24 +136,19 @@
                 constr.add(Var(xelem.attrib["label"], AngleSize(float(value_xelem.attrib["val"]))))
                 continue
         
         #raise ElementTree.ParseError(f"Unexpected XElement met:\n\t<{xelem.tag}>, {xelem.attrib}")
         print(f"Unexpected XElement met:\n\t<{xelem.tag}>, {xelem.attrib}")
 
     constr.rebuild(debug = debug)
-    
-    #print(polygon_border)
-
-    for segm in polygon_border:
-        constr.element(segm).style['z_index'] = 10
 
     #styling elements
     for name in style:
         for key in style[name]:
-            #print(f'STYLE >> {name} >> {key} = {style[name][key]}')
+            if debug: print(f'STYLE >> {name} >> {key} = {style[name][key]}')
             if key == 'show_element':
                 constr.element(name).visible = style[name][key]
                 continue
             constr.element(name).style[key] = style[name][key]
 
 def FloatOrNone(txt):
     return float(txt) if txt is not None else None
@@ -172,13 +162,13 @@
 
         if xelem.tag == "coordSystem":
             constr.style['view']['xZero'], constr.style['view']['yZero'] = FloatOrNone(xelem.attrib['xZero']), FloatOrNone(xelem.attrib['yZero'])
             constr.style['view']['scale'] = FloatOrNone(xelem.attrib['scale'])       
 
 def load(ggb_path: str, debug = False): # -> Construction:
     constr_xelem, view_xelem = get_xelems(ggb_path)
-    print(constr_xelem, view_xelem)
+    if debug: print(constr_xelem, view_xelem)
     constr = Construction()
     parse_constr(constr, constr_xelem, debug = debug)
     parse_view(constr, view_xelem, debug = debug)
     
     return constr
```

### Comparing `geodynamic-0.0.8/geodynamic/parsers/short_parser.py` & `geodynamic-0.0.9/geodynamic/parsers/short_parser.py`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.8/geodynamic/parsers/svg_parser.py` & `geodynamic-0.0.9/geodynamic/parsers/svg_parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import itertools
 import tempfile
 from contextlib import contextmanager
 from pathlib import Path
 
 import cairo
 import numpy as np
-from manim import VGroup, VMobject
+from manim import VGroup, VMobject, constants
 from manim.utils.family import extract_mobject_family_members
 
 CAIRO_LINE_WIDTH_MULTIPLE: float = 0.01
 
 __all__ = ["create_svg_from_vmobject", "create_svg_from_vgroup", "_get_cairo_context", "extract_mobject_family_members", "_create_svg_from_vmobject_internal"]
 
 @contextmanager
@@ -43,26 +43,32 @@
 
 def _apply_stroke(ctx: cairo.Context, vmobject: VMobject, style = None):
     width = vmobject.get_stroke_width()
     if width == 0: return
     
     _set_cairo_context_color(ctx, vmobject.get_stroke_rgbas(), vmobject)
     ctx.set_line_width(width * CAIRO_LINE_WIDTH_MULTIPLE)
-    if style is not None:
-        linecap = {
-            "auto": cairo.LINE_CAP_BUTT,
-            "butt": cairo.LINE_CAP_BUTT,
-            "round": cairo.LINE_CAP_ROUND,
-            "square": cairo.LINE_CAP_SQUARE
-        }
-        cap = vmobject.get_stroke_cap() if hasattr(vmobject, 'stroke_cap') else 'auto'
-        ctx.set_line_cap(linecap[cap])
+
+    linecap = {
+        "auto": cairo.LINE_CAP_BUTT,
+        "butt": cairo.LINE_CAP_BUTT,
+        "round": cairo.LINE_CAP_ROUND,
+        "square": cairo.LINE_CAP_SQUARE
+    }
+    cap = vmobject.get_stroke_cap() if hasattr(vmobject, 'stroke_cap') else 'auto'
+    ctx.set_line_cap(linecap[cap])
+        
+    joint_map = {
+        constants.LineJointType.AUTO: cairo.LINE_JOIN_MITER,
+        constants.LineJointType.BEVEL: cairo.LINE_JOIN_BEVEL,
+        constants.LineJointType.MITER: cairo.LINE_JOIN_MITER,
+        constants.LineJointType.ROUND: cairo.LINE_JOIN_ROUND
+    }
     
-    # if vmobject.joint_type != LineJointType.AUTO:
-    #     ctx.set_line_join(LINE_JOIN_MAP[vmobject.joint_type])
+    ctx.set_line_join(joint_map[vmobject.joint_type])
     ctx.stroke_preserve()
 
 def _apply_fill(ctx: cairo.Context, vmobject: VMobject, style = None):
     _set_cairo_context_color(ctx, vmobject.get_fill_rgbas(), vmobject)
     ctx.fill_preserve()
 
 def _create_svg_from_vmobject_internal(vmobject: VMobject, ctx: cairo.Content, style = None):
```

### Comparing `geodynamic-0.0.8/geodynamic.egg-info/PKG-INFO` & `geodynamic-0.0.9/geodynamic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geodynamic
-Version: 0.0.8
+Version: 0.0.9
 Summary: Geometric tools for parsing GeoGebra construction, proccess with manim animation and export to SVG
 Home-page: https://gitlab.mathem.ru/
 Author: ivaleo
 Author-email: ivaleotion@gmail.com
 Keywords: geometry dynamic geogebra manim animation svg python
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `geodynamic-0.0.8/geodynamic.egg-info/SOURCES.txt` & `geodynamic-0.0.9/geodynamic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.8/setup.py` & `geodynamic-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 setup(
   name='geodynamic',
-  version='0.0.8',
+  version='0.0.9',
   author='ivaleo',
   author_email='ivaleotion@gmail.com',
   description='Geometric tools for parsing GeoGebra construction, proccess with manim animation and export to SVG',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://gitlab.mathem.ru/',
   packages=find_packages(),
```

