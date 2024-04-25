# Comparing `tmp/pheval-0.3.3.tar.gz` & `tmp/pheval-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pheval-0.3.3.tar", max compression
+gzip compressed data, was "pheval-0.3.4.tar", max compression
```

## Comparing `pheval-0.3.3.tar` & `pheval-0.3.4.tar`

### file list

```diff
@@ -1,55 +1,56 @@
--rw-r--r--   0        0        0    11357 2024-04-24 13:39:23.412420 pheval-0.3.3/LICENSE
--rw-r--r--   0        0        0      751 2024-04-24 13:39:23.412420 pheval-0.3.3/README.md
--rw-r--r--   0        0        0     1529 2024-04-24 13:39:23.472420 pheval-0.3.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-24 13:39:23.472420 pheval-0.3.3/src/pheval/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 13:39:23.472420 pheval-0.3.3/src/pheval/analyse/__init__.py
--rw-r--r--   0        0        0     7743 2024-04-24 13:39:23.472420 pheval-0.3.3/src/pheval/analyse/analysis.py
--rw-r--r--   0        0        0     5943 2024-04-24 13:39:23.472420 pheval-0.3.3/src/pheval/analyse/benchmark_generator.py
--rw-r--r--   0        0        0      768 2024-04-24 13:39:23.472420 pheval-0.3.3/src/pheval/analyse/benchmarking_data.py
--rw-r--r--   0        0        0    12519 2024-04-24 13:39:23.472420 pheval-0.3.3/src/pheval/analyse/binary_classification_stats.py
--rw-r--r--   0        0        0    12649 2024-04-24 13:39:23.472420 pheval-0.3.3/src/pheval/analyse/disease_prioritisation_analysis.py
--rw-r--r--   0        0        0    12373 2024-04-24 13:39:23.472420 pheval-0.3.3/src/pheval/analyse/gene_prioritisation_analysis.py
--rw-r--r--   0        0        0    21350 2024-04-24 13:39:23.472420 pheval-0.3.3/src/pheval/analyse/generate_plots.py
--rw-r--r--   0        0        0     6591 2024-04-24 13:39:23.472420 pheval-0.3.3/src/pheval/analyse/generate_summary_outputs.py
--rw-r--r--   0        0        0     2384 2024-04-24 13:39:23.472420 pheval-0.3.3/src/pheval/analyse/parse_benchmark_summary.py
--rw-r--r--   0        0        0     1211 2024-04-24 13:39:23.472420 pheval-0.3.3/src/pheval/analyse/parse_pheval_result.py
--rw-r--r--   0        0        0     3223 2024-04-24 13:39:23.472420 pheval-0.3.3/src/pheval/analyse/prioritisation_rank_recorder.py
--rw-r--r--   0        0        0     1228 2024-04-24 13:39:23.472420 pheval-0.3.3/src/pheval/analyse/prioritisation_result_types.py
--rw-r--r--   0        0        0    15785 2024-04-24 13:39:23.472420 pheval-0.3.3/src/pheval/analyse/rank_stats.py
--rw-r--r--   0        0        0     1552 2024-04-24 13:39:23.472420 pheval-0.3.3/src/pheval/analyse/run_data_parser.py
--rw-r--r--   0        0        0    12384 2024-04-24 13:39:23.472420 pheval-0.3.3/src/pheval/analyse/variant_prioritisation_analysis.py
--rw-r--r--   0        0        0     1493 2024-04-24 13:39:23.472420 pheval-0.3.3/src/pheval/cli.py
--rw-r--r--   0        0        0     2424 2024-04-24 13:39:23.472420 pheval-0.3.3/src/pheval/cli_pheval.py
--rw-r--r--   0        0        0    17257 2024-04-24 13:39:23.472420 pheval-0.3.3/src/pheval/cli_pheval_utils.py
--rw-r--r--   0        0        0     1227 2024-04-24 13:39:23.472420 pheval-0.3.3/src/pheval/config_parser.py
--rw-r--r--   0        0        0      349 2024-04-24 13:39:23.472420 pheval-0.3.3/src/pheval/constants.py
--rw-r--r--   0        0        0     1228 2024-04-24 13:39:23.472420 pheval-0.3.3/src/pheval/implementations/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 13:39:23.472420 pheval-0.3.3/src/pheval/infra/__init__.py
--rw-r--r--   0        0        0     5080 2024-04-24 13:39:23.472420 pheval-0.3.3/src/pheval/infra/exomiserdb.py
--rw-r--r--   0        0        0        0 2024-04-24 13:39:23.472420 pheval-0.3.3/src/pheval/post_processing/__init__.py
--rw-r--r--   0        0        0    16030 2024-04-24 13:39:23.472420 pheval-0.3.3/src/pheval/post_processing/post_processing.py
--rw-r--r--   0        0        0        0 2024-04-24 13:39:23.472420 pheval-0.3.3/src/pheval/prepare/__init__.py
--rw-r--r--   0        0        0    11236 2024-04-24 13:39:23.472420 pheval-0.3.3/src/pheval/prepare/create_noisy_phenopackets.py
--rw-r--r--   0        0        0    20235 2024-04-24 13:39:23.472420 pheval-0.3.3/src/pheval/prepare/create_spiked_vcf.py
--rw-r--r--   0        0        0     1719 2024-04-24 13:39:23.472420 pheval-0.3.3/src/pheval/prepare/custom_exceptions.py
--rw-r--r--   0        0        0     4753 2024-04-24 13:39:23.472420 pheval-0.3.3/src/pheval/prepare/update_phenopacket.py
--rw-r--r--   0        0        0      547 2024-04-24 13:39:23.472420 pheval-0.3.3/src/pheval/resources/alternate_ouputs/CADA_results.txt
--rw-r--r--   0        0        0     1508 2024-04-24 13:39:23.472420 pheval-0.3.3/src/pheval/resources/alternate_ouputs/DeepPVP_results.txt
--rw-r--r--   0        0        0     9845 2024-04-24 13:39:23.472420 pheval-0.3.3/src/pheval/resources/alternate_ouputs/OVA_results.txt
--rw-r--r--   0        0        0    14148 2024-04-24 13:39:23.472420 pheval-0.3.3/src/pheval/resources/alternate_ouputs/Phen2Gene_results.json
--rw-r--r--   0        0        0      594 2024-04-24 13:39:23.472420 pheval-0.3.3/src/pheval/resources/alternate_ouputs/Phenolyzer_results.txt
--rw-r--r--   0        0        0   431068 2024-04-24 13:39:23.476420 pheval-0.3.3/src/pheval/resources/alternate_ouputs/lirical_results.tsv
--rw-r--r--   0        0        0      714 2024-04-24 13:39:23.476420 pheval-0.3.3/src/pheval/resources/alternate_ouputs/svanna_results.tsv
--rw-r--r--   0        0        0 16462969 2024-04-24 13:39:23.540420 pheval-0.3.3/src/pheval/resources/hgnc_complete_set.txt
--rw-r--r--   0        0        0      919 2024-04-24 13:39:23.540420 pheval-0.3.3/src/pheval/run_metadata.py
--rw-r--r--   0        0        0        0 2024-04-24 13:39:23.540420 pheval-0.3.3/src/pheval/runners/__init__.py
--rw-r--r--   0        0        0     4451 2024-04-24 13:39:23.540420 pheval-0.3.3/src/pheval/runners/runner.py
--rw-r--r--   0        0        0        0 2024-04-24 13:39:23.540420 pheval-0.3.3/src/pheval/utils/__init__.py
--rw-r--r--   0        0        0     3193 2024-04-24 13:39:23.540420 pheval-0.3.3/src/pheval/utils/docs_gen.py
--rwxr-xr-x   0        0        0      477 2024-04-24 13:39:23.540420 pheval-0.3.3/src/pheval/utils/docs_gen.sh
--rw-r--r--   0        0        0      683 2024-04-24 13:39:23.540420 pheval-0.3.3/src/pheval/utils/exomiser.py
--rw-r--r--   0        0        0     4640 2024-04-24 13:39:23.540420 pheval-0.3.3/src/pheval/utils/file_utils.py
--rw-r--r--   0        0        0    24444 2024-04-24 13:39:23.540420 pheval-0.3.3/src/pheval/utils/phenopacket_utils.py
--rw-r--r--   0        0        0     6151 2024-04-24 13:39:23.540420 pheval-0.3.3/src/pheval/utils/semsim_utils.py
--rw-r--r--   0        0        0     2343 2024-04-24 13:39:23.540420 pheval-0.3.3/src/pheval/utils/utils.py
--rw-r--r--   0        0        0     1810 1970-01-01 00:00:00.000000 pheval-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-25 11:56:32.578238 pheval-0.3.4/LICENSE
+-rw-r--r--   0        0        0      751 2024-04-25 11:56:32.578238 pheval-0.3.4/README.md
+-rw-r--r--   0        0        0     1529 2024-04-25 11:56:32.638239 pheval-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-25 11:56:32.638239 pheval-0.3.4/src/pheval/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 11:56:32.638239 pheval-0.3.4/src/pheval/analyse/__init__.py
+-rw-r--r--   0        0        0     7743 2024-04-25 11:56:32.638239 pheval-0.3.4/src/pheval/analyse/analysis.py
+-rw-r--r--   0        0        0     5943 2024-04-25 11:56:32.638239 pheval-0.3.4/src/pheval/analyse/benchmark_generator.py
+-rw-r--r--   0        0        0      768 2024-04-25 11:56:32.638239 pheval-0.3.4/src/pheval/analyse/benchmarking_data.py
+-rw-r--r--   0        0        0    12519 2024-04-25 11:56:32.638239 pheval-0.3.4/src/pheval/analyse/binary_classification_stats.py
+-rw-r--r--   0        0        0    12649 2024-04-25 11:56:32.638239 pheval-0.3.4/src/pheval/analyse/disease_prioritisation_analysis.py
+-rw-r--r--   0        0        0    12373 2024-04-25 11:56:32.638239 pheval-0.3.4/src/pheval/analyse/gene_prioritisation_analysis.py
+-rw-r--r--   0        0        0    21350 2024-04-25 11:56:32.638239 pheval-0.3.4/src/pheval/analyse/generate_plots.py
+-rw-r--r--   0        0        0     6591 2024-04-25 11:56:32.638239 pheval-0.3.4/src/pheval/analyse/generate_summary_outputs.py
+-rw-r--r--   0        0        0     2384 2024-04-25 11:56:32.638239 pheval-0.3.4/src/pheval/analyse/parse_benchmark_summary.py
+-rw-r--r--   0        0        0     1211 2024-04-25 11:56:32.638239 pheval-0.3.4/src/pheval/analyse/parse_pheval_result.py
+-rw-r--r--   0        0        0     3223 2024-04-25 11:56:32.638239 pheval-0.3.4/src/pheval/analyse/prioritisation_rank_recorder.py
+-rw-r--r--   0        0        0     1228 2024-04-25 11:56:32.638239 pheval-0.3.4/src/pheval/analyse/prioritisation_result_types.py
+-rw-r--r--   0        0        0    15785 2024-04-25 11:56:32.638239 pheval-0.3.4/src/pheval/analyse/rank_stats.py
+-rw-r--r--   0        0        0     1552 2024-04-25 11:56:32.638239 pheval-0.3.4/src/pheval/analyse/run_data_parser.py
+-rw-r--r--   0        0        0    12384 2024-04-25 11:56:32.638239 pheval-0.3.4/src/pheval/analyse/variant_prioritisation_analysis.py
+-rw-r--r--   0        0        0     1570 2024-04-25 11:56:32.638239 pheval-0.3.4/src/pheval/cli.py
+-rw-r--r--   0        0        0     2424 2024-04-25 11:56:32.638239 pheval-0.3.4/src/pheval/cli_pheval.py
+-rw-r--r--   0        0        0    20504 2024-04-25 11:56:32.638239 pheval-0.3.4/src/pheval/cli_pheval_utils.py
+-rw-r--r--   0        0        0     1227 2024-04-25 11:56:32.638239 pheval-0.3.4/src/pheval/config_parser.py
+-rw-r--r--   0        0        0      349 2024-04-25 11:56:32.638239 pheval-0.3.4/src/pheval/constants.py
+-rw-r--r--   0        0        0     1228 2024-04-25 11:56:32.638239 pheval-0.3.4/src/pheval/implementations/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 11:56:32.638239 pheval-0.3.4/src/pheval/infra/__init__.py
+-rw-r--r--   0        0        0     5080 2024-04-25 11:56:32.638239 pheval-0.3.4/src/pheval/infra/exomiserdb.py
+-rw-r--r--   0        0        0        0 2024-04-25 11:56:32.638239 pheval-0.3.4/src/pheval/post_processing/__init__.py
+-rw-r--r--   0        0        0    16030 2024-04-25 11:56:32.638239 pheval-0.3.4/src/pheval/post_processing/post_processing.py
+-rw-r--r--   0        0        0        0 2024-04-25 11:56:32.638239 pheval-0.3.4/src/pheval/prepare/__init__.py
+-rw-r--r--   0        0        0    11236 2024-04-25 11:56:32.638239 pheval-0.3.4/src/pheval/prepare/create_noisy_phenopackets.py
+-rw-r--r--   0        0        0    20235 2024-04-25 11:56:32.638239 pheval-0.3.4/src/pheval/prepare/create_spiked_vcf.py
+-rw-r--r--   0        0        0     1719 2024-04-25 11:56:32.638239 pheval-0.3.4/src/pheval/prepare/custom_exceptions.py
+-rw-r--r--   0        0        0     3187 2024-04-25 11:56:32.638239 pheval-0.3.4/src/pheval/prepare/prepare_corpus.py
+-rw-r--r--   0        0        0     4770 2024-04-25 11:56:32.638239 pheval-0.3.4/src/pheval/prepare/update_phenopacket.py
+-rw-r--r--   0        0        0      547 2024-04-25 11:56:32.638239 pheval-0.3.4/src/pheval/resources/alternate_ouputs/CADA_results.txt
+-rw-r--r--   0        0        0     1508 2024-04-25 11:56:32.638239 pheval-0.3.4/src/pheval/resources/alternate_ouputs/DeepPVP_results.txt
+-rw-r--r--   0        0        0     9845 2024-04-25 11:56:32.638239 pheval-0.3.4/src/pheval/resources/alternate_ouputs/OVA_results.txt
+-rw-r--r--   0        0        0    14148 2024-04-25 11:56:32.638239 pheval-0.3.4/src/pheval/resources/alternate_ouputs/Phen2Gene_results.json
+-rw-r--r--   0        0        0      594 2024-04-25 11:56:32.638239 pheval-0.3.4/src/pheval/resources/alternate_ouputs/Phenolyzer_results.txt
+-rw-r--r--   0        0        0   431068 2024-04-25 11:56:32.642239 pheval-0.3.4/src/pheval/resources/alternate_ouputs/lirical_results.tsv
+-rw-r--r--   0        0        0      714 2024-04-25 11:56:32.642239 pheval-0.3.4/src/pheval/resources/alternate_ouputs/svanna_results.tsv
+-rw-r--r--   0        0        0 16462969 2024-04-25 11:56:32.706241 pheval-0.3.4/src/pheval/resources/hgnc_complete_set.txt
+-rw-r--r--   0        0        0      919 2024-04-25 11:56:32.706241 pheval-0.3.4/src/pheval/run_metadata.py
+-rw-r--r--   0        0        0        0 2024-04-25 11:56:32.706241 pheval-0.3.4/src/pheval/runners/__init__.py
+-rw-r--r--   0        0        0     4451 2024-04-25 11:56:32.706241 pheval-0.3.4/src/pheval/runners/runner.py
+-rw-r--r--   0        0        0        0 2024-04-25 11:56:32.706241 pheval-0.3.4/src/pheval/utils/__init__.py
+-rw-r--r--   0        0        0     3193 2024-04-25 11:56:32.706241 pheval-0.3.4/src/pheval/utils/docs_gen.py
+-rwxr-xr-x   0        0        0      477 2024-04-25 11:56:32.706241 pheval-0.3.4/src/pheval/utils/docs_gen.sh
+-rw-r--r--   0        0        0      683 2024-04-25 11:56:32.706241 pheval-0.3.4/src/pheval/utils/exomiser.py
+-rw-r--r--   0        0        0     4640 2024-04-25 11:56:32.706241 pheval-0.3.4/src/pheval/utils/file_utils.py
+-rw-r--r--   0        0        0    26792 2024-04-25 11:56:32.706241 pheval-0.3.4/src/pheval/utils/phenopacket_utils.py
+-rw-r--r--   0        0        0     6151 2024-04-25 11:56:32.706241 pheval-0.3.4/src/pheval/utils/semsim_utils.py
+-rw-r--r--   0        0        0     2343 2024-04-25 11:56:32.706241 pheval-0.3.4/src/pheval/utils/utils.py
+-rw-r--r--   0        0        0     1810 1970-01-01 00:00:00.000000 pheval-0.3.4/PKG-INFO
```

### Comparing `pheval-0.3.3/LICENSE` & `pheval-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pheval-0.3.3/README.md` & `pheval-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `pheval-0.3.3/pyproject.toml` & `pheval-0.3.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pheval"
-version = "0.3.3"
+version = "0.3.4"
 description = ""
 authors = ["Yasemin Bridges <y.bridges@qmul.ac.uk>",
   "Julius Jacobsen <j.jacobsen@qmul.ac.uk>",
   "Nico Matentzoglu <nicolas.matentzoglu@gmail.com>",
   "Vinícius de Souza <souzadevinicius@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pheval", from = "src"}]
```

### Comparing `pheval-0.3.3/src/pheval/analyse/analysis.py` & `pheval-0.3.4/src/pheval/analyse/analysis.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.3/src/pheval/analyse/benchmark_generator.py` & `pheval-0.3.4/src/pheval/analyse/benchmark_generator.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.3/src/pheval/analyse/benchmarking_data.py` & `pheval-0.3.4/src/pheval/analyse/benchmarking_data.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.3/src/pheval/analyse/binary_classification_stats.py` & `pheval-0.3.4/src/pheval/analyse/binary_classification_stats.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.3/src/pheval/analyse/disease_prioritisation_analysis.py` & `pheval-0.3.4/src/pheval/analyse/disease_prioritisation_analysis.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.3/src/pheval/analyse/gene_prioritisation_analysis.py` & `pheval-0.3.4/src/pheval/analyse/gene_prioritisation_analysis.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.3/src/pheval/analyse/generate_plots.py` & `pheval-0.3.4/src/pheval/analyse/generate_plots.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.3/src/pheval/analyse/generate_summary_outputs.py` & `pheval-0.3.4/src/pheval/analyse/generate_summary_outputs.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.3/src/pheval/analyse/parse_benchmark_summary.py` & `pheval-0.3.4/src/pheval/analyse/parse_benchmark_summary.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.3/src/pheval/analyse/parse_pheval_result.py` & `pheval-0.3.4/src/pheval/analyse/parse_pheval_result.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.3/src/pheval/analyse/prioritisation_rank_recorder.py` & `pheval-0.3.4/src/pheval/analyse/prioritisation_rank_recorder.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.3/src/pheval/analyse/prioritisation_result_types.py` & `pheval-0.3.4/src/pheval/analyse/prioritisation_result_types.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.3/src/pheval/analyse/rank_stats.py` & `pheval-0.3.4/src/pheval/analyse/rank_stats.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.3/src/pheval/analyse/run_data_parser.py` & `pheval-0.3.4/src/pheval/analyse/run_data_parser.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.3/src/pheval/analyse/variant_prioritisation_analysis.py` & `pheval-0.3.4/src/pheval/analyse/variant_prioritisation_analysis.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.3/src/pheval/cli.py` & `pheval-0.3.4/src/pheval/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from .cli_pheval import run
 from .cli_pheval_utils import (
     benchmark,
     benchmark_comparison,
     create_spiked_vcfs_command,
     generate_stats_plot,
+    prepare_corpus_command,
     scramble_phenopackets_command,
     semsim_scramble_command,
     semsim_to_exomiserdb_command,
     update_phenopackets_command,
 )
 
 info_log = logging.getLogger("info")
@@ -56,10 +57,11 @@
 pheval_utils.add_command(scramble_phenopackets_command)
 pheval_utils.add_command(update_phenopackets_command)
 pheval_utils.add_command(create_spiked_vcfs_command)
 pheval_utils.add_command(benchmark)
 pheval_utils.add_command(benchmark_comparison)
 pheval_utils.add_command(semsim_to_exomiserdb_command)
 pheval_utils.add_command(generate_stats_plot)
+pheval_utils.add_command(prepare_corpus_command)
 
 if __name__ == "__main__":
     main()
```

### Comparing `pheval-0.3.3/src/pheval/cli_pheval.py` & `pheval-0.3.4/src/pheval/cli_pheval.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.3/src/pheval/cli_pheval_utils.py` & `pheval-0.3.4/src/pheval/cli_pheval_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     benchmark_run_comparisons,
 )
 from pheval.analyse.generate_plots import generate_plots_from_benchmark_summary_tsv
 from pheval.analyse.run_data_parser import parse_run_data_text_file
 from pheval.prepare.create_noisy_phenopackets import scramble_phenopackets
 from pheval.prepare.create_spiked_vcf import spike_vcfs
 from pheval.prepare.custom_exceptions import InputError, MutuallyExclusiveOptionError
+from pheval.prepare.prepare_corpus import prepare_corpus
 from pheval.prepare.update_phenopacket import update_phenopackets
 from pheval.utils.exomiser import semsim_to_exomiserdb
 from pheval.utils.semsim_utils import percentage_diff, semsim_heatmap_plot
 from pheval.utils.utils import semsim_scramble
 
 
 @click.command("semsim-scramble")
@@ -602,7 +603,110 @@
     plot_type: str,
     title: str = None,
 ):
     """Generate bar plot from benchmark stats summary tsv."""
     generate_plots_from_benchmark_summary_tsv(
         benchmarking_tsv, gene_analysis, variant_analysis, disease_analysis, plot_type, title
     )
+
+
+@click.command("prepare-corpus")
+@click.option(
+    "--phenopacket-dir",
+    "-p",
+    required=True,
+    metavar="PATH",
+    help="Path to phenopacket corpus directory..",
+    type=Path,
+)
+@click.option(
+    "--variant-analysis/--no-variant-analysis",
+    default=False,
+    required=False,
+    type=bool,
+    show_default=True,
+    help="Specify whether to check for complete variant records in the phenopackets.",
+)
+@click.option(
+    "--gene-analysis/--no-gene-analysis",
+    default=False,
+    required=False,
+    type=bool,
+    show_default=True,
+    help="Specify whether to check for complete gene records in the phenopackets.",
+)
+@click.option(
+    "--disease-analysis/--no-disease-analysis",
+    default=False,
+    required=False,
+    type=bool,
+    show_default=True,
+    help="Specify whether to check for complete disease records in the phenopackets.",
+)
+@click.option(
+    "--gene-identifier",
+    "-g",
+    required=False,
+    help="Gene identifier to update in phenopacket",
+    type=click.Choice(["ensembl_id", "entrez_id", "hgnc_id"]),
+)
+@click.option(
+    "--hg19-template-vcf",
+    "-hg19",
+    metavar="PATH",
+    required=False,
+    help="Template hg19 VCF file",
+    type=Path,
+)
+@click.option(
+    "--hg38-template-vcf",
+    "-hg38",
+    metavar="PATH",
+    required=False,
+    help="Template hg38 VCF file",
+    type=Path,
+)
+@click.option(
+    "--output-dir",
+    "-o",
+    metavar="PATH",
+    required=True,
+    help="Path to output prepared corpus.",
+    default="prepared_corpus",
+    type=Path,
+)
+def prepare_corpus_command(
+    phenopacket_dir: Path,
+    variant_analysis: bool,
+    gene_analysis: bool,
+    disease_analysis: bool,
+    gene_identifier: str,
+    hg19_template_vcf: Path,
+    hg38_template_vcf: Path,
+    output_dir: Path,
+):
+    """
+    Prepare a corpus of Phenopackets for analysis, optionally checking for complete variant records and updating
+    gene identifiers.
+
+        Args:
+            phenopacket_dir (Path): The path to the directory containing Phenopackets.
+            variant_analysis (bool): If True, check for complete variant records in the Phenopackets.
+            gene_analysis (bool): If True, check for complete gene records in the Phenopackets.
+            disease_analysis (bool): If True, check for complete disease records in the Phenopackets.
+            gene_identifier (str): Identifier for updating gene identifiers, if applicable.
+            hg19_template_vcf (Path): Path to the hg19 template VCF file (optional), to spike variants into
+            VCFs for variant-based analysis at least one of hg19_template_vcf or hg38_template_vcf is required.
+            hg38_template_vcf (Path): Path to the hg38 template VCF file (optional), to spike variants into
+            VCFs for variant-based analysis at least one of hg19_template_vcf or hg38_template_vcf is required.
+            output_dir (Path): The directory to save the prepared Phenopackets and, optionally, VCF files.
+    """
+    prepare_corpus(
+        phenopacket_dir,
+        variant_analysis,
+        gene_analysis,
+        disease_analysis,
+        gene_identifier,
+        hg19_template_vcf,
+        hg38_template_vcf,
+        output_dir,
+    )
```

### Comparing `pheval-0.3.3/src/pheval/config_parser.py` & `pheval-0.3.4/src/pheval/config_parser.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.3/src/pheval/implementations/__init__.py` & `pheval-0.3.4/src/pheval/implementations/__init__.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.3/src/pheval/infra/exomiserdb.py` & `pheval-0.3.4/src/pheval/infra/exomiserdb.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.3/src/pheval/post_processing/post_processing.py` & `pheval-0.3.4/src/pheval/post_processing/post_processing.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.3/src/pheval/prepare/create_noisy_phenopackets.py` & `pheval-0.3.4/src/pheval/prepare/create_noisy_phenopackets.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.3/src/pheval/prepare/create_spiked_vcf.py` & `pheval-0.3.4/src/pheval/prepare/create_spiked_vcf.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.3/src/pheval/prepare/custom_exceptions.py` & `pheval-0.3.4/src/pheval/prepare/custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.3/src/pheval/prepare/update_phenopacket.py` & `pheval-0.3.4/src/pheval/prepare/update_phenopacket.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,16 +34,15 @@
         to update to the current gene identifier in the Phenopacket. We recommend using the ENSEMBL namespace
         to describe the gene identifiers.
     """
     phenopacket = phenopacket_reader(phenopacket_path)
     interpretations = PhenopacketUtil(phenopacket).interpretations()
     updated_interpretations = GeneIdentifierUpdater(
         hgnc_data=hgnc_data, gene_identifier=gene_identifier
-    ).update_genomic_interpretations_gene_identifier(interpretations)
-
+    ).update_genomic_interpretations_gene_identifier(interpretations, phenopacket_path)
     return PhenopacketRebuilder(phenopacket).update_interpretations(updated_interpretations)
 
 
 def create_updated_phenopacket(
     gene_identifier: str, phenopacket_path: Path, output_dir: Path
 ) -> None:
     """
```

### Comparing `pheval-0.3.3/src/pheval/resources/alternate_ouputs/CADA_results.txt` & `pheval-0.3.4/src/pheval/resources/alternate_ouputs/CADA_results.txt`

 * *Files identical despite different names*

### Comparing `pheval-0.3.3/src/pheval/resources/alternate_ouputs/DeepPVP_results.txt` & `pheval-0.3.4/src/pheval/resources/alternate_ouputs/DeepPVP_results.txt`

 * *Files identical despite different names*

### Comparing `pheval-0.3.3/src/pheval/resources/alternate_ouputs/OVA_results.txt` & `pheval-0.3.4/src/pheval/resources/alternate_ouputs/OVA_results.txt`

 * *Files identical despite different names*

### Comparing `pheval-0.3.3/src/pheval/resources/alternate_ouputs/Phen2Gene_results.json` & `pheval-0.3.4/src/pheval/resources/alternate_ouputs/Phen2Gene_results.json`

 * *Files identical despite different names*

### Comparing `pheval-0.3.3/src/pheval/resources/alternate_ouputs/Phenolyzer_results.txt` & `pheval-0.3.4/src/pheval/resources/alternate_ouputs/Phenolyzer_results.txt`

 * *Files identical despite different names*

### Comparing `pheval-0.3.3/src/pheval/resources/alternate_ouputs/lirical_results.tsv` & `pheval-0.3.4/src/pheval/resources/alternate_ouputs/lirical_results.tsv`

 * *Files identical despite different names*

### Comparing `pheval-0.3.3/src/pheval/resources/alternate_ouputs/svanna_results.tsv` & `pheval-0.3.4/src/pheval/resources/alternate_ouputs/svanna_results.tsv`

 * *Files identical despite different names*

### Comparing `pheval-0.3.3/src/pheval/resources/hgnc_complete_set.txt` & `pheval-0.3.4/src/pheval/resources/hgnc_complete_set.txt`

 * *Files identical despite different names*

### Comparing `pheval-0.3.3/src/pheval/run_metadata.py` & `pheval-0.3.4/src/pheval/run_metadata.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.3/src/pheval/runners/runner.py` & `pheval-0.3.4/src/pheval/runners/runner.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.3/src/pheval/utils/docs_gen.py` & `pheval-0.3.4/src/pheval/utils/docs_gen.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.3/src/pheval/utils/exomiser.py` & `pheval-0.3.4/src/pheval/utils/exomiser.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.3/src/pheval/utils/file_utils.py` & `pheval-0.3.4/src/pheval/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.3/src/pheval/utils/phenopacket_utils.py` & `pheval-0.3.4/src/pheval/utils/phenopacket_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import json
-
-# import logging
+import logging
 import os
 from collections import defaultdict
 from copy import copy
 from dataclasses import dataclass
 from pathlib import Path
 from typing import List, Union
 
@@ -18,14 +17,16 @@
     Interpretation,
     Phenopacket,
     PhenotypicFeature,
 )
 
 from pheval.prepare.custom_exceptions import IncorrectFileFormatError
 
+info_log = logging.getLogger("info")
+
 
 class IncompatibleGenomeAssemblyError(Exception):
     """Exception raised for incompatible genome assembly."""
 
     def __init__(self, assembly, phenopacket, message="Incompatible Genome Assembly"):
         """
         Initialise IncompatibleGenomeAssemblyError.
@@ -473,14 +474,67 @@
                     pos=g.variant_interpretation.variation_descriptor.vcf_record.pos,
                     ref=g.variant_interpretation.variation_descriptor.vcf_record.ref,
                     alt=g.variant_interpretation.variation_descriptor.vcf_record.alt,
                 )
                 variants.append(variant)
         return variants
 
+    def check_incomplete_variant_record(self) -> bool:
+        """
+        Check if any variant record in the phenopacket has incomplete information.
+
+        This method iterates through the diagnosed variant records and checks if any of them
+        have missing or incomplete information such as empty chromosome, position, reference,
+        or alternate allele.
+
+        Returns:
+            bool: True if any variant record is incomplete, False otherwise.
+        """
+        variants = self.diagnosed_variants()
+        for variant in variants:
+            if (
+                variant.chrom == ""
+                or variant.pos == 0
+                or variant.pos == ""
+                or variant.ref == ""
+                or variant.alt == ""
+            ):
+                return True
+        return False
+
+    def check_incomplete_gene_record(self) -> bool:
+        """
+        Check if any gene record in the phenopacket has incomplete information.
+
+        This method iterates through the diagnosed gene records and checks if any of them
+        have missing or incomplete information such as gene name, or gene identifier.
+
+        Returns:
+            bool: True if any gene record is incomplete, False otherwise.
+        """
+        genes = self.diagnosed_genes()
+        for gene in genes:
+            if gene.gene_symbol == "" or gene.gene_identifier == "":
+                return True
+        return False
+
+    def check_incomplete_disease_record(self) -> bool:
+        """
+        Check if any disease record in the phenopacket has incomplete information.
+
+        This method iterates through the diagnosed disease records and checks if any of them
+        have missing or incomplete information such as empty disease name, or disease identifier.
+
+        Returns:
+            bool: True if any disease record is incomplete, False otherwise.
+        """
+        if len(self.diagnoses()) == 0:
+            return True
+        return False
+
 
 class PhenopacketRebuilder:
     """Class for rebuilding a Phenopacket"""
 
     def __init__(self, phenopacket: Union[Phenopacket, Family]):
         """Initialise PhenopacketUtil
 
@@ -651,32 +705,38 @@
                             data["hgnc_id"],
                             "ncbigene:" + data["entrez_id"],
                             "ensembl:" + data["ensembl_id"],
                             "symbol:" + symbol,
                         ]
 
     def update_genomic_interpretations_gene_identifier(
-        self, interpretations: List[Interpretation]
+        self, interpretations: List[Interpretation], phenopacket_path: Path
     ) -> List[Interpretation]:
         """
         Update the genomic interpretations of a Phenopacket.
 
         Args:
             interpretations (List[Interpretation]): List of Interpretation objects.
 
         Returns:
             List[Interpretation]: Updated list of Interpretation objects.
         """
         updated_interpretations = copy(list(interpretations))
         for updated_interpretation in updated_interpretations:
             for g in updated_interpretation.diagnosis.genomic_interpretations:
+                updated_gene_identifier = self.find_identifier(
+                    g.variant_interpretation.variation_descriptor.gene_context.symbol
+                )
+                info_log.info(
+                    f"Updating gene identifier in {phenopacket_path} from "
+                    f"{g.variant_interpretation.variation_descriptor.gene_context.value_id}"
+                    f"to {updated_gene_identifier}"
+                )
                 g.variant_interpretation.variation_descriptor.gene_context.value_id = (
-                    self.find_identifier(
-                        g.variant_interpretation.variation_descriptor.gene_context.symbol
-                    )
+                    updated_gene_identifier
                 )
                 del g.variant_interpretation.variation_descriptor.gene_context.alternate_ids[:]
                 g.variant_interpretation.variation_descriptor.gene_context.alternate_ids.extend(
                     self._find_alternate_ids(
                         g.variant_interpretation.variation_descriptor.gene_context.symbol
                     )
                 )
```

### Comparing `pheval-0.3.3/src/pheval/utils/semsim_utils.py` & `pheval-0.3.4/src/pheval/utils/semsim_utils.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.3/src/pheval/utils/utils.py` & `pheval-0.3.4/src/pheval/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.3/PKG-INFO` & `pheval-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheval
-Version: 0.3.3
+Version: 0.3.4
 Summary: 
 Author: Yasemin Bridges
 Author-email: y.bridges@qmul.ac.uk
 Requires-Python: >=3.9,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

