# Comparing `tmp/tglc-0.6.1.tar.gz` & `tmp/tglc-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tglc-0.6.1.tar", last modified: Tue Jan  9 06:59:11 2024, max compression
+gzip compressed data, was "tglc-0.6.2.tar", last modified: Thu Apr 25 00:48:10 2024, max compression
```

## Comparing `tglc-0.6.1.tar` & `tglc-0.6.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 tehan     (1000) tehan     (1000)        0 2024-01-09 06:59:11.121937 tglc-0.6.1/
--rw-rw-r--   0 tehan     (1000) tehan     (1000)     1063 2022-09-16 07:04:15.000000 tglc-0.6.1/LICENSE
--rw-rw-r--   0 tehan     (1000) tehan     (1000)       35 2022-09-16 07:04:15.000000 tglc-0.6.1/MANIFEST.in
--rw-rw-r--   0 tehan     (1000) tehan     (1000)     5313 2024-01-09 06:59:11.121937 tglc-0.6.1/PKG-INFO
--rw-rw-r--   0 tehan     (1000) tehan     (1000)     4890 2024-01-09 06:58:40.000000 tglc-0.6.1/README.rst
--rw-rw-r--   0 tehan     (1000) tehan     (1000)       38 2024-01-09 06:59:11.121937 tglc-0.6.1/setup.cfg
--rw-rw-r--   0 tehan     (1000) tehan     (1000)      925 2024-01-09 06:42:46.000000 tglc-0.6.1/setup.py
-drwxrwxr-x   0 tehan     (1000) tehan     (1000)        0 2024-01-09 06:59:11.121937 tglc-0.6.1/tglc/
--rw-rw-r--   0 tehan     (1000) tehan     (1000)      115 2024-01-09 06:42:46.000000 tglc-0.6.1/tglc/__init__.py
-drwxrwxr-x   0 tehan     (1000) tehan     (1000)        0 2024-01-09 06:59:11.121937 tglc-0.6.1/tglc/background_mask/
--rw-rw-r--   0 tehan     (1000) tehan     (1000)        0 2022-09-16 07:04:15.000000 tglc-0.6.1/tglc/background_mask/__init__.py
--rw-rw-r--   0 tehan     (1000) tehan     (1000)   267840 2022-09-16 07:04:15.000000 tglc-0.6.1/tglc/background_mask/median_mask.fits
--rw-rw-r--   0 tehan     (1000) tehan     (1000)    22712 2024-01-05 06:26:06.000000 tglc-0.6.1/tglc/effective_psf.py
--rw-rw-r--   0 tehan     (1000) tehan     (1000)    15527 2023-12-13 22:06:55.000000 tglc-0.6.1/tglc/ffi.py
--rw-rw-r--   0 tehan     (1000) tehan     (1000)    11963 2024-01-09 06:42:46.000000 tglc-0.6.1/tglc/ffi_cut.py
--rw-rw-r--   0 tehan     (1000) tehan     (1000)   136246 2023-02-12 08:25:40.000000 tglc-0.6.1/tglc/lc_plot.py
--rw-rw-r--   0 tehan     (1000) tehan     (1000)     4331 2023-03-18 21:06:07.000000 tglc-0.6.1/tglc/mast.py
--rw-rw-r--   0 tehan     (1000) tehan     (1000)    25909 2024-01-09 06:44:32.000000 tglc-0.6.1/tglc/quick_lc.py
--rw-rw-r--   0 tehan     (1000) tehan     (1000)     4123 2024-01-09 06:41:17.000000 tglc-0.6.1/tglc/run.py
--rw-rw-r--   0 tehan     (1000) tehan     (1000)     3171 2023-12-13 21:36:00.000000 tglc-0.6.1/tglc/source_output.py
--rw-rw-r--   0 tehan     (1000) tehan     (1000)    20692 2024-01-09 06:41:17.000000 tglc-0.6.1/tglc/target_lightcurve.py
-drwxrwxr-x   0 tehan     (1000) tehan     (1000)        0 2024-01-09 06:59:11.121937 tglc-0.6.1/tglc.egg-info/
--rw-rw-r--   0 tehan     (1000) tehan     (1000)     5313 2024-01-09 06:59:11.000000 tglc-0.6.1/tglc.egg-info/PKG-INFO
--rw-rw-r--   0 tehan     (1000) tehan     (1000)      422 2024-01-09 06:59:11.000000 tglc-0.6.1/tglc.egg-info/SOURCES.txt
--rw-rw-r--   0 tehan     (1000) tehan     (1000)        1 2024-01-09 06:59:11.000000 tglc-0.6.1/tglc.egg-info/dependency_links.txt
--rw-rw-r--   0 tehan     (1000) tehan     (1000)       96 2024-01-09 06:59:11.000000 tglc-0.6.1/tglc.egg-info/requires.txt
--rw-rw-r--   0 tehan     (1000) tehan     (1000)        5 2024-01-09 06:59:11.000000 tglc-0.6.1/tglc.egg-info/top_level.txt
+drwxrwxr-x   0 tehan     (1000) tehan     (1000)        0 2024-04-25 00:48:10.943531 tglc-0.6.2/
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)     1063 2022-09-16 07:04:15.000000 tglc-0.6.2/LICENSE
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)       35 2022-09-16 07:04:15.000000 tglc-0.6.2/MANIFEST.in
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)     5788 2024-04-25 00:48:10.943531 tglc-0.6.2/PKG-INFO
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)     4891 2024-04-25 00:48:05.000000 tglc-0.6.2/README.rst
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)       38 2024-04-25 00:48:10.943531 tglc-0.6.2/setup.cfg
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)      925 2024-04-25 00:30:27.000000 tglc-0.6.2/setup.py
+drwxrwxr-x   0 tehan     (1000) tehan     (1000)        0 2024-04-25 00:48:10.943531 tglc-0.6.2/tglc/
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)      115 2024-04-25 00:30:27.000000 tglc-0.6.2/tglc/__init__.py
+drwxrwxr-x   0 tehan     (1000) tehan     (1000)        0 2024-04-25 00:48:10.943531 tglc-0.6.2/tglc/background_mask/
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)        0 2022-09-16 07:04:15.000000 tglc-0.6.2/tglc/background_mask/__init__.py
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)   267840 2022-09-16 07:04:15.000000 tglc-0.6.2/tglc/background_mask/median_mask.fits
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)    22712 2024-02-26 08:55:20.000000 tglc-0.6.2/tglc/effective_psf.py
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)    15649 2024-04-25 00:29:36.000000 tglc-0.6.2/tglc/ffi.py
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)    11963 2024-04-25 00:30:27.000000 tglc-0.6.2/tglc/ffi_cut.py
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)   136246 2024-04-25 00:29:36.000000 tglc-0.6.2/tglc/lc_plot.py
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)     4331 2023-03-18 21:06:07.000000 tglc-0.6.2/tglc/mast.py
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)    27815 2024-04-25 00:44:55.000000 tglc-0.6.2/tglc/quick_lc.py
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)     4123 2024-04-25 00:29:12.000000 tglc-0.6.2/tglc/run.py
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)     3171 2024-04-25 00:29:12.000000 tglc-0.6.2/tglc/source_output.py
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)    20692 2024-04-25 00:29:12.000000 tglc-0.6.2/tglc/target_lightcurve.py
+drwxrwxr-x   0 tehan     (1000) tehan     (1000)        0 2024-04-25 00:48:10.943531 tglc-0.6.2/tglc.egg-info/
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)     5788 2024-04-25 00:48:10.000000 tglc-0.6.2/tglc.egg-info/PKG-INFO
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)      422 2024-04-25 00:48:10.000000 tglc-0.6.2/tglc.egg-info/SOURCES.txt
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)        1 2024-04-25 00:48:10.000000 tglc-0.6.2/tglc.egg-info/dependency_links.txt
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)       96 2024-04-25 00:48:10.000000 tglc-0.6.2/tglc.egg-info/requires.txt
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)        5 2024-04-25 00:48:10.000000 tglc-0.6.2/tglc.egg-info/top_level.txt
```

### Comparing `tglc-0.6.1/LICENSE` & `tglc-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tglc-0.6.1/PKG-INFO` & `tglc-0.6.2/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,14 @@
-Metadata-Version: 2.1
-Name: tglc
-Version: 0.6.1
-Summary: TESS-Gaia Light Curve
-Home-page: https://github.com/TeHanHunter/TESS_Gaia_Light_Curve
-Author: Te Han
-Author-email: tehanhunter@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 ==================================
 Introduction
 ==================================
 
 TESS-Gaia Light Curve (`TGLC <https://archive.stsci.edu/hlsp/tglc>`_) is a dataset of TESS full-frame image light curves publicly available via the MAST portal. It is fitted with effective PSF and decontaminated with Gaia DR3 and achieved percent-level photometric precision down to 16th TESS magnitude! It unlocks astrophysics to a vast number of dim stars below 12th TESS magnitude. A package called tglc is pip-installable for customized light curve fits.
 
+
 ==================================
 Usage
 ==================================
 There are four fluxes in each FITS file: aperture flux, PSF flux, calibrated aperture flux, and calibrated PSF flux.
 If you are uncertain which to use:
 
 * Calibrated psf flux is better in **deblending** targets. Use this if you need to deblend a target near a variable source. The best deblending can be achieved with tglc package by setting a non-zero prior. It also gives the more accurate **transit depth** in most cases, especially when fitting with an optimized prior.
```

### Comparing `tglc-0.6.1/README.rst` & `tglc-0.6.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,71 @@
-==================================
-Introduction
-==================================
-
-TESS-Gaia Light Curve (`TGLC <https://archive.stsci.edu/hlsp/tglc>`_) is a dataset of TESS full-frame image light curves publicly available via the MAST portal. It is fitted with effective PSF and decontaminated with Gaia DR3 and achieved percent-level photometric precision down to 16th TESS magnitude! It unlocks astrophysics to a vast number of dim stars below 12th TESS magnitude. A package called tglc is pip-installable for customized light curve fits.
-
-==================================
-Usage
-==================================
-There are four fluxes in each FITS file: aperture flux, PSF flux, calibrated aperture flux, and calibrated PSF flux.
-If you are uncertain which to use:
-
-* Calibrated psf flux is better in **deblending** targets. Use this if you need to deblend a target near a variable source. The best deblending can be achieved with tglc package by setting a non-zero prior. It also gives the more accurate **transit depth** in most cases, especially when fitting with an optimized prior.
-* Calibrated aperture flux usually has slightly **higher SNR**. The transit depth (or variation amplitude), however, can be imperfect since the normalization depends on the PSF fitting which is imperfect. This imperfection can be minimized by using a bigger aperture than the default aperture (3*3). One need to use the tglc package and set tglc_lc(save_aper=True) to access the 5*5 aperture. In the presence of a bright but "constant" contamination (several magnitudes brighter), the calibrated aperture flux is better in removing the constant contamination. 
-* The aperture flux and PSF flux are not detrended or normalized. Use this if you are doing stellar variability science with long baseline. Or, if the detrending is not optimal (default detrending has a window length of 1 day; see Known Problems below), start with the aperture flux or PSF flux and detrend carefully!
-* **If you are uncertain, start with calibrated aperture flux!**
-
-The `tutorial <tutorial/TGLC_tutorial.ipynb>`_ shows the syntaxes and differences among these light curves in several examples.
-
-==================================
-Data Access
-==================================
-There are three data access methods:
-
-* MAST Portal: Easiest for acquiring light curves for a few stars. However, new sectors are updated relatively slowly. 
-* MAST bulk download: Best for downloading light curves for all stars (<16 TESS magnitude) in a sectors. 
-* tglc package: Capable of producing similar quality light curves for any sector and any star with custom options. 
-
-MAST Portal/bulk download
-----------------------------
-The easiest usage requires no package installation. Simply follow the `TGLC HLSP page <https://archive.stsci.edu/hlsp/tglc>`_ to download light curves from MAST or use `MAST Portal <https://mast.stsci.edu/portal/Mashup/Clients/Mast/Portal.html>`_. Light curves are being fitted sector by sector and will be available on MAST gradually. MAST hosts all Gaia DR3 stars down to 16th magnitude. Each .fits file includes PSF and aperture light curves and their calibrated versions.
-
-MAST available sectors: `sector worklist <https://docs.google.com/spreadsheets/d/1FhHElWb1wmx9asWiZecAJ2umN0-P_aXn55OBVB34_rg/edit?usp=sharing>`_
-
-
-tglc package
-----------------------------
-Users can also fit light curves using the package tglc. Using tglc, one can specify a region, sector(s), and customized aperture shape if needed. It can also allow all field stars to float by assigning Gaussian priors, which can help decontaminate variable field stars. tglc is currently only available for linux. Run::
-
-  pip install tglc
-  
-for the latest tglc release. After installation, follow the `tutorial <tutorial/TGLC_tutorial.ipynb>`_ to fit light curves. If there is a problem, please leave a comment in the Issues section to help us improve. Thank you!
-
-
-==================================
-Known Problems
-==================================
-There are several imperfections we noticed in the MAST TGLC light curves and tglc package:
-
-* If the star is very dim (~< 15 Tmag) near a variable source, it can make the aperture and/or PSF light curve negative for some cadences. The detrending algorithm could malfunction and result in bad cal_aper_flux and/or cal_psf_flux. This is now fixed for tglc package, but this problem remains for the primary mission light curves published on MAST. Please detrend again if necessary. The extended mission light curves on MAST will not be affected. This is a very rare scenario, but could be important.
-
-==================================
-Reference
-==================================
-If you find the TGLC light curves or the tglc package useful in your research, please cite `our paper <https://iopscience.iop.org/article/10.3847/1538-3881/acaaa7>`_ published on the Astronomical Journal. 
+Metadata-Version: 2.1
+Name: tglc
+Version: 0.6.2
+Summary: TESS-Gaia Light Curve
+Home-page: https://github.com/TeHanHunter/TESS_Gaia_Light_Curve
+Author: Te Han
+Author-email: tehanhunter@gmail.com
+License: UNKNOWN
+Description: ==================================
+        Introduction
+        ==================================
+        
+        TESS-Gaia Light Curve (`TGLC <https://archive.stsci.edu/hlsp/tglc>`_) is a dataset of TESS full-frame image light curves publicly available via the MAST portal. It is fitted with effective PSF and decontaminated with Gaia DR3 and achieved percent-level photometric precision down to 16th TESS magnitude! It unlocks astrophysics to a vast number of dim stars below 12th TESS magnitude. A package called tglc is pip-installable for customized light curve fits.
+        
+        
+        ==================================
+        Usage
+        ==================================
+        There are four fluxes in each FITS file: aperture flux, PSF flux, calibrated aperture flux, and calibrated PSF flux.
+        If you are uncertain which to use:
+        
+        * Calibrated psf flux is better in **deblending** targets. Use this if you need to deblend a target near a variable source. The best deblending can be achieved with tglc package by setting a non-zero prior. It also gives the more accurate **transit depth** in most cases, especially when fitting with an optimized prior.
+        * Calibrated aperture flux usually has slightly **higher SNR**. The transit depth (or variation amplitude), however, can be imperfect since the normalization depends on the PSF fitting which is imperfect. This imperfection can be minimized by using a bigger aperture than the default aperture (3*3). One need to use the tglc package and set tglc_lc(save_aper=True) to access the 5*5 aperture. In the presence of a bright but "constant" contamination (several magnitudes brighter), the calibrated aperture flux is better in removing the constant contamination. 
+        * The aperture flux and PSF flux are not detrended or normalized. Use this if you are doing stellar variability science with long baseline. Or, if the detrending is not optimal (default detrending has a window length of 1 day; see Known Problems below), start with the aperture flux or PSF flux and detrend carefully!
+        * **If you are uncertain, start with calibrated aperture flux!**
+        
+        The `tutorial <tutorial/TGLC_tutorial.ipynb>`_ shows the syntaxes and differences among these light curves in several examples.
+        
+        ==================================
+        Data Access
+        ==================================
+        There are three data access methods:
+        
+        * MAST Portal: Easiest for acquiring light curves for a few stars. However, new sectors are updated relatively slowly. 
+        * MAST bulk download: Best for downloading light curves for all stars (<16 TESS magnitude) in a sectors. 
+        * tglc package: Capable of producing similar quality light curves for any sector and any star with custom options. 
+        
+        MAST Portal/bulk download
+        ----------------------------
+        The easiest usage requires no package installation. Simply follow the `TGLC HLSP page <https://archive.stsci.edu/hlsp/tglc>`_ to download light curves from MAST or use `MAST Portal <https://mast.stsci.edu/portal/Mashup/Clients/Mast/Portal.html>`_. Light curves are being fitted sector by sector and will be available on MAST gradually. MAST hosts all Gaia DR3 stars down to 16th magnitude. Each .fits file includes PSF and aperture light curves and their calibrated versions.
+        
+        MAST available sectors: `sector worklist <https://docs.google.com/spreadsheets/d/1FhHElWb1wmx9asWiZecAJ2umN0-P_aXn55OBVB34_rg/edit?usp=sharing>`_
+        
+        
+        tglc package
+        ----------------------------
+        Users can also fit light curves using the package tglc. Using tglc, one can specify a region, sector(s), and customized aperture shape if needed. It can also allow all field stars to float by assigning Gaussian priors, which can help decontaminate variable field stars. tglc is currently only available for linux. Run::
+        
+          pip install tglc
+          
+        for the latest tglc release. After installation, follow the `tutorial <tutorial/TGLC_tutorial.ipynb>`_ to fit light curves. If there is a problem, please leave a comment in the Issues section to help us improve. Thank you!
+        
+        
+        ==================================
+        Known Problems
+        ==================================
+        There are several imperfections we noticed in the MAST TGLC light curves and tglc package:
+        
+        * If the star is very dim (~< 15 Tmag) near a variable source, it can make the aperture and/or PSF light curve negative for some cadences. The detrending algorithm could malfunction and result in bad cal_aper_flux and/or cal_psf_flux. This is now fixed for tglc package, but this problem remains for the primary mission light curves published on MAST. Please detrend again if necessary. The extended mission light curves on MAST will not be affected. This is a very rare scenario, but could be important.
+        
+        ==================================
+        Reference
+        ==================================
+        If you find the TGLC light curves or the tglc package useful in your research, please cite `our paper <https://iopscience.iop.org/article/10.3847/1538-3881/acaaa7>`_ published on the Astronomical Journal. 
+        
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
```

### Comparing `tglc-0.6.1/setup.py` & `tglc-0.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 sys.path.insert(0, "tglc")
 with open("README.rst", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="tglc",
-    version='0.6.1',
+    version='0.6.2',
     author="Te Han",
     author_email="tehanhunter@gmail.com",
     description="TESS-Gaia Light Curve",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/TeHanHunter/TESS_Gaia_Light_Curve",
     classifiers=[
```

### Comparing `tglc-0.6.1/tglc/background_mask/median_mask.fits` & `tglc-0.6.2/tglc/background_mask/median_mask.fits`

 * *Files identical despite different names*

### Comparing `tglc-0.6.1/tglc/effective_psf.py` & `tglc-0.6.2/tglc/effective_psf.py`

 * *Files identical despite different names*

### Comparing `tglc-0.6.1/tglc/ffi.py` & `tglc-0.6.2/tglc/ffi.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,17 @@
         catalogdata_tic = tic_advanced_search_position_rows(ra=ra, dec=dec, radius=(self.size + 2) * 21 * 0.707 / 3600)
         # print(f'no_of_stars={len(catalogdata_tic)}, camera={camera}, ccd={ccd}: ra={ra}, dec={dec}, radius={(self.size + 2) * 21 * 0.707 / 3600}')
         self.tic = convert_gaia_id(catalogdata_tic)
         self.flux = flux[:, y:y + size, x:x + size]
         self.mask = mask[y:y + size, x:x + size]
         self.time = np.array(time)
         median_time = np.median(self.time)
-        interval = (median_time - 388.5) / 365.25
+        interval = (median_time + 388.5) / 365.25
+        # Julian Day Number:	2457000.0 (TBJD=0)
+        # Calendar Date/Time:	2014-12-08 12:00:00 388.5 days before J2016
 
         num_gaia = len(catalogdata)
         tic_id = np.zeros(num_gaia)
         x_gaia = np.zeros(num_gaia)
         y_gaia = np.zeros(num_gaia)
         tess_mag = np.zeros(num_gaia)
         in_frame = [True] * num_gaia
```

### Comparing `tglc-0.6.1/tglc/ffi_cut.py` & `tglc-0.6.2/tglc/ffi_cut.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,15 @@
         # data_flux_err = data_flux_err[np.where(data_quality == 0), :, :][0]
         self.wcs = wcs
         self.time = data_time
         self.flux = data_flux
         self.flux_err = data_flux_err
         self.quality = data_quality
         median_time = np.median(data_time)
-        interval = (median_time - 388.5) / 365.25
+        interval = (median_time + 388.5) / 365.25
 
         mask = np.ones(np.shape(data_flux[0]))
         bad_pixels = np.zeros(np.shape(data_flux[0]))
         med_flux = np.median(data_flux, axis=0)
         bad_pixels[med_flux > 0.8 * np.nanmax(med_flux)] = 1
         bad_pixels[med_flux < 0.2 * np.nanmedian(med_flux)] = 1
         bad_pixels[np.isnan(med_flux)] = 1
```

### Comparing `tglc-0.6.1/tglc/lc_plot.py` & `tglc-0.6.2/tglc/lc_plot.py`

 * *Files identical despite different names*

### Comparing `tglc-0.6.1/tglc/mast.py` & `tglc-0.6.2/tglc/mast.py`

 * *Files identical despite different names*

### Comparing `tglc-0.6.1/tglc/quick_lc.py` & `tglc-0.6.2/tglc/quick_lc.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from functools import partial
 from tglc.target_lightcurve import epsf
 from tglc.ffi_cut import ffi_cut
 from astroquery.mast import Catalogs
 import astropy.units as u
 from astropy.coordinates import SkyCoord
 from astroquery.mast import Tesscut
+# Tesscut._service_api_connection.TIMEOUT = 6000
 
 # warnings.simplefilter('ignore', UserWarning)
 from threadpoolctl import ThreadpoolController, threadpool_limits
 import numpy as np
 
 controller = ThreadpoolController()
 
@@ -40,15 +41,15 @@
     os.makedirs(local_directory + f'epsf/', exist_ok=True)
     os.makedirs(local_directory + f'source/', exist_ok=True)
     if first_sector_only:
         sector = 'first'
     elif last_sector_only:
         sector = 'last'
     print(f'Target: {target}')
-    target_ = Catalogs.query_object(target, radius=21 * 0.707 / 3600, catalog="Gaia", version=2)
+    target_ = Catalogs.query_object(target, radius=42 * 0.707 / 3600, catalog="Gaia", version=2)
     if len(target_) == 0:
         target_ = Catalogs.query_object(target.name, radius=5 * 21 * 0.707 / 3600, catalog="Gaia", version=2)
     ra = target_[0]['ra']
     dec = target_[0]['dec']
     coord = SkyCoord(ra=ra, dec=dec, unit=(u.degree, u.degree), frame='icrs')
     sector_table = Tesscut.get_sectors(coordinates=coord)
     print(sector_table)
@@ -156,25 +157,25 @@
                  tics=None, local_directory=None):
     for i in range(server, 27, 2):
         with Pool(16) as p:
             p.map(partial(search_stars, sector=i, tics=tics, local_directory=local_directory), range(16))
     return
 
 
-def plot_lc(local_directory=None, type='cal_aper_flux'):
-    files = glob(f'{local_directory}*.fits')
+def plot_lc(local_directory=None, type='cal_aper_flux', xlow=None, xhigh=None, ylow=None, yhigh=None):
+    files = glob(f'{local_directory}lc/*.fits')
     os.makedirs(f'{local_directory}plots/', exist_ok=True)
     for i in range(len(files)):
         with fits.open(files[i], mode='denywrite') as hdul:
             q = [a and b for a, b in zip(list(hdul[1].data['TESS_flags'] == 0), list(hdul[1].data['TGLC_flags'] == 0))]
             plt.figure(constrained_layout=False, figsize=(8, 4))
             plt.plot(hdul[1].data['time'], hdul[1].data[type], '.', c='silver', label=type)
             plt.plot(hdul[1].data['time'][q], hdul[1].data[type][q], '.k', label=f'{type}_flagged')
-            # plt.xlim(2753, 2755)
-            # plt.ylim(0.7, 1.1)
+            plt.xlim(xlow, xhigh)
+            plt.ylim(ylow, yhigh)
             plt.title(f'TIC_{hdul[0].header["TICID"]}_sector_{hdul[0].header["SECTOR"]:04d}_{type}')
             plt.legend()
             # plt.show()
             plt.savefig(
                 f'{local_directory}plots/TIC_{hdul[0].header["TICID"]}_sector_{hdul[0].header["SECTOR"]:04d}_{type}.png',
                 dpi=300)
             plt.close()
@@ -293,38 +294,41 @@
     plt.ylabel('Normalized flux')
     plt.savefig(f'{local_directory}/plots/{title}.png', dpi=300)
     plt.close(fig)
 
 
 def plot_contamination(local_directory=None, gaia_dr3=None):
     files = glob(f'{local_directory}lc/*.fits')
-    os.makedirs(f'{local_directory}lc/plots/', exist_ok=True)
+    os.makedirs(f'{local_directory}plots/', exist_ok=True)
     for i in range(len(files)):
-        with open(glob(f'{local_directory}source/*.pkl')[0], 'rb') as input_:
-            with fits.open(files[i], mode='denywrite') as hdul:
-                sector = hdul[0].header['SECTOR']
+        with fits.open(files[i], mode='denywrite') as hdul:
+            sector = hdul[0].header['SECTOR']
+            with open(glob(f'{local_directory}source/*_{sector}.pkl')[0], 'rb') as input_:
                 source = pickle.load(input_)
                 source.select_sector(sector=sector)
                 star_num = np.where(source.gaia['DESIGNATION'] == f'Gaia DR3 {gaia_dr3}')
+                plt.imshow(source.flux[0], origin='lower')
+                plt.show()
+                plt.close()
                 # print(source.gaia[891])
-                # print(source.gaia[140])
+                # print(source.gaia[star_num])
                 nearby_stars = np.argsort(
                     (source.gaia[f'sector_{sector}_x'][:500] - source.gaia[star_num][f'sector_{sector}_x']) ** 2 +
                     (source.gaia[f'sector_{sector}_y'][:500] - source.gaia[star_num][f'sector_{sector}_y']) ** 2)[0:5]
                 # print(f'sector = {source.sector}')
                 star_x = source.gaia[star_num][f'sector_{sector}_x'][0]
                 star_y = source.gaia[star_num][f'sector_{sector}_y'][0]
-                max_flux = np.max(
-                    np.median(source.flux[:, round(star_y) - 2:round(star_y) + 3, round(star_x) - 2:round(star_x) + 3],
+                max_flux = np.nanmax(
+                    np.nanmedian(source.flux[:, round(star_y) - 2:round(star_y) + 3, round(star_x) - 2:round(star_x) + 3],
                               axis=0))
-                fig = plt.figure(constrained_layout=False, figsize=(15, 7))
-                gs = fig.add_gridspec(5, 10)
-                gs.update(wspace=0.5, hspace=0.5)
+                fig = plt.figure(constrained_layout=False, figsize=(15, 5))
+                gs = fig.add_gridspec(5, 16)
+                gs.update(wspace=0.1, hspace=0.1)
                 ax0 = fig.add_subplot(gs[:5, :5])
-                ax0.imshow(source.flux[0], cmap='RdBu', vmin=-max_flux, vmax=max_flux, origin='lower')
+                ax0.imshow(np.median(source.flux, axis=0), cmap='RdBu', vmin=-max_flux, vmax=max_flux, origin='lower')
 
                 ax0.scatter(source.gaia[f'sector_{sector}_x'][:500], source.gaia[f'sector_{sector}_y'][:500], s=50,
                             c='r', label='background stars')
                 ax0.scatter(source.gaia[f'sector_{sector}_x'][nearby_stars],
                             source.gaia[f'sector_{sector}_y'][nearby_stars], s=50,
                             c='r', label='background stars')
                 for l in range(len(nearby_stars)):
@@ -376,31 +380,49 @@
                 #         ax_.plot(hdul[1].data['time'], cal_lc, '.k', ms=1, label='center pixel')
 
                 t_, y_, x_ = np.shape(hdul[0].data)
                 max_flux = np.max(
                     np.median(source.flux[:, int(star_y) - 2:int(star_y) + 3, int(star_x) - 2:int(star_x) + 3], axis=0))
                 for j in range(y_):
                     for k in range(x_):
-                        ax_ = fig.add_subplot(gs[(4 - j), (5 + k)])
+                        ax_ = fig.add_subplot(gs[(4 - j), (6 + 2 * k):(8 + 2 * k)])
                         ax_.patch.set_facecolor('C0')
                         ax_.patch.set_alpha(min(1, max(0, 5 * np.nanmedian(hdul[0].data[:, j, k]) / max_flux)))
                         q = [a and b for a, b in
                              zip(list(hdul[1].data['TESS_flags'] == 0), list(hdul[1].data['TGLC_flags'] == 0))]
 
                         _, trend = flatten(hdul[1].data['time'][q],
                                            hdul[0].data[:, j, k][q] - np.nanmin(hdul[0].data[:, j, k][q]) + 1000,
                                            window_length=1, method='biweight', return_trend=True)
                         cal_aper = (hdul[0].data[:, j, k][q] - np.nanmin(
                             hdul[0].data[:, j, k][q]) + 1000 - trend) / np.nanmedian(
                             hdul[0].data[:, j, k][q]) + 1
-                        ax_.plot(hdul[1].data['time'][q], cal_aper, '.k', ms=1, label='center pixel')
-                        ax_.set_ylim(0.95, 1.05)
-                plt.savefig(f'{local_directory}lc/plots/contamination_sector_{hdul[0].header["SECTOR"]:04d}.pdf',
+                        # ax_.plot(hdul[1].data['time'][q], cal_aper, '.k', ms=0.5)
+                        ax_.plot(hdul[1].data['time'][q], hdul[0].data[:, j, k][q], '.k', ms=0.5)
+                        # ax_.set_ylim(0.7, 1.3)
+                        if j != 0:
+                            ax_.set_xticklabels([])
+                        if k != 0:
+                            ax_.set_yticklabels([])
+
+                plt.savefig(f'{local_directory}plots/contamination_sector_{hdul[0].header["SECTOR"]:04d}.pdf',
                             dpi=300)
-                plt.show()
+                plt.close()
+
+
+def plot_epsf(local_directory=None):
+    files = glob(f'{local_directory}epsf/*.npy')
+    os.makedirs(f'{local_directory}plots/', exist_ok=True)
+    for i in range(len(files)):
+        psf = np.load(files[i])
+        plt.imshow(psf[0, :23 ** 2].reshape(23, 23), cmap='bone', origin='lower')
+        plt.tick_params(axis='x', bottom=False)
+        plt.tick_params(axis='y', left=False)
+        plt.title(f'{files[i].split("/")[-1].split(".")[0]}')
+        plt.savefig(f'{local_directory}plots/{files[i].split("/")[-1]}.png', bbox_inches='tight', dpi=300)
 
 
 def choose_prior(tics, local_directory=None, priors=np.logspace(-5, 0, 100)):
     mad = np.zeros((2, 100))
     for i in trange(len(priors)):
         resid = get_tglc_lc(tics=tics, method='query', server=1, directory=local_directory, prior=priors[i])
         print(resid)
@@ -425,25 +447,36 @@
         for i in range(len(tics)):
             target = f'TIC {tics[i]}'
             local_directory = f'{directory}{target}/'
             os.makedirs(local_directory, exist_ok=True)
             tglc_lc(target=target, local_directory=local_directory, size=90, save_aper=True, limit_mag=16,
                     get_all_lc=False, first_sector_only=False, last_sector_only=False, sector=None, prior=prior,
                     transient=None)
-            plot_lc(local_directory=f'{directory}TIC {tics[i]}/lc/', type='cal_aper_flux')
+            plot_lc(local_directory=f'{directory}TIC {tics[i]}/', type='cal_aper_flux')
     if method == 'search':
         star_spliter(server=server, tics=tics, local_directory=directory)
 
 
 if __name__ == '__main__':
-    tics = [56883709]
-    directory = f'/home/tehan/Documents/GEMS/'
+    tics = [16005254]
+    directory = f'/home/tehan/Documents/tglc/'
     # directory = f'/home/tehan/data/cosmos/GEMS/'
     os.makedirs(directory, exist_ok=True)
     get_tglc_lc(tics=tics, method='query', server=1, directory=directory)
-    plot_lc(local_directory=f'{directory}TIC {tics[0]}/lc/', type='cal_psf_flux')
-    plot_lc(local_directory=f'{directory}TIC {tics[0]}/lc/', type='cal_aper_flux')
-
+    plot_lc(local_directory=f'/home/tehan/Documents/tglc/TIC 16005254/', type='cal_aper_flux')
+    plot_contamination(local_directory=f'{directory}TIC {tics[0]}/', gaia_dr3=5751990597042725632)
+    # plot_epsf(local_directory=f'{directory}TIC {tics[0]}/')
     # plot_pf_lc(local_directory=f'{directory}TIC {tics[0]}/lc/', period=0.71912603, mid_transit_tbjd=2790.58344,
     #            type='cal_psf_flux')
     # plot_pf_lc(local_directory=f'{directory}TIC {tics[0]}/lc/', period=0.71912603, mid_transit_tbjd=2790.58344,
     #            type='cal_aper_flux')
+
+    # target = f'266.489125, -33.8428'
+    # directory = f'/home/tehan/data/cosmos/michelle/'
+    # local_directory = f'{directory}{target}/'
+    # os.makedirs(local_directory, exist_ok=True)
+    # tglc_lc(target=target, local_directory=local_directory, size=50, save_aper=True, limit_mag=17,
+    #         get_all_lc=False, first_sector_only=False, last_sector_only=False, sector=39, prior=None,
+    #         transient=['266.489125, -33.8428', 266.489125, -33.8428])
+    # plot_lc(local_directory=f'{local_directory}', type='cal_aper_flux')
+    # plot_lc(local_directory=f'{local_directory}', yhigh=150, type='aperture_flux')
+    # plot_contamination(local_directory=f'{local_directory}', gaia_dr3=4041831235071242624)
```

### Comparing `tglc-0.6.1/tglc/run.py` & `tglc-0.6.2/tglc/run.py`

 * *Files identical despite different names*

### Comparing `tglc-0.6.1/tglc/source_output.py` & `tglc-0.6.2/tglc/source_output.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -72,14 +72,14 @@
     # for i in range(16):
     #     ffi(camera=1 + i // 4, ccd=1 + i % 4, sector=sector, size=150, local_directory=local_directory)
 
 
 if __name__ == '__main__':
     sector = 56
     ffi_to_source(sector=sector, local_directory=f'/home/tehan/data/sector{sector:04d}/')
+    # med_mask = median_mask(sector_num=26)
     # ffi_to_source(sector=sector, local_directory=f'/pdo/users/tehan/sector{sector:04d}/')
     # files = glob.glob(f'/home/tehan/data/sector{sector:04d}/source/*/source_00_00.pkl')
     # for i in range(len(files)):
     #     with open(files[i], 'rb') as input_:
     #         source = pickle.load(input_)
     #         print(np.min(np.diff(source.cadence)), files[i])
-    # med_mask = median_mask(sector_num=26)
```

### Comparing `tglc-0.6.1/tglc/target_lightcurve.py` & `tglc-0.6.2/tglc/target_lightcurve.py`

 * *Files identical despite different names*

### Comparing `tglc-0.6.1/tglc.egg-info/PKG-INFO` & `tglc-0.6.2/tglc.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,69 +1,71 @@
 Metadata-Version: 2.1
 Name: tglc
-Version: 0.6.1
+Version: 0.6.2
 Summary: TESS-Gaia Light Curve
 Home-page: https://github.com/TeHanHunter/TESS_Gaia_Light_Curve
 Author: Te Han
 Author-email: tehanhunter@gmail.com
+License: UNKNOWN
+Description: ==================================
+        Introduction
+        ==================================
+        
+        TESS-Gaia Light Curve (`TGLC <https://archive.stsci.edu/hlsp/tglc>`_) is a dataset of TESS full-frame image light curves publicly available via the MAST portal. It is fitted with effective PSF and decontaminated with Gaia DR3 and achieved percent-level photometric precision down to 16th TESS magnitude! It unlocks astrophysics to a vast number of dim stars below 12th TESS magnitude. A package called tglc is pip-installable for customized light curve fits.
+        
+        
+        ==================================
+        Usage
+        ==================================
+        There are four fluxes in each FITS file: aperture flux, PSF flux, calibrated aperture flux, and calibrated PSF flux.
+        If you are uncertain which to use:
+        
+        * Calibrated psf flux is better in **deblending** targets. Use this if you need to deblend a target near a variable source. The best deblending can be achieved with tglc package by setting a non-zero prior. It also gives the more accurate **transit depth** in most cases, especially when fitting with an optimized prior.
+        * Calibrated aperture flux usually has slightly **higher SNR**. The transit depth (or variation amplitude), however, can be imperfect since the normalization depends on the PSF fitting which is imperfect. This imperfection can be minimized by using a bigger aperture than the default aperture (3*3). One need to use the tglc package and set tglc_lc(save_aper=True) to access the 5*5 aperture. In the presence of a bright but "constant" contamination (several magnitudes brighter), the calibrated aperture flux is better in removing the constant contamination. 
+        * The aperture flux and PSF flux are not detrended or normalized. Use this if you are doing stellar variability science with long baseline. Or, if the detrending is not optimal (default detrending has a window length of 1 day; see Known Problems below), start with the aperture flux or PSF flux and detrend carefully!
+        * **If you are uncertain, start with calibrated aperture flux!**
+        
+        The `tutorial <tutorial/TGLC_tutorial.ipynb>`_ shows the syntaxes and differences among these light curves in several examples.
+        
+        ==================================
+        Data Access
+        ==================================
+        There are three data access methods:
+        
+        * MAST Portal: Easiest for acquiring light curves for a few stars. However, new sectors are updated relatively slowly. 
+        * MAST bulk download: Best for downloading light curves for all stars (<16 TESS magnitude) in a sectors. 
+        * tglc package: Capable of producing similar quality light curves for any sector and any star with custom options. 
+        
+        MAST Portal/bulk download
+        ----------------------------
+        The easiest usage requires no package installation. Simply follow the `TGLC HLSP page <https://archive.stsci.edu/hlsp/tglc>`_ to download light curves from MAST or use `MAST Portal <https://mast.stsci.edu/portal/Mashup/Clients/Mast/Portal.html>`_. Light curves are being fitted sector by sector and will be available on MAST gradually. MAST hosts all Gaia DR3 stars down to 16th magnitude. Each .fits file includes PSF and aperture light curves and their calibrated versions.
+        
+        MAST available sectors: `sector worklist <https://docs.google.com/spreadsheets/d/1FhHElWb1wmx9asWiZecAJ2umN0-P_aXn55OBVB34_rg/edit?usp=sharing>`_
+        
+        
+        tglc package
+        ----------------------------
+        Users can also fit light curves using the package tglc. Using tglc, one can specify a region, sector(s), and customized aperture shape if needed. It can also allow all field stars to float by assigning Gaussian priors, which can help decontaminate variable field stars. tglc is currently only available for linux. Run::
+        
+          pip install tglc
+          
+        for the latest tglc release. After installation, follow the `tutorial <tutorial/TGLC_tutorial.ipynb>`_ to fit light curves. If there is a problem, please leave a comment in the Issues section to help us improve. Thank you!
+        
+        
+        ==================================
+        Known Problems
+        ==================================
+        There are several imperfections we noticed in the MAST TGLC light curves and tglc package:
+        
+        * If the star is very dim (~< 15 Tmag) near a variable source, it can make the aperture and/or PSF light curve negative for some cadences. The detrending algorithm could malfunction and result in bad cal_aper_flux and/or cal_psf_flux. This is now fixed for tglc package, but this problem remains for the primary mission light curves published on MAST. Please detrend again if necessary. The extended mission light curves on MAST will not be affected. This is a very rare scenario, but could be important.
+        
+        ==================================
+        Reference
+        ==================================
+        If you find the TGLC light curves or the tglc package useful in your research, please cite `our paper <https://iopscience.iop.org/article/10.3847/1538-3881/acaaa7>`_ published on the Astronomical Journal. 
+        
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
-License-File: LICENSE
-
-==================================
-Introduction
-==================================
-
-TESS-Gaia Light Curve (`TGLC <https://archive.stsci.edu/hlsp/tglc>`_) is a dataset of TESS full-frame image light curves publicly available via the MAST portal. It is fitted with effective PSF and decontaminated with Gaia DR3 and achieved percent-level photometric precision down to 16th TESS magnitude! It unlocks astrophysics to a vast number of dim stars below 12th TESS magnitude. A package called tglc is pip-installable for customized light curve fits.
-
-==================================
-Usage
-==================================
-There are four fluxes in each FITS file: aperture flux, PSF flux, calibrated aperture flux, and calibrated PSF flux.
-If you are uncertain which to use:
-
-* Calibrated psf flux is better in **deblending** targets. Use this if you need to deblend a target near a variable source. The best deblending can be achieved with tglc package by setting a non-zero prior. It also gives the more accurate **transit depth** in most cases, especially when fitting with an optimized prior.
-* Calibrated aperture flux usually has slightly **higher SNR**. The transit depth (or variation amplitude), however, can be imperfect since the normalization depends on the PSF fitting which is imperfect. This imperfection can be minimized by using a bigger aperture than the default aperture (3*3). One need to use the tglc package and set tglc_lc(save_aper=True) to access the 5*5 aperture. In the presence of a bright but "constant" contamination (several magnitudes brighter), the calibrated aperture flux is better in removing the constant contamination. 
-* The aperture flux and PSF flux are not detrended or normalized. Use this if you are doing stellar variability science with long baseline. Or, if the detrending is not optimal (default detrending has a window length of 1 day; see Known Problems below), start with the aperture flux or PSF flux and detrend carefully!
-* **If you are uncertain, start with calibrated aperture flux!**
-
-The `tutorial <tutorial/TGLC_tutorial.ipynb>`_ shows the syntaxes and differences among these light curves in several examples.
-
-==================================
-Data Access
-==================================
-There are three data access methods:
-
-* MAST Portal: Easiest for acquiring light curves for a few stars. However, new sectors are updated relatively slowly. 
-* MAST bulk download: Best for downloading light curves for all stars (<16 TESS magnitude) in a sectors. 
-* tglc package: Capable of producing similar quality light curves for any sector and any star with custom options. 
-
-MAST Portal/bulk download
-----------------------------
-The easiest usage requires no package installation. Simply follow the `TGLC HLSP page <https://archive.stsci.edu/hlsp/tglc>`_ to download light curves from MAST or use `MAST Portal <https://mast.stsci.edu/portal/Mashup/Clients/Mast/Portal.html>`_. Light curves are being fitted sector by sector and will be available on MAST gradually. MAST hosts all Gaia DR3 stars down to 16th magnitude. Each .fits file includes PSF and aperture light curves and their calibrated versions.
-
-MAST available sectors: `sector worklist <https://docs.google.com/spreadsheets/d/1FhHElWb1wmx9asWiZecAJ2umN0-P_aXn55OBVB34_rg/edit?usp=sharing>`_
-
-
-tglc package
-----------------------------
-Users can also fit light curves using the package tglc. Using tglc, one can specify a region, sector(s), and customized aperture shape if needed. It can also allow all field stars to float by assigning Gaussian priors, which can help decontaminate variable field stars. tglc is currently only available for linux. Run::
-
-  pip install tglc
-  
-for the latest tglc release. After installation, follow the `tutorial <tutorial/TGLC_tutorial.ipynb>`_ to fit light curves. If there is a problem, please leave a comment in the Issues section to help us improve. Thank you!
-
-
-==================================
-Known Problems
-==================================
-There are several imperfections we noticed in the MAST TGLC light curves and tglc package:
-
-* If the star is very dim (~< 15 Tmag) near a variable source, it can make the aperture and/or PSF light curve negative for some cadences. The detrending algorithm could malfunction and result in bad cal_aper_flux and/or cal_psf_flux. This is now fixed for tglc package, but this problem remains for the primary mission light curves published on MAST. Please detrend again if necessary. The extended mission light curves on MAST will not be affected. This is a very rare scenario, but could be important.
-
-==================================
-Reference
-==================================
-If you find the TGLC light curves or the tglc package useful in your research, please cite `our paper <https://iopscience.iop.org/article/10.3847/1538-3881/acaaa7>`_ published on the Astronomical Journal.
```

