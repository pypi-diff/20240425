# Comparing `tmp/lg-rez-4.0.2.tar.gz` & `tmp/lg_rez-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lg-rez-4.0.2.tar", last modified: Wed Mar 20 16:41:48 2024, max compression
+gzip compressed data, was "lg_rez-4.0.3.tar", last modified: Thu Apr 25 12:48:14 2024, max compression
```

## Comparing `lg-rez-4.0.2.tar` & `lg_rez-4.0.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:41:48.043823 lg-rez-4.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-03-20 16:41:39.000000 lg-rez-4.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9601 2024-03-20 16:41:48.039823 lg-rez-4.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6893 2024-03-20 16:41:39.000000 lg-rez-4.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:41:48.039823 lg-rez-4.0.2/lg_rez.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9601 2024-03-20 16:41:47.000000 lg-rez-4.0.2/lg_rez.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-03-20 16:41:48.000000 lg-rez-4.0.2/lg_rez.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 16:41:47.000000 lg-rez-4.0.2/lg_rez.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-03-20 16:41:47.000000 lg-rez-4.0.2/lg_rez.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-20 16:41:47.000000 lg-rez-4.0.2/lg_rez.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:41:48.035823 lg-rez-4.0.2/lgrez/
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-03-20 16:41:39.000000 lg-rez-4.0.2/lgrez/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14782 2024-03-20 16:41:39.000000 lg-rez-4.0.2/lgrez/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:41:48.035823 lg-rez-4.0.2/lgrez/bdd/
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-03-20 16:41:39.000000 lg-rez-4.0.2/lgrez/bdd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20725 2024-03-20 16:41:39.000000 lg-rez-4.0.2/lgrez/bdd/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-03-20 16:41:39.000000 lg-rez-4.0.2/lgrez/bdd/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)    25186 2024-03-20 16:41:39.000000 lg-rez-4.0.2/lgrez/bdd/model_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-03-20 16:41:39.000000 lg-rez-4.0.2/lgrez/bdd/model_ia.py
--rw-r--r--   0 runner    (1001) docker     (127)    18526 2024-03-20 16:41:39.000000 lg-rez-4.0.2/lgrez/bdd/model_jeu.py
--rw-r--r--   0 runner    (1001) docker     (127)    14516 2024-03-20 16:41:39.000000 lg-rez-4.0.2/lgrez/bdd/model_joueurs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:41:48.035823 lg-rez-4.0.2/lgrez/blocs/
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-03-20 16:41:39.000000 lg-rez-4.0.2/lgrez/blocs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-03-20 16:41:39.000000 lg-rez-4.0.2/lgrez/blocs/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-03-20 16:41:39.000000 lg-rez-4.0.2/lgrez/blocs/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     8951 2024-03-20 16:41:39.000000 lg-rez-4.0.2/lgrez/blocs/gsheets.py
--rw-r--r--   0 runner    (1001) docker     (127)    20325 2024-03-20 16:41:39.000000 lg-rez-4.0.2/lgrez/blocs/journey.py
--rw-r--r--   0 runner    (1001) docker     (127)    11831 2024-03-20 16:41:39.000000 lg-rez-4.0.2/lgrez/blocs/realshell.py
--rw-r--r--   0 runner    (1001) docker     (127)    10152 2024-03-20 16:41:39.000000 lg-rez-4.0.2/lgrez/blocs/structure.py
--rw-r--r--   0 runner    (1001) docker     (127)    44961 2024-03-20 16:41:39.000000 lg-rez-4.0.2/lgrez/blocs/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    15987 2024-03-20 16:41:39.000000 lg-rez-4.0.2/lgrez/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-03-20 16:41:39.000000 lg-rez-4.0.2/lgrez/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-03-20 16:41:39.000000 lg-rez-4.0.2/lgrez/commons.py
--rw-r--r--   0 runner    (1001) docker     (127)    14222 2024-03-20 16:41:39.000000 lg-rez-4.0.2/lgrez/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:41:48.039823 lg-rez-4.0.2/lgrez/features/
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-03-20 16:41:39.000000 lg-rez-4.0.2/lgrez/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11824 2024-03-20 16:41:39.000000 lg-rez-4.0.2/lgrez/features/actions_publiques.py
--rw-r--r--   0 runner    (1001) docker     (127)     8503 2024-03-20 16:41:39.000000 lg-rez-4.0.2/lgrez/features/annexe.py
--rw-r--r--   0 runner    (1001) docker     (127)    18513 2024-03-20 16:41:39.000000 lg-rez-4.0.2/lgrez/features/chans.py
--rw-r--r--   0 runner    (1001) docker     (127)    22082 2024-03-20 16:41:39.000000 lg-rez-4.0.2/lgrez/features/communication.py
--rw-r--r--   0 runner    (1001) docker     (127)    11267 2024-03-20 16:41:39.000000 lg-rez-4.0.2/lgrez/features/gestion_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)    23562 2024-03-20 16:41:39.000000 lg-rez-4.0.2/lgrez/features/gestion_ia.py
--rw-r--r--   0 runner    (1001) docker     (127)    13722 2024-03-20 16:41:39.000000 lg-rez-4.0.2/lgrez/features/informations.py
--rw-r--r--   0 runner    (1001) docker     (127)    12238 2024-03-20 16:41:39.000000 lg-rez-4.0.2/lgrez/features/inscription.py
--rw-r--r--   0 runner    (1001) docker     (127)    27484 2024-03-20 16:41:39.000000 lg-rez-4.0.2/lgrez/features/open_close.py
--rw-r--r--   0 runner    (1001) docker     (127)    14238 2024-03-20 16:41:39.000000 lg-rez-4.0.2/lgrez/features/special.py
--rw-r--r--   0 runner    (1001) docker     (127)    33108 2024-03-20 16:41:39.000000 lg-rez-4.0.2/lgrez/features/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     6565 2024-03-20 16:41:39.000000 lg-rez-4.0.2/lgrez/features/taches.py
--rw-r--r--   0 runner    (1001) docker     (127)    18863 2024-03-20 16:41:39.000000 lg-rez-4.0.2/lgrez/features/voter_agir.py
--rw-r--r--   0 runner    (1001) docker     (127)     9704 2024-03-20 16:41:39.000000 lg-rez-4.0.2/lgrez/server_structure.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 16:41:48.043823 lg-rez-4.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-03-20 16:41:39.000000 lg-rez-4.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:48:14.793448 lg_rez-4.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-25 12:48:03.000000 lg_rez-4.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9601 2024-04-25 12:48:14.793448 lg_rez-4.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6893 2024-04-25 12:48:03.000000 lg_rez-4.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:48:14.793448 lg_rez-4.0.3/lg_rez.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9601 2024-04-25 12:48:14.000000 lg_rez-4.0.3/lg_rez.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-25 12:48:14.000000 lg_rez-4.0.3/lg_rez.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 12:48:14.000000 lg_rez-4.0.3/lg_rez.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-25 12:48:14.000000 lg_rez-4.0.3/lg_rez.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-25 12:48:14.000000 lg_rez-4.0.3/lg_rez.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:48:14.789447 lg_rez-4.0.3/lgrez/
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-25 12:48:03.000000 lg_rez-4.0.3/lgrez/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14925 2024-04-25 12:48:03.000000 lg_rez-4.0.3/lgrez/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:48:14.789447 lg_rez-4.0.3/lgrez/bdd/
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-25 12:48:03.000000 lg_rez-4.0.3/lgrez/bdd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20725 2024-04-25 12:48:03.000000 lg_rez-4.0.3/lgrez/bdd/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-04-25 12:48:03.000000 lg_rez-4.0.3/lgrez/bdd/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25186 2024-04-25 12:48:03.000000 lg_rez-4.0.3/lgrez/bdd/model_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-25 12:48:03.000000 lg_rez-4.0.3/lgrez/bdd/model_ia.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18526 2024-04-25 12:48:03.000000 lg_rez-4.0.3/lgrez/bdd/model_jeu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14516 2024-04-25 12:48:03.000000 lg_rez-4.0.3/lgrez/bdd/model_joueurs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:48:14.789447 lg_rez-4.0.3/lgrez/blocs/
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-25 12:48:03.000000 lg_rez-4.0.3/lgrez/blocs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-04-25 12:48:03.000000 lg_rez-4.0.3/lgrez/blocs/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-25 12:48:03.000000 lg_rez-4.0.3/lgrez/blocs/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8951 2024-04-25 12:48:03.000000 lg_rez-4.0.3/lgrez/blocs/gsheets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20325 2024-04-25 12:48:03.000000 lg_rez-4.0.3/lgrez/blocs/journey.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11831 2024-04-25 12:48:03.000000 lg_rez-4.0.3/lgrez/blocs/realshell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10152 2024-04-25 12:48:03.000000 lg_rez-4.0.3/lgrez/blocs/structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44961 2024-04-25 12:48:03.000000 lg_rez-4.0.3/lgrez/blocs/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16005 2024-04-25 12:48:03.000000 lg_rez-4.0.3/lgrez/bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8565 2024-04-25 12:48:03.000000 lg_rez-4.0.3/lgrez/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-25 12:48:03.000000 lg_rez-4.0.3/lgrez/commons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14304 2024-04-25 12:48:03.000000 lg_rez-4.0.3/lgrez/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:48:14.793448 lg_rez-4.0.3/lgrez/features/
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-25 12:48:03.000000 lg_rez-4.0.3/lgrez/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-04-25 12:48:03.000000 lg_rez-4.0.3/lgrez/features/actions_publiques.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8509 2024-04-25 12:48:03.000000 lg_rez-4.0.3/lgrez/features/annexe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18513 2024-04-25 12:48:03.000000 lg_rez-4.0.3/lgrez/features/chans.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22506 2024-04-25 12:48:03.000000 lg_rez-4.0.3/lgrez/features/communication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11267 2024-04-25 12:48:03.000000 lg_rez-4.0.3/lgrez/features/gestion_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23562 2024-04-25 12:48:03.000000 lg_rez-4.0.3/lgrez/features/gestion_ia.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13722 2024-04-25 12:48:03.000000 lg_rez-4.0.3/lgrez/features/informations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12238 2024-04-25 12:48:03.000000 lg_rez-4.0.3/lgrez/features/inscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27484 2024-04-25 12:48:03.000000 lg_rez-4.0.3/lgrez/features/open_close.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14238 2024-04-25 12:48:03.000000 lg_rez-4.0.3/lgrez/features/special.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33108 2024-04-25 12:48:03.000000 lg_rez-4.0.3/lgrez/features/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6565 2024-04-25 12:48:03.000000 lg_rez-4.0.3/lgrez/features/taches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18863 2024-04-25 12:48:03.000000 lg_rez-4.0.3/lgrez/features/voter_agir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9704 2024-04-25 12:48:03.000000 lg_rez-4.0.3/lgrez/server_structure.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 12:48:14.793448 lg_rez-4.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-25 12:48:03.000000 lg_rez-4.0.3/setup.py
```

### Comparing `lg-rez-4.0.2/LICENSE` & `lg_rez-4.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lg-rez-4.0.2/PKG-INFO` & `lg_rez-4.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lg-rez
-Version: 4.0.2
+Version: 4.0.3
 Summary: Discord bot for organizing Werewolf RP games ESPCI-style
 Home-page: https://github.com/GRI-ESPCI/lg-rez
 Author: Loïc Simon, Tom Lacoma
 Author-email: loic.simon@espci.org, tom.lacoma@espci.org
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
@@ -89,20 +89,20 @@
 
 
 ## NOTE AUX GRIS / MJS
 
 Tout ce qui suit est du blabla READMEsque peu intéressant.
 
 Pour les trucs intéressants, c'est-à-dire les instructions pour lancer une 
-nouvelle saison, voir [`Nouvelle saison.md`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.2/Nouvelle%20saison.md).
+nouvelle saison, voir [`Nouvelle saison.md`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.3/Nouvelle%20saison.md).
 
 
 ## What's New in LG-Rez
 
-Only major features are reported here; see [`CHANGELOG.md`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.2/CHANGELOG.md)
+Only major features are reported here; see [`CHANGELOG.md`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.3/CHANGELOG.md)
 or in [the doc](https://lg-rez.readthedocs.io/fr/2.4.2/changelog.html) for
 details.
 
 # 3.0
 
 * Changed all commands to Discord builtin slash commands, using Discordpy 2.0
 * Several major commands changes
@@ -144,28 +144,28 @@
 We strongly recommand to install this package in a dedicated virtualenv
 (`python3 -m venv <yourfolder>`).
 
 
 ### Dependencies
 
 * Python 3.10+
-* Packages: see [`requirements.txt`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.2/requirements.txt)
+* Packages: see [`requirements.txt`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.3/requirements.txt)
 
 
 
 ## Configuration
 
 To run correctly, the bot needs to be connected to several external services,
 each needing more or less sensitive tokens, stocked as environments variables.
 We support and encourage the use of
 [`python-dotenv`](https://pypi.org/project/python-dotenv/) to read them from
 a `.env` file, but you may prefer exporting them as environment variables.
 
 All necessary variables, prefixed by `LGREZ_`, are listed in
-[`model.env`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.2/model.env).
+[`model.env`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.3/model.env).
 
 
 ### Configuration Assistant Tool
 
 We provide a command-line assistant tool to help you set up every services and
 generate the `.env` file (which you can later `source` and delete if you wish).
 
@@ -178,15 +178,15 @@
 needed to run the bot (see *Usage* section below).
 
 
 ### Manual configuration
 
 You may prefer to manually write your environment variables, or just check
 instructions regarding a specific one: they can be found in
-[`CONFIGURE.md`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.2/CONFIGURE.md).
+[`CONFIGURE.md`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.3/CONFIGURE.md).
 
 **Warning**: the Configuration Assistant Tool checks every variable by
 running specific tests, which is not the case for manual configuration,
 so be sure of what you do!
 
 
 
@@ -221,15 +221,15 @@
 
 Since `LGBot` is a subclass of
 [`discord.ext.commands.Bot`](https://discordpy.readthedocs.io/en/latest/ext/commands/api.html#bot),
 you can use every arguments and methods it supports or subclass it to override
 existing behavior.
 
 We also provide a direct way to customize some parameters of the game and
-of the Discord server through [`config`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.2/lgrez/config.py) module:
+of the Discord server through [`config`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.3/lgrez/config.py) module:
 roles/channels/emoji names, date of season beginning, inscription
 customization... See
 [the doc](https://lg-rez.readthedocs.io/fr/2.4.2/config.html)
 for full API usage information.
 
 See additional attributes and overriden methods on
 [the doc](https://lg-rez.readthedocs.io/) (mostly in French)
@@ -306,15 +306,15 @@
 
 Community contributions are not welcome for now. Get in touch with the authors
 (see below) for any question or suggestion about this project.
 
 
 
 ## License
-This work is shared under [the MIT license](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.2/LICENSE).
+This work is shared under [the MIT license](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.3/LICENSE).
 
 © 2020 - 2022 Loïc Simon, Tom Lacoma et al. – Club BD-Jeux × GRIs –
 ESPCI Paris - PSL
 
 Reach us on Discord:
 [LaCarpe#1674](https://discordapp.com/users/264482202966818825),
 [TaupeOrAfk#3218](https://discordapp.com/users/176763552202358785) or by mail: [loic.simon@espci.org](mailto:loic.simon@espci.org),
```

### Comparing `lg-rez-4.0.2/README.md` & `lg_rez-4.0.3/README.md`

 * *Files identical despite different names*

### Comparing `lg-rez-4.0.2/lg_rez.egg-info/PKG-INFO` & `lg_rez-4.0.3/lg_rez.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lg-rez
-Version: 4.0.2
+Version: 4.0.3
 Summary: Discord bot for organizing Werewolf RP games ESPCI-style
 Home-page: https://github.com/GRI-ESPCI/lg-rez
 Author: Loïc Simon, Tom Lacoma
 Author-email: loic.simon@espci.org, tom.lacoma@espci.org
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
@@ -89,20 +89,20 @@
 
 
 ## NOTE AUX GRIS / MJS
 
 Tout ce qui suit est du blabla READMEsque peu intéressant.
 
 Pour les trucs intéressants, c'est-à-dire les instructions pour lancer une 
-nouvelle saison, voir [`Nouvelle saison.md`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.2/Nouvelle%20saison.md).
+nouvelle saison, voir [`Nouvelle saison.md`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.3/Nouvelle%20saison.md).
 
 
 ## What's New in LG-Rez
 
-Only major features are reported here; see [`CHANGELOG.md`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.2/CHANGELOG.md)
+Only major features are reported here; see [`CHANGELOG.md`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.3/CHANGELOG.md)
 or in [the doc](https://lg-rez.readthedocs.io/fr/2.4.2/changelog.html) for
 details.
 
 # 3.0
 
 * Changed all commands to Discord builtin slash commands, using Discordpy 2.0
 * Several major commands changes
@@ -144,28 +144,28 @@
 We strongly recommand to install this package in a dedicated virtualenv
 (`python3 -m venv <yourfolder>`).
 
 
 ### Dependencies
 
 * Python 3.10+
-* Packages: see [`requirements.txt`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.2/requirements.txt)
+* Packages: see [`requirements.txt`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.3/requirements.txt)
 
 
 
 ## Configuration
 
 To run correctly, the bot needs to be connected to several external services,
 each needing more or less sensitive tokens, stocked as environments variables.
 We support and encourage the use of
 [`python-dotenv`](https://pypi.org/project/python-dotenv/) to read them from
 a `.env` file, but you may prefer exporting them as environment variables.
 
 All necessary variables, prefixed by `LGREZ_`, are listed in
-[`model.env`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.2/model.env).
+[`model.env`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.3/model.env).
 
 
 ### Configuration Assistant Tool
 
 We provide a command-line assistant tool to help you set up every services and
 generate the `.env` file (which you can later `source` and delete if you wish).
 
@@ -178,15 +178,15 @@
 needed to run the bot (see *Usage* section below).
 
 
 ### Manual configuration
 
 You may prefer to manually write your environment variables, or just check
 instructions regarding a specific one: they can be found in
-[`CONFIGURE.md`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.2/CONFIGURE.md).
+[`CONFIGURE.md`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.3/CONFIGURE.md).
 
 **Warning**: the Configuration Assistant Tool checks every variable by
 running specific tests, which is not the case for manual configuration,
 so be sure of what you do!
 
 
 
@@ -221,15 +221,15 @@
 
 Since `LGBot` is a subclass of
 [`discord.ext.commands.Bot`](https://discordpy.readthedocs.io/en/latest/ext/commands/api.html#bot),
 you can use every arguments and methods it supports or subclass it to override
 existing behavior.
 
 We also provide a direct way to customize some parameters of the game and
-of the Discord server through [`config`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.2/lgrez/config.py) module:
+of the Discord server through [`config`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.3/lgrez/config.py) module:
 roles/channels/emoji names, date of season beginning, inscription
 customization... See
 [the doc](https://lg-rez.readthedocs.io/fr/2.4.2/config.html)
 for full API usage information.
 
 See additional attributes and overriden methods on
 [the doc](https://lg-rez.readthedocs.io/) (mostly in French)
@@ -306,15 +306,15 @@
 
 Community contributions are not welcome for now. Get in touch with the authors
 (see below) for any question or suggestion about this project.
 
 
 
 ## License
-This work is shared under [the MIT license](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.2/LICENSE).
+This work is shared under [the MIT license](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.3/LICENSE).
 
 © 2020 - 2022 Loïc Simon, Tom Lacoma et al. – Club BD-Jeux × GRIs –
 ESPCI Paris - PSL
 
 Reach us on Discord:
 [LaCarpe#1674](https://discordapp.com/users/264482202966818825),
 [TaupeOrAfk#3218](https://discordapp.com/users/176763552202358785) or by mail: [loic.simon@espci.org](mailto:loic.simon@espci.org),
```

### Comparing `lg-rez-4.0.2/lg_rez.egg-info/SOURCES.txt` & `lg_rez-4.0.3/lg_rez.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lg-rez-4.0.2/lg_rez.egg-info/requires.txt` & `lg_rez-4.0.3/lg_rez.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `lg-rez-4.0.2/lgrez/__main__.py` & `lg_rez-4.0.3/lgrez/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,23 +175,24 @@
     )
 
     ok = False
     while not ok:
         LGREZ_DISCORD_TOKEN = input("Discord client secret: ")
 
         print("Testing connection...")
-        client = discord.Client()
+        intents=discord.Intents.all()
+        client = discord.Client(intents=intents)
         loop = asyncio.new_event_loop()
         try:
             loop.run_until_complete(client.login(LGREZ_DISCORD_TOKEN))
         except Exception as e:
             report_error(e)
         else:
             print("Connected!")
-            loop.run_until_complete(client.logout())
+            loop.run_until_complete(client.close())
             ok = True
             time.sleep(1)
         finally:
             loop.close()
 
     with open(".env", "a") as fich:
         fich.write("\n\n# -- Discord\n\n" + export("LGREZ_DISCORD_TOKEN"))
@@ -209,16 +210,16 @@
     )
 
     ok = False
     while not ok:
         LGREZ_SERVER_ID = input("Server ID (Server settings / Widget): ")
 
         try:
-            if not (LGREZ_SERVER_ID.isdigit() and len(LGREZ_SERVER_ID) == 18):
-                raise ValueError("Server ID must be a 18-digits number")
+            if not (LGREZ_SERVER_ID.isdigit() and (len(LGREZ_SERVER_ID) == 18 or len(LGREZ_SERVER_ID) == 19 )):
+                raise ValueError("Server ID must be a 18 or 19-digits number")
         except Exception as e:
             report_error(e)
         else:
             ok = True
             time.sleep(1)
 
     with open(".env", "a") as fich:
@@ -272,14 +273,15 @@
     )
 
     ok = False
     while not ok:
         LGREZ_GCP_CREDENTIALS = input("JSON key (one-line file contents): ")
 
         print("Authentificating...")
+        print(json.loads(LGREZ_GCP_CREDENTIALS))
         try:
             scope = ["https://spreadsheets.google.com/feeds"]
             with warnings.catch_warnings(record=True) as warns:
                 creds = ServiceAccountCredentials.from_json_keyfile_dict(json.loads(LGREZ_GCP_CREDENTIALS), scope)
                 client = gspread.Client(creds)
                 if warns:
                     raise RuntimeError(warns[0].message)
@@ -432,15 +434,15 @@
 The bot execution is quiet, except at startup and if an exception
 occurs, so we advise you to log the output stream somewhere!
 We also advise you to use an external script to ensure the bot has
 not crashed -- pretty unlikely, but it might always happen; see also
 "output_liveness" customization option in the docs:
 https://lg-rez.readthedocs.io/fr/2.0.0/config.html#lgrez.config.output_liveness
 
-You can no try to interact with the bot!
+You can now try to interact with the bot!
 (For your first tests, note that the bot ignore every messages posted by
 a member without any role! Assign yourself the "MJ" role to get full
 rights with the bot.)
 
 Do not hesitate to reach us for any issue or suggestion, we're always
 happy to get news. See bottom of README for contacts.
```

### Comparing `lg-rez-4.0.2/lgrez/bdd/__init__.py` & `lg_rez-4.0.3/lgrez/bdd/__init__.py`

 * *Files identical despite different names*

### Comparing `lg-rez-4.0.2/lgrez/bdd/base.py` & `lg_rez-4.0.3/lgrez/bdd/base.py`

 * *Files identical despite different names*

### Comparing `lg-rez-4.0.2/lgrez/bdd/enums.py` & `lg_rez-4.0.3/lgrez/bdd/enums.py`

 * *Files identical despite different names*

### Comparing `lg-rez-4.0.2/lgrez/bdd/model_actions.py` & `lg_rez-4.0.3/lgrez/bdd/model_actions.py`

 * *Files identical despite different names*

### Comparing `lg-rez-4.0.2/lgrez/bdd/model_ia.py` & `lg_rez-4.0.3/lgrez/bdd/model_ia.py`

 * *Files identical despite different names*

### Comparing `lg-rez-4.0.2/lgrez/bdd/model_jeu.py` & `lg_rez-4.0.3/lgrez/bdd/model_jeu.py`

 * *Files identical despite different names*

### Comparing `lg-rez-4.0.2/lgrez/bdd/model_joueurs.py` & `lg_rez-4.0.3/lgrez/bdd/model_joueurs.py`

 * *Files identical despite different names*

### Comparing `lg-rez-4.0.2/lgrez/blocs/__init__.py` & `lg_rez-4.0.3/lgrez/blocs/__init__.py`

 * *Files identical despite different names*

### Comparing `lg-rez-4.0.2/lgrez/blocs/console.py` & `lg_rez-4.0.3/lgrez/blocs/console.py`

 * *Files identical despite different names*

### Comparing `lg-rez-4.0.2/lgrez/blocs/env.py` & `lg_rez-4.0.3/lgrez/blocs/env.py`

 * *Files identical despite different names*

### Comparing `lg-rez-4.0.2/lgrez/blocs/gsheets.py` & `lg_rez-4.0.3/lgrez/blocs/gsheets.py`

 * *Files identical despite different names*

### Comparing `lg-rez-4.0.2/lgrez/blocs/journey.py` & `lg_rez-4.0.3/lgrez/blocs/journey.py`

 * *Files identical despite different names*

### Comparing `lg-rez-4.0.2/lgrez/blocs/realshell.py` & `lg_rez-4.0.3/lgrez/blocs/realshell.py`

 * *Files identical despite different names*

### Comparing `lg-rez-4.0.2/lgrez/blocs/structure.py` & `lg_rez-4.0.3/lgrez/blocs/structure.py`

 * *Files identical despite different names*

### Comparing `lg-rez-4.0.2/lgrez/blocs/tools.py` & `lg_rez-4.0.3/lgrez/blocs/tools.py`

 * *Files identical despite different names*

### Comparing `lg-rez-4.0.2/lgrez/bot.py` & `lg_rez-4.0.3/lgrez/bot.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,17 +16,18 @@
 
 from lgrez import __version__, commands, config, bdd
 from lgrez.blocs import env, tools, console
 from lgrez.features import gestion_ia, inscription
 
 
 async def _check_and_prepare_objects(bot: LGBot) -> None:
+        
     if not config.is_setup:
         return
-
+        
     if len(config.guild.channels) < 20:
         config.is_setup = False
         # *really* needed objects, even if nothing is setup
         config.Channel.logs = config.guild.text_channels[0]
         await tools.log("Server not setup - call `/setup` !")
         config.bot.tree.enable_command("setup")
         await config.bot.tree.sync(guild=config.guild)
```

### Comparing `lg-rez-4.0.2/lgrez/commands.py` & `lg_rez-4.0.3/lgrez/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
         # Commandes désactivées de base
         # self.disable_command("vote")
         # self.disable_command("votemaire")
         # self.disable_command("voteloups")
         # self.disable_command("haro")
         # self.disable_command("candid")
-        self.disable_command("setup")
+        # self.disable_command("setup")
 
     def _add_module_commands(self, module: types.ModuleType) -> None:
         for name, value in inspect.getmembers(module):
             if isinstance(value, (app_commands.Command, app_commands.Group)):
                 self.add_and_enable_command(value)
 
             if isinstance(value, app_commands.ContextMenu):
```

### Comparing `lg-rez-4.0.2/lgrez/config.py` & `lg_rez-4.0.3/lgrez/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,17 +139,19 @@
 #: de modifier un vote (rôle de l'*Intrigant* dans le jeu PCéen).
 #: Cette baseaction doit avoir deux ciblages de slugs "cible" et "vote".
 modif_vote_baseaction: str = "modification-vote"
 
 #: :attr:`.bdd.BaseAction.slug` de l'action de base permettant
 #: d'ajouter un/des vote(s) (rôle du *Corbeau* dans le jeu PCéen).
 ajout_vote_baseaction: str = "ajout-vote"
+ajout_vote__impr_baseaction: str = "dépôt-affiche"
 
 #: Nombre de votes ajoutés par l'action :attr:`ajout_vote_baseaction`.
 n_ajouts_votes: int = 2
+n_ajouts_votes_impr: int = 1
 
 
 #: Nom de la feuille du GSheet *Données brûtes* où enregistrer
 #: les votes brutes pour le condamné du jour.
 db_votecond_sheet: str = "votecond_brut"
 
 #: Nom de la feuille du GSheet *Données brûtes* où enregistrer
```

### Comparing `lg-rez-4.0.2/lgrez/features/__init__.py` & `lg_rez-4.0.3/lgrez/features/__init__.py`

 * *Files identical despite different names*

### Comparing `lg-rez-4.0.2/lgrez/features/actions_publiques.py` & `lg_rez-4.0.3/lgrez/features/actions_publiques.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
             raise error
 
     haro_message = await config.Channel.haros.send(
         f"(Psst, {joueur.member.mention} :3)", embed=emb, view=_HaroView(timeout=None)
     )
     await config.Channel.debats.send(
         f"{config.Emoji.ha}{config.Emoji.ro} de {journey.member.mention} sur {joueur.member.mention} ! "
-        f"Vous en pensez quoi vous ? (détails sur {config.Channel.haros.mention})"
+        f"Vous en pensez quoi vous? (détails sur {config.Channel.haros.mention})"
     )
 
     haro = CandidHaro(joueur=joueur, type=CandidHaroType.haro, message_id=haro_message.id)
     contre_haro = CandidHaro(joueur=moi, type=CandidHaroType.haro)
     CandidHaro.add(haro, contre_haro)
 
     if journey.channel != config.Channel.haros:
@@ -212,37 +212,50 @@
     for candid_haro in candid_haros:
         await candid_haro.disable_message_buttons()
     CandidHaro.delete(*candid_haros)
 
     await journey.send("Fait.")
     await tools.log(f"/wipe : {len(candid_haros)} {quoi} supprimés")
  
- 
- 
-  
+
+@app_commands.command()
+@tools.mjs_only
+@journey_command
+async def imprimeur(journey: DiscordJourney, *, joueur: app_commands.Transform[Joueur, tools.VivantTransformer]):
+    """Lance publiquement un haro contre la personne visée par l'imprimeur. (COMMANDE MJ)
+
+    Args:
+        joueur: Le joueur ou la joueuse à accuser de tous les maux.
+
+    Cette commande n'est utilisable que lorsqu'un vote pour le condamné est en cours.
+    """
+    await _imprimeur(journey, joueur=joueur)
+
 async def _imprimeur(journey: DiscordJourney, joueur: Joueur):
     try:
         vaction = joueur.action_vote(Vote.cond)
     except RuntimeError:
         await journey.send(":x: Minute papillon, le jeu n'est pas encore lancé !")
         return
 
     if not vaction.is_open:
         await journey.send(":x: Pas de vote pour le condamné du jour en cours !")
         return
 
     (motif,) = await journey.modal(
-        f"Accusation contre {joueur.nom}",
+        f"Haro contre {joueur.nom}",
+        discord.ui.TextInput(label="Quelle est la raison de cette haine ?", style=discord.TextStyle.paragraph),
     )
 
     emb = discord.Embed(
         title=(f"**{config.Emoji.ha}{config.Emoji.ro} contre {joueur.nom} !**"),
+        description=f"**« {motif} »\n**",
         color=0xFF0000,
     )
-    emb.set_author(name=f"L'Imprimeur en a gros 😡😡")
+    emb.set_author(name=f"L'imprimeur en a gros 😡😡")
     emb.set_thumbnail(url=config.Emoji.bucher.url)
 
     await journey.ok_cancel("C'est tout bon ?", embed=emb)
 
     class _HaroView(discord.ui.View):
         @discord.ui.button(
             label=f"Voter contre {joueur.nom}"[:80], style=discord.ButtonStyle.primary, emoji=config.Emoji.bucher
@@ -259,51 +272,17 @@
         async def on_error(self, _interaction: discord.Interaction, error: Exception, _item: discord.ui.Item) -> None:
             raise error
 
     haro_message = await config.Channel.haros.send(
         f"(Psst, {joueur.member.mention} :3)", embed=emb, view=_HaroView(timeout=None)
     )
     await config.Channel.debats.send(
-        f"{config.Emoji.ha}{config.Emoji.ro} de {journey.member.mention} sur {joueur.member.mention} ! "
-        f"Vous en pensez quoi vous ? (détails sur {config.Channel.haros.mention})"
+        f"{config.Emoji.ha}{config.Emoji.ro} de L'imprimeur sur {joueur.member.mention} ! "
+        f"Vous en pensez quoi vous? (détails sur {config.Channel.haros.mention})"
     )
 
     haro = CandidHaro(joueur=joueur, type=CandidHaroType.haro, message_id=haro_message.id)
-    CandidHaro.add(haro)
-
+    
     if journey.channel != config.Channel.haros:
         await journey.send(f"Allez, c'est parti ! ({config.Channel.haros.mention})")
 
 
-@app_commands.command()
-@tools.mjs_only
-@journey_command
-async def imprimeur(journey: DiscordJourney, *, joueur: app_commands.Transform[Joueur, tools.VivantTransformer]):
-    """Lance publiquement un haro contre la personne visée par l'imprimeur. (COMMANDE MJ)
-
-    Args:
-        joueur: Le joueur ou la joueuse à accuser de tous les maux.
-
-    Cette commande n'est utilisable que lorsqu'un vote pour le condamné est en cours.
-    """
-    await _imprimeur(journey, joueur=joueur)
-
-
-@app_commands.context_menu(name="Lancer un haro contre ce joueur")
-@tools.mjs_only
-@journey_context_menu
-async def haro_menu(journey: DiscordJourney, member: discord.Member):
-    if member.top_role >= config.Role.mj:
-        await journey.send(":x: Attends deux secondes, tu pensais faire quoi là ?")
-        return
-
-    if member == config.bot.user:
-        await journey.send(":x: Tu ne peux pas haro le bot, enfin !!!")
-        return
-
-    try:
-        joueur = Joueur.from_member(member)
-    except ValueError:
-        await journey.send(":x: Hmm, ce joueur n'a pas l'air inscrit !")
-        return
-
-    await _haro(journey, joueur=joueur)
```

### Comparing `lg-rez-4.0.2/lgrez/features/annexe.py` & `lg_rez-4.0.3/lgrez/features/annexe.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,7 +234,8 @@
 
     url = rep.json().get("img")
     if not url:
         await journey.send(":x: Paramètre incorrect ou service non accessible.")
         return
 
     await journey.send(url)
+
```

### Comparing `lg-rez-4.0.2/lgrez/features/chans.py` & `lg_rez-4.0.3/lgrez/features/chans.py`

 * *Files identical despite different names*

### Comparing `lg-rez-4.0.2/lgrez/features/communication.py` & `lg_rez-4.0.3/lgrez/features/communication.py`

 * *Files 2% similar despite different names*

```diff
@@ -266,14 +266,22 @@
     corba = BaseAction.query.get(config.ajout_vote_baseaction)
     if corba:
         log += "\n  - Corbeau(x) : "
         for util in query.join(Utilisation.action).filter(Action.base == corba).all():
             log += f"{util.action.joueur.nom} -> {util.cible} / "
             cibles.setdefault(util.cible, [])
             cibles[util.cible].extend([util.action.joueur.role.nom] * config.n_ajouts_votes)
+    
+    impri = BaseAction.query.get(config.ajout_vote_impr_baseaction)
+    if impri:
+        log += "\n  - Imprimante(x) : "
+        for util in query.join(Utilisation.action).filter(Action.base == impri).all():
+            log += f"{util.action.joueur.nom} -> {util.cible} / "
+            cibles.setdefault(util.cible, [])
+            cibles[util.cible].extend([util.action.joueur.role.nom] * config.n_ajouts_votes_impr)
 
     # Classe utilitaire
     @functools.total_ordering
     class _Cible:
         """Représente un joueur ciblé, pour usage dans /plot"""
 
         def __init__(self, joueur, votants):
```

### Comparing `lg-rez-4.0.2/lgrez/features/gestion_actions.py` & `lg_rez-4.0.3/lgrez/features/gestion_actions.py`

 * *Files identical despite different names*

### Comparing `lg-rez-4.0.2/lgrez/features/gestion_ia.py` & `lg_rez-4.0.3/lgrez/features/gestion_ia.py`

 * *Files identical despite different names*

### Comparing `lg-rez-4.0.2/lgrez/features/informations.py` & `lg_rez-4.0.3/lgrez/features/informations.py`

 * *Files identical despite different names*

### Comparing `lg-rez-4.0.2/lgrez/features/inscription.py` & `lg_rez-4.0.3/lgrez/features/inscription.py`

 * *Files identical despite different names*

### Comparing `lg-rez-4.0.2/lgrez/features/open_close.py` & `lg_rez-4.0.3/lgrez/features/open_close.py`

 * *Files identical despite different names*

### Comparing `lg-rez-4.0.2/lgrez/features/special.py` & `lg_rez-4.0.3/lgrez/features/special.py`

 * *Files identical despite different names*

### Comparing `lg-rez-4.0.2/lgrez/features/sync.py` & `lg_rez-4.0.3/lgrez/features/sync.py`

 * *Files identical despite different names*

### Comparing `lg-rez-4.0.2/lgrez/features/taches.py` & `lg_rez-4.0.3/lgrez/features/taches.py`

 * *Files identical despite different names*

### Comparing `lg-rez-4.0.2/lgrez/features/voter_agir.py` & `lg_rez-4.0.3/lgrez/features/voter_agir.py`

 * *Files identical despite different names*

### Comparing `lg-rez-4.0.2/lgrez/server_structure.json` & `lg_rez-4.0.3/lgrez/server_structure.json`

 * *Files identical despite different names*

### Comparing `lg-rez-4.0.2/setup.py` & `lg_rez-4.0.3/setup.py`

 * *Files identical despite different names*

