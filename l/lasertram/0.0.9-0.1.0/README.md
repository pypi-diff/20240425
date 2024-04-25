# Comparing `tmp/lasertram-0.0.9.tar.gz` & `tmp/lasertram-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lasertram-0.0.9.tar", last modified: Fri Oct 27 00:52:26 2023, max compression
+gzip compressed data, was "lasertram-0.1.0.tar", last modified: Thu Apr 25 17:37:28 2024, max compression
```

## Comparing `lasertram-0.0.9.tar` & `lasertram-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 00:52:26.044353 lasertram-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2023-10-27 00:52:13.000000 lasertram-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2023-10-27 00:52:26.044353 lasertram-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      690 2023-10-27 00:52:13.000000 lasertram-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 00:52:26.040353 lasertram-0.0.9/lasertram/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-27 00:52:13.000000 lasertram-0.0.9/lasertram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44536 2023-10-27 00:52:13.000000 lasertram-0.0.9/lasertram/lasertram.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 00:52:26.044353 lasertram-0.0.9/lasertram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2023-10-27 00:52:26.000000 lasertram-0.0.9/lasertram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      275 2023-10-27 00:52:26.000000 lasertram-0.0.9/lasertram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-27 00:52:26.000000 lasertram-0.0.9/lasertram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-10-27 00:52:26.000000 lasertram-0.0.9/lasertram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-10-27 00:52:26.000000 lasertram-0.0.9/lasertram.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-10-27 00:52:13.000000 lasertram-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      688 2023-10-27 00:52:26.044353 lasertram-0.0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 00:52:26.044353 lasertram-0.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    33094 2023-10-27 00:52:13.000000 lasertram-0.0.9/tests/test_lasertram.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:37:28.801510 lasertram-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-25 17:37:25.000000 lasertram-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-25 17:37:28.801510 lasertram-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-25 17:37:25.000000 lasertram-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:37:28.797510 lasertram-0.1.0/lasertram/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-25 17:37:25.000000 lasertram-0.1.0/lasertram/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:37:28.801510 lasertram-0.1.0/lasertram/calc/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-25 17:37:25.000000 lasertram-0.1.0/lasertram/calc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31659 2024-04-25 17:37:25.000000 lasertram-0.1.0/lasertram/calc/calc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:37:28.801510 lasertram-0.1.0/lasertram/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:37:25.000000 lasertram-0.1.0/lasertram/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-25 17:37:25.000000 lasertram-0.1.0/lasertram/helpers/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-25 17:37:25.000000 lasertram-0.1.0/lasertram/helpers/conversions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:37:28.801510 lasertram-0.1.0/lasertram/tram/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-25 17:37:25.000000 lasertram-0.1.0/lasertram/tram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11286 2024-04-25 17:37:25.000000 lasertram-0.1.0/lasertram/tram/tram.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:37:28.801510 lasertram-0.1.0/lasertram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-25 17:37:28.000000 lasertram-0.1.0/lasertram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-25 17:37:28.000000 lasertram-0.1.0/lasertram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 17:37:28.000000 lasertram-0.1.0/lasertram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-25 17:37:28.000000 lasertram-0.1.0/lasertram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-25 17:37:28.000000 lasertram-0.1.0/lasertram.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-25 17:37:25.000000 lasertram-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-25 17:37:28.801510 lasertram-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:37:28.801510 lasertram-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    37874 2024-04-25 17:37:25.000000 lasertram-0.1.0/tests/test_lasertram.py
```

### Comparing `lasertram-0.0.9/LICENSE` & `lasertram-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lasertram-0.0.9/PKG-INFO` & `lasertram-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lasertram
-Version: 0.0.9
+Version: 0.1.0
 Summary: For processing LA-ICP-MS data
 Home-page: https://github.com/jlubbersgeo/lasertram
 Author: Jordan Lubbers
 Author-email: jelubber@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lasertram-0.0.9/README.md` & `lasertram-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `lasertram-0.0.9/lasertram/lasertram.py` & `lasertram-0.1.0/lasertram/calc/calc.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,440 +1,25 @@
 """
-    The API for the package `lasertram`
-    This will largely be comprised of two classes:
 
-    - `LaserTRAM`: for taking raw counts per second data from a
-    Laser Ablation Inductively Coupled Plasma Mass Spectrometry (LA-ICP-MS)
-    experiment, choosing an interval to be turned into a concentration, normalizing
-    that interval to an internal standard and outputting that value + other metadata
-
-    - `LaserCalc`: for taking the output from `LaserTRAM` along with user input
-    to calculate concentrations for a series of `LaserTRAM` spot objects along
-    with statistics on calibration standards
-
-    Created and maintained by:
-    Jordan Lubbers
-    jlubbers@usgs.gov
+Calc module:
+This is for taking the output from `tram.LaserTRAM` along with user input
+to calculate concentrations for a series of `LaserTRAM` spot objects along
+with statistics on calibration standards
 
 """
+
 import re
 
-import mendeleev
 import numpy as np
 import pandas as pd
 import statsmodels.api as sm
 from scipy import stats
 from statsmodels.tools.eval_measures import rmse
 
-
-class LaserTRAM:
-    """
-    # LaserTRAM
-    The class `LaserTRAM` which is devoted to the "time resolved analysis"
-    operations during the laser data reduction process. To be used in
-    conjunction with the `LaserCalc` class. The general idea is that
-    this creates an object that contains all the information related
-    to one individual spot analysis.
-
-    """
-
-    def __init__(self, name):
-        """
-
-        Args:
-            name (str): your sample name i.e. the value in the `SampleLabel` column of the LT_ready file
-        """
-        self.name = name
-        self.despiked = False
-        self.despiked_elements = None
-
-    def get_data(self, df):
-        """assigns raw counts/sec data to the object
-
-        Args:
-            df (pandas DataFrame): raw data corresponding to the spot being processed i.e., `all_data.loc[spot,:]` if `all_data` is the LT_ready file
-        """
-        self.data = df.reset_index()
-        self.data = self.data.set_index("SampleLabel")
-        self.data["Time"] = self.data["Time"] / 1000
-        self.data_matrix = self.data.iloc[:, 1:].to_numpy()
-        self.analytes = self.data.loc[:, "Time":].columns.tolist()[1:]
-
-        # need to add check for if this exists otherwise there is no timestamp attribute
-        self.timestamp = str(self.data.loc[:, "timestamp"].unique()[0])
-
-    def assign_int_std(self, int_std):
-        """assigns the spot an internal standard
-        analyte
-
-        Args:
-            int_std (str): the name of the column for the internal standard analyte e.g., "29Si"
-        """
-        self.int_std = int_std
-
-    def assign_intervals(self, bkgd, keep, omit=None):
-        """assigns the intervals to be used as background
-        as well as the portion of the ablation interval to
-        be used in calculating concentrations
-
-        Args:
-            bkgd (tuple): (start, stop) pair of values corresponding to the analysis time where the background signal starts and stops
-            keep (tuple): (start, stop) pair of values correpsonding to the analysis time where the interval signal for concentrations starts and stops
-            omit (tuple): (start, stop) pair of values corresponding to the analysis time to be omitted from the `keep` interval. Defaults to None.
-        """
-
-        self.bkgd_start = bkgd[0]
-        self.bkgd_stop = bkgd[1]
-        self.int_start = keep[0]
-        self.int_stop = keep[1]
-
-        self.bkgd_start_idx = np.where(self.data["Time"] > self.bkgd_start)[0][0]
-        self.bkgd_stop_idx = np.where(self.data["Time"] > self.bkgd_stop)[0][0]
-        self.int_start_idx = np.where(self.data["Time"] > self.int_start)[0][0]
-        self.int_stop_idx = np.where((self.data["Time"] > self.int_stop))[0][0]
-
-        self.omitted_region = False
-
-        if omit:
-            self.omit_start = omit[0]
-            self.omit_stop = omit[1]
-            self.omit_start_idx = (
-                np.where(self.data["Time"] > self.omit_start)[0][0] - self.int_start_idx
-            )
-            self.omit_stop_idx = (
-                np.where(self.data["Time"] > self.omit_stop)[0][0] - self.int_start_idx
-            )
-
-            self.omitted_region = True
-
-    def get_bkgd_data(self):
-        """
-        uses the intervals assigned in `assign_intervals` to take the median
-        value of all analytes within that range and use them as the
-        background signal that gets subtracted from the ablation signal
-        """
-
-        self.bkgd_data = np.median(
-            self.data_matrix[self.bkgd_start_idx : self.bkgd_stop_idx, 1:], axis=0
-        )
-
-    def get_detection_limits(self):
-        """
-        Calculates detection limits in counts per second for each analyte. This
-        is defined as the value that is three standard deviations away from the
-        background.
-        """
-        self.detection_limits = np.std(
-            self.data_matrix[self.bkgd_start_idx : self.bkgd_stop_idx, 1:], axis=0
-        ) * 3 + np.median(
-            self.data_matrix[self.bkgd_start_idx : self.bkgd_stop_idx, 1:], axis=0
-        )
-
-    def subtract_bkgd(self):
-        """
-        subtract the median background values calculated in `get_bkgd_data`
-        from the signal in the "keep" interval established in `assign_intervals`
-
-        """
-        self.bkgd_correct_data = (
-            self.data_matrix[self.int_start_idx : self.int_stop_idx, 1:]
-            - self.bkgd_data
-        )
-
-    def normalize_interval(self):
-        """
-        normalize the analytes from the "keep" portion of the signal
-        the internal standard analyte. This is done by simply
-        dividing the analytes by the internal standard analyte.
-
-        This also calculates the median normalized value, its
-        standard error of the mean, and relative standard error
-        of the mean.
-        """
-        self.int_std_loc = np.where(np.array(self.analytes) == self.int_std)[0][0]
-
-        threshold = self.detection_limits - np.median(
-            self.data_matrix[self.bkgd_start_idx : self.bkgd_stop_idx, 1:], axis=0
-        )
-
-        if self.omitted_region is True:
-            self.bkgd_subtract_normal_data = np.delete(
-                self.bkgd_correct_data,
-                np.arange(self.omit_start_idx, self.omit_stop_idx),
-                axis=0,
-            ) / np.delete(
-                self.bkgd_correct_data[:, self.int_std_loc][:, None],
-                np.arange(self.omit_start_idx, self.omit_stop_idx),
-                axis=0,
-            )
-
-        else:
-            self.bkgd_subtract_normal_data = (
-                self.bkgd_correct_data
-                / self.bkgd_correct_data[:, self.int_std_loc][:, None]
-            )
-
-        self.bkgd_correct_med = np.median(self.bkgd_subtract_normal_data, axis=0)
-        self.bkgd_correct_med[
-            np.median(self.bkgd_correct_data, axis=0) <= threshold
-        ] = -9999
-        self.bkgd_correct_med[np.median(self.bkgd_correct_data, axis=0) == 0] = -9999
-
-        self.bkgd_correct_std_err = self.bkgd_subtract_normal_data.std(
-            axis=0
-        ) / np.sqrt(abs(self.int_stop_idx - self.int_start_idx))
-        self.bkgd_correct_std_err_rel = 100 * (
-            self.bkgd_correct_std_err / self.bkgd_correct_med
-        )
-
-    def make_output_report(self):
-        """
-        create an output report for the spot processing. This is a
-        pandas DataFrame that has the following format:
-
-        |timestamp|Spot|despiked|omitted_region|bkgd_start|bkgd_stop|int_start|int_stop|norm|norm_cps|analyte vals and uncertainties -->|
-        |---------|----|--------|--------------|----------|---------|---------|--------|----|--------|----------------------------------|
-        """
-        if self.despiked is True:
-            despike_col = self.despiked_elements
-        else:
-            despike_col = "None"
-
-        if self.omitted_region is True:
-            omitted_col = (
-                self.data["Time"].iloc[self.omit_start_idx + self.int_start_idx],
-                self.data["Time"].iloc[self.omit_stop_idx + self.int_start_idx],
-            )
-        else:
-            omitted_col = "None"
-
-        spot_data = pd.DataFrame(
-            [
-                self.timestamp,
-                self.name,
-                despike_col,
-                omitted_col,
-                self.data["Time"].iloc[self.bkgd_start_idx],
-                self.data["Time"].iloc[self.bkgd_stop_idx],
-                self.data["Time"].iloc[self.int_start_idx],
-                self.data["Time"].iloc[self.int_stop_idx],
-                self.int_std,
-                np.median(self.bkgd_correct_data[:, self.int_std_loc]),
-            ]
-        ).T
-        spot_data.columns = [
-            "timestamp",
-            "Spot",
-            "despiked",
-            "omitted_region",
-            "bkgd_start",
-            "bkgd_stop",
-            "int_start",
-            "int_stop",
-            "norm",
-            "norm_cps",
-        ]
-        spot_data = pd.concat(
-            [
-                spot_data,
-                pd.DataFrame(
-                    self.bkgd_correct_med[np.newaxis, :], columns=self.analytes
-                ),
-                pd.DataFrame(
-                    self.bkgd_correct_std_err_rel[np.newaxis, :],
-                    columns=[f"{analyte}_se" for analyte in self.analytes],
-                ),
-            ],
-            axis="columns",
-        )
-
-        for col in ["bkgd_start", "bkgd_stop", "int_start", "int_stop", "norm_cps"]:
-            spot_data[col] = spot_data[col].astype(np.float64)
-
-        self.output_report = spot_data
-
-    def despike_data(self, analyte_list="all"):
-        """
-        apply a standard deviation filter to all specified
-        analytes.
-
-
-        Args:
-            analyte_list (str or list, optional):analyte to despike (e.g., '7Li'). Or list of analytes to despike (e.g., ['7Li','88Sr']). If 'all', despikes all analytes in the experiment. Defaults to "all".
-        """
-
-        def despike_signal(data, analyte, passes=2):
-            """
-            apply a standard deviation filter to analyte signal
-
-            Args:
-                data (pandas DataFrame): dataframe representing the spot raw counts per second data.
-                analyte (string): analyte to despike
-                passes (int, optional): the number of iterations for the filter to complete. Defaults to 2.
-
-            Returns:
-                signal (ndarray): the filtered signal
-            """
-            window = 3
-            sigma = 25
-            kernel = np.ones(window) / window
-
-            signal_raw = data[analyte].to_numpy()
-            signal = signal_raw.copy()
-
-            for i in range(passes):
-                signal_mean = np.convolve(signal, kernel, "valid")
-                signal_mean = np.insert(
-                    signal_mean,
-                    0,
-                    signal_mean[0],
-                )
-                signal_mean = np.append(signal_mean, signal_mean[-1])
-                signal_std = np.sqrt(signal_mean)
-
-                spikes = signal > signal_mean + signal_std * sigma
-                despiked_signal = signal.copy()
-                despiked_signal[spikes] = signal_mean[spikes]
-                signal = despiked_signal
-
-            return signal
-
-        self.despiked = True
-
-        if analyte_list == "all":
-            filter_list = self.analytes
-        else:
-            if analyte_list is not type(list):
-                filter_list = [analyte_list]
-            else:
-                filter_list = analyte_list
-
-        self.despiked_elements = filter_list
-        for analyte in filter_list:
-            despiked.append(despike_signal(self.data, analyte))
-
-        despiked = pd.DataFrame(np.array(despiked).T, columns=self.analytes)
-        despiked.insert(0, "Time", self.data["Time"])
-
-        self.data = despiked
-        self.data_matrix = despiked.to_numpy()
-
-
-def process_spot(
-    spot,
-    raw_data,
-    bkgd,
-    keep,
-    internal_std,
-    omit=None,
-    despike=False,
-    output_report=True,
-):
-    """a function to incorporate all the methods of the `LaserTRAM` class
-    so a spot can be processed in an efficient and compact way.
-
-    Args:
-        spot (LaserTRAM spot object): an empty `LaserTRAM` spot object to be processed
-        raw_data (pandas DataFrame): the raw counts per second dataframe to be assigned to the spot. Shape is (m x n) where m is the number of cycles through the mass range
-        bkgd (tuple): (start, stop) pair of values corresponding to the analysis time where the background signal starts and stops
-        keep (tuple): (start, stop) pair of values correpsonding to the analysis time where the interval signal for concentrations starts and stops
-        internal_std (str): column name for the internal standard analyte (e.g., 29Si)
-        omit (tuple): (start, stop) pair of values corresponding to the analysis time to be omitted from the `keep` interval. Defaults to None.
-        despike (bool, optional): Whether or not to despike all analyte signals using the standard deviation filter from `LaserTRAM.despike_data()`. Defaults to False
-        output_report (bool, optional): Whether or not to create a 1-row pandas DataFrame output report in the following format. Defaults to True.
-
-
-    """
-    # assign data to the spot
-    spot.get_data(raw_data)
-    # despike the data if desired
-    if despike is True:
-        spot.despike_data(analyte_list="all")
-    # assign the internal standard analyte
-    spot.assign_int_std(internal_std)
-    # assign intervals for background and ablation signal
-    spot.assign_intervals(bkgd=bkgd, keep=keep, omit=omit)
-    # assign and save the median background values
-    spot.get_bkgd_data()
-    # remove the median background values from the ablation interval
-    spot.subtract_bkgd()
-    # calculate detection limits based off background values
-    spot.get_detection_limits()
-    # normalize the ablation interval to the internal standard analyte,
-    # get the median values, and the standard error
-    spot.normalize_interval()
-
-    if output_report is True:
-        spot.make_output_report()
-
-
-def oxide_to_ppm(wt_percent, int_std):
-    """
-    convert concentration internal standard analyte oxide in weight percent to
-    concentration ppm for a 1D series of data
-
-    Args:
-    wt_percent (array-like): the oxide values to be converted to ppm
-    int_std (str): the internal standard used in the experiment (e.g., '29Si', '43Ca','47Ti')
-
-    Returns:
-    ppm (array-like): concentrations in ppm the same shape as the wt_percent input
-
-    """
-
-    el = [i for i in int_std if not i.isdigit()]
-
-    if len(el) == 2:
-        element = el[0] + el[1]
-
-    else:
-        element = el[0]
-
-    oxides = [
-        "SiO2",
-        "TiO2",
-        "Al2O3",
-        "Cr2O3",
-        "MnO",
-        "FeO",
-        "K2O",
-        "CaO",
-        "Na2O",
-        "NiO",
-        "MgO",
-    ]
-
-    for o in oxides:
-        if element in o:
-            oxide = o
-
-    s = oxide.split("O")
-    cat_subscript = s[0]
-    an_subscript = s[1]
-
-    cat_subscript = [i for i in cat_subscript if i.isdigit()]
-    if cat_subscript:
-        cat_subscript = int(cat_subscript[0])
-    else:
-        cat_subscript = 1
-
-    an_subscript = [i for i in an_subscript if i.isdigit()]
-    if an_subscript:
-        an_subscript = int(an_subscript[0])
-    else:
-        an_subscript = 1
-
-    ppm = 1e4 * (
-        (wt_percent * mendeleev.element(element).atomic_weight * cat_subscript)
-        / (
-            mendeleev.element(element).atomic_weight
-            + mendeleev.element("O").atomic_weight * an_subscript
-        )
-    )
-    return ppm
+from ..helpers import conversions
 
 
 class LaserCalc:
     """
     # LaserCalc
 
     The class `LaserCalc` which is devoted to calculating
@@ -486,15 +71,15 @@
         self.standards_data = df.set_index("Standard")
         self.database_standards = self.standards_data.index.unique().to_list()
         # Get a list of all of the elements supported in the published standard datasheet
         # Get a second list for the same elements but their corresponding uncertainty columns
         self.standard_elements = [
             analyte
             for analyte in self.standards_data.columns.tolist()
-            if not ("_std" in analyte)
+            if "_std" not in analyte
         ]
         self.standard_element_uncertainties = [
             analyte + "_std" for analyte in self.standard_elements
         ]
 
     def get_data(self, df):
         """load in output from `LaserTRAM` for calculation of concentrations
@@ -562,15 +147,15 @@
                 or "despiked" in analyte
                 or "omitted_region" in analyte
             )
         ]
         analytes_nomass = []
         for i in range(len(self.analytes)):
             # strip the atomic number from our analyte data
-            nomass = re.split("(\d+)", self.analytes[i])[2]
+            nomass = re.split(r"(\d+)", self.analytes[i])[2]
             analytes_nomass.append(nomass)
         self.elements = analytes_nomass
 
     def set_calibration_standard(self, std):
         """Assign which standard reference material will be the calibration
         standard for calculating concentrations.
 
@@ -629,15 +214,15 @@
                         for d in self.calibration_std_data["timestamp"]
                     ]
                 ).astype(np.float64)
                 # x = np.cumsum(np.diff(x))
                 # x = np.insert(x, 0, 0).astype(np.float64)
 
             else:
-                x = self.calibration_std_data["index"]
+                x = self.calibration_std_data["index"].to_numpy()
 
             y = self.calibration_std_data.loc[:, self.analytes[j]].astype("float64")
 
             X = sm.add_constant(x)
             # Note the difference in argument order
             model = sm.OLS(y, X).fit()
             # now generate predictions
@@ -698,26 +283,26 @@
         # For our calibration standard, calculate the concentration ratio
         # of each analyte to the element used as the internal standard
         std_conc_ratios = []
         myanalytes_nomass = []
 
         for i in range(len(self.analytes)):
             # strip the atomic number from our analyte data
-            nomass = re.split("(\d+)", self.analytes[i])[2]
+            nomass = re.split(r"(\d+)", self.analytes[i])[2]
             # make it a list
             myanalytes_nomass.append(nomass)
 
             # if our element is in the list of standard elements take the ratio
             if nomass in self.standard_elements:
                 std_conc_ratios.append(
                     self.standards_data.loc[self.calibration_std, nomass]
                     / self.standards_data.loc[
                         self.calibration_std,
                         re.split(
-                            "(\d+)", self.calibration_std_data["norm"].unique()[0]
+                            r"(\d+)", self.calibration_std_data["norm"].unique()[0]
                         )[2],
                     ]
                 )
 
         # make our list an array for easier math going forward
         # std_conc_ratios = pd.DataFrame(np.array(std_conc_ratios)[np.newaxis,:],columns = myanalytes)
         self.calibration_std_conc_ratios = np.array(std_conc_ratios)
@@ -772,15 +357,15 @@
         secondary_standards_concentrations_list = []
         unknown_concentrations_list = []
 
         for sample in secondary_standards:
             Cn_u = self.standards_data.loc[
                 sample,
                 re.split(
-                    "(\d+)",
+                    r"(\d+)",
                     self.calibration_std_data["norm"].unique()[0],
                 )[2],
             ]
             Cin_std = self.calibration_std_conc_ratios
             Ni_std = self.calibration_std_stats["mean"][self.analytes]
             Ni_u = self.data.loc[sample, self.analytes]
 
@@ -845,15 +430,15 @@
                 concentrations["sample"] = sample
                 concentrations.set_index("sample", inplace=True)
 
             secondary_standards_concentrations_list.append(concentrations)
 
         ###############################
         for sample in self.samples_nostandards:
-            Cn_u = oxide_to_ppm(
+            Cn_u = conversions.oxide_to_ppm(
                 self.data.loc[sample, "internal_std_comp"],
                 self.data.loc[sample, "norm"].unique()[0],
             ).to_numpy()
             Cin_std = self.calibration_std_conc_ratios
             Ni_std = self.calibration_std_stats["mean"][self.analytes].to_numpy()
             Ni_u = self.data.loc[sample, self.analytes].to_numpy()
 
@@ -966,19 +551,20 @@
         self.unknown_concentrations.index.name = "sample"
 
     def calculate_uncertainties(self):
         """
         Calculate the uncertainties for each analysis.
 
         """
-        # self.SRM_concentration_uncertainties = 1
-        # self.unknown_concentration_uncertainties = 1
+
         myuncertainties = [analyte + "_se" for analyte in self.analytes]
-        srm_rel_uncertainties_list = []
-        unk_rel_uncertainties_list = []
+        srm_rel_ext_uncertainties_list = []
+        unk_rel_ext_uncertainties_list = []
+        srm_rel_int_uncertainties_list = []
+        unk_rel_int_uncertainties_list = []
         # use RMSE of regression for elements where drift correction is applied rather than the standard error
         # of the mean of all the calibration standard normalized ratios
         rse_i_std = []
         for analyte in self.analytes:
             if "True" in self.calibration_std_stats.loc[analyte, "drift_correct"]:
                 rse_i_std.append(
                     100
@@ -991,15 +577,15 @@
                 )
 
         rse_i_std = np.array(rse_i_std)
 
         for sample in self.secondary_standards:
             # concentration of internal standard in unknown uncertainties
             int_std_element = re.split(
-                "(\d+)", self.calibration_std_data["norm"].unique()[0]
+                r"(\d+)", self.calibration_std_data["norm"].unique()[0]
             )[2]
             t1 = (
                 self.standards_data.loc[sample, f"{int_std_element}_std"]
                 / self.standards_data.loc[sample, f"{int_std_element}"]
             ) ** 2
 
             # concentration of internal standard in calibration standard uncertainties
@@ -1008,15 +594,15 @@
                 / self.standards_data.loc[self.calibration_std, f"{int_std_element}"]
             ) ** 2
 
             # concentration of each analyte in calibration standard uncertainties
             std_conc_stds = []
             for i in range(len(self.analytes)):
                 # strip the atomic number from our analyte data
-                nomass = re.split("(\d+)", self.analytes[i])[2]
+                nomass = re.split(r"(\d+)", self.analytes[i])[2]
 
                 # if our element is in the list of standard elements take the ratio
                 if nomass in self.standard_elements:
                     std_conc_stds.append(
                         (
                             self.standards_data.loc[
                                 self.calibration_std, f"{nomass}_std"
@@ -1027,47 +613,68 @@
                     )
 
             std_conc_stds = np.array(std_conc_stds)
 
             # Overall uncertainties
             # Need to loop through each row?
 
-            rel_uncertainty = pd.DataFrame(
+            rel_ext_uncertainty = pd.DataFrame(
                 np.sqrt(
                     np.array(
                         t1
                         + t2
                         + std_conc_stds
                         + (rse_i_std[np.newaxis, :] / 100) ** 2
                         + (self.data.loc[sample, myuncertainties].to_numpy() / 100) ** 2
                     ).astype(np.float64)
                 )
             )
-            rel_uncertainty.columns = myuncertainties
-            srm_rel_uncertainties_list.append(rel_uncertainty)
+            rel_int_uncertainty = pd.DataFrame(
+                np.sqrt(
+                    np.array(
+                        t1
+                        # +t2
+                        # + std_conc_stds
+                        + (rse_i_std[np.newaxis, :] / 100) ** 2
+                        + (self.data.loc[sample, myuncertainties].to_numpy() / 100) ** 2
+                    ).astype(np.float64)
+                )
+            )
+            rel_ext_uncertainty.columns = [f"{a}_exterr" for a in self.analytes]
+            srm_rel_ext_uncertainties_list.append(rel_ext_uncertainty)
+            rel_int_uncertainty.columns = [f"{a}_interr" for a in self.analytes]
+            srm_rel_int_uncertainties_list.append(rel_int_uncertainty)
 
-        srm_rel_uncertainties = pd.concat(srm_rel_uncertainties_list)
+        srm_rel_ext_uncertainties = pd.concat(srm_rel_ext_uncertainties_list)
+        srm_rel_int_uncertainties = pd.concat(srm_rel_int_uncertainties_list)
 
-        srm_uncertainties = pd.DataFrame(
-            srm_rel_uncertainties.values
+        srm_ext_uncertainties = pd.DataFrame(
+            srm_rel_ext_uncertainties.values
+            * self.SRM_concentrations.loc[:, self.analytes].values,
+            columns=[f"{a}_exterr" for a in self.analytes],
+            index=self.SRM_concentrations.index,
+        )
+        srm_int_uncertainties = pd.DataFrame(
+            srm_rel_int_uncertainties.values
             * self.SRM_concentrations.loc[:, self.analytes].values,
-            columns=myuncertainties,
+            columns=[f"{a}_interr" for a in self.analytes],
             index=self.SRM_concentrations.index,
         )
 
         self.SRM_concentrations = pd.concat(
-            [self.SRM_concentrations, srm_uncertainties], axis="columns"
+            [self.SRM_concentrations, srm_ext_uncertainties, srm_int_uncertainties],
+            axis="columns",
         )
 
         ######################################
 
         for sample in self.samples_nostandards:
             # concentration of internal standard in unknown uncertainties
             int_std_element = re.split(
-                "(\d+)", self.calibration_std_data["norm"].unique()[0]
+                r"(\d+)", self.calibration_std_data["norm"].unique()[0]
             )[2]
             # concentration of internal standard in unknown uncertainties
             t1 = (self.data.loc[sample, "internal_std_rel_unc"] / 100) ** 2
             t1 = np.array(t1)
             t1 = t1[:, np.newaxis]
 
             # concentration of internal standard in calibration standard uncertainties
@@ -1076,15 +683,15 @@
                 / self.standards_data.loc[self.calibration_std, f"{int_std_element}"]
             ) ** 2
 
             # concentration of each analyte in calibration standard uncertainties
             std_conc_stds = []
             for i in range(len(self.analytes)):
                 # strip the atomic number from our analyte data
-                nomass = re.split("(\d+)", self.analytes[i])[2]
+                nomass = re.split(r"(\d+)", self.analytes[i])[2]
 
                 # if our element is in the list of standard elements take the ratio
                 if nomass in self.standard_elements:
                     std_conc_stds.append(
                         (
                             self.standards_data.loc[
                                 self.calibration_std, f"{nomass}_std"
@@ -1095,54 +702,80 @@
                     )
 
             std_conc_stds = np.array(std_conc_stds)
 
             # Overall uncertainties
             # Need to loop through each row?
 
-            rel_uncertainty = pd.DataFrame(
+            rel_ext_uncertainty = pd.DataFrame(
                 np.sqrt(
                     np.array(
                         t1
                         + t2
                         + std_conc_stds
                         + (rse_i_std[np.newaxis, :] / 100) ** 2
                         + (self.data.loc[sample, myuncertainties].to_numpy() / 100) ** 2
                     ).astype(np.float64)
                 )
             )
-            rel_uncertainty.columns = myuncertainties
-            unk_rel_uncertainties_list.append(rel_uncertainty)
+            rel_int_uncertainty = pd.DataFrame(
+                np.sqrt(
+                    np.array(
+                        t1
+                        # +t2
+                        # + std_conc_stds
+                        + (rse_i_std[np.newaxis, :] / 100) ** 2
+                        + (self.data.loc[sample, myuncertainties].to_numpy() / 100) ** 2
+                    ).astype(np.float64)
+                )
+            )
+            rel_ext_uncertainty.columns = [f"{a}_exterr" for a in self.analytes]
+            unk_rel_ext_uncertainties_list.append(rel_ext_uncertainty)
+            rel_int_uncertainty.columns = [f"{a}_interr" for a in self.analytes]
+            unk_rel_int_uncertainties_list.append(rel_int_uncertainty)
+
+        unk_rel_ext_uncertainties = pd.concat(unk_rel_ext_uncertainties_list)
+        unk_rel_int_uncertainties = pd.concat(unk_rel_int_uncertainties_list)
 
-        unk_rel_uncertainties = pd.concat(unk_rel_uncertainties_list)
+        unknown_ext_uncertainties = pd.DataFrame(
+            unk_rel_ext_uncertainties.values
+            * self.unknown_concentrations.loc[:, self.analytes].values,
+            columns=[f"{a}_exterr" for a in self.analytes],
+            index=self.unknown_concentrations.index,
+        )
 
-        unknown_uncertainties = pd.DataFrame(
-            unk_rel_uncertainties.values
+        unknown_int_uncertainties = pd.DataFrame(
+            unk_rel_int_uncertainties.values
             * self.unknown_concentrations.loc[:, self.analytes].values,
-            columns=myuncertainties,
+            columns=[f"{a}_interr" for a in self.analytes],
             index=self.unknown_concentrations.index,
         )
 
         self.unknown_concentrations = pd.concat(
-            [self.unknown_concentrations, unknown_uncertainties], axis="columns"
+            [
+                self.unknown_concentrations,
+                unknown_ext_uncertainties,
+                unknown_int_uncertainties,
+            ],
+            axis="columns",
         )
 
     # make an accuracy checking function
     # need to use analytes no mass to check SRM vals
     def get_secondary_standard_accuracies(self):
         """
         calculate the accuracy of each secondary standard where accuracy is 100 * measured / accepted value
 
         Here `accepted` value is the GEOREM preferred value for that SRM analyte pair.
 
         """
         df_list = []
 
         nomass = [
-            re.split("(\d+)", self.analytes[i])[2] for i in range(len(self.analytes))
+            re.split(r"(\d+)", self.analytes[i])[2] for i in range(len(self.analytes))
         ]
 
         for standard in self.secondary_standards:
             df = pd.DataFrame(
                 100
                 * self.SRM_concentrations.loc[standard, self.analytes]
                 .replace("b.d.l.", np.nan)
```

### Comparing `lasertram-0.0.9/lasertram.egg-info/PKG-INFO` & `lasertram-0.1.0/lasertram.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lasertram
-Version: 0.0.9
+Version: 0.1.0
 Summary: For processing LA-ICP-MS data
 Home-page: https://github.com/jlubbersgeo/lasertram
 Author: Jordan Lubbers
 Author-email: jelubber@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lasertram-0.0.9/setup.cfg` & `lasertram-0.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lasertram
-version = 0.0.9
+version = 0.1.0
 author = Jordan Lubbers
 author_email = jelubber@gmail.com
 description = For processing LA-ICP-MS data
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jlubbersgeo/lasertram
 classifiers =
```

