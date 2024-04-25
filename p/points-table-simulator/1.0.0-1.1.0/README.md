# Comparing `tmp/points-table-simulator-1.0.0.tar.gz` & `tmp/points_table_simulator-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "points-table-simulator-1.0.0.tar", last modified: Thu Mar  7 14:41:38 2024, max compression
+gzip compressed data, was "points_table_simulator-1.1.0.tar", last modified: Thu Apr 25 07:00:26 2024, max compression
```

## Comparing `points-table-simulator-1.0.0.tar` & `points_table_simulator-1.1.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:41:38.110314 points-table-simulator-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:41:38.098314 points-table-simulator-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:41:38.102314 points-table-simulator-1.0.0/.github/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-03-07 14:41:26.000000 points-table-simulator-1.0.0/.github/scripts/quality_checks.sh
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-03-07 14:41:26.000000 points-table-simulator-1.0.0/.github/scripts/setup_environment.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:41:38.102314 points-table-simulator-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-03-07 14:41:26.000000 points-table-simulator-1.0.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-03-07 14:41:26.000000 points-table-simulator-1.0.0/.github/workflows/quality_check.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-03-07 14:41:26.000000 points-table-simulator-1.0.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:41:38.102314 points-table-simulator-1.0.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-03-07 14:41:26.000000 points-table-simulator-1.0.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-03-07 14:41:26.000000 points-table-simulator-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-03-07 14:41:38.110314 points-table-simulator-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-03-07 14:41:26.000000 points-table-simulator-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-07 14:41:26.000000 points-table-simulator-1.0.0/create_venv.sh
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-03-07 14:41:26.000000 points-table-simulator-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-07 14:41:38.110314 points-table-simulator-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 14:41:26.000000 points-table-simulator-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:41:38.098314 points-table-simulator-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:41:38.106314 points-table-simulator-1.0.0/src/points_table_simulator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:41:26.000000 points-table-simulator-1.0.0/src/points_table_simulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-03-07 14:41:26.000000 points-table-simulator-1.0.0/src/points_table_simulator/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-03-07 14:41:26.000000 points-table-simulator-1.0.0/src/points_table_simulator/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    23894 2024-03-07 14:41:26.000000 points-table-simulator-1.0.0/src/points_table_simulator/points_table_simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:41:38.110314 points-table-simulator-1.0.0/src/points_table_simulator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-03-07 14:41:38.000000 points-table-simulator-1.0.0/src/points_table_simulator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-03-07 14:41:38.000000 points-table-simulator-1.0.0/src/points_table_simulator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 14:41:38.000000 points-table-simulator-1.0.0/src/points_table_simulator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-07 14:41:38.000000 points-table-simulator-1.0.0/src/points_table_simulator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-07 14:41:38.000000 points-table-simulator-1.0.0/src/points_table_simulator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:41:38.106314 points-table-simulator-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:41:26.000000 points-table-simulator-1.0.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:41:38.110314 points-table-simulator-1.0.0/tests/points_table_simulator_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:41:26.000000 points-table-simulator-1.0.0/tests/points_table_simulator_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:41:38.110314 points-table-simulator-1.0.0/tests/points_table_simulator_tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-03-07 14:41:26.000000 points-table-simulator-1.0.0/tests/points_table_simulator_tests/data/psl_2024_fixture.csv
--rw-r--r--   0 runner    (1001) docker     (127)    12987 2024-03-07 14:41:26.000000 points-table-simulator-1.0.0/tests/points_table_simulator_tests/error_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-03-07 14:41:26.000000 points-table-simulator-1.0.0/tests/points_table_simulator_tests/success_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:00:26.704224 points_table_simulator-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:00:26.696224 points_table_simulator-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:00:26.700224 points_table_simulator-1.1.0/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-25 07:00:18.000000 points_table_simulator-1.1.0/.github/scripts/quality_checks.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-25 07:00:18.000000 points_table_simulator-1.1.0/.github/scripts/setup_environment.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:00:26.700224 points_table_simulator-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-25 07:00:18.000000 points_table_simulator-1.1.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-25 07:00:18.000000 points_table_simulator-1.1.0/.github/workflows/quality_check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-25 07:00:18.000000 points_table_simulator-1.1.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:00:26.700224 points_table_simulator-1.1.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-25 07:00:18.000000 points_table_simulator-1.1.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-25 07:00:18.000000 points_table_simulator-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-25 07:00:26.704224 points_table_simulator-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-04-25 07:00:18.000000 points_table_simulator-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-25 07:00:18.000000 points_table_simulator-1.1.0/create_venv.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-25 07:00:18.000000 points_table_simulator-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-25 07:00:26.704224 points_table_simulator-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 07:00:18.000000 points_table_simulator-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:00:26.696224 points_table_simulator-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:00:26.700224 points_table_simulator-1.1.0/src/points_table_simulator/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-25 07:00:18.000000 points_table_simulator-1.1.0/src/points_table_simulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-25 07:00:18.000000 points_table_simulator-1.1.0/src/points_table_simulator/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-25 07:00:18.000000 points_table_simulator-1.1.0/src/points_table_simulator/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25624 2024-04-25 07:00:18.000000 points_table_simulator-1.1.0/src/points_table_simulator/points_table_simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:00:26.704224 points_table_simulator-1.1.0/src/points_table_simulator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-25 07:00:26.000000 points_table_simulator-1.1.0/src/points_table_simulator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-25 07:00:26.000000 points_table_simulator-1.1.0/src/points_table_simulator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 07:00:26.000000 points_table_simulator-1.1.0/src/points_table_simulator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-25 07:00:26.000000 points_table_simulator-1.1.0/src/points_table_simulator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-25 07:00:26.000000 points_table_simulator-1.1.0/src/points_table_simulator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:00:26.700224 points_table_simulator-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 07:00:18.000000 points_table_simulator-1.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:00:26.704224 points_table_simulator-1.1.0/tests/points_table_simulator_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 07:00:18.000000 points_table_simulator-1.1.0/tests/points_table_simulator_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:00:26.704224 points_table_simulator-1.1.0/tests/points_table_simulator_tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-25 07:00:18.000000 points_table_simulator-1.1.0/tests/points_table_simulator_tests/data/psl_2024_fixture.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    12923 2024-04-25 07:00:18.000000 points_table_simulator-1.1.0/tests/points_table_simulator_tests/error_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-25 07:00:18.000000 points_table_simulator-1.1.0/tests/points_table_simulator_tests/success_tests.py
```

### Comparing `points-table-simulator-1.0.0/.github/workflows/quality_check.yml` & `points_table_simulator-1.1.0/.github/workflows/quality_check.yml`

 * *Files identical despite different names*

### Comparing `points-table-simulator-1.0.0/.gitignore` & `points_table_simulator-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `points-table-simulator-1.0.0/LICENSE` & `points_table_simulator-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `points-table-simulator-1.0.0/PKG-INFO` & `points_table_simulator-1.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: points-table-simulator
-Version: 1.0.0
+Version: 1.1.0
 Summary: This package will simulate the points table based on different possible results in a sports tournament
 Home-page: https://github.com/NishanthMuruganantham/points-table-simulator
 Author: Nishanth Muruganantham
 Author-email: nishanthmurugananth10@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -15,28 +15,30 @@
 
 During the later part of the league stages in many multi-team tournaments 🏆 such as 🏏 Indian Premier League(IPL), Australian Big Bash League (BBL), ets., the fans will look for possible match outcomes for the remaining league matches, which could lead their favourite team to get qualified for further stage in the tournament (Playoffs). Here, the fans calculate their points table📊 to see their favourite team being placed in the position needed to qualify for Playoffs🏃🏻.
 
 This tool🛠️ come as handy for those Sports enthusiasts which would help them to forsee the necessary remaining match outcomes to see their favourite team qualifying for playoffs✅ with the necessary match outcomes along with the respective points table📊.
 
 <hr>
 
-This package📦 will simulate the points table📊 based on different possible results in a sports tournament.
+This python package📦 will simulate the points table📊 based on different possible results in a sports tournament.
 
 The PointsTableSimulator package provides a powerful tool for simulating and analyzing points tables for sports tournaments. Whether you're organizing or following a tournament, this package offers the flexibility to input tournament schedules, define points systems, and explore various match outcome scenarios to understand team standings and qualification possibilities.
 
 ## Installation
 
-Install my-project with npm
+Install this package with pip
 
 ```
 pip install points-table-simulator
 ```
     
 ## Usage/Examples
 
+Please find the example usage from the below python code
+
 ```python
 from points_table_simulator import PointsTableSimulator
 import pandas as pd
 
 # Load the tournament schedule DataFrame
 tournament_schedule = pd.read_csv("tournament_schedule.csv")
 
@@ -54,21 +56,26 @@
 simulator = PointsTableSimulator(
     tournament_schedule=tournament_schedule,
     points_for_a_win=3,
     points_for_a_no_result=1,
     points_for_a_draw=1
 )
 
-# Calculate the current points table
-current_table = simulator.current_points_table()
+# Get the current points table
+current_table = simulator.current_points_table      # current_points_table is an attribute of PointsTableSimulator class
 
 # Simulate qualification scenarios for a specific team
 points_tables, qualification_match_results = simulator.simulate_the_qualification_scenarios(
     team_name="Team A",
     top_x_position_in_the_table=4,
     desired_number_of_scenarios=5
 )
 
 # points_tables - will return the list of points_tables (pd.Dataframe) for different qualification scenarios
 # qualification_match_results - will return the list of table containing remaining match outcomes which could favour their team to get qualified for the given position
 ```
 
+>This package can also be used in Football tournaments such as English Premier League (EPL), Laliga, etc., when you want to generate the scenarios in which your favourite team can be placed in your expected position in the pointstable.
+
+## License
+
+[MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `points-table-simulator-1.0.0/README.md` & `points_table_simulator-1.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,28 +2,30 @@
 
 During the later part of the league stages in many multi-team tournaments 🏆 such as 🏏 Indian Premier League(IPL), Australian Big Bash League (BBL), ets., the fans will look for possible match outcomes for the remaining league matches, which could lead their favourite team to get qualified for further stage in the tournament (Playoffs). Here, the fans calculate their points table📊 to see their favourite team being placed in the position needed to qualify for Playoffs🏃🏻.
 
 This tool🛠️ come as handy for those Sports enthusiasts which would help them to forsee the necessary remaining match outcomes to see their favourite team qualifying for playoffs✅ with the necessary match outcomes along with the respective points table📊.
 
 <hr>
 
-This package📦 will simulate the points table📊 based on different possible results in a sports tournament.
+This python package📦 will simulate the points table📊 based on different possible results in a sports tournament.
 
 The PointsTableSimulator package provides a powerful tool for simulating and analyzing points tables for sports tournaments. Whether you're organizing or following a tournament, this package offers the flexibility to input tournament schedules, define points systems, and explore various match outcome scenarios to understand team standings and qualification possibilities.
 
 ## Installation
 
-Install my-project with npm
+Install this package with pip
 
 ```
 pip install points-table-simulator
 ```
     
 ## Usage/Examples
 
+Please find the example usage from the below python code
+
 ```python
 from points_table_simulator import PointsTableSimulator
 import pandas as pd
 
 # Load the tournament schedule DataFrame
 tournament_schedule = pd.read_csv("tournament_schedule.csv")
 
@@ -41,21 +43,26 @@
 simulator = PointsTableSimulator(
     tournament_schedule=tournament_schedule,
     points_for_a_win=3,
     points_for_a_no_result=1,
     points_for_a_draw=1
 )
 
-# Calculate the current points table
-current_table = simulator.current_points_table()
+# Get the current points table
+current_table = simulator.current_points_table      # current_points_table is an attribute of PointsTableSimulator class
 
 # Simulate qualification scenarios for a specific team
 points_tables, qualification_match_results = simulator.simulate_the_qualification_scenarios(
     team_name="Team A",
     top_x_position_in_the_table=4,
     desired_number_of_scenarios=5
 )
 
 # points_tables - will return the list of points_tables (pd.Dataframe) for different qualification scenarios
 # qualification_match_results - will return the list of table containing remaining match outcomes which could favour their team to get qualified for the given position
 ```
 
+>This package can also be used in Football tournaments such as English Premier League (EPL), Laliga, etc., when you want to generate the scenarios in which your favourite team can be placed in your expected position in the pointstable.
+
+## License
+
+[MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `points-table-simulator-1.0.0/pyproject.toml` & `points_table_simulator-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `points-table-simulator-1.0.0/setup.cfg` & `points_table_simulator-1.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `points-table-simulator-1.0.0/src/points_table_simulator/exceptions.py` & `points_table_simulator-1.1.0/src/points_table_simulator/exceptions.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,42 +13,47 @@
 
 
 class InvalidColumnNamesError(ValueError):
     """
     Custom error class for invalid column names in the tournament schedule DataFrame.
     """
 
-    def __init__(self, column_name):
+    def __init__(self, column_name: str, column_value: str):
         self.column_name = column_name
-        super().__init__(f"{column_name} is not found in tournament_schedule columns")
+        self.column_value = column_value
+        super().__init__(f"{column_name} '{column_value}' is not found in given tournament_schedule columns")
 
 
 class InvalidScheduleDataError(ValueError):
     """Exception raised when the input schedule dataframe is invalid."""
 
-    def __init__(self, message="Invalid schedule data"):
-        self.message = message
-        super().__init__(self.message)
+    def __init__(self, column_name: str):
+        self.column_name = column_name
+        super().__init__(f"the given schedule contains rows with empty values or NaN in the {column_name} column")
 
 
 class NoQualifyingScenariosError(Exception):
     """Exception raised when no qualifying scenarios are found for the given team."""
 
-    def __init__(self, message="No qualifying scenarios found"):
-        self.message = message
-        super().__init__(self.message)
+    def __init__(self, points_table_position: int, team_name: str):
+        self.points_table_position = points_table_position
+        self.team_name = team_name
+        super().__init__(f"No qualifying scenarios found for team '{team_name}' at position {points_table_position}")
 
 
 class TeamNotFoundError(Exception):
     """Exception raised when the team is not found in the tournament schedule."""
 
     def __init__(self, message="Team not found in tournament schedule"):
         self.message = message
         super().__init__(self.message)
 
 
 class TournamentCompletionBelowCutoffError(Exception):
     """Exception raised when the percentage of tournament completion is below the specified cutoff."""
 
-    def __init__(self, message="Percentage of tournament completion is below the specified cutoff."):
-        self.message = message
-        super().__init__(self.message)
+    def __init__(self, cutoff_percentage: float, tournament_completion_percentage: float):
+        self.cutoff_percentage = cutoff_percentage
+        self.tournament_completion_percentage = tournament_completion_percentage
+        super().__init__(
+            f"Tournament completion percentage is {tournament_completion_percentage}%, which is less than the specified cutoff of {self.cutoff_percentage}%"
+        )
```

### Comparing `points-table-simulator-1.0.0/src/points_table_simulator/points_table_simulator.py` & `points_table_simulator-1.1.0/src/points_table_simulator/points_table_simulator.py`

 * *Files 10% similar despite different names*

```diff
@@ -49,26 +49,26 @@
 Author:
     Nishanth Muruganantham
     email: nishanthmurugananth10@gmail.com
 
 """
 
 import itertools
-from typing import Dict, List, Tuple
+from typing import Dict, List, Tuple, Union
 import pandas as pd
-from points_table_simulator.constants import (
-    TOURNAMENT_COMPLETION_CUTOFF_PERCENTAGE
-)
-from points_table_simulator.exceptions import (
+from points_table_simulator import (
     InvalidColumnNamesError,
     InvalidScheduleDataError,
     NoQualifyingScenariosError,
     TeamNotFoundError,
     TournamentCompletionBelowCutoffError
 )
+from points_table_simulator.constants import (
+    TOURNAMENT_COMPLETION_CUTOFF_PERCENTAGE
+)
 
 
 class PointsTableSimulator:     # pylint: disable = too-many-instance-attributes
 
     """
     PointsTableSimulator
 
@@ -153,14 +153,26 @@
         self.tournament_schedule_home_team_column_name: str = tournament_schedule_home_team_column_name
         self.tournament_schedule_match_number_column_name: str = tournament_schedule_match_number_column_name
         self.tournament_schedule_winning_team_column_name: str = tournament_schedule_winning_team_column_name
         self._validate_schedule_dataframe_columns()
         self._validate_schedule_dataframe_data()
 
     @property
+    def available_teams_in_fixture(self) -> set[str]:
+        """
+        Returns a set of available teams in the tournament schedule.
+
+        Returns:
+            set: Set of available teams in the tournament schedule.
+        """
+        return set(self.tournament_schedule[self.tournament_schedule_away_team_column_name].unique()).union(
+            set(self.tournament_schedule[self.tournament_schedule_home_team_column_name].unique())
+        )
+
+    @property
     def current_points_table(self) -> pd.DataFrame:
         """
         Calculates the current points table based on the provided tournament schedule.
 
         Returns:
             pd.DataFrame: DataFrame containing the current points table with the following columns:
                 - 'team': The name of the team.
@@ -171,19 +183,15 @@
                 - 'matches_with_no_result': The total number of matches with no result for the team.
                 - 'remaining_matches': The total number of remaining matches for the team.
                 - 'points': The total points earned by the team based on wins, draws, and no results.
         """
 
         team_points_data: List = []
 
-        teams: set = set(self.tournament_schedule[self.tournament_schedule_away_team_column_name].unique()).union(
-            set(self.tournament_schedule[self.tournament_schedule_home_team_column_name].unique())
-        )
-
-        for team in teams:
+        for team in self.available_teams_in_fixture:
             matches_played: int = len(self.tournament_schedule[
                 (
                     (self.tournament_schedule[self.tournament_schedule_away_team_column_name] == team) |
                     (self.tournament_schedule[self.tournament_schedule_home_team_column_name] == team)
                 ) &
                 (
                     (self.tournament_schedule[self.tournament_schedule_winning_team_column_name].fillna("") != "")
@@ -243,14 +251,35 @@
 
         current_points_table = pd.DataFrame(team_points_data)
         current_points_table.sort_values(by="points", ascending=False, inplace=True)
         current_points_table.reset_index(drop=True, inplace=True)
 
         return current_points_table
 
+    @property
+    def remaining_matches(self) -> List[Tuple[str, str]]:
+        """
+        Returns a list of tuples containing the remaining fixture matches in the tournament schedule.
+
+        Returns:
+            List[Tuple[str, str]]: List of tuples containing the remaining matches in the tournament schedule.
+        """
+        remaining_matches_df = self.tournament_schedule[
+            self.tournament_schedule[self.tournament_schedule_winning_team_column_name].fillna("") == ""
+        ]
+        remaining_matches = list(remaining_matches_df.apply(
+            lambda row: (row[self.tournament_schedule_home_team_column_name], row[self.tournament_schedule_away_team_column_name]),
+            axis=1
+        ))
+        return remaining_matches
+
+    @property
+    def various_probable_outcomes_for_remaining_matches(self) -> itertools.product:
+        return itertools.product(*self.remaining_matches)
+
     def simulate_the_qualification_scenarios(
         self, team_name: str, top_x_position_in_the_table: int, desired_number_of_scenarios: int = 3
     ) -> Tuple[List[pd.DataFrame], List[pd.DataFrame]]:
         """
         Finds qualification scenarios for a specified team to reach the desired position in the points table.
 
         This function simulates various match result scenarios for the remaining matches in the tournament schedule
@@ -285,73 +314,90 @@
                 print(qualification_match_results[i])
                 print("\n")
         """
 
         self._validate_the_inputs_for_simulate_qualification_scenarios(
             team_name, top_x_position_in_the_table, desired_number_of_scenarios
         )
+        self._check_for_minimal_tournament_completion()
         list_of_points_tables_for_qualification_scenarios = []
         list_of_remaining_match_result_for_qualification_scenarios = []
 
-        remaining_matches_in_the_schedule = self._find_remaining_matches_in_the_schedule()
-        number_of_completed_matches: int = len(self.tournament_schedule) - len(remaining_matches_in_the_schedule)
-        remaining_schedule_df: pd.DataFrame = self.tournament_schedule.iloc[
-            number_of_completed_matches:, :
-        ]
-
-        initial_points_table = self.current_points_table
-
-        for possible_results_for_remaining_matches in itertools.product(*remaining_matches_in_the_schedule):
-            temporary_schedule_df = remaining_schedule_df.copy()
-            updated_points_table = initial_points_table.copy()
-
-            for match_number, possible_winning_team in enumerate(possible_results_for_remaining_matches):
-                home_team, away_team = remaining_matches_in_the_schedule[match_number]
-                temporary_schedule_df.loc[
-                    number_of_completed_matches + match_number,
-                    self.tournament_schedule_winning_team_column_name
-                ] = possible_winning_team
-                updated_points_table = self._update_points_table(
-                    updated_points_table, home_team, away_team, possible_winning_team
-                )
-
-            updated_points_table.sort_values(by="points", ascending=False, inplace=True)
-            updated_points_table.reset_index(drop=True, inplace=True)
-
-            if team_name in updated_points_table["team"].values[:top_x_position_in_the_table]:
+        for tuple_of_remaining_match_results in self.various_probable_outcomes_for_remaining_matches:
+            _is_favourable_scenario = self._check_the_given_scenario_for_favourable_outcome(
+                team_name, top_x_position_in_the_table, tuple_of_remaining_match_results
+            )
+            if _is_favourable_scenario:
+                updated_points_table, temporary_schedule_df = _is_favourable_scenario
                 list_of_points_tables_for_qualification_scenarios.append(updated_points_table)
                 list_of_remaining_match_result_for_qualification_scenarios.append(temporary_schedule_df)
 
             if len(list_of_points_tables_for_qualification_scenarios) >= desired_number_of_scenarios:
                 break
 
         if not list_of_points_tables_for_qualification_scenarios:
-            raise NoQualifyingScenariosError(
-                f"No qualifying scenarios found for the team '{team_name}' in the top '{top_x_position_in_the_table}' positions."
-            )
+            raise NoQualifyingScenariosError(top_x_position_in_the_table, team_name)
 
         return list_of_points_tables_for_qualification_scenarios, list_of_remaining_match_result_for_qualification_scenarios
 
-    def _find_remaining_matches_in_the_schedule(self) -> List[Tuple[str, str]]:
-        remaining_matches_df = self.tournament_schedule[
-            self.tournament_schedule[self.tournament_schedule_winning_team_column_name].fillna("") == ""
-        ]
-        remaining_matches = list(remaining_matches_df.apply(
-            lambda row: (row[self.tournament_schedule_home_team_column_name], row[self.tournament_schedule_away_team_column_name]),
-            axis=1
-        ))
-        total_matches_in_the_schedule = len(self.tournament_schedule)
-        completed_matches = total_matches_in_the_schedule - len(remaining_matches)
-        tournament_completion_percentage = (completed_matches / total_matches_in_the_schedule) * 100
+    def _check_for_minimal_tournament_completion(self) -> None:
+        """
+        Checks if the percentage of tournament completion is below the specified cutoff.
+
+        Raises:
+            TournamentCompletionBelowCutoffError: Exception raised when the percentage of tournament completion is below the specified cutoff.
+        """
+        tournament_completion_percentage = (
+            (len(self.tournament_schedule) - len(self.remaining_matches)) / len(self.tournament_schedule)
+        ) * 100
         if tournament_completion_percentage < TOURNAMENT_COMPLETION_CUTOFF_PERCENTAGE:
-            raise TournamentCompletionBelowCutoffError(
-                f"This utility cannot be used at this stage, since the tournament completion percentage is {tournament_completion_percentage:.2f}%, \
-                    which is below the cutoff percentage of {TOURNAMENT_COMPLETION_CUTOFF_PERCENTAGE}%."
+            raise TournamentCompletionBelowCutoffError(TOURNAMENT_COMPLETION_CUTOFF_PERCENTAGE, round(tournament_completion_percentage, 2))
+
+    def _check_the_given_scenario_for_favourable_outcome(
+        self, team_name: str, top_x_position_in_the_table:int, tuple_of_remaining_match_results: Tuple[str]
+    ) -> Union[Tuple[pd.DataFrame, pd.DataFrame], None]:
+        """
+        Checks if the given scenario is favourable for the specified team.
+
+        This function iterates through all possible combinations of match results for the remaining matches
+        in the tournament schedule. For each combination, it calculates the updated points table and checks
+        if the specified team qualifies within the top X positions. Once enough qualifying scenarios are found
+        based on the desired number of scenarios, the function stops iterating and returns the results.
+
+        Returns:
+            Union[Tuple[pd.DataFrame, pd.DataFrame], None]: A tuple containing two dataframes:
+                - The updated points table for the given scenario.
+                - The remaining match outcome for the given scenario.
+        """
+        number_of_completed_matches: int = len(self.tournament_schedule) - len(self.remaining_matches)
+        remaining_schedule_df: pd.DataFrame = self.tournament_schedule.iloc[
+            number_of_completed_matches:, :
+        ]
+        initial_points_table = self.current_points_table
+
+        temporary_schedule_df = remaining_schedule_df.copy()
+        updated_points_table = initial_points_table.copy()
+
+        for match_number, possible_winning_team in enumerate(tuple_of_remaining_match_results):
+            home_team, away_team = self.remaining_matches[match_number]
+            temporary_schedule_df.loc[
+                number_of_completed_matches + match_number,
+                self.tournament_schedule_winning_team_column_name
+            ] = possible_winning_team
+            updated_points_table = self._update_points_table(
+                updated_points_table, home_team, away_team, possible_winning_team
             )
-        return remaining_matches
+
+        updated_points_table.sort_values(by="points", ascending=False, inplace=True)
+        updated_points_table.reset_index(drop=True, inplace=True)
+
+        if team_name in updated_points_table["team"].values[:top_x_position_in_the_table]:
+            return updated_points_table, temporary_schedule_df
+
+        return None
 
     def _update_points_table(
         self, points_table: pd.DataFrame, home_team: str, away_team: str, winning_team: str
     ) -> pd.DataFrame:
         points_table.loc[points_table["team"] == winning_team, "matches_won"] += 1
         points_table.loc[points_table['team'] == winning_team, 'points'] += self.points_for_a_win
         points_table.loc[points_table['team'] == home_team, 'matches_played'] += 1
@@ -412,26 +458,24 @@
             "tournament_schedule_home_team_column_name": self.tournament_schedule_home_team_column_name,
             "tournament_schedule_match_number_column_name": self.tournament_schedule_match_number_column_name,
             "tournament_schedule_winning_team_column_name": self.tournament_schedule_winning_team_column_name,
         }
         schedule_dataframe_columns = self.tournament_schedule.columns
         for column_name, column_value in _column_map.items():
             if column_value not in schedule_dataframe_columns:
-                raise InvalidColumnNamesError(f"{column_name} '{column_value}' is not found in given tournament_schedule columns")
+                raise InvalidColumnNamesError(column_name, column_value)
 
     def _validate_schedule_dataframe_data(self):
         for column in (
             self.tournament_schedule_away_team_column_name,
             self.tournament_schedule_home_team_column_name,
             self.tournament_schedule_match_number_column_name,
         ):
             if bool(self.tournament_schedule[column].isnull().any()):
-                raise InvalidScheduleDataError(
-                    f"the given schedule contains rows with empty values or NaN in the {column} column"
-                )
+                raise InvalidScheduleDataError(column)
 
     def _validate_the_inputs_for_simulate_qualification_scenarios(
         self, team_name: str, top_x_position_in_the_table: int, desired_number_of_scenarios: int
     ):
         _type_map: Dict[str, type] = {
             "team_name": str,
             "top_x_position_in_the_table": int,
@@ -440,13 +484,13 @@
         for key, value in _type_map.items():
             if not isinstance(locals()[key], value):
                 raise TypeError(f"'{key}' must be a '{value}'")
         if desired_number_of_scenarios <= 0:
             raise ValueError("'desired_number_of_scenarios' must be greater than 0")
         if top_x_position_in_the_table <= 0:
             raise ValueError("'top_x_position_in_the_table' must be greater than 0")
-        if team_name not in self.current_points_table["team"].values:
+        if team_name not in self.available_teams_in_fixture:
             raise TeamNotFoundError(f"'{team_name}' is not found in the current points table or in the given schedule")
         if top_x_position_in_the_table > len(self.current_points_table):
             raise ValueError(
                 "'top_x_position_in_the_table' must be less than or equal to the number of teams in the table"
             )
```

### Comparing `points-table-simulator-1.0.0/src/points_table_simulator.egg-info/PKG-INFO` & `points_table_simulator-1.1.0/src/points_table_simulator.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: points-table-simulator
-Version: 1.0.0
+Version: 1.1.0
 Summary: This package will simulate the points table based on different possible results in a sports tournament
 Home-page: https://github.com/NishanthMuruganantham/points-table-simulator
 Author: Nishanth Muruganantham
 Author-email: nishanthmurugananth10@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -15,28 +15,30 @@
 
 During the later part of the league stages in many multi-team tournaments 🏆 such as 🏏 Indian Premier League(IPL), Australian Big Bash League (BBL), ets., the fans will look for possible match outcomes for the remaining league matches, which could lead their favourite team to get qualified for further stage in the tournament (Playoffs). Here, the fans calculate their points table📊 to see their favourite team being placed in the position needed to qualify for Playoffs🏃🏻.
 
 This tool🛠️ come as handy for those Sports enthusiasts which would help them to forsee the necessary remaining match outcomes to see their favourite team qualifying for playoffs✅ with the necessary match outcomes along with the respective points table📊.
 
 <hr>
 
-This package📦 will simulate the points table📊 based on different possible results in a sports tournament.
+This python package📦 will simulate the points table📊 based on different possible results in a sports tournament.
 
 The PointsTableSimulator package provides a powerful tool for simulating and analyzing points tables for sports tournaments. Whether you're organizing or following a tournament, this package offers the flexibility to input tournament schedules, define points systems, and explore various match outcome scenarios to understand team standings and qualification possibilities.
 
 ## Installation
 
-Install my-project with npm
+Install this package with pip
 
 ```
 pip install points-table-simulator
 ```
     
 ## Usage/Examples
 
+Please find the example usage from the below python code
+
 ```python
 from points_table_simulator import PointsTableSimulator
 import pandas as pd
 
 # Load the tournament schedule DataFrame
 tournament_schedule = pd.read_csv("tournament_schedule.csv")
 
@@ -54,21 +56,26 @@
 simulator = PointsTableSimulator(
     tournament_schedule=tournament_schedule,
     points_for_a_win=3,
     points_for_a_no_result=1,
     points_for_a_draw=1
 )
 
-# Calculate the current points table
-current_table = simulator.current_points_table()
+# Get the current points table
+current_table = simulator.current_points_table      # current_points_table is an attribute of PointsTableSimulator class
 
 # Simulate qualification scenarios for a specific team
 points_tables, qualification_match_results = simulator.simulate_the_qualification_scenarios(
     team_name="Team A",
     top_x_position_in_the_table=4,
     desired_number_of_scenarios=5
 )
 
 # points_tables - will return the list of points_tables (pd.Dataframe) for different qualification scenarios
 # qualification_match_results - will return the list of table containing remaining match outcomes which could favour their team to get qualified for the given position
 ```
 
+>This package can also be used in Football tournaments such as English Premier League (EPL), Laliga, etc., when you want to generate the scenarios in which your favourite team can be placed in your expected position in the pointstable.
+
+## License
+
+[MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `points-table-simulator-1.0.0/src/points_table_simulator.egg-info/SOURCES.txt` & `points_table_simulator-1.1.0/src/points_table_simulator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `points-table-simulator-1.0.0/tests/points_table_simulator_tests/data/psl_2024_fixture.csv` & `points_table_simulator-1.1.0/tests/points_table_simulator_tests/data/psl_2024_fixture.csv`

 * *Files identical despite different names*

### Comparing `points-table-simulator-1.0.0/tests/points_table_simulator_tests/error_tests.py` & `points_table_simulator-1.1.0/tests/points_table_simulator_tests/error_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from unittest import TestCase
 import pandas as pd
-from points_table_simulator.exceptions import (
+from points_table_simulator import (
     InvalidColumnNamesError,
     InvalidScheduleDataError,
     NoQualifyingScenariosError,
+    PointsTableSimulator,
     TeamNotFoundError,
     TournamentCompletionBelowCutoffError
 )
-from points_table_simulator.points_table_simulator import PointsTableSimulator
 
 
 class ErrorTests(TestCase):
 
     """
         This class contains tests for the errors raised by the PointsTableSimulator class. It covers both default exceptions and custom exceptions.
     """
```

### Comparing `points-table-simulator-1.0.0/tests/points_table_simulator_tests/success_tests.py` & `points_table_simulator-1.1.0/tests/points_table_simulator_tests/success_tests.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from unittest import TestCase
 import pandas as pd
-from points_table_simulator.points_table_simulator import PointsTableSimulator
+from points_table_simulator import PointsTableSimulator
 
 
 class SuccessTests(TestCase):
 
     test_data_folder = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'data')
 
     def test_simulate_the_qualification_scenarios_function_with_psl_2024_fixture(self):
```

