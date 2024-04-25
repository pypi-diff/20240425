# Comparing `tmp/rHDPE_Data_Analysis-1.0.2.tar.gz` & `tmp/rHDPE_Data_Analysis-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rHDPE_Data_Analysis-1.0.2.tar", last modified: Fri Apr 19 16:24:38 2024, max compression
+gzip compressed data, was "rHDPE_Data_Analysis-1.0.3.tar", last modified: Thu Apr 25 12:10:56 2024, max compression
```

## Comparing `rHDPE_Data_Analysis-1.0.2.tar` & `rHDPE_Data_Analysis-1.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-04-19 16:24:38.347230 rHDPE_Data_Analysis-1.0.2/
--rw-r--r--   0 philsmith   (501) staff       (20)      353 2024-04-19 16:24:38.346564 rHDPE_Data_Analysis-1.0.2/PKG-INFO
-drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-04-19 16:24:38.253903 rHDPE_Data_Analysis-1.0.2/rHDPE_Data_Analysis/
-drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-04-19 16:24:38.300499 rHDPE_Data_Analysis-1.0.2/rHDPE_Data_Analysis/FTIR_Analysis/
--rw-r--r--   0 philsmith   (501) staff       (20)     2704 2024-02-20 12:55:58.000000 rHDPE_Data_Analysis-1.0.2/rHDPE_Data_Analysis/FTIR_Analysis/Analysis.py
--rw-r--r--   0 philsmith   (501) staff       (20)     7997 2024-04-18 15:38:31.000000 rHDPE_Data_Analysis-1.0.2/rHDPE_Data_Analysis/FTIR_Analysis/FTIR_plotting.py
--rw-r--r--   0 philsmith   (501) staff       (20)     1878 2023-12-22 10:54:22.000000 rHDPE_Data_Analysis-1.0.2/rHDPE_Data_Analysis/FTIR_Analysis/Input_Parameters_Class.py
--rw-r--r--   0 philsmith   (501) staff       (20)     9844 2024-03-14 15:29:24.000000 rHDPE_Data_Analysis-1.0.2/rHDPE_Data_Analysis/FTIR_Analysis/Preprocessing.py
--rw-r--r--   0 philsmith   (501) staff       (20)    43726 2024-03-12 12:08:57.000000 rHDPE_Data_Analysis-1.0.2/rHDPE_Data_Analysis/FTIR_Analysis/Utilities.py
--rw-r--r--   0 philsmith   (501) staff       (20)      148 2023-12-22 10:54:51.000000 rHDPE_Data_Analysis-1.0.2/rHDPE_Data_Analysis/FTIR_Analysis/__init__.py
-drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-04-19 16:24:38.335365 rHDPE_Data_Analysis-1.0.2/rHDPE_Data_Analysis/Global_Analysis/
--rw-r--r--   0 philsmith   (501) staff       (20)     2122 2024-02-27 12:52:11.000000 rHDPE_Data_Analysis-1.0.2/rHDPE_Data_Analysis/Global_Analysis/Analysis.py
--rw-r--r--   0 philsmith   (501) staff       (20)     1446 2024-01-09 12:15:24.000000 rHDPE_Data_Analysis-1.0.2/rHDPE_Data_Analysis/Global_Analysis/Input_Parameters_Class.py
--rw-r--r--   0 philsmith   (501) staff       (20)     3534 2024-03-18 15:04:29.000000 rHDPE_Data_Analysis-1.0.2/rHDPE_Data_Analysis/Global_Analysis/Preprocessing.py
--rw-r--r--   0 philsmith   (501) staff       (20)    37985 2024-03-28 13:43:47.000000 rHDPE_Data_Analysis-1.0.2/rHDPE_Data_Analysis/Global_Analysis/Utilities.py
--rw-r--r--   0 philsmith   (501) staff       (20)      120 2024-01-03 12:56:03.000000 rHDPE_Data_Analysis-1.0.2/rHDPE_Data_Analysis/Global_Analysis/__init__.py
--rw-r--r--   0 philsmith   (501) staff       (20)    35883 2024-04-19 16:24:08.000000 rHDPE_Data_Analysis-1.0.2/rHDPE_Data_Analysis/Global_Utilities.py
--rw-r--r--   0 philsmith   (501) staff       (20)       37 2022-08-08 17:17:04.000000 rHDPE_Data_Analysis-1.0.2/rHDPE_Data_Analysis/__init__.py
-drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-04-19 16:24:38.345792 rHDPE_Data_Analysis-1.0.2/rHDPE_Data_Analysis.egg-info/
--rw-r--r--   0 philsmith   (501) staff       (20)      353 2024-04-19 16:24:38.000000 rHDPE_Data_Analysis-1.0.2/rHDPE_Data_Analysis.egg-info/PKG-INFO
--rw-r--r--   0 philsmith   (501) staff       (20)      813 2024-04-19 16:24:38.000000 rHDPE_Data_Analysis-1.0.2/rHDPE_Data_Analysis.egg-info/SOURCES.txt
--rw-r--r--   0 philsmith   (501) staff       (20)        1 2024-04-19 16:24:38.000000 rHDPE_Data_Analysis-1.0.2/rHDPE_Data_Analysis.egg-info/dependency_links.txt
--rw-r--r--   0 philsmith   (501) staff       (20)       20 2024-04-19 16:24:38.000000 rHDPE_Data_Analysis-1.0.2/rHDPE_Data_Analysis.egg-info/top_level.txt
--rw-r--r--   0 philsmith   (501) staff       (20)       38 2024-04-19 16:24:38.347378 rHDPE_Data_Analysis-1.0.2/setup.cfg
--rw-r--r--   0 philsmith   (501) staff       (20)      416 2024-04-19 16:24:22.000000 rHDPE_Data_Analysis-1.0.2/setup.py
+drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-04-25 12:10:56.573047 rHDPE_Data_Analysis-1.0.3/
+-rw-r--r--   0 philsmith   (501) staff       (20)      353 2024-04-25 12:10:56.572163 rHDPE_Data_Analysis-1.0.3/PKG-INFO
+drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-04-25 12:10:56.551104 rHDPE_Data_Analysis-1.0.3/rHDPE_Data_Analysis/
+drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-04-25 12:10:56.566074 rHDPE_Data_Analysis-1.0.3/rHDPE_Data_Analysis/FTIR_Analysis/
+-rw-r--r--   0 philsmith   (501) staff       (20)     2704 2024-02-20 12:55:58.000000 rHDPE_Data_Analysis-1.0.3/rHDPE_Data_Analysis/FTIR_Analysis/Analysis.py
+-rw-r--r--   0 philsmith   (501) staff       (20)     8041 2024-04-25 11:29:42.000000 rHDPE_Data_Analysis-1.0.3/rHDPE_Data_Analysis/FTIR_Analysis/FTIR_plotting.py
+-rw-r--r--   0 philsmith   (501) staff       (20)     1878 2023-12-22 10:54:22.000000 rHDPE_Data_Analysis-1.0.3/rHDPE_Data_Analysis/FTIR_Analysis/Input_Parameters_Class.py
+-rw-r--r--   0 philsmith   (501) staff       (20)     9887 2024-04-25 11:29:42.000000 rHDPE_Data_Analysis-1.0.3/rHDPE_Data_Analysis/FTIR_Analysis/Preprocessing.py
+-rw-r--r--   0 philsmith   (501) staff       (20)    43763 2024-04-25 11:29:42.000000 rHDPE_Data_Analysis-1.0.3/rHDPE_Data_Analysis/FTIR_Analysis/Utilities.py
+-rw-r--r--   0 philsmith   (501) staff       (20)      148 2023-12-22 10:54:51.000000 rHDPE_Data_Analysis-1.0.3/rHDPE_Data_Analysis/FTIR_Analysis/__init__.py
+drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-04-25 12:10:56.570905 rHDPE_Data_Analysis-1.0.3/rHDPE_Data_Analysis/Global_Analysis/
+-rw-r--r--   0 philsmith   (501) staff       (20)     2077 2024-04-25 11:31:49.000000 rHDPE_Data_Analysis-1.0.3/rHDPE_Data_Analysis/Global_Analysis/Analysis.py
+-rw-r--r--   0 philsmith   (501) staff       (20)     1446 2024-01-09 12:15:24.000000 rHDPE_Data_Analysis-1.0.3/rHDPE_Data_Analysis/Global_Analysis/Input_Parameters_Class.py
+-rw-r--r--   0 philsmith   (501) staff       (20)     3503 2024-04-25 11:31:49.000000 rHDPE_Data_Analysis-1.0.3/rHDPE_Data_Analysis/Global_Analysis/Preprocessing.py
+-rw-r--r--   0 philsmith   (501) staff       (20)    37968 2024-04-25 11:31:49.000000 rHDPE_Data_Analysis-1.0.3/rHDPE_Data_Analysis/Global_Analysis/Utilities.py
+-rw-r--r--   0 philsmith   (501) staff       (20)      120 2024-01-03 12:56:03.000000 rHDPE_Data_Analysis-1.0.3/rHDPE_Data_Analysis/Global_Analysis/__init__.py
+-rw-r--r--   0 philsmith   (501) staff       (20)    35883 2024-04-19 16:24:08.000000 rHDPE_Data_Analysis-1.0.3/rHDPE_Data_Analysis/Global_Utilities.py
+-rw-r--r--   0 philsmith   (501) staff       (20)        1 2024-04-25 11:22:18.000000 rHDPE_Data_Analysis-1.0.3/rHDPE_Data_Analysis/__init__.py
+drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-04-25 12:10:56.559758 rHDPE_Data_Analysis-1.0.3/rHDPE_Data_Analysis.egg-info/
+-rw-r--r--   0 philsmith   (501) staff       (20)      353 2024-04-25 12:10:56.000000 rHDPE_Data_Analysis-1.0.3/rHDPE_Data_Analysis.egg-info/PKG-INFO
+-rw-r--r--   0 philsmith   (501) staff       (20)      813 2024-04-25 12:10:56.000000 rHDPE_Data_Analysis-1.0.3/rHDPE_Data_Analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 philsmith   (501) staff       (20)        1 2024-04-25 12:10:56.000000 rHDPE_Data_Analysis-1.0.3/rHDPE_Data_Analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 philsmith   (501) staff       (20)       20 2024-04-25 12:10:56.000000 rHDPE_Data_Analysis-1.0.3/rHDPE_Data_Analysis.egg-info/top_level.txt
+-rw-r--r--   0 philsmith   (501) staff       (20)       38 2024-04-25 12:10:56.573236 rHDPE_Data_Analysis-1.0.3/setup.cfg
+-rw-r--r--   0 philsmith   (501) staff       (20)      416 2024-04-25 12:07:47.000000 rHDPE_Data_Analysis-1.0.3/setup.py
```

### Comparing `rHDPE_Data_Analysis-1.0.2/rHDPE_Data_Analysis/FTIR_Analysis/Analysis.py` & `rHDPE_Data_Analysis-1.0.3/rHDPE_Data_Analysis/FTIR_Analysis/Analysis.py`

 * *Files identical despite different names*

### Comparing `rHDPE_Data_Analysis-1.0.2/rHDPE_Data_Analysis/FTIR_Analysis/FTIR_plotting.py` & `rHDPE_Data_Analysis-1.0.3/rHDPE_Data_Analysis/FTIR_Analysis/FTIR_plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 
 import numpy as np
 import matplotlib.pyplot as plt
 import matplotlib as mpl
 import sys
 from pathlib import Path
 
-sys.path.append( Path( __file__ ).absolute().parents[3].as_posix() )
+# sys.path.append( Path( __file__ ).absolute().parents[3].as_posix() )
+#
+# from rHDPE_Data_Analysis import Global_Utilities as gu
 
-from rHDPE_Data_Analysis import Global_Utilities as gu
+from .. import Global_Utilities as gu
 
 # Function definitions.
 
 def plot_data( directory, file_data, data, first_derivative_data, second_derivative_data, third_derivative_data, m_peaks, m_peaks_array, y_peaks, y_peaks_array, savefig = False ):
 
     # for i in range( len( data[1] ) ):
     #
```

### Comparing `rHDPE_Data_Analysis-1.0.2/rHDPE_Data_Analysis/FTIR_Analysis/Input_Parameters_Class.py` & `rHDPE_Data_Analysis-1.0.3/rHDPE_Data_Analysis/FTIR_Analysis/Input_Parameters_Class.py`

 * *Files identical despite different names*

### Comparing `rHDPE_Data_Analysis-1.0.2/rHDPE_Data_Analysis/FTIR_Analysis/Preprocessing.py` & `rHDPE_Data_Analysis-1.0.3/rHDPE_Data_Analysis/FTIR_Analysis/Preprocessing.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 import glob
 import re
 import numpy as np
 import pandas as pd
 import sys
 from pathlib import Path
 
-sys.path.append( Path( __file__ ).absolute().parents[3].as_posix() )
+# sys.path.append( Path( __file__ ).absolute().parents[3].as_posix() )
 
-from rHDPE_Data_Analysis import Global_Utilities as gu
+# from rHDPE_Data_Analysis import Global_Utilities as gu
+
+from .. import Global_Utilities as gu
 
 # Function definitions.
 
 def read_raw_data_file_1( filename, r, resin_data, file_data, data ):
 
     pattern = re.compile( r"^Resin(\d+)" )
```

### Comparing `rHDPE_Data_Analysis-1.0.2/rHDPE_Data_Analysis/FTIR_Analysis/Utilities.py` & `rHDPE_Data_Analysis-1.0.3/rHDPE_Data_Analysis/FTIR_Analysis/Utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 import numpy as np
 import pandas as pd
 from scipy.stats import pearsonr
 import sys
 from pathlib import Path
 
-sys.path.append( Path( __file__ ).absolute().parents[3].as_posix() )
+# sys.path.append( Path( __file__ ).absolute().parents[3].as_posix() )
 
-from rHDPE_Data_Analysis import Global_Utilities as gu
+from .. import Global_Utilities as gu
 
 # Function definitions.
 
 def compute_derivatives( data, width = 1 ):
     '''Compute the derivatives.'''
 
     derivative_data = [data[0][width: -width], [], []]
@@ -994,15 +994,16 @@
         wavenumber_values.append( data[2][j][index_pearson] )
 
     wavenumber_values_array = np.array( wavenumber_values )
 
     gu.plot_scatterplot_of_two_features( feature, wavenumber_values_array, sample_mask, [resin_data.loc[i]["Label"] for i in sample_mask] )
 
 from . import Preprocessing
-from rHDPE_Data_Analysis.Global.Global_Analysis import Utilities as util2
+# from rHDPE_Data_Analysis.Global.Global_Analysis import Utilities as util2
+from .. import Global_Analysis.Utilities as util2
 from sklearn.preprocessing import StandardScaler
 
 def normalisation_experimentation( directory, file_data, data ):
     '''Experimenting to find best preprocessing for PCA.'''
 
     for i in range( len( data[1] ) ):
```

### Comparing `rHDPE_Data_Analysis-1.0.2/rHDPE_Data_Analysis/Global_Analysis/Analysis.py` & `rHDPE_Data_Analysis-1.0.3/rHDPE_Data_Analysis/Global_Analysis/Analysis.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # Imports.
 
 import sys
 from pathlib import Path
 
 sys.path.append( Path( __file__ ).absolute().parents[1].as_posix() )
 
-from Global_Analysis import Preprocessing
-from Global_Analysis import Utilities as util
+from . import Preprocessing
+from . import Utilities as util
 
 sys.path.append( Path( __file__ ).absolute().parents[3].as_posix() )
 
-from rHDPE_Data_Analysis import Global_Utilities as gu
+from .. import Global_Utilities as gu
 
 # Main function definition.
 
 def Global_Analysis_Main( directory, ip ):
 
     if ip.datasets_to_read == False:
```

### Comparing `rHDPE_Data_Analysis-1.0.2/rHDPE_Data_Analysis/Global_Analysis/Input_Parameters_Class.py` & `rHDPE_Data_Analysis-1.0.3/rHDPE_Data_Analysis/Global_Analysis/Input_Parameters_Class.py`

 * *Files identical despite different names*

### Comparing `rHDPE_Data_Analysis-1.0.2/rHDPE_Data_Analysis/Global_Analysis/Preprocessing.py` & `rHDPE_Data_Analysis-1.0.3/rHDPE_Data_Analysis/Global_Analysis/Preprocessing.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 import numpy as np
 import pandas as pd
 import sys
 from pathlib import Path
 
 sys.path.append( Path( __file__ ).absolute().parents[1].as_posix() )
 
-from Global_Analysis import Utilities as util
+from . import Utilities as util
 
 sys.path.append( Path( __file__ ).absolute().parents[3].as_posix() )
 
-from rHDPE_Data_Analysis import Global_Utilities as gu
+from .. import Global_Utilities as gu
 
 # Function definitions.
 
 def read_files_and_preprocess( directory, datasets_to_read, sample_mask ):
 
     resin_data = gu.get_list_of_resins_data( directory )
```

### Comparing `rHDPE_Data_Analysis-1.0.2/rHDPE_Data_Analysis/Global_Analysis/Utilities.py` & `rHDPE_Data_Analysis-1.0.3/rHDPE_Data_Analysis/Global_Analysis/Utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from sklearn import datasets, linear_model
 
 import sys
 from pathlib import Path
 
 sys.path.append( Path( __file__ ).absolute().parents[3].as_posix() )
 
-from rHDPE_Data_Analysis import Global_Utilities as gu
+from .. import Global_Utilities as gu
 
 def compile_full_dataset_of_features( dataset ):
 
     samples_present = []
 
     for i in dataset:
```

### Comparing `rHDPE_Data_Analysis-1.0.2/rHDPE_Data_Analysis/Global_Utilities.py` & `rHDPE_Data_Analysis-1.0.3/rHDPE_Data_Analysis/Global_Utilities.py`

 * *Files identical despite different names*

### Comparing `rHDPE_Data_Analysis-1.0.2/rHDPE_Data_Analysis.egg-info/SOURCES.txt` & `rHDPE_Data_Analysis-1.0.3/rHDPE_Data_Analysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

