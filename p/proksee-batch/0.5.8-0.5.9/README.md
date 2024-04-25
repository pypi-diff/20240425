# Comparing `tmp/proksee_batch-0.5.8.tar.gz` & `tmp/proksee_batch-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proksee_batch-0.5.8.tar", max compression
+gzip compressed data, was "proksee_batch-0.5.9.tar", max compression
```

## Comparing `proksee_batch-0.5.8.tar` & `proksee_batch-0.5.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     1089 2024-04-17 21:23:08.914157 proksee_batch-0.5.8/LICENSE
--rw-r--r--   0        0        0     3861 2024-04-17 21:23:08.914157 proksee_batch-0.5.8/README.md
--rw-r--r--   0        0        0     1797 2024-04-17 21:23:17.478129 proksee_batch-0.5.8/pyproject.toml
--rw-r--r--   0        0        0       21 2024-04-17 21:23:08.918157 proksee_batch-0.5.8/src/proksee_batch/__init__.py
--rw-r--r--   0        0        0    15177 2024-04-17 21:23:08.918157 proksee_batch-0.5.8/src/proksee_batch/__main__.py
--rw-r--r--   0        0        0     2330 2024-04-17 21:23:08.918157 proksee_batch-0.5.8/src/proksee_batch/data/assets/images/GitHub-Mark-Light-64px.png
--rw-r--r--   0        0        0    22591 2024-04-17 21:23:08.918157 proksee_batch-0.5.8/src/proksee_batch/data/assets/scripts/batch.js
--rw-r--r--   0        0        0   208923 2024-04-17 21:23:08.918157 proksee_batch-0.5.8/src/proksee_batch/data/assets/scripts/cgview.min.js
--rw-r--r--   0        0        0     1843 2024-04-17 21:23:08.918157 proksee_batch-0.5.8/src/proksee_batch/data/assets/scripts/controls.js
--rw-r--r--   0        0        0   274269 2024-04-17 21:23:08.918157 proksee_batch-0.5.8/src/proksee_batch/data/assets/scripts/d3.min.js
--rw-r--r--   0        0        0    61938 2024-04-17 21:23:08.918157 proksee_batch-0.5.8/src/proksee_batch/data/assets/scripts/svgcanvas.iife.js
--rw-r--r--   0        0        0    14980 2024-04-17 21:23:08.918157 proksee_batch-0.5.8/src/proksee_batch/data/assets/styles/cgview.css
--rw-r--r--   0        0        0     5696 2024-04-17 21:23:08.918157 proksee_batch-0.5.8/src/proksee_batch/data/assets/styles/controls.css
--rw-r--r--   0        0        0    12170 2024-04-17 21:23:08.918157 proksee_batch-0.5.8/src/proksee_batch/data/assets/styles/style.css
--rw-r--r--   0        0        0  5809583 2024-04-17 21:23:08.950157 proksee_batch-0.5.8/src/proksee_batch/data/data.example/genome_maps/genome_1.js
--rw-r--r--   0        0        0  5469891 2024-04-17 21:23:08.958157 proksee_batch-0.5.8/src/proksee_batch/data/data.example/genome_maps/genome_2.js
--rw-r--r--   0        0        0  6164597 2024-04-17 21:23:08.978157 proksee_batch-0.5.8/src/proksee_batch/data/data.example/genome_maps/genome_3.js
--rw-r--r--   0        0        0  7518134 2024-04-17 21:23:09.002157 proksee_batch-0.5.8/src/proksee_batch/data/data.example/genome_maps/genome_4.js
--rw-r--r--   0        0        0     3605 2024-04-17 21:23:09.002157 proksee_batch-0.5.8/src/proksee_batch/data/data.example/table_data.js
--rw-r--r--   0        0        0   221376 2024-04-17 21:23:09.002157 proksee_batch-0.5.8/src/proksee_batch/data/default_proksee_template.json
--rw-r--r--   0        0        0      158 2024-04-17 21:23:09.002157 proksee_batch-0.5.8/src/proksee_batch/data/example_input_dir/Escherichia_coli_str._K-12_substr._MG1655/bed/e_coli_features.bed
--rw-r--r--   0        0        0      269 2024-04-17 21:23:09.002157 proksee_batch-0.5.8/src/proksee_batch/data/example_input_dir/Escherichia_coli_str._K-12_substr._MG1655/blast/blast_against_e_coli.txt
--rw-r--r--   0        0        0      180 2024-04-17 21:23:09.002157 proksee_batch-0.5.8/src/proksee_batch/data/example_input_dir/Escherichia_coli_str._K-12_substr._MG1655/vcf/e_coli_variants.vcf
--rw-r--r--   0        0        0       79 2024-04-17 21:23:09.002157 proksee_batch-0.5.8/src/proksee_batch/data/example_input_dir/Klebsiella_aerogenes/bed/k_aerogenes_features.bed
--rw-r--r--   0        0        0      134 2024-04-17 21:23:09.002157 proksee_batch-0.5.8/src/proksee_batch/data/example_input_dir/Klebsiella_aerogenes/blast/blast_against_k_aerogenes.txt
--rw-r--r--   0        0        0       75 2024-04-17 21:23:09.002157 proksee_batch-0.5.8/src/proksee_batch/data/example_input_dir/Salmonella_enterica_subsp._enterica_serovar_Typhimurium_str._LT2/bed/s_enterica_features.bed
--rw-r--r--   0        0        0      130 2024-04-17 21:23:09.002157 proksee_batch-0.5.8/src/proksee_batch/data/example_input_dir/Salmonella_enterica_subsp._enterica_serovar_Typhimurium_str._LT2/blast/blast_against_s_enterica.txt
--rw-r--r--   0        0        0       75 2024-04-17 21:23:09.002157 proksee_batch-0.5.8/src/proksee_batch/data/example_input_dir/Shigella_flexneri_2a_str._301/bed/s_flexneri_features.bed
--rw-r--r--   0        0        0      130 2024-04-17 21:23:09.002157 proksee_batch-0.5.8/src/proksee_batch/data/example_input_dir/Shigella_flexneri_2a_str._301/blast/blast_against_s_flexneri.txt
--rw-r--r--   0        0        0     5127 2024-04-17 21:23:09.002157 proksee_batch-0.5.8/src/proksee_batch/data/report.html
--rw-r--r--   0        0        0     6474 2024-04-17 21:23:09.002157 proksee_batch-0.5.8/src/proksee_batch/download_example_input.py
--rw-r--r--   0        0        0      895 2024-04-17 21:23:09.002157 proksee_batch-0.5.8/src/proksee_batch/generate_proksee_link.py
--rw-r--r--   0        0        0     5311 2024-04-17 21:23:09.006157 proksee_batch-0.5.8/src/proksee_batch/generate_report_html.py
--rw-r--r--   0        0        0     1037 2024-04-17 21:23:09.006157 proksee_batch-0.5.8/src/proksee_batch/get_stats_from_seq_file.py
--rw-r--r--   0        0        0     1952 2024-04-17 21:23:09.006157 proksee_batch-0.5.8/src/proksee_batch/merge_cgview_json_with_template.py
--rw-r--r--   0        0        0    21297 2024-04-17 21:23:09.006157 proksee_batch-0.5.8/src/proksee_batch/parse_additional_features.py
--rw-r--r--   0        0        0        0 2024-04-17 21:23:09.006157 proksee_batch-0.5.8/src/proksee_batch/py.typed
--rw-r--r--   0        0        0     1163 2024-04-17 21:23:09.006157 proksee_batch-0.5.8/src/proksee_batch/remove_covered_features.py
--rw-r--r--   0        0        0     2658 2024-04-17 21:23:09.006157 proksee_batch-0.5.8/src/proksee_batch/scrape_proksee_image.py
--rw-r--r--   0        0        0    11471 2024-04-17 21:23:09.006157 proksee_batch-0.5.8/src/proksee_batch/seq_file_to_cgview_json.py
--rw-r--r--   0        0        0    24047 2024-04-17 21:23:09.006157 proksee_batch-0.5.8/src/proksee_batch/validate_input_data.py
--rw-r--r--   0        0        0     5058 1970-01-01 00:00:00.000000 proksee_batch-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-04-18 15:56:28.918512 proksee_batch-0.5.9/LICENSE
+-rw-r--r--   0        0        0     3861 2024-04-18 15:56:28.918512 proksee_batch-0.5.9/README.md
+-rw-r--r--   0        0        0     1797 2024-04-18 15:56:40.294520 proksee_batch-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0       21 2024-04-18 15:56:28.922512 proksee_batch-0.5.9/src/proksee_batch/__init__.py
+-rw-r--r--   0        0        0    15177 2024-04-18 15:56:28.922512 proksee_batch-0.5.9/src/proksee_batch/__main__.py
+-rw-r--r--   0        0        0     2330 2024-04-18 15:56:28.922512 proksee_batch-0.5.9/src/proksee_batch/data/assets/images/GitHub-Mark-Light-64px.png
+-rw-r--r--   0        0        0    22591 2024-04-18 15:56:28.922512 proksee_batch-0.5.9/src/proksee_batch/data/assets/scripts/batch.js
+-rw-r--r--   0        0        0   208923 2024-04-18 15:56:28.926512 proksee_batch-0.5.9/src/proksee_batch/data/assets/scripts/cgview.min.js
+-rw-r--r--   0        0        0     1843 2024-04-18 15:56:28.926512 proksee_batch-0.5.9/src/proksee_batch/data/assets/scripts/controls.js
+-rw-r--r--   0        0        0   274269 2024-04-18 15:56:28.926512 proksee_batch-0.5.9/src/proksee_batch/data/assets/scripts/d3.min.js
+-rw-r--r--   0        0        0    61938 2024-04-18 15:56:28.926512 proksee_batch-0.5.9/src/proksee_batch/data/assets/scripts/svgcanvas.iife.js
+-rw-r--r--   0        0        0    14980 2024-04-18 15:56:28.926512 proksee_batch-0.5.9/src/proksee_batch/data/assets/styles/cgview.css
+-rw-r--r--   0        0        0     5696 2024-04-18 15:56:28.926512 proksee_batch-0.5.9/src/proksee_batch/data/assets/styles/controls.css
+-rw-r--r--   0        0        0    12170 2024-04-18 15:56:28.926512 proksee_batch-0.5.9/src/proksee_batch/data/assets/styles/style.css
+-rw-r--r--   0        0        0  5809583 2024-04-18 15:56:28.954512 proksee_batch-0.5.9/src/proksee_batch/data/data.example/genome_maps/genome_1.js
+-rw-r--r--   0        0        0  5469891 2024-04-18 15:56:28.962512 proksee_batch-0.5.9/src/proksee_batch/data/data.example/genome_maps/genome_2.js
+-rw-r--r--   0        0        0  6164597 2024-04-18 15:56:28.986512 proksee_batch-0.5.9/src/proksee_batch/data/data.example/genome_maps/genome_3.js
+-rw-r--r--   0        0        0  7518134 2024-04-18 15:56:29.010512 proksee_batch-0.5.9/src/proksee_batch/data/data.example/genome_maps/genome_4.js
+-rw-r--r--   0        0        0     3605 2024-04-18 15:56:29.010512 proksee_batch-0.5.9/src/proksee_batch/data/data.example/table_data.js
+-rw-r--r--   0        0        0   221376 2024-04-18 15:56:29.010512 proksee_batch-0.5.9/src/proksee_batch/data/default_proksee_template.json
+-rw-r--r--   0        0        0      158 2024-04-18 15:56:29.010512 proksee_batch-0.5.9/src/proksee_batch/data/example_input_dir/Escherichia_coli_str._K-12_substr._MG1655/bed/e_coli_features.bed
+-rw-r--r--   0        0        0      269 2024-04-18 15:56:29.010512 proksee_batch-0.5.9/src/proksee_batch/data/example_input_dir/Escherichia_coli_str._K-12_substr._MG1655/blast/blast_against_e_coli.txt
+-rw-r--r--   0        0        0      180 2024-04-18 15:56:29.010512 proksee_batch-0.5.9/src/proksee_batch/data/example_input_dir/Escherichia_coli_str._K-12_substr._MG1655/vcf/e_coli_variants.vcf
+-rw-r--r--   0        0        0       79 2024-04-18 15:56:29.010512 proksee_batch-0.5.9/src/proksee_batch/data/example_input_dir/Klebsiella_aerogenes/bed/k_aerogenes_features.bed
+-rw-r--r--   0        0        0      134 2024-04-18 15:56:29.010512 proksee_batch-0.5.9/src/proksee_batch/data/example_input_dir/Klebsiella_aerogenes/blast/blast_against_k_aerogenes.txt
+-rw-r--r--   0        0        0       75 2024-04-18 15:56:29.010512 proksee_batch-0.5.9/src/proksee_batch/data/example_input_dir/Salmonella_enterica_subsp._enterica_serovar_Typhimurium_str._LT2/bed/s_enterica_features.bed
+-rw-r--r--   0        0        0      130 2024-04-18 15:56:29.010512 proksee_batch-0.5.9/src/proksee_batch/data/example_input_dir/Salmonella_enterica_subsp._enterica_serovar_Typhimurium_str._LT2/blast/blast_against_s_enterica.txt
+-rw-r--r--   0        0        0       75 2024-04-18 15:56:29.010512 proksee_batch-0.5.9/src/proksee_batch/data/example_input_dir/Shigella_flexneri_2a_str._301/bed/s_flexneri_features.bed
+-rw-r--r--   0        0        0      130 2024-04-18 15:56:29.010512 proksee_batch-0.5.9/src/proksee_batch/data/example_input_dir/Shigella_flexneri_2a_str._301/blast/blast_against_s_flexneri.txt
+-rw-r--r--   0        0        0     5127 2024-04-18 15:56:29.010512 proksee_batch-0.5.9/src/proksee_batch/data/report.html
+-rw-r--r--   0        0        0     6474 2024-04-18 15:56:29.010512 proksee_batch-0.5.9/src/proksee_batch/download_example_input.py
+-rw-r--r--   0        0        0      895 2024-04-18 15:56:29.010512 proksee_batch-0.5.9/src/proksee_batch/generate_proksee_link.py
+-rw-r--r--   0        0        0     5311 2024-04-18 15:56:29.010512 proksee_batch-0.5.9/src/proksee_batch/generate_report_html.py
+-rw-r--r--   0        0        0     1037 2024-04-18 15:56:29.010512 proksee_batch-0.5.9/src/proksee_batch/get_stats_from_seq_file.py
+-rw-r--r--   0        0        0     1952 2024-04-18 15:56:29.010512 proksee_batch-0.5.9/src/proksee_batch/merge_cgview_json_with_template.py
+-rw-r--r--   0        0        0    21812 2024-04-18 15:56:29.010512 proksee_batch-0.5.9/src/proksee_batch/parse_additional_features.py
+-rw-r--r--   0        0        0        0 2024-04-18 15:56:29.010512 proksee_batch-0.5.9/src/proksee_batch/py.typed
+-rw-r--r--   0        0        0     1163 2024-04-18 15:56:29.010512 proksee_batch-0.5.9/src/proksee_batch/remove_covered_features.py
+-rw-r--r--   0        0        0     2658 2024-04-18 15:56:29.010512 proksee_batch-0.5.9/src/proksee_batch/scrape_proksee_image.py
+-rw-r--r--   0        0        0    11471 2024-04-18 15:56:29.010512 proksee_batch-0.5.9/src/proksee_batch/seq_file_to_cgview_json.py
+-rw-r--r--   0        0        0    24047 2024-04-18 15:56:29.010512 proksee_batch-0.5.9/src/proksee_batch/validate_input_data.py
+-rw-r--r--   0        0        0     5058 1970-01-01 00:00:00.000000 proksee_batch-0.5.9/PKG-INFO
```

### Comparing `proksee_batch-0.5.8/LICENSE` & `proksee_batch-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.8/README.md` & `proksee_batch-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.8/pyproject.toml` & `proksee_batch-0.5.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "proksee-batch"
-version = "0.5.8"
+version = "0.5.9"
 description = "Proksee Batch"
 authors = ["Lael D. Barlow"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/stothard-group/proksee-batch"
 repository = "https://github.com/stothard-group/proksee-batch"
 documentation = "https://proksee-batch.readthedocs.io"
```

### Comparing `proksee_batch-0.5.8/src/proksee_batch/__main__.py` & `proksee_batch-0.5.9/src/proksee_batch/__main__.py`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.8/src/proksee_batch/data/assets/images/GitHub-Mark-Light-64px.png` & `proksee_batch-0.5.9/src/proksee_batch/data/assets/images/GitHub-Mark-Light-64px.png`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.8/src/proksee_batch/data/assets/scripts/batch.js` & `proksee_batch-0.5.9/src/proksee_batch/data/assets/scripts/batch.js`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.8/src/proksee_batch/data/assets/scripts/cgview.min.js` & `proksee_batch-0.5.9/src/proksee_batch/data/assets/scripts/cgview.min.js`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.8/src/proksee_batch/data/assets/scripts/controls.js` & `proksee_batch-0.5.9/src/proksee_batch/data/assets/scripts/controls.js`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.8/src/proksee_batch/data/assets/scripts/d3.min.js` & `proksee_batch-0.5.9/src/proksee_batch/data/assets/scripts/d3.min.js`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.8/src/proksee_batch/data/assets/scripts/svgcanvas.iife.js` & `proksee_batch-0.5.9/src/proksee_batch/data/assets/scripts/svgcanvas.iife.js`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.8/src/proksee_batch/data/assets/styles/cgview.css` & `proksee_batch-0.5.9/src/proksee_batch/data/assets/styles/cgview.css`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.8/src/proksee_batch/data/assets/styles/controls.css` & `proksee_batch-0.5.9/src/proksee_batch/data/assets/styles/controls.css`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.8/src/proksee_batch/data/assets/styles/style.css` & `proksee_batch-0.5.9/src/proksee_batch/data/assets/styles/style.css`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.8/src/proksee_batch/data/data.example/genome_maps/genome_1.js` & `proksee_batch-0.5.9/src/proksee_batch/data/data.example/genome_maps/genome_1.js`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.8/src/proksee_batch/data/data.example/genome_maps/genome_2.js` & `proksee_batch-0.5.9/src/proksee_batch/data/data.example/genome_maps/genome_2.js`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.8/src/proksee_batch/data/data.example/genome_maps/genome_3.js` & `proksee_batch-0.5.9/src/proksee_batch/data/data.example/genome_maps/genome_3.js`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.8/src/proksee_batch/data/data.example/genome_maps/genome_4.js` & `proksee_batch-0.5.9/src/proksee_batch/data/data.example/genome_maps/genome_4.js`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.8/src/proksee_batch/data/data.example/table_data.js` & `proksee_batch-0.5.9/src/proksee_batch/data/data.example/table_data.js`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.8/src/proksee_batch/data/default_proksee_template.json` & `proksee_batch-0.5.9/src/proksee_batch/data/default_proksee_template.json`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.8/src/proksee_batch/data/report.html` & `proksee_batch-0.5.9/src/proksee_batch/data/report.html`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.8/src/proksee_batch/download_example_input.py` & `proksee_batch-0.5.9/src/proksee_batch/download_example_input.py`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.8/src/proksee_batch/generate_proksee_link.py` & `proksee_batch-0.5.9/src/proksee_batch/generate_proksee_link.py`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.8/src/proksee_batch/generate_report_html.py` & `proksee_batch-0.5.9/src/proksee_batch/generate_report_html.py`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.8/src/proksee_batch/get_stats_from_seq_file.py` & `proksee_batch-0.5.9/src/proksee_batch/get_stats_from_seq_file.py`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.8/src/proksee_batch/merge_cgview_json_with_template.py` & `proksee_batch-0.5.9/src/proksee_batch/merge_cgview_json_with_template.py`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.8/src/proksee_batch/parse_additional_features.py` & `proksee_batch-0.5.9/src/proksee_batch/parse_additional_features.py`

 * *Files 1% similar despite different names*

```diff
@@ -529,35 +529,48 @@
             ":memory:",
             force=True,
             keep_order=True,
             merge_strategy="merge",
             sort_attribute_values=True,
         )
 
+        # Define feature types to include.
+        feature_types_to_exclude = ["gene", "exon", "region"]
+
         # Parse the GFF file.
         for gff_result in db.all_features():
-            # Skip the header line(s), if present.
-            if gff_result.featuretype == "region":
+            # Skip the header line(s), if present, and feature types to exclude.
+            if gff_result.featuretype in feature_types_to_exclude:
                 continue
 
+            # Define the name based on availability.
+            name = gff_result.id
+            if "gene" in gff_result.attributes:
+                name = gff_result.attributes["gene"][0]
+
             # Define the GFF feature.
             gff_feature = {
-                "name": gff_result.id,
+                "name": name,
                 "type": "gff",
                 "start": gff_result.start,
                 "stop": gff_result.stop,
                 "strand": gff_result.strand,
                 "source": f"gff_{num}",
                 "contig": gff_result.seqid,
                 "legend": os.path.basename(gff_file),
                 "tags": [],
                 "meta": {
-                    "score": gff_result.score,
+                    "score": "0",
                 },
             }
+
+            # Add any additional metadata, if present.
+            for attribute in gff_result.attributes:
+                gff_feature["meta"][attribute] = gff_result.attributes[attribute][0]
+
             # Add the GFF feature to the list of GFF features.
             gff_features.append(gff_feature)
 
     # Remove GFF features that are completely covered by another GFF feature
     # with an equal or higher score.
     gff_features = [
         gff_feature
```

### Comparing `proksee_batch-0.5.8/src/proksee_batch/remove_covered_features.py` & `proksee_batch-0.5.9/src/proksee_batch/remove_covered_features.py`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.8/src/proksee_batch/scrape_proksee_image.py` & `proksee_batch-0.5.9/src/proksee_batch/scrape_proksee_image.py`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.8/src/proksee_batch/seq_file_to_cgview_json.py` & `proksee_batch-0.5.9/src/proksee_batch/seq_file_to_cgview_json.py`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.8/src/proksee_batch/validate_input_data.py` & `proksee_batch-0.5.9/src/proksee_batch/validate_input_data.py`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.8/PKG-INFO` & `proksee_batch-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proksee-batch
-Version: 0.5.8
+Version: 0.5.9
 Summary: Proksee Batch
 Home-page: https://github.com/stothard-group/proksee-batch
 License: MIT
 Author: Lael D. Barlow
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

