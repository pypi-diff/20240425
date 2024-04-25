# Comparing `tmp/fortitudo_tech-1.0.5.tar.gz` & `tmp/fortitudo_tech-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fortitudo_tech-1.0.5.tar", max compression
+gzip compressed data, was "fortitudo_tech-1.0.6.tar", max compression
```

## Comparing `fortitudo_tech-1.0.5.tar` & `fortitudo_tech-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    35149 2024-04-04 18:15:08.717857 fortitudo_tech-1.0.5/LICENSE
--rw-r--r--   0        0        0     3683 2024-04-04 18:15:08.717857 fortitudo_tech-1.0.5/README.rst
--rw-r--r--   0        0        0     1219 2024-04-04 18:15:08.737857 fortitudo_tech-1.0.5/fortitudo/tech/__init__.py
--rw-r--r--   0        0        0      636 2024-04-04 18:15:08.737857 fortitudo_tech-1.0.5/fortitudo/tech/data/parameters.csv
--rw-r--r--   0        0        0  2056742 2024-04-04 18:15:08.747857 fortitudo_tech-1.0.5/fortitudo/tech/data/pnl.csv
--rw-r--r--   0        0        0  8127147 2024-04-04 18:15:08.777857 fortitudo_tech-1.0.5/fortitudo/tech/data/risk_factors.csv
--rw-r--r--   0        0        0  3725592 2024-04-04 18:15:08.787857 fortitudo_tech-1.0.5/fortitudo/tech/data/time_series.csv
--rw-r--r--   0        0        0     3626 2024-04-04 18:15:08.737857 fortitudo_tech-1.0.5/fortitudo/tech/data.py
--rw-r--r--   0        0        0     3122 2024-04-04 18:15:08.787857 fortitudo_tech-1.0.5/fortitudo/tech/entropy_pooling.py
--rw-r--r--   0        0        0     7336 2024-04-04 18:15:08.787857 fortitudo_tech-1.0.5/fortitudo/tech/functions.py
--rw-r--r--   0        0        0    13170 2024-04-04 18:15:08.787857 fortitudo_tech-1.0.5/fortitudo/tech/optimization.py
--rw-r--r--   0        0        0     2770 2024-04-04 18:15:08.787857 fortitudo_tech-1.0.5/fortitudo/tech/option_pricing.py
--rw-r--r--   0        0        0     2083 2024-04-04 18:15:08.787857 fortitudo_tech-1.0.5/fortitudo/tech/simulation.py
--rw-r--r--   0        0        0     1743 2024-04-04 18:16:41.037859 fortitudo_tech-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     4591 1970-01-01 00:00:00.000000 fortitudo_tech-1.0.5/setup.py
--rw-r--r--   0        0        0     5358 1970-01-01 00:00:00.000000 fortitudo_tech-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-25 10:46:40.955727 fortitudo_tech-1.0.6/LICENSE
+-rw-r--r--   0        0        0     3869 2024-04-25 10:54:46.905726 fortitudo_tech-1.0.6/README.rst
+-rw-r--r--   0        0        0     1219 2024-04-25 10:46:40.985727 fortitudo_tech-1.0.6/fortitudo/tech/__init__.py
+-rw-r--r--   0        0        0      636 2024-04-25 10:46:40.985727 fortitudo_tech-1.0.6/fortitudo/tech/data/parameters.csv
+-rw-r--r--   0        0        0  2056742 2024-04-25 10:46:40.995727 fortitudo_tech-1.0.6/fortitudo/tech/data/pnl.csv
+-rw-r--r--   0        0        0  8127147 2024-04-25 10:46:41.015727 fortitudo_tech-1.0.6/fortitudo/tech/data/risk_factors.csv
+-rw-r--r--   0        0        0  3725592 2024-04-25 10:46:41.025727 fortitudo_tech-1.0.6/fortitudo/tech/data/time_series.csv
+-rw-r--r--   0        0        0     3626 2024-04-25 10:46:40.985727 fortitudo_tech-1.0.6/fortitudo/tech/data.py
+-rw-r--r--   0        0        0     3122 2024-04-25 10:46:41.025727 fortitudo_tech-1.0.6/fortitudo/tech/entropy_pooling.py
+-rw-r--r--   0        0        0     7336 2024-04-25 10:46:41.025727 fortitudo_tech-1.0.6/fortitudo/tech/functions.py
+-rw-r--r--   0        0        0    13170 2024-04-25 10:46:41.025727 fortitudo_tech-1.0.6/fortitudo/tech/optimization.py
+-rw-r--r--   0        0        0     2770 2024-04-25 10:46:41.025727 fortitudo_tech-1.0.6/fortitudo/tech/option_pricing.py
+-rw-r--r--   0        0        0     2083 2024-04-25 10:46:41.025727 fortitudo_tech-1.0.6/fortitudo/tech/simulation.py
+-rw-r--r--   0        0        0     1743 2024-04-25 10:57:36.155726 fortitudo_tech-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     4782 1970-01-01 00:00:00.000000 fortitudo_tech-1.0.6/setup.py
+-rw-r--r--   0        0        0     5544 1970-01-01 00:00:00.000000 fortitudo_tech-1.0.6/PKG-INFO
```

### Comparing `fortitudo_tech-1.0.5/LICENSE` & `fortitudo_tech-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fortitudo_tech-1.0.5/README.rst` & `fortitudo_tech-1.0.6/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -9,20 +9,25 @@
 
 Fortitudo Technologies Open Source
 ==================================
 
 This package allows you to explore open-source implementations of some of our
 fundamental technologies, e.g., Entropy Pooling and CVaR optimization in Python.
 See this `YouTube playlist <https://www.youtube.com/playlist?list=PLfI2BKNVj_b2rurUsCtc2F8lqtPWqcs2K>`_
-for a walkthrough of the package's functionality and examples. For a high-level
-introduction to the investment framework, see this `YouTube video <https://youtu.be/4ESigySdGf8>`_
+for a walkthrough of the package's functionality and examples.
+
+For a high-level introduction to the investment framework, see this `YouTube video <https://youtu.be/4ESigySdGf8>`_
 and `Medium article <https://medium.com/@ft_anvo/entropy-pooling-and-cvar-portfolio-optimization-in-python-ffed736a8347>`_.
 For an in-depth mathematical introduction to the investment framework, see
 these `SSRN articles <https://ssrn.com/author=2738420>`_.
 
+For a careful and pedagogical presentation of the investment framework,
+see the `Portfolio Construction and Risk Management Book <https://igg.me/at/pcrm-book>`_
+crowdfunding campaign.
+
 The package is intended for advanced users who are comfortable specifying
 portfolio constraints and Entropy Pooling views using matrices and vectors.
 This gives full flexibility in relation to working with these technologies.
 Hence, input checking is intentionally kept to a minimum.
 
 If you like this package, we invite you to show your support by giving it a
 GitHub star. The greater the number of stars it receives, the more time and
```

### Comparing `fortitudo_tech-1.0.5/fortitudo/tech/__init__.py` & `fortitudo_tech-1.0.6/fortitudo/tech/__init__.py`

 * *Files identical despite different names*

### Comparing `fortitudo_tech-1.0.5/fortitudo/tech/data/parameters.csv` & `fortitudo_tech-1.0.6/fortitudo/tech/data/parameters.csv`

 * *Files identical despite different names*

### Comparing `fortitudo_tech-1.0.5/fortitudo/tech/data/pnl.csv` & `fortitudo_tech-1.0.6/fortitudo/tech/data/pnl.csv`

 * *Files identical despite different names*

### Comparing `fortitudo_tech-1.0.5/fortitudo/tech/data/risk_factors.csv` & `fortitudo_tech-1.0.6/fortitudo/tech/data/risk_factors.csv`

 * *Files identical despite different names*

### Comparing `fortitudo_tech-1.0.5/fortitudo/tech/data/time_series.csv` & `fortitudo_tech-1.0.6/fortitudo/tech/data/time_series.csv`

 * *Files identical despite different names*

### Comparing `fortitudo_tech-1.0.5/fortitudo/tech/data.py` & `fortitudo_tech-1.0.6/fortitudo/tech/data.py`

 * *Files identical despite different names*

### Comparing `fortitudo_tech-1.0.5/fortitudo/tech/entropy_pooling.py` & `fortitudo_tech-1.0.6/fortitudo/tech/entropy_pooling.py`

 * *Files identical despite different names*

### Comparing `fortitudo_tech-1.0.5/fortitudo/tech/functions.py` & `fortitudo_tech-1.0.6/fortitudo/tech/functions.py`

 * *Files identical despite different names*

### Comparing `fortitudo_tech-1.0.5/fortitudo/tech/optimization.py` & `fortitudo_tech-1.0.6/fortitudo/tech/optimization.py`

 * *Files identical despite different names*

### Comparing `fortitudo_tech-1.0.5/fortitudo/tech/option_pricing.py` & `fortitudo_tech-1.0.6/fortitudo/tech/option_pricing.py`

 * *Files identical despite different names*

### Comparing `fortitudo_tech-1.0.5/fortitudo/tech/simulation.py` & `fortitudo_tech-1.0.6/fortitudo/tech/simulation.py`

 * *Files identical despite different names*

### Comparing `fortitudo_tech-1.0.5/pyproject.toml` & `fortitudo_tech-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fortitudo.tech"
-version = "1.0.5"
+version = "1.0.6"
 description = "Conditional Value-at-Risk (CVaR) portfolio optimization and Entropy Pooling views / stress-testing in Python."
 authors = ["Fortitudo Technologies <software@fortitudo.tech>"]
 license = "GPL-3.0-or-later"
 readme = "README.rst"
 homepage = "https://fortitudo.tech"
 repository = "https://github.com/fortitudo-tech/fortitudo.tech"
 documentation = "https://os.fortitudo.tech"
```

### Comparing `fortitudo_tech-1.0.5/setup.py` & `fortitudo_tech-1.0.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,17 +12,17 @@
  'matplotlib>=3.4,<4.0',
  'numpy>=1.22,<2.0',
  'pandas>=1.3.4',
  'scipy>=1.10,<2.0']
 
 setup_kwargs = {
     'name': 'fortitudo-tech',
-    'version': '1.0.5',
+    'version': '1.0.6',
     'description': 'Conditional Value-at-Risk (CVaR) portfolio optimization and Entropy Pooling views / stress-testing in Python.',
-    'long_description': ".. image:: https://github.com/fortitudo-tech/fortitudo.tech/actions/workflows/tests.yml/badge.svg\n   :target: https://github.com/fortitudo-tech/fortitudo.tech/actions/workflows/tests.yml\n\n.. image:: https://codecov.io/gh/fortitudo-tech/fortitudo.tech/graph/badge.svg?token=Z16XK92Gkl \n   :target: https://codecov.io/gh/fortitudo-tech/fortitudo.tech\n\n.. image:: https://mybinder.org/badge_logo.svg\n   :target: https://mybinder.org/v2/gh/fortitudo-tech/fortitudo.tech/main?labpath=examples\n\nFortitudo Technologies Open Source\n==================================\n\nThis package allows you to explore open-source implementations of some of our\nfundamental technologies, e.g., Entropy Pooling and CVaR optimization in Python.\nSee this `YouTube playlist <https://www.youtube.com/playlist?list=PLfI2BKNVj_b2rurUsCtc2F8lqtPWqcs2K>`_\nfor a walkthrough of the package's functionality and examples. For a high-level\nintroduction to the investment framework, see this `YouTube video <https://youtu.be/4ESigySdGf8>`_\nand `Medium article <https://medium.com/@ft_anvo/entropy-pooling-and-cvar-portfolio-optimization-in-python-ffed736a8347>`_.\nFor an in-depth mathematical introduction to the investment framework, see\nthese `SSRN articles <https://ssrn.com/author=2738420>`_.\n\nThe package is intended for advanced users who are comfortable specifying\nportfolio constraints and Entropy Pooling views using matrices and vectors.\nThis gives full flexibility in relation to working with these technologies.\nHence, input checking is intentionally kept to a minimum.\n\nIf you like this package, we invite you to show your support by giving it a\nGitHub star. The greater the number of stars it receives, the more time and\nenergy we will invest in enhancing its functionality and providing additional\nexamples.\n\nFortitudo Technologies offers novel investment software as well as quantitative\nand digitalization consultancy to the investment management industry. For more\ninformation, please visit our `website <https://fortitudo.tech>`_.\n\nInstallation Instructions\n-------------------------\n\nInstallation can be done via pip::\n\n   pip install fortitudo.tech\n\nFor best performance, we recommend that you install the package in a `conda environment\n<https://conda.io/projects/conda/en/latest/user-guide/concepts/environments.html>`_\nand let conda handle the installation of dependencies before installing the\npackage using pip. You can do this by following these steps::\n\n   conda create -n fortitudo.tech -c conda-forge python scipy pandas matplotlib cvxopt\n   conda activate fortitudo.tech\n   pip install fortitudo.tech\n\nThe examples might require you to install additional packages, e.g., seaborn and\nipykernel / notebook / jupyterlab if you want to run the notebooks. Using pip to\ninstall these packages should not cause any dependency issues.\n\nYou can also explore the examples in the cloud without any local installations using\n`Binder <https://mybinder.org/v2/gh/fortitudo-tech/fortitudo.tech/main?labpath=examples>`_.\nHowever, note that Binder servers have very limited resources and might not support\nsome of the optimized routines this package uses. If you want access to a stable\nand optimized environment with persistent storage, please subscribe to our Data\nScience Server.\n\nDisclaimer\n----------\n\nThis package is completely separate from our proprietary solutions and therefore\nnot representative of the quality and functionality offered by the Investment Simulation\nand Investment Analysis modules. If you are an institutional investor who wants to\nexperience how these methods can be used for sophisticated analysis in practice,\nplease request a demo by sending an email to demo@fortitudo.tech.\n",
+    'long_description': ".. image:: https://github.com/fortitudo-tech/fortitudo.tech/actions/workflows/tests.yml/badge.svg\n   :target: https://github.com/fortitudo-tech/fortitudo.tech/actions/workflows/tests.yml\n\n.. image:: https://codecov.io/gh/fortitudo-tech/fortitudo.tech/graph/badge.svg?token=Z16XK92Gkl \n   :target: https://codecov.io/gh/fortitudo-tech/fortitudo.tech\n\n.. image:: https://mybinder.org/badge_logo.svg\n   :target: https://mybinder.org/v2/gh/fortitudo-tech/fortitudo.tech/main?labpath=examples\n\nFortitudo Technologies Open Source\n==================================\n\nThis package allows you to explore open-source implementations of some of our\nfundamental technologies, e.g., Entropy Pooling and CVaR optimization in Python.\nSee this `YouTube playlist <https://www.youtube.com/playlist?list=PLfI2BKNVj_b2rurUsCtc2F8lqtPWqcs2K>`_\nfor a walkthrough of the package's functionality and examples.\n\nFor a high-level introduction to the investment framework, see this `YouTube video <https://youtu.be/4ESigySdGf8>`_\nand `Medium article <https://medium.com/@ft_anvo/entropy-pooling-and-cvar-portfolio-optimization-in-python-ffed736a8347>`_.\nFor an in-depth mathematical introduction to the investment framework, see\nthese `SSRN articles <https://ssrn.com/author=2738420>`_.\n\nFor a careful and pedagogical presentation of the investment framework,\nsee the `Portfolio Construction and Risk Management Book <https://igg.me/at/pcrm-book>`_\ncrowdfunding campaign.\n\nThe package is intended for advanced users who are comfortable specifying\nportfolio constraints and Entropy Pooling views using matrices and vectors.\nThis gives full flexibility in relation to working with these technologies.\nHence, input checking is intentionally kept to a minimum.\n\nIf you like this package, we invite you to show your support by giving it a\nGitHub star. The greater the number of stars it receives, the more time and\nenergy we will invest in enhancing its functionality and providing additional\nexamples.\n\nFortitudo Technologies offers novel investment software as well as quantitative\nand digitalization consultancy to the investment management industry. For more\ninformation, please visit our `website <https://fortitudo.tech>`_.\n\nInstallation Instructions\n-------------------------\n\nInstallation can be done via pip::\n\n   pip install fortitudo.tech\n\nFor best performance, we recommend that you install the package in a `conda environment\n<https://conda.io/projects/conda/en/latest/user-guide/concepts/environments.html>`_\nand let conda handle the installation of dependencies before installing the\npackage using pip. You can do this by following these steps::\n\n   conda create -n fortitudo.tech -c conda-forge python scipy pandas matplotlib cvxopt\n   conda activate fortitudo.tech\n   pip install fortitudo.tech\n\nThe examples might require you to install additional packages, e.g., seaborn and\nipykernel / notebook / jupyterlab if you want to run the notebooks. Using pip to\ninstall these packages should not cause any dependency issues.\n\nYou can also explore the examples in the cloud without any local installations using\n`Binder <https://mybinder.org/v2/gh/fortitudo-tech/fortitudo.tech/main?labpath=examples>`_.\nHowever, note that Binder servers have very limited resources and might not support\nsome of the optimized routines this package uses. If you want access to a stable\nand optimized environment with persistent storage, please subscribe to our Data\nScience Server.\n\nDisclaimer\n----------\n\nThis package is completely separate from our proprietary solutions and therefore\nnot representative of the quality and functionality offered by the Investment Simulation\nand Investment Analysis modules. If you are an institutional investor who wants to\nexperience how these methods can be used for sophisticated analysis in practice,\nplease request a demo by sending an email to demo@fortitudo.tech.\n",
     'author': 'Fortitudo Technologies',
     'author_email': 'software@fortitudo.tech',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://fortitudo.tech',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `fortitudo_tech-1.0.5/PKG-INFO` & `fortitudo_tech-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortitudo-tech
-Version: 1.0.5
+Version: 1.0.6
 Summary: Conditional Value-at-Risk (CVaR) portfolio optimization and Entropy Pooling views / stress-testing in Python.
 Home-page: https://fortitudo.tech
 License: GPL-3.0-or-later
 Keywords: CVaR,Efficient Frontier,Entropy Pooling,Quantitative Finance,Portfolio Optimization
 Author: Fortitudo Technologies
 Author-email: software@fortitudo.tech
 Requires-Python: >=3.9,<3.13
@@ -44,20 +44,25 @@
 
 Fortitudo Technologies Open Source
 ==================================
 
 This package allows you to explore open-source implementations of some of our
 fundamental technologies, e.g., Entropy Pooling and CVaR optimization in Python.
 See this `YouTube playlist <https://www.youtube.com/playlist?list=PLfI2BKNVj_b2rurUsCtc2F8lqtPWqcs2K>`_
-for a walkthrough of the package's functionality and examples. For a high-level
-introduction to the investment framework, see this `YouTube video <https://youtu.be/4ESigySdGf8>`_
+for a walkthrough of the package's functionality and examples.
+
+For a high-level introduction to the investment framework, see this `YouTube video <https://youtu.be/4ESigySdGf8>`_
 and `Medium article <https://medium.com/@ft_anvo/entropy-pooling-and-cvar-portfolio-optimization-in-python-ffed736a8347>`_.
 For an in-depth mathematical introduction to the investment framework, see
 these `SSRN articles <https://ssrn.com/author=2738420>`_.
 
+For a careful and pedagogical presentation of the investment framework,
+see the `Portfolio Construction and Risk Management Book <https://igg.me/at/pcrm-book>`_
+crowdfunding campaign.
+
 The package is intended for advanced users who are comfortable specifying
 portfolio constraints and Entropy Pooling views using matrices and vectors.
 This gives full flexibility in relation to working with these technologies.
 Hence, input checking is intentionally kept to a minimum.
 
 If you like this package, we invite you to show your support by giving it a
 GitHub star. The greater the number of stars it receives, the more time and
```

