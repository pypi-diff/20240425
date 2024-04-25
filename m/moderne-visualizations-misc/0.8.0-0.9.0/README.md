# Comparing `tmp/moderne_visualizations_misc-0.8.0.tar.gz` & `tmp/moderne_visualizations_misc-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moderne_visualizations_misc-0.8.0.tar", last modified: Wed Aug 23 19:04:20 2023, max compression
+gzip compressed data, was "moderne_visualizations_misc-0.9.0.tar", last modified: Thu Aug 24 00:26:41 2023, max compression
```

## Comparing `moderne_visualizations_misc-0.8.0.tar` & `moderne_visualizations_misc-0.9.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 19:04:20.016949 moderne_visualizations_misc-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-23 19:03:30.000000 moderne_visualizations_misc-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-08-23 19:04:20.012949 moderne_visualizations_misc-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-08-23 19:03:30.000000 moderne_visualizations_misc-0.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 19:04:20.004949 moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-23 19:03:30.000000 moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-08-23 19:03:30.000000 moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/cobol_find_copybook.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-08-23 19:03:30.000000 moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/cobol_relationships.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-08-23 19:03:30.000000 moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/cobol_relationships_data_grid.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-08-23 19:03:30.000000 moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/dependency_vulnerabilities.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 19:04:20.008949 moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/dev/
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-08-23 19:03:30.000000 moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/dev/parse_failure_analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-08-23 19:03:30.000000 moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/find_methods.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-08-23 19:03:30.000000 moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/find_source_files.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-08-23 19:03:30.000000 moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/gradle_wrappers.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 19:04:20.012949 moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/images/
--rw-r--r--   0 runner    (1001) docker     (123)    14039 2023-08-23 19:03:30.000000 moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/images/cobol_find_copy_book.300.png
--rw-r--r--   0 runner    (1001) docker     (123)    26977 2023-08-23 19:03:30.000000 moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/images/cobol_relationships.300.png
--rw-r--r--   0 runner    (1001) docker     (123)    37937 2023-08-23 19:03:30.000000 moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/images/cobol_relationships_data_grid.300.png
--rw-r--r--   0 runner    (1001) docker     (123)    14680 2023-08-23 19:03:30.000000 moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/images/dependency_vulnerabilities.300.png
--rw-r--r--   0 runner    (1001) docker     (123)    16602 2023-08-23 19:03:30.000000 moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/images/gradle_wrappers.300.png
--rw-r--r--   0 runner    (1001) docker     (123)    31410 2023-08-23 19:03:30.000000 moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/images/language_composition.300.png
--rw-r--r--   0 runner    (1001) docker     (123)    17328 2023-08-23 19:03:30.000000 moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/images/language_composition_by_folder.300.png
--rw-r--r--   0 runner    (1001) docker     (123)    23912 2023-08-23 19:03:30.000000 moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/images/parse_failure_analysis.300.png
--rw-r--r--   0 runner    (1001) docker     (123)    24871 2023-08-23 19:03:30.000000 moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/images/sql_crud.300.png
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-08-23 19:03:30.000000 moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/language_composition.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-08-23 19:03:30.000000 moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/language_composition_by_folder.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-08-23 19:03:30.000000 moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/lst_provenance.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11912 2023-08-23 19:03:30.000000 moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/parse_failure_analysis.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 19:04:20.012949 moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/specs/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-23 19:03:30.000000 moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/specs/cobol_find_copybook.yml
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-23 19:03:30.000000 moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/specs/cobol_relationships.yml
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-08-23 19:03:30.000000 moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/specs/cobol_relationships_data_grid.yml
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-08-23 19:03:30.000000 moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/specs/dependency_vulnerabilities.yml
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-08-23 19:03:30.000000 moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/specs/find_methods.yml
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-08-23 19:03:30.000000 moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/specs/find_source_files.yml
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-08-23 19:03:30.000000 moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/specs/gradle_wrappers.yml
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-08-23 19:03:30.000000 moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/specs/language_composition.yml
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-08-23 19:03:30.000000 moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/specs/language_composition_by_folder.yml
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-08-23 19:03:30.000000 moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/specs/lst_provenance.yml
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-08-23 19:03:30.000000 moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/specs/sql_crud.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-08-23 19:03:30.000000 moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/sql_crud.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 19:04:20.008949 moderne_visualizations_misc-0.8.0/moderne_visualizations_misc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-08-23 19:04:19.000000 moderne_visualizations_misc-0.8.0/moderne_visualizations_misc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-08-23 19:04:19.000000 moderne_visualizations_misc-0.8.0/moderne_visualizations_misc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-23 19:04:19.000000 moderne_visualizations_misc-0.8.0/moderne_visualizations_misc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-08-23 19:04:19.000000 moderne_visualizations_misc-0.8.0/moderne_visualizations_misc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-23 19:04:19.000000 moderne_visualizations_misc-0.8.0/moderne_visualizations_misc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-08-23 19:04:11.000000 moderne_visualizations_misc-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-23 19:04:20.016949 moderne_visualizations_misc-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 00:26:41.469718 moderne_visualizations_misc-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (999)      133 2023-08-24 00:25:51.000000 moderne_visualizations_misc-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (999)      352 2023-08-24 00:26:41.469718 moderne_visualizations_misc-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)      273 2023-08-24 00:25:51.000000 moderne_visualizations_misc-0.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 00:26:41.465717 moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-24 00:25:51.000000 moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1999 2023-08-24 00:25:51.000000 moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/cobol_find_copybook.ipynb
+-rw-r--r--   0 runner    (1001) docker     (999)     8300 2023-08-24 00:25:51.000000 moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/cobol_relationships.ipynb
+-rw-r--r--   0 runner    (1001) docker     (999)     2131 2023-08-24 00:25:51.000000 moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/cobol_relationships_data_grid.ipynb
+-rw-r--r--   0 runner    (1001) docker     (999)     8263 2023-08-24 00:25:51.000000 moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/dependency_vulnerabilities.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 00:26:41.465717 moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/dev/
+-rw-r--r--   0 runner    (1001) docker     (999)      675 2023-08-24 00:25:51.000000 moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/dev/parse_failure_analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (999)     1882 2023-08-24 00:25:51.000000 moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/find_methods.ipynb
+-rw-r--r--   0 runner    (1001) docker     (999)     1252 2023-08-24 00:25:51.000000 moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/find_source_files.ipynb
+-rw-r--r--   0 runner    (1001) docker     (999)     1903 2023-08-24 00:25:51.000000 moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/gradle_wrappers.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 00:26:41.469718 moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/images/
+-rw-r--r--   0 runner    (1001) docker     (999)    14039 2023-08-24 00:25:51.000000 moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/images/cobol_find_copy_book.300.png
+-rw-r--r--   0 runner    (1001) docker     (999)    26977 2023-08-24 00:25:51.000000 moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/images/cobol_relationships.300.png
+-rw-r--r--   0 runner    (1001) docker     (999)    37937 2023-08-24 00:25:51.000000 moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/images/cobol_relationships_data_grid.300.png
+-rw-r--r--   0 runner    (1001) docker     (999)    14680 2023-08-24 00:25:51.000000 moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/images/dependency_vulnerabilities.300.png
+-rw-r--r--   0 runner    (1001) docker     (999)    16602 2023-08-24 00:25:51.000000 moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/images/gradle_wrappers.300.png
+-rw-r--r--   0 runner    (1001) docker     (999)    31410 2023-08-24 00:25:51.000000 moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/images/language_composition.300.png
+-rw-r--r--   0 runner    (1001) docker     (999)    17328 2023-08-24 00:25:51.000000 moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/images/language_composition_by_folder.300.png
+-rw-r--r--   0 runner    (1001) docker     (999)    23912 2023-08-24 00:25:51.000000 moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/images/parse_failure_analysis.300.png
+-rw-r--r--   0 runner    (1001) docker     (999)    24871 2023-08-24 00:25:51.000000 moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/images/sql_crud.300.png
+-rw-r--r--   0 runner    (1001) docker     (999)     4888 2023-08-24 00:25:51.000000 moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/language_composition.ipynb
+-rw-r--r--   0 runner    (1001) docker     (999)     2566 2023-08-24 00:25:51.000000 moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/language_composition_by_folder.ipynb
+-rw-r--r--   0 runner    (1001) docker     (999)     2148 2023-08-24 00:25:51.000000 moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/lst_provenance.ipynb
+-rw-r--r--   0 runner    (1001) docker     (999)    11912 2023-08-24 00:25:51.000000 moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/parse_failure_analysis.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 00:26:41.469718 moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/specs/
+-rw-r--r--   0 runner    (1001) docker     (999)      405 2023-08-24 00:25:51.000000 moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/specs/cobol_find_copybook.yml
+-rw-r--r--   0 runner    (1001) docker     (999)     1012 2023-08-24 00:25:51.000000 moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/specs/cobol_relationships.yml
+-rw-r--r--   0 runner    (1001) docker     (999)      600 2023-08-24 00:25:51.000000 moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/specs/cobol_relationships_data_grid.yml
+-rw-r--r--   0 runner    (1001) docker     (999)      738 2023-08-24 00:25:51.000000 moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/specs/dependency_vulnerabilities.yml
+-rw-r--r--   0 runner    (1001) docker     (999)      330 2023-08-24 00:25:51.000000 moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/specs/find_methods.yml
+-rw-r--r--   0 runner    (1001) docker     (999)      335 2023-08-24 00:25:51.000000 moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/specs/find_source_files.yml
+-rw-r--r--   0 runner    (1001) docker     (999)      328 2023-08-24 00:25:51.000000 moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/specs/gradle_wrappers.yml
+-rw-r--r--   0 runner    (1001) docker     (999)      309 2023-08-24 00:25:51.000000 moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/specs/language_composition.yml
+-rw-r--r--   0 runner    (1001) docker     (999)      383 2023-08-24 00:25:51.000000 moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/specs/language_composition_by_folder.yml
+-rw-r--r--   0 runner    (1001) docker     (999)      295 2023-08-24 00:25:51.000000 moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/specs/lst_provenance.yml
+-rw-r--r--   0 runner    (1001) docker     (999)      568 2023-08-24 00:25:51.000000 moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/specs/sql_crud.yml
+-rw-r--r--   0 runner    (1001) docker     (999)     2403 2023-08-24 00:25:51.000000 moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/sql_crud.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 00:26:41.465717 moderne_visualizations_misc-0.9.0/moderne_visualizations_misc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (999)      352 2023-08-24 00:26:41.000000 moderne_visualizations_misc-0.9.0/moderne_visualizations_misc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)     2264 2023-08-24 00:26:41.000000 moderne_visualizations_misc-0.9.0/moderne_visualizations_misc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-24 00:26:41.000000 moderne_visualizations_misc-0.9.0/moderne_visualizations_misc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (999)      206 2023-08-24 00:26:41.000000 moderne_visualizations_misc-0.9.0/moderne_visualizations_misc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       28 2023-08-24 00:26:41.000000 moderne_visualizations_misc-0.9.0/moderne_visualizations_misc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (999)     1228 2023-08-24 00:26:32.000000 moderne_visualizations_misc-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-24 00:26:41.469718 moderne_visualizations_misc-0.9.0/setup.cfg
```

### Comparing `moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/cobol_find_copybook.ipynb` & `moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/cobol_find_copybook.ipynb`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/cobol_relationships.ipynb` & `moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/cobol_relationships.ipynb`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9960477941176471%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(1, \'filter_resources_related_to: str = ""\\n\'), (2, '*

 * *            '\'exclude_incoming_relationships: str = "false"\')], delete: [1]}}, 2: {\'source\': '*

 * *            "{insert: [(7, '\\n'), (8, '\\n'), (9, 'dot.graph_attr = {\\n'), (10, '    "*

 * *            '"overlap": "prism",\\n\'), (11, \'    "smoothing": "graph_dist",\\n\'), (12, \'    '*

 * *            '"normalize": "true",\\n\'), (13, \'    "overlap_scaling": str(max(10, df.size / '*

 * *            "150)),\\n'), (14, '}\ […]*

```diff
@@ -9,15 +9,16 @@
                 "tags": [
                     "parameters"
                 ]
             },
             "outputs": [],
             "source": [
                 "node_shape: str = \"ellipse\"\n",
-                "filter_resources_related_to: str = \"\""
+                "filter_resources_related_to: str = \"\"\n",
+                "exclude_incoming_relationships: str = \"false\""
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "1934da7b",
             "metadata": {
@@ -42,28 +43,76 @@
                     "end_time": "2023-08-04T16:02:27.603653Z",
                     "start_time": "2023-08-04T16:02:26.607939Z"
                 }
             },
             "outputs": [],
             "source": [
                 "graphviz.set_jupyter_format(\"svg\")\n",
-                "\n",
                 "dot = graphviz.Digraph(\n",
                 "    \"cobol-relationships\", comment=\"COBOL relationships\", engine=\"sfdp\"\n",
                 ")\n",
                 "\n",
-                "dot.graph_attr = {\"overlap\": \"prism\", \"smoothing\": \"graph_dist\", \"normalize\": \"true\"}\n",
-                "\n",
                 "# clean dependent field remove all content up to first slash\n",
                 "df[\"dependent\"] = df[\"dependent\"].apply(lambda x: re.sub(r\"^.*\\/\", \"\", x))\n",
                 "\n",
+                "\n",
+                "dot.graph_attr = {\n",
+                "    \"overlap\": \"prism\",\n",
+                "    \"smoothing\": \"graph_dist\",\n",
+                "    \"normalize\": \"true\",\n",
+                "    \"overlap_scaling\": str(max(10, df.size / 150)),\n",
+                "}\n",
+                "\n",
+                "\n",
+                "def apply_filter(node, node_map, seen):\n",
+                "    if node in seen or node not in node_map:\n",
+                "        return\n",
+                "\n",
+                "    seen.add(node)\n",
+                "    to = node_map[node]\n",
+                "    for type in to:\n",
+                "        for next in node_map[node][type]:\n",
+                "            apply_filter(next, node_map, seen)\n",
+                "\n",
+                "\n",
                 "if filter_resources_related_to:\n",
+                "    node_map = {}\n",
+                "    for i, z in enumerate(\n",
+                "        zip(\n",
+                "            df[\"dependent\"], df[\"dependentType\"], df[\"dependency\"], df[\"dependencyType\"]\n",
+                "        )\n",
+                "    ):\n",
+                "        dependent = str(z[0])\n",
+                "        dependentType = str(z[1])\n",
+                "        dependency = str(z[2])\n",
+                "        dependencyType = str(z[3])\n",
+                "\n",
+                "        if not bool(node_map):\n",
+                "            node_map = {}\n",
+                "\n",
+                "        if dependent not in node_map:\n",
+                "            node_map[dependent] = {}\n",
+                "\n",
+                "        if dependentType not in node_map[dependent]:\n",
+                "            node_map[dependent][dependentType] = {}\n",
+                "\n",
+                "        if dependency not in node_map[dependent][dependentType]:\n",
+                "            node_map[dependent][dependentType][dependency] = {}\n",
+                "\n",
+                "        if dependencyType not in node_map[dependent][dependentType][dependency]:\n",
+                "            node_map[dependent][dependentType][dependency][dependencyType] = {i}\n",
+                "\n",
+                "    seen = set()\n",
+                "    apply_filter(filter_resources_related_to, node_map, seen)\n",
+                "\n",
                 "    df = df[\n",
-                "        (df[\"dependent\"].str.contains(filter_resources_related_to))\n",
-                "        | (df[\"dependency\"].str.contains(filter_resources_related_to))\n",
+                "        (df[\"dependent\"].isin(seen))\n",
+                "        if exclude_incoming_relationships == \"true\"\n",
+                "        else (df[\"dependent\"].isin(seen))\n",
+                "             | (df[\"dependency\"].str.contains(filter_resources_related_to))\n",
                 "    ]\n",
                 "    dot.graph_attr[\"beautify\"] = \"true\"\n",
                 "\n",
                 "\n",
                 "def style_node(is_missing, dependency_type):\n",
                 "    if is_missing == \"true\":\n",
                 "        return palette.__moderneColorMap[\"red\"][200]\n",
@@ -88,22 +137,26 @@
                 "    return f\"<<b>{value}</b><br/><i>({docType})</i>>\"\n",
                 "\n",
                 "\n",
                 "def map_relationship(row):\n",
                 "    if is_node(row):\n",
                 "        dot.node(\n",
                 "            make_node(row[\"dependent\"], row[\"dependentType\"]),\n",
-                "            shape=node_shape,\n",
+                "            shape=\"Mdiamond\"\n",
+                "            if filter_resources_related_to == row[\"dependent\"]\n",
+                "            else node_shape,\n",
                 "            label=add_annotation(row[\"dependent\"], row[\"dependentType\"]),\n",
                 "            style=\"filled\",\n",
                 "            fillcolor=style_node(row[\"dependencyMissing\"], row[\"dependentType\"]),\n",
                 "        )\n",
                 "        dot.node(\n",
                 "            make_node(row[\"dependency\"], row[\"dependencyType\"]),\n",
-                "            shape=node_shape,\n",
+                "            shape=\"Mdiamond\"\n",
+                "            if filter_resources_related_to == row[\"dependency\"]\n",
+                "            else node_shape,\n",
                 "            label=add_annotation(row[\"dependency\"], row[\"dependencyType\"]),\n",
                 "            style=\"filled\",\n",
                 "            fillcolor=style_node(row[\"dependencyMissing\"], row[\"dependencyType\"]),\n",
                 "        )\n",
                 "        dot.edge(\n",
                 "            make_node(row[\"dependent\"], row[\"dependentType\"]),\n",
                 "            make_node(row[\"dependency\"], row[\"dependencyType\"]),\n",
```

### Comparing `moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/cobol_relationships_data_grid.ipynb` & `moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/cobol_relationships_data_grid.ipynb`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/dependency_vulnerabilities.ipynb` & `moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/dependency_vulnerabilities.ipynb`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/dev/parse_failure_analysis.yml` & `moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/dev/parse_failure_analysis.yml`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/find_methods.ipynb` & `moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/find_methods.ipynb`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/find_source_files.ipynb` & `moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/find_source_files.ipynb`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/gradle_wrappers.ipynb` & `moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/gradle_wrappers.ipynb`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/images/cobol_find_copy_book.300.png` & `moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/images/cobol_find_copy_book.300.png`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/images/cobol_relationships.300.png` & `moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/images/cobol_relationships.300.png`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/images/cobol_relationships_data_grid.300.png` & `moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/images/cobol_relationships_data_grid.300.png`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/images/dependency_vulnerabilities.300.png` & `moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/images/dependency_vulnerabilities.300.png`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/images/gradle_wrappers.300.png` & `moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/images/gradle_wrappers.300.png`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/images/language_composition.300.png` & `moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/images/language_composition.300.png`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/images/language_composition_by_folder.300.png` & `moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/images/language_composition_by_folder.300.png`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/images/parse_failure_analysis.300.png` & `moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/images/parse_failure_analysis.300.png`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/images/sql_crud.300.png` & `moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/images/sql_crud.300.png`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/language_composition.ipynb` & `moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/language_composition.ipynb`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/language_composition_by_folder.ipynb` & `moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/language_composition_by_folder.ipynb`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/lst_provenance.ipynb` & `moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/lst_provenance.ipynb`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/parse_failure_analysis.ipynb` & `moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/parse_failure_analysis.ipynb`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/specs/cobol_relationships.yml` & `moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/specs/cobol_relationships.yml`

 * *Files 16% similar despite different names*

```diff
@@ -16,7 +16,14 @@
         - box
       required: false
   - filter_resources_related_to:
       displayName: Show only resources related to
       description: >
         Enter the name of a resource to filter the diagram to only show dependents and dependencies containing that resource.
       required: false
+  - exclude_incoming_relationships:
+      displayName: Exclude incoming relationships
+      description: Removes incoming relationships from the graph.
+      valid:
+        - true
+        - false
+      required: false
```

### Comparing `moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/specs/cobol_relationships_data_grid.yml` & `moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/specs/cobol_relationships_data_grid.yml`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/specs/dependency_vulnerabilities.yml` & `moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/specs/dependency_vulnerabilities.yml`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/specs/sql_crud.yml` & `moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/specs/sql_crud.yml`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.8.0/moderne_visualizations_misc/sql_crud.ipynb` & `moderne_visualizations_misc-0.9.0/moderne_visualizations_misc/sql_crud.ipynb`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.8.0/moderne_visualizations_misc.egg-info/SOURCES.txt` & `moderne_visualizations_misc-0.9.0/moderne_visualizations_misc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.8.0/pyproject.toml` & `moderne_visualizations_misc-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # @see https://packaging.python.org/en/latest/specifications/declaring-project-metadata/
 [project]
 name = "moderne_visualizations_misc"
-version = "0.8.0"
+version = "0.9.0"
 description = "Miscellaneous visualizations for the Moderne platform"
 authors = [
     { name = "Jonathan Schneider", email = "jonathan@moderne.io" },
     { name = "Kyle Scully", email = "kyle@moderne.io" }
 ]
 license = { text = "Apache-2.0" }
 dependencies = [
```

