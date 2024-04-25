# Comparing `tmp/bivariate-2.0.2.tar.gz` & `tmp/bivariate-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bivariate-2.0.2.tar", last modified: Thu Apr 18 05:18:58 2024, max compression
+gzip compressed data, was "bivariate-2.0.3.tar", last modified: Thu Apr 25 06:27:20 2024, max compression
```

## Comparing `bivariate-2.0.2.tar` & `bivariate-2.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:18:58.704314 bivariate-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-18 05:18:54.000000 bivariate-2.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    45928 2024-04-18 05:18:58.704314 bivariate-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-04-18 05:18:54.000000 bivariate-2.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-18 05:18:54.000000 bivariate-2.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 05:18:58.704314 bivariate-2.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:18:58.700313 bivariate-2.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:18:58.704314 bivariate-2.0.2/src/bivariate/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-18 05:18:54.000000 bivariate-2.0.2/src/bivariate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10483 2024-04-18 05:18:54.000000 bivariate-2.0.2/src/bivariate/class_component_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    29684 2024-04-18 05:18:54.000000 bivariate-2.0.2/src/bivariate/class_copula.py
--rw-r--r--   0 runner    (1001) docker     (127)    33386 2024-04-18 05:18:54.000000 bivariate-2.0.2/src/bivariate/class_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    19355 2024-04-18 05:18:54.000000 bivariate-2.0.2/src/bivariate/class_emperical.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-18 05:18:54.000000 bivariate-2.0.2/src/bivariate/class_fitresults.py
--rw-r--r--   0 runner    (1001) docker     (127)    24921 2024-04-18 05:18:54.000000 bivariate-2.0.2/src/bivariate/class_multivar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:18:58.704314 bivariate-2.0.2/src/bivariate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    45928 2024-04-18 05:18:58.000000 bivariate-2.0.2/src/bivariate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-18 05:18:58.000000 bivariate-2.0.2/src/bivariate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 05:18:58.000000 bivariate-2.0.2/src/bivariate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-18 05:18:58.000000 bivariate-2.0.2/src/bivariate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-18 05:18:58.000000 bivariate-2.0.2/src/bivariate.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:18:58.704314 bivariate-2.0.2/src/component_reliability/
--rw-r--r--   0 runner    (1001) docker     (127)    14320 2024-04-18 05:18:54.000000 bivariate-2.0.2/src/component_reliability/Case_Study_Compontent_Reliability_Tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:18:58.704314 bivariate-2.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-04-18 05:18:54.000000 bivariate-2.0.2/tests/test_bivariate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:27:20.325484 bivariate-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-25 06:27:16.000000 bivariate-2.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    45928 2024-04-25 06:27:20.325484 bivariate-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-04-25 06:27:16.000000 bivariate-2.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-25 06:27:16.000000 bivariate-2.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 06:27:20.325484 bivariate-2.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:27:20.321484 bivariate-2.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:27:20.321484 bivariate-2.0.3/src/bivariate/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-25 06:27:16.000000 bivariate-2.0.3/src/bivariate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10483 2024-04-25 06:27:16.000000 bivariate-2.0.3/src/bivariate/class_component_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30795 2024-04-25 06:27:16.000000 bivariate-2.0.3/src/bivariate/class_copula.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33386 2024-04-25 06:27:16.000000 bivariate-2.0.3/src/bivariate/class_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23735 2024-04-25 06:27:16.000000 bivariate-2.0.3/src/bivariate/class_emperical.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-25 06:27:16.000000 bivariate-2.0.3/src/bivariate/class_fitresults.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24921 2024-04-25 06:27:16.000000 bivariate-2.0.3/src/bivariate/class_multivar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:27:20.325484 bivariate-2.0.3/src/bivariate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    45928 2024-04-25 06:27:20.000000 bivariate-2.0.3/src/bivariate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-25 06:27:20.000000 bivariate-2.0.3/src/bivariate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 06:27:20.000000 bivariate-2.0.3/src/bivariate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-25 06:27:20.000000 bivariate-2.0.3/src/bivariate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-25 06:27:20.000000 bivariate-2.0.3/src/bivariate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:27:20.325484 bivariate-2.0.3/src/component_reliability/
+-rw-r--r--   0 runner    (1001) docker     (127)    14320 2024-04-25 06:27:16.000000 bivariate-2.0.3/src/component_reliability/Case_Study_Compontent_Reliability_Tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:27:20.325484 bivariate-2.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-04-25 06:27:16.000000 bivariate-2.0.3/tests/test_bivariate.py
```

### Comparing `bivariate-2.0.2/LICENSE.txt` & `bivariate-2.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bivariate-2.0.2/PKG-INFO` & `bivariate-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bivariate
-Version: 2.0.2
+Version: 2.0.3
 Summary: This package contains methods that assist in performing bivariate analysis of datasets.
 Author: Robert Lanzafame
 Author-email: r.lanzafame@tudelft.nl
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `bivariate-2.0.2/README.md` & `bivariate-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `bivariate-2.0.2/pyproject.toml` & `bivariate-2.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name='bivariate'
-version='2.0.2'
+version='2.0.3'
 description='This package contains methods that assist in performing bivariate analysis of datasets.'
 license = {file = "LICENSE.txt"}
 authors = [
   {email = "r.lanzafame@tudelft.nl"},
   {name = "Robert Lanzafame"}
 ]
 readme = "README.md"
```

### Comparing `bivariate-2.0.2/src/bivariate/class_component_analysis.py` & `bivariate-2.0.3/src/bivariate/class_component_analysis.py`

 * *Files identical despite different names*

### Comparing `bivariate-2.0.2/src/bivariate/class_copula.py` & `bivariate-2.0.3/src/bivariate/class_copula.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 from matplotlib import cm
 
 # This class is made by Siemen Algra, based on study material provided by the MUDE teaching team and Benjamin Rouse
 
 class Region_of_interest():
     def __init__(self,
                  function = None,
-                 random_samples : np.array = None
+                 random_samples : np.array = None,
+                 labels = None
                  ):
         """
         Region_of_interest class for 2 dimensional probabilistic analysis.
         This class is used to define a Region of interest. 
         This region can be any arbitrary shape, and is defined by the user using a function.
         
         Random samples are given as input, and the region of interest is defined by the user.
@@ -42,18 +43,22 @@
         function : function
             Function that defines the region of interest.
             The function should return True if the point is inside the region of interest, and False if it is not.
         random_samples : np.array
             Q-Dimensional array of random samples.
             Each row is 1 random sample of the Q-Dimensional distribution
             1st column is X1, 2nd column is X2,...., Qth column = Q.
+        labels : list
+            List of labels for the random samples.
+            labels = ['X1', 'X2', ...]
             
         """
         self.function = function
         self.random_samples = random_samples
+        self.labels = labels
     
         # Create empty dictionary to store the emperical contour plot values
         self.emperical_contour = {}
     
         
     def plot_function(self, 
                       xy_lim = None,
@@ -142,15 +147,16 @@
 
         return amount_inside, percentage_inside
     
     def plot_emperical_contours(self,
                                 xy_lim = None,
                                 axes=None,
                                 fig=None,
-                                bandwidth=0.5):
+                                bandwidth=0.5,
+                                equal_axis = None):
         """
         Plot the emperical contours of the random samples using the KernelDensity.
         
         Parameters
         ----------
         self : object
             The instance of the class.
@@ -210,18 +216,22 @@
                                   'density_values': density_values}      
         
         
         if axes is None:
             fig, axes = plt.subplots(1, 1, figsize=(14, 5))
         
             
-        if xy_lim is None:
+        if equal_axis is None and xy_lim is None:
+            xy_lim = [np.min(self.random_samples[:, 0]), np.max(self.random_samples[:, 0]), 
+                      np.min(self.random_samples[:, 1]), np.max(self.random_samples[:, 1])]
+        if equal_axis is not None and xy_lim is None:
             xy_lim = [np.min(self.random_samples), np.max(self.random_samples), 
                       np.min(self.random_samples), np.max(self.random_samples)]
             
+            
         # Set the x and y limits of the plot
         axes.set_xlim(xy_lim[0], xy_lim[1])
         axes.set_ylim(xy_lim[2], xy_lim[3])
         
         # Plot the random samples
         axes.scatter(self.random_samples[:, 0], self.random_samples[:, 1], alpha=0.05, label='Samples', color='gray') 
         
@@ -229,29 +239,33 @@
         axes.contour(self.emperical_contour_dict['X1_values'], 
                      self.emperical_contour_dict['X2_values'], 
                      self.emperical_contour_dict['density_values']
                      , levels=8, cmap=cm.Blues, alpha=0.8, zorder=4)
 
         
 
-         
-        axes.set_xlabel('X1')
-        axes.set_ylabel('X2')
+        if self.labels is not None:
+            axes.set_xlabel(self.labels[0])
+            axes.set_ylabel(self.labels[1])
+        else:
+            axes.set_xlabel('X1')
+            axes.set_ylabel('X2')
         axes.set_title('Emperical Contour Plot of Sampled Data')
         axes.legend()  
         axes.grid(True)
         axes.set_aspect("equal")
 
         plt.show()
     
     
     def plot_inside_function(self,
                              xy_lim = None,
                              axes=None,
-                             fig=None):
+                             fig=None,
+                             equal_axis = None):
         """
         Plot all the random samples, and highlight the ones inside the function region of interest.
         
         Parameters
         ----------
         self : object
             The instance of the class.
@@ -290,33 +304,42 @@
 
         # Something is going wrong with this.
         axes.contour(self.emperical_contour_dict['X1_values'], 
                      self.emperical_contour_dict['X2_values'], 
                      self.emperical_contour_dict['density_values']
                      , levels=8, cmap=cm.Blues, alpha=0.8, zorder=4)
 
-        if xy_lim is None:
+        if equal_axis is None and xy_lim is None:
+            xy_lim = [np.min(self.random_samples[:, 0]), np.max(self.random_samples[:, 0]), 
+                      np.min(self.random_samples[:, 1]), np.max(self.random_samples[:, 1])]
+        if equal_axis is not None and xy_lim is None:
             xy_lim = [np.min(self.random_samples), np.max(self.random_samples), 
                       np.min(self.random_samples), np.max(self.random_samples)]
 
+            
         # Plot the function
         x = np.linspace(xy_lim[0], xy_lim[1], 100)
         y = np.linspace(xy_lim[2], xy_lim[3], 100)
         X, Y = np.meshgrid(x, y)
         axes.contour(X, Y, self.function(X, Y), levels=[0], linewidths=2, colors='black')
 
             
         # Set the x and y limits of the plot
         axes.set_xlim(xy_lim[0], xy_lim[1])
         axes.set_ylim(xy_lim[2], xy_lim[3])
         
         axes.set_zorder(4)
         axes.legend()
-        axes.set_xlabel(f'X1')
-        axes.set_ylabel(f'X2')
+        
+        if self.labels is not None:
+            axes.set_xlabel(self.labels[0])
+            axes.set_ylabel(self.labels[1])
+        else:
+            axes.set_xlabel('X1')
+            axes.set_ylabel('X2')
         axes.set_title(f"Random samples inside the function region of interest \n {self.function_percentage_inside*100:.2f}% samples inside")
         axes.set_aspect("equal")
         axes.grid(True)
         axes.legend()
```

### Comparing `bivariate-2.0.2/src/bivariate/class_dataset.py` & `bivariate-2.0.3/src/bivariate/class_dataset.py`

 * *Files identical despite different names*

### Comparing `bivariate-2.0.2/src/bivariate/class_emperical.py` & `bivariate-2.0.3/src/bivariate/class_emperical.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 # This class is made by Siemen Algra, based on study material provided by the MUDE teaching team 
 # and a class made by Benjamin Rouse
 
 class Emperical_data():
 
     def __init__(self,
-                 time_series_data: np.array,
+                 time_series_data= None,
                  data_title = None,
                  data_units = None
                  ):
         """This class is used to perform emperical statistical analysis on time series data.
         It can be used to perform:
         - statistical analysis
         - plot time series data
@@ -335,14 +335,128 @@
             #     - 'params': fitted parameters are stored
             #     - 'RV_'   : instance of the rv_continuous_frozen class is stored
             #     - 'scipy_name': name used in scipy, done for operations
             self.distributions[name] = {'params': params, 'RV_': rv, 'scipy_name': distr_scipy_names[name]
                                         , 'method_of_fitting': fit_method}
 
  
+    def add_distribution(self, 
+                         distribution_name: str,
+                         params: str = None,
+                         rv_continous_frozen: Type[st.rv_continuous] = None,
+                         scipy_name: str = None,
+                         fit_method: str = None):
+        """Add a distribution to the data
+        
+        This function adds a distribution to the data. 
+        This can be used to add a distribution that is not fitted to the data, but is known.
+        This can be used to compare the emperical data to a known distribution.
+        
+        Parameters
+        ----------
+        self : `data_array`
+            Numpy array containing time series data. 
+            Note that this is already an attribute of the class.
+        distribution_name : `str`
+            Name of the distribution to be added.
+        params : `list`
+            List containing the parameters of the distribution.
+        fit_method : `str`
+            Method of fitting the distribution to the data.
+            Options are:
+            - 'MLE' Maximum Likelyhood Estimator
+            - 'MM'  Method of moments
+        
+        Returns
+        -------
+        None
+        
+        """
+        
+        distribution_mapping = {
+            'lognormal': st.lognorm,
+            'gumbel': st.gumbel_r,
+            'exponential': st.expon,
+            'weibull': st.weibull_min,
+            'normal': st.norm,
+            'gamma': st.gamma
+            # Add more distributions if needed
+        }
+        
+        # This is necessary because of name convention in other packages
+        distr_scipy_names = {
+            'lognormal': 'lognorm',
+            'gumbel': 'gumbel_r',
+            'exponential': 'expon',
+            'weibull': 'weibul_min',
+            'normal': 'norm',
+            'gamma': 'gamma'
+            # Add more distributions if needed
+        }
+        
+        
+        self.distributions[distribution_name] = {'params': params, 'RV_': rv_continous_frozen,
+                                                 'scipy_name': None,
+                                                 'method_of_fitting': fit_method}
+        
+    def plot_distributions(self,
+                            axes=None,
+                            fig=None,
+                            log_scale = True):
+        """
+        Plot the defined distributions
+        
+        Parameters
+        ----------
+        self : `data_array`
+            Numpy array containing time series data. 
+            Note that this is already an attribute of the class.
+        axes : `matplotlib.axes.Axes`
+            Axes object to plot on. If not provided, a new figure will be created.
+        fig : `matplotlib.figure.Figure`
+            Figure object to plot on. If not provided, a new figure will be created.
+        
+        Returns
+        -------
+        fig : `matplotlib.figure.Figure`
+            Figure object containing the plot.
+        ax : `matplotlib.axes.Axes`
+            Axes object containing the plot.        
+        
+        """
+        
+        # Create figure and axes if not provided
+        if axes is None:
+            fig, axes = plt.subplots(1, 1, figsize=(14, 5))
+            
+        # Plot the PDF's of all the fitted distributions, if none, prints statement
+        if not self.distributions:
+            print("No fitted distributions defined.")
+        else:
+            # Loops over all items (which are also dictionaries) in the {distributions} dictionary
+            # It extracts:
+            #  - name of the speficifc distribution 
+            #  - dictionary containing all information for that specific distribution
+            for distribution_name, distribution_dict in self.distributions.items():
+                quantiles = np.linspace(0.01, 0.99, 100)  # From 1% to 99% quantile
+
+                # Use the ppf to get x values
+                x = distribution_dict['RV_'].ppf(quantiles)
+                axes.plot(x, 1 - distribution_dict['RV_'].cdf(x), label=distribution_name)
+        
+        # Define the labels and text for the plot
+        axes.set_xlabel(f'{self.data_units}')
+        axes.set_ylabel('Probability of exceedance')
+        axes.set_title(f'PDF of {self.data_title}', fontsize=18)
+        
+        if log_scale == True:
+            axes.set_yscale('log')
+        axes.legend()
+        axes.grid()
+        
         
     def graphical_assessing_goodness_of_fit(self,
                                          axes=None,
                                          fig=None):
         """Plots the Emperical CDF and the fitted CDF's
```

### Comparing `bivariate-2.0.2/src/bivariate/class_fitresults.py` & `bivariate-2.0.3/src/bivariate/class_fitresults.py`

 * *Files identical despite different names*

### Comparing `bivariate-2.0.2/src/bivariate/class_multivar.py` & `bivariate-2.0.3/src/bivariate/class_multivar.py`

 * *Files identical despite different names*

### Comparing `bivariate-2.0.2/src/bivariate.egg-info/PKG-INFO` & `bivariate-2.0.3/src/bivariate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bivariate
-Version: 2.0.2
+Version: 2.0.3
 Summary: This package contains methods that assist in performing bivariate analysis of datasets.
 Author: Robert Lanzafame
 Author-email: r.lanzafame@tudelft.nl
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `bivariate-2.0.2/src/bivariate.egg-info/SOURCES.txt` & `bivariate-2.0.3/src/bivariate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bivariate-2.0.2/src/component_reliability/Case_Study_Compontent_Reliability_Tools.py` & `bivariate-2.0.3/src/component_reliability/Case_Study_Compontent_Reliability_Tools.py`

 * *Files identical despite different names*

### Comparing `bivariate-2.0.2/tests/test_bivariate.py` & `bivariate-2.0.3/tests/test_bivariate.py`

 * *Files identical despite different names*

