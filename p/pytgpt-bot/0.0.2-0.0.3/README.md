# Comparing `tmp/pytgpt-bot-0.0.2.tar.gz` & `tmp/pytgpt_bot-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytgpt-bot-0.0.2.tar", last modified: Thu Apr 25 08:16:17 2024, max compression
+gzip compressed data, was "pytgpt_bot-0.0.3.tar", last modified: Thu Apr 25 08:24:42 2024, max compression
```

## Comparing `pytgpt-bot-0.0.2.tar` & `pytgpt_bot-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 smartwa   (1000) smartwa   (1001)        0 2024-04-25 08:16:17.694173 pytgpt-bot-0.0.2/
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     1064 2024-04-24 09:24:26.000000 pytgpt-bot-0.0.2/LICENSE
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     7406 2024-04-25 08:16:17.690839 pytgpt-bot-0.0.2/PKG-INFO
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     5661 2024-04-25 08:10:25.000000 pytgpt-bot-0.0.2/README.md
-drwxr-xr-x   0 smartwa   (1000) smartwa   (1001)        0 2024-04-25 08:16:17.687506 pytgpt-bot-0.0.2/pytgpt_bot/
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)      225 2024-04-25 08:10:25.000000 pytgpt-bot-0.0.2/pytgpt_bot/__init__.py
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)       42 2024-04-25 08:10:25.000000 pytgpt-bot-0.0.2/pytgpt_bot/__main__.py
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     2195 2024-04-25 08:10:25.000000 pytgpt-bot-0.0.2/pytgpt_bot/cli.py
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)      628 2024-04-25 08:10:25.000000 pytgpt-bot-0.0.2/pytgpt_bot/config.py
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     4919 2024-04-24 13:42:16.000000 pytgpt-bot-0.0.2/pytgpt_bot/db.py
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     6529 2024-04-25 08:10:25.000000 pytgpt-bot-0.0.2/pytgpt_bot/main.py
-drwxr-xr-x   0 smartwa   (1000) smartwa   (1001)        0 2024-04-25 08:16:17.690839 pytgpt-bot-0.0.2/pytgpt_bot.egg-info/
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     7406 2024-04-25 08:16:17.000000 pytgpt-bot-0.0.2/pytgpt_bot.egg-info/PKG-INFO
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)      353 2024-04-25 08:16:17.000000 pytgpt-bot-0.0.2/pytgpt_bot.egg-info/SOURCES.txt
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)        1 2024-04-25 08:16:17.000000 pytgpt-bot-0.0.2/pytgpt_bot.egg-info/dependency_links.txt
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)       52 2024-04-25 08:16:17.000000 pytgpt-bot-0.0.2/pytgpt_bot.egg-info/entry_points.txt
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)       80 2024-04-25 08:16:17.000000 pytgpt-bot-0.0.2/pytgpt_bot.egg-info/requires.txt
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)       11 2024-04-25 08:16:17.000000 pytgpt-bot-0.0.2/pytgpt_bot.egg-info/top_level.txt
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)       38 2024-04-25 08:16:17.694173 pytgpt-bot-0.0.2/setup.cfg
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     2353 2024-04-25 08:15:12.000000 pytgpt-bot-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:24:42.259015 pytgpt_bot-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-25 08:24:26.000000 pytgpt_bot-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-04-25 08:24:42.259015 pytgpt_bot-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-04-25 08:24:26.000000 pytgpt_bot-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:24:42.259015 pytgpt_bot-0.0.3/pytgpt_bot/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-25 08:24:26.000000 pytgpt_bot-0.0.3/pytgpt_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-25 08:24:26.000000 pytgpt_bot-0.0.3/pytgpt_bot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-25 08:24:26.000000 pytgpt_bot-0.0.3/pytgpt_bot/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-25 08:24:26.000000 pytgpt_bot-0.0.3/pytgpt_bot/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-04-25 08:24:26.000000 pytgpt_bot-0.0.3/pytgpt_bot/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6529 2024-04-25 08:24:26.000000 pytgpt_bot-0.0.3/pytgpt_bot/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:24:42.259015 pytgpt_bot-0.0.3/pytgpt_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-04-25 08:24:42.000000 pytgpt_bot-0.0.3/pytgpt_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-25 08:24:42.000000 pytgpt_bot-0.0.3/pytgpt_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 08:24:42.000000 pytgpt_bot-0.0.3/pytgpt_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-25 08:24:42.000000 pytgpt_bot-0.0.3/pytgpt_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-25 08:24:42.000000 pytgpt_bot-0.0.3/pytgpt_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-25 08:24:42.000000 pytgpt_bot-0.0.3/pytgpt_bot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 08:24:42.263015 pytgpt_bot-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-25 08:24:26.000000 pytgpt_bot-0.0.3/setup.py
```

### Comparing `pytgpt-bot-0.0.2/LICENSE` & `pytgpt_bot-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytgpt-bot-0.0.2/PKG-INFO` & `pytgpt_bot-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytgpt-bot
-Version: 0.0.2
+Version: 0.0.3
 Summary: Telegram bot for text generation, text-to-image and text-to-audio conversions.
 Home-page: https://github.com/Simatwa/pytgpt-bot
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/pytgpt-bot/issues/new
@@ -31,14 +31,15 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pytelegrambotapi==4.17.0
 Requires-Dist: python-tgpt==0.6.6
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: appdirs==1.4.4
+Requires-Dist: click==8.1.3
 
 <p align="center">
 <a href="https://github.com/Simatwa/pytgpt-bot/blob/main/LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=MIT&color=Blue&message=MIT&label=License"/></a>
 <a href="#"><img alt="Python version" src="https://img.shields.io/pypi/pyversions/pytgpt"/></a>
 <a href="https://pypi.org/project/pytgpt-bot"><img alt="PyPi" src="https://img.shields.io/pypi/v/pytgpt-bot?color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/badge/code%20style-black-000000.svg"/></a>
 <a href="https://pepy.tech/project/pytgpt-bot"><img src="https://static.pepy.tech/personalized-badge/pytgpt-bot?period=total&units=international_system&left_color=grey&right_color=green&left_text=Downloads" alt="Downloads"></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.0.2 Summary: Telegram bot for
+Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.0.3 Summary: Telegram bot for
 text generation, text-to-image and text-to-audio conversions. Home-page: https:
 //github.com/Simatwa/pytgpt-bot Author: Smartwa Author-email:
 simatwacaleb@proton.me Maintainer: Smartwa License: MIT Project-URL: Bug
 Report, https://github.com/Simatwa/pytgpt-bot/issues/new Project-URL: Homepage,
 https://github.com/Simatwa/pytgpt-bot Project-URL: Source Code, https://
 github.com/Simatwa/pytgpt-bot Project-URL: Issue Tracker, https://github.com/
 Simatwa/pytgpt-bot/issues Project-URL: Download, https://github.com/Simatwa/
@@ -17,15 +17,15 @@
 Python Modules Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 pytelegrambotapi==4.17.0 Requires-Dist: python-tgpt==0.6.6 Requires-Dist:
-python-dotenv==1.0.0 Requires-Dist: appdirs==1.4.4
+python-dotenv==1.0.0 Requires-Dist: appdirs==1.4.4 Requires-Dist: click==8.1.3
 _[_L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_P_y_P_i_]_[_B_l_a_c_k_]_[_D_o_w_n_l_o_a_d_s_]_[_h_t_t_p_s_:_/_/_h_i_t_s_._s_e_e_y_o_u_f_a_r_m_._c_o_m_/
    _a_p_i_/_c_o_u_n_t_/_i_n_c_r_/_b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_/_S_i_m_a_t_w_a_/_p_y_t_g_p_t_-_b_o_t_]
                                   _[_w_a_k_a_t_i_m_e_]
                       ************ WWeellccoommee ttoo _pp_yy_tt_gg_pp_tt_--_bb_oo_tt ************
 This is a Telegram bot based on [python-tgpt](https://github.com/Simatwa/
 python-tgpt), a powerful tool designed to enhance your interactions with AI.
 This bot is built on the robust foundation of the `pyTelegramBotAPI` and offers
```

### Comparing `pytgpt-bot-0.0.2/README.md` & `pytgpt_bot-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pytgpt-bot-0.0.2/pytgpt_bot/cli.py` & `pytgpt_bot-0.0.3/pytgpt_bot/cli.py`

 * *Files identical despite different names*

### Comparing `pytgpt-bot-0.0.2/pytgpt_bot/config.py` & `pytgpt_bot-0.0.3/pytgpt_bot/config.py`

 * *Files identical despite different names*

### Comparing `pytgpt-bot-0.0.2/pytgpt_bot/db.py` & `pytgpt_bot-0.0.3/pytgpt_bot/db.py`

 * *Files identical despite different names*

### Comparing `pytgpt-bot-0.0.2/pytgpt_bot/main.py` & `pytgpt_bot-0.0.3/pytgpt_bot/main.py`

 * *Files identical despite different names*

### Comparing `pytgpt-bot-0.0.2/pytgpt_bot.egg-info/PKG-INFO` & `pytgpt_bot-0.0.3/pytgpt_bot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytgpt-bot
-Version: 0.0.2
+Version: 0.0.3
 Summary: Telegram bot for text generation, text-to-image and text-to-audio conversions.
 Home-page: https://github.com/Simatwa/pytgpt-bot
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/pytgpt-bot/issues/new
@@ -31,14 +31,15 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pytelegrambotapi==4.17.0
 Requires-Dist: python-tgpt==0.6.6
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: appdirs==1.4.4
+Requires-Dist: click==8.1.3
 
 <p align="center">
 <a href="https://github.com/Simatwa/pytgpt-bot/blob/main/LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=MIT&color=Blue&message=MIT&label=License"/></a>
 <a href="#"><img alt="Python version" src="https://img.shields.io/pypi/pyversions/pytgpt"/></a>
 <a href="https://pypi.org/project/pytgpt-bot"><img alt="PyPi" src="https://img.shields.io/pypi/v/pytgpt-bot?color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/badge/code%20style-black-000000.svg"/></a>
 <a href="https://pepy.tech/project/pytgpt-bot"><img src="https://static.pepy.tech/personalized-badge/pytgpt-bot?period=total&units=international_system&left_color=grey&right_color=green&left_text=Downloads" alt="Downloads"></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.0.2 Summary: Telegram bot for
+Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.0.3 Summary: Telegram bot for
 text generation, text-to-image and text-to-audio conversions. Home-page: https:
 //github.com/Simatwa/pytgpt-bot Author: Smartwa Author-email:
 simatwacaleb@proton.me Maintainer: Smartwa License: MIT Project-URL: Bug
 Report, https://github.com/Simatwa/pytgpt-bot/issues/new Project-URL: Homepage,
 https://github.com/Simatwa/pytgpt-bot Project-URL: Source Code, https://
 github.com/Simatwa/pytgpt-bot Project-URL: Issue Tracker, https://github.com/
 Simatwa/pytgpt-bot/issues Project-URL: Download, https://github.com/Simatwa/
@@ -17,15 +17,15 @@
 Python Modules Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 pytelegrambotapi==4.17.0 Requires-Dist: python-tgpt==0.6.6 Requires-Dist:
-python-dotenv==1.0.0 Requires-Dist: appdirs==1.4.4
+python-dotenv==1.0.0 Requires-Dist: appdirs==1.4.4 Requires-Dist: click==8.1.3
 _[_L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_P_y_P_i_]_[_B_l_a_c_k_]_[_D_o_w_n_l_o_a_d_s_]_[_h_t_t_p_s_:_/_/_h_i_t_s_._s_e_e_y_o_u_f_a_r_m_._c_o_m_/
    _a_p_i_/_c_o_u_n_t_/_i_n_c_r_/_b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_/_S_i_m_a_t_w_a_/_p_y_t_g_p_t_-_b_o_t_]
                                   _[_w_a_k_a_t_i_m_e_]
                       ************ WWeellccoommee ttoo _pp_yy_tt_gg_pp_tt_--_bb_oo_tt ************
 This is a Telegram bot based on [python-tgpt](https://github.com/Simatwa/
 python-tgpt), a powerful tool designed to enhance your interactions with AI.
 This bot is built on the robust foundation of the `pyTelegramBotAPI` and offers
```

### Comparing `pytgpt-bot-0.0.2/setup.py` & `pytgpt_bot-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     full_path: Path = ROOT_PATH / path
     return full_path.read_text(encoding="utf-8")
 
 
 setup(
     name="pytgpt-bot",
     packages=["pytgpt_bot"],
-    version="0.0.2",
+    version="0.0.3",
     license="MIT",
     author="Smartwa",
     maintainer="Smartwa",
     author_email="simatwacaleb@proton.me",
     description="Telegram bot for text generation, text-to-image and text-to-audio conversions.",
     url="https://github.com/Simatwa/pytgpt-bot",
     project_urls={
@@ -34,14 +34,15 @@
         ],
     },
     install_requires=[
         "pytelegrambotapi==4.17.0",
         "python-tgpt==0.6.6",
         "python-dotenv==1.0.0",
         "appdirs==1.4.4",
+        "click==8.1.3",
         ],
     python_requires=">=3.10",
     keywords=[
         "ai",
         "tgpt",
         "pytgpt",
         "chatbot",
```

