# Comparing `tmp/entropy_pooling-1.0.3.tar.gz` & `tmp/entropy_pooling-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "entropy_pooling-1.0.3.tar", max compression
+gzip compressed data, was "entropy_pooling-1.0.4.tar", max compression
```

## Comparing `entropy_pooling-1.0.3.tar` & `entropy_pooling-1.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1514 2024-03-14 09:34:19.430301 entropy_pooling-1.0.3/LICENSE
--rw-r--r--   0        0        0     2746 2024-03-14 09:38:49.000306 entropy_pooling-1.0.3/README.md
--rw-r--r--   0        0        0      224 2024-03-14 09:34:19.430301 entropy_pooling-1.0.3/entropy_pooling/__init__.py
--rw-r--r--   0        0        0     2583 2024-03-14 09:34:19.430301 entropy_pooling-1.0.3/entropy_pooling/entropy_pooling.py
--rw-r--r--   0        0        0     1337 2024-03-14 09:40:38.840308 entropy_pooling-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     3500 1970-01-01 00:00:00.000000 entropy_pooling-1.0.3/setup.py
--rw-r--r--   0        0        0     4172 1970-01-01 00:00:00.000000 entropy_pooling-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1514 2024-04-25 11:04:29.405725 entropy_pooling-1.0.4/LICENSE
+-rw-r--r--   0        0        0     3282 2024-04-25 11:11:07.715725 entropy_pooling-1.0.4/README.md
+-rw-r--r--   0        0        0      224 2024-04-25 11:04:29.405725 entropy_pooling-1.0.4/entropy_pooling/__init__.py
+-rw-r--r--   0        0        0     2583 2024-04-25 11:04:29.405725 entropy_pooling-1.0.4/entropy_pooling/entropy_pooling.py
+-rw-r--r--   0        0        0     1337 2024-04-25 11:11:34.995725 entropy_pooling-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4047 1970-01-01 00:00:00.000000 entropy_pooling-1.0.4/setup.py
+-rw-r--r--   0        0        0     4708 1970-01-01 00:00:00.000000 entropy_pooling-1.0.4/PKG-INFO
```

### Comparing `entropy_pooling-1.0.3/LICENSE` & `entropy_pooling-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `entropy_pooling-1.0.3/README.md` & `entropy_pooling-1.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -50,8 +50,18 @@
 
 Video walkthroughs
 ------------------
 
 Video walkthroughs of the two notebook examples are available here https://youtu.be/hDt103zEML8
 and here https://youtu.be/DK1Pv5tuLgo. The videos give additional insights into
 Entropy Pooling theory and its sequential refinements. It is highly encouraged
-to watch these two quickly increase your understanding.
+to watch these two quickly increase your understanding.
+
+Portfolio Construction and Risk Management Book
+-----------------------------------------------
+
+Entropy Pooling is a core part of the next generation investment framework that
+also utilizes fully general Monte Carlo distributions and CVaR analysis, see
+[this YouTube video](https://youtu.be/4ESigySdGf8?si) for an introduction. To
+get a careful and pedagogical presentation of all the possibilities Entropy Pooling
+offers, see the [Portfolio Construction and Risk Management Book](https://igg.me/at/pcrm-book)
+crowdfunding campaign.
```

### Comparing `entropy_pooling-1.0.3/entropy_pooling/entropy_pooling.py` & `entropy_pooling-1.0.4/entropy_pooling/entropy_pooling.py`

 * *Files identical despite different names*

### Comparing `entropy_pooling-1.0.3/pyproject.toml` & `entropy_pooling-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "entropy-pooling"
-version = "1.0.3"
+version = "1.0.4"
 description = "Entropy Pooling in Python with a BSD 3-Clause license."
 authors = ["Fortitudo Technologies <software@fortitudo.tech>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://fortitudo.tech"
 repository = "https://github.com/fortitudo-tech/entropy-pooling"
 documentation = "https://os.fortitudo.tech"
```

### Comparing `entropy_pooling-1.0.3/setup.py` & `entropy_pooling-1.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['scipy>=1.10,<2.0']
 
 setup_kwargs = {
     'name': 'entropy-pooling',
-    'version': '1.0.3',
+    'version': '1.0.4',
     'description': 'Entropy Pooling in Python with a BSD 3-Clause license.',
-    'long_description': '[![pytest](https://github.com/fortitudo-tech/entropy-pooling/actions/workflows/tests.yml/badge.svg)](https://github.com/fortitudo-tech/entropy-pooling/actions/workflows/tests.yml)\n[![codecov](https://codecov.io/gh/fortitudo-tech/entropy-pooling/graph/badge.svg?token=XGIQ78ZLDN)](https://codecov.io/gh/fortitudo-tech/entropy-pooling)\n[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/fortitudo-tech/entropy-pooling/HEAD?labpath=examples)\n\nEntropy Pooling in Python\n=========================\n\nDue to popular demand from developers, this package contains the Entropy Pooling\nimplementation from the [fortitudo.tech Python package](https://github.com/fortitudo-tech/fortitudo.tech)\nwith a more permissive BSD 3-Clause license.\n\nThis package contains only one function called ep and has minimal dependencies\nwith just scipy. See [this example](https://github.com/fortitudo-tech/entropy-pooling/blob/main/example/EntropyPooling.ipynb)\nfor how you can import and use the ep function.\n\nYou can explore the example without local installations using\n[Binder](https://mybinder.org/v2/gh/fortitudo-tech/entropy-pooling/HEAD?labpath=examples).\n\nInstallation instructions\n-------------------------\n\nInstallation can be done via pip:\n\n    pip install entropy-pooling\n\nTheory\n------\nEntropy Pooling is a powerful method for implementing subjective views and\nperforming stress-tests for fully general Monte Carlo distributions. It was first\nintroduced by [Meucci (2008)](https://ssrn.com/abstract=1213325) and refined\nwith sequential algorithms by [Vorobets (2021)](https://ssrn.com/abstract=3936392).\n\nThe original Entropy Pooling approach solves the minimum relative entropy problem\n\n$$q=\\underset{x}{\\text{argmin}}\\lbrace x^{T}\\left(\\ln x-\\ln p\\right)\\rbrace$$\n\nsubject to the constraints\n\n$$Gx\\leq h \\quad \\text{and} \\quad Ax=b.$$\n\nThe constraints matrices $A$ and $G$ contain transformations of the Monte Carlo\nsimulation that allow you to implement subjective views and stress-tests by\nchanging the joint scenario probabilities from a prior probability vector $p$\nto a posterior probability vector $q$.\n\nA useful statistic when working with Entropy Pooling is the effective number of\nscenarios introduced by [Meucci (2012)](https://ssrn.com/abstract=1971808). For\na causal Bayesian nets overlay on top of Entropy Pooling, see\n[Vorobets (2023)](https://ssrn.com/abstract=4444291).\n\nVideo walkthroughs\n------------------\n\nVideo walkthroughs of the two notebook examples are available here https://youtu.be/hDt103zEML8\nand here https://youtu.be/DK1Pv5tuLgo. The videos give additional insights into\nEntropy Pooling theory and its sequential refinements. It is highly encouraged\nto watch these two quickly increase your understanding.',
+    'long_description': '[![pytest](https://github.com/fortitudo-tech/entropy-pooling/actions/workflows/tests.yml/badge.svg)](https://github.com/fortitudo-tech/entropy-pooling/actions/workflows/tests.yml)\n[![codecov](https://codecov.io/gh/fortitudo-tech/entropy-pooling/graph/badge.svg?token=XGIQ78ZLDN)](https://codecov.io/gh/fortitudo-tech/entropy-pooling)\n[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/fortitudo-tech/entropy-pooling/HEAD?labpath=examples)\n\nEntropy Pooling in Python\n=========================\n\nDue to popular demand from developers, this package contains the Entropy Pooling\nimplementation from the [fortitudo.tech Python package](https://github.com/fortitudo-tech/fortitudo.tech)\nwith a more permissive BSD 3-Clause license.\n\nThis package contains only one function called ep and has minimal dependencies\nwith just scipy. See [this example](https://github.com/fortitudo-tech/entropy-pooling/blob/main/example/EntropyPooling.ipynb)\nfor how you can import and use the ep function.\n\nYou can explore the example without local installations using\n[Binder](https://mybinder.org/v2/gh/fortitudo-tech/entropy-pooling/HEAD?labpath=examples).\n\nInstallation instructions\n-------------------------\n\nInstallation can be done via pip:\n\n    pip install entropy-pooling\n\nTheory\n------\nEntropy Pooling is a powerful method for implementing subjective views and\nperforming stress-tests for fully general Monte Carlo distributions. It was first\nintroduced by [Meucci (2008)](https://ssrn.com/abstract=1213325) and refined\nwith sequential algorithms by [Vorobets (2021)](https://ssrn.com/abstract=3936392).\n\nThe original Entropy Pooling approach solves the minimum relative entropy problem\n\n$$q=\\underset{x}{\\text{argmin}}\\lbrace x^{T}\\left(\\ln x-\\ln p\\right)\\rbrace$$\n\nsubject to the constraints\n\n$$Gx\\leq h \\quad \\text{and} \\quad Ax=b.$$\n\nThe constraints matrices $A$ and $G$ contain transformations of the Monte Carlo\nsimulation that allow you to implement subjective views and stress-tests by\nchanging the joint scenario probabilities from a prior probability vector $p$\nto a posterior probability vector $q$.\n\nA useful statistic when working with Entropy Pooling is the effective number of\nscenarios introduced by [Meucci (2012)](https://ssrn.com/abstract=1971808). For\na causal Bayesian nets overlay on top of Entropy Pooling, see\n[Vorobets (2023)](https://ssrn.com/abstract=4444291).\n\nVideo walkthroughs\n------------------\n\nVideo walkthroughs of the two notebook examples are available here https://youtu.be/hDt103zEML8\nand here https://youtu.be/DK1Pv5tuLgo. The videos give additional insights into\nEntropy Pooling theory and its sequential refinements. It is highly encouraged\nto watch these two quickly increase your understanding.\n\nPortfolio Construction and Risk Management Book\n-----------------------------------------------\n\nEntropy Pooling is a core part of the next generation investment framework that\nalso utilizes fully general Monte Carlo distributions and CVaR analysis, see\n[this YouTube video](https://youtu.be/4ESigySdGf8?si) for an introduction. To\nget a careful and pedagogical presentation of all the possibilities Entropy Pooling\noffers, see the [Portfolio Construction and Risk Management Book](https://igg.me/at/pcrm-book)\ncrowdfunding campaign.\n',
     'author': 'Fortitudo Technologies',
     'author_email': 'software@fortitudo.tech',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://fortitudo.tech',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `entropy_pooling-1.0.3/PKG-INFO` & `entropy_pooling-1.0.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: entropy-pooling
-Version: 1.0.3
+Version: 1.0.4
 Summary: Entropy Pooling in Python with a BSD 3-Clause license.
 Home-page: https://fortitudo.tech
 License: BSD-3-Clause
 Keywords: Entropy Pooling,Quantitative Finance,Monte Carlo,Stress-Testing,CVaR
 Author: Fortitudo Technologies
 Author-email: software@fortitudo.tech
 Requires-Python: >=3.9,<3.13
@@ -82,7 +82,18 @@
 Video walkthroughs
 ------------------
 
 Video walkthroughs of the two notebook examples are available here https://youtu.be/hDt103zEML8
 and here https://youtu.be/DK1Pv5tuLgo. The videos give additional insights into
 Entropy Pooling theory and its sequential refinements. It is highly encouraged
 to watch these two quickly increase your understanding.
+
+Portfolio Construction and Risk Management Book
+-----------------------------------------------
+
+Entropy Pooling is a core part of the next generation investment framework that
+also utilizes fully general Monte Carlo distributions and CVaR analysis, see
+[this YouTube video](https://youtu.be/4ESigySdGf8?si) for an introduction. To
+get a careful and pedagogical presentation of all the possibilities Entropy Pooling
+offers, see the [Portfolio Construction and Risk Management Book](https://igg.me/at/pcrm-book)
+crowdfunding campaign.
+
```

