# Comparing `tmp/vizable-0.8.0.tar.gz` & `tmp/vizable-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vizable-0.8.0.tar", max compression
+gzip compressed data, was "vizable-0.9.0.tar", max compression
```

## Comparing `vizable-0.8.0.tar` & `vizable-0.9.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1072 2024-04-04 05:20:24.424450 vizable-0.8.0/LICENSE
--rw-r--r--   0        0        0     3548 2024-04-04 05:20:24.424450 vizable-0.8.0/README.md
--rw-r--r--   0        0        0       72 2024-04-04 05:20:24.424450 vizable-0.8.0/VizAble/__init__.py
--rw-r--r--   0        0        0    28072 2024-04-04 05:20:24.424450 vizable-0.8.0/VizAble/app.py
--rw-r--r--   0        0        0     2026 2024-04-04 05:20:24.424450 vizable-0.8.0/VizAble/check_datatypes.py
--rw-r--r--   0        0        0     7907 2024-04-04 05:20:24.424450 vizable-0.8.0/VizAble/functions.py
--rw-r--r--   0        0        0     6092 2024-04-04 05:20:24.424450 vizable-0.8.0/VizAble/generate_plots.py
--rw-r--r--   0        0        0      615 2024-04-04 05:20:24.424450 vizable-0.8.0/VizAble/introductions.py
--rw-r--r--   0        0        0      433 2024-04-04 05:20:24.424450 vizable-0.8.0/VizAble/rsconnect-python/VizAble.json
--rw-r--r--   0        0        0     2493 2024-04-04 05:20:24.424450 vizable-0.8.0/VizAble/select_columns.py
--rw-r--r--   0        0        0     1011 2024-04-04 05:20:24.424450 vizable-0.8.0/VizAble/select_plottypes.py
--rw-r--r--   0        0        0     2804 2024-04-04 05:20:24.424450 vizable-0.8.0/VizAble/upload_file.py
--rw-r--r--   0        0        0     1819 2024-04-04 05:20:24.432450 vizable-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     5300 1970-01-01 00:00:00.000000 vizable-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-10 05:17:51.170549 vizable-0.9.0/LICENSE
+-rw-r--r--   0        0        0     3548 2024-04-10 05:17:51.170549 vizable-0.9.0/README.md
+-rw-r--r--   0        0        0       72 2024-04-10 05:17:51.170549 vizable-0.9.0/VizAble/__init__.py
+-rw-r--r--   0        0        0    31892 2024-04-10 05:17:51.170549 vizable-0.9.0/VizAble/app.py
+-rw-r--r--   0        0        0     2026 2024-04-10 05:17:51.170549 vizable-0.9.0/VizAble/check_datatypes.py
+-rw-r--r--   0        0        0     9245 2024-04-10 05:17:51.170549 vizable-0.9.0/VizAble/functions.py
+-rw-r--r--   0        0        0     6780 2024-04-10 05:17:51.170549 vizable-0.9.0/VizAble/generate_plots.py
+-rw-r--r--   0        0        0      615 2024-04-10 05:17:51.170549 vizable-0.9.0/VizAble/introductions.py
+-rw-r--r--   0        0        0      433 2024-04-10 05:17:51.170549 vizable-0.9.0/VizAble/rsconnect-python/VizAble.json
+-rw-r--r--   0        0        0     2851 2024-04-10 05:17:51.170549 vizable-0.9.0/VizAble/select_columns.py
+-rw-r--r--   0        0        0     1011 2024-04-10 05:17:51.170549 vizable-0.9.0/VizAble/select_plottypes.py
+-rw-r--r--   0        0        0     2804 2024-04-10 05:17:51.170549 vizable-0.9.0/VizAble/upload_file.py
+-rw-r--r--   0        0        0     1819 2024-04-10 05:17:51.178549 vizable-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     5300 1970-01-01 00:00:00.000000 vizable-0.9.0/PKG-INFO
```

### Comparing `vizable-0.8.0/LICENSE` & `vizable-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vizable-0.8.0/README.md` & `vizable-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `vizable-0.8.0/VizAble/app.py` & `vizable-0.9.0/VizAble/app.py`

 * *Files 14% similar despite different names*

```diff
@@ -342,15 +342,23 @@
     @reactive.Effect
     @reactive.event(input.file_format, reactive_df, input.sheet_name)
     def update_plot_types_select() -> None:
         """ Update the dropdown for users to select the plot types based on the uploaded data frame.
         """
         data_frame = reactive_df.get()
         if data_frame is not None and not data_frame.empty:
-            choices: list[str] = ["Select an option", "Line Plot", "Bar Plot", "Box Plot", "Histogram", "Scatter Plot"]
+            choices: list[str] = [
+                "Select an option",
+                "Line Plot",
+                "Bar Plot",
+                "Box Plot",
+                "Grouped_Box Plot",
+                "Histogram",
+                "Scatter Plot"
+            ]
         else:
             choices: list[str] = ["Select an option"]
 
         ui.update_select(
             id="plot_types",
             choices=choices,
             selected=None,
@@ -418,15 +426,40 @@
                     """
                 ## **Instructions:**
                 If you would like to create a box plot, please select:
                  - one numerical column (containing the  data for which you want to see the distribution)
                 """
                 ),
             )
+        elif input.plot_types() == "Grouped_Box Plot":
+            return (
+                ui.markdown(
+                    """
+                ## **Grouped Box Plot:**
+                A grouped box plot is a graphical representation that enables the comparison of distributions between multiple groups or categories within a dataset. It provides insights into the variability, central tendency, and spread of a variable across different groupings.
 
+                Here are the components of a box plot:
+                1. `Boxes`: Each box represents the interquartile range (IQR), which is the middle 50% of the data. The top and bottom edges of the box correspond to the first quartile (Q1) and third quartile (Q3), respectively. The length of the box thus indicates the spread of the central 50% of the data.
+                2. `Line` (whisker): Lines (whiskers) extend from the top and bottom of the box to indicate the range of the data. These lines can extend to a certain distance (often 1.5 times the IQR) beyond the quartiles or may represent the minimum and maximum values within that range.
+                3. `Median` (line inside the box): A line inside the box represents the median (Q2) of the dataset, which is the middle value when the data is ordered.
+                4. `Grouping`: The boxes are grouped together, allowing for a visual comparison of the distribution of the variable across different groups. This facilitates the identification of differences or similarities in the data distribution between the groups.
+                5. `Outliers`: Individual data points beyond the whiskers may be considered outliers and are often plotted individually.
+                """
+                ),
+                ui.tags.hr(),
+                ui.markdown(
+                    """
+                ## **Instructions:**
+                If you would like to create a box plot, please select:
+                 - one numerical column (containing the  data for which you want to see the distribution)
+                 - one categorical column for `grouping` (to compare the distribution across different groups)
+                """
+                ), 
+            )
+        
         elif input.plot_types() == "Histogram":
             return (
                 ui.markdown(
                     """
                 ## **Histogram:**
                 A histogram is a graphical representation of the distribution of a continuous dataset. It is used to visualize the underlying frequency distribution of a set of continuous or interval data. Histograms provide insights into the shape, center, and spread of the data.
                 """
@@ -480,16 +513,21 @@
             functions.update_yaxis_input_select(input.plot_types(), choices)
         
         # update only x-axis dropdowns
         elif input.plot_types() in ["Bar Plot", "Histogram"]:
             functions.update_xaxis_input_select(input.plot_types(), choices)
         
         # update only y-axis dropdowns
-        elif input.plot_types() == "Box Plot":
+        elif input.plot_types() in ["Box Plot"]:
+            functions.update_yaxis_input_select(input.plot_types(), choices)
+        
+        # update y-axis and grouping dropdowns
+        elif input.plot_types() in ["Grouped_Box Plot"]:
             functions.update_yaxis_input_select(input.plot_types(), choices)
+            functions.update_grouping_input_select(input.plot_types(), functions.return_choices_for_columns(data_frame, "Categorical"))
             
     @render.data_frame
     def get_output_selected_cols() -> pd.DataFrame:
         """ Display the selected columns after users' column selections.
 
         :return: A data frame containing the selected columns.
         :rtype: pd.DataFrame
@@ -514,14 +552,21 @@
                 selected_cols = data_frame[[x_col]]
 
         elif input.plot_types() == "Box Plot":
             req(input.box_y_axis())
             y_col: str = input.box_y_axis()
             if y_col in data_frame.columns:
                 selected_cols = data_frame[[y_col]]
+        
+        elif input.plot_types() == "Grouped_Box Plot":
+            req(input.grouped_box_y_axis(), input.grouped_box_grouping())
+            y_col: str = input.grouped_box_y_axis()
+            grouping_col: str = input.grouped_box_grouping()
+            if y_col in data_frame.columns and grouping_col in data_frame.columns:
+                selected_cols = data_frame[[y_col, grouping_col]]
 
         elif input.plot_types() == "Histogram":
             req(input.histogram_x_axis())
             x_col: str = input.histogram_x_axis()
             if x_col in data_frame.columns:
                 selected_cols = data_frame[[x_col]]
 
@@ -619,14 +664,35 @@
                 title={"text": plot_title, "x": 0.5},
             ).update_yaxes(
                 title_text = y_axis_title,
             )
 
             return box_plot
         
+        # Grouped_Box Plot:
+        if input.plot_types() == "Grouped_Box Plot":
+            req(input.grouped_box_y_axis(), input.grouped_box_grouping())
+            plot_title = input.grouped_box_plot_title()
+            y_axis_title = input.grouped_box_y_axis_title()
+            grouping = input.grouped_box_grouping()
+
+            box_plot_grouped = px.box(
+                data_frame = data_frame,
+                x = grouping,
+                y = input.grouped_box_y_axis(),
+                color = grouping,
+            ).update_layout(
+                template="seaborn",
+                title={"text": plot_title, "x": 0.5},
+            ).update_yaxes(
+                title_text = y_axis_title,
+            )
+
+            return box_plot_grouped
+
         # Histogram:
         if input.plot_types() == "Histogram":
             req(input.histogram_x_axis())
             plot_title = input.histogram_plot_title()
 
             # x_axis title
             x_axis_title = input.histogram_x_axis_title()
```

### Comparing `vizable-0.8.0/VizAble/check_datatypes.py` & `vizable-0.9.0/VizAble/check_datatypes.py`

 * *Files identical despite different names*

### Comparing `vizable-0.8.0/VizAble/functions.py` & `vizable-0.9.0/VizAble/functions.py`

 * *Files 18% similar despite different names*

```diff
@@ -125,14 +125,31 @@
         id = y_axis_id,
         label = ui.strong("Y-axis"),
         choices = [],
         selected = None,
         multiple = False
     )
 
+def grouping_input_select(plot_type_str: str) -> ui.input_select:
+    """ Create a dropdown for users to select the column for grouping.
+
+    :param plot_type_str: Plot type string, e.g., "grouped_box".
+    :type plot_type_str: str
+    :return: An empty dropdown for users to select `grouping`, where the input id is based on the provided `plot_type_str`.
+    :rtype: ui.input_select
+    """
+    grouping_id = f"{plot_type_str}_grouping"
+    return ui.input_select(
+        id = grouping_id,
+        label = ui.strong("Group By"),
+        choices = [],
+        selected = None,
+        multiple = False
+    )
+
 def get_excel_sheet_names(file_path: Path) -> List[str]:
     """ Get a list of all sheet names for the uploaded Excel file.
 
     :param file_path: Path to the uploaded Excel file.
     :type file_path: Path
     :return: A list of all sheet names for the uploaded Excel file. 
             Returns an empty list if the file path is invalid or there is an error reading the file.
@@ -156,17 +173,19 @@
     :return: A list of column names for the dropdown based on the plot type.
     :rtype: List[str]
     """
     choices = ["Select an option"]
     
     # Mapping of plot types to data types they accept(add more if needed)
     plot_type_to_dtypes = {
+        "Categorical": ["object", "category"],
         "Line Plot": None,
         "Bar Plot": ["object", "category"],
         "Box Plot": ["number"],
+        "Grouped_Box Plot": ["number"],
         "Histogram": ["number"],
         "Scatter Plot": ["number"],
     }
 
     # Get the relevant data types for the selected plot type
     dtypes = plot_type_to_dtypes.get(plot_type)
 
@@ -207,8 +226,26 @@
     """
     axis_id = plot_type.split(" ")[0].lower() + "_y_axis"
 
     return ui.update_select(
         id=axis_id,
         choices=choices,
         selected=None
+    )
+
+def update_grouping_input_select(plot_type: str, choices: List[str]) -> ui.update_select:
+    """ Update the grouping dropdown based on the selected plot type.
+
+    :param plot_type: The plot type selected by the user.
+    :type plot_type: str
+    :param choices: A list of column names for the dropdown based on the plot type.
+    :type choices: List[str]
+    :return: An updated grouping dropdown based on the selected plot type.
+    :rtype: ui.update_select
+    """
+    grouping_id = plot_type.split(" ")[0].lower() + "_grouping"
+
+    return ui.update_select(
+        id=grouping_id,
+        choices=choices,
+        selected=None
     )
```

### Comparing `vizable-0.8.0/VizAble/generate_plots.py` & `vizable-0.9.0/VizAble/generate_plots.py`

 * *Files 9% similar despite different names*

```diff
@@ -55,14 +55,29 @@
                         ui.input_text(
                             id="box_y_axis_title",
                             label="Y-axis Title",
                             placeholder="Enter a title for the y-axis"
                         ),
                     ),
 
+                    # Show when user selects "Grouped_Box Plot" on plot_types
+                    ui.panel_conditional(
+                        "input.plot_types == 'Grouped_Box Plot'",
+                        ui.input_text(
+                            id="grouped_box_plot_title",
+                            label="Plot Title",
+                            placeholder="Enter a plot title"
+                        ),
+                        ui.input_text(
+                            id="grouped_box_y_axis_title",
+                            label="Y-axis Title",
+                            placeholder="Enter a title for the y-axis"
+                        ),
+                    ),
+
                     # Show when user selects "Bar Plot" on plot_types
                     ui.panel_conditional(
                         "input.plot_types == 'Bar Plot'",
                         ui.input_text(
                             id="bar_plot_title",
                             label="Plot Title",
                             placeholder="Enter a plot title"
```

### Comparing `vizable-0.8.0/VizAble/introductions.py` & `vizable-0.9.0/VizAble/introductions.py`

 * *Files identical despite different names*

### Comparing `vizable-0.8.0/VizAble/select_columns.py` & `vizable-0.9.0/VizAble/select_columns.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,20 @@
                     ),
                     # Add condition: if user selects "Box Plot" on plot_types
                     ui.panel_conditional(
                         "input.plot_types == 'Box Plot'",
                         # add dropdown for x-axis
                         functions.yaxis_input_select("box"),
                     ),
+                    # Add condition: if user selects "Grouped_Box Plot" on plot_types
+                    ui.panel_conditional(
+                        "input.plot_types == 'Grouped_Box Plot'",
+                        functions.yaxis_input_select("grouped_box"),
+                        functions.grouping_input_select("grouped_box"),
+                    ),
                     # Add condition: if user selects "Histogram" on plot_types
                     ui.panel_conditional(
                         "input.plot_types == 'Histogram'",
                         # add dropdown for x-axis
                         functions.xaxis_input_select("histogram"),
                     ),
                     # Add condition: if user selects "Scatter Plot" on plot_types
```

### Comparing `vizable-0.8.0/VizAble/select_plottypes.py` & `vizable-0.9.0/VizAble/select_plottypes.py`

 * *Files identical despite different names*

### Comparing `vizable-0.8.0/VizAble/upload_file.py` & `vizable-0.9.0/VizAble/upload_file.py`

 * *Files identical despite different names*

### Comparing `vizable-0.8.0/pyproject.toml` & `vizable-0.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "VizAble"
-version = "0.8.0"
+version = "0.9.0"
 description = "A web-based data visualization tool that generates accessible visualizations for all users, including people with visual impairments (low vision or blind)."
 license = "MIT"
 authors = ["Chi-Ying Chuang <rebekah890110@gmail.com>"]
 readme = "README.md"
 packages = [{include = "VizAble"}]
 
 [tool.poetry.dependencies]
```

### Comparing `vizable-0.8.0/PKG-INFO` & `vizable-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VizAble
-Version: 0.8.0
+Version: 0.9.0
 Summary: A web-based data visualization tool that generates accessible visualizations for all users, including people with visual impairments (low vision or blind).
 License: MIT
 Author: Chi-Ying Chuang
 Author-email: rebekah890110@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

