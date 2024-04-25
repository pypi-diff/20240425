# Comparing `tmp/cdcs-0.2.2.tar.gz` & `tmp/cdcs-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\lmh1\Documents\Python-packages\pycdcs\dist\.tmp-2p1qn8nc\cdcs-0.2.2.tar", last modified: Thu Jul 27 14:26:45 2023, max compression
+gzip compressed data, was "cdcs-0.2.3.tar", last modified: Thu Apr 25 19:37:43 2024, max compression
```

## Comparing `cdcs-0.2.2.tar` & `cdcs-0.2.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 14:26:45.000000 cdcs-0.2.2/
--rw-rw-rw-   0        0        0     2776 2019-07-10 17:30:09.000000 cdcs-0.2.2/LICENSE.TXT
--rw-rw-rw-   0        0        0     2584 2023-07-27 14:26:45.000000 cdcs-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     1776 2023-01-25 20:27:28.000000 cdcs-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 14:26:45.000000 cdcs-0.2.2/cdcs/
-drwxrwxrwx   0        0        0        0 2023-07-27 14:26:45.000000 cdcs-0.2.2/cdcs/CDCS/
--rw-rw-rw-   0        0        0     5811 2023-03-24 16:59:19.000000 cdcs-0.2.2/cdcs/CDCS/__init__.py
--rw-rw-rw-   0        0        0    10931 2022-07-27 10:57:44.000000 cdcs-0.2.2/cdcs/CDCS/_blob.py
--rw-rw-rw-   0        0        0     4957 2022-07-20 17:25:54.000000 cdcs-0.2.2/cdcs/CDCS/_pid_xpath.py
--rw-rw-rw-   0        0        0    13469 2022-12-06 16:24:16.000000 cdcs-0.2.2/cdcs/CDCS/_query.py
--rw-rw-rw-   0        0        0    23612 2023-07-26 14:08:04.000000 cdcs-0.2.2/cdcs/CDCS/_record.py
--rw-rw-rw-   0        0        0    26279 2023-01-25 19:18:42.000000 cdcs-0.2.2/cdcs/CDCS/_template.py
--rw-rw-rw-   0        0        0     1696 2022-03-01 22:03:10.000000 cdcs-0.2.2/cdcs/CDCS/_workspace.py
--rw-rw-rw-   0        0        0    10628 2023-01-24 19:26:21.000000 cdcs-0.2.2/cdcs/CDCS/_xslt.py
--rw-rw-rw-   0        0        0    14641 2022-03-01 22:03:10.000000 cdcs-0.2.2/cdcs/RestClient.py
--rw-rw-rw-   0        0        0        5 2023-07-26 14:08:04.000000 cdcs-0.2.2/cdcs/VERSION
--rw-rw-rw-   0        0        0      959 2023-07-26 14:08:04.000000 cdcs-0.2.2/cdcs/__init__.py
--rw-rw-rw-   0        0        0     1041 2023-03-24 16:58:09.000000 cdcs-0.2.2/cdcs/aslist.py
--rw-rw-rw-   0        0        0      607 2022-07-26 19:26:46.000000 cdcs-0.2.2/cdcs/date_parser.py
-drwxrwxrwx   0        0        0        0 2023-07-27 14:26:45.000000 cdcs-0.2.2/cdcs.egg-info/
--rw-rw-rw-   0        0        0     2584 2023-07-27 14:26:45.000000 cdcs-0.2.2/cdcs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      467 2023-07-27 14:26:45.000000 cdcs-0.2.2/cdcs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 14:26:45.000000 cdcs-0.2.2/cdcs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2019-12-17 16:24:01.000000 cdcs-0.2.2/cdcs.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       29 2023-07-27 14:26:45.000000 cdcs-0.2.2/cdcs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-27 14:26:45.000000 cdcs-0.2.2/cdcs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2022-02-03 20:26:52.000000 cdcs-0.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-27 14:26:45.000000 cdcs-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1522 2023-07-26 14:08:04.000000 cdcs-0.2.2/setup.py
+drwxr-xr-x   0 lmh1      (1000) lmh1      (1000)        0 2024-04-25 19:37:43.718540 cdcs-0.2.3/
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)     2760 2023-08-31 19:58:02.000000 cdcs-0.2.3/LICENSE.TXT
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)     2574 2024-04-25 19:37:43.717542 cdcs-0.2.3/PKG-INFO
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)     1746 2023-08-31 19:58:02.000000 cdcs-0.2.3/README.md
+drwxr-xr-x   0 lmh1      (1000) lmh1      (1000)        0 2024-04-25 19:37:43.702541 cdcs-0.2.3/cdcs/
+drwxr-xr-x   0 lmh1      (1000) lmh1      (1000)        0 2024-04-25 19:37:43.715541 cdcs-0.2.3/cdcs/CDCS/
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)     5838 2024-04-02 15:17:51.000000 cdcs-0.2.3/cdcs/CDCS/__init__.py
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)    10599 2023-08-31 19:58:02.000000 cdcs-0.2.3/cdcs/CDCS/_blob.py
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)     6752 2024-04-02 14:57:20.000000 cdcs-0.2.3/cdcs/CDCS/_pid.py
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)    13182 2023-11-01 18:39:15.000000 cdcs-0.2.3/cdcs/CDCS/_query.py
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)    24782 2024-04-04 18:14:42.000000 cdcs-0.2.3/cdcs/CDCS/_record.py
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)    25938 2024-03-26 16:55:50.000000 cdcs-0.2.3/cdcs/CDCS/_template.py
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)     1631 2023-08-31 19:58:02.000000 cdcs-0.2.3/cdcs/CDCS/_workspace.py
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)    10312 2023-08-31 19:58:02.000000 cdcs-0.2.3/cdcs/CDCS/_xslt.py
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)    14876 2024-03-21 20:14:22.000000 cdcs-0.2.3/cdcs/RestClient.py
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)        5 2024-03-25 18:29:45.000000 cdcs-0.2.3/cdcs/VERSION
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)      569 2023-08-31 19:58:02.000000 cdcs-0.2.3/cdcs/__init__.py
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)      993 2023-08-31 19:58:02.000000 cdcs-0.2.3/cdcs/aslist.py
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)      584 2023-08-31 19:58:02.000000 cdcs-0.2.3/cdcs/date_parser.py
+drwxr-xr-x   0 lmh1      (1000) lmh1      (1000)        0 2024-04-25 19:37:43.716542 cdcs-0.2.3/cdcs.egg-info/
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)     2574 2024-04-25 19:37:43.000000 cdcs-0.2.3/cdcs.egg-info/PKG-INFO
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)      461 2024-04-25 19:37:43.000000 cdcs-0.2.3/cdcs.egg-info/SOURCES.txt
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)        1 2024-04-25 19:37:43.000000 cdcs-0.2.3/cdcs.egg-info/dependency_links.txt
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)        1 2023-09-01 15:40:17.000000 cdcs-0.2.3/cdcs.egg-info/not-zip-safe
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)       29 2024-04-25 19:37:43.000000 cdcs-0.2.3/cdcs.egg-info/requires.txt
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)        5 2024-04-25 19:37:43.000000 cdcs-0.2.3/cdcs.egg-info/top_level.txt
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)      103 2023-08-31 19:58:02.000000 cdcs-0.2.3/pyproject.toml
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)       38 2024-04-25 19:37:43.719559 cdcs-0.2.3/setup.cfg
+-rw-r--r--   0 lmh1      (1000) lmh1      (1000)     1465 2023-08-31 19:58:02.000000 cdcs-0.2.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cdcs-0.2.2/LICENSE.TXT` & `cdcs-0.2.3/LICENSE.TXT`

 * *Ordering differences only*

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-Licensing
-=========
-
-License Information for NIST data (other than Standard Reference Data (SRD))
-
-This data was developed by employees of the National Institute of Standards and Technology (NIST), an agency of the Federal Government. Pursuant to title 15 United States Code Section 105, works of NIST employees are not subject to copyright protection in the United States and are considered to be in the public domain.
-
-The data is provided by NIST as a public service and is expressly provided “AS IS.” NIST MAKES NO WARRANTY OF ANY KIND, EXPRESS, IMPLIED OR STATUTORY, INCLUDING, WITHOUT LIMITATION, THE IMPLIED WARRANTY OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, NON-INFRINGEMENT AND DATA ACCURACY. NIST does not warrant or make any representations regarding the use of the data or the results thereof, including but not limited to the correctness, accuracy, reliability or usefulness of the data. NIST SHALL NOT BE LIABLE AND YOU HEREBY RELEASE NIST FROM LIABILITY FOR ANY INDIRECT, CONSEQUENTIAL, SPECIAL, OR INCIDENTAL DAMAGES (INCLUDING DAMAGES FOR LOSS OF BUSINESS PROFITS, BUSINESS INTERRUPTION, LOSS OF BUSINESS INFORMATION, AND THE LIKE), WHETHER ARISING IN TORT, CONTRACT, OR OTHERWISE, ARISING FROM OR RELATING TO THE DATA (OR THE USE OF OR INABILITY TO USE THIS DATA), EVEN IF NIST HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.
-To the extent that NIST may hold copyright in countries other than the United States, you are hereby granted the non-exclusive irrevocable and unconditional right to print, publish, prepare derivative works and distribute the NIST data, in any medium, or authorize others to do so on your behalf, on a royalty-free basis throughout the World.
-
-You may improve, modify, and create derivative works of the data or any portion of the data, and you may copy and distribute such modifications or works. Modified works should carry a notice stating that you changed the data and should note the date and nature of any such change. Please explicitly acknowledge the National Institute of Standards and Technology as the source of the data.
-
-Permission to use this data is contingent upon your acceptance of the terms of this agreement and upon your providing appropriate acknowledgments of NIST’s creation of the data.
-
-Copyright Protection for NIST Standard Reference Data (SRD)
-
+Licensing
+=========
+
+License Information for NIST data (other than Standard Reference Data (SRD))
+
+This data was developed by employees of the National Institute of Standards and Technology (NIST), an agency of the Federal Government. Pursuant to title 15 United States Code Section 105, works of NIST employees are not subject to copyright protection in the United States and are considered to be in the public domain.
+
+The data is provided by NIST as a public service and is expressly provided “AS IS.” NIST MAKES NO WARRANTY OF ANY KIND, EXPRESS, IMPLIED OR STATUTORY, INCLUDING, WITHOUT LIMITATION, THE IMPLIED WARRANTY OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, NON-INFRINGEMENT AND DATA ACCURACY. NIST does not warrant or make any representations regarding the use of the data or the results thereof, including but not limited to the correctness, accuracy, reliability or usefulness of the data. NIST SHALL NOT BE LIABLE AND YOU HEREBY RELEASE NIST FROM LIABILITY FOR ANY INDIRECT, CONSEQUENTIAL, SPECIAL, OR INCIDENTAL DAMAGES (INCLUDING DAMAGES FOR LOSS OF BUSINESS PROFITS, BUSINESS INTERRUPTION, LOSS OF BUSINESS INFORMATION, AND THE LIKE), WHETHER ARISING IN TORT, CONTRACT, OR OTHERWISE, ARISING FROM OR RELATING TO THE DATA (OR THE USE OF OR INABILITY TO USE THIS DATA), EVEN IF NIST HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.
+To the extent that NIST may hold copyright in countries other than the United States, you are hereby granted the non-exclusive irrevocable and unconditional right to print, publish, prepare derivative works and distribute the NIST data, in any medium, or authorize others to do so on your behalf, on a royalty-free basis throughout the World.
+
+You may improve, modify, and create derivative works of the data or any portion of the data, and you may copy and distribute such modifications or works. Modified works should carry a notice stating that you changed the data and should note the date and nature of any such change. Please explicitly acknowledge the National Institute of Standards and Technology as the source of the data.
+
+Permission to use this data is contingent upon your acceptance of the terms of this agreement and upon your providing appropriate acknowledgments of NIST’s creation of the data.
+
+Copyright Protection for NIST Standard Reference Data (SRD)
+
 Copyright protection on this compilation of data has been secured by the U.S. Department of Commerce in the United States and in other countries that are parties to the Universal Copyright Convention, pursuant to Section 290(e) of Title 15 of the United States Code. NIST Standard Reference Data (SRD); ©Copyright ©2013 by the U.S. Secretary of Commerce on behalf of the United States of America. All rights reserved.
```

### Comparing `cdcs-0.2.2/PKG-INFO` & `cdcs-0.2.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,52 @@
-Metadata-Version: 2.1
-Name: cdcs
-Version: 0.2.2
-Summary: Python API client for performing REST calls to configurable data curation system (CDCS) databases
-Home-page: https://github.com/usnistgov/pycdcs
-Author: Lucas Hale
-Author-email: lucas.hale@nist.gov
-Keywords: CDCS,database,rest API,configurable data curation system
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering :: Physics
-License-File: LICENSE.TXT
-
-# Python CDCS REST API client
-
-This is a base Python package for accessing instances of the NIST Configurable Data Curation System (CDCS) databases, versions 2.X.X and 3.X.X.  It defines a Python CDCS class that streamlines REST calls to a database by
-
-- Taking access settings once (username, password, etc) and saving them for subsequent REST calls.
-- Defining methods that wrap around REST calls to interact with the database in a more Pythonic way.
-- Automatically converting any accessed information to pandas Series and DataFrame objects to allow for the information to be easily manipulated.
-
-## Installation
-
-The package can be installed using pip:
-
-    pip install cdcs
-
-or conda:
-
-    conda install -c conda-forge cdcs
-
-Alternatively, the source code can be downloaded from github at
-
-- Stable releases: [https://github.com/usnistgov/pycdcs](https://github.com/usnistgov/pycdcs)
-- In development: [https://github.com/lmhale99/pycdcs](https://github.com/lmhale99/pycdcs)
-
-## Documentation
-
-Documentation for the package is given as Jupyter Notebooks that can be found on the github site.  Each Notebook is focused on providing details and examples related to different use cases for the package.
-
-- **CDCS Public Data Exploration** outlines the basic functions allowing an anonymous user (i.e. not logged in) to explore the available public data on a curator.
-- **CDCS Data Management** outlines the basic pre-defined functions allowing a logged-in user to manage their own templates, data records and blobs.
-- **CDCS Rest Builder** provides a simple explanation of how users can easily build their own functions and make their own REST API calls should they wish to interact with the database in ways outside the pre-defined functions.
+Metadata-Version: 2.1
+Name: cdcs
+Version: 0.2.3
+Summary: Python API client for performing REST calls to configurable data curation system (CDCS) databases
+Home-page: https://github.com/usnistgov/pycdcs
+Author: Lucas Hale
+Author-email: lucas.hale@nist.gov
+Keywords: CDCS,database,rest API,configurable data curation system
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering :: Physics
+License-File: LICENSE.TXT
+Requires-Dist: requests
+Requires-Dist: pandas
+Requires-Dist: tqdm
+Requires-Dist: ipython
+
+# Python CDCS REST API client
+
+This is a base Python package for accessing instances of the NIST Configurable Data Curation System (CDCS) databases, versions 2.X.X and 3.X.X.  It defines a Python CDCS class that streamlines REST calls to a database by
+
+- Taking access settings once (username, password, etc) and saving them for subsequent REST calls.
+- Defining methods that wrap around REST calls to interact with the database in a more Pythonic way.
+- Automatically converting any accessed information to pandas Series and DataFrame objects to allow for the information to be easily manipulated.
+
+## Installation
+
+The package can be installed using pip:
+
+    pip install cdcs
+
+or conda:
+
+    conda install -c conda-forge cdcs
+
+Alternatively, the source code can be downloaded from github at
+
+- Stable releases: [https://github.com/usnistgov/pycdcs](https://github.com/usnistgov/pycdcs)
+- In development: [https://github.com/lmhale99/pycdcs](https://github.com/lmhale99/pycdcs)
+
+## Documentation
+
+Documentation for the package is given as Jupyter Notebooks that can be found on the github site.  Each Notebook is focused on providing details and examples related to different use cases for the package.
+
+- **CDCS Public Data Exploration** outlines the basic functions allowing an anonymous user (i.e. not logged in) to explore the available public data on a curator.
+- **CDCS Data Management** outlines the basic pre-defined functions allowing a logged-in user to manage their own templates, data records and blobs.
+- **CDCS Rest Builder** provides a simple explanation of how users can easily build their own functions and make their own REST API calls should they wish to interact with the database in ways outside the pre-defined functions.
```

### Comparing `cdcs-0.2.2/README.md` & `cdcs-0.2.3/README.md`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-# Python CDCS REST API client
-
-This is a base Python package for accessing instances of the NIST Configurable Data Curation System (CDCS) databases, versions 2.X.X and 3.X.X.  It defines a Python CDCS class that streamlines REST calls to a database by
-
-- Taking access settings once (username, password, etc) and saving them for subsequent REST calls.
-- Defining methods that wrap around REST calls to interact with the database in a more Pythonic way.
-- Automatically converting any accessed information to pandas Series and DataFrame objects to allow for the information to be easily manipulated.
-
-## Installation
-
-The package can be installed using pip:
-
-    pip install cdcs
-
-or conda:
-
-    conda install -c conda-forge cdcs
-
-Alternatively, the source code can be downloaded from github at
-
-- Stable releases: [https://github.com/usnistgov/pycdcs](https://github.com/usnistgov/pycdcs)
-- In development: [https://github.com/lmhale99/pycdcs](https://github.com/lmhale99/pycdcs)
-
-## Documentation
-
-Documentation for the package is given as Jupyter Notebooks that can be found on the github site.  Each Notebook is focused on providing details and examples related to different use cases for the package.
-
-- **CDCS Public Data Exploration** outlines the basic functions allowing an anonymous user (i.e. not logged in) to explore the available public data on a curator.
-- **CDCS Data Management** outlines the basic pre-defined functions allowing a logged-in user to manage their own templates, data records and blobs.
-- **CDCS Rest Builder** provides a simple explanation of how users can easily build their own functions and make their own REST API calls should they wish to interact with the database in ways outside the pre-defined functions.
+# Python CDCS REST API client
+
+This is a base Python package for accessing instances of the NIST Configurable Data Curation System (CDCS) databases, versions 2.X.X and 3.X.X.  It defines a Python CDCS class that streamlines REST calls to a database by
+
+- Taking access settings once (username, password, etc) and saving them for subsequent REST calls.
+- Defining methods that wrap around REST calls to interact with the database in a more Pythonic way.
+- Automatically converting any accessed information to pandas Series and DataFrame objects to allow for the information to be easily manipulated.
+
+## Installation
+
+The package can be installed using pip:
+
+    pip install cdcs
+
+or conda:
+
+    conda install -c conda-forge cdcs
+
+Alternatively, the source code can be downloaded from github at
+
+- Stable releases: [https://github.com/usnistgov/pycdcs](https://github.com/usnistgov/pycdcs)
+- In development: [https://github.com/lmhale99/pycdcs](https://github.com/lmhale99/pycdcs)
+
+## Documentation
+
+Documentation for the package is given as Jupyter Notebooks that can be found on the github site.  Each Notebook is focused on providing details and examples related to different use cases for the package.
+
+- **CDCS Public Data Exploration** outlines the basic functions allowing an anonymous user (i.e. not logged in) to explore the available public data on a curator.
+- **CDCS Data Management** outlines the basic pre-defined functions allowing a logged-in user to manage their own templates, data records and blobs.
+- **CDCS Rest Builder** provides a simple explanation of how users can easily build their own functions and make their own REST API calls should they wish to interact with the database in ways outside the pre-defined functions.
```

### Comparing `cdcs-0.2.2/cdcs/CDCS/_blob.py` & `cdcs-0.2.3/cdcs/CDCS/_blob.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,332 +1,332 @@
-# coding: utf-8
-
-# Standard library imports
-import io
-from pathlib import Path
-from typing import Optional, Union
-
-# https://pandas.pydata.org/
-import pandas as pd
-
-# Local imports
-from .. import aslist, date_parser
-
-blob_keys = ['id', ',user_id', 'filename', 'handle', 'upload_date', 'pid']
-
-def upload_blob(self, filename: Union[str, Path],
-                blobbytes: Optional[io.BytesIO] = None,
-                workspace: Union[str, pd.Series, None] = None,
-                verbose: bool = False) -> str:
-    """
-    Adds a blob file to the repository.
-    
-    Parameters
-    ----------
-    filename : str or Path
-        The path to the file to upload.
-    blobbytes : io.BytesIO, optional
-        Pre-loaded file contents.  Allows files already opened to be passed in.
-    workspace : str or pandas.Series, optional
-        If given, the blob will be assigned to this workspace after
-        successfully being uploaded.
-    verbose : bool, optional
-        Setting this to True will print extra status messages.  Default value
-        is False.
-    
-    Returns
-    -------
-    str
-        The URL handle where the blob can be downloaded from.
-    """
-    # Read file content
-    if blobbytes is None:
-        blobbytes = open(filename, 'rb')
-    
-    # Read file content
-    files = {}
-    files['blob'] = blobbytes
-    
-    # Set file name
-    data  = {}
-    data = {'filename': filename}
-    
-    # Send request
-    rest_url = '/rest/blob/'
-    response = self.post(rest_url, files=files, data=data)
-    blob = pd.Series(response.json())
-
-    if verbose and response.status_code == 201:    
-        print(f'File "{filename}" uploaded as blob "{blob.filename}" ({blob.id})')
-    
-    if workspace is not None:
-        assign_blobs(self, workspace, ids=blob.id, verbose=verbose)
-
-    return blob.handle
-    
-def get_blobs(self,
-              filename: Optional[str] = None,
-              parse_dates: bool = True) -> pd.DataFrame:
-    """
-    Retrieves the metadata for blobs
-    
-    Parameters
-    ----------
-    filename : str, optional
-        The name of the file to limit the search by.
-    parse_dates : bool, optional
-        If True (default) then date fields will automatically be parsed into
-        pandas.Timestamp objects.  If False they will be left as str values.
-
-    Returns
-    -------
-    pandas.DataFrame
-        The metadata for all matching blobs.
-    """
-    
-    # Set params
-    params = {}
-    if filename is not None:
-        params['filename'] = filename
-    
-    # Send response
-    rest_url = '/rest/blob/'
-    response = self.get(rest_url, params=params)
-    
-    blobs = pd.DataFrame(response.json())
-    if len(blobs) == 0:
-        blobs = pd.DataFrame(columns=blob_keys)
-
-    if parse_dates and len(blobs) > 0:
-        blobs.upload_date = blobs.apply(date_parser, args=['upload_date'], axis=1)
-
-    return blobs
-
-def get_blob(self,
-             id: Optional[str] = None,
-             filename: Optional[str] = None,
-             parse_dates: bool = True) -> pd.Series:
-    """
-    Retrieves the metadata for a single blob.  The blob can be uniquely
-    identified using its id or filename.
-    
-    Parameters
-    ----------
-    id : str, optional
-        The unique ID associated with the blob.
-    filename : str, optional
-        The name of the file to limit the search by.
-    parse_dates : bool, optional
-        If True (default) then date fields will automatically be parsed into
-        pandas.Timestamp objects.  If False they will be left as str values.
-
-    Returns
-    -------
-    pandas.Series
-        The metadata for the matching blob.
-
-    Raises
-    ------
-    ValueError
-        If both id and filename are given, or if exactly one matching blob not
-        found.
-    """
-    if id is None:
-        blobs = self.get_blobs(filename=filename, parse_dates=parse_dates)
-        
-        if len(blobs) == 1:
-            return blobs.iloc[0]
-        elif len(blobs) == 0:
-            raise ValueError('No matching blobs found')
-        else:
-            raise ValueError('Multiple matching blobs found')
-    else:
-        if filename is not None:
-            raise ValueError('id and filename cannot both be given')
-        rest_url = f'/rest/blob/{id}'
-        response = self.get(rest_url)
-        blob = pd.Series(response.json())
-
-        if parse_dates:
-            blob.upload_date = date_parser(blob, 'upload_date')
-
-        return blob
-
-def assign_blobs(self, workspace: Union[str, pd.Series],
-                 blobs: Union[pd.Series, pd.DataFrame, None] = None,
-                 ids: Union[str, list, None] = None,
-                 filename: Optional[str] = None,
-                 verbose: bool = False):
-    """
-    Assigns one or more blobs to a workspace.
-
-    Parameters
-    ----------
-    workspace : str or pandas.Series
-        The workspace or workspace title to assign the blobs to.
-    blobs : pandas.Series or pandas.DataFrame, optional
-        Pre-selected blobs to assign to the workspace.  Cannot be given with
-        ids or filename.
-    ids : str or list, optional
-        The ID(s) of the blobs to assign to the workspace.  Selecting blobs
-        using ids has the least overhead. Cannot be given with blobs or
-        filename.
-    filename : str, optional
-        The name of the blob file to assign to the workspace.  Cannot be given
-        with blobs or ids.
-    verbose : bool, optional
-        Setting this to True will print extra status messages.  Default value
-        is False.
-    """
-    # Get workspace id
-    if isinstance(workspace, str):
-        workspace = self.get_workspace(workspace)
-    workspace_id = workspace.id
-    
-    # Get blobs from filename
-    if filename is not None:
-        if blobs is not None or ids is not None:
-            raise ValueError('filename cannot be given with blobs or ids')
-        blobs = get_blobs(self, filename=filename)
-
-    # Get ids from blobs
-    if blobs is not None:
-        if ids is not None:
-            raise ValueError('blobs and ids cannot both be given')
-        if isinstance(blobs, pd.Series):
-            ids = [blobs.id]
-        elif isinstance(blobs, pd.DataFrame):
-            ids = blobs.id.tolist()
-        else:
-            raise TypeError('invalid blobs type')
-    
-    if ids is None:
-        raise ValueError('No blobs specified to assign to the workspace')
-
-    # Assign blobs to the workspace
-    for blob_id in aslist(ids):
-        rest_url = f'/rest/blob/{blob_id}/assign/{workspace_id}'
-        response = self.patch(rest_url)
-
-        if verbose and response.status_code == 200:
-            print(f'blob {blob_id} assigned to workspace {workspace_id}')
-
-def get_blob_contents(self, blob: Optional[pd.Series] = None, 
-                      id: Optional[str] = None,
-                      filename: Optional[str] = None) -> bytes:
-    """
-    Retrieves the contents for a single blob.  The blob can be uniquely
-    identified by passing the blob metadata, or by using its id or filename.
-    
-    Parameters
-    ----------
-    blob : pandas.Series, optional
-        The blob metadata for a blob.
-    id : str, optional
-        The unique ID associated with the blob.
-    filename : str, optional
-        The name of the file to limit the search by.
-    
-    Returns
-    -------
-    bytes
-        The blob file contents.
-
-    Raises
-    ------
-    ValueError
-        If more than one argument given, or if filename does not uniquely
-        identify a blob.
-    """
-
-    if blob is None:
-        blob = self.get_blob(id=id, filename=filename)
-    elif id is not None:
-        raise ValueError('blob and id cannot both be given')
-    elif filename is not None:
-        raise ValueError('blob and filename cannot both be given')
-    
-    rest_url = f'/rest/blob/download/{blob.id}'
-    response = self.get(rest_url)
-    return response.content
-        
-def download_blob(self, blob: Optional[pd.Series] = None,
-                  id: Optional[str] = None,
-                  filename: Optional[str] = None,
-                  savedir: Union[str, Path] = '.') -> bytes:
-    """
-    Retrieves the contents for a single blob and saves it using the stored file
-    name.  The blob can be uniquely identified by passing the blob metadata, or
-    by using its id or filename.
-    
-    Parameters
-    ----------
-    blob : pandas.Series, optional 
-        The blob metadata for a blob.
-    id : str, optional
-        The unique ID associated with the blob.
-    filename : str, optional
-        The name of the file to limit the search by.
-    savedir : str or Path, optional
-        The directory to save the file to.  Default value uses the current
-        working directory.
-    
-    Returns
-    -------
-    bytes
-        The blob file contents.
-
-    Raises
-    ------
-    ValueError
-        If more than one argument given, or if filename does not uniquely
-        identify a blob.
-    """
-    if blob is None:
-        blob = self.get_blob(id=id, filename=filename)
-    elif id is not None:
-        raise ValueError('blob and id cannot both be given')
-    elif filename is not None:
-        raise ValueError('blob and filename cannot both be given')
-        
-    savepath = Path(savedir, blob.filename)
-    with open(savepath, 'wb') as f:
-        f.write(self.get_blob_contents(blob=blob))
-
-def delete_blob(self, blob: Optional[pd.Series] = None,
-                id: Optional[str] = None,
-                filename: Optional[str] = None,
-                verbose: bool = False):
-    """
-    Deletes a single blob from the curator.  The blob can be uniquely
-    identified by passing the blob metadata, or by using its id or filename.
-    
-    Parameters
-    ----------
-    blob : pandas.Series, optional
-        The blob metadata for a blob.
-    id : str, optional
-        The unique ID associated with the blob.
-    filename : str, optional
-        The name of the file to limit the search by.
-    verbose : bool, optional
-        Setting this to True will print extra status messages.  Default value
-        is False.
-    
-    Raises
-    ------
-    ValueError
-        If more than one argument given, or if filename does not uniquely
-        identify a blob.
-    """
-    if blob is None:
-        blob = self.get_blob(id=id, filename=filename)
-    elif id is not None:
-        raise ValueError('blob and id cannot both be given')
-    elif filename is not None:
-        raise ValueError('blob and filename cannot both be given')
-        
-    rest_url = f'/rest/blob/{blob.id}'
-    response = self.delete(rest_url)
-    
-    if verbose and response.status_code == 204:
-        print(f'Successfully deleted blob "{blob.filename}" ({blob.id})')
+# coding: utf-8
+
+# Standard library imports
+import io
+from pathlib import Path
+from typing import Optional, Union
+
+# https://pandas.pydata.org/
+import pandas as pd
+
+# Local imports
+from .. import aslist, date_parser
+
+blob_keys = ['id', ',user_id', 'filename', 'handle', 'upload_date', 'pid']
+
+def upload_blob(self, filename: Union[str, Path],
+                blobbytes: Optional[io.BytesIO] = None,
+                workspace: Union[str, pd.Series, None] = None,
+                verbose: bool = False) -> str:
+    """
+    Adds a blob file to the repository.
+    
+    Parameters
+    ----------
+    filename : str or Path
+        The path to the file to upload.
+    blobbytes : io.BytesIO, optional
+        Pre-loaded file contents.  Allows files already opened to be passed in.
+    workspace : str or pandas.Series, optional
+        If given, the blob will be assigned to this workspace after
+        successfully being uploaded.
+    verbose : bool, optional
+        Setting this to True will print extra status messages.  Default value
+        is False.
+    
+    Returns
+    -------
+    str
+        The URL handle where the blob can be downloaded from.
+    """
+    # Read file content
+    if blobbytes is None:
+        blobbytes = open(filename, 'rb')
+    
+    # Read file content
+    files = {}
+    files['blob'] = blobbytes
+    
+    # Set file name
+    data  = {}
+    data = {'filename': filename}
+    
+    # Send request
+    rest_url = '/rest/blob/'
+    response = self.post(rest_url, files=files, data=data)
+    blob = pd.Series(response.json())
+
+    if verbose and response.status_code == 201:    
+        print(f'File "{filename}" uploaded as blob "{blob.filename}" ({blob.id})')
+    
+    if workspace is not None:
+        assign_blobs(self, workspace, ids=blob.id, verbose=verbose)
+
+    return blob.handle
+    
+def get_blobs(self,
+              filename: Optional[str] = None,
+              parse_dates: bool = True) -> pd.DataFrame:
+    """
+    Retrieves the metadata for blobs
+    
+    Parameters
+    ----------
+    filename : str, optional
+        The name of the file to limit the search by.
+    parse_dates : bool, optional
+        If True (default) then date fields will automatically be parsed into
+        pandas.Timestamp objects.  If False they will be left as str values.
+
+    Returns
+    -------
+    pandas.DataFrame
+        The metadata for all matching blobs.
+    """
+    
+    # Set params
+    params = {}
+    if filename is not None:
+        params['filename'] = filename
+    
+    # Send response
+    rest_url = '/rest/blob/'
+    response = self.get(rest_url, params=params)
+    
+    blobs = pd.DataFrame(response.json())
+    if len(blobs) == 0:
+        blobs = pd.DataFrame(columns=blob_keys)
+
+    if parse_dates and len(blobs) > 0:
+        blobs.upload_date = blobs.apply(date_parser, args=['upload_date'], axis=1)
+
+    return blobs
+
+def get_blob(self,
+             id: Optional[str] = None,
+             filename: Optional[str] = None,
+             parse_dates: bool = True) -> pd.Series:
+    """
+    Retrieves the metadata for a single blob.  The blob can be uniquely
+    identified using its id or filename.
+    
+    Parameters
+    ----------
+    id : str, optional
+        The unique ID associated with the blob.
+    filename : str, optional
+        The name of the file to limit the search by.
+    parse_dates : bool, optional
+        If True (default) then date fields will automatically be parsed into
+        pandas.Timestamp objects.  If False they will be left as str values.
+
+    Returns
+    -------
+    pandas.Series
+        The metadata for the matching blob.
+
+    Raises
+    ------
+    ValueError
+        If both id and filename are given, or if exactly one matching blob not
+        found.
+    """
+    if id is None:
+        blobs = self.get_blobs(filename=filename, parse_dates=parse_dates)
+        
+        if len(blobs) == 1:
+            return blobs.iloc[0]
+        elif len(blobs) == 0:
+            raise ValueError('No matching blobs found')
+        else:
+            raise ValueError('Multiple matching blobs found')
+    else:
+        if filename is not None:
+            raise ValueError('id and filename cannot both be given')
+        rest_url = f'/rest/blob/{id}'
+        response = self.get(rest_url)
+        blob = pd.Series(response.json())
+
+        if parse_dates:
+            blob.upload_date = date_parser(blob, 'upload_date')
+
+        return blob
+
+def assign_blobs(self, workspace: Union[str, pd.Series],
+                 blobs: Union[pd.Series, pd.DataFrame, None] = None,
+                 ids: Union[str, list, None] = None,
+                 filename: Optional[str] = None,
+                 verbose: bool = False):
+    """
+    Assigns one or more blobs to a workspace.
+
+    Parameters
+    ----------
+    workspace : str or pandas.Series
+        The workspace or workspace title to assign the blobs to.
+    blobs : pandas.Series or pandas.DataFrame, optional
+        Pre-selected blobs to assign to the workspace.  Cannot be given with
+        ids or filename.
+    ids : str or list, optional
+        The ID(s) of the blobs to assign to the workspace.  Selecting blobs
+        using ids has the least overhead. Cannot be given with blobs or
+        filename.
+    filename : str, optional
+        The name of the blob file to assign to the workspace.  Cannot be given
+        with blobs or ids.
+    verbose : bool, optional
+        Setting this to True will print extra status messages.  Default value
+        is False.
+    """
+    # Get workspace id
+    if isinstance(workspace, str):
+        workspace = self.get_workspace(workspace)
+    workspace_id = workspace.id
+    
+    # Get blobs from filename
+    if filename is not None:
+        if blobs is not None or ids is not None:
+            raise ValueError('filename cannot be given with blobs or ids')
+        blobs = get_blobs(self, filename=filename)
+
+    # Get ids from blobs
+    if blobs is not None:
+        if ids is not None:
+            raise ValueError('blobs and ids cannot both be given')
+        if isinstance(blobs, pd.Series):
+            ids = [blobs.id]
+        elif isinstance(blobs, pd.DataFrame):
+            ids = blobs.id.tolist()
+        else:
+            raise TypeError('invalid blobs type')
+    
+    if ids is None:
+        raise ValueError('No blobs specified to assign to the workspace')
+
+    # Assign blobs to the workspace
+    for blob_id in aslist(ids):
+        rest_url = f'/rest/blob/{blob_id}/assign/{workspace_id}'
+        response = self.patch(rest_url)
+
+        if verbose and response.status_code == 200:
+            print(f'blob {blob_id} assigned to workspace {workspace_id}')
+
+def get_blob_contents(self, blob: Optional[pd.Series] = None, 
+                      id: Optional[str] = None,
+                      filename: Optional[str] = None) -> bytes:
+    """
+    Retrieves the contents for a single blob.  The blob can be uniquely
+    identified by passing the blob metadata, or by using its id or filename.
+    
+    Parameters
+    ----------
+    blob : pandas.Series, optional
+        The blob metadata for a blob.
+    id : str, optional
+        The unique ID associated with the blob.
+    filename : str, optional
+        The name of the file to limit the search by.
+    
+    Returns
+    -------
+    bytes
+        The blob file contents.
+
+    Raises
+    ------
+    ValueError
+        If more than one argument given, or if filename does not uniquely
+        identify a blob.
+    """
+
+    if blob is None:
+        blob = self.get_blob(id=id, filename=filename)
+    elif id is not None:
+        raise ValueError('blob and id cannot both be given')
+    elif filename is not None:
+        raise ValueError('blob and filename cannot both be given')
+    
+    rest_url = f'/rest/blob/download/{blob.id}'
+    response = self.get(rest_url)
+    return response.content
+        
+def download_blob(self, blob: Optional[pd.Series] = None,
+                  id: Optional[str] = None,
+                  filename: Optional[str] = None,
+                  savedir: Union[str, Path] = '.') -> bytes:
+    """
+    Retrieves the contents for a single blob and saves it using the stored file
+    name.  The blob can be uniquely identified by passing the blob metadata, or
+    by using its id or filename.
+    
+    Parameters
+    ----------
+    blob : pandas.Series, optional 
+        The blob metadata for a blob.
+    id : str, optional
+        The unique ID associated with the blob.
+    filename : str, optional
+        The name of the file to limit the search by.
+    savedir : str or Path, optional
+        The directory to save the file to.  Default value uses the current
+        working directory.
+    
+    Returns
+    -------
+    bytes
+        The blob file contents.
+
+    Raises
+    ------
+    ValueError
+        If more than one argument given, or if filename does not uniquely
+        identify a blob.
+    """
+    if blob is None:
+        blob = self.get_blob(id=id, filename=filename)
+    elif id is not None:
+        raise ValueError('blob and id cannot both be given')
+    elif filename is not None:
+        raise ValueError('blob and filename cannot both be given')
+        
+    savepath = Path(savedir, blob.filename)
+    with open(savepath, 'wb') as f:
+        f.write(self.get_blob_contents(blob=blob))
+
+def delete_blob(self, blob: Optional[pd.Series] = None,
+                id: Optional[str] = None,
+                filename: Optional[str] = None,
+                verbose: bool = False):
+    """
+    Deletes a single blob from the curator.  The blob can be uniquely
+    identified by passing the blob metadata, or by using its id or filename.
+    
+    Parameters
+    ----------
+    blob : pandas.Series, optional
+        The blob metadata for a blob.
+    id : str, optional
+        The unique ID associated with the blob.
+    filename : str, optional
+        The name of the file to limit the search by.
+    verbose : bool, optional
+        Setting this to True will print extra status messages.  Default value
+        is False.
+    
+    Raises
+    ------
+    ValueError
+        If more than one argument given, or if filename does not uniquely
+        identify a blob.
+    """
+    if blob is None:
+        blob = self.get_blob(id=id, filename=filename)
+    elif id is not None:
+        raise ValueError('blob and id cannot both be given')
+    elif filename is not None:
+        raise ValueError('blob and filename cannot both be given')
+        
+    rest_url = f'/rest/blob/{blob.id}'
+    response = self.delete(rest_url)
+    
+    if verbose and response.status_code == 204:
+        print(f'Successfully deleted blob "{blob.filename}" ({blob.id})')
```

### Comparing `cdcs-0.2.2/cdcs/CDCS/_query.py` & `cdcs-0.2.3/cdcs/CDCS/_query.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,380 +1,382 @@
-# coding: utf-8
-
-# Standard library imports
-from typing import Optional, Union
-from tqdm import tqdm
-
-# Standard library imports
-import json
-
-# https://pandas.pydata.org/
-import pandas as pd
-
-# Local imports
-from .. import aslist, date_parser
-
-query_keys = ['id', 'template', 'workspace', 'user_id', 'title', 'xml_content',
-              'creation_date', 'last_modification_date', 'last_change_date',
-              'template_title']
-
-def query(self,
-          template: Union[list, str, pd.Series, pd.DataFrame, None] = None,
-          title: Optional[str] = None,
-          keyword: Union[str, list, None] = None,
-          mongoquery: Union[str, dict, None] = None,
-          page: Optional[int] = None,
-          parse_dates: bool = True,
-          progress_bar: bool = True) -> pd.DataFrame:
-    """
-    Search all published local data records using either keyword or mongo-style
-    queries. Note: specifying no parameters will return all records in the
-    database!
-
-    Parameters
-    ----------
-    template : list, str, pandas.Series or pandas.DataFrame, optional
-        One or more templates or template titles to limit the search by.
-    title : str, optional
-        Record title to limit the search by.
-    keyword : str or list, optional
-        Keyword(s) to use for a string-based search of record content.  Only
-        records containing all keywords will be returned. keyword and
-        mongoquery cannot both be given.
-    mongoquery : str or dict, optional
-        Mongodb find query to use in limiting searches by record element
-        fields.  Note: only record parsing is supported, not field projection.
-        keyword and mongoquery cannot both be given.
-    page : int or None, optional
-        If an int, then will return results only for that page of 10 records.
-        If None (default), then results for all pages will be compiled and
-        returned.
-    parse_dates : bool, optional
-        If True (default) then date fields will automatically be parsed into
-        pandas.Timestamp objects.  If False they will be left as str values.
-    progress_bar : bool, optional
-        If True (default) a progress bar will be displayed for multi-page
-        query results.
-    Returns
-    -------
-    pandas.DataFrame
-        All records matching the search request.
-    
-    Raises
-    ------
-    ValueError
-        If query and keyword are both given.
-    """  
-    # Set data based on arguments
-    data = {'all': 'true'} 
-    data = {}
-    
-    # Manage query field and rest_url
-    if keyword is not None:
-        rest_url = '/rest/data/query/keyword/'
-        if mongoquery is not None:
-            raise ValueError('keyword and mongoquery cannot both be given')
-        data['query'] = keyword
-        
-    elif mongoquery is not None:
-        rest_url = '/rest/data/query/'
-        if not isinstance(mongoquery, str):
-            data['query'] = json.dumps(mongoquery)
-        else:
-            data['query'] = mongoquery
-    else:
-        rest_url = '/rest/data/query/'
-        data['query'] = '{}'
-    
-    # Manage template 
-    if template is not None:
-        data['templates'] = []
-        
-        # Handle DataFrames
-        if isinstance(template, pd.DataFrame):
-            templates = template
-            for template_id in template.id.values:
-                data['templates'].append({"id":template_id})
-        else:
-            for t in aslist(template):
-                templates = []
-                if not isinstance(t, pd.Series):
-                    t = self.get_template(title=t)
-                t_id = t.id
-                if self.cdcsversion[0] > 2:
-                    t_id = int(t_id)
-                data['templates'].append({"id":t_id})
-                templates.append(t)
-            templates = pd.DataFrame(templates)
-                    
-        data['templates'] = json.dumps(data['templates'])
-    else:
-        templates = self.get_templates()
-
-    # Manage title
-    if title is not None:
-        data['title'] = title
-
-    # Get results from all pages
-    if page is None:
-
-        # Get response
-        response = self.post(rest_url, data=data)
-        response_json = response.json()
-        records = response_json['results']
-
-        if len(records) < response_json['count']:
-            
-            if progress_bar:
-                pbar = tqdm(total=response_json['count'], initial=len(records))
-            
-            # Repeat post until all content received
-            params = {'page':2}
-            while response_json['next'] is not None:
-                response = self.post(rest_url, params=params, data=data)
-                response_json = response.json()
-                newrecords = response_json['results']
-                records.extend(newrecords)
-                params['page'] += 1
-
-                if progress_bar:
-                    pbar.update(len(newrecords))
-            
-            if progress_bar:
-                pbar.close()
-
-            assert len(records) == response_json['count']
-        
-        records = pd.DataFrame(records)
-
-    else:
-        params = {'page':page}
-        response = self.post(rest_url, params=params, data=data)
-        response_json = response.json()
-        records = pd.DataFrame(response_json['results'])
-
-    if len(records) == 0:
-        records = pd.DataFrame(columns=query_keys)
-
-    # Set template titles
-    def set_template_titles(series, templates):
-        return templates[templates.id == series.template].iloc[0].title
-    if len(records) > 0:
-        records['template_title'] = records.apply(set_template_titles, args=[templates], axis=1)
-
-    # Parse date fields
-    if parse_dates and len(records) > 0:
-        for key in ['creation_date', 'last_modification_date', 'last_change_date']:
-            records[key] = records.apply(date_parser, args=[key], axis=1)
-    
-    return records
-
-def query_count(self,
-                template: Union[list, str, pd.Series, pd.DataFrame, None] = None,
-                title: Optional[str] = None,
-                keyword: Union[str, list, None] = None,
-                mongoquery: Union[str, dict, None] = None,
-                ) -> pd.DataFrame:
-    """
-    Search all published local data records using either keyword or mongo-style
-    queries and return only the total count of matching records.
-
-    Parameters
-    ----------
-    template : list, str, pandas.Series or pandas.DataFrame, optional
-        One or more templates or template titles to limit the search by.
-    title : str, optional
-        Record title to limit the search by.
-    keyword : str or list, optional
-        Keyword(s) to use for a string-based search of record content.  Only
-        records containing all keywords will be returned. keyword and
-        mongoquery cannot both be given.
-    mongoquery : str or dict, optional
-        Mongodb find query to use in limiting searches by record element
-        fields.  Note: only record parsing is supported, not field projection.
-        keyword and mongoquery cannot both be given.
-
-    Returns
-    -------
-    int
-        The number of records matching the search request.
-    
-    Raises
-    ------
-    ValueError
-        If query and keyword are both given.
-    """
-    # Set data based on arguments
-    data = {'all': 'true'} 
-    data = {}
-    
-    # Manage query field and rest_url
-    if keyword is not None:
-        rest_url = '/rest/data/query/keyword/'
-        if mongoquery is not None:
-            raise ValueError('keyword and mongoquery cannot both be given')
-        data['query'] = keyword
-        
-    elif mongoquery is not None:
-        rest_url = '/rest/data/query/'
-        if not isinstance(mongoquery, str):
-            data['query'] = json.dumps(mongoquery)
-        else:
-            data['query'] = mongoquery
-    else:
-        rest_url = '/rest/data/query/'
-        data['query'] = '{}'
-    
-    # Manage template 
-    if template is not None:
-        data['templates'] = []
-        
-        # Handle DataFrames
-        if isinstance(template, pd.DataFrame):
-            templates = template
-            for template_id in template.id.values:
-                data['templates'].append({"id":template_id})
-        else:
-            for t in aslist(template):
-                templates = []
-                if not isinstance(t, pd.Series):
-                    t = self.get_template(title=t)
-                
-                data['templates'].append({"id":t.id})
-                templates.append(t)
-            templates = pd.DataFrame(templates)    
-                    
-        data['templates'] = json.dumps(data['templates'])
-    else:
-        templates = self.get_templates()
-
-    # Manage title
-    if title is not None:
-        data['title'] = title
-
-    # Get response
-    response = self.post(rest_url, data=data)
-    response_json = response.json()
-
-    return response_json['count']
-
-def query_ipyparallel(self,
-                      client,
-                      template: Union[list, str, pd.Series, pd.DataFrame, None] = None,
-                      title: Optional[str] = None,
-                      keyword: Union[str, list, None] = None,
-                      mongoquery: Union[str, dict, None] = None
-                      ) -> pd.DataFrame:
-    """
-    Search all published local data records using either keyword or mongo-style
-    queries. Note: specifying no parameters will return all records in the
-    database!
-
-    Parameters
-    ----------
-    client : ipyparallel.client.client.Client
-        An ipyparallel Client object to use for performing multiple
-        parallel web requests.
-    template : list, str, pandas.Series or pandas.DataFrame, optional
-        One or more templates or template titles to limit the search by.
-    title : str, optional
-        Record title to limit the search by.
-    keyword : str or list, optional
-        Keyword(s) to use for a string-based search of record content.  Only
-        records containing all keywords will be returned. keyword and
-        mongoquery cannot both be given.
-    mongoquery : str or dict, optional
-        Mongodb find query to use in limiting searches by record element
-        fields.  Note: only record parsing is supported, not field projection.
-        keyword and mongoquery cannot both be given.
-
-    Returns
-    -------
-    pandas.DataFrame
-        All records matching the search request.
-    
-    Raises
-    ------
-    ValueError
-        If query and keyword are both given.
-    """  
-    raise NotImplementedError('Still need to finish')
-    # Create direct and load balanced views
-    dview = client[:]
-    lview = client.load_balanced_view()
-
-    # Set data based on arguments
-    data = {'all': 'true'} 
-    data = {}
-    
-    # Manage query field and rest_url
-    if keyword is not None:
-        rest_url = '/rest/data/query/keyword/'
-        if mongoquery is not None:
-            raise ValueError('keyword and mongoquery cannot both be given')
-        data['query'] = keyword
-        
-    elif mongoquery is not None:
-        rest_url = '/rest/data/query/'
-        if not isinstance(mongoquery, str):
-            data['query'] = json.dumps(mongoquery)
-        else:
-            data['query'] = mongoquery
-    else:
-        rest_url = '/rest/data/query/'
-        data['query'] = '{}'
-    
-    # Manage template 
-    if template is not None:
-        data['templates'] = []
-        
-        # Handle DataFrames
-        if isinstance(template, pd.DataFrame):
-            templates = template
-            for template_id in template.id.values:
-                data['templates'].append({"id":template_id})
-        else:
-            for t in aslist(template):
-                templates = []
-                if not isinstance(t, pd.Series):
-                    t = self.get_template(title=t)
-                
-                data['templates'].append({"id":t.id})
-                templates.append(t)
-            templates = pd.DataFrame(templates)    
-                    
-        data['templates'] = json.dumps(data['templates'])
-    else:
-        templates = self.get_templates()
-
-    # Manage title
-    if title is not None:
-        data['title'] = title
-
-    # Get response for page 1
-    response = self.post(rest_url, data=data)
-    response_json = response.json()
-    records = response_json['results']
-
-    numpages = response_json['count'] / len(records)
-    pages = list(range(2, numpages+1))
-    if numpages > 1:
-
-        dview.push(dict(self=self, data=data))
-        
-        def post_page(page):
-            params = {'page':page}
-            response = self.post(rest_url, params=params, data=data)
-            response_json = response.json()
-            return response_json['results']
-
-        results = lview.map_async(post_page, pages)
-        assert len(records) == response_json['count']
-        records = pd.DataFrame(records)
-
-    # Set template titles
-    def set_template_titles(series, templates):
-        return templates[templates.id == series.template].iloc[0].title
-    if len(records) > 0:
-        records['template_title'] = records.apply(set_template_titles, args=[templates], axis=1)
-
+# coding: utf-8
+
+# Standard library imports
+from typing import Optional, Union
+from tqdm import tqdm
+
+# Standard library imports
+import json
+
+# https://pandas.pydata.org/
+import pandas as pd
+
+# Local imports
+from .. import aslist, date_parser
+
+query_keys = ['id', 'template', 'workspace', 'user_id', 'title', 'xml_content',
+              'creation_date', 'last_modification_date', 'last_change_date',
+              'template_title']
+
+def query(self,
+          template: Union[list, str, pd.Series, pd.DataFrame, None] = None,
+          title: Optional[str] = None,
+          keyword: Union[str, list, None] = None,
+          mongoquery: Union[str, dict, None] = None,
+          page: Optional[int] = None,
+          parse_dates: bool = True,
+          progress_bar: bool = True) -> pd.DataFrame:
+    """
+    Search all published local data records using either keyword or mongo-style
+    queries. Note: specifying no parameters will return all records in the
+    database!
+
+    Parameters
+    ----------
+    template : list, str, pandas.Series or pandas.DataFrame, optional
+        One or more templates or template titles to limit the search by.
+    title : str, optional
+        Record title to limit the search by.
+    keyword : str or list, optional
+        Keyword(s) to use for a string-based search of record content.  Only
+        records containing all keywords will be returned. keyword and
+        mongoquery cannot both be given.
+    mongoquery : str or dict, optional
+        Mongodb find query to use in limiting searches by record element
+        fields.  Note: only record parsing is supported, not field projection.
+        keyword and mongoquery cannot both be given.
+    page : int or None, optional
+        If an int, then will return results only for that page of 10 records.
+        If None (default), then results for all pages will be compiled and
+        returned.
+    parse_dates : bool, optional
+        If True (default) then date fields will automatically be parsed into
+        pandas.Timestamp objects.  If False they will be left as str values.
+    progress_bar : bool, optional
+        If True (default) a progress bar will be displayed for multi-page
+        query results.
+    Returns
+    -------
+    pandas.DataFrame
+        All records matching the search request.
+    
+    Raises
+    ------
+    ValueError
+        If query and keyword are both given.
+    """  
+    # Set data based on arguments
+    data = {'all': 'true'} 
+    data = {}
+    
+    # Manage query field and rest_url
+    if keyword is not None:
+        rest_url = '/rest/data/query/keyword/'
+        if mongoquery is not None:
+            raise ValueError('keyword and mongoquery cannot both be given')
+        data['query'] = keyword
+        
+    elif mongoquery is not None:
+        rest_url = '/rest/data/query/'
+        if not isinstance(mongoquery, str):
+            data['query'] = json.dumps(mongoquery)
+        else:
+            data['query'] = mongoquery
+    else:
+        rest_url = '/rest/data/query/'
+        data['query'] = '{}'
+    
+    # Manage template 
+    if template is not None:
+        data['templates'] = []
+        
+        # Handle DataFrames
+        if isinstance(template, pd.DataFrame):
+            templates = template
+            for template_id in template.id.values:
+                data['templates'].append({"id":template_id})
+        else:
+            for t in aslist(template):
+                templates = []
+                if not isinstance(t, pd.Series):
+                    t = self.get_template(title=t)
+                t_id = t.id
+                if self.cdcsversion[0] > 2:
+                    t_id = int(t_id)
+                data['templates'].append({"id":t_id})
+                templates.append(t)
+            templates = pd.DataFrame(templates)
+                    
+        data['templates'] = json.dumps(data['templates'])
+    else:
+        templates = self.get_templates()
+
+    # Manage title
+    if title is not None:
+        data['title'] = title
+
+    # Get results from all pages
+    if page is None:
+
+        # Get response
+        response = self.post(rest_url, data=data)
+        response_json = response.json()
+        records = response_json['results']
+
+        if len(records) < response_json['count']:
+            
+            if progress_bar:
+                pbar = tqdm(total=response_json['count'], initial=len(records))
+            
+            # Repeat post until all content received
+            params = {'page':2}
+            while response_json['next'] is not None:
+                response = self.post(rest_url, params=params, data=data)
+                response_json = response.json()
+                newrecords = response_json['results']
+                records.extend(newrecords)
+                params['page'] += 1
+
+                if progress_bar:
+                    pbar.update(len(newrecords))
+            
+            if progress_bar:
+                pbar.close()
+
+            assert len(records) == response_json['count']
+        
+        records = pd.DataFrame(records)
+
+    else:
+        params = {'page':page}
+        response = self.post(rest_url, params=params, data=data)
+        response_json = response.json()
+        records = pd.DataFrame(response_json['results'])
+
+    if len(records) == 0:
+        records = pd.DataFrame(columns=query_keys)
+
+    # Set template titles
+    def set_template_titles(series, templates):
+        return templates[templates.id == series.template].iloc[0].title
+    if len(records) > 0:
+        records['template_title'] = records.apply(set_template_titles, args=[templates], axis=1)
+
+    # Parse date fields
+    if parse_dates and len(records) > 0:
+        for key in ['creation_date', 'last_modification_date', 'last_change_date']:
+            records[key] = records.apply(date_parser, args=[key], axis=1)
+    
+    return records
+
+def query_count(self,
+                template: Union[list, str, pd.Series, pd.DataFrame, None] = None,
+                title: Optional[str] = None,
+                keyword: Union[str, list, None] = None,
+                mongoquery: Union[str, dict, None] = None,
+                ) -> pd.DataFrame:
+    """
+    Search all published local data records using either keyword or mongo-style
+    queries and return only the total count of matching records.
+
+    Parameters
+    ----------
+    template : list, str, pandas.Series or pandas.DataFrame, optional
+        One or more templates or template titles to limit the search by.
+    title : str, optional
+        Record title to limit the search by.
+    keyword : str or list, optional
+        Keyword(s) to use for a string-based search of record content.  Only
+        records containing all keywords will be returned. keyword and
+        mongoquery cannot both be given.
+    mongoquery : str or dict, optional
+        Mongodb find query to use in limiting searches by record element
+        fields.  Note: only record parsing is supported, not field projection.
+        keyword and mongoquery cannot both be given.
+
+    Returns
+    -------
+    int
+        The number of records matching the search request.
+    
+    Raises
+    ------
+    ValueError
+        If query and keyword are both given.
+    """
+    # Set data based on arguments
+    data = {'all': 'true'} 
+    data = {}
+    
+    # Manage query field and rest_url
+    if keyword is not None:
+        rest_url = '/rest/data/query/keyword/'
+        if mongoquery is not None:
+            raise ValueError('keyword and mongoquery cannot both be given')
+        data['query'] = keyword
+        
+    elif mongoquery is not None:
+        rest_url = '/rest/data/query/'
+        if not isinstance(mongoquery, str):
+            data['query'] = json.dumps(mongoquery)
+        else:
+            data['query'] = mongoquery
+    else:
+        rest_url = '/rest/data/query/'
+        data['query'] = '{}'
+    
+    # Manage template 
+    if template is not None:
+        data['templates'] = []
+        
+        # Handle DataFrames
+        if isinstance(template, pd.DataFrame):
+            templates = template
+            for template_id in template.id.values:
+                data['templates'].append({"id":template_id})
+        else:
+            for t in aslist(template):
+                templates = []
+                if not isinstance(t, pd.Series):
+                    t = self.get_template(title=t)
+                t_id = t.id
+                if self.cdcsversion[0] > 2:
+                    t_id = int(t_id)
+                data['templates'].append({"id":t_id})
+                templates.append(t)
+            templates = pd.DataFrame(templates)    
+                    
+        data['templates'] = json.dumps(data['templates'])
+    else:
+        templates = self.get_templates()
+
+    # Manage title
+    if title is not None:
+        data['title'] = title
+
+    # Get response
+    response = self.post(rest_url, data=data)
+    response_json = response.json()
+
+    return response_json['count']
+
+def query_ipyparallel(self,
+                      client,
+                      template: Union[list, str, pd.Series, pd.DataFrame, None] = None,
+                      title: Optional[str] = None,
+                      keyword: Union[str, list, None] = None,
+                      mongoquery: Union[str, dict, None] = None
+                      ) -> pd.DataFrame:
+    """
+    Search all published local data records using either keyword or mongo-style
+    queries. Note: specifying no parameters will return all records in the
+    database!
+
+    Parameters
+    ----------
+    client : ipyparallel.client.client.Client
+        An ipyparallel Client object to use for performing multiple
+        parallel web requests.
+    template : list, str, pandas.Series or pandas.DataFrame, optional
+        One or more templates or template titles to limit the search by.
+    title : str, optional
+        Record title to limit the search by.
+    keyword : str or list, optional
+        Keyword(s) to use for a string-based search of record content.  Only
+        records containing all keywords will be returned. keyword and
+        mongoquery cannot both be given.
+    mongoquery : str or dict, optional
+        Mongodb find query to use in limiting searches by record element
+        fields.  Note: only record parsing is supported, not field projection.
+        keyword and mongoquery cannot both be given.
+
+    Returns
+    -------
+    pandas.DataFrame
+        All records matching the search request.
+    
+    Raises
+    ------
+    ValueError
+        If query and keyword are both given.
+    """  
+    raise NotImplementedError('Still need to finish')
+    # Create direct and load balanced views
+    dview = client[:]
+    lview = client.load_balanced_view()
+
+    # Set data based on arguments
+    data = {'all': 'true'} 
+    data = {}
+    
+    # Manage query field and rest_url
+    if keyword is not None:
+        rest_url = '/rest/data/query/keyword/'
+        if mongoquery is not None:
+            raise ValueError('keyword and mongoquery cannot both be given')
+        data['query'] = keyword
+        
+    elif mongoquery is not None:
+        rest_url = '/rest/data/query/'
+        if not isinstance(mongoquery, str):
+            data['query'] = json.dumps(mongoquery)
+        else:
+            data['query'] = mongoquery
+    else:
+        rest_url = '/rest/data/query/'
+        data['query'] = '{}'
+    
+    # Manage template 
+    if template is not None:
+        data['templates'] = []
+        
+        # Handle DataFrames
+        if isinstance(template, pd.DataFrame):
+            templates = template
+            for template_id in template.id.values:
+                data['templates'].append({"id":template_id})
+        else:
+            for t in aslist(template):
+                templates = []
+                if not isinstance(t, pd.Series):
+                    t = self.get_template(title=t)
+                
+                data['templates'].append({"id":t.id})
+                templates.append(t)
+            templates = pd.DataFrame(templates)    
+                    
+        data['templates'] = json.dumps(data['templates'])
+    else:
+        templates = self.get_templates()
+
+    # Manage title
+    if title is not None:
+        data['title'] = title
+
+    # Get response for page 1
+    response = self.post(rest_url, data=data)
+    response_json = response.json()
+    records = response_json['results']
+
+    numpages = response_json['count'] / len(records)
+    pages = list(range(2, numpages+1))
+    if numpages > 1:
+
+        dview.push(dict(self=self, data=data))
+        
+        def post_page(page):
+            params = {'page':page}
+            response = self.post(rest_url, params=params, data=data)
+            response_json = response.json()
+            return response_json['results']
+
+        results = lview.map_async(post_page, pages)
+        assert len(records) == response_json['count']
+        records = pd.DataFrame(records)
+
+    # Set template titles
+    def set_template_titles(series, templates):
+        return templates[templates.id == series.template].iloc[0].title
+    if len(records) > 0:
+        records['template_title'] = records.apply(set_template_titles, args=[templates], axis=1)
+
     return records
```

### Comparing `cdcs-0.2.2/cdcs/CDCS/_record.py` & `cdcs-0.2.3/cdcs/CDCS/_record.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,631 +1,659 @@
-# coding: utf-8
-
-# Standard library imports
-from pathlib import Path
-from typing import Optional, Union
-
-from tqdm import tqdm
-
-from IPython.display import display, HTML
-
-# https://pandas.pydata.org/
-import pandas as pd
-
-from .. import aslist, date_parser
-
-record_keys = ['id', 'template', 'workspace', 'user_id', 'title', 'xml_content',
-               'creation_date', 'last_modification_date', 'last_change_date']
-
-def get_records(self, template: Union[str, pd.Series, None] = None,
-                title: Optional[str] = None,
-                page: Optional[int] = None,
-                parse_dates: bool = True,
-                progress_bar: bool = True) -> pd.DataFrame:
-    """
-    Retrieves user records.
-
-    Parameters
-    ----------
-    template : str or pandas.Series, optional
-        The template or template title to limit the search by.
-    title : str, optional
-        The data record title to limit the search by.
-    page : int or None, optional
-        If an int, then will return results only for that page of 10 records.
-        If None (default), then results for all pages will be compiled and
-        returned.  Only used for CDCS versions 3.X.X.
-    parse_dates : bool, optional
-        If True (default) then date fields will automatically be parsed into
-        pandas.Timestamp objects.  If False they will be left as str values.
-    progress_bar : bool, optional
-        If True (default) a progress bar will be displayed for multi-page
-        query results. Only used for CDCS versions 3.X.X.
-
-    Returns
-    -------
-    pandas.DataFrame
-        All matching user records.
-    """
-
-    # Use old method for CDCS 2.X.X
-    if self.cdcsversion[0] == 2:
-        return self.get_records_v2(template=template, title=title,
-        parse_dates=parse_dates)
-
-    # Build params
-    params = {}
-
-    # Manage template
-    if template is not None:
-        
-        # Handle template series
-        if isinstance(template, pd.Series):
-            params['template'] = template.id
-            
-        # Handle template titles
-        else:
-            template = self.get_template(title=template)
-            params['template'] = template.id
-            
-    # Manage title
-    if title is not None:
-        params['title'] = title
-
-    rest_url = '/rest/data/'
-
-    # Get results from all pages
-    if page is None:
-        response = self.get(rest_url, params=params)
-        response_json = response.json()
-        records = response_json['results']
-        
-        if len(records) < response_json['count']:
-
-            if progress_bar:
-                pbar = tqdm(total=response_json['count'], initial=len(records))
-        
-            # Repeat post until all content received
-            params['page'] = 2
-            while response_json['next'] is not None:
-                response = self.get(rest_url, params=params)
-                response_json = response.json()
-                newrecords = response_json['results']
-                records.extend(newrecords)
-                params['page'] += 1
-
-                if progress_bar:
-                    pbar.update(len(newrecords))
-            
-            if progress_bar:
-                pbar.close()
-
-            assert len(records) == response_json['count']
-        
-        records = pd.DataFrame(records)
-
-    else:
-        params['page'] = page
-        response = self.get(rest_url, params=params)
-        response_json = response.json()
-        records = pd.DataFrame(response_json['results'])
-        
-    if len(records) == 0:
-        records = pd.DataFrame(columns=record_keys)
-
-    # Parse date fields
-    if parse_dates and len(records) > 0:
-        for key in ['creation_date', 'last_modification_date', 'last_change_date']:
-            records[key] = records.apply(date_parser, args=[key], axis=1)
-    
-    return records
-
-def get_records_v2(self, template: Union[str, pd.Series, None] = None,
-                   title: Optional[str] = None,
-                   parse_dates: bool = True) -> pd.DataFrame:
-    """
-    Retrieves user records for a CDCS version 2.X.X database.
-
-    Parameters
-    ----------
-    template : str or pandas.Series, optional
-        The template or template title to limit the search by.
-    title : str, optional
-        The data record title to limit the search by.
-    parse_dates : bool, optional
-        If True (default) then date fields will automatically be parsed into
-        pandas.Timestamp objects.  If False they will be left as str values.
-    
-    Returns
-    -------
-    pandas.DataFrame
-        All matching user records.
-    """
-    # Build params
-    params = {}
-
-    # Manage template
-    if template is not None:
-        
-        # Handle template series
-        if isinstance(template, pd.Series):
-            params['template'] = template.id
-            
-        # Handle template titles
-        else:
-            template = self.get_template(title=template)
-            params['template'] = template.id
-            
-    # Manage title
-    if title is not None:
-        params['title'] = title
-    
-    # Get response
-    rest_url = '/rest/data/'
-    response = self.get(rest_url, params=params)
-    records = response.json()
-    records = pd.DataFrame(records)
-    if len(records) == 0:
-        records = pd.DataFrame(columns=record_keys)
-    
-    # Parse date fields
-    if parse_dates and len(records) > 0:
-        for key in ['creation_date', 'last_modification_date', 'last_change_date']:
-            records[key] = records.apply(date_parser, args=[key], axis=1)
-    
-    return records
-
-def get_record(self, template: Union[str, pd.Series, None] = None,
-               title: Optional[str] = None,
-               parse_dates: bool = True) -> pd.Series:
-    """
-    Retrieves a single user record.  Given parameters must uniquely
-    identify a record.
-
-    Parameters
-    ----------
-    template : str or pandas.Series, optional
-        The template or template title to limit the search by.
-    title : str, optional
-        The data record title to limit the search by.
-    parse_dates : bool, optional
-        If True (default) then date fields will automatically be parsed into
-        pandas.Timestamp objects.  If False they will be left as str values.
-        
-    Returns
-    -------
-    pandas.Series
-        The matching user record.
-
-    Raises
-    ------
-    ValueError
-        If no or multiple matching records found.
-    """
-
-    records = self.get_records(template=template, title=title,
-                               parse_dates=parse_dates)
-    
-    # Check that number of records is exactly one.
-    if len(records) == 1:
-        return records.iloc[0]
-    elif len(records) == 0:
-        raise ValueError('No matching records found')
-    else:
-        raise ValueError('Multiple matching records found')
-
-def assign_records(self, workspace: Union[str, pd.Series],
-                   records: Union[pd.Series, pd.DataFrame, None] = None,
-                   ids: Union[str, list, None] = None,
-                   template: Union[str, pd.Series, None] = None,
-                   title: Optional[str] = None,
-                   verbose: bool = False):
-    """
-    Assigns one or more records to a workspace.
-
-    Parameters
-    ----------
-    workspace : str or pandas.Series
-        The workspace or workspace title to assign the records to.
-    records : pandas.Series or pandas.DataFrame, optional
-        Pre-selected records to assign to the workspace.  Cannot be given with
-        ids, template, or title.
-    ids : str or list, optional
-        The ID(s) of the records to assign to the workspace.  Selecting records
-        using ids has the least overhead. Cannot be given with records,
-        template, or title.
-    template : str or pandas.Series, optional
-        The template or template title of records to assign to the workspace.
-        Cannot be given with records or ids.
-    title : str, optional
-        The title of a record to assign to the workspace. Cannot be given with
-        records or ids.
-    verbose : bool, optional
-        Setting this to True will print extra status messages.  Default value
-        is False.
-    """
-    # Get workspace id
-    if isinstance(workspace, str):
-        workspace = self.get_workspace(workspace)
-    workspace_id = workspace.id
-    
-    # Get records from template and/or title
-    if template is not None or title is not None:
-        if records is not None or ids is not None:
-            raise ValueError('template/title cannot be given with records or ids')
-        records = get_records(self, template=template, title=title)
-
-    # Get ids from records
-    if records is not None:
-        if ids is not None:
-            raise ValueError('records and ids cannot both be given')
-        if isinstance(records, pd.Series):
-            ids = [records.id]
-        elif isinstance(records, pd.DataFrame):
-            ids = records.id.tolist()
-        else:
-            raise TypeError('invalid records type')
-    
-    if ids is None:
-        raise ValueError('No records specified to assign to the workspace')
-
-    # Assign records to the workspace
-    for record_id in aslist(ids):
-        rest_url = f'/rest/data/{record_id}/assign/{workspace_id}'
-        response = self.patch(rest_url)
-
-        if verbose and response.status_code == 200:
-            print(f'record {record_id} assigned to workspace {workspace_id}')
-
-def upload_record(self, template: Union[str, pd.Series],
-                  filename: Optional[str] = None,
-                  content: Union[str, bytes, None] = None,
-                  title: Optional[str] = None,
-                  workspace: Union[str, pd.Series] = None,
-                  duplicatecheck: bool = True,
-                  verbose: bool = False):
-    """
-    Adds a data record to the curator
-
-    Parameters
-    ----------
-    template : str or pandas.Series
-        The template or template title to associate with the record.
-    filename : str, optional
-        Name of an XML file whose contents are to be uploaded.  Either filename
-        or content required.
-    content : str or bytes, optional
-        String content to upload. Either filename or content required.
-    title : str, optional
-        Title to save the record as.  Optional if filename is given (title will
-        be taken as filename without ext).
-    workspace : str or pandas.Series, optional
-        If given, the record will be assigned to this workspace after
-        successfully being uploaded.
-    duplicatecheck : bool, optional
-        If True (default), then a ValueError will be raised if a record already
-        exists in the database with the same template and title.  If False, no
-        check is performed possibly allowing for multiple records with the same
-        title to exist in the database.
-    verbose : bool, optional
-        Setting this to True will print extra status messages.  Default value
-        is False.
-
-    Raises
-    ------
-    ValueError
-        If an improper or incomplete combination of filename, content, and
-        title parameters are given, or if duplicatecheck=True and a record
-        with the same title and template exist.
-    TypeError
-        If content is not str or bytes.
-    """
-
-    # Fetch template by title if needed
-    if isinstance(template, str):
-        template = self.get_template(title=template)
-    
-    # Load content from file
-    if filename is not None:
-        if content is not None:
-            raise ValueError('filename and content cannot both be given')
-        
-        with open(filename, 'rb') as xmlfile:
-            content = xmlfile.read()
-            
-        if title is None:
-            title = Path(filename).stem
-    
-    elif content is not None:
-        if title is None:
-            raise ValueError('title must be given with content')
-        
-        # Encode str as bytes if needed
-        if isinstance(content, str):
-            try:
-                e = content.index('?>')
-            except:
-                encoding = 'UTF-8'
-            else:
-                try:
-                    s = content[:e].index('encoding') + 8
-                except:
-                    encoding = 'UTF-8'
-                else:
-                    s = content[s:e].index('"')+s+1
-                    e = content[s:e].index('"') + s
-                    encoding = content[s:e]
-            content = content.encode(encoding)
-        
-        elif not isinstance(content, bytes):
-            raise TypeError('content must be str or bytes')
-        
-    else:
-        raise ValueError('filename or content must be given')
-    
-    # Check if matching record already exists
-    if duplicatecheck is True:
-        matches = self.query(template=template, title=title)
-        if len(matches) > 0:
-            raise ValueError('Record with matching title and template found!')
-    
-    # Set data dict
-    data = {
-        'title': title, 
-        'template': template.id, 
-        'xml_content': content
-    }
-    
-    rest_url = '/rest/data/'
-    response = self.post(rest_url, data=data)
-    
-    if verbose and response.status_code == 201:
-        record_id = response.json()['id']
-        print(f'record {title} ({record_id}) successfully uploaded.')
-
-    if workspace is not None:
-        assign_records(self, workspace=workspace, ids=[response.json()['id']],
-                       verbose=verbose)
-
-def update_record(self, record: Optional[pd.Series] = None,
-                  template: Union[str, pd.Series, None] = None,
-                  title: Optional[str] = None,
-                  filename: Union[str, Path, None] = None,
-                  content: Union[str, bytes, None] = None,
-                  workspace: Union[str, pd.Series, None] = None,
-                  verbose: bool = False):
-    """
-    Updates the content for a single data record in the curator.
-
-    Parameters
-    ----------
-    record : pandas.Series, optional
-        A previously identified record to delete.  As this uniquely defines a
-        record, the template and title parameters are ignored if given.
-    template : str or pandas.Series, optional
-        The template or template title associated with the record.  template +
-        title values must uniquely identify one record.
-    title : str, optional
-        Title of the record to delete.  template + title values must uniquely
-        identify one record.
-    filename : str or Path, optional
-        Path to file containing the new record content to upload. Either
-        filename or content required.
-    content : str or bytes, optional
-        New content to upload. Either filename or content required.
-    workspace : str or pandas.Series, optional
-        If given, the record will be assigned to this workspace after
-        successfully being updated.
-    verbose : bool, optional
-        Setting this to True will print extra status messages.  Default value
-        is False.
-    """
-    # Load content from file
-    if filename is not None:
-        if content is not None:
-            raise ValueError('filename and content cannot both be given')
-        
-        with open(filename, 'rb') as xmlfile:
-            content = xmlfile.read()
-            
-        if title is None:
-            title = Path(filename).stem
-    
-    elif content is not None:
-        
-        # Encode str as bytes if needed
-        if isinstance(content, str):
-            try:
-                e = content.index('?>')
-            except:
-                encoding = 'UTF-8'
-            else:
-                try:
-                    s = content[:e].index('encoding') + 8
-                except:
-                    encoding = 'UTF-8'
-                else:
-                    s = content[s:e].index('"')+s+1
-                    e = content[s:e].index('"') + s
-                    encoding = content[s:e]
-            content = content.encode(encoding)
-        
-        elif not isinstance(content, bytes):
-            raise TypeError('content must be str or bytes')
-        
-    else:
-        raise ValueError('filename or content must be given')
-
-    # Get matching record
-    if record is None:
-        record = self.get_record(template=template, title=title)
-    
-    # Set data dict
-    data = {
-        'xml_content': content
-    }
-
-    rest_url = f'/rest/data/{record.id}/'
-    response = self.patch(rest_url, data=data)
-    
-    if verbose and response.status_code == 200:
-        print(f'record {record.title} ({record.id}) has been updated.')
-    
-    if workspace is not None:
-        assign_records(self, workspace=workspace, ids=[record.id],
-                       verbose=verbose)
-
-def delete_record(self, record: Optional[pd.Series] = None,
-                  template: Union[str, pd.Series, None] = None,
-                  title: Optional[str] = None,
-                  verbose: bool = False):
-    """
-    Deletes a single data record from the curator.
-
-    Parameters
-    ----------
-    record : pandas.Series, optional
-        A previously identified record to delete.  As this uniquely defines a
-        record, the other parameters are ignored.
-    template : str or pandas.Series, optional
-        The template or template title associated with the record.  template +
-        title values must uniquely identify one record.
-    title : str, optional
-        Title of the record to delete.  template + title values must uniquely
-        identify one record.
-    verbose : bool, optional
-        Setting this to True will print extra status messages.  Default value
-        is False.
-    """
-    if record is None:
-        record = self.get_record(template=template, title=title)
-    
-    rest_url = f'/rest/data/{record.id}/'
-    response = self.delete(rest_url)
-    
-    if verbose and response.status_code == 204:
-        print(f'record {record.title} ({record.id}) has been deleted.')
-
-def transform_record(self,
-                     record: Optional[pd.Series] = None,
-                     record_template: Optional[str] = None,
-                     record_title: Optional[str] = None,
-                     record_content: Union[str, bytes, None] = None,
-                     record_filename: Union[str, Path, None] = None,
-                     xslt: Optional[pd.Series] = None,
-                     xslt_name: Optional[str] = None,
-                     render_html: bool = False):
-    """
-    Transforms an XML record using an XSLT in the curator.  Note that this
-    transformation is done by the curator and therefore involves at least one
-    web request.  If the XML and XSLT files are local then it is likely more
-    efficient to transform them locally (e.g. use lxml).
-    
-    Parameters
-    ----------
-    record : pandas.Series, optional
-        The record information as retrieved from get_record(s) or query. Cannot
-        be given with any other record parameter.
-    record_template : str, optional
-        The template title for a record to retrieve from the curator to render.
-        The values of record_template and record_name together must uniquely 
-        identify a record.  Cannot be given with record, record_content or
-        record_filename.
-    record_title : str, optional
-        The record title for a record to retrieve from the curator to render.
-        The values of record_template and record_name together must uniquely 
-        identify a record.  Cannot be given with record, record_content or
-        record_filename.
-    record_content : str or bytes, optional
-        Allows for XML content to be directly passed in.  Cannot be given with
-        any other record parameter.
-    record_filename : pathlike-object, optional
-        Allows for XML content to be loaded from a local file. Cannot be given
-        with any other record parameter.
-    xslt : pandas.Series, optional
-        The xslt information as retrieved from get_xslt(s).  Cannot be given
-        with any other xslt parameter.
-    xslt_name : str, optional
-        The name associated with an xslt entry in the database.
-    render_html : bool, optional
-        If True, will use ipython's display options to render the transformed
-        content as HTML.  This can be useful for ipython environments, such as
-        Jupyter.  The default value of False will return the transformed
-        contents as a str.
-
-    Returns
-    -------
-    str
-        The XML record contents as transformed by the XSLT.  Only returned when
-        render_html=False.
-    """
-    
-    # Extract record content from a record series
-    if record is not None:
-        try:
-            assert record_template is None
-            assert record_title is None
-            assert record_content is None
-            assert record_filename is None
-        except AssertionError:
-            raise ValueError('record cannot be given with any other record parameters')
-
-        record_content = record.xml_content
-
-    # Load record content from file
-    elif record_filename is not None:
-        if record_content is not None:
-            raise ValueError('record_filename and record_content cannot both be given')
-        if record_title is not None or record_template is not None:
-            raise ValueError('record_filename cannot be given with record_title or record_template')
-        
-        with open(record_filename, 'rb') as xmlfile:
-            record_content = xmlfile.read()
-    
-    # Convert record_content to str if needed
-    elif record_content is not None:
-        if record_title is not None or record_template is not None:
-            raise ValueError('record_content cannot be given with record_title or record_template')
-        
-        # Encode str as bytes if needed
-        if isinstance(record_content, str):
-            try:
-                e = record_content.index('?>')
-            except:
-                encoding = 'UTF-8'
-            else:
-                try:
-                    s = record_content[:e].index('encoding') + 8
-                except:
-                    encoding = 'UTF-8'
-                else:
-                    s = record_content[s:e].index('"')+s+1
-                    e = record_content[s:e].index('"') + s
-                    encoding = record_content[s:e]
-            record_content = record_content.encode(encoding)
-        
-        elif not isinstance(record_content, bytes):
-            raise TypeError('record_content must be str or bytes')
-
-    # Fetch record from curator
-    else:
-        record = self.get_record(title=record_title, template=record_template)
-        record_content = record.xml_content
-
-    # Extract xslt name from series
-    if xslt is not None:
-        if xslt_name is not None:
-            raise ValueError('xslt and xslt_name cannot both be given')
-    elif xslt_name is None:
-        raise ValueError('xslt or xslt_name must be given')
-
-    data = {}
-    data['xslt_name'] = xslt_name
-    data['xml_content'] = record_content
-
-    rest_url = '/rest/xslt/transform/'
-    response = self.post(rest_url, data=data)
-    
-    if render_html:
-        display(HTML(response.text))
-    else:
+# coding: utf-8
+
+# Standard library imports
+from pathlib import Path
+from typing import Optional, Union
+
+from tqdm import tqdm
+
+from IPython.display import display, HTML
+
+# https://pandas.pydata.org/
+import pandas as pd
+
+from .. import aslist, date_parser
+
+record_keys = ['id', 'template', 'workspace', 'user_id', 'title', 'xml_content',
+               'creation_date', 'last_modification_date', 'last_change_date']
+
+def get_records(self, template: Union[str, pd.Series, None] = None,
+                title: Optional[str] = None,
+                page: Optional[int] = None,
+                parse_dates: bool = True,
+                progress_bar: bool = True) -> pd.DataFrame:
+    """
+    Retrieves user records.
+
+    Parameters
+    ----------
+    template : str or pandas.Series, optional
+        The template or template title to limit the search by.
+    title : str, optional
+        The data record title to limit the search by.
+    page : int or None, optional
+        If an int, then will return results only for that page of 10 records.
+        If None (default), then results for all pages will be compiled and
+        returned.  Only used for CDCS versions 3.X.X.
+    parse_dates : bool, optional
+        If True (default) then date fields will automatically be parsed into
+        pandas.Timestamp objects.  If False they will be left as str values.
+    progress_bar : bool, optional
+        If True (default) a progress bar will be displayed for multi-page
+        query results. Only used for CDCS versions 3.X.X.
+
+    Returns
+    -------
+    pandas.DataFrame
+        All matching user records.
+    """
+
+    # Use old method for CDCS 2.X.X
+    if self.cdcsversion[0] == 2:
+        return self.get_records_v2(template=template, title=title,
+        parse_dates=parse_dates)
+
+    # Build params
+    params = {}
+
+    # Manage template
+    if template is not None:
+        
+        # Handle template series
+        if isinstance(template, pd.Series):
+            params['template'] = template.id
+            
+        # Handle template titles
+        else:
+            template = self.get_template(title=template)
+            params['template'] = template.id
+            
+    # Manage title
+    if title is not None:
+        params['title'] = title
+
+    rest_url = '/rest/data/'
+
+    # Get results from all pages
+    if page is None:
+        response = self.get(rest_url, params=params)
+        response_json = response.json()
+        records = response_json['results']
+        
+        if len(records) < response_json['count']:
+
+            if progress_bar:
+                pbar = tqdm(total=response_json['count'], initial=len(records))
+        
+            # Repeat post until all content received
+            params['page'] = 2
+            while response_json['next'] is not None:
+                response = self.get(rest_url, params=params)
+                response_json = response.json()
+                newrecords = response_json['results']
+                records.extend(newrecords)
+                params['page'] += 1
+
+                if progress_bar:
+                    pbar.update(len(newrecords))
+            
+            if progress_bar:
+                pbar.close()
+
+            assert len(records) == response_json['count']
+        
+        records = pd.DataFrame(records)
+
+    else:
+        params['page'] = page
+        response = self.get(rest_url, params=params)
+        response_json = response.json()
+        records = pd.DataFrame(response_json['results'])
+        
+    if len(records) == 0:
+        records = pd.DataFrame(columns=record_keys)
+
+    # Parse date fields
+    if parse_dates and len(records) > 0:
+        for key in ['creation_date', 'last_modification_date', 'last_change_date']:
+            records[key] = records.apply(date_parser, args=[key], axis=1)
+    
+    return records
+
+def get_records_v2(self, template: Union[str, pd.Series, None] = None,
+                   title: Optional[str] = None,
+                   parse_dates: bool = True) -> pd.DataFrame:
+    """
+    Retrieves user records for a CDCS version 2.X.X database.
+
+    Parameters
+    ----------
+    template : str or pandas.Series, optional
+        The template or template title to limit the search by.
+    title : str, optional
+        The data record title to limit the search by.
+    parse_dates : bool, optional
+        If True (default) then date fields will automatically be parsed into
+        pandas.Timestamp objects.  If False they will be left as str values.
+    
+    Returns
+    -------
+    pandas.DataFrame
+        All matching user records.
+    """
+    # Build params
+    params = {}
+
+    # Manage template
+    if template is not None:
+        
+        # Handle template series
+        if isinstance(template, pd.Series):
+            params['template'] = template.id
+            
+        # Handle template titles
+        else:
+            template = self.get_template(title=template)
+            params['template'] = template.id
+            
+    # Manage title
+    if title is not None:
+        params['title'] = title
+    
+    # Get response
+    rest_url = '/rest/data/'
+    response = self.get(rest_url, params=params)
+    records = response.json()
+    records = pd.DataFrame(records)
+    if len(records) == 0:
+        records = pd.DataFrame(columns=record_keys)
+    
+    # Parse date fields
+    if parse_dates and len(records) > 0:
+        for key in ['creation_date', 'last_modification_date', 'last_change_date']:
+            records[key] = records.apply(date_parser, args=[key], axis=1)
+    
+    return records
+
+def get_record(self, template: Union[str, pd.Series, None] = None,
+               title: Optional[str] = None,
+               parse_dates: bool = True) -> pd.Series:
+    """
+    Retrieves a single user record.  Given parameters must uniquely
+    identify a record.
+
+    Parameters
+    ----------
+    template : str or pandas.Series, optional
+        The template or template title to limit the search by.
+    title : str, optional
+        The data record title to limit the search by.
+    parse_dates : bool, optional
+        If True (default) then date fields will automatically be parsed into
+        pandas.Timestamp objects.  If False they will be left as str values.
+        
+    Returns
+    -------
+    pandas.Series
+        The matching user record.
+
+    Raises
+    ------
+    ValueError
+        If no or multiple matching records found.
+    """
+
+    records = self.get_records(template=template, title=title,
+                               parse_dates=parse_dates)
+    
+    # Check that number of records is exactly one.
+    if len(records) == 1:
+        return records.iloc[0]
+    elif len(records) == 0:
+        raise ValueError('No matching records found')
+    else:
+        raise ValueError('Multiple matching records found')
+
+def assign_records(self, workspace: Union[str, pd.Series],
+                   records: Union[pd.Series, pd.DataFrame, None] = None,
+                   ids: Union[str, list, None] = None,
+                   template: Union[str, pd.Series, None] = None,
+                   title: Optional[str] = None,
+                   auto_set_pid_off: bool = False,
+                   verbose: bool = False):
+    """
+    Assigns one or more records to a workspace.
+
+    Parameters
+    ----------
+    workspace : str or pandas.Series
+        The workspace or workspace title to assign the records to.
+    records : pandas.Series or pandas.DataFrame, optional
+        Pre-selected records to assign to the workspace.  Cannot be given with
+        ids, template, or title.
+    ids : str or list, optional
+        The ID(s) of the records to assign to the workspace.  Selecting records
+        using ids has the least overhead. Cannot be given with records,
+        template, or title.
+    template : str or pandas.Series, optional
+        The template or template title of records to assign to the workspace.
+        Cannot be given with records or ids.
+    title : str, optional
+        The title of a record to assign to the workspace. Cannot be given with
+        records or ids.
+    auto_set_pid_off : bool, optional
+        If True the auto_set PID will automatically be turned off before and
+        turned on after uploading. Not  needed if the record has no PID value
+        or pid_xpath set.  Convenient if a single record with a PID
+        value is being uploaded.  For uploading multiple records with PID values
+        use the auto_set_pid_off context manager around batch uploads, or
+        manually turn the setting on/off with auto_set_pid.
+    verbose : bool, optional
+        Setting this to True will print extra status messages.  Default value
+        is False.
+    """
+    # Get workspace id
+    if isinstance(workspace, str):
+        workspace = self.get_workspace(workspace)
+    workspace_id = workspace.id
+    
+    # Get records from template and/or title
+    if template is not None or title is not None:
+        if records is not None or ids is not None:
+            raise ValueError('template/title cannot be given with records or ids')
+        records = get_records(self, template=template, title=title)
+
+    # Get ids from records
+    if records is not None:
+        if ids is not None:
+            raise ValueError('records and ids cannot both be given')
+        if isinstance(records, pd.Series):
+            ids = [records.id]
+        elif isinstance(records, pd.DataFrame):
+            ids = records.id.tolist()
+        else:
+            raise TypeError('invalid records type')
+    
+    if ids is None:
+        raise ValueError('No records specified to assign to the workspace')
+
+    # Assign records to the workspace
+    with self.auto_set_pid_off(auto_set_pid_off):
+        for record_id in aslist(ids):
+            rest_url = f'/rest/data/{record_id}/assign/{workspace_id}'
+            response = self.patch(rest_url)
+
+            if verbose and response.status_code == 200:
+                print(f'record {record_id} assigned to workspace {workspace_id}')
+
+def upload_record(self, template: Union[str, pd.Series],
+                  filename: Optional[str] = None,
+                  content: Union[str, bytes, None] = None,
+                  title: Optional[str] = None,
+                  workspace: Union[str, pd.Series] = None,
+                  duplicatecheck: bool = True,
+                  auto_set_pid_off: bool = False,
+                  verbose: bool = False):
+    """
+    Adds a data record to the curator
+
+    Parameters
+    ----------
+    template : str or pandas.Series
+        The template or template title to associate with the record.
+    filename : str, optional
+        Name of an XML file whose contents are to be uploaded.  Either filename
+        or content required.
+    content : str or bytes, optional
+        String content to upload. Either filename or content required.
+    title : str, optional
+        Title to save the record as.  Optional if filename is given (title will
+        be taken as filename without ext).
+    workspace : str or pandas.Series, optional
+        If given, the record will be assigned to this workspace after
+        successfully being uploaded.
+    duplicatecheck : bool, optional
+        If True (default), then a ValueError will be raised if a record already
+        exists in the database with the same template and title.  If False, no
+        check is performed possibly allowing for multiple records with the same
+        title to exist in the database.
+    auto_set_pid_off : bool, optional
+        If True the auto_set PID will automatically be turned off before and
+        turned on after uploading. Not  needed if the record has no PID value
+        or pid_xpath set.  Convenient if a single record with a PID
+        value is being uploaded.  For uploading multiple records with PID values
+        use the auto_set_pid_off context manager around batch uploads, or
+        manually turn the setting on/off with auto_set_pid.
+    verbose : bool, optional
+        Setting this to True will print extra status messages.  Default value
+        is False.
+
+    Raises
+    ------
+    ValueError
+        If an improper or incomplete combination of filename, content, and
+        title parameters are given, or if duplicatecheck=True and a record
+        with the same title and template exist.
+    TypeError
+        If content is not str or bytes.
+    """
+
+    # Fetch template by title if needed
+    if isinstance(template, str):
+        template = self.get_template(title=template)
+    
+    # Load content from file
+    if filename is not None:
+        if content is not None:
+            raise ValueError('filename and content cannot both be given')
+        
+        with open(filename, 'rb') as xmlfile:
+            content = xmlfile.read()
+            
+        if title is None:
+            title = Path(filename).stem
+    
+    elif content is not None:
+        if title is None:
+            raise ValueError('title must be given with content')
+        
+        # Encode str as bytes if needed
+        if isinstance(content, str):
+            try:
+                e = content.index('?>')
+            except:
+                encoding = 'UTF-8'
+            else:
+                try:
+                    s = content[:e].index('encoding') + 8
+                except:
+                    encoding = 'UTF-8'
+                else:
+                    s = content[s:e].index('"')+s+1
+                    e = content[s:e].index('"') + s
+                    encoding = content[s:e]
+            content = content.encode(encoding)
+        
+        elif not isinstance(content, bytes):
+            raise TypeError('content must be str or bytes')
+        
+    else:
+        raise ValueError('filename or content must be given')
+    
+    # Check if matching record already exists
+    if duplicatecheck is True:
+        matches = self.query(template=template, title=title)
+        if len(matches) > 0:
+            raise ValueError('Record with matching title and template found!')
+    
+    # Set data dict
+    data = {
+        'title': title, 
+        'template': template.id, 
+        'xml_content': content
+    }
+    
+    rest_url = '/rest/data/'
+
+    with self.auto_set_pid_off(auto_set_pid_off):
+        response = self.post(rest_url, data=data)
+    
+        if verbose and response.status_code == 201:
+            record_id = response.json()['id']
+            print(f'record {title} ({record_id}) successfully uploaded.')
+
+        if workspace is not None:
+            assign_records(self, workspace=workspace, ids=[response.json()['id']],
+                        verbose=verbose)
+
+def update_record(self, record: Optional[pd.Series] = None,
+                  template: Union[str, pd.Series, None] = None,
+                  title: Optional[str] = None,
+                  filename: Union[str, Path, None] = None,
+                  content: Union[str, bytes, None] = None,
+                  workspace: Union[str, pd.Series, None] = None,
+                  auto_set_pid_off: bool = False,
+                  verbose: bool = False):
+    """
+    Updates the content for a single data record in the curator.
+
+    Parameters
+    ----------
+    record : pandas.Series, optional
+        A previously identified record to delete.  As this uniquely defines a
+        record, the template and title parameters are ignored if given.
+    template : str or pandas.Series, optional
+        The template or template title associated with the record.  template +
+        title values must uniquely identify one record.
+    title : str, optional
+        Title of the record to delete.  template + title values must uniquely
+        identify one record.
+    filename : str or Path, optional
+        Path to file containing the new record content to upload. Either
+        filename or content required.
+    content : str or bytes, optional
+        New content to upload. Either filename or content required.
+    workspace : str or pandas.Series, optional
+        If given, the record will be assigned to this workspace after
+        successfully being updated.
+    auto_set_pid_off : bool, optional
+        If True the auto_set PID will automatically be turned off before and
+        turned on after uploading. Not  needed if the record has no PID value
+        or pid_xpath set.  Convenient if a single record with a PID
+        value is being uploaded.  For uploading multiple records with PID values
+        use the auto_set_pid_off context manager around batch uploads, or
+        manually turn the setting on/off with auto_set_pid.
+    verbose : bool, optional
+        Setting this to True will print extra status messages.  Default value
+        is False.
+    """
+    # Load content from file
+    if filename is not None:
+        if content is not None:
+            raise ValueError('filename and content cannot both be given')
+        
+        with open(filename, 'rb') as xmlfile:
+            content = xmlfile.read()
+            
+        if title is None:
+            title = Path(filename).stem
+    
+    elif content is not None:
+        
+        # Encode str as bytes if needed
+        if isinstance(content, str):
+            try:
+                e = content.index('?>')
+            except:
+                encoding = 'UTF-8'
+            else:
+                try:
+                    s = content[:e].index('encoding') + 8
+                except:
+                    encoding = 'UTF-8'
+                else:
+                    s = content[s:e].index('"')+s+1
+                    e = content[s:e].index('"') + s
+                    encoding = content[s:e]
+            content = content.encode(encoding)
+        
+        elif not isinstance(content, bytes):
+            raise TypeError('content must be str or bytes')
+        
+    else:
+        raise ValueError('filename or content must be given')
+
+    # Get matching record
+    if record is None:
+        record = self.get_record(template=template, title=title)
+    
+    # Set data dict
+    data = {
+        'xml_content': content
+    }
+
+    rest_url = f'/rest/data/{record.id}/'
+    with self.auto_set_pid_off(auto_set_pid_off):
+        response = self.patch(rest_url, data=data)
+    
+        if verbose and response.status_code == 200:
+            print(f'record {record.title} ({record.id}) has been updated.')
+        
+        if workspace is not None:
+            assign_records(self, workspace=workspace, ids=[record.id],
+                        verbose=verbose)
+
+def delete_record(self, record: Optional[pd.Series] = None,
+                  template: Union[str, pd.Series, None] = None,
+                  title: Optional[str] = None,
+                  verbose: bool = False):
+    """
+    Deletes a single data record from the curator.
+
+    Parameters
+    ----------
+    record : pandas.Series, optional
+        A previously identified record to delete.  As this uniquely defines a
+        record, the other parameters are ignored.
+    template : str or pandas.Series, optional
+        The template or template title associated with the record.  template +
+        title values must uniquely identify one record.
+    title : str, optional
+        Title of the record to delete.  template + title values must uniquely
+        identify one record.
+    verbose : bool, optional
+        Setting this to True will print extra status messages.  Default value
+        is False.
+    """
+    if record is None:
+        record = self.get_record(template=template, title=title)
+    
+    rest_url = f'/rest/data/{record.id}/'
+    response = self.delete(rest_url)
+    
+    if verbose and response.status_code == 204:
+        print(f'record {record.title} ({record.id}) has been deleted.')
+
+def transform_record(self,
+                     record: Optional[pd.Series] = None,
+                     record_template: Optional[str] = None,
+                     record_title: Optional[str] = None,
+                     record_content: Union[str, bytes, None] = None,
+                     record_filename: Union[str, Path, None] = None,
+                     xslt: Optional[pd.Series] = None,
+                     xslt_name: Optional[str] = None,
+                     render_html: bool = False):
+    """
+    Transforms an XML record using an XSLT in the curator.  Note that this
+    transformation is done by the curator and therefore involves at least one
+    web request.  If the XML and XSLT files are local then it is likely more
+    efficient to transform them locally (e.g. use lxml).
+    
+    Parameters
+    ----------
+    record : pandas.Series, optional
+        The record information as retrieved from get_record(s) or query. Cannot
+        be given with any other record parameter.
+    record_template : str, optional
+        The template title for a record to retrieve from the curator to render.
+        The values of record_template and record_name together must uniquely 
+        identify a record.  Cannot be given with record, record_content or
+        record_filename.
+    record_title : str, optional
+        The record title for a record to retrieve from the curator to render.
+        The values of record_template and record_name together must uniquely 
+        identify a record.  Cannot be given with record, record_content or
+        record_filename.
+    record_content : str or bytes, optional
+        Allows for XML content to be directly passed in.  Cannot be given with
+        any other record parameter.
+    record_filename : pathlike-object, optional
+        Allows for XML content to be loaded from a local file. Cannot be given
+        with any other record parameter.
+    xslt : pandas.Series, optional
+        The xslt information as retrieved from get_xslt(s).  Cannot be given
+        with any other xslt parameter.
+    xslt_name : str, optional
+        The name associated with an xslt entry in the database.
+    render_html : bool, optional
+        If True, will use ipython's display options to render the transformed
+        content as HTML.  This can be useful for ipython environments, such as
+        Jupyter.  The default value of False will return the transformed
+        contents as a str.
+
+    Returns
+    -------
+    str
+        The XML record contents as transformed by the XSLT.  Only returned when
+        render_html=False.
+    """
+    
+    # Extract record content from a record series
+    if record is not None:
+        try:
+            assert record_template is None
+            assert record_title is None
+            assert record_content is None
+            assert record_filename is None
+        except AssertionError:
+            raise ValueError('record cannot be given with any other record parameters')
+
+        record_content = record.xml_content
+
+    # Load record content from file
+    elif record_filename is not None:
+        if record_content is not None:
+            raise ValueError('record_filename and record_content cannot both be given')
+        if record_title is not None or record_template is not None:
+            raise ValueError('record_filename cannot be given with record_title or record_template')
+        
+        with open(record_filename, 'rb') as xmlfile:
+            record_content = xmlfile.read()
+    
+    # Convert record_content to str if needed
+    elif record_content is not None:
+        if record_title is not None or record_template is not None:
+            raise ValueError('record_content cannot be given with record_title or record_template')
+        
+        # Encode str as bytes if needed
+        if isinstance(record_content, str):
+            try:
+                e = record_content.index('?>')
+            except:
+                encoding = 'UTF-8'
+            else:
+                try:
+                    s = record_content[:e].index('encoding') + 8
+                except:
+                    encoding = 'UTF-8'
+                else:
+                    s = record_content[s:e].index('"')+s+1
+                    e = record_content[s:e].index('"') + s
+                    encoding = record_content[s:e]
+            record_content = record_content.encode(encoding)
+        
+        elif not isinstance(record_content, bytes):
+            raise TypeError('record_content must be str or bytes')
+
+    # Fetch record from curator
+    else:
+        record = self.get_record(title=record_title, template=record_template)
+        record_content = record.xml_content
+
+    # Extract xslt name from series
+    if xslt is not None:
+        if xslt_name is not None:
+            raise ValueError('xslt and xslt_name cannot both be given')
+    elif xslt_name is None:
+        raise ValueError('xslt or xslt_name must be given')
+
+    data = {}
+    data['xslt_name'] = xslt_name
+    data['xml_content'] = record_content
+
+    rest_url = '/rest/xslt/transform/'
+    response = self.post(rest_url, data=data)
+    
+    if render_html:
+        display(HTML(response.text))
+    else:
         return response.text
```

### Comparing `cdcs-0.2.2/cdcs/CDCS/_template.py` & `cdcs-0.2.3/cdcs/CDCS/_template.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,700 +1,706 @@
-# coding: utf-8
-
-# Standard library imports
-from pathlib import Path
-from typing import Optional, Union
-
-# https://pandas.pydata.org/
-import pandas as pd
-
-def get_template_managers(self, title: Optional[str] = None,
-                          is_disabled: bool = False,
-                          useronly: bool = False) -> pd.DataFrame:
-    """
-    Get template managers from a curator
-
-    Parameters
-    ----------
-    title : str, optional
-        The template title to limit the search by.
-    is_disabled : bool, optional
-        If True, then disabled templates will be returned.  If False (default),
-        then active templates will be returned.
-    useronly : bool, optional
-        If True, only a user's templates are returned. If False (default),
-        then all global templates are returned.
-
-    Returns
-    -------
-    pandas.DataFrame
-        All template managers.
-
-    Raises
-    ------
-    TypeError
-        If useronly is not bool.
-    """
-    # Set url based on useronly value
-    if useronly is False:
-        rest_url = '/rest/template-version-manager/global/'
-    elif useronly is True:
-        rest_url = '/rest/template-version-manager/user/'
-    else:
-        raise TypeError('useronly must be bool')
-
-    # Set params dict based on arguments
-    params = {}
-    if title is not None:
-        params['title'] = title
-    if is_disabled is True:
-        params['is_disabled'] = is_disabled
-    
-    # Get response
-    response = self.get(rest_url, params=params)
-    template_managers = pd.DataFrame(response.json())
-    
-    return template_managers
-    
-def disable_template_manager(self,
-                             title: Optional[str] = None,
-                             template_manager: Optional[pd.Series] = None,
-                             verbose: bool = False):
-    """
-    Disables a template manager (all versions of a template).
-    
-    Parameters
-    ----------
-    title : str, optional
-        The template title.
-    template_manager : pandas.Series, optional
-        Template manager information for the template.  This can be given instead
-        of title to avoid querying for the template manager.
-    verbose : bool, optional
-        Setting this to True will print extra status messages.  Default value
-        is False.
-    """
-    
-    if title is not None:
-        # Check that title and template_manager are not both given
-        if template_manager is not None:
-            raise ValueError('title and template_manager cannot both be given')
-
-        # Fetch template manager
-        template_manager = self.get_template_managers(title).loc[0]
-
-    # Check that template_manager is given if title is not
-    elif template_manager is None:
-        raise ValueError('title or template_manager must be given')
-        
-    if template_manager.is_disabled:
-        raise ValueError('template manager already disabled')
-
-    manager_id = template_manager["id"]
-    self.patch(f'/rest/template-version-manager/{manager_id}/disable/')
-    
-    if verbose:
-        print(f'template manager with id {manager_id} disabled')
-
-def restore_template_manager(self,
-                             title: Optional[str] = None,
-                             template_manager: Optional[pd.Series] = None,
-                             verbose: bool = False):
-    """
-    Restores a disabled template manager.
-    
-    Parameters
-    ----------
-    title : str, optional
-        The template title.
-    template_manager : pandas.Series, optional
-        Template manager information for the template.  This can be given instead
-        of title to avoid querying for the template manager.
-    verbose : bool, optional
-        Setting this to True will print extra status messages.  Default value
-        is False.
-    """
-    
-    if title is not None:
-        # Check that title and template_manager are not both given
-        if template_manager is not None:
-            raise ValueError('title and template_manager cannot both be given')
-
-        # Fetch template manager
-        template_manager = self.get_template_managers(title).loc[0]
-
-    # Check that template_manager is given if title is not
-    elif template_manager is None:
-        raise ValueError('title or template_manager must be given')
-
-    if not template_manager.is_disabled:
-        raise ValueError('template manager already active')
-
-    manager_id = template_manager["id"]
-    self.patch(f'/rest/template-version-manager/{manager_id}/restore/')
-
-    if verbose:
-        print(f'template manager with id {manager_id} restored')
-
-def get_templates(self, title: Optional[str] = None,
-                  is_disabled: bool = False,
-                  current: bool = True,
-                  useronly: bool = False) -> pd.DataFrame:
-    """
-    Get all templates from a curator.
-
-    Parameters
-    ----------
-    title : str, optional
-        The template title to limit the search by.
-    is_disabled : bool, optional
-        If True, then disabled templates will be returned.  If False (default),
-        then active templates will be returned.
-    current : bool, optional
-        If True (default), only current template versions will be returned.
-    useronly : bool, optional
-        If True, only a user's templates are returned. If False (default),
-        then all global templates are returned.
-
-    Returns
-    -------
-    pandas.DataFrame
-        All current templates.
-    """
-
-    # Get template managers
-    template_managers = self.get_template_managers(title=title,
-                                                   is_disabled=is_disabled,
-                                                   useronly=useronly)      
-    if len(template_managers) > 0:
-        # Get all current templates
-        if current is True:
-            templates = []
-            for current_id in template_managers.current:
-
-                # Set url and get response
-                rest_url = f'/rest/template/{current_id}/'
-                response = self.get(rest_url)
-                templates.append(response.json())
-            templates = pd.DataFrame(templates)
-
-            # Add title to content
-            templates['title'] = template_managers.title
-
-        # Get all templates
-        elif current is False:
-            templates = []
-            for template_manager in template_managers.itertuples():
-                for version_id in template_manager.versions:
-
-                    # Set url and get response
-                    rest_url = f'/rest/template/{version_id}/'
-                    response = self.get(rest_url)
-
-                    # Add title to content
-                    content = response.json()
-                    content['title'] = template_manager.title
-                    templates.append(content)
-
-            templates = pd.DataFrame(templates)
-
-        else:
-            raise TypeError('current must be bool')
-    else:
-        templates = pd.DataFrame([])
-            
-    return templates
-
-def get_template(self, title: Optional[str] = None,
-                 is_disabled: bool = False,
-                 current: bool = True,
-                 useronly: bool = False) -> pd.Series:
-    """
-    Gets a single template from a curator.
-
-    Parameters
-    ----------
-    title : str, optional
-        The template title to limit the search by.
-    is_disabled : bool, optional
-        If True, then disabled templates will be returned.  If False (default),
-        then active templates will be returned.
-    current : bool, optional
-        If True (default), only current template versions will be returned.
-    useronly : bool, optional
-        If True, only a user's templates are returned. If False (default), then
-        all global templates are returned.
-
-    Returns
-    -------
-    pandas.Series
-        The matching template.
-
-    Raises
-    ------
-    ValueError
-        If no template named title found.
-    """
-
-    # Get templates 
-    templates = self.get_templates(title=title, is_disabled=is_disabled,
-                                    current=current, useronly=useronly)
-
-    # Check that number of templates is exactly one.
-    if len(templates) == 1:
-        return templates.iloc[0]
-    elif len(templates) == 0:
-        raise ValueError('No matching template found')
-    else:
-        raise ValueError('Multiple matching templates found')
-
-@property
-def template_titles(self) -> list:
-    """list: All template titles"""
-    return self.get_template_managers().title.tolist()
-
-def upload_template(self,
-                    filename: Optional[str] = None,
-                    content: Union[str, bytes, None] = None,
-                    title: Optional[str] = None,
-                    useronly: bool = False,
-                    verbose: bool = False):
-    """
-    Uploads a new template schema to the curator.  Use update_template if a
-    template already exists with the wanted title.
-
-    Parameters
-    ----------
-    filename : str, optional
-        Name of the XSD schema file to upload for the template.  Optional if title
-        is given (filename will be taken as "title".xsd).
-    content : str or bytes, optional
-        String contents of an XSD schema file to upload for the template.  Optional
-        if filename is given as a full path to the XSD file.
-    title : str, optional
-        Title to save the template as.  Optional if filename is given (title will
-        be taken as filename without ext).
-    useronly : bool, optional
-        If True, the template will be associated only with the user. If False (default),
-        it will be made a global template.
-    verbose : bool, optional
-        Setting this to True will print extra status messages.  Default value
-        is False.
-
-    Raises
-    ------
-    ValueError
-        If an improper or incomplete combination of filename, content, and
-        title parameters are given, or if a template with the same title already exists.
-    TypeError
-        If content is not str or bytes.
-    """
-    
-    # Check if filename has been given
-    if filename is not None:
-        
-        # Load content if needed
-        if content is None:
-            with open(filename, 'rb') as xmlfile:
-                content = xmlfile.read()
-        
-        # Set title if needed
-        if title is None:
-            title = Path(filename).stem
-        
-        # Remove directory path from filename
-        filename = Path(filename).name
-    
-    elif title is not None:
-        filename = title + '.xsd'
-        
-    else:
-        raise ValueError('filename or title must be given')
-        
-    if content is None:
-        raise ValueError('filename or content must be given')
-    
-    if title in self.template_titles:
-        raise ValueError(f'template {title} already exists')
-
-    # Encode str as bytes if needed
-    if isinstance(content, str):
-        try:
-            e = content.index('?>')
-        except:
-            encoding = 'UTF-8'
-        else:
-            try:
-                s = content[:e].index('encoding') + 8
-            except:
-                encoding = 'UTF-8'
-            else:
-                s = content[s:e].index('"')+s+1
-                e = content[s:e].index('"') + s
-                encoding = content[s:e]
-        content = content.encode(encoding)
-
-    elif not isinstance(content, bytes):
-        raise TypeError('content must be str or bytes')
-    
-    # Set data dict
-    data = {
-        'title': title, 
-        'filename': filename, 
-        'content': content
-    }
-    # Set rest url based on useronly
-    if useronly:
-        rest_url = '/rest/template/user/'
-    else:
-        rest_url = '/rest/template/global/'
-
-    # Send request
-    response = self.post(rest_url, data=data)
-    
-    if verbose and response.status_code == 201:
-        template_id = response.json()['id']
-        print(f'template {title} ({template_id}) successfully uploaded.')
-
-def update_template(self,
-                    filename: Optional[str] = None,
-                    content: Union[str, bytes, None] = None,
-                    title: Optional[str] = None,
-                    template_manager: Optional[pd.Series] = None,
-                    #validate: bool = False,
-                    #migrate: bool = False,
-                    set_current: bool = True,
-                    disable_old: bool = False,
-                    verbose: bool = False):
-    """
-    Uploads a new version of a template schema to the curator.
-
-    Parameters
-    ----------
-    filename : str, optional
-        Name of the XSD schema file to upload for the template.  Optional if title
-        is given (filename will be taken as "title".xsd).
-    content : str or bytes, optional
-        String contents of an XSD schema file to upload for the template.  Optional
-        if filename is given as a full path to the XSD file.
-    title : str, optional
-        Title to save the template as.  Optional if filename is given (title will
-        be taken as filename without ext).
-    template_manager : pandas.Series, optional
-        Can be given instead of title if the template_manager info has already been
-        retrieved from the database.
-    validate : bool, optional 
-        NOT IMPLEMENTED YET! If True, all records in the current active version of the template will be validated against
-        the newly uploaded version to determine if migration is possible. Default value is False.
-    migrate : bool, optional
-        NOT IMPLEMENTED YET! If True, will attempt to migrate all records in the current active version to the newly
-        uploaded version.  Default value is False.
-    set_current : bool, optional
-        If True (default), will set the uploaded version of the template to be the current
-        active version.
-    disable_old : bool, optional
-        If True, all active old versions of the template will be disabled. Default value is False.
-    verbose : bool, optional
-        Setting this to True will print extra status messages.  Default value
-        is False.
-
-    Raises
-    ------
-    ValueError
-        If an improper or incomplete combination of filename, content, and
-        title parameters are given, or if a template with the same title already exists.
-    TypeError
-        If content is not str or bytes.
-    """
-    
-    # Check if filename has been given
-    if filename is not None:
-        
-        # Load content if needed
-        if content is None:
-            with open(filename, 'rb') as xmlfile:
-                content = xmlfile.read()
-        
-        # Set title if needed
-        if title is None:
-            if template_manager is None:
-                title = Path(filename).stem
-            else:
-                title = template_manager.title
-        
-        # Remove directory path from filename
-        filename = Path(filename).name
-    
-    elif title is not None:
-        filename = title + '.xsd'
-        
-    else:
-        raise ValueError('filename or title must be given')
-        
-    if content is None:
-        raise ValueError('filename or content must be given')
-    
-    # Get template manager
-    if template_manager is None:
-        template_managers = self.get_template_managers(title=title)
-        if len(template_managers) == 1:
-            template_manager = template_managers.iloc[0]
-        else:
-            raise ValueError(f'template {title} does not exist')
-    
-    # Encode str as bytes if needed
-    if isinstance(content, str):
-        try:
-            e = content.index('?>')
-        except:
-            encoding = 'UTF-8'
-        else:
-            try:
-                s = content[:e].index('encoding') + 8
-            except:
-                encoding = 'UTF-8'
-            else:
-                s = content[s:e].index('"')+s+1
-                e = content[s:e].index('"') + s
-                encoding = content[s:e]
-        content = content.encode(encoding)
-
-    elif not isinstance(content, bytes):
-        raise TypeError('content must be str or bytes')
-    
-    # Set data dict
-    data = {
-        'filename': filename, 
-        'content': content
-    }
-    # Set rest url based on useronly
-    rest_url = f'/rest/template-version-manager/{template_manager["id"]}/version/'
-
-    # Send request
-    response = self.post(rest_url, data=data)
-    
-    template_id = response.json()['id']
-    if verbose and response.status_code == 201:
-        print(f'template {title} ({template_id}) successfully uploaded.')
-    
-    # Set new version as the current template
-    if set_current:
-        self.set_current_template(template_id=template_id, verbose=verbose)
-    
-    # Disable all old versions of the template
-    if disable_old:
-        for version in template_manager.versions:
-            
-            # Skip already disabled versions
-            if version in template_manager.disabled_versions:
-                continue
-                
-            # Skip "current" version if new version was not set as current
-            if version == template_manager.current and not set_current:
-                continue
-            
-            # Disable the old version
-            self.disable_template(template_id=version, verbose=verbose)
-
-def disable_template(self,
-                     title: Optional[str] = None,
-                     version: Optional[int] = None,
-                     template_manager: Optional[pd.Series] = None,
-                     template_id: Optional[str] = None,
-                     verbose: bool = False):
-    """
-    Disables a non-current version of a template.
-    
-    Parameters
-    ----------
-    title : str, optional
-        The template title.
-    version : int, optional
-        The version of the template to disable.  Required unless template_id is
-        given.  Note that version numbers start at 1.
-    template_manager : pandas.Series, optional
-        Template manager information for the template.  This can be given instead
-        of title to avoid querying for the template manager.
-    template_id : str, optional
-        The database id for the template to disable.  If given, then no other
-        parameters are allowed (or needed).
-    verbose : bool, optional
-        Setting this to True will print extra status messages.  Default value
-        is False.
-    """
-    
-    # Check if template_id is given with any other parameters
-    if template_id is not None:
-        if template_manager is not None:
-            raise ValueError('template_id and template_manager cannot both be given')
-        if title is not None:
-            raise ValueError('template_id and title cannot both be given')
-        if version is not None:
-            raise ValueError('template_id and version cannot both be given')
-    
-    else:
-        if title is not None:
-            # Check that title and template_manager are not both given
-            if template_manager is not None:
-                raise ValueError('title and template_manager cannot both be given')
-            
-            # Fetch template manager
-            template_manager = self.get_template_managers(title).loc[0]
-
-        # Check that template_manager is given if title is not
-        elif template_manager is None:
-            raise ValueError('title, template_manager or template_id must be given')
-        
-        # Check value of version
-        if version is None:
-            raise ValueError('version is required with title or template_manager')
-        elif version < 1 or version > len(template_manager.versions):
-            raise IndexError('version number out of range')
-
-        # Get template id
-        template_id = template_manager.versions[version-1]
-
-        if template_id == template_manager.current:
-            raise ValueError('cannot disable the current template version')
-            
-        if template_id in template_manager.disabled_versions:
-            raise ValueError('template version already disabled')
-
-    self.patch(f'/rest/template/version/{template_id}/disable/')
-    
-    if verbose:
-        print(f'template with id {template_id} disabled')
-    
-def restore_template(self,
-                     title: Optional[str] = None,
-                     version: Optional[int] = None,
-                     template_manager: Optional[pd.Series] = None,
-                     template_id: Optional[str] = None,
-                     verbose: bool = False):
-    """
-    Restores a disabled version of a template.
-    
-    Parameters
-    ----------
-    title : str, optional
-        The template title.
-    version : int, optional
-        The version of the template to restore.  Required unless template_id is
-        given.  Note that version numbers start at 1.
-    template_manager : pandas.Series, optional
-        Template manager information for the template.  This can be given instead
-        of title to avoid querying for the template manager.
-    template_id : str, optional
-        The database id for the template to restore.  If given, then no other
-        parameters are allowed (or needed).
-    verbose : bool, optional
-        Setting this to True will print extra status messages.  Default value
-        is False.
-    """
-    
-    # Check if template_id is given with any other parameters
-    if template_id is not None:
-        if template_manager is not None:
-            raise ValueError('template_id and template_manager cannot both be given')
-        if title is not None:
-            raise ValueError('template_id and title cannot both be given')
-        if version is not None:
-            raise ValueError('template_id and version cannot both be given')
-    
-    else:
-        if title is not None:
-            # Check that title and template_manager are not both given
-            if template_manager is not None:
-                raise ValueError('title and template_manager cannot both be given')
-            
-            # Fetch template manager
-            template_manager = self.get_template_managers(title).loc[0]
-
-        # Check that template_manager is given if title is not
-        elif template_manager is None:
-            raise ValueError('title, template_manager or template_id must be given')
-        
-        # Check value of version
-        if version is None:
-            raise ValueError('version is required with title or template_manager')
-        elif version < 1 or version > len(template_manager.versions):
-            raise IndexError('version number out of range')
-
-        # Get template id
-        template_id = template_manager.versions[version-1]
-
-        if template_id not in template_manager.disabled_versions:
-            raise ValueError('template version already active')
-
-    self.patch(f'/rest/template/version/{template_id}/restore/')
-
-    if verbose:
-        print(f'template with id {template_id} restored')
-
-def set_current_template(self,
-                         title: Optional[str] = None,
-                         version: Optional[int] = None,
-                         template_manager: Optional[pd.Series] = None,
-                         template_id: Optional[str] = None,
-                         verbose: bool = False):
-    """
-    Sets an active version of a template as the current version.
-    
-    Parameters
-    ----------
-    title : str, optional
-        The template title.
-    version : int, optional
-        The version of the template to make current.  Required unless template_id is
-        given.  Note that version numbers start at 1.
-    template_manager : pandas.Series, optional
-        Template manager information for the template.  This can be given instead
-        of title to avoid querying for the template manager.
-    template_id : str, optional
-        The database id for the template to set as current.  If given, then no other
-        parameters are allowed (or needed).
-    verbose : bool, optional
-        Setting this to True will print extra status messages.  Default value
-        is False.
-    """
-    
-    # Check if template_id is given with any other parameters
-    if template_id is not None:
-        if template_manager is not None:
-            raise ValueError('template_id and template_manager cannot both be given')
-        if title is not None:
-            raise ValueError('template_id and title cannot both be given')
-        if version is not None:
-            raise ValueError('template_id and version cannot both be given')
-    
-    else:
-        if title is not None:
-            # Check that title and template_manager are not both given
-            if template_manager is not None:
-                raise ValueError('title and template_manager cannot both be given')
-            
-            # Fetch template manager
-            template_manager = self.get_template_managers(title).loc[0]
-
-        # Check that template_manager is given if title is not
-        elif template_manager is None:
-            raise ValueError('title, template_manager or template_id must be given')
-        
-        # Check value of version
-        if version is None:
-            raise ValueError('version is required with title or template_manager')
-        elif version < 1 or version > len(template_manager.versions):
-            raise IndexError('version number out of range')
-
-        # Get template id
-        template_id = template_manager.versions[version-1]
-
-        if template_id == template_manager.current:
-            raise ValueError('template version is already current')
-            
-        if template_id in template_manager.disabled_versions:
-            raise ValueError('template version is disabled')
-
-    self.patch(f'/rest/template/version/{template_id}/current/')
-
-    if verbose:
+# coding: utf-8
+
+# Standard library imports
+from pathlib import Path
+from typing import Optional, Union
+
+# https://pandas.pydata.org/
+import pandas as pd
+
+manager_keys = ['id','versions','current','disabled_versions','title',
+                'user','is_disabled','_cls','creation_date','display_rank']
+template_keys = ['id','user','filename','checksum','content','hash','dependencies','title']
+
+def get_template_managers(self, title: Optional[str] = None,
+                          is_disabled: bool = False,
+                          useronly: bool = False) -> pd.DataFrame:
+    """
+    Get template managers from a curator
+
+    Parameters
+    ----------
+    title : str, optional
+        The template title to limit the search by.
+    is_disabled : bool, optional
+        If True, then disabled templates will be returned.  If False (default),
+        then active templates will be returned.
+    useronly : bool, optional
+        If True, only a user's templates are returned. If False (default),
+        then all global templates are returned.
+
+    Returns
+    -------
+    pandas.DataFrame
+        All template managers.
+
+    Raises
+    ------
+    TypeError
+        If useronly is not bool.
+    """
+    # Set url based on useronly value
+    if useronly is False:
+        rest_url = '/rest/template-version-manager/global/'
+    elif useronly is True:
+        rest_url = '/rest/template-version-manager/user/'
+    else:
+        raise TypeError('useronly must be bool')
+
+    # Set params dict based on arguments
+    params = {}
+    if title is not None:
+        params['title'] = title
+    if is_disabled is True:
+        params['is_disabled'] = is_disabled
+    
+    # Get response
+    response = self.get(rest_url, params=params)
+    template_managers = pd.DataFrame(response.json())
+    if len(template_managers) == 0:
+        template_managers = pd.DataFrame(columns=manager_keys)
+    
+    return template_managers
+    
+def disable_template_manager(self,
+                             title: Optional[str] = None,
+                             template_manager: Optional[pd.Series] = None,
+                             verbose: bool = False):
+    """
+    Disables a template manager (all versions of a template).
+    
+    Parameters
+    ----------
+    title : str, optional
+        The template title.
+    template_manager : pandas.Series, optional
+        Template manager information for the template.  This can be given instead
+        of title to avoid querying for the template manager.
+    verbose : bool, optional
+        Setting this to True will print extra status messages.  Default value
+        is False.
+    """
+    
+    if title is not None:
+        # Check that title and template_manager are not both given
+        if template_manager is not None:
+            raise ValueError('title and template_manager cannot both be given')
+
+        # Fetch template manager
+        template_manager = self.get_template_managers(title).loc[0]
+
+    # Check that template_manager is given if title is not
+    elif template_manager is None:
+        raise ValueError('title or template_manager must be given')
+        
+    if template_manager.is_disabled:
+        raise ValueError('template manager already disabled')
+
+    manager_id = template_manager["id"]
+    self.patch(f'/rest/template-version-manager/{manager_id}/disable/')
+    
+    if verbose:
+        print(f'template manager with id {manager_id} disabled')
+
+def restore_template_manager(self,
+                             title: Optional[str] = None,
+                             template_manager: Optional[pd.Series] = None,
+                             verbose: bool = False):
+    """
+    Restores a disabled template manager.
+    
+    Parameters
+    ----------
+    title : str, optional
+        The template title.
+    template_manager : pandas.Series, optional
+        Template manager information for the template.  This can be given instead
+        of title to avoid querying for the template manager.
+    verbose : bool, optional
+        Setting this to True will print extra status messages.  Default value
+        is False.
+    """
+    
+    if title is not None:
+        # Check that title and template_manager are not both given
+        if template_manager is not None:
+            raise ValueError('title and template_manager cannot both be given')
+
+        # Fetch template manager
+        template_manager = self.get_template_managers(title).loc[0]
+
+    # Check that template_manager is given if title is not
+    elif template_manager is None:
+        raise ValueError('title or template_manager must be given')
+
+    if not template_manager.is_disabled:
+        raise ValueError('template manager already active')
+
+    manager_id = template_manager["id"]
+    self.patch(f'/rest/template-version-manager/{manager_id}/restore/')
+
+    if verbose:
+        print(f'template manager with id {manager_id} restored')
+
+def get_templates(self, title: Optional[str] = None,
+                  is_disabled: bool = False,
+                  current: bool = True,
+                  useronly: bool = False) -> pd.DataFrame:
+    """
+    Get all templates from a curator.
+
+    Parameters
+    ----------
+    title : str, optional
+        The template title to limit the search by.
+    is_disabled : bool, optional
+        If True, then disabled templates will be returned.  If False (default),
+        then active templates will be returned.
+    current : bool, optional
+        If True (default), only current template versions will be returned.
+    useronly : bool, optional
+        If True, only a user's templates are returned. If False (default),
+        then all global templates are returned.
+
+    Returns
+    -------
+    pandas.DataFrame
+        All current templates.
+    """
+
+    # Get template managers
+    template_managers = self.get_template_managers(title=title,
+                                                   is_disabled=is_disabled,
+                                                   useronly=useronly)      
+    if len(template_managers) > 0:
+        # Get all current templates
+        if current is True:
+            templates = []
+            for current_id in template_managers.current:
+
+                # Set url and get response
+                rest_url = f'/rest/template/{current_id}/'
+                response = self.get(rest_url)
+                templates.append(response.json())
+            templates = pd.DataFrame(templates)
+
+            # Add title to content
+            templates['title'] = template_managers.title
+
+        # Get all templates
+        elif current is False:
+            templates = []
+            for template_manager in template_managers.itertuples():
+                for version_id in template_manager.versions:
+
+                    # Set url and get response
+                    rest_url = f'/rest/template/{version_id}/'
+                    response = self.get(rest_url)
+
+                    # Add title to content
+                    content = response.json()
+                    content['title'] = template_manager.title
+                    templates.append(content)
+
+            templates = pd.DataFrame(templates)
+
+        else:
+            raise TypeError('current must be bool')
+    else:
+        templates = pd.DataFrame(columns=template_keys)
+            
+    return templates
+
+def get_template(self, title: Optional[str] = None,
+                 is_disabled: bool = False,
+                 current: bool = True,
+                 useronly: bool = False) -> pd.Series:
+    """
+    Gets a single template from a curator.
+
+    Parameters
+    ----------
+    title : str, optional
+        The template title to limit the search by.
+    is_disabled : bool, optional
+        If True, then disabled templates will be returned.  If False (default),
+        then active templates will be returned.
+    current : bool, optional
+        If True (default), only current template versions will be returned.
+    useronly : bool, optional
+        If True, only a user's templates are returned. If False (default), then
+        all global templates are returned.
+
+    Returns
+    -------
+    pandas.Series
+        The matching template.
+
+    Raises
+    ------
+    ValueError
+        If no template named title found.
+    """
+
+    # Get templates 
+    templates = self.get_templates(title=title, is_disabled=is_disabled,
+                                    current=current, useronly=useronly)
+
+    # Check that number of templates is exactly one.
+    if len(templates) == 1:
+        return templates.iloc[0]
+    elif len(templates) == 0:
+        raise ValueError('No matching template found')
+    else:
+        raise ValueError('Multiple matching templates found')
+
+@property
+def template_titles(self) -> list:
+    """list: All template titles"""
+    return self.get_template_managers().title.tolist()
+
+def upload_template(self,
+                    filename: Optional[str] = None,
+                    content: Union[str, bytes, None] = None,
+                    title: Optional[str] = None,
+                    useronly: bool = False,
+                    verbose: bool = False):
+    """
+    Uploads a new template schema to the curator.  Use update_template if a
+    template already exists with the wanted title.
+
+    Parameters
+    ----------
+    filename : str, optional
+        Name of the XSD schema file to upload for the template.  Optional if title
+        is given (filename will be taken as "title".xsd).
+    content : str or bytes, optional
+        String contents of an XSD schema file to upload for the template.  Optional
+        if filename is given as a full path to the XSD file.
+    title : str, optional
+        Title to save the template as.  Optional if filename is given (title will
+        be taken as filename without ext).
+    useronly : bool, optional
+        If True, the template will be associated only with the user. If False (default),
+        it will be made a global template.
+    verbose : bool, optional
+        Setting this to True will print extra status messages.  Default value
+        is False.
+
+    Raises
+    ------
+    ValueError
+        If an improper or incomplete combination of filename, content, and
+        title parameters are given, or if a template with the same title already exists.
+    TypeError
+        If content is not str or bytes.
+    """
+    
+    # Check if filename has been given
+    if filename is not None:
+        
+        # Load content if needed
+        if content is None:
+            with open(filename, 'rb') as xmlfile:
+                content = xmlfile.read()
+        
+        # Set title if needed
+        if title is None:
+            title = Path(filename).stem
+        
+        # Remove directory path from filename
+        filename = Path(filename).name
+    
+    elif title is not None:
+        filename = title + '.xsd'
+        
+    else:
+        raise ValueError('filename or title must be given')
+        
+    if content is None:
+        raise ValueError('filename or content must be given')
+    
+    if title in self.template_titles:
+        raise ValueError(f'template {title} already exists')
+
+    # Encode str as bytes if needed
+    if isinstance(content, str):
+        try:
+            e = content.index('?>')
+        except:
+            encoding = 'UTF-8'
+        else:
+            try:
+                s = content[:e].index('encoding') + 8
+            except:
+                encoding = 'UTF-8'
+            else:
+                s = content[s:e].index('"')+s+1
+                e = content[s:e].index('"') + s
+                encoding = content[s:e]
+        content = content.encode(encoding)
+
+    elif not isinstance(content, bytes):
+        raise TypeError('content must be str or bytes')
+    
+    # Set data dict
+    data = {
+        'title': title, 
+        'filename': filename, 
+        'content': content
+    }
+    # Set rest url based on useronly
+    if useronly:
+        rest_url = '/rest/template/user/'
+    else:
+        rest_url = '/rest/template/global/'
+
+    # Send request
+    response = self.post(rest_url, data=data)
+    
+    if verbose and response.status_code == 201:
+        template_id = response.json()['id']
+        print(f'template {title} ({template_id}) successfully uploaded.')
+
+def update_template(self,
+                    filename: Optional[str] = None,
+                    content: Union[str, bytes, None] = None,
+                    title: Optional[str] = None,
+                    template_manager: Optional[pd.Series] = None,
+                    #validate: bool = False,
+                    #migrate: bool = False,
+                    set_current: bool = True,
+                    disable_old: bool = False,
+                    verbose: bool = False):
+    """
+    Uploads a new version of a template schema to the curator.
+
+    Parameters
+    ----------
+    filename : str, optional
+        Name of the XSD schema file to upload for the template.  Optional if title
+        is given (filename will be taken as "title".xsd).
+    content : str or bytes, optional
+        String contents of an XSD schema file to upload for the template.  Optional
+        if filename is given as a full path to the XSD file.
+    title : str, optional
+        Title to save the template as.  Optional if filename is given (title will
+        be taken as filename without ext).
+    template_manager : pandas.Series, optional
+        Can be given instead of title if the template_manager info has already been
+        retrieved from the database.
+    validate : bool, optional 
+        NOT IMPLEMENTED YET! If True, all records in the current active version of the template will be validated against
+        the newly uploaded version to determine if migration is possible. Default value is False.
+    migrate : bool, optional
+        NOT IMPLEMENTED YET! If True, will attempt to migrate all records in the current active version to the newly
+        uploaded version.  Default value is False.
+    set_current : bool, optional
+        If True (default), will set the uploaded version of the template to be the current
+        active version.
+    disable_old : bool, optional
+        If True, all active old versions of the template will be disabled. Default value is False.
+    verbose : bool, optional
+        Setting this to True will print extra status messages.  Default value
+        is False.
+
+    Raises
+    ------
+    ValueError
+        If an improper or incomplete combination of filename, content, and
+        title parameters are given, or if a template with the same title already exists.
+    TypeError
+        If content is not str or bytes.
+    """
+    
+    # Check if filename has been given
+    if filename is not None:
+        
+        # Load content if needed
+        if content is None:
+            with open(filename, 'rb') as xmlfile:
+                content = xmlfile.read()
+        
+        # Set title if needed
+        if title is None:
+            if template_manager is None:
+                title = Path(filename).stem
+            else:
+                title = template_manager.title
+        
+        # Remove directory path from filename
+        filename = Path(filename).name
+    
+    elif title is not None:
+        filename = title + '.xsd'
+        
+    else:
+        raise ValueError('filename or title must be given')
+        
+    if content is None:
+        raise ValueError('filename or content must be given')
+    
+    # Get template manager
+    if template_manager is None:
+        template_managers = self.get_template_managers(title=title)
+        if len(template_managers) == 1:
+            template_manager = template_managers.iloc[0]
+        else:
+            raise ValueError(f'template {title} does not exist')
+    
+    # Encode str as bytes if needed
+    if isinstance(content, str):
+        try:
+            e = content.index('?>')
+        except:
+            encoding = 'UTF-8'
+        else:
+            try:
+                s = content[:e].index('encoding') + 8
+            except:
+                encoding = 'UTF-8'
+            else:
+                s = content[s:e].index('"')+s+1
+                e = content[s:e].index('"') + s
+                encoding = content[s:e]
+        content = content.encode(encoding)
+
+    elif not isinstance(content, bytes):
+        raise TypeError('content must be str or bytes')
+    
+    # Set data dict
+    data = {
+        'filename': filename, 
+        'content': content
+    }
+    # Set rest url based on useronly
+    rest_url = f'/rest/template-version-manager/{template_manager["id"]}/version/'
+
+    # Send request
+    response = self.post(rest_url, data=data)
+    
+    template_id = response.json()['id']
+    if verbose and response.status_code == 201:
+        print(f'template {title} ({template_id}) successfully uploaded.')
+    
+    # Set new version as the current template
+    if set_current:
+        self.set_current_template(template_id=template_id, verbose=verbose)
+    
+    # Disable all old versions of the template
+    if disable_old:
+        for version in template_manager.versions:
+            
+            # Skip already disabled versions
+            if version in template_manager.disabled_versions:
+                continue
+                
+            # Skip "current" version if new version was not set as current
+            if version == template_manager.current and not set_current:
+                continue
+            
+            # Disable the old version
+            self.disable_template(template_id=version, verbose=verbose)
+
+def disable_template(self,
+                     title: Optional[str] = None,
+                     version: Optional[int] = None,
+                     template_manager: Optional[pd.Series] = None,
+                     template_id: Optional[str] = None,
+                     verbose: bool = False):
+    """
+    Disables a non-current version of a template.
+    
+    Parameters
+    ----------
+    title : str, optional
+        The template title.
+    version : int, optional
+        The version of the template to disable.  Required unless template_id is
+        given.  Note that version numbers start at 1.
+    template_manager : pandas.Series, optional
+        Template manager information for the template.  This can be given instead
+        of title to avoid querying for the template manager.
+    template_id : str, optional
+        The database id for the template to disable.  If given, then no other
+        parameters are allowed (or needed).
+    verbose : bool, optional
+        Setting this to True will print extra status messages.  Default value
+        is False.
+    """
+    
+    # Check if template_id is given with any other parameters
+    if template_id is not None:
+        if template_manager is not None:
+            raise ValueError('template_id and template_manager cannot both be given')
+        if title is not None:
+            raise ValueError('template_id and title cannot both be given')
+        if version is not None:
+            raise ValueError('template_id and version cannot both be given')
+    
+    else:
+        if title is not None:
+            # Check that title and template_manager are not both given
+            if template_manager is not None:
+                raise ValueError('title and template_manager cannot both be given')
+            
+            # Fetch template manager
+            template_manager = self.get_template_managers(title).loc[0]
+
+        # Check that template_manager is given if title is not
+        elif template_manager is None:
+            raise ValueError('title, template_manager or template_id must be given')
+        
+        # Check value of version
+        if version is None:
+            raise ValueError('version is required with title or template_manager')
+        elif version < 1 or version > len(template_manager.versions):
+            raise IndexError('version number out of range')
+
+        # Get template id
+        template_id = template_manager.versions[version-1]
+
+        if template_id == template_manager.current:
+            raise ValueError('cannot disable the current template version')
+            
+        if template_id in template_manager.disabled_versions:
+            raise ValueError('template version already disabled')
+
+    self.patch(f'/rest/template/version/{template_id}/disable/')
+    
+    if verbose:
+        print(f'template with id {template_id} disabled')
+    
+def restore_template(self,
+                     title: Optional[str] = None,
+                     version: Optional[int] = None,
+                     template_manager: Optional[pd.Series] = None,
+                     template_id: Optional[str] = None,
+                     verbose: bool = False):
+    """
+    Restores a disabled version of a template.
+    
+    Parameters
+    ----------
+    title : str, optional
+        The template title.
+    version : int, optional
+        The version of the template to restore.  Required unless template_id is
+        given.  Note that version numbers start at 1.
+    template_manager : pandas.Series, optional
+        Template manager information for the template.  This can be given instead
+        of title to avoid querying for the template manager.
+    template_id : str, optional
+        The database id for the template to restore.  If given, then no other
+        parameters are allowed (or needed).
+    verbose : bool, optional
+        Setting this to True will print extra status messages.  Default value
+        is False.
+    """
+    
+    # Check if template_id is given with any other parameters
+    if template_id is not None:
+        if template_manager is not None:
+            raise ValueError('template_id and template_manager cannot both be given')
+        if title is not None:
+            raise ValueError('template_id and title cannot both be given')
+        if version is not None:
+            raise ValueError('template_id and version cannot both be given')
+    
+    else:
+        if title is not None:
+            # Check that title and template_manager are not both given
+            if template_manager is not None:
+                raise ValueError('title and template_manager cannot both be given')
+            
+            # Fetch template manager
+            template_manager = self.get_template_managers(title).loc[0]
+
+        # Check that template_manager is given if title is not
+        elif template_manager is None:
+            raise ValueError('title, template_manager or template_id must be given')
+        
+        # Check value of version
+        if version is None:
+            raise ValueError('version is required with title or template_manager')
+        elif version < 1 or version > len(template_manager.versions):
+            raise IndexError('version number out of range')
+
+        # Get template id
+        template_id = template_manager.versions[version-1]
+
+        if template_id not in template_manager.disabled_versions:
+            raise ValueError('template version already active')
+
+    self.patch(f'/rest/template/version/{template_id}/restore/')
+
+    if verbose:
+        print(f'template with id {template_id} restored')
+
+def set_current_template(self,
+                         title: Optional[str] = None,
+                         version: Optional[int] = None,
+                         template_manager: Optional[pd.Series] = None,
+                         template_id: Optional[str] = None,
+                         verbose: bool = False):
+    """
+    Sets an active version of a template as the current version.
+    
+    Parameters
+    ----------
+    title : str, optional
+        The template title.
+    version : int, optional
+        The version of the template to make current.  Required unless template_id is
+        given.  Note that version numbers start at 1.
+    template_manager : pandas.Series, optional
+        Template manager information for the template.  This can be given instead
+        of title to avoid querying for the template manager.
+    template_id : str, optional
+        The database id for the template to set as current.  If given, then no other
+        parameters are allowed (or needed).
+    verbose : bool, optional
+        Setting this to True will print extra status messages.  Default value
+        is False.
+    """
+    
+    # Check if template_id is given with any other parameters
+    if template_id is not None:
+        if template_manager is not None:
+            raise ValueError('template_id and template_manager cannot both be given')
+        if title is not None:
+            raise ValueError('template_id and title cannot both be given')
+        if version is not None:
+            raise ValueError('template_id and version cannot both be given')
+    
+    else:
+        if title is not None:
+            # Check that title and template_manager are not both given
+            if template_manager is not None:
+                raise ValueError('title and template_manager cannot both be given')
+            
+            # Fetch template manager
+            template_manager = self.get_template_managers(title).loc[0]
+
+        # Check that template_manager is given if title is not
+        elif template_manager is None:
+            raise ValueError('title, template_manager or template_id must be given')
+        
+        # Check value of version
+        if version is None:
+            raise ValueError('version is required with title or template_manager')
+        elif version < 1 or version > len(template_manager.versions):
+            raise IndexError('version number out of range')
+
+        # Get template id
+        template_id = template_manager.versions[version-1]
+
+        if template_id == template_manager.current:
+            raise ValueError('template version is already current')
+            
+        if template_id in template_manager.disabled_versions:
+            raise ValueError('template version is disabled')
+
+    self.patch(f'/rest/template/version/{template_id}/current/')
+
+    if verbose:
         print(f'template with id {template_id} set as current version')
```

### Comparing `cdcs-0.2.2/cdcs/CDCS/_workspace.py` & `cdcs-0.2.3/cdcs/CDCS/_workspace.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-# coding: utf-8
-
-# Standard library imports
-from typing import Optional
-
-# https://pandas.pydata.org/
-import pandas as pd
-
-def get_workspaces(self, title:Optional[str]=None) -> pd.DataFrame:
-    """
-    Retrieves information for the existing workspaces.
-
-    Parameters
-    ----------
-    title : str, optional
-        The workspace title to limit the search by.
-    
-    Returns
-    -------
-    pandas.DataFrame
-        The matching workspaces.
-    """
-    rest_url = '/rest/workspace/'
-    response = self.get(rest_url)
-    workspaces = pd.DataFrame(response.json())
-
-    if title is not None:
-        workspaces = workspaces[workspaces.title == title]
-
-    return workspaces
-
-def get_workspace(self, title:Optional[str]=None) -> pd.Series:
-    """
-    Retrieves a single workspace.  Given parameters must uniquely
-    identify a workspace.
-
-    Parameters
-    ----------
-    title : str, optional
-        The workspace title to limit the search by.
-    
-    Returns
-    -------
-    pandas.Series
-        The matching workspace.
-
-    Raises
-    ------
-    ValueError
-        If no or multiple matching workspaces found.
-    """
-
-    workspaces = self.get_workspaces(title=title)
-    
-    # Check that number of workspaces is exactly one.
-    if len(workspaces) == 1:
-        return workspaces.iloc[0]
-    elif len(workspaces) == 0:
-        raise ValueError('No matching workspaces found')
-    else:
-        raise ValueError('Multiple matching workspaces found')
-
-@property
-def global_workspace(self) -> pd.Series:
-    """pandas.Series: The global public workspace"""
+# coding: utf-8
+
+# Standard library imports
+from typing import Optional
+
+# https://pandas.pydata.org/
+import pandas as pd
+
+def get_workspaces(self, title:Optional[str]=None) -> pd.DataFrame:
+    """
+    Retrieves information for the existing workspaces.
+
+    Parameters
+    ----------
+    title : str, optional
+        The workspace title to limit the search by.
+    
+    Returns
+    -------
+    pandas.DataFrame
+        The matching workspaces.
+    """
+    rest_url = '/rest/workspace/'
+    response = self.get(rest_url)
+    workspaces = pd.DataFrame(response.json())
+
+    if title is not None:
+        workspaces = workspaces[workspaces.title == title]
+
+    return workspaces
+
+def get_workspace(self, title:Optional[str]=None) -> pd.Series:
+    """
+    Retrieves a single workspace.  Given parameters must uniquely
+    identify a workspace.
+
+    Parameters
+    ----------
+    title : str, optional
+        The workspace title to limit the search by.
+    
+    Returns
+    -------
+    pandas.Series
+        The matching workspace.
+
+    Raises
+    ------
+    ValueError
+        If no or multiple matching workspaces found.
+    """
+
+    workspaces = self.get_workspaces(title=title)
+    
+    # Check that number of workspaces is exactly one.
+    if len(workspaces) == 1:
+        return workspaces.iloc[0]
+    elif len(workspaces) == 0:
+        raise ValueError('No matching workspaces found')
+    else:
+        raise ValueError('Multiple matching workspaces found')
+
+@property
+def global_workspace(self) -> pd.Series:
+    """pandas.Series: The global public workspace"""
     return self.get_workspace(title='Global Public Workspace')
```

### Comparing `cdcs-0.2.2/cdcs/CDCS/_xslt.py` & `cdcs-0.2.3/cdcs/CDCS/_xslt.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,316 +1,316 @@
-# coding: utf-8
-
-# Standard library imports
-from pathlib import Path
-from re import template
-from typing import Optional, Union
-
-# https://pandas.pydata.org/
-import pandas as pd
-
-xslt_keys = ['id', 'name', 'filename', 'content', '_cls']
-
-def get_xslts(self,
-              name: Optional[str] = None,
-              filename: Optional[str] = None) -> pd.DataFrame:
-    """
-    Retrieves XSLTs.
-
-    Parameters
-    ----------
-    name : str, optional
-        The XSLT name to limit the search by.
-    filename : str, optional
-        The XSLT filename to limit the search by.
-        
-    Returns
-    -------
-    pandas.DataFrame
-        All matching XSLTs.
-    """
-    rest_url = '/rest/xslt/'
-
-    response = self.get(rest_url)
-    xslts = pd.DataFrame(response.json())
-    if len(xslts) == 0:
-        xslts = pd.DataFrame(columns=xslt_keys)
-
-    if name is not None:
-        xslts = xslts[xslts.name == name]
-    if filename is not None:
-        xslts = xslts[xslts.filename == filename]
-    xslts = xslts.reset_index(drop=True)
-
-    return xslts
-
-def get_xslt(self, 
-             name: Optional[str] = None,
-             filename: Optional[str] = None) -> pd.Series:
-    """
-    Retrieves a single XSLT.  Given parameters must uniquely
-    identify an XSLT.
-
-    Parameters
-    ----------
-    name : str, optional
-        The XSLT name to limit the search by.
-    filename : str, optional
-        The XSLT filename to limit the search by.
-
-    Returns
-    -------
-    pandas.Series
-        The matching XSLT.
-
-    Raises
-    ------
-    ValueError
-        If no or multiple matching XSLTs found.
-    """
-
-    xslts = self.get_xslts(name=name, filename=filename)
-    
-    # Check that number of xslts is exactly one.
-    if len(xslts) == 1:
-        return xslts.iloc[0]
-    elif len(xslts) == 0:
-        raise ValueError('No matching xslts found')
-    else:
-        raise ValueError('Multiple matching xslts found')
-
-def upload_xslt(self,
-                name: Optional[str] = None,
-                filename: Optional[str] = None,
-                content: Union[str, bytes, None] = None,
-                verbose: bool = False):
-    """
-    Adds a new XSLT file to the CDCS database.
-
-    Parameters
-    ----------
-    name : str, optional
-        The name to associate with the XSLT file.  Optional if filename is
-        given as name will be taken as filename without its extension.
-    filename : str, optional
-        The filename to associate with the XSLT file.  Optional if name and
-        content are given.  If not given, filename will be set to name + '.xsl'.
-        Will read the file contents if the file exists and content is not given.
-    content : str or bytes, optional
-        XSLT file contents.  Optional if filename is given and points to a file
-        that exists.
-    verbose : bool, optional
-        Setting this to True will print extra status messages.  Default value
-        is False.
-    """
-    # Check if filename has been given
-    if filename is not None:
-        
-        # Load content if needed
-        if content is None:
-            with open(filename, 'rb') as xmlfile:
-                content = xmlfile.read()
-        
-        # Set name if needed
-        if name is None:
-            name = Path(filename).stem
-
-        # Remove directory path from filename
-        filename = Path(filename).name
-
-    elif name is not None:
-        filename = f'{name}.xsl'
-        
-    else:
-        raise ValueError('filename or name must be given')
-        
-    if content is None:
-        raise ValueError('filename or content must be given')
-
-    # Encode str as bytes if needed
-    if isinstance(content, str):
-        try:
-            e = content.index('?>')
-        except:
-            encoding = 'UTF-8'
-        else:
-            try:
-                s = content[:e].index('encoding') + 8
-            except:
-                encoding = 'UTF-8'
-            else:
-                s = content[s:e].index('"')+s+1
-                e = content[s:e].index('"') + s
-                encoding = content[s:e]
-        content = content.encode(encoding)
-
-    elif not isinstance(content, bytes):
-        raise TypeError('content must be str or bytes')
-    
-    # Set data dict
-    data = {
-        'name': name, 
-        'filename': filename, 
-        'content': content
-    }
-
-    # Send request
-    rest_url = '/rest/xslt/'
-    response = self.post(rest_url, data=data)
-
-    if verbose and response.status_code == 201:
-        xslt_id = response.json()['id']
-        print(f'xslt {name} ({xslt_id}) successfully uploaded.')
-
-def update_xslt(self,
-                name: Optional[str] = None,
-                filename: Optional[str] = None,
-                content: Union[str, bytes, None] = None,
-                newname: Optional[str] = None,
-                newfilename: Optional[str] = None,
-                xslt: Optional[pd.Series] = None,
-                xslt_id: Optional[str] = None,
-                verbose: bool = False):
-    """
-    Updates values associated with an XSLT transformation.  The XSLT entry to be
-    updated can be uniquely identified using name and filename, xslt, or xslt_id.
-    
-    Parameters
-    ----------
-    name : str, optional
-        An XSLT name. Will be used to identify the existing xslt entry to update if
-        neither xslt nor xslt_id parameters are given. If either xslt or xslt_id are
-        given, this can be used to assign a new name to the entry.
-    filename : str, optional
-        An xslt filename. Will be used to identify the existing xslt entry to update if
-        neither xslt nor xslt_id parameters are given. If either xslt or xslt_id are
-        given, this can be used to assign a new filename to the entry.
-    content : str, optional
-        New xsl content to assign to the entry.
-    newname : str, optional
-        New name to assign to the entry.
-    newfilename : str, optional
-        New filename to assign to the entry.
-    xslt : pd.Series, optional
-        The XSLT entry information for the entry that is being updated.  
-    xslt_id : str, optional
-        The database id that uniquely identifies the XSLT entry. 
-    verbose : bool, optional
-        Setting this to True will print extra status messages.  Default value
-        is False.
-    """
-    
-    # Get xslt_id from xslt
-    if xslt is not None:
-        if xslt_id is not None:
-            raise ValueError('xslt and xslt_id cannot both be given')
-        xslt_id = xslt['id']
-    
-    # Get new values if xslt_id is known
-    if xslt_id is not None:
-        
-        if name is not None:
-            if newname is not None:
-                raise ValueError('name and newname are aliases when xslt or xslt_id are given')
-            newname = name
-            
-        if filename is not None:
-            if newfilename is not None:
-                raise ValueError('filename and newfilename are aliases when xslt or xslt_id are given')
-            newfilename = filename
-    
-    # Get matching xslt from name, filename values
-    else:
-        xslt = self.get_xslt(name=name, filename=filename)
-        xslt_id = xslt['id']
-           
-    if newfilename is not None:
-        if content is None and Path(newfilename).is_file():
-            with open(newfilename, 'rb') as xmlfile:
-                content = xmlfile.read()
-        newfilename = Path(newfilename).name
-    
-    if isinstance(content, str):
-        try:
-            e = content.index('?>')
-        except:
-            encoding = 'UTF-8'
-        else:
-            try:
-                s = content[:e].index('encoding') + 8
-            except:
-                encoding = 'UTF-8'
-            else:
-                s = content[s:e].index('"')+s+1
-                e = content[s:e].index('"') + s
-                encoding = content[s:e]
-        content = content.encode(encoding)
-    
-    # Set data dict
-    data = {
-        'name': newname, 
-        'filename': newfilename, 
-        'content': content
-    }
-    
-    rest_url = f'/rest/xslt/{xslt_id}/'
-    response = self.patch(rest_url, data=data)
-    
-    if verbose and response.status_code == 201:
-        name = response.json()['name']
-        print(f'xslt {name} ({xslt_id}) successfully updated.')
-
-def delete_xslt(self,
-                name: Optional[str] = None,
-                filename: Optional[str] = None,
-                xslt: Optional[pd.Series] = None,
-                xslt_id: Optional[str] = None,
-                verbose: bool = False):
-    """
-    Deletes an XSLT file from the database.
-
-    Parameters
-    ----------
-    name : str, optional
-        Values for name and filename can be specified to try to uniquely
-        identify the XSLT entry to delete.  Cannot be combined with xslt or
-        xslt_id as they uniquely identify the XSLT on their own.
-    filename : str, optional
-        Values for name and filename can be specified to try to uniquely
-        identify the XSLT entry to delete.  Cannot be combined with xslt or
-        xslt_id as they uniquely identify the XSLT on their own.
-    xslt : pd.Series, optional
-        The xslt entry information for the entry that is to be deleted.  
-        Cannot be combined with name, filename or xslt_id.
-    xslt_id : str, optional
-        The database id that uniquely identifies the xslt entry to delete. 
-        Cannot be combined with name, filename or xslt.
-    verbose : bool, optional
-        Setting this to True will print extra status messages.  Default value
-        is False.
-    """
-
-    # Get xslt_id from xslt
-    if xslt is not None:
-        if xslt_id is not None:
-            raise ValueError('xslt and xslt_id cannot both be given')
-        xslt_id = xslt['id']
-    
-    # Get new values if xslt_id is known
-    if xslt_id is not None:
-        
-        if name is not None:
-            raise ValueError('name cannot be given with xslt or xslt_id')
-                        
-        if filename is not None:
-            raise ValueError('filename cannot be given with xslt or xslt_id')
-            
-    # Get matching xslt from name, filename values
-    else:
-        xslt = self.get_xslt(name=name, filename=filename)
-        xslt_id = xslt['id']
-
-    rest_url = f'/rest/xslt/{xslt_id}/'
-    response = self.delete(rest_url)
-
-    if verbose and response.status_code == 204:
-        print(f'xslt with id ({xslt_id}) has been deleted.')
+# coding: utf-8
+
+# Standard library imports
+from pathlib import Path
+from re import template
+from typing import Optional, Union
+
+# https://pandas.pydata.org/
+import pandas as pd
+
+xslt_keys = ['id', 'name', 'filename', 'content', '_cls']
+
+def get_xslts(self,
+              name: Optional[str] = None,
+              filename: Optional[str] = None) -> pd.DataFrame:
+    """
+    Retrieves XSLTs.
+
+    Parameters
+    ----------
+    name : str, optional
+        The XSLT name to limit the search by.
+    filename : str, optional
+        The XSLT filename to limit the search by.
+        
+    Returns
+    -------
+    pandas.DataFrame
+        All matching XSLTs.
+    """
+    rest_url = '/rest/xslt/'
+
+    response = self.get(rest_url)
+    xslts = pd.DataFrame(response.json())
+    if len(xslts) == 0:
+        xslts = pd.DataFrame(columns=xslt_keys)
+
+    if name is not None:
+        xslts = xslts[xslts.name == name]
+    if filename is not None:
+        xslts = xslts[xslts.filename == filename]
+    xslts = xslts.reset_index(drop=True)
+
+    return xslts
+
+def get_xslt(self, 
+             name: Optional[str] = None,
+             filename: Optional[str] = None) -> pd.Series:
+    """
+    Retrieves a single XSLT.  Given parameters must uniquely
+    identify an XSLT.
+
+    Parameters
+    ----------
+    name : str, optional
+        The XSLT name to limit the search by.
+    filename : str, optional
+        The XSLT filename to limit the search by.
+
+    Returns
+    -------
+    pandas.Series
+        The matching XSLT.
+
+    Raises
+    ------
+    ValueError
+        If no or multiple matching XSLTs found.
+    """
+
+    xslts = self.get_xslts(name=name, filename=filename)
+    
+    # Check that number of xslts is exactly one.
+    if len(xslts) == 1:
+        return xslts.iloc[0]
+    elif len(xslts) == 0:
+        raise ValueError('No matching xslts found')
+    else:
+        raise ValueError('Multiple matching xslts found')
+
+def upload_xslt(self,
+                name: Optional[str] = None,
+                filename: Optional[str] = None,
+                content: Union[str, bytes, None] = None,
+                verbose: bool = False):
+    """
+    Adds a new XSLT file to the CDCS database.
+
+    Parameters
+    ----------
+    name : str, optional
+        The name to associate with the XSLT file.  Optional if filename is
+        given as name will be taken as filename without its extension.
+    filename : str, optional
+        The filename to associate with the XSLT file.  Optional if name and
+        content are given.  If not given, filename will be set to name + '.xsl'.
+        Will read the file contents if the file exists and content is not given.
+    content : str or bytes, optional
+        XSLT file contents.  Optional if filename is given and points to a file
+        that exists.
+    verbose : bool, optional
+        Setting this to True will print extra status messages.  Default value
+        is False.
+    """
+    # Check if filename has been given
+    if filename is not None:
+        
+        # Load content if needed
+        if content is None:
+            with open(filename, 'rb') as xmlfile:
+                content = xmlfile.read()
+        
+        # Set name if needed
+        if name is None:
+            name = Path(filename).stem
+
+        # Remove directory path from filename
+        filename = Path(filename).name
+
+    elif name is not None:
+        filename = f'{name}.xsl'
+        
+    else:
+        raise ValueError('filename or name must be given')
+        
+    if content is None:
+        raise ValueError('filename or content must be given')
+
+    # Encode str as bytes if needed
+    if isinstance(content, str):
+        try:
+            e = content.index('?>')
+        except:
+            encoding = 'UTF-8'
+        else:
+            try:
+                s = content[:e].index('encoding') + 8
+            except:
+                encoding = 'UTF-8'
+            else:
+                s = content[s:e].index('"')+s+1
+                e = content[s:e].index('"') + s
+                encoding = content[s:e]
+        content = content.encode(encoding)
+
+    elif not isinstance(content, bytes):
+        raise TypeError('content must be str or bytes')
+    
+    # Set data dict
+    data = {
+        'name': name, 
+        'filename': filename, 
+        'content': content
+    }
+
+    # Send request
+    rest_url = '/rest/xslt/'
+    response = self.post(rest_url, data=data)
+
+    if verbose and response.status_code == 201:
+        xslt_id = response.json()['id']
+        print(f'xslt {name} ({xslt_id}) successfully uploaded.')
+
+def update_xslt(self,
+                name: Optional[str] = None,
+                filename: Optional[str] = None,
+                content: Union[str, bytes, None] = None,
+                newname: Optional[str] = None,
+                newfilename: Optional[str] = None,
+                xslt: Optional[pd.Series] = None,
+                xslt_id: Optional[str] = None,
+                verbose: bool = False):
+    """
+    Updates values associated with an XSLT transformation.  The XSLT entry to be
+    updated can be uniquely identified using name and filename, xslt, or xslt_id.
+    
+    Parameters
+    ----------
+    name : str, optional
+        An XSLT name. Will be used to identify the existing xslt entry to update if
+        neither xslt nor xslt_id parameters are given. If either xslt or xslt_id are
+        given, this can be used to assign a new name to the entry.
+    filename : str, optional
+        An xslt filename. Will be used to identify the existing xslt entry to update if
+        neither xslt nor xslt_id parameters are given. If either xslt or xslt_id are
+        given, this can be used to assign a new filename to the entry.
+    content : str, optional
+        New xsl content to assign to the entry.
+    newname : str, optional
+        New name to assign to the entry.
+    newfilename : str, optional
+        New filename to assign to the entry.
+    xslt : pd.Series, optional
+        The XSLT entry information for the entry that is being updated.  
+    xslt_id : str, optional
+        The database id that uniquely identifies the XSLT entry. 
+    verbose : bool, optional
+        Setting this to True will print extra status messages.  Default value
+        is False.
+    """
+    
+    # Get xslt_id from xslt
+    if xslt is not None:
+        if xslt_id is not None:
+            raise ValueError('xslt and xslt_id cannot both be given')
+        xslt_id = xslt['id']
+    
+    # Get new values if xslt_id is known
+    if xslt_id is not None:
+        
+        if name is not None:
+            if newname is not None:
+                raise ValueError('name and newname are aliases when xslt or xslt_id are given')
+            newname = name
+            
+        if filename is not None:
+            if newfilename is not None:
+                raise ValueError('filename and newfilename are aliases when xslt or xslt_id are given')
+            newfilename = filename
+    
+    # Get matching xslt from name, filename values
+    else:
+        xslt = self.get_xslt(name=name, filename=filename)
+        xslt_id = xslt['id']
+           
+    if newfilename is not None:
+        if content is None and Path(newfilename).is_file():
+            with open(newfilename, 'rb') as xmlfile:
+                content = xmlfile.read()
+        newfilename = Path(newfilename).name
+    
+    if isinstance(content, str):
+        try:
+            e = content.index('?>')
+        except:
+            encoding = 'UTF-8'
+        else:
+            try:
+                s = content[:e].index('encoding') + 8
+            except:
+                encoding = 'UTF-8'
+            else:
+                s = content[s:e].index('"')+s+1
+                e = content[s:e].index('"') + s
+                encoding = content[s:e]
+        content = content.encode(encoding)
+    
+    # Set data dict
+    data = {
+        'name': newname, 
+        'filename': newfilename, 
+        'content': content
+    }
+    
+    rest_url = f'/rest/xslt/{xslt_id}/'
+    response = self.patch(rest_url, data=data)
+    
+    if verbose and response.status_code == 201:
+        name = response.json()['name']
+        print(f'xslt {name} ({xslt_id}) successfully updated.')
+
+def delete_xslt(self,
+                name: Optional[str] = None,
+                filename: Optional[str] = None,
+                xslt: Optional[pd.Series] = None,
+                xslt_id: Optional[str] = None,
+                verbose: bool = False):
+    """
+    Deletes an XSLT file from the database.
+
+    Parameters
+    ----------
+    name : str, optional
+        Values for name and filename can be specified to try to uniquely
+        identify the XSLT entry to delete.  Cannot be combined with xslt or
+        xslt_id as they uniquely identify the XSLT on their own.
+    filename : str, optional
+        Values for name and filename can be specified to try to uniquely
+        identify the XSLT entry to delete.  Cannot be combined with xslt or
+        xslt_id as they uniquely identify the XSLT on their own.
+    xslt : pd.Series, optional
+        The xslt entry information for the entry that is to be deleted.  
+        Cannot be combined with name, filename or xslt_id.
+    xslt_id : str, optional
+        The database id that uniquely identifies the xslt entry to delete. 
+        Cannot be combined with name, filename or xslt.
+    verbose : bool, optional
+        Setting this to True will print extra status messages.  Default value
+        is False.
+    """
+
+    # Get xslt_id from xslt
+    if xslt is not None:
+        if xslt_id is not None:
+            raise ValueError('xslt and xslt_id cannot both be given')
+        xslt_id = xslt['id']
+    
+    # Get new values if xslt_id is known
+    if xslt_id is not None:
+        
+        if name is not None:
+            raise ValueError('name cannot be given with xslt or xslt_id')
+                        
+        if filename is not None:
+            raise ValueError('filename cannot be given with xslt or xslt_id')
+            
+    # Get matching xslt from name, filename values
+    else:
+        xslt = self.get_xslt(name=name, filename=filename)
+        xslt_id = xslt['id']
+
+    rest_url = f'/rest/xslt/{xslt_id}/'
+    response = self.delete(rest_url)
+
+    if verbose and response.status_code == 204:
+        print(f'xslt with id ({xslt_id}) has been deleted.')
```

### Comparing `cdcs-0.2.2/cdcs/RestClient.py` & `cdcs-0.2.3/cdcs/RestClient.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,403 +1,421 @@
-# coding: utf-8
-
-# Standard library imports
-import getpass
-from pathlib import Path
-from typing import Optional, Union, Tuple
-
-
-# http://docs.python-requests.org
-import requests
-
-# Ignore certification warnings (for now)
-from requests.packages.urllib3.exceptions import InsecureRequestWarning 
-requests.packages.urllib3.disable_warnings(InsecureRequestWarning)
-
-class RestClient(object):
-    """
-    Generic class for building REST calls to web databases in Python.
-    """
-    def __init__(self, host: str,
-                 username: Optional[str] = None,
-                 password: Optional[str] = None,
-                 auth: Optional[Tuple[str]] = None,
-                 cert: Union[str, Tuple[str], None] = None, 
-                 certification: Union[str, Tuple[str], None] = None,
-                 verify: Optional[bool] = True):
-        """
-        Class initializer. Tests and stores access information.
-        
-        Parameters
-        ----------
-        host : str
-            URL for the database's server.
-        username : str, optional
-            Username of desired account on the server. A prompt will ask for
-            the username if not given.
-        password : str, optional
-            Password of desired account on the server.  A prompt will ask for
-            the password if not given.
-        auth : tuple, optional
-            Auth tuple to enable Basic/Digest/Custom HTTP Auth.  Alternative to
-            giving username and password seperately.
-        cert : str, optional
-            if String, path to ssl client cert file (.pem). If Tuple,
-            ('cert', 'key') pair.
-        certification : str, optional
-            Alias for cert. Retained for compatibility.
-        verify : bool or str, optional
-            Either a boolean, in which case it controls whether we verify the
-            server's TLS certificate, or a string, in which case it must be a
-            path to a CA bundle to use. Defaults to True.
-        """
-        # Set access information
-        self.login(host, username=username, password=password,
-                   auth=auth, cert=cert, certification=certification,
-                   verify=verify)
-
-    def __str__(self) -> str:
-        """str: String representation gives username and host info."""
-        return f'RestClient for {self.username} @ {self.host}'
-        
-    @property
-    def host(self) -> str:
-        """str: The host url for the server."""
-        return self.__host
-    
-    @property
-    def username(self) -> str:
-        """str: The username to use for the server."""
-        return self.__user
-    
-    @property
-    def cert(self) -> Optional[str]:
-        """str or None: The certification information."""
-        return self.__cert
-
-    @property
-    def verify(self) -> bool:
-        """bool: The verify setting for the database."""
-        return self.__verify
-
-    def login(self, host: str,
-              username: Optional[str] = None,
-              password: Optional[str] = None, 
-              auth: Optional[Tuple[str]] = None,
-              cert: Union[str, Tuple[str], None] = None, 
-              certification: Union[str, Tuple[str], None] = None,
-              verify: Optional[bool] = True):
-        """
-        Tests and stores access information.
-        
-        Parameters
-        ----------
-        host : str
-            URL for the database's server.
-        username : str, optional
-            Username of desired account on the server. A prompt will ask for
-            the username if not given.
-        password : str, optional
-            Password of desired account on the server.  A prompt will ask for
-            the password if not given.
-        auth : tuple, optional
-            Auth tuple to enable Basic/Digest/Custom HTTP Auth.  Alternative to
-            giving username and password seperately.
-        cert : str, optional
-            if String, path to ssl client cert file (.pem). If Tuple,
-            ('cert', 'key') pair.
-        certification : str, optional
-            Alias for cert. Retained for compatibility.
-        verify : bool or str, optional
-            Either a boolean, in which case it controls whether we verify the
-            server's TLS certificate, or a string, in which case it must be a
-            path to a CA bundle to use. Defaults to True.
-        """
-        # Handle host
-        host = host.strip('/')
-
-        # Handle username and password
-        if auth is None:
-
-            # Handle username
-            if username is None:
-                username = input(f'Enter username for {host}:')
-       
-            # Handle non-anonymous 
-            if username != '':
-
-                # Handle password
-                if password is None:
-                    password = getpass.getpass(f'Enter password for {username} @ {host}:')
-                auth = (username, password)
-            
-            # Handle anonymous
-            else:
-                username = None
-                auth = None
-
-        # Handle auth 
-        else:
-            assert username is None and password is None, 'auth cannot be given with username and password'
-            username = auth[0]
-
-        # Handle certification
-        if certification is not None:
-            if cert is not None:
-                raise ValueError('Both certification and cert given - they are aliases of each other')
-            cert = certification
-        if isinstance(cert, str):
-            cert = Path(cert)
-            if cert.is_file():
-                cert = str(cert.resolve())
-            else:
-                raise ValueError('Certification file not found!')
-        elif isinstance(cert, (list, tuple)):
-            assert len(cert) == 2
-            if not Path(cert[0]).is_file() or not Path(cert[1].is_file()):
-                raise ValueError('Certification file not found!')
-            
-        # Set object values
-        self.__host = host
-        self.__user = username
-        self.__auth = auth
-        self.__cert = cert
-        self.__verify = verify
-
-        # Test login info
-        if self.__user is not None:
-            self.testcall()
-    
-    def testcall(self):
-        """Simple rest call to check if authentication parameters are valid."""
-        # Default behavior is no test: must be set specific to database type
-        pass
-
-    def request(self, method: str,
-                rest_url: str,
-                checkstatus: bool = True,
-                **kwargs) -> requests.Response:
-        """
-        Wrapper around requests.request that automatically sets any access
-        parameters based on the stored login information.
-        
-        Parameters
-        ----------
-        method : str
-            Method for the new Request object.
-        rest_url : str
-            The REST command URL, i.e. URL path after host.
-        checkstatus : bool
-            If True (default) then the response status of the call will be
-            checked and an error thrown if bad.  Setting this to False will
-            not automatically check the status.
-        **kwargs : any, optional
-            Any other arguments supported by requests.request() except for url.
-            Default values for auth, verify, and cert will be used based on the
-            values set during class initialization/login.
-        
-        Returns
-        -------
-        requests.Response
-            The response object.
-
-        Raises
-        ------
-        requests.HTTPError
-            Any requests errors if the response code is not ok.
-        """
-        
-        # Set url and access parameters
-        url = self.host + '/' + rest_url.lstrip('/')
-        
-        auth = kwargs.pop('auth', self.__auth)
-        cert = kwargs.pop('cert', self.cert)
-        verify = kwargs.pop('verify', self.verify)
-        
-        # Send request
-        response = requests.request(method, url, auth=auth, verify=verify,
-                                    cert=cert, **kwargs)
-        
-        # Check for errors
-        if checkstatus and not response.ok:
-            try:
-                print(response.json())
-            except:
-                print(response.text)
-            response.raise_for_status()
-        
-        return response
-    
-    def head(self, rest_url: str,
-             **kwargs) -> requests.Response:
-        """
-        Wrapper around requests.head that automatically sets any access
-        parameters based on the stored login information.
-        
-        Parameters
-        ----------
-        rest_url : str
-            The REST command URL, i.e. URL path after host.
-        **kwargs : any, optional
-            Any other arguments supported by requests.request() except for url.
-            Default values for auth, verify, and cert will be used based on the
-            values set during class initialization/login.
-        
-        Returns
-        -------
-        requests.Response
-            The response object.
-
-        Raises
-        ------
-        requests.HTTPError
-            Any requests errors if the response code is not ok.
-        """
-        # Change default allow_redirects to reflect requests.head()
-        if 'allow_redirects' not in kwargs:
-            kwargs['allow_redirects'] = False
-            
-        return self.request('head', rest_url, **kwargs)
-    
-    def get(self, rest_url: str,
-            **kwargs) -> requests.Response:
-        """
-        Wrapper around requests.get that automatically sets any access
-        parameters based on the stored login information.
-        
-        Parameters
-        ----------
-        rest_url : str
-            The REST command URL, i.e. URL path after host.
-        **kwargs : any, optional
-            Any other arguments supported by requests.request() except for url.
-            Default values for auth, verify, and cert will be used based on the
-            values set during class initialization/login.
-        
-        Returns
-        -------
-        requests.Response
-            The response object.
-
-        Raises
-        ------
-        requests.HTTPError
-            Any requests errors if the response code is not ok.
-        """
-        return self.request('get', rest_url, **kwargs)
-        
-    def post(self, rest_url: str,
-             data: Union[dict, bytes, None] = None,
-             **kwargs) -> requests.Response:
-        """
-        Wrapper around requests.post that automatically sets any access
-        parameters based on the stored login information.
-        
-        Parameters
-        ----------
-        rest_url : str
-            The REST command URL, i.e. URL path after host.
-        data : dict or bytes, optional
-            Data to send in the body of the Request.
-        **kwargs : any, optional
-            Any other arguments supported by requests.request() except for url.
-            Default values for auth, verify, and cert will be used based on the
-            values set during class initialization/login.
-        
-        Returns
-        -------
-        requests.Response
-            The response object.
-
-        Raises
-        ------
-        requests.HTTPError
-            Any requests errors if the response code is not ok.
-        """
-        return self.request('post', rest_url, data=data, **kwargs)
-    
-    def put(self, rest_url: str,
-            data: Union[dict, bytes, None] = None,
-            **kwargs) -> requests.Response:
-        """
-        Wrapper around requests.put that automatically sets any access
-        parameters based on the stored login information.
-        
-        Parameters
-        ----------
-        rest_url : str
-            The REST command URL, i.e. URL path after host.
-        data : dict or bytes, optional
-            Data to send in the body of the Request.
-        **kwargs : any, optional
-            Any other arguments supported by requests.request() except for url.
-            Default values for auth, verify, and cert will be used based on the
-            values set during class initialization/login.
-        
-        Returns
-        -------
-        requests.Response
-            The response object.
-
-        Raises
-        ------
-        requests.HTTPError
-            Any requests errors if the response code is not ok.
-        """
-        return self.request('put', rest_url, data=data, **kwargs)
-    
-    def patch(self, rest_url: str,
-              data: Union[dict, bytes, None] = None,
-              **kwargs) -> requests.Response:
-        """
-        Wrapper around requests.patch that automatically sets any access
-        parameters based on the stored login information.
-        
-        Parameters
-        ----------
-        rest_url : str
-            The REST command URL, i.e. URL path after host.
-        data : dict or bytes, optional
-            Data to send in the body of the Request.
-        **kwargs : any, optional
-            Any other arguments supported by requests.request() except for url.
-            Default values for auth, verify, and cert will be used based on the
-            values set during class initialization/login.
-        
-        Returns
-        -------
-        requests.Response
-            The response object.
-
-        Raises
-        ------
-        requests.HTTPError
-            Any requests errors if the response code is not ok.
-        """
-        return self.request('patch', rest_url, data=data, **kwargs)
-    
-    def delete(self, rest_url: str,
-               **kwargs) -> requests.Response:
-        """
-        Wrapper around requests.delete that automatically sets any access
-        parameters based on the stored login information.
-        
-        Parameters
-        ----------
-        rest_url : str
-            The REST command URL, i.e. URL path after host.
-        **kwargs : any, optional
-            Any other arguments supported by requests.request() except for url.
-            Default values for auth, verify, and cert will be used based on the
-            values set during class initialization/login.
-        
-        Returns
-        -------
-        requests.Response
-            The response object.
-
-        Raises
-        ------
-        requests.HTTPError
-            Any requests errors if the response code is not ok.
-        """
+# coding: utf-8
+
+# Standard library imports
+import getpass
+from pathlib import Path
+from typing import Optional, Union, Tuple
+
+
+# http://docs.python-requests.org
+import requests
+
+# Ignore certification warnings (for now)
+from requests.packages.urllib3.exceptions import InsecureRequestWarning 
+requests.packages.urllib3.disable_warnings(InsecureRequestWarning)
+
+class RestClient(object):
+    """
+    Generic class for building REST calls to web databases in Python.
+    """
+    def __init__(self, host: str,
+                 username: Optional[str] = None,
+                 password: Optional[str] = None,
+                 auth: Optional[Tuple[str]] = None,
+                 cert: Union[str, Tuple[str], None] = None, 
+                 certification: Union[str, Tuple[str], None] = None,
+                 verify: Optional[bool] = True):
+        """
+        Class initializer. Tests and stores access information.
+        
+        Parameters
+        ----------
+        host : str
+            URL for the database's server.
+        username : str, optional
+            Username of desired account on the server. A prompt will ask for
+            the username if not given.
+        password : str, optional
+            Password of desired account on the server.  A prompt will ask for
+            the password if not given.
+        auth : tuple, optional
+            Auth tuple to enable Basic/Digest/Custom HTTP Auth.  Alternative to
+            giving username and password seperately.
+        cert : str, optional
+            if String, path to ssl client cert file (.pem). If Tuple,
+            ('cert', 'key') pair.
+        certification : str, optional
+            Alias for cert. Retained for compatibility.
+        verify : bool or str, optional
+            Either a boolean, in which case it controls whether we verify the
+            server's TLS certificate, or a string, in which case it must be a
+            path to a CA bundle to use. Defaults to True.
+        """
+        # Set access information
+        self.login(host, username=username, password=password,
+                   auth=auth, cert=cert, certification=certification,
+                   verify=verify)
+
+    def __str__(self) -> str:
+        """str: String representation gives username and host info."""
+        return f'RestClient for {self.username} @ {self.host}'
+        
+    @property
+    def host(self) -> str:
+        """str: The host url for the server."""
+        return self.__host
+    
+    @property
+    def username(self) -> str:
+        """str: The username to use for the server."""
+        return self.__user
+    
+    @property
+    def cert(self) -> Optional[str]:
+        """str or None: The certification information."""
+        return self.__cert
+
+    @property
+    def verify(self) -> bool:
+        """bool: The verify setting for the database."""
+        return self.__verify
+
+    def login(self, host: str,
+              username: Optional[str] = None,
+              password: Optional[str] = None, 
+              auth: Optional[Tuple[str]] = None,
+              cert: Union[str, Tuple[str], None] = None, 
+              certification: Union[str, Tuple[str], None] = None,
+              verify: Optional[bool] = True):
+        """
+        Tests and stores access information.
+        
+        Parameters
+        ----------
+        host : str
+            URL for the database's server.
+        username : str, optional
+            Username of desired account on the server. A prompt will ask for
+            the username if not given.
+        password : str, optional
+            Password of desired account on the server.  A prompt will ask for
+            the password if not given.
+        auth : tuple, optional
+            Auth tuple to enable Basic/Digest/Custom HTTP Auth.  Alternative to
+            giving username and password seperately.
+        cert : str, optional
+            if String, path to ssl client cert file (.pem). If Tuple,
+            ('cert', 'key') pair.
+        certification : str, optional
+            Alias for cert. Retained for compatibility.
+        verify : bool or str, optional
+            Either a boolean, in which case it controls whether we verify the
+            server's TLS certificate, or a string, in which case it must be a
+            path to a CA bundle to use. Defaults to True.
+        """
+        # Handle host
+        host = host.strip('/')
+
+        # Handle username and password
+        if auth is None:
+
+            # Handle username
+            if username is None:
+                username = input(f'Enter username for {host}:')
+       
+            # Handle non-anonymous 
+            if username != '':
+
+                # Handle password
+                if password is None:
+                    password = getpass.getpass(f'Enter password for {username} @ {host}:')
+                auth = (username, password)
+            
+            # Handle anonymous
+            else:
+                username = None
+                auth = None
+
+        # Handle auth 
+        else:
+            assert username is None and password is None, 'auth cannot be given with username and password'
+            username = auth[0]
+
+        # Handle certification
+        if certification is not None:
+            if cert is not None:
+                raise ValueError('Both certification and cert given - they are aliases of each other')
+            cert = certification
+        if isinstance(cert, str):
+            cert = Path(cert)
+            if cert.is_file():
+                cert = str(cert.resolve())
+            else:
+                raise ValueError('Certification file not found!')
+        elif isinstance(cert, (list, tuple)):
+            assert len(cert) == 2
+            if not Path(cert[0]).is_file() or not Path(cert[1].is_file()):
+                raise ValueError('Certification file not found!')
+            
+        # Set object values
+        self.__host = host
+        self.__user = username
+        self.__auth = auth
+        self.__cert = cert
+        self.__verify = verify
+
+        # Test login info
+        if self.__user is not None:
+            self.testcall()
+    
+    def testcall(self):
+        """Simple rest call to check if authentication parameters are valid."""
+        # Default behavior is no test: must be set specific to database type
+        pass
+
+    def request(self, method: str,
+                rest_url: str,
+                checkstatus: bool = True,
+                retry504: int = 5,
+                **kwargs) -> requests.Response:
+        """
+        Wrapper around requests.request that automatically sets any access
+        parameters based on the stored login information.
+        
+        Parameters
+        ----------
+        method : str
+            Method for the new Request object.
+        rest_url : str
+            The REST command URL, i.e. URL path after host.
+        checkstatus : bool
+            If True (default) then the response status of the call will be
+            checked and an error thrown if bad.  Setting this to False will
+            not automatically check the status.
+        retry504 : int, optional
+            Number of times the request will be tried if a 504 gateway timeout
+            status is received.  Useful for finnicky databases.  Default value
+            is 5.
+        **kwargs : any, optional
+            Any other arguments supported by requests.request() except for url.
+            Default values for auth, verify, and cert will be used based on the
+            values set during class initialization/login.
+        
+        Returns
+        -------
+        requests.Response
+            The response object.
+
+        Raises
+        ------
+        requests.HTTPError
+            Any requests errors if the response code is not ok.
+        """
+        
+        # Set url and access parameters
+        url = self.host + '/' + rest_url.lstrip('/')
+        
+        auth = kwargs.pop('auth', self.__auth)
+        cert = kwargs.pop('cert', self.cert)
+        verify = kwargs.pop('verify', self.verify)
+        
+        # Loop to repeat request calls
+        count504 = 0
+        while True:
+            # Send request
+            response = requests.request(method, url, auth=auth, verify=verify,
+                                        cert=cert, **kwargs)
+            
+            # Count 504 Gateway timeout errors
+            if response.status_code == 504:
+                count504 += 1
+                if count504 == retry504:
+                    break
+            
+            # Break for all other status codes
+            else:
+                break
+        
+        # Check for errors
+        if checkstatus and not response.ok:
+            try:
+                print(response.json())
+            except:
+                print(response.text)
+            response.raise_for_status()
+        
+        return response
+    
+    def head(self, rest_url: str,
+             **kwargs) -> requests.Response:
+        """
+        Wrapper around requests.head that automatically sets any access
+        parameters based on the stored login information.
+        
+        Parameters
+        ----------
+        rest_url : str
+            The REST command URL, i.e. URL path after host.
+        **kwargs : any, optional
+            Any other arguments supported by requests.request() except for url.
+            Default values for auth, verify, and cert will be used based on the
+            values set during class initialization/login.
+        
+        Returns
+        -------
+        requests.Response
+            The response object.
+
+        Raises
+        ------
+        requests.HTTPError
+            Any requests errors if the response code is not ok.
+        """
+        # Change default allow_redirects to reflect requests.head()
+        if 'allow_redirects' not in kwargs:
+            kwargs['allow_redirects'] = False
+            
+        return self.request('head', rest_url, **kwargs)
+    
+    def get(self, rest_url: str,
+            **kwargs) -> requests.Response:
+        """
+        Wrapper around requests.get that automatically sets any access
+        parameters based on the stored login information.
+        
+        Parameters
+        ----------
+        rest_url : str
+            The REST command URL, i.e. URL path after host.
+        **kwargs : any, optional
+            Any other arguments supported by requests.request() except for url.
+            Default values for auth, verify, and cert will be used based on the
+            values set during class initialization/login.
+        
+        Returns
+        -------
+        requests.Response
+            The response object.
+
+        Raises
+        ------
+        requests.HTTPError
+            Any requests errors if the response code is not ok.
+        """
+        return self.request('get', rest_url, **kwargs)
+        
+    def post(self, rest_url: str,
+             data: Union[dict, bytes, None] = None,
+             **kwargs) -> requests.Response:
+        """
+        Wrapper around requests.post that automatically sets any access
+        parameters based on the stored login information.
+        
+        Parameters
+        ----------
+        rest_url : str
+            The REST command URL, i.e. URL path after host.
+        data : dict or bytes, optional
+            Data to send in the body of the Request.
+        **kwargs : any, optional
+            Any other arguments supported by requests.request() except for url.
+            Default values for auth, verify, and cert will be used based on the
+            values set during class initialization/login.
+        
+        Returns
+        -------
+        requests.Response
+            The response object.
+
+        Raises
+        ------
+        requests.HTTPError
+            Any requests errors if the response code is not ok.
+        """
+        return self.request('post', rest_url, data=data, **kwargs)
+    
+    def put(self, rest_url: str,
+            data: Union[dict, bytes, None] = None,
+            **kwargs) -> requests.Response:
+        """
+        Wrapper around requests.put that automatically sets any access
+        parameters based on the stored login information.
+        
+        Parameters
+        ----------
+        rest_url : str
+            The REST command URL, i.e. URL path after host.
+        data : dict or bytes, optional
+            Data to send in the body of the Request.
+        **kwargs : any, optional
+            Any other arguments supported by requests.request() except for url.
+            Default values for auth, verify, and cert will be used based on the
+            values set during class initialization/login.
+        
+        Returns
+        -------
+        requests.Response
+            The response object.
+
+        Raises
+        ------
+        requests.HTTPError
+            Any requests errors if the response code is not ok.
+        """
+        return self.request('put', rest_url, data=data, **kwargs)
+    
+    def patch(self, rest_url: str,
+              data: Union[dict, bytes, None] = None,
+              **kwargs) -> requests.Response:
+        """
+        Wrapper around requests.patch that automatically sets any access
+        parameters based on the stored login information.
+        
+        Parameters
+        ----------
+        rest_url : str
+            The REST command URL, i.e. URL path after host.
+        data : dict or bytes, optional
+            Data to send in the body of the Request.
+        **kwargs : any, optional
+            Any other arguments supported by requests.request() except for url.
+            Default values for auth, verify, and cert will be used based on the
+            values set during class initialization/login.
+        
+        Returns
+        -------
+        requests.Response
+            The response object.
+
+        Raises
+        ------
+        requests.HTTPError
+            Any requests errors if the response code is not ok.
+        """
+        return self.request('patch', rest_url, data=data, **kwargs)
+    
+    def delete(self, rest_url: str,
+               **kwargs) -> requests.Response:
+        """
+        Wrapper around requests.delete that automatically sets any access
+        parameters based on the stored login information.
+        
+        Parameters
+        ----------
+        rest_url : str
+            The REST command URL, i.e. URL path after host.
+        **kwargs : any, optional
+            Any other arguments supported by requests.request() except for url.
+            Default values for auth, verify, and cert will be used based on the
+            values set during class initialization/login.
+        
+        Returns
+        -------
+        requests.Response
+            The response object.
+
+        Raises
+        ------
+        requests.HTTPError
+            Any requests errors if the response code is not ok.
+        """
         return self.request('delete', rest_url, **kwargs)
```

### Comparing `cdcs-0.2.2/cdcs/aslist.py` & `cdcs-0.2.3/cdcs/aslist.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-# coding: utf-8
-
-# Standard library imports
-from typing import Any, Generator
-
-# https://pandas.pydata.org/
-import pandas as pd
-
-def iaslist(term: Any) -> Generator[Any, None, None]:
-    """
-    Iterate over items in term as if term was a list. Treats a str
-    term as a single item.
-    
-    Parameters
-    ----------
-    term : any
-        Term to iterate over.
-    
-    Yields
-    ------
-    any
-        Items in the list representation of term.
-    """
-    if isinstance(term, (str, bytes, pd.Series)):
-        yield term
-    else:
-        try:
-            for t in term:
-                yield t
-        except TypeError:
-            yield term
-
-def aslist(term: Any) -> list:
-    """
-    Create list representation of term. Treats a str term as a single
-    item.
-    
-    Parameters
-    ----------
-    term : any
-        Term to convert into a list, if needed.
-        
-    Returns
-    -------
-    list
-        All items in term as a list.
-    """
-    return [t for t in iaslist(term)]
+# coding: utf-8
+
+# Standard library imports
+from typing import Any, Generator
+
+# https://pandas.pydata.org/
+import pandas as pd
+
+def iaslist(term: Any) -> Generator[Any, None, None]:
+    """
+    Iterate over items in term as if term was a list. Treats a str
+    term as a single item.
+    
+    Parameters
+    ----------
+    term : any
+        Term to iterate over.
+    
+    Yields
+    ------
+    any
+        Items in the list representation of term.
+    """
+    if isinstance(term, (str, bytes, pd.Series)):
+        yield term
+    else:
+        try:
+            for t in term:
+                yield t
+        except TypeError:
+            yield term
+
+def aslist(term: Any) -> list:
+    """
+    Create list representation of term. Treats a str term as a single
+    item.
+    
+    Parameters
+    ----------
+    term : any
+        Term to convert into a list, if needed.
+        
+    Returns
+    -------
+    list
+        All items in term as a list.
+    """
+    return [t for t in iaslist(term)]
```

### Comparing `cdcs-0.2.2/cdcs/date_parser.py` & `cdcs-0.2.3/cdcs/date_parser.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-# coding: utf-8
-
-# https://pandas.pydata.org/
-import pandas as pd
-
-def date_parser(series: pd.Series,
-                key: str) -> pd.Timestamp:
-    """
-    Parses iso date fields into Python objects. Can be used as a DataFrame
-    apply function.
-
-    Parameters
-    ----------
-    series : pandas.Series
-        A series containing a date field represented in iso string format.
-    key : str
-        The name of the series field containing the iso string date.
-
-    Returns
-    -------
-    pandas.Timestamp
-        The date as an object
-    """
+# coding: utf-8
+
+# https://pandas.pydata.org/
+import pandas as pd
+
+def date_parser(series: pd.Series,
+                key: str) -> pd.Timestamp:
+    """
+    Parses iso date fields into Python objects. Can be used as a DataFrame
+    apply function.
+
+    Parameters
+    ----------
+    series : pandas.Series
+        A series containing a date field represented in iso string format.
+    key : str
+        The name of the series field containing the iso string date.
+
+    Returns
+    -------
+    pandas.Timestamp
+        The date as an object
+    """
     return pd.Timestamp(series[key])
```

### Comparing `cdcs-0.2.2/cdcs.egg-info/PKG-INFO` & `cdcs-0.2.3/cdcs.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,52 @@
-Metadata-Version: 2.1
-Name: cdcs
-Version: 0.2.2
-Summary: Python API client for performing REST calls to configurable data curation system (CDCS) databases
-Home-page: https://github.com/usnistgov/pycdcs
-Author: Lucas Hale
-Author-email: lucas.hale@nist.gov
-Keywords: CDCS,database,rest API,configurable data curation system
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering :: Physics
-License-File: LICENSE.TXT
-
-# Python CDCS REST API client
-
-This is a base Python package for accessing instances of the NIST Configurable Data Curation System (CDCS) databases, versions 2.X.X and 3.X.X.  It defines a Python CDCS class that streamlines REST calls to a database by
-
-- Taking access settings once (username, password, etc) and saving them for subsequent REST calls.
-- Defining methods that wrap around REST calls to interact with the database in a more Pythonic way.
-- Automatically converting any accessed information to pandas Series and DataFrame objects to allow for the information to be easily manipulated.
-
-## Installation
-
-The package can be installed using pip:
-
-    pip install cdcs
-
-or conda:
-
-    conda install -c conda-forge cdcs
-
-Alternatively, the source code can be downloaded from github at
-
-- Stable releases: [https://github.com/usnistgov/pycdcs](https://github.com/usnistgov/pycdcs)
-- In development: [https://github.com/lmhale99/pycdcs](https://github.com/lmhale99/pycdcs)
-
-## Documentation
-
-Documentation for the package is given as Jupyter Notebooks that can be found on the github site.  Each Notebook is focused on providing details and examples related to different use cases for the package.
-
-- **CDCS Public Data Exploration** outlines the basic functions allowing an anonymous user (i.e. not logged in) to explore the available public data on a curator.
-- **CDCS Data Management** outlines the basic pre-defined functions allowing a logged-in user to manage their own templates, data records and blobs.
-- **CDCS Rest Builder** provides a simple explanation of how users can easily build their own functions and make their own REST API calls should they wish to interact with the database in ways outside the pre-defined functions.
+Metadata-Version: 2.1
+Name: cdcs
+Version: 0.2.3
+Summary: Python API client for performing REST calls to configurable data curation system (CDCS) databases
+Home-page: https://github.com/usnistgov/pycdcs
+Author: Lucas Hale
+Author-email: lucas.hale@nist.gov
+Keywords: CDCS,database,rest API,configurable data curation system
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering :: Physics
+License-File: LICENSE.TXT
+Requires-Dist: requests
+Requires-Dist: pandas
+Requires-Dist: tqdm
+Requires-Dist: ipython
+
+# Python CDCS REST API client
+
+This is a base Python package for accessing instances of the NIST Configurable Data Curation System (CDCS) databases, versions 2.X.X and 3.X.X.  It defines a Python CDCS class that streamlines REST calls to a database by
+
+- Taking access settings once (username, password, etc) and saving them for subsequent REST calls.
+- Defining methods that wrap around REST calls to interact with the database in a more Pythonic way.
+- Automatically converting any accessed information to pandas Series and DataFrame objects to allow for the information to be easily manipulated.
+
+## Installation
+
+The package can be installed using pip:
+
+    pip install cdcs
+
+or conda:
+
+    conda install -c conda-forge cdcs
+
+Alternatively, the source code can be downloaded from github at
+
+- Stable releases: [https://github.com/usnistgov/pycdcs](https://github.com/usnistgov/pycdcs)
+- In development: [https://github.com/lmhale99/pycdcs](https://github.com/lmhale99/pycdcs)
+
+## Documentation
+
+Documentation for the package is given as Jupyter Notebooks that can be found on the github site.  Each Notebook is focused on providing details and examples related to different use cases for the package.
+
+- **CDCS Public Data Exploration** outlines the basic functions allowing an anonymous user (i.e. not logged in) to explore the available public data on a curator.
+- **CDCS Data Management** outlines the basic pre-defined functions allowing a logged-in user to manage their own templates, data records and blobs.
+- **CDCS Rest Builder** provides a simple explanation of how users can easily build their own functions and make their own REST API calls should they wish to interact with the database in ways outside the pre-defined functions.
```

