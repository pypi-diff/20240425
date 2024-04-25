# Comparing `tmp/eflips_depot-3.0.4.tar.gz` & `tmp/eflips_depot-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eflips_depot-3.0.4.tar", max compression
+gzip compressed data, was "eflips_depot-3.0.5.tar", max compression
```

## Comparing `eflips_depot-3.0.4.tar` & `eflips_depot-3.0.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    34143 2023-09-12 12:04:52.313847 eflips_depot-3.0.4/LICENSE.md
--rw-r--r--   0        0        0     4923 2024-01-30 11:53:09.584369 eflips_depot-3.0.4/README.md
--rw-r--r--   0        0        0     1556 2023-09-18 10:32:47.648700 eflips_depot-3.0.4/eflips/depot/__init__.py
--rw-r--r--   0        0        0    49861 2024-04-22 15:47:52.732246 eflips_depot-3.0.4/eflips/depot/api/__init__.py
--rw-r--r--   0        0        0     5375 2024-03-19 13:55:55.791236 eflips_depot-3.0.4/eflips/depot/api/defaults/default_settings.json
--rw-r--r--   0        0        0        0 2024-03-20 16:37:13.222393 eflips_depot-3.0.4/eflips/depot/api/private/__init__.py
--rw-r--r--   0        0        0    17136 2024-04-17 13:40:18.399085 eflips_depot-3.0.4/eflips/depot/api/private/depot.py
--rw-r--r--   0        0        0    15261 2024-03-20 16:37:13.222833 eflips_depot-3.0.4/eflips/depot/api/private/util.py
--rw-r--r--   0        0        0    35678 2024-03-19 13:55:55.792840 eflips_depot-3.0.4/eflips/depot/configuration.py
--rw-r--r--   0        0        0   105566 2024-04-08 08:44:07.632864 eflips_depot-3.0.4/eflips/depot/depot.py
--rw-r--r--   0        0        0   140842 2024-03-19 13:55:55.793916 eflips_depot-3.0.4/eflips/depot/evaluation.py
--rw-r--r--   0        0        0    16131 2024-04-17 12:44:22.875673 eflips_depot-3.0.4/eflips/depot/filters.py
--rw-r--r--   0        0        0     5569 2023-09-12 07:17:14.199982 eflips_depot-3.0.4/eflips/depot/input_epex_power_price.py
--rw-r--r--   0        0        0        0 2023-07-04 10:37:34.116338 eflips_depot-3.0.4/eflips/depot/layout_opt/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 10:37:34.116399 eflips_depot-3.0.4/eflips/depot/layout_opt/doc/__init__.py
--rw-r--r--   0        0        0    22330 2023-07-04 10:37:34.116540 eflips_depot-3.0.4/eflips/depot/layout_opt/doc/direct_details.pdf
--rw-r--r--   0        0        0    24855 2023-11-27 13:13:21.354478 eflips_depot-3.0.4/eflips/depot/layout_opt/evaluation.py
--rw-r--r--   0        0        0      594 2023-09-12 07:17:14.200220 eflips_depot-3.0.4/eflips/depot/layout_opt/opt_tools/__init__.py
--rw-r--r--   0        0        0     1057 2023-07-04 10:37:34.116782 eflips_depot-3.0.4/eflips/depot/layout_opt/opt_tools/crossover.py
--rw-r--r--   0        0        0     8230 2024-03-19 13:55:55.794538 eflips_depot-3.0.4/eflips/depot/layout_opt/opt_tools/fitness_c_urfd.py
--rw-r--r--   0        0        0     7027 2024-03-19 13:55:55.794746 eflips_depot-3.0.4/eflips/depot/layout_opt/opt_tools/fitness_util.py
--rw-r--r--   0        0        0    14707 2023-09-18 10:44:13.136159 eflips_depot-3.0.4/eflips/depot/layout_opt/opt_tools/init.py
--rw-r--r--   0        0        0    12238 2023-09-18 10:44:13.095315 eflips_depot-3.0.4/eflips/depot/layout_opt/opt_tools/mutation.py
--rw-r--r--   0        0        0     9821 2023-11-27 13:13:21.355200 eflips_depot-3.0.4/eflips/depot/layout_opt/optimize_c_urfd.py
--rw-r--r--   0        0        0    56989 2023-11-27 13:13:21.355852 eflips_depot-3.0.4/eflips/depot/layout_opt/packing.py
--rw-r--r--   0        0        0      810 2023-09-12 07:17:14.201273 eflips_depot-3.0.4/eflips/depot/layout_opt/settings.py
--rw-r--r--   0        0        0     9736 2023-09-18 10:44:13.156260 eflips_depot-3.0.4/eflips/depot/layout_opt/template_creation.py
--rw-r--r--   0        0        0     3780 2023-09-18 10:44:13.048607 eflips_depot-3.0.4/eflips/depot/layout_opt/util.py
--rw-r--r--   0        0        0     2509 2023-10-26 12:56:09.063373 eflips_depot-3.0.4/eflips/depot/plots.py
--rw-r--r--   0        0        0    58757 2024-04-08 08:44:07.633396 eflips_depot-3.0.4/eflips/depot/processes.py
--rw-r--r--   0        0        0    16648 2023-09-18 10:44:12.914701 eflips_depot-3.0.4/eflips/depot/rating.py
--rw-r--r--   0        0        0    13568 2024-01-15 15:15:16.955650 eflips_depot-3.0.4/eflips/depot/resources.py
--rw-r--r--   0        0        0     2527 2023-09-24 11:00:36.366976 eflips_depot-3.0.4/eflips/depot/settings_config.py
--rw-r--r--   0        0        0     9375 2023-10-09 12:48:51.301551 eflips_depot-3.0.4/eflips/depot/simple_vehicle.py
--rw-r--r--   0        0        0    10676 2024-03-20 16:37:13.224092 eflips_depot-3.0.4/eflips/depot/simulation.py
--rw-r--r--   0        0        0    54311 2023-11-27 13:13:21.357629 eflips_depot-3.0.4/eflips/depot/smart_charging.py
--rw-r--r--   0        0        0    22338 2023-11-13 11:10:33.262925 eflips_depot-3.0.4/eflips/depot/standalone.py
--rw-r--r--   0        0        0     7097 2023-09-18 10:44:13.235715 eflips_depot-3.0.4/eflips/depot/validation.py
--rw-r--r--   0        0        0     1215 2024-04-22 15:47:52.732722 eflips_depot-3.0.4/pyproject.toml
--rw-r--r--   0        0        0     5833 1970-01-01 00:00:00.000000 eflips_depot-3.0.4/PKG-INFO
+-rw-r--r--   0        0        0    34143 2024-04-25 09:28:48.912686 eflips_depot-3.0.5/LICENSE.md
+-rw-r--r--   0        0        0     4899 2024-04-25 09:28:48.912686 eflips_depot-3.0.5/README.md
+-rw-r--r--   0        0        0     1556 2024-04-25 09:28:48.912686 eflips_depot-3.0.5/eflips/depot/__init__.py
+-rw-r--r--   0        0        0    51939 2024-04-25 09:28:48.912686 eflips_depot-3.0.5/eflips/depot/api/__init__.py
+-rw-r--r--   0        0        0     5375 2024-04-25 09:28:48.912686 eflips_depot-3.0.5/eflips/depot/api/defaults/default_settings.json
+-rw-r--r--   0        0        0        0 2024-04-25 09:28:48.912686 eflips_depot-3.0.5/eflips/depot/api/private/__init__.py
+-rw-r--r--   0        0        0    17136 2024-04-25 09:28:48.912686 eflips_depot-3.0.5/eflips/depot/api/private/depot.py
+-rw-r--r--   0        0        0    15362 2024-04-25 09:28:48.912686 eflips_depot-3.0.5/eflips/depot/api/private/util.py
+-rw-r--r--   0        0        0    35678 2024-04-25 09:28:48.912686 eflips_depot-3.0.5/eflips/depot/configuration.py
+-rw-r--r--   0        0        0   105566 2024-04-25 09:28:48.912686 eflips_depot-3.0.5/eflips/depot/depot.py
+-rw-r--r--   0        0        0   140842 2024-04-25 09:28:48.912686 eflips_depot-3.0.5/eflips/depot/evaluation.py
+-rw-r--r--   0        0        0    16131 2024-04-25 09:28:48.912686 eflips_depot-3.0.5/eflips/depot/filters.py
+-rw-r--r--   0        0        0     5569 2024-04-25 09:28:48.912686 eflips_depot-3.0.5/eflips/depot/input_epex_power_price.py
+-rw-r--r--   0        0        0        0 2024-04-25 09:28:48.912686 eflips_depot-3.0.5/eflips/depot/layout_opt/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 09:28:48.912686 eflips_depot-3.0.5/eflips/depot/layout_opt/doc/__init__.py
+-rw-r--r--   0        0        0    22330 2024-04-25 09:28:48.912686 eflips_depot-3.0.5/eflips/depot/layout_opt/doc/direct_details.pdf
+-rw-r--r--   0        0        0    24855 2024-04-25 09:28:48.912686 eflips_depot-3.0.5/eflips/depot/layout_opt/evaluation.py
+-rw-r--r--   0        0        0      594 2024-04-25 09:28:48.916686 eflips_depot-3.0.5/eflips/depot/layout_opt/opt_tools/__init__.py
+-rw-r--r--   0        0        0     1057 2024-04-25 09:28:48.916686 eflips_depot-3.0.5/eflips/depot/layout_opt/opt_tools/crossover.py
+-rw-r--r--   0        0        0     8230 2024-04-25 09:28:48.916686 eflips_depot-3.0.5/eflips/depot/layout_opt/opt_tools/fitness_c_urfd.py
+-rw-r--r--   0        0        0     7027 2024-04-25 09:28:48.916686 eflips_depot-3.0.5/eflips/depot/layout_opt/opt_tools/fitness_util.py
+-rw-r--r--   0        0        0    14707 2024-04-25 09:28:48.916686 eflips_depot-3.0.5/eflips/depot/layout_opt/opt_tools/init.py
+-rw-r--r--   0        0        0    12238 2024-04-25 09:28:48.916686 eflips_depot-3.0.5/eflips/depot/layout_opt/opt_tools/mutation.py
+-rw-r--r--   0        0        0     9821 2024-04-25 09:28:48.916686 eflips_depot-3.0.5/eflips/depot/layout_opt/optimize_c_urfd.py
+-rw-r--r--   0        0        0    56989 2024-04-25 09:28:48.916686 eflips_depot-3.0.5/eflips/depot/layout_opt/packing.py
+-rw-r--r--   0        0        0      810 2024-04-25 09:28:48.916686 eflips_depot-3.0.5/eflips/depot/layout_opt/settings.py
+-rw-r--r--   0        0        0     9736 2024-04-25 09:28:48.916686 eflips_depot-3.0.5/eflips/depot/layout_opt/template_creation.py
+-rw-r--r--   0        0        0     3780 2024-04-25 09:28:48.916686 eflips_depot-3.0.5/eflips/depot/layout_opt/util.py
+-rw-r--r--   0        0        0     2509 2024-04-25 09:28:48.916686 eflips_depot-3.0.5/eflips/depot/plots.py
+-rw-r--r--   0        0        0    58757 2024-04-25 09:28:48.916686 eflips_depot-3.0.5/eflips/depot/processes.py
+-rw-r--r--   0        0        0    16648 2024-04-25 09:28:48.916686 eflips_depot-3.0.5/eflips/depot/rating.py
+-rw-r--r--   0        0        0    13568 2024-04-25 09:28:48.916686 eflips_depot-3.0.5/eflips/depot/resources.py
+-rw-r--r--   0        0        0     2527 2024-04-25 09:28:48.916686 eflips_depot-3.0.5/eflips/depot/settings_config.py
+-rw-r--r--   0        0        0     9375 2024-04-25 09:28:48.916686 eflips_depot-3.0.5/eflips/depot/simple_vehicle.py
+-rw-r--r--   0        0        0    10676 2024-04-25 09:28:48.916686 eflips_depot-3.0.5/eflips/depot/simulation.py
+-rw-r--r--   0        0        0    54311 2024-04-25 09:28:48.916686 eflips_depot-3.0.5/eflips/depot/smart_charging.py
+-rw-r--r--   0        0        0    22338 2024-04-25 09:28:48.916686 eflips_depot-3.0.5/eflips/depot/standalone.py
+-rw-r--r--   0        0        0     7097 2024-04-25 09:28:48.916686 eflips_depot-3.0.5/eflips/depot/validation.py
+-rw-r--r--   0        0        0     1215 2024-04-25 09:28:48.916686 eflips_depot-3.0.5/pyproject.toml
+-rw-r--r--   0        0        0     5809 1970-01-01 00:00:00.000000 eflips_depot-3.0.5/PKG-INFO
```

### Comparing `eflips_depot-3.0.4/LICENSE.md` & `eflips_depot-3.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.4/README.md` & `eflips_depot-3.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![Tests](https://github.com/mpm-tu-berlin/eflips-depot/actions/workflows/postgres_eflips_depot.yml/badge.svg)](https://github.com/mpm-tu-berlin/eflips-depot/actions/workflows/postgres_eflips_depot.yml)
+[![Tests](https://github.com/mpm-tu-berlin/eflips-depot/actions/workflows/unittests.yml/badge.svg)](https://github.com/mpm-tu-berlin/eflips-depot/actions/workflows/unittests.yml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 
 # eflips-depot
 
 ---
```

### Comparing `eflips_depot-3.0.4/eflips/depot/__init__.py` & `eflips_depot-3.0.5/eflips/depot/__init__.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.4/eflips/depot/api/__init__.py` & `eflips_depot-3.0.5/eflips/depot/api/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -659,16 +659,14 @@
     # Read simulation start time
 
     for depot_evaluation in depot_evaluations.values():
         simulation_start_time = depot_evaluation.sim_start_datetime
 
         # Initialization of empty lists
 
-        list_of_vehicles = []
-
         list_of_assigned_schedules = []
 
         # Read results from depot_evaluation categorized by vehicle
         for current_vehicle in depot_evaluation.vehicle_generator.items:
             vehicle_type_id = int(current_vehicle.vehicle_type.ID)
 
             # Create a Vehicle object for database
@@ -677,320 +675,358 @@
                 scenario=scenario,
                 name=current_vehicle.ID,
                 name_short=None,
             )
             # Flush the vehicle object to get the vehicle id
             session.add(current_vehicle_db)
             session.flush()
-            list_of_vehicles.append(current_vehicle_db)
 
             dict_of_events = {}
 
-            # Generate process log for each schedule
-            for finished_trip in current_vehicle.finished_trips:
-                dict_of_events[finished_trip.atd] = {
-                    "type": "trip",
-                    "is_copy": finished_trip.is_copy,
-                    "id": finished_trip.ID,
-                }
+            # Generate process log for each
+            list_of_finished_trips = current_vehicle.finished_trips
+            list_of_finished_trips.sort(key=lambda x: x.atd)
+
+            for i in range(len(list_of_finished_trips)):
+                if list_of_finished_trips[i].is_copy is False:
+                    current_trip = list_of_finished_trips[i]
+
+                    # Add all non-copy trips to the dictionary
+                    dict_of_events[current_trip.atd] = {
+                        "type": "Trip",
+                        "end": current_trip.ata,
+                        "is_copy": current_trip.is_copy,
+                        "id": current_trip.ID,
+                    }
 
-                if finished_trip.is_copy is False:
-                    assigned_schedule_id = int(finished_trip.ID)
+                    # Match current trip to its serving vehicle
+                    assigned_schedule_id = int(current_trip.ID)
                     list_of_assigned_schedules.append(
                         (assigned_schedule_id, current_vehicle_db.id)
                     )
+                    # Also add two copy trips before and after the non-copy trip as "time boarders" for the depot process
+                    try:
+                        if list_of_finished_trips[i + 1].is_copy is True:
+                            dict_of_events[list_of_finished_trips[i + 1].atd] = {
+                                "type": "Trip",
+                                "end": list_of_finished_trips[i + 1].ata,
+                                "is_copy": list_of_finished_trips[i + 1].is_copy,
+                                "id": list_of_finished_trips[i + 1].ID,
+                            }
+
+                        if list_of_finished_trips[i - 1].is_copy is True:
+                            dict_of_events[list_of_finished_trips[i - 1].atd] = {
+                                "type": "Trip",
+                                "end": list_of_finished_trips[i - 1].ata,
+                                "is_copy": list_of_finished_trips[i - 1].is_copy,
+                                "id": list_of_finished_trips[i - 1].ID,
+                            }
+
+                    except IndexError:
+                        # In case there are no copy trips before or after the non-copy trip
+                        continue
 
-            # Generate a dictionary of data logs from DepotEvaluation with time as keys. Logs for repeated schedules
-            # and their depot processes are included but will not be written into database.
+            # The range of time of events to be generated. It is between the copy trip before the first non-copy trip and the
+            # copy trip after the last non-copy trip
+            earliest_time = sorted(dict_of_events.keys())[0]
+            latest_time = sorted(dict_of_events.keys())[-1]
 
             last_standby_departure_start = 0
 
             # For convenience
             area_log = current_vehicle.logger.loggedData["dwd.current_area"]
             slot_log = current_vehicle.logger.loggedData["dwd.current_slot"]
 
-            # For future uses
             waiting_log = current_vehicle.logger.loggedData["area_waiting_time"]
             battery_log = current_vehicle.battery_logs
 
             # Create standby events according to waiting_log
             waiting_log_timekeys = sorted(waiting_log.keys())
 
             for idx in range(len(waiting_log_timekeys)):
                 end_time = waiting_log_timekeys[idx]
-                waiting_info = waiting_log[end_time]
 
-                if waiting_info["waiting_time"] == 0:
-                    continue
+                # Only extract events if the time is within the upper mentioned range
+
+                if earliest_time < end_time < latest_time:
+                    waiting_info = waiting_log[end_time]
+
+                    if waiting_info["waiting_time"] == 0:
+                        continue
 
-                # Vehicle is waiting in the last area in waiting_log and expecting to enter the current area
-                expected_area = waiting_info["area"]
-                # Find the area for standby arrival event
-
-                waiting_area_id = (
-                    session.query(Area.id)
-                    .join(AssocAreaProcess, AssocAreaProcess.area_id == Area.id)
-                    .join(Process, Process.id == AssocAreaProcess.process_id)
-                    .filter(
-                        Process.dispatchable == False,
-                        Process.duration.is_(None),
-                        Process.electric_power.is_(None),
-                        Area.vehicle_type_id == int(current_vehicle.vehicle_type.ID),
-                        Area.scenario_id == scenario.id,
+                    # Vehicle is waiting in the last area in waiting_log and expecting to enter the current area
+                    expected_area = waiting_info["area"]
+                    # Find the area for standby arrival event
+
+                    waiting_area_id = (
+                        session.query(Area.id)
+                        .join(AssocAreaProcess, AssocAreaProcess.area_id == Area.id)
+                        .join(Process, Process.id == AssocAreaProcess.process_id)
+                        .filter(
+                            Process.dispatchable == False,
+                            # Must use "==" instead of "is". Or it would be recongnize as a python statement rather than a SQL statement
+                            Process.duration.is_(None),
+                            Process.electric_power.is_(None),
+                            Area.vehicle_type_id
+                            == int(current_vehicle.vehicle_type.ID),
+                            Area.scenario_id == scenario.id,
+                        )
+                        .one()[0]
                     )
-                    .one()[0]
-                )
 
-                # Make sure the vehicle is waiting at an area with enough capacity
+                    # Make sure the vehicle is waiting at an area with enough capacity
+
+                    current_slot = slot_log[waiting_log_timekeys[idx - 1]]
 
-                current_slot = slot_log[waiting_log_timekeys[idx - 1]]
+                    start_time = end_time - waiting_info["waiting_time"]
 
-                start_time = end_time - waiting_info["waiting_time"]
+                    warnings.warn(
+                        f"Vehicle {current_vehicle.ID} is waiting at {waiting_area_id} because area {expected_area} is full."
+                    )
 
-                warnings.warn(
-                    f"Vehicle {current_vehicle.ID} is waiting at {waiting_area_id} because area {expected_area} is full."
-                )
-
-                dict_of_events[start_time] = {
-                    "type": "Standby",
-                    "end": end_time,
-                    "area": waiting_area_id,
-                    "slot": current_slot,
-                    "is_area_sink": False,
-                }
+                    dict_of_events[start_time] = {
+                        "type": "Standby",
+                        "end": end_time,
+                        "area": waiting_area_id,
+                        "slot": current_slot,
+                        "is_area_sink": False,
+                    }
 
             # Create a list of battery log in order of time asc. Convenient for looking up corresponding soc
             battery_log_list = []
             for log in battery_log:
                 battery_log_list.append((log.t, log.energy / log.energy_real))
 
             for start_time, process_log in current_vehicle.logger.loggedData[
                 "dwd.active_processes_copy"
             ].items():
-                if len(process_log) == 0:
-                    # A departure happens
-                    if last_standby_departure_start != 0:
-                        # Update the last standby-departure end time
-                        dict_of_events[last_standby_departure_start]["end"] = start_time
-                    else:
-                        continue
+                if earliest_time < start_time < latest_time:
+                    if len(process_log) == 0:
+                        # A departure happens
+                        if last_standby_departure_start != 0:
+                            # Update the last standby-departure end time
+                            dict_of_events[last_standby_departure_start][
+                                "end"
+                            ] = start_time
+                        else:
+                            continue
 
-                else:
-                    for process in process_log:
-                        match process.status:
-                            case ProcessStatus.COMPLETED | ProcessStatus.CANCELLED:
-                                assert (
-                                    len(process.starts) == 1 and len(process.ends) == 1
-                                ), (
-                                    f"Current process {process.ID} is completed and should only contain one start and "
-                                    f"one end time."
-                                )
-                                current_area = area_log[start_time]
-                                current_slot = slot_log[start_time]
-
-                                if current_area is None or current_slot is None:
-                                    raise ValueError(
-                                        f"For process {process.ID} Area and slot should not be None."
+                    else:
+                        for process in process_log:
+                            match process.status:
+                                case ProcessStatus.COMPLETED | ProcessStatus.CANCELLED:
+                                    assert (
+                                        len(process.starts) == 1
+                                        and len(process.ends) == 1
+                                    ), (
+                                        f"Current process {process.ID} is completed and should only contain one start and "
+                                        f"one end time."
                                     )
+                                    current_area = area_log[start_time]
+                                    current_slot = slot_log[start_time]
 
-                                if process.dur > 0:
-                                    # Valid duration
-                                    dict_of_events[start_time] = {
-                                        "type": type(process).__name__,
-                                        "end": process.ends[0],
-                                        "area": current_area.ID,
-                                        "slot": current_slot,
-                                        "id": process.ID,
-                                    }
-                                else:
-                                    # Duration is 0
-                                    if current_area.issink is True:
-                                        # Standby departure
-                                        if start_time in dict_of_events:
-                                            # Actual start time should be the end time of the other positive duration
-                                            # process starting at the same time
-                                            actual_start_time = dict_of_events[
-                                                start_time
-                                            ]["end"]
-                                        else:
-                                            for other_process in process_log:
-                                                if (
-                                                    other_process.dur > 0
-                                                    and len(other_process.ends) != 0
-                                                ):
-                                                    actual_start_time = (
-                                                        other_process.ends[0]
-                                                    )
-                                                else:
-                                                    # Invalid standby before a process in progress will be ignored
-                                                    continue
-
-                                        last_standby_departure_start = actual_start_time
-
-                                        # If this standby event lasts actually 0 seconds, it is not a real event
-                                        if (
-                                            actual_start_time in dict_of_events.keys()
-                                            and dict_of_events[actual_start_time][
-                                                "type"
-                                            ]
-                                            == "trip"
-                                        ):
-                                            continue
-                                        dict_of_events[actual_start_time] = {
+                                    if current_area is None or current_slot is None:
+                                        raise ValueError(
+                                            f"For process {process.ID} Area and slot should not be None."
+                                        )
+
+                                    if process.dur > 0:
+                                        # Valid duration
+                                        dict_of_events[start_time] = {
                                             "type": type(process).__name__,
+                                            "end": process.ends[0],
                                             "area": current_area.ID,
-                                            "is_area_sink": current_area.issink,
                                             "slot": current_slot,
                                             "id": process.ID,
                                         }
-
                                     else:
-                                        # Standby arrival
-                                        assert current_area.issink is False, (
-                                            f"A bus cannot go from Area {current_area.ID} to other areas. A Parking Area"
-                                            f" for standby arrival should be added."
+                                        # Duration is 0
+                                        if current_area.issink is True:
+                                            # Standby departure
+                                            if start_time in dict_of_events:
+                                                # Actual start time should be the end time of the other positive
+                                                # duration process starting at the same time
+                                                actual_start_time = dict_of_events[
+                                                    start_time
+                                                ]["end"]
+                                            else:
+                                                for other_process in process_log:
+                                                    if (
+                                                        other_process.dur > 0
+                                                        and len(other_process.ends) != 0
+                                                    ):
+                                                        actual_start_time = (
+                                                            other_process.ends[0]
+                                                        )
+                                                    else:
+                                                        # Invalid standby before a process in progress will be ignored
+                                                        continue
+
+                                            last_standby_departure_start = (
+                                                actual_start_time
+                                            )
+
+                                            # If this standby event lasts actually 0 seconds, it is not a real event
+                                            if (
+                                                actual_start_time
+                                                in dict_of_events.keys()
+                                                and dict_of_events[actual_start_time][
+                                                    "type"
+                                                ]
+                                                == "Trip"
+                                            ):
+                                                continue
+                                            dict_of_events[actual_start_time] = {
+                                                "type": type(process).__name__,
+                                                "area": current_area.ID,
+                                                "is_area_sink": current_area.issink,
+                                                "slot": current_slot,
+                                                "id": process.ID,
+                                            }
+
+                                        else:
+                                            # Standby arrival
+                                            assert current_area.issink is False, (
+                                                f"A bus cannot go from Area {current_area.ID} to other areas. A Parking Area"
+                                                f" for standby arrival should be added."
+                                            )
+                                            dict_of_events[start_time] = {
+                                                "type": type(process).__name__,
+                                                "area": current_area.ID,
+                                                "is_area_sink": current_area.issink,
+                                                "slot": current_slot,
+                                                "id": process.ID,
+                                            }
+                                case ProcessStatus.IN_PROGRESS:
+                                    assert (
+                                        len(process.starts) == 1
+                                        and len(process.ends) == 0
+                                    ), f"Current process {process.ID} is marked IN_PROGRESS, but has an end."
+                                    current_area = area_log[start_time]
+                                    current_slot = slot_log[start_time]
+
+                                    if current_area is None or current_slot is None:
+                                        raise ValueError(
+                                            f"For process {process.ID} Area and slot should not be None."
                                         )
+
+                                    if process.dur > 0:
+                                        # Valid duration
                                         dict_of_events[start_time] = {
                                             "type": type(process).__name__,
+                                            "end": process.etc,
                                             "area": current_area.ID,
-                                            "is_area_sink": current_area.issink,
                                             "slot": current_slot,
                                             "id": process.ID,
                                         }
-                            case ProcessStatus.IN_PROGRESS:
-                                assert (
-                                    len(process.starts) == 1 and len(process.ends) == 0
-                                ), f"Current process {process.ID} is marked IN_PROGRESS, but has an end."
-                                current_area = area_log[start_time]
-                                current_slot = slot_log[start_time]
-
-                                if current_area is None or current_slot is None:
-                                    raise ValueError(
-                                        f"For process {process.ID} Area and slot should not be None."
+                                    else:
+                                        raise NotImplementedError(
+                                            "We believe this should never happen. If it happens, handle it here."
+                                        )
+                                case ProcessStatus.WAITING:
+                                    raise NotImplementedError(
+                                        f"Current process {process.ID} is waiting. Not implemented yet."
                                     )
 
-                                if process.dur > 0:
-                                    # Valid duration
-                                    dict_of_events[start_time] = {
-                                        "type": type(process).__name__,
-                                        "end": process.etc,
-                                        "area": current_area.ID,
-                                        "slot": current_slot,
-                                        "id": process.ID,
-                                    }
-                                else:
+                                case ProcessStatus.NOT_STARTED:
                                     raise NotImplementedError(
-                                        "We believe this should never happen. If it happens, handle it here."
+                                        f"Current process {process.ID} is not started. Not implemented yet."
                                     )
-                            case ProcessStatus.WAITING:
-                                raise NotImplementedError(
-                                    f"Current process {process.ID} is waiting. Not implemented yet."
-                                )
-
-                            case ProcessStatus.NOT_STARTED:
-                                raise NotImplementedError(
-                                    f"Current process {process.ID} is not started. Not implemented yet."
-                                )
-
-                            case _:
-                                raise ValueError(
-                                    f"Invalid process status {process.status} for process {process.ID}."
-                                )
 
-            reversed_time_keys = sorted(dict_of_events.keys(), reverse=True)
-            if len(reversed_time_keys) != 0:
-                # Generating valid event-list
-                is_copy = True
-                for start_time in reversed_time_keys:
-                    process_dict = dict_of_events[start_time]
-                    if process_dict["type"] == "trip":
-                        is_copy = process_dict["is_copy"]
-                    else:
-                        if is_copy is False:
-                            # Generate EventType
-                            match process_dict["type"]:
-                                case "Serve":
-                                    event_type = EventType.SERVICE
-                                case "Charge":
-                                    event_type = EventType.CHARGING_DEPOT
-                                case "Standby":
-                                    if process_dict["is_area_sink"] is True:
-                                        event_type = EventType.STANDBY_DEPARTURE
-                                    else:
-                                        event_type = EventType.STANDBY
-                                case "Precondition":
-                                    event_type = EventType.PRECONDITIONING
                                 case _:
                                     raise ValueError(
-                                        'Invalid process type %s. Valid process types are "Serve", "Charge", '
-                                        '"Standby", "Precondition"'
+                                        f"Invalid process status {process.status} for process {process.ID}."
                                     )
 
-                            # End time of 0-duration processes are start time of the next process
+            # Reverse the time keys to make generation of events before the trip easier
+            time_keys = sorted(dict_of_events.keys())
+            if len(time_keys) != 0:
+                # Generating valid event-list
+
+                for start_time in time_keys:
+                    process_dict = dict_of_events[start_time]
 
-                            if "end" not in process_dict:
-                                # End time will be the one time key "later"
-                                end_time = reversed_time_keys[
-                                    reversed_time_keys.index(start_time) - 1
-                                ]
-                                process_dict["end"] = end_time
-
-                            # Get soc
-                            soc_start = None
-                            soc_end = None
-
-                            for i in range(len(battery_log_list)):
-                                log = battery_log_list[i]
-
-                                if log[0] == start_time:
-                                    soc_start = log[1]
-                                if log[0] == process_dict["end"]:
-                                    soc_end = log[1]
-                                if log[0] < start_time < battery_log_list[i + 1][0]:
-                                    soc_start = log[1]
-                                if (
-                                    log[0]
-                                    < process_dict["end"]
-                                    < battery_log_list[i + 1][0]
-                                ):
-                                    soc_end = log[1]
-
-                            current_event = Event(
-                                scenario=scenario,
-                                vehicle_type_id=vehicle_type_id,
-                                vehicle=current_vehicle_db,
-                                station_id=None,
-                                area_id=int(process_dict["area"]),
-                                subloc_no=int(process_dict["slot"]),
-                                trip_id=None,
-                                time_start=timedelta(seconds=start_time)
-                                + simulation_start_time,
-                                time_end=timedelta(seconds=process_dict["end"])
-                                + simulation_start_time,
-                                soc_start=soc_start
-                                if soc_start is not None
-                                else soc_end,
-                                soc_end=soc_end
-                                if soc_end is not None
-                                else soc_start,  # if only one battery log is found,
-                                # then this is not an event with soc change
-                                event_type=event_type,
-                                description=None,
-                                timeseries=None,
+                    # Generate EventType
+                    match process_dict["type"]:
+                        case "Serve":
+                            event_type = EventType.SERVICE
+                        case "Charge":
+                            event_type = EventType.CHARGING_DEPOT
+                        case "Standby":
+                            if process_dict["is_area_sink"] is True:
+                                event_type = EventType.STANDBY_DEPARTURE
+                            else:
+                                event_type = EventType.STANDBY
+                        case "Precondition":
+                            event_type = EventType.PRECONDITIONING
+                        case "Trip":
+                            continue
+                        case _:
+                            raise ValueError(
+                                'Invalid process type %s. Valid process types are "Serve", "Charge", '
+                                '"Standby", "Precondition"'
                             )
-                            session.add(current_event)
+
+                    # End time of 0-duration processes are start time of the next process
+
+                    if "end" not in process_dict:
+                        # End time will be the one time key "later"
+                        end_time = time_keys[time_keys.index(start_time) + 1]
+
+                        process_dict["end"] = end_time
+
+                    # Get soc
+                    soc_start = None
+                    soc_end = None
+
+                    for i in range(len(battery_log_list)):
+                        # Access the correct battery log according to time since there is only one battery log for each time
+                        log = battery_log_list[i]
+
+                        if log[0] == start_time:
+                            soc_start = log[1]
+                        if log[0] == process_dict["end"]:
+                            soc_end = log[1]
+                        if log[0] < start_time < battery_log_list[i + 1][0]:
+                            soc_start = log[1]
+                        if log[0] < process_dict["end"] < battery_log_list[i + 1][0]:
+                            soc_end = log[1]
+
+                    current_event = Event(
+                        scenario=scenario,
+                        vehicle_type_id=vehicle_type_id,
+                        vehicle=current_vehicle_db,
+                        station_id=None,
+                        area_id=int(process_dict["area"]),
+                        subloc_no=int(process_dict["slot"]),
+                        trip_id=None,
+                        time_start=timedelta(seconds=start_time)
+                        + simulation_start_time,
+                        time_end=timedelta(seconds=process_dict["end"])
+                        + simulation_start_time,
+                        soc_start=soc_start if soc_start is not None else soc_end,
+                        soc_end=soc_end
+                        if soc_end is not None
+                        else soc_start,  # if only one battery log is found,
+                        # then this is not an event with soc change
+                        event_type=event_type,
+                        description=None,
+                        timeseries=None,
+                    )
+
+                    session.add(current_event)
 
                 # For non-copy schedules with no predecessor events, adding a dummy standby-departure
                 if (
-                    dict_of_events[reversed_time_keys[-1]]["type"] == "trip"
-                    and dict_of_events[reversed_time_keys[-1]]["is_copy"] is False
+                    dict_of_events[time_keys[0]]["type"] == "Trip"
+                    and dict_of_events[time_keys[0]]["is_copy"] is False
                 ):
-                    standby_start = reversed_time_keys[-1] - 1
-                    standby_end = reversed_time_keys[-1]
-                    rotation_id = str(dict_of_events[reversed_time_keys[-1]]["id"])
+                    standby_start = time_keys[0] - 1
+                    standby_end = time_keys[0]
+                    rotation_id = int(dict_of_events[time_keys[0]]["id"])
                     area = (
                         session.query(Area)
                         .filter(Area.vehicle_type_id == vehicle_type_id)
                         .first()
                     )
 
                     first_trip = (
```

### Comparing `eflips_depot-3.0.4/eflips/depot/api/defaults/default_settings.json` & `eflips_depot-3.0.5/eflips/depot/api/defaults/default_settings.json`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.4/eflips/depot/api/private/depot.py` & `eflips_depot-3.0.5/eflips/depot/api/private/depot.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.4/eflips/depot/api/private/util.py` & `eflips_depot-3.0.5/eflips/depot/api/private/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -336,26 +336,26 @@
         :return: A :class:`eflips.depot.standalone.SimpleTrip` object.
         """
 
         vehicle_types = [self.vehicle_type]
         departure = int((self.departure - simulation_start_time).total_seconds())
         arrival = int((self.arrival - simulation_start_time).total_seconds())
         simple_trip = SimpleTrip(
-            env,
-            self.id,
-            None,
-            self.start_depot_id,
-            self.end_depot_id,
-            vehicle_types,
-            departure,
-            arrival,
-            None,
-            self.departure_soc,
-            self.arrival_soc,
-            self.opportunity_charging,
+            env=env,
+            ID=self.id,
+            line_name=None,
+            origin=self.start_depot_id,
+            destination=self.end_depot_id,
+            vehicle_types=vehicle_types,
+            std=departure,
+            sta=arrival,
+            distance=None,
+            start_soc=self.departure_soc,
+            end_soc=self.arrival_soc,
+            charge_on_track=self.opportunity_charging,
             is_copy=self._is_copy,
         )
         return simple_trip
 
     def repeat(self, interval: timedelta) -> "VehicleSchedule":
         """
         Repeats a given VehicleSchedule.
```

### Comparing `eflips_depot-3.0.4/eflips/depot/configuration.py` & `eflips_depot-3.0.5/eflips/depot/configuration.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.4/eflips/depot/depot.py` & `eflips_depot-3.0.5/eflips/depot/depot.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.4/eflips/depot/evaluation.py` & `eflips_depot-3.0.5/eflips/depot/evaluation.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.4/eflips/depot/filters.py` & `eflips_depot-3.0.5/eflips/depot/filters.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.4/eflips/depot/input_epex_power_price.py` & `eflips_depot-3.0.5/eflips/depot/input_epex_power_price.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.4/eflips/depot/layout_opt/doc/direct_details.pdf` & `eflips_depot-3.0.5/eflips/depot/layout_opt/doc/direct_details.pdf`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.4/eflips/depot/layout_opt/evaluation.py` & `eflips_depot-3.0.5/eflips/depot/layout_opt/evaluation.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.4/eflips/depot/layout_opt/opt_tools/__init__.py` & `eflips_depot-3.0.5/eflips/depot/layout_opt/opt_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.4/eflips/depot/layout_opt/opt_tools/crossover.py` & `eflips_depot-3.0.5/eflips/depot/layout_opt/opt_tools/crossover.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.4/eflips/depot/layout_opt/opt_tools/fitness_c_urfd.py` & `eflips_depot-3.0.5/eflips/depot/layout_opt/opt_tools/fitness_c_urfd.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.4/eflips/depot/layout_opt/opt_tools/fitness_util.py` & `eflips_depot-3.0.5/eflips/depot/layout_opt/opt_tools/fitness_util.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.4/eflips/depot/layout_opt/opt_tools/init.py` & `eflips_depot-3.0.5/eflips/depot/layout_opt/opt_tools/init.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.4/eflips/depot/layout_opt/opt_tools/mutation.py` & `eflips_depot-3.0.5/eflips/depot/layout_opt/opt_tools/mutation.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.4/eflips/depot/layout_opt/optimize_c_urfd.py` & `eflips_depot-3.0.5/eflips/depot/layout_opt/optimize_c_urfd.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.4/eflips/depot/layout_opt/packing.py` & `eflips_depot-3.0.5/eflips/depot/layout_opt/packing.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.4/eflips/depot/layout_opt/settings.py` & `eflips_depot-3.0.5/eflips/depot/layout_opt/settings.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.4/eflips/depot/layout_opt/template_creation.py` & `eflips_depot-3.0.5/eflips/depot/layout_opt/template_creation.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.4/eflips/depot/layout_opt/util.py` & `eflips_depot-3.0.5/eflips/depot/layout_opt/util.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.4/eflips/depot/plots.py` & `eflips_depot-3.0.5/eflips/depot/plots.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.4/eflips/depot/processes.py` & `eflips_depot-3.0.5/eflips/depot/processes.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.4/eflips/depot/rating.py` & `eflips_depot-3.0.5/eflips/depot/rating.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.4/eflips/depot/resources.py` & `eflips_depot-3.0.5/eflips/depot/resources.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.4/eflips/depot/settings_config.py` & `eflips_depot-3.0.5/eflips/depot/settings_config.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.4/eflips/depot/simple_vehicle.py` & `eflips_depot-3.0.5/eflips/depot/simple_vehicle.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.4/eflips/depot/simulation.py` & `eflips_depot-3.0.5/eflips/depot/simulation.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.4/eflips/depot/smart_charging.py` & `eflips_depot-3.0.5/eflips/depot/smart_charging.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.4/eflips/depot/standalone.py` & `eflips_depot-3.0.5/eflips/depot/standalone.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.4/eflips/depot/validation.py` & `eflips_depot-3.0.5/eflips/depot/validation.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.0.4/pyproject.toml` & `eflips_depot-3.0.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eflips-depot"
-version = "3.0.4"
+version = "3.0.5"
 description = "Depot Simulation for eFLIPS"
 authors = ["Enrico Lauth <enrico.lauth@tu-berlin.de>",
     "Ludger Heide <ludger.heide@tu-berlin.de",
     "Shuyao Guo <shuyao.guo@tu-berlin.de"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/mpm-tu-berlin/eflips-depot"
```

### Comparing `eflips_depot-3.0.4/PKG-INFO` & `eflips_depot-3.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eflips-depot
-Version: 3.0.4
+Version: 3.0.5
 Summary: Depot Simulation for eFLIPS
 Home-page: https://github.com/mpm-tu-berlin/eflips-depot
 License: AGPL-3.0-or-later
 Author: Enrico Lauth
 Author-email: enrico.lauth@tu-berlin.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
@@ -17,15 +17,15 @@
 Requires-Dist: pandas (>=2.1.4,<3.0.0)
 Requires-Dist: simpy (>=4.0.1,<5.0.0)
 Requires-Dist: xlrd (<=1.2.0)
 Requires-Dist: xlsxwriter (>=3.1.9,<4.0.0)
 Project-URL: Repository, https://github.com/mpm-tu-berlin/eflips-depot
 Description-Content-Type: text/markdown
 
-[![Tests](https://github.com/mpm-tu-berlin/eflips-depot/actions/workflows/postgres_eflips_depot.yml/badge.svg)](https://github.com/mpm-tu-berlin/eflips-depot/actions/workflows/postgres_eflips_depot.yml)
+[![Tests](https://github.com/mpm-tu-berlin/eflips-depot/actions/workflows/unittests.yml/badge.svg)](https://github.com/mpm-tu-berlin/eflips-depot/actions/workflows/unittests.yml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 
 # eflips-depot
 
 ---
```

