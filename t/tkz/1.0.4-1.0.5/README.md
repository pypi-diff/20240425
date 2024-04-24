# Comparing `tmp/tkz-1.0.4.tar.gz` & `tmp/tkz-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkz-1.0.4.tar", last modified: Wed Apr 24 18:35:02 2024, max compression
+gzip compressed data, was "tkz-1.0.5.tar", last modified: Wed Apr 24 22:14:55 2024, max compression
```

## Comparing `tkz-1.0.4.tar` & `tkz-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-24 18:35:02.420924 tkz-1.0.4/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     1058 2023-12-11 21:28:06.000000 tkz-1.0.4/LICENSE.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)    15717 2024-04-24 18:35:02.420838 tkz-1.0.4/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)    15271 2024-04-24 18:34:35.000000 tkz-1.0.4/README.md
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 tkz-1.0.4/pyproject.toml
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      568 2024-04-24 18:35:02.421147 tkz-1.0.4/setup.cfg
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-24 18:35:02.418508 tkz-1.0.4/src/
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-24 18:35:02.419864 tkz-1.0.4/src/tkz/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       50 2023-12-11 22:09:38.000000 tkz-1.0.4/src/tkz/__init__.py
--rw-r--r--   0 davidwoodburn   (501) staff       (20)    86161 2024-04-24 18:34:14.000000 tkz-1.0.4/src/tkz/tkz.py
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-24 18:35:02.420641 tkz-1.0.4/src/tkz.egg-info/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)    15717 2024-04-24 18:35:02.000000 tkz-1.0.4/src/tkz.egg-info/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      235 2024-04-24 18:35:02.000000 tkz-1.0.4/src/tkz.egg-info/SOURCES.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-04-24 18:35:02.000000 tkz-1.0.4/src/tkz.egg-info/dependency_links.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-04-24 18:35:02.000000 tkz-1.0.4/src/tkz.egg-info/requires.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        4 2024-04-24 18:35:02.000000 tkz-1.0.4/src/tkz.egg-info/top_level.txt
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-24 22:14:55.631350 tkz-1.0.5/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     1058 2023-12-11 21:28:06.000000 tkz-1.0.5/LICENSE.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)    15911 2024-04-24 22:14:55.631267 tkz-1.0.5/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)    15465 2024-04-24 22:14:25.000000 tkz-1.0.5/README.md
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 tkz-1.0.5/pyproject.toml
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      568 2024-04-24 22:14:55.631573 tkz-1.0.5/setup.cfg
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-24 22:14:55.629143 tkz-1.0.5/src/
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-24 22:14:55.630228 tkz-1.0.5/src/tkz/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       50 2023-12-11 22:09:38.000000 tkz-1.0.5/src/tkz/__init__.py
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)    87234 2024-04-24 22:03:33.000000 tkz-1.0.5/src/tkz/tkz.py
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-24 22:14:55.631069 tkz-1.0.5/src/tkz.egg-info/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)    15911 2024-04-24 22:14:55.000000 tkz-1.0.5/src/tkz.egg-info/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      235 2024-04-24 22:14:55.000000 tkz-1.0.5/src/tkz.egg-info/SOURCES.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-04-24 22:14:55.000000 tkz-1.0.5/src/tkz.egg-info/dependency_links.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-04-24 22:14:55.000000 tkz-1.0.5/src/tkz.egg-info/requires.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        4 2024-04-24 22:14:55.000000 tkz-1.0.5/src/tkz.egg-info/top_level.txt
```

### Comparing `tkz-1.0.4/LICENSE.txt` & `tkz-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tkz-1.0.4/PKG-INFO` & `tkz-1.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: tkz
-Version: 1.0.4
-Summary: TikZ Figure Generator
-Home-page: https://gitlab.com/davidwoodburn/tkz
-Author: David Woodburn
-Author-email: david.woodburn@icloud.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: numpy
-
 # TikZ Figure Generator
 
 There is a need for professional-looking figures. Good quality figures in
 publications are clear and easy to understand. This means they should not be
 badly pixelated. Though it is tempting to take a screen shot of your figures to
 then include in your papers, this is a sure way to produce poor-quality images.
 Often, the text will be hard to read, the lines will be pixelated, and important
@@ -97,30 +82,32 @@
 ```
 
 There are some options you can set for all figures in your file:
 
 | Option       | Description                                 | Default Value |
 | :----------- | :------------------------------------------ | ------------- |
 | `skip`       | flag to skip all subsequent plotting        | `False`       |
-| `silent`     | flag to silence most of the pdflatex output | `True`        |
 | `directory`  | directory of the generated figure files     | `None`        |
 | `standalone` | flag to create standalone LaTeX file        | `True`        |
-| `savepng`    | flag to output png version too              | `False`       |
+| `savepng`    | flag to convert pdf to png too              | `False`       |
+| `savetex`    | flag to keep the LaTeX source file          | `False`       |
 
-The `silent` option silences most of the pdflatex output messages, but not all.
-This is turned on by default. If you want to see all the messages, set this
-option to `False`. If `directory` is left as `None` then the figures will be
-generated in the current working directory. If the `standalone` flag is `True`,
-this library will attempt to call the `pdflatex` command line program to compile
-the `.tex` file and produce a pdf image. Because you may need a rasterized
-version of your figure after all (see Microsoft Office's lack of support for pdf
-vector images), the `savepng` option will produce a png version of the image
-from the pdf version. This requires the program `pdftoppm` from the `poppler`
-command line utilities package, and that the `standalone` option be set to
-`True`.
+Because compiling LaTeX files can be slow, it might be helpful sometimes to turn
+off all tkz renders. This can be done by setting `skip` to `True`. If
+`directory` is left as `None` then the figures will be generated in the current
+working directory. If the `standalone` flag is `True`, this library will attempt
+to call the `pdflatex` command line program to compile the `.tex` file and
+produce a pdf image. Because you may need a rasterized version of your figure
+after all (see Microsoft Office's lack of support for pdf vector images), the
+`savepng` option will produce a png version of the image from the pdf version.
+This requires the program `pdftoppm` from the `poppler` command line utilities
+package, and that the `standalone` option is set to `True`. By default, after a
+standalone LaTeX file is created and the pdf file is compiled, the source LaTeX
+file will be deleted. If you want to save the LaTeX file for inspection or
+tweaking, set the `savetex` option to `True`.
 
 ## Figure Options
 
 ```python
 fig = tkz.graph(<options>)
 ```
```

### Comparing `tkz-1.0.4/README.md` & `tkz-1.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: tkz
+Version: 1.0.5
+Summary: TikZ Figure Generator
+Home-page: https://gitlab.com/davidwoodburn/tkz
+Author: David Woodburn
+Author-email: david.woodburn@icloud.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: numpy
+
 # TikZ Figure Generator
 
 There is a need for professional-looking figures. Good quality figures in
 publications are clear and easy to understand. This means they should not be
 badly pixelated. Though it is tempting to take a screen shot of your figures to
 then include in your papers, this is a sure way to produce poor-quality images.
 Often, the text will be hard to read, the lines will be pixelated, and important
@@ -82,30 +97,32 @@
 ```
 
 There are some options you can set for all figures in your file:
 
 | Option       | Description                                 | Default Value |
 | :----------- | :------------------------------------------ | ------------- |
 | `skip`       | flag to skip all subsequent plotting        | `False`       |
-| `silent`     | flag to silence most of the pdflatex output | `True`        |
 | `directory`  | directory of the generated figure files     | `None`        |
 | `standalone` | flag to create standalone LaTeX file        | `True`        |
-| `savepng`    | flag to output png version too              | `False`       |
+| `savepng`    | flag to convert pdf to png too              | `False`       |
+| `savetex`    | flag to keep the LaTeX source file          | `False`       |
 
-The `silent` option silences most of the pdflatex output messages, but not all.
-This is turned on by default. If you want to see all the messages, set this
-option to `False`. If `directory` is left as `None` then the figures will be
-generated in the current working directory. If the `standalone` flag is `True`,
-this library will attempt to call the `pdflatex` command line program to compile
-the `.tex` file and produce a pdf image. Because you may need a rasterized
-version of your figure after all (see Microsoft Office's lack of support for pdf
-vector images), the `savepng` option will produce a png version of the image
-from the pdf version. This requires the program `pdftoppm` from the `poppler`
-command line utilities package, and that the `standalone` option be set to
-`True`.
+Because compiling LaTeX files can be slow, it might be helpful sometimes to turn
+off all tkz renders. This can be done by setting `skip` to `True`. If
+`directory` is left as `None` then the figures will be generated in the current
+working directory. If the `standalone` flag is `True`, this library will attempt
+to call the `pdflatex` command line program to compile the `.tex` file and
+produce a pdf image. Because you may need a rasterized version of your figure
+after all (see Microsoft Office's lack of support for pdf vector images), the
+`savepng` option will produce a png version of the image from the pdf version.
+This requires the program `pdftoppm` from the `poppler` command line utilities
+package, and that the `standalone` option is set to `True`. By default, after a
+standalone LaTeX file is created and the pdf file is compiled, the source LaTeX
+file will be deleted. If you want to save the LaTeX file for inspection or
+tweaking, set the `savetex` option to `True`.
 
 ## Figure Options
 
 ```python
 fig = tkz.graph(<options>)
 ```
```

### Comparing `tkz-1.0.4/setup.cfg` & `tkz-1.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tkz
-version = 1.0.4
+version = 1.0.5
 author = David Woodburn
 author_email = david.woodburn@icloud.com
 description = TikZ Figure Generator
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/davidwoodburn/tkz
 classifiers =
```

### Comparing `tkz-1.0.4/src/tkz/tkz.py` & `tkz-1.0.5/src/tkz/tkz.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 __license__ = "MIT"
 __date__ = "2024-04-24"
 __maintainer__ = "David Woodburn"
 __email__ = "david.woodburn@icloud.com"
 __status__ = "Development"
 
 import os
+import subprocess
 import warnings
 import math                         # 5-10x faster than NumPy for scalars
 import numpy as np
 
 # Generic constants
 PT_PER_CM = 28.45274                # points per centimeter
 WIDTH = 8.636                       # default figure width (cm)
@@ -92,20 +93,20 @@
 R_DECIMAL = 0.28                    # decimal width as ratio of font size
 R_TIMES = 0.89                      # times width as ratio of font size
 R_POWER = 0.85                      # scaling factor for widths in powers
 
 
 # Library-wide attributes
 class config:
+    colormap = MAP_WHEEL            # main color map
     skip = False                    # flag to skip plotting
-    silent = True                   # flag to silence pdflatex output
     directory = None                # directory for figure files
-    colormap = MAP_WHEEL            # main color map
     standalone = True               # flag to create standalone LaTeX file
     savepng = False                 # flag to send call to `pdftoppm`
+    savetex = False                 # flag to keep the .tex files
 
 
 class GraphLayout:
     """ Settings for the layout of the graph. """
     def __init__(self): # These are the internal, calculated settings.
         self.width = 0.0            # width of figure (cm)
         self.height = 0.0           # height of figure (cm)
@@ -181,15 +182,15 @@
         self.func = func            # plot, scatter, fill
         self.label = label          # data set label string
         self.simp = simp            # flag to simplify path
         self.fmt = fmt              # additional format string
 
 
 class graph:
-    def __init__(self, filename='fig', width=None, height=None,
+    def __init__(self, filename="fig", width=None, height=None,
             xmin=None, xmax=None, ymin=None, ymax=None,
             xpad=False, ypad=True, xlog=False, ylog=False,
             equal=False, fontsize=9, xlabel=None, ylabel=None,
             xaxis=True, yaxis=True, xgrid=True, ygrid=True,
             xsubgrid=True, ysubgrid=True, xtick=True, ytick=True,
             ticksize=TICK_SIZE, xout=False, yout=False,
             rowmajor=False, columns=None, preamble=None):
@@ -347,18 +348,17 @@
             lay.y_tick_fmt = "right"
             lay.y_tick_shift = lay.L_tick_shift
 
         # -----------------------
         # Write the data to file.
         # -----------------------
 
-        # Open the output file.
-        filepath = "" if config.directory is None else config.directory + "/"
-        filepath += self.filename + ".tex"
-        fid = open(filepath, "w")
+        # Open the output file. FIXME
+        filetex = self.filename + ".tex"
+        fid = open(filetex, "w")
 
         # Open the standalone TikZ script.
         if config.standalone:
             write_open(fid, self.preamble)
         elif self.preamble is not None:
             print("Because this plot is not standalone, "
                     + "the additional preamble cannot be used.")
@@ -567,39 +567,65 @@
         # Close the output file.
         fid.close()
 
         # -----------------
         # Compile the file.
         # -----------------
 
-        # Compile the LaTeX file.
-        if config.standalone:
-            # Build the pdf compile command.
-            cmd = 'pdflatex'
-            if config.silent:
-                cmd = cmd + ' --interaction=batchmode'
-
-            # Get the file name.
-            filename = self.filename
-
-            # Append to the command and file name if a directory is specified.
-            if config.directory is not None:
-                pwd = os.getcwd()
-                cmd = f'{cmd} -output-directory="{pwd}/{config.directory}"'
-                filename = config.directory + '/' + filename
+        # Return if there is nothing to compile.
+        if not config.standalone:
+            if config.savepng:
+                print("`config.standalone` must be True for a png to be made.")
+            return
 
+        # Compile the LaTeX file.
+        try:
             # Compile the image to pdf.
-            os.system(f'{cmd} "{filename}.tex"')
-            os.system(f'rm "{filename}.aux"')
-            os.system(f'rm "{filename}.log"')
+            result = subprocess.run(["pdflatex", "-halt-on-error", filetex],
+                    stdout=subprocess.PIPE, stderr=subprocess.PIPE)
 
-            # Compile the image to png.
-            if config.savepng:
-                os.system(f'pdftoppm "{filename}.pdf" '
-                        + f'"{filename}" -png -r 600 -singlefile')
+            # Check the return code.
+            if result.returncode == 0:
+                filepdf = self.filename + ".pdf"
+
+                # Compile the image to png.
+                png_saved = False
+                if config.savepng:
+                    try:
+                        subprocess.run(["pdftoppm", filepdf, self.filename,
+                                "-png", "-r", "600", "-singlefile"])
+                        png_saved = True
+                    except FileNotFoundError:
+                        print("Could not convert to png. "
+                                + f"pdftoppm might not be available.")
+                        print("Consider installing poppler.")
+
+                # Move the pdf.
+                if config.directory is not None:
+                    if os.path.exists(config.directory):
+                        subprocess.run(["mv", self.filename + ".pdf",
+                                config.directory])
+                        if png_saved:
+                            subprocess.run(["mv", self.filename + ".png",
+                                    config.directory])
+                    else:
+                        print(f"config.directory = '{config.directory}'")
+                        print("This path does not exist.")
+
+                # Remove the temporary files.
+                subprocess.run(["rm", self.filename + ".aux"])
+                subprocess.run(["rm", self.filename + ".log"])
+                if not config.savetex:
+                    subprocess.run(["rm", filetex])
+            else:
+                print(result.stdout.decode())
+        except FileNotFoundError:
+            print("Could not compile .tex file. "
+                    + "pdflatex might not be available.")
+            print("Consider installing texlive.")
 
 
 # ---------------------
 # Calculation Functions
 # ---------------------
 
 def check_shapes(sets):
@@ -800,15 +826,15 @@
     if is_log:
         precision = 0
         format_func = lstr
     else:
         # The decision to use scientific notation (3.14x10^1) versus
         # floating-point notation (31.4) depends on the extrema grid
         # values being larger than 999 or smaller than 0.01. The
-        # 'precision' is of the whole number, not just the mantissa,
+        # "precision" is of the whole number, not just the mantissa,
         # and depends on the grid step size.
         e_min = get_base_exp(grids[0])
         e_max = get_base_exp(grids[-1])
         precision = -get_base_exp(grids[1] - grids[0])
         if math.fabs(e_min) > 3 or math.fabs(e_max) > 3:
             format_func = gstr
         else:
@@ -1066,15 +1092,15 @@
         lay.y_min = 10.0**lay.y_min
         lay.y_max = 10.0**lay.y_max
 
 def dstr(x, p=0, f=10):
     """
     Given a floating-point number `x`, the precision `p`, and  the font size `f`
     in points, return a LaTeX string `s` of the number as an integer and the
-    estimated width `w` in points. 'p' is unused.
+    estimated width `w` in points. `p` is unused.
     """
     x = int(round(x))
     s = "%d" % x
     if x >= 0:
         w = (len(s)*R_DIGIT)*f
     else:
         w = (R_SIGN + (len(s) - 1)*R_DIGIT)*f
@@ -1095,15 +1121,15 @@
     return s, w
 
 
 def gstr(x, p=6, f=10):
     """
     Given a floating-point number `x`, the precision `p`, and  the font size `f`
     in points, return a LaTeX string `s` of the number in the format `m x 10^e`
-    and the estimated width `w` in points. 'p' is the precision of the whole
+    and the estimated width `w` in points. `p` is the precision of the whole
     number, not of the mantissa alone.
     """
 
     # Simplify for zero.
     if x == 0:
         return "0", (R_DIGIT*f)
 
@@ -1860,32 +1886,28 @@
 
 # --------------------------
 # LaTeX Code Write Functions
 # --------------------------
 
 def write_open(fid, preamble=None):
     fid.write("% Preamble")
-    fid.write("\n\\batchmode")
     fid.write("\n\\documentclass{standalone}")
     fid.write("\n\\usepackage{bm}")
     fid.write("\n\\usepackage{tikz}")
     fid.write("\n\\usepackage{pdfrender}")
     fid.write("\n\\newcommand{\\ul}[1] % vectors")
     fid.write("\n    {{}\\mkern1mu\\underline")
     fid.write("{\\mkern-1mu#1\\mkern-1mu}\\mkern1mu}")
     fid.write("\n\\DeclareSymbolFont{euler}{U}{eur}{m}{n}")
     fid.write("\n\\DeclareMathSymbol{\\PI}{\\mathord}{euler}{25}")
     if preamble is not None:
-        fid.write("\n\\errorstopmode")
         fid.write("\n%s" % preamble)
-        fid.write("\n\\batchmode")
     fid.write("\n% Document contents")
     fid.write("\n\\begin{document}")
     fid.write("\n\\begin{tikzpicture}")
-    fid.write("\n\\errorstopmode")
 
 
 def write_textstyle(fid, font_size_name):
     txt = "\n% Set the style of all text."
     txt += "\n\\tikzset{every node/.style={inner sep=0pt"
     if font_size_name != "normalsize":
         txt += ", font=\\" + font_size_name
```

### Comparing `tkz-1.0.4/src/tkz.egg-info/PKG-INFO` & `tkz-1.0.5/src/tkz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkz
-Version: 1.0.4
+Version: 1.0.5
 Summary: TikZ Figure Generator
 Home-page: https://gitlab.com/davidwoodburn/tkz
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -97,30 +97,32 @@
 ```
 
 There are some options you can set for all figures in your file:
 
 | Option       | Description                                 | Default Value |
 | :----------- | :------------------------------------------ | ------------- |
 | `skip`       | flag to skip all subsequent plotting        | `False`       |
-| `silent`     | flag to silence most of the pdflatex output | `True`        |
 | `directory`  | directory of the generated figure files     | `None`        |
 | `standalone` | flag to create standalone LaTeX file        | `True`        |
-| `savepng`    | flag to output png version too              | `False`       |
+| `savepng`    | flag to convert pdf to png too              | `False`       |
+| `savetex`    | flag to keep the LaTeX source file          | `False`       |
 
-The `silent` option silences most of the pdflatex output messages, but not all.
-This is turned on by default. If you want to see all the messages, set this
-option to `False`. If `directory` is left as `None` then the figures will be
-generated in the current working directory. If the `standalone` flag is `True`,
-this library will attempt to call the `pdflatex` command line program to compile
-the `.tex` file and produce a pdf image. Because you may need a rasterized
-version of your figure after all (see Microsoft Office's lack of support for pdf
-vector images), the `savepng` option will produce a png version of the image
-from the pdf version. This requires the program `pdftoppm` from the `poppler`
-command line utilities package, and that the `standalone` option be set to
-`True`.
+Because compiling LaTeX files can be slow, it might be helpful sometimes to turn
+off all tkz renders. This can be done by setting `skip` to `True`. If
+`directory` is left as `None` then the figures will be generated in the current
+working directory. If the `standalone` flag is `True`, this library will attempt
+to call the `pdflatex` command line program to compile the `.tex` file and
+produce a pdf image. Because you may need a rasterized version of your figure
+after all (see Microsoft Office's lack of support for pdf vector images), the
+`savepng` option will produce a png version of the image from the pdf version.
+This requires the program `pdftoppm` from the `poppler` command line utilities
+package, and that the `standalone` option is set to `True`. By default, after a
+standalone LaTeX file is created and the pdf file is compiled, the source LaTeX
+file will be deleted. If you want to save the LaTeX file for inspection or
+tweaking, set the `savetex` option to `True`.
 
 ## Figure Options
 
 ```python
 fig = tkz.graph(<options>)
 ```
```

