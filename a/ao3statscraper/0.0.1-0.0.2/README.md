# Comparing `tmp/ao3statscraper-0.0.1.tar.gz` & `tmp/ao3statscraper-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ao3statscraper-0.0.1.tar", last modified: Wed Apr 24 14:41:46 2024, max compression
+gzip compressed data, was "ao3statscraper-0.0.2.tar", last modified: Wed Apr 24 22:55:47 2024, max compression
```

## Comparing `ao3statscraper-0.0.1.tar` & `ao3statscraper-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 mivkov    (1000) mivkov    (1000)        0 2024-04-24 14:41:46.445742 ao3statscraper-0.0.1/
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)    35137 2024-04-10 17:46:52.000000 ao3statscraper-0.0.1/LICENSE
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      220 2024-04-24 14:13:41.000000 ao3statscraper-0.0.1/MANIFEST.in
--rw-r--r--   0 mivkov    (1000) mivkov    (1000)    43968 2024-04-24 14:41:46.445742 ao3statscraper-0.0.1/PKG-INFO
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     2590 2024-04-24 14:25:45.000000 ao3statscraper-0.0.1/README.md
-drwxrwxr-x   0 mivkov    (1000) mivkov    (1000)        0 2024-04-24 14:41:46.445742 ao3statscraper-0.0.1/ao3statscraper/
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      523 2024-04-24 14:13:41.000000 ao3statscraper-0.0.1/ao3statscraper/__init__.py
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)       22 2024-04-24 14:13:41.000000 ao3statscraper-0.0.1/ao3statscraper/__version__.py
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     2355 2024-04-24 14:13:41.000000 ao3statscraper-0.0.1/ao3statscraper/ao3requester.py
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     6533 2024-04-24 14:13:41.000000 ao3statscraper-0.0.1/ao3statscraper/configuration.py
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     6530 2024-04-24 14:13:41.000000 ao3statscraper-0.0.1/ao3statscraper/plotting.py
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     3862 2024-04-24 14:13:41.000000 ao3statscraper-0.0.1/ao3statscraper/pw.py
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     8015 2024-04-24 14:13:41.000000 ao3statscraper-0.0.1/ao3statscraper/scrape.py
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)    11255 2024-04-24 14:13:41.000000 ao3statscraper-0.0.1/ao3statscraper/statsdata.py
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     1396 2024-04-24 14:13:41.000000 ao3statscraper-0.0.1/ao3statscraper/utils.py
-drwxrwxr-x   0 mivkov    (1000) mivkov    (1000)        0 2024-04-24 14:41:46.445742 ao3statscraper-0.0.1/ao3statscraper.egg-info/
--rw-r--r--   0 mivkov    (1000) mivkov    (1000)    43968 2024-04-24 14:41:46.000000 ao3statscraper-0.0.1/ao3statscraper.egg-info/PKG-INFO
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      570 2024-04-24 14:41:46.000000 ao3statscraper-0.0.1/ao3statscraper.egg-info/SOURCES.txt
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)        1 2024-04-24 14:41:46.000000 ao3statscraper-0.0.1/ao3statscraper.egg-info/dependency_links.txt
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      263 2024-04-24 14:41:46.000000 ao3statscraper-0.0.1/ao3statscraper.egg-info/entry_points.txt
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      109 2024-04-24 14:41:46.000000 ao3statscraper-0.0.1/ao3statscraper.egg-info/requires.txt
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)       15 2024-04-24 14:41:46.000000 ao3statscraper-0.0.1/ao3statscraper.egg-info/top_level.txt
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     1586 2024-04-24 14:13:41.000000 ao3statscraper-0.0.1/pyproject.toml
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)       38 2024-04-24 14:41:46.445742 ao3statscraper-0.0.1/setup.cfg
-drwxrwxr-x   0 mivkov    (1000) mivkov    (1000)        0 2024-04-24 14:41:46.445742 ao3statscraper-0.0.1/tests/
--rwxrwxr-x   0 mivkov    (1000) mivkov    (1000)      933 2024-04-24 14:13:41.000000 ao3statscraper-0.0.1/tests/test_passwords.py
--rwxrwxr-x   0 mivkov    (1000) mivkov    (1000)      642 2024-04-24 14:13:41.000000 ao3statscraper-0.0.1/tests/test_writing_data.py
+drwxrwxr-x   0 mivkov    (1000) mivkov    (1000)        0 2024-04-24 22:55:47.801983 ao3statscraper-0.0.2/
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)    35137 2024-04-10 17:46:52.000000 ao3statscraper-0.0.2/LICENSE
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      220 2024-04-24 14:13:41.000000 ao3statscraper-0.0.2/MANIFEST.in
+-rw-r--r--   0 mivkov    (1000) mivkov    (1000)    47047 2024-04-24 22:55:47.801983 ao3statscraper-0.0.2/PKG-INFO
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     5669 2024-04-24 22:54:15.000000 ao3statscraper-0.0.2/README.md
+drwxrwxr-x   0 mivkov    (1000) mivkov    (1000)        0 2024-04-24 22:55:47.801983 ao3statscraper-0.0.2/ao3statscraper/
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      523 2024-04-24 14:13:41.000000 ao3statscraper-0.0.2/ao3statscraper/__init__.py
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)       22 2024-04-24 22:55:41.000000 ao3statscraper-0.0.2/ao3statscraper/__version__.py
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     2355 2024-04-24 14:13:41.000000 ao3statscraper-0.0.2/ao3statscraper/ao3requester.py
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     6517 2024-04-24 21:10:25.000000 ao3statscraper-0.0.2/ao3statscraper/configuration.py
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     6530 2024-04-24 14:13:41.000000 ao3statscraper-0.0.2/ao3statscraper/plotting.py
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     3862 2024-04-24 14:13:41.000000 ao3statscraper-0.0.2/ao3statscraper/pw.py
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     8015 2024-04-24 22:00:25.000000 ao3statscraper-0.0.2/ao3statscraper/scrape.py
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)    11255 2024-04-24 14:13:41.000000 ao3statscraper-0.0.2/ao3statscraper/statsdata.py
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     1396 2024-04-24 14:13:41.000000 ao3statscraper-0.0.2/ao3statscraper/utils.py
+drwxrwxr-x   0 mivkov    (1000) mivkov    (1000)        0 2024-04-24 22:55:47.801983 ao3statscraper-0.0.2/ao3statscraper.egg-info/
+-rw-r--r--   0 mivkov    (1000) mivkov    (1000)    47047 2024-04-24 22:55:47.000000 ao3statscraper-0.0.2/ao3statscraper.egg-info/PKG-INFO
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      570 2024-04-24 22:55:47.000000 ao3statscraper-0.0.2/ao3statscraper.egg-info/SOURCES.txt
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)        1 2024-04-24 22:55:47.000000 ao3statscraper-0.0.2/ao3statscraper.egg-info/dependency_links.txt
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      263 2024-04-24 22:55:47.000000 ao3statscraper-0.0.2/ao3statscraper.egg-info/entry_points.txt
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      109 2024-04-24 22:55:47.000000 ao3statscraper-0.0.2/ao3statscraper.egg-info/requires.txt
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)       15 2024-04-24 22:55:47.000000 ao3statscraper-0.0.2/ao3statscraper.egg-info/top_level.txt
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     1586 2024-04-24 22:55:41.000000 ao3statscraper-0.0.2/pyproject.toml
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)       38 2024-04-24 22:55:47.801983 ao3statscraper-0.0.2/setup.cfg
+drwxrwxr-x   0 mivkov    (1000) mivkov    (1000)        0 2024-04-24 22:55:47.801983 ao3statscraper-0.0.2/tests/
+-rwxrwxr-x   0 mivkov    (1000) mivkov    (1000)      933 2024-04-24 14:13:41.000000 ao3statscraper-0.0.2/tests/test_passwords.py
+-rwxrwxr-x   0 mivkov    (1000) mivkov    (1000)      642 2024-04-24 14:13:41.000000 ao3statscraper-0.0.2/tests/test_writing_data.py
```

### Comparing `ao3statscraper-0.0.1/LICENSE` & `ao3statscraper-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ao3statscraper-0.0.1/PKG-INFO` & `ao3statscraper-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ao3statscraper
-Version: 0.0.1
+Version: 0.0.2
 Summary: Scrape stats from your AO3 stats page.
 Author-email: Lars Ikarion <lars.ikarion@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -701,37 +701,153 @@
 # AO3StatScraper
 
 `AO3StatScraper` is a small python package that provides command line scripts
 to fetch your AO3 (*Archive Of Our Own*) statistics to store and display them.
 
 ## Installation
 
-The main use case is to fetch and display your current statistics.
+`AO3StatScraper` is available on [PyPI](https://pypi.org/project/ao3statscraper/), and
+can obtained any regular way you'd install a python package, e.g. using `pip`, `conda`, etc.
+
+For example, using `pip`:
+
+On Unix/OSX:
+
+```
+python3 -m pip install ao3statscraper
+```
+
+On Windows:
+
+```
+py -m pip install ao3statscraper
+```
+
+
+Alternately, the source code is available on [gitlab](https://gitlab.com/athenaslilowl1/AO3StatScraper). 
+On OSX and Linux, you can install a local version by cloning the repository using git:
+
+```
+git clone https://gitlab.com/athenaslilowl1/AO3StatScraper.git
+cd AO3StatScraper  # go into the directory
+python3 -m pip install .
+```
+
+
+
+## User Guide
+
+### Getting Started
+
+The main use case for `AO3StatScraper` is to fetch and display your current AO3 statistics using
+scripts provided by `AO3StatScraper`. Currently, there are 4 scripts:
+
+- `ao3get` : The main script to fetch your AO3 stats.
+- `ao3plot`: Plots the stats stored with `ao3get`
+- `ao3_hits_to_kudos`: List all your works in ascending order of their hits/kudos ratio
+- `ao3_purge`: Deletes saved stats such that there is a minumum time between the remaining ones
+
+
+**IMPORTANT**: Before you can run the other scripts, you first need to configure `AO3StatScraper`.
+This is done by calling `ao3get`. It will launch the configuration dialogue automatically if it hasn't
+been configured yet. You can always re-configure it by invoking `ao3get -c`.
+
+
+
+
+### `ao3get`
+
+This is the main script to fetch and store your AO3 stats. There are several running modes.
+When in doubt, invoke `ao3get --help` to see the available options.
+
+The default running mode is `--diff`.
+
+- `--all`: Fetch and store current stats from AO3 into a snapshot, and display stats for all works.
+- `--repeat`: Don't fetch new stats, but show the changes between the last two stored stats snapshots.
+- `--diff`: Fetch and store current stats from AO3 into a snapshot, and display only stats for works that have changed since the last snapshot. If there were no changes in work stats, it will display only the user's total stats.
+- `--config`: Run the configuration dialogue and exit.
+- `--remove-last`: Deletes the last snapshot `ao3get` stored and exits. May come in handy if you're nervously re-downloading your stats every minute.
+- `--no-write`: This flag modifies the behavious for `--all` and `--diff` running modes. While current stats are fetched from AO3, they won't be written into a snapshot.
+
+
+Using `ao3get` requires you to log in to your AO3 account. You can either type in your username and password
+each time you invoke it, or you can store it with `AO3StatScraper`, locked behind a master password. There
+are no restrictions on how sophisticated your master password needs to be, so if you can't be inconvenienced,
+you can even leave it empty.
+
+
+### `ao3plot`
+
+`ao3plot` will display some simple graphs based on the stored snapshots. It never stores snapshots itself,
+you will need to do that using `ao3get`. 
+
+By default, `ao3plot` will ask you to select which work you would like to see graphs of stats for. You can
+also select to plot your total user statistics.
+
+Alternately, you can skip that dialogue by using the following flags:
+
+- `-u`: Show total user statistics.
+- `-i [ID]`: Show the statistics for the work with AO3 ID `[ID]`. For example, if your work is under the link `https://archiveofourown.org/works/24280306`, the ID would be `24280306`.
+
+It is possible that the stats graphs aren't displayed nicely on all screens. If that is the case for you,
+you may want to try the `--no-prettify` flag to obtain a bare-bones plot without any prettifications. It
+may not look as nice, but at least you should be able to see the data.
+
+
+
+### `ao3_hits_to_kudos`
+
+This script just reads in the last stored snapshot and prints out all your works in ascending order of their hits/kudos ratio.
+
+
+
+### `ao3_purge`
+
+In case you find yourself in a situation where you feel you have stored way too many snapshots, `ao3_purge` offers
+you the option to delete stats snapshots such that there is some minimal time between them. By default, this frequency
+is set to 12h. You can provide the frequency you like using the `--frequency` flag.
+
+
+
+
+
+## Examples
+
+This is example output what `ao3get` will show you when you run it:
+
+![default running mode, diff](webdata/ao3get.png)
+
+It will only list the works that have changes since you last cheked (i.e. stored a snapshot).
+
+But you can also view all your works:
+
+![show all works](webdata/ao3get-all.png)
+
+
+Plotting the total user statistics with `ao3plot` will show you something like this:
+
+![plotting user stats](webdata/plot-user.png)
+
+
+Running `ao3plot` for a specific work will give you 2 plots:
+
+![plotting work, Figure 1](webdata/plot-work1.png)
+![plotting work, Figure 2](webdata/plot-work2.png)
 
 
-## Installation
-Within a particular ecosystem, there may be a common way of installing things, such as using Yarn, NuGet, or Homebrew. However, consider the possibility that whoever is reading your README is a novice and would like more guidance. Listing specific steps helps remove ambiguity and gets people to using your project as quickly as possible. If it only runs in a specific context like a particular programming language version or operating system or has dependencies that have to be installed manually, also add a Requirements subsection.
 
-## Usage
-Use examples liberally, and show the expected output if you can. It's helpful to have inline the smallest example of usage that you can demonstrate, while providing links to more sophisticated examples if they are too long to reasonably include in the README.
 
-## Support
-Tell people where they can go to for help. It can be any combination of an issue tracker, a chat room, an email address, etc.
 
-## Roadmap
-If you have ideas for releases in the future, it is a good idea to list them in the README.
+# Having issues?
 
-## Contributing
-State if you are open to contributions and what your requirements are for accepting them.
+Please let me know by raising an issue on [gitlab](https://gitlab.com/athenaslilowl1/AO3StatScraper/-/issues)
 
-For people who want to make changes to your project, it's helpful to have some documentation on how to get started. Perhaps there is a script that they should run or some environment variables that they need to set. Make these steps explicit. These instructions could also be useful to your future self.
 
-You can also document commands to lint the code or run tests. These steps help to ensure high code quality and reduce the likelihood that the changes inadvertently break something. Having instructions for running tests is especially helpful if it requires external setup, such as starting a Selenium server for testing in a browser.
 
-## Authors and acknowledgment
-Show your appreciation to those who have contributed to the project.
+# Roadmap and Contributing
 
-## License
-For open source projects, say how it is licensed.
+This tool was always intended to be a command line tool on my end. Having never programmed a GUI in my life,
+I don't intend to start now. However, if anybody is willing to pack this up in a nice simple portable GUI, 
+you are very welcome and encouraged to do so! I'll gladly add it to the repository.
 
-## Project status
-If you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.
+I'm using unix exclusively, so there may be issues on other operating systems. Testers and devs on OSX and
+windows are also very welcome to let me know what's working and what needs fixing.
```

### Comparing `ao3statscraper-0.0.1/ao3statscraper/__init__.py` & `ao3statscraper-0.0.2/ao3statscraper/__init__.py`

 * *Files identical despite different names*

### Comparing `ao3statscraper-0.0.1/ao3statscraper/ao3requester.py` & `ao3statscraper-0.0.2/ao3statscraper/ao3requester.py`

 * *Files identical despite different names*

### Comparing `ao3statscraper-0.0.1/ao3statscraper/configuration.py` & `ao3statscraper-0.0.2/ao3statscraper/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,15 +124,15 @@
         datadir = input(f"(default: '{self.ao3dir}')\n")
 
         clear_terminal()
         print("Optionally, you can store your AO3 login on your local machine.")
         print("Your username and password will be encrypted and locked with a ")
         print("master password that you'll be asked to set next.")
         print("(If you forget the master password, you'll need to re-run this")
-        print("configuration dialogue. You can do that by running `getAO3stats.py -c`)")
+        print("configuration dialogue. You can do that by running `ao3get -c`)")
         store_login_str = "b"
         a = 0
         while not store_login_str.startswith(("n", "N", "y", "Y")):
             if a > 0:
                 print("Invalid input.")
             store_login_str = input(
                 "Do you want to store your AO3 login on your local machine? [y/n]\n"
@@ -201,15 +201,15 @@
 
         try:
             self.datadir = confdata["Globals"]["data_directory"]
             self.store_login = confdata["Globals"]["store_login"]
         except KeyError:
             print("ERROR: Some fields are missing from your config file.")
             print("It might be out of date.")
-            print("Re-generate it using `getAO3stats.py -c`")
+            print("Re-generate it using `ao3get -c`")
             quit(1)
 
         return
 
     def prep_scrape(self):
         """
         Ensure everything is set for a scrape.
```

### Comparing `ao3statscraper-0.0.1/ao3statscraper/plotting.py` & `ao3statscraper-0.0.2/ao3statscraper/plotting.py`

 * *Files identical despite different names*

### Comparing `ao3statscraper-0.0.1/ao3statscraper/pw.py` & `ao3statscraper-0.0.2/ao3statscraper/pw.py`

 * *Files identical despite different names*

### Comparing `ao3statscraper-0.0.1/ao3statscraper/scrape.py` & `ao3statscraper-0.0.2/ao3statscraper/scrape.py`

 * *Files identical despite different names*

### Comparing `ao3statscraper-0.0.1/ao3statscraper/statsdata.py` & `ao3statscraper-0.0.2/ao3statscraper/statsdata.py`

 * *Files identical despite different names*

### Comparing `ao3statscraper-0.0.1/ao3statscraper/utils.py` & `ao3statscraper-0.0.2/ao3statscraper/utils.py`

 * *Files identical despite different names*

### Comparing `ao3statscraper-0.0.1/ao3statscraper.egg-info/PKG-INFO` & `ao3statscraper-0.0.2/ao3statscraper.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ao3statscraper
-Version: 0.0.1
+Version: 0.0.2
 Summary: Scrape stats from your AO3 stats page.
 Author-email: Lars Ikarion <lars.ikarion@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -701,37 +701,153 @@
 # AO3StatScraper
 
 `AO3StatScraper` is a small python package that provides command line scripts
 to fetch your AO3 (*Archive Of Our Own*) statistics to store and display them.
 
 ## Installation
 
-The main use case is to fetch and display your current statistics.
+`AO3StatScraper` is available on [PyPI](https://pypi.org/project/ao3statscraper/), and
+can obtained any regular way you'd install a python package, e.g. using `pip`, `conda`, etc.
+
+For example, using `pip`:
+
+On Unix/OSX:
+
+```
+python3 -m pip install ao3statscraper
+```
+
+On Windows:
+
+```
+py -m pip install ao3statscraper
+```
+
+
+Alternately, the source code is available on [gitlab](https://gitlab.com/athenaslilowl1/AO3StatScraper). 
+On OSX and Linux, you can install a local version by cloning the repository using git:
+
+```
+git clone https://gitlab.com/athenaslilowl1/AO3StatScraper.git
+cd AO3StatScraper  # go into the directory
+python3 -m pip install .
+```
+
+
+
+## User Guide
+
+### Getting Started
+
+The main use case for `AO3StatScraper` is to fetch and display your current AO3 statistics using
+scripts provided by `AO3StatScraper`. Currently, there are 4 scripts:
+
+- `ao3get` : The main script to fetch your AO3 stats.
+- `ao3plot`: Plots the stats stored with `ao3get`
+- `ao3_hits_to_kudos`: List all your works in ascending order of their hits/kudos ratio
+- `ao3_purge`: Deletes saved stats such that there is a minumum time between the remaining ones
+
+
+**IMPORTANT**: Before you can run the other scripts, you first need to configure `AO3StatScraper`.
+This is done by calling `ao3get`. It will launch the configuration dialogue automatically if it hasn't
+been configured yet. You can always re-configure it by invoking `ao3get -c`.
+
+
+
+
+### `ao3get`
+
+This is the main script to fetch and store your AO3 stats. There are several running modes.
+When in doubt, invoke `ao3get --help` to see the available options.
+
+The default running mode is `--diff`.
+
+- `--all`: Fetch and store current stats from AO3 into a snapshot, and display stats for all works.
+- `--repeat`: Don't fetch new stats, but show the changes between the last two stored stats snapshots.
+- `--diff`: Fetch and store current stats from AO3 into a snapshot, and display only stats for works that have changed since the last snapshot. If there were no changes in work stats, it will display only the user's total stats.
+- `--config`: Run the configuration dialogue and exit.
+- `--remove-last`: Deletes the last snapshot `ao3get` stored and exits. May come in handy if you're nervously re-downloading your stats every minute.
+- `--no-write`: This flag modifies the behavious for `--all` and `--diff` running modes. While current stats are fetched from AO3, they won't be written into a snapshot.
+
+
+Using `ao3get` requires you to log in to your AO3 account. You can either type in your username and password
+each time you invoke it, or you can store it with `AO3StatScraper`, locked behind a master password. There
+are no restrictions on how sophisticated your master password needs to be, so if you can't be inconvenienced,
+you can even leave it empty.
+
+
+### `ao3plot`
+
+`ao3plot` will display some simple graphs based on the stored snapshots. It never stores snapshots itself,
+you will need to do that using `ao3get`. 
+
+By default, `ao3plot` will ask you to select which work you would like to see graphs of stats for. You can
+also select to plot your total user statistics.
+
+Alternately, you can skip that dialogue by using the following flags:
+
+- `-u`: Show total user statistics.
+- `-i [ID]`: Show the statistics for the work with AO3 ID `[ID]`. For example, if your work is under the link `https://archiveofourown.org/works/24280306`, the ID would be `24280306`.
+
+It is possible that the stats graphs aren't displayed nicely on all screens. If that is the case for you,
+you may want to try the `--no-prettify` flag to obtain a bare-bones plot without any prettifications. It
+may not look as nice, but at least you should be able to see the data.
+
+
+
+### `ao3_hits_to_kudos`
+
+This script just reads in the last stored snapshot and prints out all your works in ascending order of their hits/kudos ratio.
+
+
+
+### `ao3_purge`
+
+In case you find yourself in a situation where you feel you have stored way too many snapshots, `ao3_purge` offers
+you the option to delete stats snapshots such that there is some minimal time between them. By default, this frequency
+is set to 12h. You can provide the frequency you like using the `--frequency` flag.
+
+
+
+
+
+## Examples
+
+This is example output what `ao3get` will show you when you run it:
+
+![default running mode, diff](webdata/ao3get.png)
+
+It will only list the works that have changes since you last cheked (i.e. stored a snapshot).
+
+But you can also view all your works:
+
+![show all works](webdata/ao3get-all.png)
+
+
+Plotting the total user statistics with `ao3plot` will show you something like this:
+
+![plotting user stats](webdata/plot-user.png)
+
+
+Running `ao3plot` for a specific work will give you 2 plots:
+
+![plotting work, Figure 1](webdata/plot-work1.png)
+![plotting work, Figure 2](webdata/plot-work2.png)
 
 
-## Installation
-Within a particular ecosystem, there may be a common way of installing things, such as using Yarn, NuGet, or Homebrew. However, consider the possibility that whoever is reading your README is a novice and would like more guidance. Listing specific steps helps remove ambiguity and gets people to using your project as quickly as possible. If it only runs in a specific context like a particular programming language version or operating system or has dependencies that have to be installed manually, also add a Requirements subsection.
 
-## Usage
-Use examples liberally, and show the expected output if you can. It's helpful to have inline the smallest example of usage that you can demonstrate, while providing links to more sophisticated examples if they are too long to reasonably include in the README.
 
-## Support
-Tell people where they can go to for help. It can be any combination of an issue tracker, a chat room, an email address, etc.
 
-## Roadmap
-If you have ideas for releases in the future, it is a good idea to list them in the README.
+# Having issues?
 
-## Contributing
-State if you are open to contributions and what your requirements are for accepting them.
+Please let me know by raising an issue on [gitlab](https://gitlab.com/athenaslilowl1/AO3StatScraper/-/issues)
 
-For people who want to make changes to your project, it's helpful to have some documentation on how to get started. Perhaps there is a script that they should run or some environment variables that they need to set. Make these steps explicit. These instructions could also be useful to your future self.
 
-You can also document commands to lint the code or run tests. These steps help to ensure high code quality and reduce the likelihood that the changes inadvertently break something. Having instructions for running tests is especially helpful if it requires external setup, such as starting a Selenium server for testing in a browser.
 
-## Authors and acknowledgment
-Show your appreciation to those who have contributed to the project.
+# Roadmap and Contributing
 
-## License
-For open source projects, say how it is licensed.
+This tool was always intended to be a command line tool on my end. Having never programmed a GUI in my life,
+I don't intend to start now. However, if anybody is willing to pack this up in a nice simple portable GUI, 
+you are very welcome and encouraged to do so! I'll gladly add it to the repository.
 
-## Project status
-If you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.
+I'm using unix exclusively, so there may be issues on other operating systems. Testers and devs on OSX and
+windows are also very welcome to let me know what's working and what needs fixing.
```

### Comparing `ao3statscraper-0.0.1/ao3statscraper.egg-info/SOURCES.txt` & `ao3statscraper-0.0.2/ao3statscraper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ao3statscraper-0.0.1/pyproject.toml` & `ao3statscraper-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.setuptools]
 packages = ["ao3statscraper"]
 
 [project]
 name = "ao3statscraper"
 description="Scrape stats from your AO3 stats page."
 readme = "README.md"
-version = "0.0.1"
+version = "0.0.2"
 authors= [
     { name = "Lars Ikarion", email="lars.ikarion@gmail.com"},
     ]
 license = { file = "LICENSE" }
 classifiers=[
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -43,15 +43,15 @@
 ao3get= "ao3statscraper.scripts:ao3scrape"
 
 
 [project.urls]
 "Homepage" = "https://gitlab.com/athenaslilowl1/AO3StatScraper"
 
 [tool.bumpver]
-current_version = "0.0.1"
+current_version = "0.0.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `ao3statscraper-0.0.1/tests/test_passwords.py` & `ao3statscraper-0.0.2/tests/test_passwords.py`

 * *Files identical despite different names*

### Comparing `ao3statscraper-0.0.1/tests/test_writing_data.py` & `ao3statscraper-0.0.2/tests/test_writing_data.py`

 * *Files identical despite different names*

