# Comparing `tmp/omniplate-1.0.tar.gz` & `tmp/omniplate-1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omniplate-1.0.tar", max compression
+gzip compressed data, was "omniplate-1.0a0.tar", max compression
```

## Comparing `omniplate-1.0.tar` & `omniplate-1.0a0.tar`

### file list

```diff
@@ -1,30 +1,32 @@
--rw-r--r--   0        0        0      244 2024-03-04 11:11:29.000000 omniplate-1.0/README.md
--rw-r--r--   0        0        0      201 2024-03-08 17:39:22.000000 omniplate-1.0/omniplate/__init__.py
--rw-r--r--   0        0        0     4144 2024-03-08 12:52:20.000000 omniplate-1.0/omniplate/admin.py
--rw-r--r--   0        0        0     1289 2024-03-08 11:28:12.000000 omniplate-1.0/omniplate/clogger.py
--rw-r--r--   0        0        0    42927 2024-03-14 12:17:45.904010 omniplate-1.0/omniplate/corrections.py
--rw-r--r--   0        0        0     1380 2024-03-08 11:28:21.000000 omniplate-1.0/omniplate/dilution_data_lucia.tsv
--rw-r--r--   0        0        0     1893 2024-03-08 11:28:21.000000 omniplate-1.0/omniplate/dilution_data_xiao.tsv
--rw-r--r--   0        0        0     9484 2024-03-14 12:17:12.097073 omniplate-1.0/omniplate/getstats.py
--rw-r--r--   0        0        0    12643 2024-03-13 13:23:18.000000 omniplate-1.0/omniplate/loaddata.py
--rw-r--r--   0        0        0    19121 2024-03-21 16:51:56.721344 omniplate-1.0/omniplate/manipulatedfs.py
--rw-r--r--   0        0        0     8474 2024-03-09 17:49:24.000000 omniplate-1.0/omniplate/midlog.py
--rw-r--r--   0        0        0    10217 2024-03-14 12:18:53.929142 omniplate-1.0/omniplate/misc.py
--rw-r--r--   0        0        0     2577 2024-03-08 11:28:12.000000 omniplate-1.0/omniplate/old_analyseOldTecan.py
--rw-r--r--   0        0        0     2609 2024-03-08 11:28:12.000000 omniplate-1.0/omniplate/old_analyseTecan.py
--rw-r--r--   0        0        0      435 2024-03-08 11:28:12.000000 omniplate-1.0/omniplate/omerrors.py
--rw-r--r--   0        0        0    12992 2024-03-09 12:23:12.000000 omniplate-1.0/omniplate/omfitderiv.py
--rw-r--r--   0        0        0     3925 2024-03-08 11:28:12.000000 omniplate-1.0/omniplate/omgenutils.py
--rw-r--r--   0        0        0     3274 2024-03-08 12:42:05.000000 omniplate-1.0/omniplate/ominfo.py
--rw-r--r--   0        0        0     6091 2024-03-08 15:30:48.000000 omniplate-1.0/omniplate/omio.py
--rw-r--r--   0        0        0    21013 2024-03-14 12:18:28.204783 omniplate-1.0/omniplate/omplot.py
--rw-r--r--   0        0        0     6794 2024-03-08 11:28:12.000000 omniplate-1.0/omniplate/omstats.py
--rw-r--r--   0        0        0     6907 2024-03-08 12:21:15.000000 omniplate-1.0/omniplate/omwells.py
--rw-r--r--   0        0        0      797 2024-03-08 11:28:12.000000 omniplate-1.0/omniplate/parseSunrise.py
--rw-r--r--   0        0        0     1598 2024-03-08 11:28:12.000000 omniplate-1.0/omniplate/parseTecan.py
--rw-r--r--   0        0        0     2898 2024-03-08 15:11:40.000000 omniplate-1.0/omniplate/parseplate.py
--rw-r--r--   0        0        0     6161 2024-03-14 12:18:04.994595 omniplate-1.0/omniplate/platereader.py
--rw-r--r--   0        0        0     6321 2024-03-09 11:56:29.000000 omniplate-1.0/omniplate/runfitderiv.py
--rw-r--r--   0        0        0     5120 2024-03-09 10:25:17.000000 omniplate-1.0/omniplate/sunder.py
--rw-r--r--   0        0        0     1107 2024-03-08 17:56:09.000000 omniplate-1.0/pyproject.toml
--rw-r--r--   0        0        0     1532 1970-01-01 00:00:00.000000 omniplate-1.0/PKG-INFO
+-rw-r--r--   0        0        0      244 2024-03-04 11:11:29.000000 omniplate-1.0a0/README.md
+-rw-r--r--   0        0        0      201 2024-03-08 17:39:22.000000 omniplate-1.0a0/omniplate/__init__.py
+-rw-r--r--   0        0        0     4163 2024-04-12 15:46:43.988619 omniplate-1.0a0/omniplate/admin.py
+-rw-r--r--   0        0        0     1289 2024-03-08 11:28:12.000000 omniplate-1.0a0/omniplate/clogger.py
+-rw-r--r--   0        0        0    12877 2024-04-18 12:59:13.108428 omniplate-1.0a0/omniplate/correctauto_bayesian.py
+-rw-r--r--   0        0        0    41253 2024-04-18 11:20:14.135894 omniplate-1.0a0/omniplate/corrections.py
+-rw-r--r--   0        0        0     1380 2024-03-08 11:28:21.000000 omniplate-1.0a0/omniplate/dilution_data_lucia.tsv
+-rw-r--r--   0        0        0     1893 2024-03-08 11:28:21.000000 omniplate-1.0a0/omniplate/dilution_data_xiao.tsv
+-rw-r--r--   0        0        0     9484 2024-03-14 12:17:12.097073 omniplate-1.0a0/omniplate/getstats.py
+-rw-r--r--   0        0        0    12333 2024-03-31 12:04:44.000000 omniplate-1.0a0/omniplate/loaddata.py
+-rw-r--r--   0        0        0    19121 2024-03-21 16:51:56.721344 omniplate-1.0a0/omniplate/manipulatedfs.py
+-rw-r--r--   0        0        0     8791 2024-04-12 15:48:50.293118 omniplate-1.0a0/omniplate/midlog.py
+-rw-r--r--   0        0        0    10217 2024-03-14 12:18:53.929142 omniplate-1.0a0/omniplate/misc.py
+-rw-r--r--   0        0        0     2577 2024-03-08 11:28:12.000000 omniplate-1.0a0/omniplate/old_analyseOldTecan.py
+-rw-r--r--   0        0        0     2609 2024-03-08 11:28:12.000000 omniplate-1.0a0/omniplate/old_analyseTecan.py
+-rw-r--r--   0        0        0      435 2024-03-08 11:28:12.000000 omniplate-1.0a0/omniplate/omerrors.py
+-rw-r--r--   0        0        0    12992 2024-04-15 18:29:26.000000 omniplate-1.0a0/omniplate/omfitderiv.py
+-rw-r--r--   0        0        0     3925 2024-03-08 11:28:12.000000 omniplate-1.0a0/omniplate/omgenutils.py
+-rw-r--r--   0        0        0     3274 2024-03-08 12:42:05.000000 omniplate-1.0a0/omniplate/ominfo.py
+-rw-r--r--   0        0        0     6320 2024-03-27 15:57:57.000000 omniplate-1.0a0/omniplate/omio.py
+-rw-r--r--   0        0        0    21013 2024-03-14 12:18:28.204783 omniplate-1.0a0/omniplate/omplot.py
+-rw-r--r--   0        0        0     6794 2024-03-08 11:28:12.000000 omniplate-1.0a0/omniplate/omstats.py
+-rw-r--r--   0        0        0     6907 2024-03-08 12:21:15.000000 omniplate-1.0a0/omniplate/omwells.py
+-rw-r--r--   0        0        0      797 2024-03-08 11:28:12.000000 omniplate-1.0a0/omniplate/parseSunrise.py
+-rw-r--r--   0        0        0     1598 2024-03-08 11:28:12.000000 omniplate-1.0a0/omniplate/parseTecan.py
+-rw-r--r--   0        0        0     2898 2024-03-08 15:11:40.000000 omniplate-1.0a0/omniplate/parseplate.py
+-rw-r--r--   0        0        0     6199 2024-03-31 12:15:36.000000 omniplate-1.0a0/omniplate/platereader.py
+-rw-r--r--   0        0        0     6620 2024-03-31 16:27:06.000000 omniplate-1.0a0/omniplate/promoteractivity.py
+-rw-r--r--   0        0        0     6232 2024-04-15 18:27:00.000000 omniplate-1.0a0/omniplate/runfitderiv.py
+-rw-r--r--   0        0        0     5285 2024-03-25 14:18:47.000000 omniplate-1.0a0/omniplate/sunder.py
+-rw-r--r--   0        0        0     1108 2024-04-25 14:26:31.547279 omniplate-1.0a0/pyproject.toml
+-rw-r--r--   0        0        0     1534 1970-01-01 00:00:00.000000 omniplate-1.0a0/PKG-INFO
```

### Comparing `omniplate-1.0/omniplate/admin.py` & `omniplate-1.0a0/omniplate/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,17 @@
     # find any extra columns
     good_columns = [
         "experiment",
         "condition",
         "strain",
         "time",
         "well",
-    ] + list(set([dtype for e in self.datatypes for dtype in self.datatypes[e]]))
+    ] + list(
+        set([dtype for e in self.datatypes for dtype in self.datatypes[e]])
+    )
     bad_columns = [col for col in rdf.columns if col not in good_columns]
     if bad_columns:
         print()
         for column in bad_columns:
             print(f"Dropping {column} when making s dataframe.")
         rdf = rdf.drop(columns=bad_columns)
     # find means
@@ -97,15 +99,15 @@
         self.s = gu.absorbdf(
             self.s,
             outdf,
             ["experiment", "condition", "strain", "time"],
         )
 
 
-def add_to_sc(self, statsdict):
+def add_dict_to_sc(self, statsdict):
     """Add one-line dict to sc dataframe."""
     statsdf = pd.DataFrame(statsdict, index=pd.RangeIndex(0, 1, 1))
     newstats = np.count_nonzero(
         [True if stat not in self.sc.columns else False for stat in statsdict]
     )
     if newstats:
         # add new columns to sc dataframe
```

### Comparing `omniplate-1.0/omniplate/clogger.py` & `omniplate-1.0a0/omniplate/clogger.py`

 * *Files identical despite different names*

### Comparing `omniplate-1.0/omniplate/corrections.py` & `omniplate-1.0a0/omniplate/corrections.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,24 +14,27 @@
 
 import omniplate.admin as admin
 import omniplate.omerrors as errors
 import omniplate.omgenutils as gu
 import omniplate.sunder as sunder
 from omniplate.runfitderiv import runfitderiv
 import omniplate.clogger as clogger
+from omniplate.correctauto_bayesian import correctauto_bayesian
 
 
 @clogger.log
 def correctOD(
     self,
     figs=True,
     bd=None,
     gp_results=False,
     ODfname=None,
     odmatch_min=0.1,
+    correctformedia=True,
+    frac=0.33,
     experiments="all",
     experimentincludes=False,
     experimentexcludes=False,
     conditions="all",
     conditionincludes=False,
     conditionexcludes=False,
 ):
@@ -60,14 +63,19 @@
     ODfname: string, optional
         The name of the file with the dilution data used to correct OD for
         its non-linear dependence on numbers of cells. If unspecified, data
         for haploid budding yeast growing in glucose is used.
     odmatch_min: float, optional
         An expected minimal value of the OD up to which there is a linear
         scaling of the OD with cell numbers.
+    correctformedia: boolean, optional
+        If True (default), correct OD for background levels from media.
+    frac: float
+        The fraction of the data used for smoothing the media OD via lowess.
+        Used to correct OD for the background OD of the media.
     experiments: string or list of strings
         The experiments to include.
     conditions: string or list of strings
         The conditions to include.
     experimentincludes: string, optional
         Selects only experiments that include the specified string in their
         name.
@@ -103,73 +111,176 @@
         nomedia=False,
     )
     # fit dilution data
     gc, odmatch = findODcorrection(
         self.wdirpath, ODfname, figs, bd, gp_results, odmatch_min
     )
     # correct ODs
-    for exp in exps:
+    for e in exps:
         for c in cons:
-            if self.sc[(self.sc.experiment == exp) & (self.sc.condition == c)][
+            if self.sc[(self.sc.experiment == e) & (self.sc.condition == c)][
                 "OD_corrected"
             ].any():
-                print(f"{exp}: OD is already corrected for {c}.")
+                print(f"{e}: OD is already corrected for {c}.")
             else:
+                if correctformedia:
+                    print("Corrected for the background OD of the media.")
+                    correctODformedia(
+                        self, figs=figs, frac=frac, experiments=e, conditions=c
+                    )
                 # correct all wells
                 r_data = self.r.query(
-                    "experiment == @exp and condition == @c"
-                )["OD"].to_numpy()
+                    "experiment == @e and condition == @c"
+                ).OD.to_numpy()
                 gc.batchpredict(r_data)
                 # leave small ODs unchanged
                 new_r = gc.f
                 new_r[r_data < odmatch] = r_data[r_data < odmatch]
                 # update r data frame
                 self.r.loc[
-                    (self.r.experiment == exp) & (self.r.condition == c),
+                    (self.r.experiment == e) & (self.r.condition == c),
                     "OD",
                 ] = new_r
                 # flag corrections in summary stats dataframe
                 self.sc.loc[
-                    (self.sc.experiment == exp) & (self.sc.condition == c),
+                    (self.sc.experiment == e) & (self.sc.condition == c),
                     "OD_corrected",
                 ] = True
     # update s dataframe
     admin.update_s(self)
 
 
+def findODcorrection(wdirpath, ODfname, figs, bd, gp_results, odmatch_min):
+    """
+    Determine a function to correct OD.
+
+    Use a Gaussian process to fit serial dilution data to correct for
+    non-linearities in the relationship between OD and cell density.
+
+    The data are either loaded from file ODfname or the default
+    data for haploid yeast growing in glucose are used.
+    """
+    print("Fitting dilution data for OD correction for non-linearities.")
+    if ODfname is not None:
+        try:
+            od_df = pd.read_csv(
+                str(wdirpath / ODfname), sep=None, engine="python", header=None
+            )
+            print(f"Using {ODfname}")
+            od_data = od_df.to_numpy()
+            od, dilfac = od_data[:, 0], od_data[:, 1]
+        except (FileNotFoundError, OSError):
+            raise errors.FileNotFound(str(wdirpath / ODfname))
+    else:
+        print("Using default data.")
+        fname = "dilution_data_xiao.tsv"
+        od, dilfac = read_dilution_data(fname)
+    od, dilfac = arrange_into_replicates(od, dilfac)
+    # run nunchaku
+    X = np.mean(dilfac, 1)
+    nc = Nunchaku(X, od.T, estimate_err=True, prior=[-5, 5])
+    num_regions, _ = nc.get_number(4)
+    bds, _ = nc.get_iboundaries(num_regions)
+    # find linear region, which starts from origin
+    odmatch_pts = np.mean(od, 1)[bds]
+    # pick end point with OD at least equal to odmatch_min
+    ipick = np.where(odmatch_pts > odmatch_min)[0][0]
+    odmatch = odmatch_pts[ipick]
+    dilfacmatch = X[bds[ipick]]
+    # process data
+    dilfac = dilfac.flatten()[np.argsort(od.flatten())]
+    od = np.sort(od.flatten())
+    # rescale so that OD and dilfac match
+    y = dilfac / dilfacmatch * odmatch
+    # set up Gaussian process
+    bds = {0: (-4, 4), 1: (-4, 4), 2: (-3, -1)}
+    # find bounds
+    if bd is not None:
+        bds = gu.mergedicts(original=bds, update=bd)
+    gc = gp.maternGP(bds, od, y)
+    # run Gaussian process
+    gc.findhyperparameters(noruns=5, exitearly=True, quiet=True)
+    if gp_results:
+        gc.results()
+    gc.predict(od)
+    if figs:
+        plt.figure()
+        gc.sketch(".")
+        plt.plot(odmatch, odmatch, "bs")
+        plt.grid(True)
+        plt.xlabel("OD")
+        plt.ylabel("corrected OD (relative cell numbers)")
+        if ODfname:
+            plt.title("Fitting " + ODfname)
+        else:
+            plt.title("for haploid budding yeast in glucose")
+        plt.show(block=False)
+    return gc, odmatch
+
+
+def read_dilution_data(fname):
+    d = import_files.read_text("omniplate", fname)
+    res = np.array(re.split(r"\n|\t", d)[:-1]).astype(float)
+    od, dilfac = res[::2], res[1::2]
+    if fname == "dilution_data_xiao.tsv":
+        # missing replicate - use mean of existing ones
+        dilfac = np.insert(dilfac, 0, dilfac[0])
+        od = np.insert(od, 0, np.mean(od[:2]))
+    else:
+        raise SystemExit("Dilution data unrecognised.")
+    return od, dilfac
+
+
+def arrange_into_replicates(od, dilfac):
+    """Rearrange so that data from each replicate is in a column."""
+    udilfac, indices, counts = np.unique(
+        dilfac, return_inverse=True, return_counts=True
+    )
+    ucounts = np.unique(counts)
+    if len(ucounts) == 1:
+        noreps = np.unique(counts)[0]
+        dilfac_reps = np.tile(np.atleast_2d(udilfac).T, noreps)
+        od_reps = np.array(
+            [od[indices == i] for i in range(udilfac.size)]
+        ).reshape((udilfac.size, noreps))
+        return od_reps, dilfac_reps
+    else:
+        raise Exception(
+            "There are inconsistent numbers of replicates"
+            " in the OD correction data."
+        )
+
+
 @clogger.log
-def correctmedia(
+def correctODformedia(
     self,
-    datatypes="all",
-    commonmedia=False,
+    figs=False,
+    frac=0.33,
     experiments="all",
     experimentincludes=False,
     experimentexcludes=False,
     conditions="all",
     conditionincludes=False,
     conditionexcludes=False,
-    figs=False,
-    log=True,
-    frac=0.33,
 ):
     """
     Correct OD or fluorescence for that of the media.
 
     Data from wells marked Null is used.
 
     Uses lowess to smooth measurements of from all Null wells and subtracts
     this smoothed time series from the raw data.
 
     Parameters
     ----------
-    datatypes: string or list of strings
-        Data types to be corrected.
-    commonmedia: string
-        A condition containing Null wells that should be used to correct
-        media for other conditions.
+    figs: boolean, optional
+        If True, display fits to data for the Null wells.
+    frac: float
+        The fraction of the data used for smoothing via lowess.
+        https://www.statsmodels.org/devel/generated/statsmodels.nonparametric.smoothers_lowess.lowess.html
     experiments: string or list of strings
         The experiments to include.
     conditions: string or list of strings
         The conditions to include.
     experimentincludes: string, optional
         Selects only experiments that include the specified string in their
         name.
@@ -177,25 +288,18 @@
         Ignores experiments that include the specified string in their
         name.
     conditionincludes: string, optional
         Selects only conditions that include the specified string in their
         name.
     conditionexcludes: string, optional
         Ignores conditions that include the specified string in their name.
-    figs: boolean, optional
-        If True, display fits to data for the Null wells.
-    frac: float
-        The fraction of the data used for smoothing via lowess.
-        https://www.statsmodels.org/devel/generated/statsmodels.nonparametric.smoothers_lowess.lowess.html
 
     Examples
     --------
-    >>> p.correctmedia()
-    >>> p.correctmedia('OD')
-    >>> p.correctmedia(commonmedia= '1% Glu')
+    >>> p.correctODformedia()
     """
     exps = sunder.getset(
         self,
         experiments,
         experimentincludes,
         experimentexcludes,
         "experiment",
@@ -206,87 +310,136 @@
         conditions,
         conditionincludes,
         conditionexcludes,
         "condition",
         nonull=True,
         nomedia=False,
     )
-    for exp in exps:
-        # data types
-        expdatatypes = (
-            self.datatypes[exp]
-            if datatypes == "all"
-            else gu.makelist(datatypes)
-        )
-        # correct for media
-        for dtype in expdatatypes:
-            for c in cons:
-                if self.sc[
-                    (self.sc.experiment == exp) & (self.sc.condition == c)
-                ][dtype + "_corrected_for_media"].any():
-                    print(
-                        f"{exp}: {dtype} is already corrected for media"
-                        f" in {c}."
+    for e in exps:
+        for c in cons:
+            if self.sc[(self.sc.experiment == e) & (self.sc.condition == c)][
+                "OD_corrected_for_media"
+            ].any():
+                print(f"{e}: OD for {c} is already corrected for media.")
+            else:
+                if c in self.allconditions[e]:
+                    print(f"{e}: Correcting OD for {c} for media.")
+                    negvalues = find_Null_and_correct(
+                        self, self.r, "OD", e, c, figs, frac
                     )
-                else:
-                    if c in self.allconditions[exp]:
-                        print(f"{exp}: Correcting {dtype} for media in {c}.")
-                        cm = commonmedia if commonmedia else c
-                        # update r dataframe
-                        (
-                            success,
-                            negvalues,
-                        ) = performmediacorrection(
-                            self.r, dtype, exp, c, figs, cm, frac
-                        )
-                        if success:
-                            self.sc.loc[
-                                (self.sc.experiment == exp)
-                                & (self.sc.condition == c),
-                                dtype + "_corrected_for_media",
-                            ] = True
-                            if negvalues:
-                                if not self.progress["negativevalues"][exp]:
-                                    self.progress["negativevalues"][
-                                        exp
-                                    ] = negvalues
-                                else:
-                                    self.progress["negativevalues"][
-                                        exp
-                                    ] += negvalues
-        if self.progress["negativevalues"][exp]:
-            print(
-                "\nWarning: correcting media has created negative "
-                f"values in {exp} for"
-            )
-            print(self.progress["negativevalues"][exp])
+                    if negvalues is not None:
+                        if not self.progress["negativevalues"][e]:
+                            self.progress["negativevalues"][e] = negvalues
+                        else:
+                            self.progress["negativevalues"][e] += negvalues
+    if self.progress["negativevalues"][e]:
+        print(
+            "\nWarning: correcting OD for media has created negative "
+            f"values in {e} for"
+        )
+        print(self.progress["negativevalues"][e])
     # update s dataframe
     admin.update_s(self)
 
 
+def find_Null_and_correct(self, df, dtype, e, c, figs, frac):
+    """Find data for Null strain and pass to performmediacorrection."""
+    null_df = self.r[
+        (self.r.experiment == e)
+        & (self.r.condition == c)
+        & (self.r.strain == "Null")
+    ]
+    if null_df.empty:
+        print(f"{e}: No Null strain found for {c}.")
+    else:
+        negvalues = performmediacorrection(
+            null_df, df, dtype, e, c, figs, frac
+        )
+        return negvalues
+
+
+def performmediacorrection(
+    null_df, df, dtype, experiment, condition, figs, frac
+):
+    """
+    Correct data of type dtype for any signal from the media.
+
+    Data for the Null strain is in null_df; data to be ovewritten
+    is in df.
+
+    Use lowess to smooth over time the media data from the Null
+    wells and subtract the smoothed values from the data.
+    """
+    t, data = null_df["time"].to_numpy(), null_df[dtype].to_numpy()
+    if ~np.any(data[~np.isnan(data)]):
+        # all data is NaN
+        return
+    # find correction
+    res = lowess(data, t, frac=frac)
+    correctionfn = interp1d(
+        res[:, 0],
+        res[:, 1],
+        fill_value=(res[0, 1], res[-1, 1]),
+        bounds_error=False,
+    )
+    if figs:
+        plt.figure()
+        plt.plot(t, data, "ro", res[:, 0], res[:, 1], "b-")
+        plt.xlabel("time (hours)")
+        plt.title(
+            f"{experiment}: media correction for {dtype} in {condition}."
+        )
+        plt.show(block=False)
+    # perform correction to data in df
+    choose = (df.experiment == experiment) & (df.condition == condition)
+    df.loc[choose, dtype] = df[choose][dtype] - correctionfn(
+        df[choose]["time"]
+    )
+    # check for any negative values
+    negvalues = ""
+    for s in np.unique(df[choose]["strain"][df[choose][dtype] < 0]):
+        if s != "Null":
+            wstr = f"\t{dtype}: {s} in {condition} for wells "
+            for well in np.unique(
+                df[choose][df[choose].strain == s]["well"][
+                    df[choose][dtype] < 0
+                ]
+            ):
+                wstr += f"{well}, "
+            wstr = wstr[:-2] + "\n"
+            negvalues += wstr
+    return negvalues
+
+
 @clogger.log
 def correctauto(
     self,
     f=["GFP", "AutoFL"],
     refstrain="WT",
+    usebayesian=False,
     figs=True,
     useGPs=True,
     flcvfn="matern",
     bd=None,
     nosamples=1000,
+    max_data_pts=None,
+    frac=0.33,
+    commonmedia=None,
+    nosamples_for_fl=10,
+    nosamples_for_ra=100,
+    nosamples_for_bg=100,
     experiments="all",
     experimentincludes=False,
     experimentexcludes=False,
     conditions="all",
     conditionincludes=False,
     conditionexcludes=False,
     strains="all",
     strainincludes=False,
     strainexcludes=False,
-    **kwargs,
 ):
     """
     Correct fluorescence for autofluorescence.
 
     The correction is made using the fluorescence of an untagged
     reference strain.
 
@@ -302,29 +455,53 @@
 
     Arguments
     --
     f: string or list of strings
         The fluorescence measurements, typically either ['mCherry'] or
         ['GFP', 'AutoFL'].
     refstrain: string
-        The reference strain.
+        The reference strain used to estimate autofluorescence.
+    usebayesian: boolean
+        If True, use a Bayesian method that is more accurate for low
+        fluorescence if slower.
     figs: boolean
         If True, display plots showing the fits to the reference strain's
         fluorescence.
     useGPs: boolean
         If True, use Gaussian processes to generate extra samples from
         the replicates. Recommended, particularly if there are only a few
         replicates, but slower.
     flcvfn: str, optional
         The covariance function to use for the Gaussian process applied
         to the logarithm of the fluorescence.
     bd: dict, optional
         Specifies the bounds on the hyperparameters for the Gaussian
         process applied to the logarithm of the fluorescence,
         e.g. {2: (-2, 0)}.
+    nosamples: int, optional
+        The number of samples to take when using Gaussian processes.
+    max_data_pts: int, optional
+        The maximum number of data points to use for the Gaussian process.
+        Too many data points, over 1500, can be slow.
+    nosamples_for_fl: int, optional
+        The number of samples of the posterior of the fluorescence when
+        using the Bayesian method.
+    nosamples_for_bg: int, optional
+        The number of samples of the background fluorescence when using the
+        Bayesian method.
+    frac: float, optional
+        Only when correcting with two fluorescence measurements and using
+        not Bayesian.
+        The fraction of the data used for smoothing via lowess.
+        https://www.statsmodels.org/devel/generated/statsmodels.nonparametric.smoothers_lowess.lowess.html
+    commonmedia: string, optional
+        Only when correcting with two fluorescence measurements and using
+        not Bayesian.
+        A condition containing Null wells that should be used to correct
+        media for other conditions.
     experiments: string or list of strings
         The experiments to include.
     conditions: string or list of strings
         The conditions to include.
     strains: string or list of strings
         The strains to include.
     experimentincludes: string, optional
@@ -339,61 +516,29 @@
     conditionexcludes: string, optional
         Ignores conditions that include the specified string in their name.
     strainincludes: string, optional
         Selects only strains that include the specified string in their
         name.
     strainexcludes: string, optional
         Ignores strains that include the specified string in their name.
-    **kwargs: passed to fitderiv when fitting the fluorescence.
-
-    Notes
-    -----
-    In principle
-
-    >>> p.correctmedia()
-
-    should be run before running correctauto when processing data with two
-    fluorescence measurements.
-
-    It is unnecessary with only one fluorescence measurement because the
-    normalisation is then done directly with the reference strain's
-    fluorescence and this fluorescence can include the fluorescence from
-    the media.
-
-    In practice, running correctmedia may generate negative values of the
-    fluorescence at some time points. These negative values will create
-    NaNs in the corrected fluorescence, which are normally harmless.
-
-    With sufficiently many negative values of the fluorescence, however,
-    correcting data with two fluorescence measurements can become
-    corrupted.
 
-    If correctmedia generates negative fluorescence values, we therefore
-    recommend comparing the corrected fluorescence between
-
-    >>> p.correctmedia()
-    >>> p.correctauto(['GFP', 'AutoFL')
-
-    and
-
-    >>> p.correctauto('GFP')
-
-    to determine if these negative values are deleterious.
 
     Examples
     --------
     To correct data with one type of fluorescence measurement, use:
 
     >>> p.correctauto('GFP')
     >>> p.correctauto('mCherry', refstrain= 'BY4741')
 
     To correct data with two types of fluorescence measurement, use:
 
     >>> p.correctauto(['GFP', 'AutoFL'])
-    >>> p.correctauto(['GFP', 'AutoFL'], refstrain= 'wild-type')
+    >>> p.correctauto(['GFP', 'AutoFL'], refstrain= 'WT')
+    >>> p.correctauto(['GFP', 'AutoFL'], refstrain= 'WT', useGPs=False)
+    >>> p.correctauto(['GFP', 'AutoFL'], refstrain= 'WT', bayesian=True)
 
     References
     ----------
     S Berthoumieux, H De Jong, G Baptist, C Pinel, C Ranquet, D Ropers,
     J Geiselmann (2013).
     Shared control of gene expression in bacteria by transcription factors
     and global physiology of the cell.
@@ -404,17 +549,15 @@
     measurements of gene expression in plate readers.
     BMC Biotech, 14, 1-11.
 
     I Mihalcescu, MVM Gateau, B Chelli, C Pinel, JL Ravanat (2015).
     Green autofluorescence, a double edged monitoring tool for bacterial
     growth and activity in micro-plates.
     Phys Biol, 12, 066016.
-
     """
-    admin.check_kwargs(kwargs)
     f = gu.makelist(f)
     exps, cons, _ = sunder.getall(
         self,
         experiments,
         experimentincludes,
         experimentexcludes,
         conditions,
@@ -435,325 +578,105 @@
                         and c in self.progress["negativevalues"][e]
                     ):
                         print(
                             f"{e}: The negative values for {datatype}"
                             f" in {c} will generate NaNs."
                         )
     # going ahead
-    print(f"Using {refstrain} as the reference.")
+    print(f"\nCorrecting autofluorescence using {refstrain} as the reference.")
     # correct for autofluorescence
-    if len(f) == 2:
+    if len(f) == 2 and usebayesian:
+        correctauto_bayesian(
+            self,
+            f,
+            refstrain,
+            flcvfn,
+            bd,
+            max_data_pts,
+            nosamples_for_fl,
+            nosamples_for_ra,
+            nosamples_for_bg,
+            nosamples,
+            experiments,
+            experimentincludes,
+            experimentexcludes,
+            conditions,
+            conditionincludes,
+            conditionexcludes,
+            strains,
+            strainincludes,
+            strainexcludes,
+        )
+    elif len(f) == 2:
         correctauto2(
             self,
             f,
             refstrain,
             figs,
             useGPs,
             flcvfn,
             bd,
             nosamples,
+            max_data_pts,
+            frac,
+            commonmedia,
             experiments,
             experimentincludes,
             experimentexcludes,
             conditions,
             conditionincludes,
             conditionexcludes,
             strains,
             strainincludes,
             strainexcludes,
-            **kwargs,
         )
     elif len(f) == 1:
         correctauto1(
             self,
             f,
             refstrain,
             figs,
             useGPs,
             flcvfn,
             bd,
             nosamples,
+            max_data_pts,
             experiments,
             experimentincludes,
             experimentexcludes,
             conditions,
             conditionincludes,
             conditionexcludes,
             strains,
             strainincludes,
             strainexcludes,
-            **kwargs,
         )
     else:
         print(f"f = {f} must be a list of length 1 or 2.")
 
 
-def corrections(
-    self,
-    experiments="all",
-    conditions="all",
-    strains="all",
-    experimentincludes=False,
-    experimentexcludes=False,
-    conditionincludes=False,
-    conditionexcludes=False,
-    strainincludes=False,
-    strainexcludes=False,
-):
-    """
-    Display the current corrections to the data.
-
-    Parameters
-    ----------
-    experiments: string or list of strings
-        The experiments to include.
-    conditions: string or list of strings
-        The conditions to include.
-    strains: string or list of strings
-        The strains to include.
-    experimentincludes: string, optional
-        Selects only experiments that include the specified string in their
-        name.
-    experimentexcludes: string, optional
-        Ignores experiments that include the specified string in their
-        name.
-    conditionincludes: string, optional
-        Selects only conditions that include the specified string in their
-        name.
-    conditionexcludes: string, optional
-        Ignores conditions that include the specified string in their name.
-    strainincludes: string, optional
-        Selects only strains that include the specified string in their
-        name.
-    strainexcludes: string, optional
-        Ignores strains that include the specified string in their name.
-
-    Returns
-    -------
-    df: dataframe
-        Contains the status of the corrections for the specified strains,
-        conditions, and experiments.
-
-    Examples
-    --------
-    >>> p.corrections()
-    >>> p.corrections(strainincludes= 'GAL')
-    """
-    exps, cons, strs = sunder.getall(
-        self,
-        experiments,
-        experimentincludes,
-        experimentexcludes,
-        conditions,
-        conditionincludes,
-        conditionexcludes,
-        strains,
-        strainincludes,
-        strainexcludes,
-        nonull=True,
-    )
-    df = self.sc.query(
-        "experiment == @exps and condition == @cons and strain == @strs"
-    )
-    # only show corrections and not stats
-    df = df[
-        ["experiment", "strain", "condition"]
-        + [col for col in df.columns if "correct" in col]
-    ]
-    df = df.T
-    return df
-
-
-def read_dilution_data(fname):
-    d = import_files.read_text("omniplate", fname)
-    res = np.array(re.split(r"\n|\t", d)[:-1]).astype(float)
-    od, dilfac = res[::2], res[1::2]
-    if fname == "dilution_data_xiao.tsv":
-        # missing replicate - use mean of existing ones
-        dilfac = np.insert(dilfac, 0, dilfac[0])
-        od = np.insert(od, 0, np.mean(od[:2]))
-    else:
-        raise SystemExit("Dilution data unrecognised.")
-    return od, dilfac
-
-
-def arrange_into_replicates(od, dilfac):
-    """Rearrange so that data from each replicate is in a column."""
-    udilfac, indices, counts = np.unique(
-        dilfac, return_inverse=True, return_counts=True
-    )
-    ucounts = np.unique(counts)
-    if len(ucounts) == 1:
-        noreps = np.unique(counts)[0]
-        dilfac_reps = np.tile(np.atleast_2d(udilfac).T, noreps)
-        od_reps = np.array(
-            [od[indices == i] for i in range(udilfac.size)]
-        ).reshape((udilfac.size, noreps))
-        return od_reps, dilfac_reps
-    else:
-        raise Exception(
-            "There are inconsistent numbers of replicates"
-            " in the OD correction data."
-        )
-
-
-def findODcorrection(wdirpath, ODfname, figs, bd, gp_results, odmatch_min):
-    """
-    Determine a function to correct OD.
-
-    Use a Gaussian process to fit serial dilution data to correct for
-    non-linearities in the relationship between OD and cell density.
-
-    The data are either loaded from file ODfname or the default
-    data for haploid yeast growing in glucose are used.
-    """
-    print("Fitting dilution data for OD correction for non-linearities.")
-    if ODfname is not None:
-        try:
-            od_df = pd.read_csv(
-                str(wdirpath / ODfname), sep=None, engine="python", header=None
-            )
-            print(f"Using {ODfname}")
-            od_data = od_df.to_numpy()
-            od, dilfac = od_data[:, 0], od_data[:, 1]
-        except (FileNotFoundError, OSError):
-            raise errors.FileNotFound(str(wdirpath / ODfname))
-    else:
-        print("Using default data.")
-        fname = "dilution_data_xiao.tsv"
-        od, dilfac = read_dilution_data(fname)
-    od, dilfac = arrange_into_replicates(od, dilfac)
-    # run nunchaku
-    X = np.mean(dilfac, 1)
-    nc = Nunchaku(X, od.T, estimate_err=True, prior=[-5, 5])
-    num_regions, _ = nc.get_number(4)
-    bds, _ = nc.get_iboundaries(num_regions)
-    # find linear region, which starts from origin
-    odmatch_pts = np.mean(od, 1)[bds]
-    # pick end point with OD at least equal to odmatch_min
-    ipick = np.where(odmatch_pts > odmatch_min)[0][0]
-    odmatch = odmatch_pts[ipick]
-    dilfacmatch = X[bds[ipick]]
-    # process data
-    dilfac = dilfac.flatten()[np.argsort(od.flatten())]
-    od = np.sort(od.flatten())
-    # rescale so that OD and dilfac match
-    y = dilfac / dilfacmatch * odmatch
-    # set up Gaussian process
-    bds = {0: (-4, 4), 1: (-4, 4), 2: (-3, -1)}
-    # find bounds
-    if bd is not None:
-        bds = gu.mergedicts(original=bds, update=bd)
-    gc = gp.maternGP(bds, od, y)
-    # run Gaussian process
-    gc.findhyperparameters(noruns=5, exitearly=True, quiet=True)
-    if gp_results:
-        gc.results()
-    gc.predict(od)
-    if figs:
-        plt.figure()
-        gc.sketch(".")
-        plt.plot(odmatch, odmatch, "bs")
-        plt.grid(True)
-        plt.xlabel("OD")
-        plt.ylabel("corrected OD (relative cell numbers)")
-        if ODfname:
-            plt.title("Fitting " + ODfname)
-        else:
-            plt.title("for haploid budding yeast in glucose")
-        plt.show(block=False)
-    return gc, odmatch
-
-
-def performmediacorrection(
-    r_df, dtype, exp, condition, figs, commonmedia, frac
-):
-    """
-    Correct data of type dtype for any signal from the media.
-
-    Use lowess to smooth over time the media data from the Null
-    wells and subtract the smoothed values from the data.
-    """
-    # find data for correction with condition equal to commonmedia
-    df = r_df.query(
-        "experiment == @exp and condition == @commonmedia"
-        " and strain == 'Null'"
-    )
-    if df.empty:
-        # no data
-        print(
-            f' No well annotated "Null" was found for {commonmedia} '
-            f"in experiment {exp}."
-        )
-        print(
-            f"-> Correcting for media for {dtype} in {commonmedia} abandoned!"
-        )
-        return False, None
-    else:
-        # there is data - change r dataframe
-        rtest = (r_df.experiment == exp) & (r_df.condition == condition)
-        t, data = df["time"].to_numpy(), df[dtype].to_numpy()
-        if ~np.any(data[~np.isnan(data)]):
-            # all data is NaN
-            return False, None
-        # find correction
-        res = lowess(data, t, frac=frac)
-        correctionfn = interp1d(
-            res[:, 0],
-            res[:, 1],
-            fill_value=(res[0, 1], res[-1, 1]),
-            bounds_error=False,
-        )
-        if figs:
-            plt.figure()
-            plt.plot(t, data, "ro", res[:, 0], res[:, 1], "b-")
-            plt.xlabel("time (hours)")
-            plt.title(
-                exp + ": media correction for " + dtype + " in " + condition
-            )
-            plt.show(block=False)
-        # perform correction
-        r_df.loc[rtest, dtype] = r_df[rtest][dtype] - correctionfn(
-            r_df[rtest]["time"]
-        )
-        # check for any negative values
-        negvalues = ""
-        for s in np.unique(r_df[rtest]["strain"][r_df[rtest][dtype] < 0]):
-            if s != "Null":
-                wstr = f"\t{dtype}: {s} in {condition} for wells "
-                for well in np.unique(
-                    r_df[rtest][r_df[rtest].strain == s]["well"][
-                        r_df[rtest][dtype] < 0
-                    ]
-                ):
-                    wstr += f"{well}, "
-                wstr = wstr[:-2] + "\n"
-                negvalues += wstr
-        return True, negvalues
-
-
 def correctauto1(
     self,
     f,
     refstrain,
     figs,
     useGPs,
     flcvfn,
     bd,
     nosamples,
+    max_data_pts,
     experiments,
     experimentincludes,
     experimentexcludes,
     conditions,
     conditionincludes,
     conditionexcludes,
     strains,
     strainincludes,
     strainexcludes,
-    **kwargs,
 ):
     """
     Correct autofluorescence for measurements with emissions at one wavelength.
 
     Corrects for autofluorescence for data with emissions measured at one
     wavelength using the fluorescence of the reference strain
     interpolated to the OD of the tagged strain.
@@ -819,54 +742,53 @@
                             f,
                             t,
                             fl,
                             od,
                             flcvfn,
                             bd,
                             nosamples,
+                            max_data_pts,
                             e,
                             c,
                             s,
                             figs,
-                            **kwargs,
                         )
                     else:
                         # use only the replicates
                         flperod = np.transpose(
                             [fl[:, i] / od[:, i] for i in range(od.shape[1])]
                         )
                         flperod[flperod < 0] = np.nan
                     # check number of NaN
                     nonans = np.count_nonzero(np.isnan(fl))
                     if np.any(nonans):
                         if nonans == fl.size:
                             print(
-                                f"\n-> Corrected fluorescence is all NaN for {e}: {s} in {c}.\n"
+                                "\n-> Corrected fluorescence is all NaN "
+                                f"for {e}: {s} in {c}.\n"
                             )
                         else:
                             print(
                                 f"Warning - {e}: {s} in {c}\n"
                                 f"{nonans} corrected data points are"
                                 " NaN because the corrected fluorescence"
                                 " was negative.",
                             )
                     # store results
-                    bname = "c" + f[0]
                     autofdict = {
                         "experiment": e,
                         "condition": c,
                         "strain": s,
                         "time": t,
-                        bname: np.nanmean(fl, 1),
-                        bname + "_err": nanstdzeros2nan(fl, 1),
-                        bname + "perOD": np.nanmean(flperod, 1),
-                        bname + "perOD_err": nanstdzeros2nan(flperod, 1),
+                        f"c{f[0]}": np.nanmean(fl, 1),
+                        f"c{f[0]}_err": nanstdzeros2nan(fl, 1),
+                        f"c{f[0]}perOD": np.nanmean(flperod, 1),
+                        f"c{f[0]}perOD_err": nanstdzeros2nan(flperod, 1),
                     }
-                    addtodataframes(self, autofdict, bname)
-                    addrecord(self, f[0], e, c, s)
+                    addtodataframes(self, autofdict, f"c{f[0]}")
 
 
 def processref1(self, f, refstrain, figs, experiment, condition):
     """
     Process reference strain for data with one fluorescence measurement.
 
     Use lowess to smooth the fluorescence of the reference
@@ -887,15 +809,15 @@
 
     Returns
     -------
     refstrfn: function
         The reference strain's fluorescence as a function of OD.
     """
     e, c = experiment, condition
-    print(f"\n{e}: Processing reference strain {refstrain} for {f[0]} in {c}.")
+    print(f"{e}: Processing reference strain {refstrain} for {f[0]} in {c}.")
     _, (od, fl) = sunder.extractwells(
         self.r, self.s, e, c, refstrain, ["OD", f[0]]
     )
     if od.size == 0 or fl.size == 0:
         raise errors.CorrectAuto(f"{e}: {refstrain} not found in {c}.")
     else:
         odf = od.flatten("F")
@@ -943,24 +865,26 @@
     f,
     refstrain,
     figs,
     useGPs,
     flcvfn,
     bd,
     nosamples,
+    max_data_pts,
+    frac,
+    commonmedia,
     experiments,
     experimentincludes,
     experimentexcludes,
     conditions,
     conditionincludes,
     conditionexcludes,
     strains,
     strainincludes,
     strainexcludes,
-    **kwargs,
 ):
     """
     Correct autofluorescence for measurements with two emission wavelengths.
 
     Corrects for autofluorescence using spectral unmixing for data with
     measured emissions at two wavelengths.
 
@@ -987,16 +911,26 @@
             conditions,
             conditionincludes,
             conditionexcludes,
             labeltype="condition",
             nonull=True,
             nomedia=True,
         ):
+            # local r data frame for media corrections
+            lrdf = self.r[
+                (self.r.experiment == e) & (self.r.condition == c)
+            ].copy()
+            # correct for background fluorescence using Null strain
+            print("Correcting for background fluorescence of media.")
+            if commonmedia is not None:
+                c = commonmedia
+            find_Null_and_correct(self, lrdf, f[0], e, c, figs, frac)
+            find_Null_and_correct(self, lrdf, f[1], e, c, figs, frac)
             # process reference strain
-            refqrfn = processref2(self, f, refstrain, figs, e, c)
+            refqrfn = processref2(self, lrdf, f, refstrain, figs, e, c)
             if refqrfn is None:
                 # too many NaNs in reference strain
                 continue
             # process other strains
             for s in sunder.getset(
                 self,
                 strains,
@@ -1006,81 +940,78 @@
                 nonull=True,
             ):
                 if (
                     s != refstrain
                     and f"{s} in {c}" in self.allstrainsconditions[e]
                 ):
                     t, (fl_0, fl_1, od) = sunder.extractwells(
-                        self.r, self.s, e, c, s, f.copy() + ["OD"]
+                        lrdf, self.s, e, c, s, f.copy() + ["OD"]
                     )
                     if fl_0.size == 0 or fl_1.size == 0:
-                        print(f"Warning: No data found for {e}: {s} in {c} !!")
+                        print(f"Warning: No data found for {e}: {s} in {c}.")
                         continue
-                    nodata, nr = fl_0.shape
                     # set negative values to NaNs
                     fl_0[fl_0 < 0] = np.nan
                     fl_1[fl_1 < 0] = np.nan
-                    # use mean OD for correction
+                    # use mean OD for predicting ra from refstrain
                     odmean = np.nanmean(od, axis=1)
                     # correct autofluorescence
                     ra = refqrfn(odmean)
                     fl = applyautoflcorrection(self, ra, fl_0, fl_1)
                     fl[fl < 0] = np.nan
-                    # store corrected fluorescence
-                    bname = "c" + f[0]
-                    autofdict = {
-                        "experiment": e,
-                        "condition": c,
-                        "strain": s,
-                        "time": t,
-                        bname: np.nanmean(fl, 1),
-                        bname + " err": nanstdzeros2nan(fl, 1),
-                    }
                     if useGPs:
+                        # sample to estimate errors
                         flperod = samplewithGPs(
                             self,
                             f[0],
                             t,
                             fl,
                             od,
                             flcvfn,
                             bd,
                             nosamples,
+                            max_data_pts,
                             e,
                             c,
                             s,
                             figs,
-                            **kwargs,
                         )
                     else:
-                        # use only the replicates
+                        # use the replicates
                         flperod = fl / od
                         flperod[flperod < 0] = np.nan
-                    # update dict
-                    autofdict[bname + "perOD_err"] = naniqrzeros2nan(
-                        flperod, 1
-                    )
-                    autofdict[bname + "perOD"] = np.nanmean(flperod, 1)
+                    # store results
+                    autofdict = {
+                        "experiment": e,
+                        "condition": c,
+                        "strain": s,
+                        "time": t,
+                        f"c{f[0]}": np.nanmean(fl, 1),
+                        f"c{f[0]}_err": naniqrzeros2nan(fl, 1),
+                        f"c{f[0]}perOD_err": naniqrzeros2nan(flperod, 1),
+                        f"c{f[0]}perOD": np.nanmean(flperod, 1),
+                    }
                     # add to data frames
-                    addtodataframes(self, autofdict, bname)
-                    addrecord(self, f[0], e, c, s)
+                    addtodataframes(self, autofdict, f"c{f[0]}")
 
 
-def processref2(self, f, refstrain, figs, experiment, condition):
+def processref2(self, lrdf, f, refstrain, figs, experiment, condition):
     """
     Process reference strain for spectral unmixing.
 
     Requires data with two fluorescence measurements.
 
     Use lowess to smooth the ratio of emitted fluorescence measurements
     so that the reference strain's data is corrected to zero as best
     as possible.
 
     Parameters
     ----------
+    lrdf: pd.DataFrame
+        A copy of the r data frame with fluorescence corrected for media.
     f: list of strings
         The fluorescence measurements. For example, ['GFP', 'AutoFL'].
     refstrain: string
         The reference strain. For example, 'WT'.
     figs: boolean
         If True, display fits of the fluorescence ratios.
     experiment: string
@@ -1091,18 +1022,18 @@
     Returns
     -------
     qrfn: function
         The ratio of the two fluorescence values for the reference strain
         as a function of OD.
     """
     e, c = experiment, condition
-    print(f"\n{e}: Processing reference strain {refstrain} for {f[0]} in {c}.")
+    print(f"{e}: Processing reference strain {refstrain} for {f[0]} in {c}.")
     # refstrain data
     t, (f0, f1, od) = sunder.extractwells(
-        self.r, self.s, e, c, refstrain, f + ["OD"]
+        lrdf, self.s, e, c, refstrain, f.copy() + ["OD"]
     )
     if f0.size == 0 or f1.size == 0 or od.size == 0:
         raise errors.CorrectAuto(f"{e}: {refstrain} not found in {c}.")
     else:
         f0[f0 < 0] = np.nan
         f1[f1 < 0] = np.nan
         odf = od.flatten("F")
@@ -1145,26 +1076,25 @@
         # check autofluorescence correction for reference strain
         flref = applyautoflcorrection(self, qrfn(odrefmean), f0, f1)
         flrefperod = flref / od
         # set negative values to NaNs
         flref[flref < 0] = np.nan
         flrefperod[flrefperod < 0] = np.nan
         # store results
-        bname = "c" + f[0]
         autofdict = {
             "experiment": e,
             "condition": c,
             "strain": refstrain,
             "time": t,
-            bname: np.nanmean(flref, 1),
-            bname + "perOD": np.nanmean(flrefperod, 1),
-            bname + "_err": nanstdzeros2nan(flref, 1),
-            bname + "perOD_err": nanstdzeros2nan(flrefperod, 1),
+            f"c{f[0]}": np.nanmean(flref, 1),
+            f"c{f[0]}perOD": np.nanmean(flrefperod, 1),
+            f"c{f[0]}_err": nanstdzeros2nan(flref, 1),
+            f"c{f[0]}perOD_err": nanstdzeros2nan(flrefperod, 1),
         }
-        addtodataframes(self, autofdict, bname)
+        addtodataframes(self, autofdict, f"c{f[0]}")
         return qrfn
 
 
 def applyautoflcorrection(self, ra, f0data, f1data):
     """Correct for autofluorescence returning an array of replicates."""
     nr = f0data.shape[1]
     raa = np.reshape(np.tile(ra, nr), (np.size(ra), nr), order="F")
@@ -1184,24 +1114,14 @@
         self.s = gu.absorbdf(
             self.s,
             autofdf,
             ["experiment", "condition", "strain", "time"],
         )
 
 
-def addrecord(self, fname, e, c, s):
-    """Record correction."""
-    self.sc.loc[
-        (self.sc.experiment == e)
-        & (self.sc.condition == c)
-        & (self.sc.strain == s),
-        fname + "_corrected_for_autofluorescence",
-    ] = True
-
-
 def nanstdzeros2nan(a, axis=None):
     """Like nanstd but setting zeros to nan."""
     err = np.nanstd(a, axis)
     err[err == 0] = np.nan
     return err
 
 
@@ -1216,19 +1136,19 @@
     """Find parameters for GP from sc data frame."""
     sdf = self.sc[
         (self.sc.experiment == exp)
         & (self.sc.condition == con)
         & (self.sc.strain == s)
     ]
     try:
-        cvfn = sdf["gp_for_gr"].values[0]
+        cvfn = sdf[f"gp_for_{dtype}"].values[0]
         hypers = [
             sdf[col].values[0]
             for col in sorted(sdf.columns)
-            if ("hyper" in col and "gr" in col)
+            if ("hyper" in col and dtype in col)
         ]
         if np.any(np.isnan(hypers)):
             return None, None
         else:
             return hypers, cvfn
     except KeyError:
         return None, None
@@ -1244,56 +1164,74 @@
     go = getattr(gp, cvfn + "GP")({0: (-5, 5), 1: (-4, 4), 2: (-5, 2)}, x1, y1)
     go.lth_opt = hypers
     # make predictions so that samples can be generated
     go.predict(x, derivs=2)
     return go
 
 
-def samplewithGPs(
-    self, flname, t, fl, od, flcvfn, bd, nosamples, e, c, s, figs, **kwargs
-):
-    """Generate extra samples of flperod using Gaussian processes."""
-    hypers, cvfn = gethypers(self, e, c, s)
+def sample_ODs_with_GP(self, e, c, s, t, od, nosamples):
+    """Instantiate Gaussian process for log OD and sample."""
+    hypers, cvfn = gethypers(self, e, c, s, dtype="gr")
     if hypers is None or cvfn is None:
         raise SystemExit(
-            f"\nYou first must run getstats for {s} in {c} for {e}."
+            f"\nYou first must run getstats for {s} in {c} for {e}"
+            " unless useGPs=False."
         )
-    fitvar = f"log_{flname}"
-    derivname = f"d/dt_{fitvar}"
     od[od < 0] = np.finfo(float).eps
     # OD replicates with no NaN
     od_reps = np.setdiff1d(
         np.arange(od.shape[1]), np.unique(np.argwhere(np.isnan(od))[:, 1])
     )
-    # run GP for log fluorescence; omfitderiv deals with NaNs
-    if np.any(fl[~np.isnan(fl)]) and np.any(od_reps):
+    # initialise GP for log ODs
+    go = instantiateGP(hypers, cvfn, t, np.log(od)[:, od_reps])
+    # sample
+    lod_samples = go.sample(nosamples)
+    return lod_samples
+
+
+def samplewithGPs(
+    self,
+    flname,
+    t,
+    fl,
+    od,
+    flcvfn,
+    bd,
+    nosamples,
+    max_data_pts,
+    e,
+    c,
+    s,
+    figs,
+):
+    """Generate extra samples of fluorescence using Gaussian processes."""
+    if np.any(fl[~np.isnan(fl)]):
+        # run GP for log fluorescence; omfitderiv deals with NaNs
+        fitvar = f"log_{flname}"
+        derivname = f"d/dt_{fitvar}"
         ff, _ = runfitderiv(
             self,
             t,
             fl,
             fitvar,
             derivname,
             e,
             c,
             s,
             bd=bd,
             cvfn=flcvfn,
             logs=True,
             figs=figs,
-            **kwargs,
+            max_data_pts=max_data_pts,
         )
         if not ff.success:
             print(f"\n-> Fitting fluorescence failed for {e}: {s} in {c}.\n")
             return np.nan * np.ones((t.size, nosamples))
-        # initialise GP for log ODs
-        go = instantiateGP(hypers, cvfn, t, np.log(od)[:, od_reps])
-        # sample
-        lod_samples = go.sample(nosamples)
+        # samples
+        lod_samples = sample_ODs_with_GP(self, e, c, s, t, od, nosamples)
         lfl_samples = ff.fitderivsample(nosamples)[0]
+        # flperod samples
         flperod_samples = np.exp(lfl_samples - lod_samples)
-        # insert into or replace matrix of NaNs
-        flperod = np.nan * np.ones((t.size, nosamples))
-        flperod = flperod_samples
     else:
         # all NaN
-        flperod = np.nan * np.ones((t.size, nosamples))
-    return flperod
+        flperod_samples = np.nan * np.ones((t.size, nosamples))
+    return flperod_samples
```

### Comparing `omniplate-1.0/omniplate/dilution_data_lucia.tsv` & `omniplate-1.0a0/omniplate/dilution_data_lucia.tsv`

 * *Files identical despite different names*

### Comparing `omniplate-1.0/omniplate/dilution_data_xiao.tsv` & `omniplate-1.0a0/omniplate/dilution_data_xiao.tsv`

 * *Files identical despite different names*

### Comparing `omniplate-1.0/omniplate/getstats.py` & `omniplate-1.0a0/omniplate/getstats.py`

 * *Files identical despite different names*

### Comparing `omniplate-1.0/omniplate/loaddata.py` & `omniplate-1.0a0/omniplate/loaddata.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,36 +109,26 @@
             strs.append(cs.split(" in ")[0])
             cons.append(cs.split(" in ")[1])
         corrdict = {
             "experiment": exp,
             "strain": strs,
             "condition": cons,
             "OD_corrected": False,
+            "OD_corrected_for_media": False,
         }
         corrdict.update(
             {dtype + "_measured": True for dtype in self.datatypes[exp]}
         )
-        corrdict.update(
-            {
-                dtype + "_corrected_for_media": False
-                for dtype in self.datatypes[exp]
-            }
-        )
-        corrdict.update(
-            {
-                dtype + "_corrected_for_autofluorescence": False
-                for dtype in self.datatypes[exp]
-                if dtype not in ["AutoFL", "OD"]
-            }
-        )
         alldfs.append(pd.DataFrame(corrdict))
     self.sc = pd.concat(alldfs)
     # replace NaN with False for datatypes_measured
     for column in self.sc.columns[self.sc.columns.str.contains("_measured")]:
-        self.sc[column] = self.sc[column].astype(bool).fillna(False)
+        self.sc[column] = (
+            self.sc[column].infer_objects(copy=False).fillna(False)
+        )
     # make backup dataframe of original data
     self.origr = self.r.copy()
     # make dataframe for well contents
     self.wellsdf = admin.makewellsdf(self.r)
     # make s dataframe for summary data
     self.s = admin.make_s(self)
     # display info on experiment, conditions and strains
```

### Comparing `omniplate-1.0/omniplate/manipulatedfs.py` & `omniplate-1.0a0/omniplate/manipulatedfs.py`

 * *Files identical despite different names*

### Comparing `omniplate-1.0/omniplate/midlog.py` & `omniplate-1.0a0/omniplate/midlog.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,15 +156,24 @@
                     # run nunchaku on log(OD)
                     if use_smoothed:
                         # use standard deviation from GP
                         err = sd
                     else:
                         # estimate standard deviation from replicates
                         err = None
-                    nc = Nunchaku(t, Y, err=err, prior=prior, **kwargs)
+                    # find time points with no NaN
+                    common_i = np.all(~np.isnan(Y), axis=0)
+                    # run nunchaku
+                    nc = Nunchaku(
+                        t[common_i],
+                        Y[:, common_i],
+                        err=err,
+                        prior=prior,
+                        **kwargs,
+                    )
                     num_segs, evidence = nc.get_number(num_range=max_num)
                     bds, bds_std = nc.get_iboundaries(num_segs)
                     res_df = nc.get_info(bds)
                     # pick midlog segment
                     t_st, t_en = pick_midlog(res_df, min_duration)
                     if np.isnan(t_st) or np.isnan(t_en):
                         print(
@@ -214,15 +223,15 @@
                                     "strain",
                                 ]
                                 else k
                             ): v
                             for k, v in res_dict.items()
                         }
                         # add to sc dataframe
-                        admin.add_to_sc(self, res_dict)
+                        admin.add_dict_to_sc(self, res_dict)
 
 
 def pick_midlog(res_df, min_duration):
     """Find midlog from nunchaku's results dataframe."""
     # midlog had a minimal duration and positive growth rate
     sdf = res_df[(res_df["delta x"] > min_duration) & (res_df.gradient > 0)]
     if sdf.empty:
```

### Comparing `omniplate-1.0/omniplate/misc.py` & `omniplate-1.0a0/omniplate/misc.py`

 * *Files identical despite different names*

### Comparing `omniplate-1.0/omniplate/old_analyseOldTecan.py` & `omniplate-1.0a0/omniplate/old_analyseOldTecan.py`

 * *Files identical despite different names*

### Comparing `omniplate-1.0/omniplate/old_analyseTecan.py` & `omniplate-1.0a0/omniplate/old_analyseTecan.py`

 * *Files identical despite different names*

### Comparing `omniplate-1.0/omniplate/omfitderiv.py` & `omniplate-1.0a0/omniplate/omfitderiv.py`

 * *Files identical despite different names*

### Comparing `omniplate-1.0/omniplate/omgenutils.py` & `omniplate-1.0a0/omniplate/omgenutils.py`

 * *Files identical despite different names*

### Comparing `omniplate-1.0/omniplate/ominfo.py` & `omniplate-1.0a0/omniplate/ominfo.py`

 * *Files identical despite different names*

### Comparing `omniplate-1.0/omniplate/omio.py` & `omniplate-1.0a0/omniplate/omio.py`

 * *Files 3% similar despite different names*

```diff
@@ -129,15 +129,21 @@
                         )
                         return
             # ensure all are imported as strings
             for var in ["experiment", "condition", "strain"]:
                 exec("impdf[var]= impdf[var].astype(str)")
             # merge dataframes
             if hasattr(self, df):
-                exec("self." + df + "= pd.merge(self." + df + ", impdf, how= 'outer')")
+                exec(
+                    "self."
+                    + df
+                    + "= pd.merge(self."
+                    + df
+                    + ", impdf, how= 'outer')"
+                )
             else:
                 exec("self." + df + "= impdf")
         print()
 
     # update attributes
     self.allexperiments = list(self.s.experiment.unique())
     self.allconditions.update(
@@ -177,7 +183,12 @@
 
     # display warning if duplicates created
     if len(self.allexperiments) != np.unique(self.allexperiments).size:
         print(
             "\nLikely ERROR: data with the same experiment, condition, "
             "strain, and time now appears twice!!"
         )
+
+
+def save(self, name):
+    """Remind user that save is undefined."""
+    print("You probably mean exportdf.")
```

### Comparing `omniplate-1.0/omniplate/omplot.py` & `omniplate-1.0a0/omniplate/omplot.py`

 * *Files identical despite different names*

### Comparing `omniplate-1.0/omniplate/omstats.py` & `omniplate-1.0a0/omniplate/omstats.py`

 * *Files identical despite different names*

### Comparing `omniplate-1.0/omniplate/omwells.py` & `omniplate-1.0a0/omniplate/omwells.py`

 * *Files identical despite different names*

### Comparing `omniplate-1.0/omniplate/parseSunrise.py` & `omniplate-1.0a0/omniplate/parseSunrise.py`

 * *Files identical despite different names*

### Comparing `omniplate-1.0/omniplate/parseTecan.py` & `omniplate-1.0a0/omniplate/parseTecan.py`

 * *Files identical despite different names*

### Comparing `omniplate-1.0/omniplate/parseplate.py` & `omniplate-1.0a0/omniplate/parseplate.py`

 * *Files identical despite different names*

### Comparing `omniplate-1.0/omniplate/platereader.py` & `omniplate-1.0a0/omniplate/platereader.py`

 * *Files 3% similar despite different names*

```diff
@@ -156,16 +156,15 @@
 
     ###
     # import methods
     ###
     from .admin import cols_to_underscore
     from .corrections import (
         correctauto,
-        corrections,
-        correctmedia,
+        correctODformedia,
         correctOD,
     )
     from .getstats import getstats
     from .loaddata import combine_experiments, load
     from .manipulatedfs import (
         add_to_sc,
         addcolumn,
@@ -184,14 +183,15 @@
         log,
         ls,
         webhelp,
     )
     from .omio import exportdf, importdf, savelog
     from .omplot import close, plot, savefigs
     from .omwells import contentsofwells, ignorewells, showwells
+    from .promoteractivity import getpromoteractivity
 
     def __repr__(self):
         """Give standard representation."""
         repstr = f"omniplate.{self.__class__.__name__}: "
         if self.allexperiments:
             for e in self.allexperiments:
                 repstr += e + " ; "
```

### Comparing `omniplate-1.0/omniplate/runfitderiv.py` & `omniplate-1.0a0/omniplate/runfitderiv.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import matplotlib.pyplot as plt
-import pandas as pd
 
 import omniplate.admin as admin
 import omniplate.omstats as omstats
 from omniplate.omfitderiv import fitderiv
 
 
 def runfitderiv(
@@ -178,14 +177,13 @@
         dict_for_sc[f"logmaxlikehood_for_{derivname}"] = f.logmaxlike
         dict_for_sc["gp_for_" + derivname] = cvfn
         for j, val in enumerate(f.lth):
             dict_for_sc[f"log_hyperparameter_{j}_for_{derivname}"] = val
         # add time series to s dataframe
         admin.add_to_s(self, derivname, df_for_s)
         # create or add summary stats to sc dataframe
-        df_for_sc = pd.DataFrame(dict_for_sc, index=pd.RangeIndex(0, 1, 1))
-        admin.add_to_sc(self, df_for_sc)
+        admin.add_dict_to_sc(self, dict_for_sc)
         if figs:
             plt.show(block=False)
         return f, warning
     else:
         return f, None
```

### Comparing `omniplate-1.0/omniplate/sunder.py` & `omniplate-1.0a0/omniplate/sunder.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,35 +148,38 @@
     lrdf = r_df[
         (r_df.time >= s_df.time.min()) & (r_df.time <= s_df.time.max())
     ]
     df = lrdf.query(
         "experiment == @experiment and condition == @condition "
         "and strain == @strain"
     )
-    # extract time
-    dfw_time = (
-        df[["time", "well"]]
-        .groupby("well", group_keys=True)["time"]
-        .apply(list)
-    )
-    well_times = [dfw_time[well] for well in dfw_time.index]
-    # data may have different durations
-    longest_i = np.argmax([len(dfw_time[well]) for well in dfw_time.index])
-    t = np.array(well_times[longest_i])
-    # extract data
-    matrices = []
-    for dtype in datatypes:
-        dfw_dtype = (
-            df[[dtype, "well"]]
-            .groupby("well", group_keys=True)[dtype]
+    if df.empty:
+        return None, None
+    else:
+        # extract time
+        dfw_time = (
+            df[["time", "well"]]
+            .groupby("well", group_keys=True)["time"]
             .apply(list)
         )
-        data = np.nan * np.ones((len(t), dfw_dtype.shape[0]))
-        for i, well in enumerate(dfw_dtype.index):
-            data[: len(dfw_dtype[well]), i] = np.array(dfw_dtype[well])
-        matrices.append(data)
-    if len(datatypes) == 1:
-        # return array
-        return t, matrices[0]
-    else:
-        # return list of arrays
-        return t, matrices
+        well_times = [dfw_time[well] for well in dfw_time.index]
+        # data may have different durations
+        longest_i = np.argmax([len(dfw_time[well]) for well in dfw_time.index])
+        t = np.array(well_times[longest_i])
+        # extract data
+        matrices = []
+        for dtype in datatypes:
+            dfw_dtype = (
+                df[[dtype, "well"]]
+                .groupby("well", group_keys=True)[dtype]
+                .apply(list)
+            )
+            data = np.nan * np.ones((len(t), dfw_dtype.shape[0]))
+            for i, well in enumerate(dfw_dtype.index):
+                data[: len(dfw_dtype[well]), i] = np.array(dfw_dtype[well])
+            matrices.append(data)
+        if len(datatypes) == 1:
+            # return array
+            return t, matrices[0]
+        else:
+            # return list of arrays
+            return t, matrices
```

### Comparing `omniplate-1.0/pyproject.toml` & `omniplate-1.0a0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "omniplate"
-version = "1.0"
+version = "1.0a"
 description = "For analysing and meta-analysing plate-reader data"
 authors = ["Peter Swain <peter.swain@ed.ac.uk>"]
 
 license = "MIT"
 readme = "README.md"
 homepage = "https://swainlab.bio.ed.ac.uk/software/omniplate"
 repository = "https://git.ecdf.ed.ac.uk/pswain/omniplate"
```

### Comparing `omniplate-1.0/PKG-INFO` & `omniplate-1.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniplate
-Version: 1.0
+Version: 1.0a0
 Summary: For analysing and meta-analysing plate-reader data
 Home-page: https://swainlab.bio.ed.ac.uk/software/omniplate
 License: MIT
 Keywords: omniplate,systems biology,bioinformatics,plate readers
 Author: Peter Swain
 Author-email: peter.swain@ed.ac.uk
 Requires-Python: >=3.8,<3.11
```

