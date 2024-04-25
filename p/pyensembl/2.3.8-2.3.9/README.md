# Comparing `tmp/pyensembl-2.3.8.tar.gz` & `tmp/pyensembl-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyensembl-2.3.8.tar", last modified: Wed Jan 17 05:29:57 2024, max compression
+gzip compressed data, was "pyensembl-2.3.9.tar", last modified: Wed Jan 17 05:35:01 2024, max compression
```

## Comparing `pyensembl-2.3.8.tar` & `pyensembl-2.3.9.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2024-01-17 05:29:57.829570 pyensembl-2.3.8/
--rw-r--r--   0 iskander   (501) staff       (20)    11323 2022-03-10 18:56:17.000000 pyensembl-2.3.8/LICENSE
--rw-r--r--   0 iskander   (501) staff       (20)       34 2022-03-10 18:56:17.000000 pyensembl-2.3.8/MANIFEST.in
--rw-r--r--   0 iskander   (501) staff       (20)     9434 2024-01-17 05:29:57.829276 pyensembl-2.3.8/PKG-INFO
--rw-r--r--   0 iskander   (501) staff       (20)     8469 2024-01-17 05:29:01.000000 pyensembl-2.3.8/README.md
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2024-01-17 05:29:57.822883 pyensembl-2.3.8/pyensembl/
--rw-r--r--   0 iskander   (501) staff       (20)     1809 2024-01-11 19:57:20.000000 pyensembl-2.3.8/pyensembl/__init__.py
--rw-r--r--   0 iskander   (501) staff       (20)     2619 2024-01-11 19:50:40.000000 pyensembl-2.3.8/pyensembl/common.py
--rw-r--r--   0 iskander   (501) staff       (20)    21986 2024-01-16 18:12:31.000000 pyensembl-2.3.8/pyensembl/database.py
--rw-r--r--   0 iskander   (501) staff       (20)    11807 2023-12-28 23:02:50.000000 pyensembl-2.3.8/pyensembl/download_cache.py
--rw-r--r--   0 iskander   (501) staff       (20)     5168 2024-01-11 20:12:17.000000 pyensembl-2.3.8/pyensembl/ensembl_release.py
--rw-r--r--   0 iskander   (501) staff       (20)     5418 2024-01-11 19:56:49.000000 pyensembl-2.3.8/pyensembl/ensembl_url_templates.py
--rw-r--r--   0 iskander   (501) staff       (20)     1053 2024-01-11 19:56:51.000000 pyensembl-2.3.8/pyensembl/ensembl_versions.py
--rw-r--r--   0 iskander   (501) staff       (20)     2144 2023-08-17 17:45:33.000000 pyensembl-2.3.8/pyensembl/exon.py
--rw-r--r--   0 iskander   (501) staff       (20)     5186 2023-08-17 17:45:33.000000 pyensembl-2.3.8/pyensembl/fasta.py
--rw-r--r--   0 iskander   (501) staff       (20)     3271 2023-08-17 17:45:33.000000 pyensembl-2.3.8/pyensembl/gene.py
--rw-r--r--   0 iskander   (501) staff       (20)    40018 2024-01-11 19:25:15.000000 pyensembl-2.3.8/pyensembl/genome.py
--rw-r--r--   0 iskander   (501) staff       (20)     7661 2023-08-17 17:45:33.000000 pyensembl-2.3.8/pyensembl/locus.py
--rw-r--r--   0 iskander   (501) staff       (20)     2021 2023-08-17 17:45:33.000000 pyensembl-2.3.8/pyensembl/locus_with_genome.py
--rw-r--r--   0 iskander   (501) staff       (20)      722 2023-08-17 17:45:10.000000 pyensembl-2.3.8/pyensembl/logging.conf
--rw-r--r--   0 iskander   (501) staff       (20)     1995 2023-08-17 17:45:33.000000 pyensembl-2.3.8/pyensembl/normalization.py
--rw-r--r--   0 iskander   (501) staff       (20)     3026 2023-08-17 17:45:33.000000 pyensembl-2.3.8/pyensembl/reference_name.py
--rw-r--r--   0 iskander   (501) staff       (20)     1174 2023-08-17 17:45:33.000000 pyensembl-2.3.8/pyensembl/search.py
--rw-r--r--   0 iskander   (501) staff       (20)     5319 2023-08-17 17:45:33.000000 pyensembl-2.3.8/pyensembl/sequence_data.py
--rwxr-xr-x   0 iskander   (501) staff       (20)     9337 2023-08-17 17:45:33.000000 pyensembl-2.3.8/pyensembl/shell.py
--rw-r--r--   0 iskander   (501) staff       (20)    10984 2024-01-11 19:54:52.000000 pyensembl-2.3.8/pyensembl/species.py
--rw-r--r--   0 iskander   (501) staff       (20)    16639 2024-01-15 22:36:00.000000 pyensembl-2.3.8/pyensembl/transcript.py
--rw-r--r--   0 iskander   (501) staff       (20)       22 2024-01-17 05:29:19.000000 pyensembl-2.3.8/pyensembl/version.py
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2024-01-17 05:29:57.828933 pyensembl-2.3.8/pyensembl.egg-info/
--rw-r--r--   0 iskander   (501) staff       (20)     9434 2024-01-17 05:29:57.000000 pyensembl-2.3.8/pyensembl.egg-info/PKG-INFO
--rw-r--r--   0 iskander   (501) staff       (20)     1475 2024-01-17 05:29:57.000000 pyensembl-2.3.8/pyensembl.egg-info/SOURCES.txt
--rw-r--r--   0 iskander   (501) staff       (20)        1 2024-01-17 05:29:57.000000 pyensembl-2.3.8/pyensembl.egg-info/dependency_links.txt
--rw-r--r--   0 iskander   (501) staff       (20)       50 2024-01-17 05:29:57.000000 pyensembl-2.3.8/pyensembl.egg-info/entry_points.txt
--rw-r--r--   0 iskander   (501) staff       (20)      170 2024-01-17 05:29:57.000000 pyensembl-2.3.8/pyensembl.egg-info/requires.txt
--rw-r--r--   0 iskander   (501) staff       (20)       10 2024-01-17 05:29:57.000000 pyensembl-2.3.8/pyensembl.egg-info/top_level.txt
--rw-r--r--   0 iskander   (501) staff       (20)      170 2024-01-17 04:42:14.000000 pyensembl-2.3.8/requirements.txt
--rw-r--r--   0 iskander   (501) staff       (20)       38 2024-01-17 05:29:57.829609 pyensembl-2.3.8/setup.cfg
--rw-r--r--   0 iskander   (501) staff       (20)     2544 2024-01-16 19:04:02.000000 pyensembl-2.3.8/setup.py
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2024-01-17 05:29:57.828594 pyensembl-2.3.8/tests/
--rw-r--r--   0 iskander   (501) staff       (20)      282 2024-01-10 22:38:55.000000 pyensembl-2.3.8/tests/test_contigs.py
--rw-r--r--   0 iskander   (501) staff       (20)     1856 2024-01-15 22:20:24.000000 pyensembl-2.3.8/tests/test_download_cache.py
--rw-r--r--   0 iskander   (501) staff       (20)      266 2024-01-10 22:38:55.000000 pyensembl-2.3.8/tests/test_ensembl_gtf.py
--rw-r--r--   0 iskander   (501) staff       (20)      564 2024-01-15 22:20:24.000000 pyensembl-2.3.8/tests/test_ensembl_object_properties.py
--rw-r--r--   0 iskander   (501) staff       (20)     3958 2024-01-10 22:38:55.000000 pyensembl-2.3.8/tests/test_exon_id.py
--rw-r--r--   0 iskander   (501) staff       (20)     3702 2024-01-10 22:38:55.000000 pyensembl-2.3.8/tests/test_exon_object.py
--rw-r--r--   0 iskander   (501) staff       (20)     2257 2024-01-10 22:38:55.000000 pyensembl-2.3.8/tests/test_gene_ids.py
--rw-r--r--   0 iskander   (501) staff       (20)     2120 2024-01-10 22:38:55.000000 pyensembl-2.3.8/tests/test_gene_names.py
--rw-r--r--   0 iskander   (501) staff       (20)     1649 2024-01-15 22:20:24.000000 pyensembl-2.3.8/tests/test_gene_objects.py
--rw-r--r--   0 iskander   (501) staff       (20)      697 2024-01-15 22:20:24.000000 pyensembl-2.3.8/tests/test_id_length.py
--rw-r--r--   0 iskander   (501) staff       (20)     5060 2024-01-15 22:20:24.000000 pyensembl-2.3.8/tests/test_locus.py
--rw-r--r--   0 iskander   (501) staff       (20)     3875 2024-01-10 22:38:55.000000 pyensembl-2.3.8/tests/test_missing_genome_sources.py
--rw-r--r--   0 iskander   (501) staff       (20)     2042 2024-01-10 22:38:55.000000 pyensembl-2.3.8/tests/test_mouse.py
--rw-r--r--   0 iskander   (501) staff       (20)      971 2024-01-10 22:38:55.000000 pyensembl-2.3.8/tests/test_release_versions.py
--rw-r--r--   0 iskander   (501) staff       (20)     1887 2024-01-15 22:20:24.000000 pyensembl-2.3.8/tests/test_search.py
--rw-r--r--   0 iskander   (501) staff       (20)     1951 2024-01-10 22:38:55.000000 pyensembl-2.3.8/tests/test_sequence_data.py
--rw-r--r--   0 iskander   (501) staff       (20)     4032 2024-01-10 22:38:55.000000 pyensembl-2.3.8/tests/test_serialization.py
--rw-r--r--   0 iskander   (501) staff       (20)      407 2024-01-10 22:38:55.000000 pyensembl-2.3.8/tests/test_shell.py
--rw-r--r--   0 iskander   (501) staff       (20)     1975 2024-01-10 22:38:55.000000 pyensembl-2.3.8/tests/test_string_representation.py
--rw-r--r--   0 iskander   (501) staff       (20)     2639 2024-01-10 22:38:55.000000 pyensembl-2.3.8/tests/test_timings.py
--rw-r--r--   0 iskander   (501) staff       (20)     2015 2024-01-15 22:20:24.000000 pyensembl-2.3.8/tests/test_transcript_ids.py
--rw-r--r--   0 iskander   (501) staff       (20)     6710 2024-01-10 22:38:55.000000 pyensembl-2.3.8/tests/test_transcript_objects.py
--rw-r--r--   0 iskander   (501) staff       (20)      624 2024-01-10 22:38:55.000000 pyensembl-2.3.8/tests/test_transcript_sequences.py
--rw-r--r--   0 iskander   (501) staff       (20)     1675 2024-01-10 22:38:55.000000 pyensembl-2.3.8/tests/test_transcript_support_level.py
--rw-r--r--   0 iskander   (501) staff       (20)     3838 2024-01-11 19:37:23.000000 pyensembl-2.3.8/tests/test_ucsc_gtf.py
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2024-01-17 05:35:01.880285 pyensembl-2.3.9/
+-rw-r--r--   0 iskander   (501) staff       (20)    11323 2022-03-10 18:56:17.000000 pyensembl-2.3.9/LICENSE
+-rw-r--r--   0 iskander   (501) staff       (20)       34 2022-03-10 18:56:17.000000 pyensembl-2.3.9/MANIFEST.in
+-rw-r--r--   0 iskander   (501) staff       (20)     9430 2024-01-17 05:35:01.880032 pyensembl-2.3.9/PKG-INFO
+-rw-r--r--   0 iskander   (501) staff       (20)     8465 2024-01-17 05:34:26.000000 pyensembl-2.3.9/README.md
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2024-01-17 05:35:01.874243 pyensembl-2.3.9/pyensembl/
+-rw-r--r--   0 iskander   (501) staff       (20)     1809 2024-01-11 19:57:20.000000 pyensembl-2.3.9/pyensembl/__init__.py
+-rw-r--r--   0 iskander   (501) staff       (20)     2619 2024-01-11 19:50:40.000000 pyensembl-2.3.9/pyensembl/common.py
+-rw-r--r--   0 iskander   (501) staff       (20)    21986 2024-01-16 18:12:31.000000 pyensembl-2.3.9/pyensembl/database.py
+-rw-r--r--   0 iskander   (501) staff       (20)    11807 2023-12-28 23:02:50.000000 pyensembl-2.3.9/pyensembl/download_cache.py
+-rw-r--r--   0 iskander   (501) staff       (20)     5168 2024-01-11 20:12:17.000000 pyensembl-2.3.9/pyensembl/ensembl_release.py
+-rw-r--r--   0 iskander   (501) staff       (20)     5418 2024-01-11 19:56:49.000000 pyensembl-2.3.9/pyensembl/ensembl_url_templates.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1053 2024-01-11 19:56:51.000000 pyensembl-2.3.9/pyensembl/ensembl_versions.py
+-rw-r--r--   0 iskander   (501) staff       (20)     2144 2023-08-17 17:45:33.000000 pyensembl-2.3.9/pyensembl/exon.py
+-rw-r--r--   0 iskander   (501) staff       (20)     5186 2023-08-17 17:45:33.000000 pyensembl-2.3.9/pyensembl/fasta.py
+-rw-r--r--   0 iskander   (501) staff       (20)     3271 2023-08-17 17:45:33.000000 pyensembl-2.3.9/pyensembl/gene.py
+-rw-r--r--   0 iskander   (501) staff       (20)    40018 2024-01-11 19:25:15.000000 pyensembl-2.3.9/pyensembl/genome.py
+-rw-r--r--   0 iskander   (501) staff       (20)     7661 2023-08-17 17:45:33.000000 pyensembl-2.3.9/pyensembl/locus.py
+-rw-r--r--   0 iskander   (501) staff       (20)     2021 2023-08-17 17:45:33.000000 pyensembl-2.3.9/pyensembl/locus_with_genome.py
+-rw-r--r--   0 iskander   (501) staff       (20)      722 2023-08-17 17:45:10.000000 pyensembl-2.3.9/pyensembl/logging.conf
+-rw-r--r--   0 iskander   (501) staff       (20)     1995 2023-08-17 17:45:33.000000 pyensembl-2.3.9/pyensembl/normalization.py
+-rw-r--r--   0 iskander   (501) staff       (20)     3026 2023-08-17 17:45:33.000000 pyensembl-2.3.9/pyensembl/reference_name.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1174 2023-08-17 17:45:33.000000 pyensembl-2.3.9/pyensembl/search.py
+-rw-r--r--   0 iskander   (501) staff       (20)     5319 2023-08-17 17:45:33.000000 pyensembl-2.3.9/pyensembl/sequence_data.py
+-rwxr-xr-x   0 iskander   (501) staff       (20)     9337 2023-08-17 17:45:33.000000 pyensembl-2.3.9/pyensembl/shell.py
+-rw-r--r--   0 iskander   (501) staff       (20)    10984 2024-01-11 19:54:52.000000 pyensembl-2.3.9/pyensembl/species.py
+-rw-r--r--   0 iskander   (501) staff       (20)    16639 2024-01-15 22:36:00.000000 pyensembl-2.3.9/pyensembl/transcript.py
+-rw-r--r--   0 iskander   (501) staff       (20)       22 2024-01-17 05:34:16.000000 pyensembl-2.3.9/pyensembl/version.py
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2024-01-17 05:35:01.879763 pyensembl-2.3.9/pyensembl.egg-info/
+-rw-r--r--   0 iskander   (501) staff       (20)     9430 2024-01-17 05:35:01.000000 pyensembl-2.3.9/pyensembl.egg-info/PKG-INFO
+-rw-r--r--   0 iskander   (501) staff       (20)     1475 2024-01-17 05:35:01.000000 pyensembl-2.3.9/pyensembl.egg-info/SOURCES.txt
+-rw-r--r--   0 iskander   (501) staff       (20)        1 2024-01-17 05:35:01.000000 pyensembl-2.3.9/pyensembl.egg-info/dependency_links.txt
+-rw-r--r--   0 iskander   (501) staff       (20)       50 2024-01-17 05:35:01.000000 pyensembl-2.3.9/pyensembl.egg-info/entry_points.txt
+-rw-r--r--   0 iskander   (501) staff       (20)      170 2024-01-17 05:35:01.000000 pyensembl-2.3.9/pyensembl.egg-info/requires.txt
+-rw-r--r--   0 iskander   (501) staff       (20)       10 2024-01-17 05:35:01.000000 pyensembl-2.3.9/pyensembl.egg-info/top_level.txt
+-rw-r--r--   0 iskander   (501) staff       (20)      170 2024-01-17 04:42:14.000000 pyensembl-2.3.9/requirements.txt
+-rw-r--r--   0 iskander   (501) staff       (20)       38 2024-01-17 05:35:01.880324 pyensembl-2.3.9/setup.cfg
+-rw-r--r--   0 iskander   (501) staff       (20)     2544 2024-01-16 19:04:02.000000 pyensembl-2.3.9/setup.py
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2024-01-17 05:35:01.879455 pyensembl-2.3.9/tests/
+-rw-r--r--   0 iskander   (501) staff       (20)      282 2024-01-10 22:38:55.000000 pyensembl-2.3.9/tests/test_contigs.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1856 2024-01-15 22:20:24.000000 pyensembl-2.3.9/tests/test_download_cache.py
+-rw-r--r--   0 iskander   (501) staff       (20)      266 2024-01-10 22:38:55.000000 pyensembl-2.3.9/tests/test_ensembl_gtf.py
+-rw-r--r--   0 iskander   (501) staff       (20)      564 2024-01-15 22:20:24.000000 pyensembl-2.3.9/tests/test_ensembl_object_properties.py
+-rw-r--r--   0 iskander   (501) staff       (20)     3958 2024-01-10 22:38:55.000000 pyensembl-2.3.9/tests/test_exon_id.py
+-rw-r--r--   0 iskander   (501) staff       (20)     3702 2024-01-10 22:38:55.000000 pyensembl-2.3.9/tests/test_exon_object.py
+-rw-r--r--   0 iskander   (501) staff       (20)     2257 2024-01-10 22:38:55.000000 pyensembl-2.3.9/tests/test_gene_ids.py
+-rw-r--r--   0 iskander   (501) staff       (20)     2120 2024-01-10 22:38:55.000000 pyensembl-2.3.9/tests/test_gene_names.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1649 2024-01-15 22:20:24.000000 pyensembl-2.3.9/tests/test_gene_objects.py
+-rw-r--r--   0 iskander   (501) staff       (20)      697 2024-01-15 22:20:24.000000 pyensembl-2.3.9/tests/test_id_length.py
+-rw-r--r--   0 iskander   (501) staff       (20)     5060 2024-01-15 22:20:24.000000 pyensembl-2.3.9/tests/test_locus.py
+-rw-r--r--   0 iskander   (501) staff       (20)     3875 2024-01-10 22:38:55.000000 pyensembl-2.3.9/tests/test_missing_genome_sources.py
+-rw-r--r--   0 iskander   (501) staff       (20)     2042 2024-01-10 22:38:55.000000 pyensembl-2.3.9/tests/test_mouse.py
+-rw-r--r--   0 iskander   (501) staff       (20)      971 2024-01-10 22:38:55.000000 pyensembl-2.3.9/tests/test_release_versions.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1887 2024-01-15 22:20:24.000000 pyensembl-2.3.9/tests/test_search.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1951 2024-01-10 22:38:55.000000 pyensembl-2.3.9/tests/test_sequence_data.py
+-rw-r--r--   0 iskander   (501) staff       (20)     4032 2024-01-10 22:38:55.000000 pyensembl-2.3.9/tests/test_serialization.py
+-rw-r--r--   0 iskander   (501) staff       (20)      407 2024-01-10 22:38:55.000000 pyensembl-2.3.9/tests/test_shell.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1975 2024-01-10 22:38:55.000000 pyensembl-2.3.9/tests/test_string_representation.py
+-rw-r--r--   0 iskander   (501) staff       (20)     2639 2024-01-10 22:38:55.000000 pyensembl-2.3.9/tests/test_timings.py
+-rw-r--r--   0 iskander   (501) staff       (20)     2015 2024-01-15 22:20:24.000000 pyensembl-2.3.9/tests/test_transcript_ids.py
+-rw-r--r--   0 iskander   (501) staff       (20)     6710 2024-01-10 22:38:55.000000 pyensembl-2.3.9/tests/test_transcript_objects.py
+-rw-r--r--   0 iskander   (501) staff       (20)      624 2024-01-10 22:38:55.000000 pyensembl-2.3.9/tests/test_transcript_sequences.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1675 2024-01-10 22:38:55.000000 pyensembl-2.3.9/tests/test_transcript_support_level.py
+-rw-r--r--   0 iskander   (501) staff       (20)     3838 2024-01-11 19:37:23.000000 pyensembl-2.3.9/tests/test_ucsc_gtf.py
```

### Comparing `pyensembl-2.3.8/LICENSE` & `pyensembl-2.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyensembl-2.3.8/PKG-INFO` & `pyensembl-2.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyensembl
-Version: 2.3.8
+Version: 2.3.9
 Summary: Python interface to Ensembl reference genome metadata
 Home-page: https://github.com/openvax/pyensembl
 Author: Alex Rubinsteyn
 Author-email: alex.rubinsteyn@unc.edu
 License: http://www.apache.org/licenses/LICENSE-2.0.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -20,15 +20,15 @@
 Requires-Dist: memoized-property>=1.0.2
 Requires-Dist: tinytimer<1.0.0,>=0.0.0
 Requires-Dist: gtfparse<3.0.0,>=2.5.0
 Requires-Dist: serializable<1.0.0,>=0.2.1
 Requires-Dist: pylint<3.0.0,>=2.17.2
 
 [![Tests](https://github.com/openvax/pyensembl/actions/workflows/tests.yml/badge.svg)](https://github.com/openvax/pyensembl/actions/workflows/tests.yml)
-[![Coverage Status](https://coveralls.io/repos/github/openvax/pyensembl/badge.svg?branch=master)](https://coveralls.io/github/openvax/pyensembl?branch=master)
+[![Coverage Status](https://coveralls.io/repos/github/openvax/pyensembl/badge.svg?branch=main)](https://coveralls.io/github/openvax/pyensembl?branch=main)
 <a href="https://pypi.python.org/pypi/pyensembl/">
 <img src="https://img.shields.io/pypi/v/pyensembl.svg?maxAge=1000" alt="PyPI" />
 </a>
 
 # PyEnsembl
 
 PyEnsembl is a Python interface to [Ensembl](http://www.ensembl.org) reference genome metadata such as exons and transcripts. PyEnsembl downloads [GTF](https://en.wikipedia.org/wiki/Gene_transfer_format) and [FASTA](https://en.wikipedia.org/wiki/FASTA_format) files from the [Ensembl FTP server](ftp://ftp.ensembl.org) and loads them into a local database. PyEnsembl can also work with custom reference data specified using user-supplied GTF and FASTA files.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyensembl Version: 2.3.8 Summary: Python interface
+Metadata-Version: 2.1 Name: pyensembl Version: 2.3.9 Summary: Python interface
 to Ensembl reference genome metadata Home-page: https://github.com/openvax/
 pyensembl Author: Alex Rubinsteyn Author-email: alex.rubinsteyn@unc.edu
 License: http://www.apache.org/licenses/LICENSE-2.0.html Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: Console Classifier:
 Operating System :: OS Independent Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python Classifier: Topic :: Scientific/
@@ -10,16 +10,16 @@
 File: LICENSE Requires-Dist: typechecks<1.0.0,>=0.0.2 Requires-Dist:
 datacache<2.0.0,>=1.4.0 Requires-Dist: memoized-property>=1.0.2 Requires-Dist:
 tinytimer<1.0.0,>=0.0.0 Requires-Dist: gtfparse<3.0.0,>=2.5.0 Requires-Dist:
 serializable<1.0.0,>=0.2.1 Requires-Dist: pylint<3.0.0,>=2.17.2 [![Tests]
 (https://github.com/openvax/pyensembl/actions/workflows/tests.yml/badge.svg)]
 (https://github.com/openvax/pyensembl/actions/workflows/tests.yml) [![Coverage
 Status](https://coveralls.io/repos/github/openvax/pyensembl/
-badge.svg?branch=master)](https://coveralls.io/github/openvax/
-pyensembl?branch=master) _[_P_y_P_I_]# PyEnsembl PyEnsembl is a Python interface to
+badge.svg?branch=main)](https://coveralls.io/github/openvax/
+pyensembl?branch=main) _[_P_y_P_I_]# PyEnsembl PyEnsembl is a Python interface to
 [Ensembl](http://www.ensembl.org) reference genome metadata such as exons and
 transcripts. PyEnsembl downloads [GTF](https://en.wikipedia.org/wiki/
 Gene_transfer_format) and [FASTA](https://en.wikipedia.org/wiki/FASTA_format)
 files from the [Ensembl FTP server](ftp://ftp.ensembl.org) and loads them into
 a local database. PyEnsembl can also work with custom reference data specified
 using user-supplied GTF and FASTA files. # Example Usage ```python from
 pyensembl import EnsemblRelease # release 77 uses human reference genome GRCh38
```

### Comparing `pyensembl-2.3.8/README.md` & `pyensembl-2.3.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [![Tests](https://github.com/openvax/pyensembl/actions/workflows/tests.yml/badge.svg)](https://github.com/openvax/pyensembl/actions/workflows/tests.yml)
-[![Coverage Status](https://coveralls.io/repos/github/openvax/pyensembl/badge.svg?branch=master)](https://coveralls.io/github/openvax/pyensembl?branch=master)
+[![Coverage Status](https://coveralls.io/repos/github/openvax/pyensembl/badge.svg?branch=main)](https://coveralls.io/github/openvax/pyensembl?branch=main)
 <a href="https://pypi.python.org/pypi/pyensembl/">
 <img src="https://img.shields.io/pypi/v/pyensembl.svg?maxAge=1000" alt="PyPI" />
 </a>
 
 # PyEnsembl
 
 PyEnsembl is a Python interface to [Ensembl](http://www.ensembl.org) reference genome metadata such as exons and transcripts. PyEnsembl downloads [GTF](https://en.wikipedia.org/wiki/Gene_transfer_format) and [FASTA](https://en.wikipedia.org/wiki/FASTA_format) files from the [Ensembl FTP server](ftp://ftp.ensembl.org) and loads them into a local database. PyEnsembl can also work with custom reference data specified using user-supplied GTF and FASTA files.
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 [![Tests](https://github.com/openvax/pyensembl/actions/workflows/tests.yml/
 badge.svg)](https://github.com/openvax/pyensembl/actions/workflows/tests.yml)
 [![Coverage Status](https://coveralls.io/repos/github/openvax/pyensembl/
-badge.svg?branch=master)](https://coveralls.io/github/openvax/
-pyensembl?branch=master) _[_P_y_P_I_]# PyEnsembl PyEnsembl is a Python interface to
+badge.svg?branch=main)](https://coveralls.io/github/openvax/
+pyensembl?branch=main) _[_P_y_P_I_]# PyEnsembl PyEnsembl is a Python interface to
 [Ensembl](http://www.ensembl.org) reference genome metadata such as exons and
 transcripts. PyEnsembl downloads [GTF](https://en.wikipedia.org/wiki/
 Gene_transfer_format) and [FASTA](https://en.wikipedia.org/wiki/FASTA_format)
 files from the [Ensembl FTP server](ftp://ftp.ensembl.org) and loads them into
 a local database. PyEnsembl can also work with custom reference data specified
 using user-supplied GTF and FASTA files. # Example Usage ```python from
 pyensembl import EnsemblRelease # release 77 uses human reference genome GRCh38
```

### Comparing `pyensembl-2.3.8/pyensembl/__init__.py` & `pyensembl-2.3.9/pyensembl/__init__.py`

 * *Files identical despite different names*

### Comparing `pyensembl-2.3.8/pyensembl/common.py` & `pyensembl-2.3.9/pyensembl/common.py`

 * *Files identical despite different names*

### Comparing `pyensembl-2.3.8/pyensembl/database.py` & `pyensembl-2.3.9/pyensembl/database.py`

 * *Files identical despite different names*

### Comparing `pyensembl-2.3.8/pyensembl/download_cache.py` & `pyensembl-2.3.9/pyensembl/download_cache.py`

 * *Files identical despite different names*

### Comparing `pyensembl-2.3.8/pyensembl/ensembl_release.py` & `pyensembl-2.3.9/pyensembl/ensembl_release.py`

 * *Files identical despite different names*

### Comparing `pyensembl-2.3.8/pyensembl/ensembl_url_templates.py` & `pyensembl-2.3.9/pyensembl/ensembl_url_templates.py`

 * *Files identical despite different names*

### Comparing `pyensembl-2.3.8/pyensembl/ensembl_versions.py` & `pyensembl-2.3.9/pyensembl/ensembl_versions.py`

 * *Files identical despite different names*

### Comparing `pyensembl-2.3.8/pyensembl/exon.py` & `pyensembl-2.3.9/pyensembl/exon.py`

 * *Files identical despite different names*

### Comparing `pyensembl-2.3.8/pyensembl/fasta.py` & `pyensembl-2.3.9/pyensembl/fasta.py`

 * *Files identical despite different names*

### Comparing `pyensembl-2.3.8/pyensembl/gene.py` & `pyensembl-2.3.9/pyensembl/gene.py`

 * *Files identical despite different names*

### Comparing `pyensembl-2.3.8/pyensembl/genome.py` & `pyensembl-2.3.9/pyensembl/genome.py`

 * *Files identical despite different names*

### Comparing `pyensembl-2.3.8/pyensembl/locus.py` & `pyensembl-2.3.9/pyensembl/locus.py`

 * *Files identical despite different names*

### Comparing `pyensembl-2.3.8/pyensembl/locus_with_genome.py` & `pyensembl-2.3.9/pyensembl/locus_with_genome.py`

 * *Files identical despite different names*

### Comparing `pyensembl-2.3.8/pyensembl/logging.conf` & `pyensembl-2.3.9/pyensembl/logging.conf`

 * *Files identical despite different names*

### Comparing `pyensembl-2.3.8/pyensembl/normalization.py` & `pyensembl-2.3.9/pyensembl/normalization.py`

 * *Files identical despite different names*

### Comparing `pyensembl-2.3.8/pyensembl/reference_name.py` & `pyensembl-2.3.9/pyensembl/reference_name.py`

 * *Files identical despite different names*

### Comparing `pyensembl-2.3.8/pyensembl/search.py` & `pyensembl-2.3.9/pyensembl/search.py`

 * *Files identical despite different names*

### Comparing `pyensembl-2.3.8/pyensembl/sequence_data.py` & `pyensembl-2.3.9/pyensembl/sequence_data.py`

 * *Files identical despite different names*

### Comparing `pyensembl-2.3.8/pyensembl/shell.py` & `pyensembl-2.3.9/pyensembl/shell.py`

 * *Files identical despite different names*

### Comparing `pyensembl-2.3.8/pyensembl/species.py` & `pyensembl-2.3.9/pyensembl/species.py`

 * *Files identical despite different names*

### Comparing `pyensembl-2.3.8/pyensembl/transcript.py` & `pyensembl-2.3.9/pyensembl/transcript.py`

 * *Files identical despite different names*

### Comparing `pyensembl-2.3.8/pyensembl.egg-info/PKG-INFO` & `pyensembl-2.3.9/pyensembl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyensembl
-Version: 2.3.8
+Version: 2.3.9
 Summary: Python interface to Ensembl reference genome metadata
 Home-page: https://github.com/openvax/pyensembl
 Author: Alex Rubinsteyn
 Author-email: alex.rubinsteyn@unc.edu
 License: http://www.apache.org/licenses/LICENSE-2.0.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -20,15 +20,15 @@
 Requires-Dist: memoized-property>=1.0.2
 Requires-Dist: tinytimer<1.0.0,>=0.0.0
 Requires-Dist: gtfparse<3.0.0,>=2.5.0
 Requires-Dist: serializable<1.0.0,>=0.2.1
 Requires-Dist: pylint<3.0.0,>=2.17.2
 
 [![Tests](https://github.com/openvax/pyensembl/actions/workflows/tests.yml/badge.svg)](https://github.com/openvax/pyensembl/actions/workflows/tests.yml)
-[![Coverage Status](https://coveralls.io/repos/github/openvax/pyensembl/badge.svg?branch=master)](https://coveralls.io/github/openvax/pyensembl?branch=master)
+[![Coverage Status](https://coveralls.io/repos/github/openvax/pyensembl/badge.svg?branch=main)](https://coveralls.io/github/openvax/pyensembl?branch=main)
 <a href="https://pypi.python.org/pypi/pyensembl/">
 <img src="https://img.shields.io/pypi/v/pyensembl.svg?maxAge=1000" alt="PyPI" />
 </a>
 
 # PyEnsembl
 
 PyEnsembl is a Python interface to [Ensembl](http://www.ensembl.org) reference genome metadata such as exons and transcripts. PyEnsembl downloads [GTF](https://en.wikipedia.org/wiki/Gene_transfer_format) and [FASTA](https://en.wikipedia.org/wiki/FASTA_format) files from the [Ensembl FTP server](ftp://ftp.ensembl.org) and loads them into a local database. PyEnsembl can also work with custom reference data specified using user-supplied GTF and FASTA files.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyensembl Version: 2.3.8 Summary: Python interface
+Metadata-Version: 2.1 Name: pyensembl Version: 2.3.9 Summary: Python interface
 to Ensembl reference genome metadata Home-page: https://github.com/openvax/
 pyensembl Author: Alex Rubinsteyn Author-email: alex.rubinsteyn@unc.edu
 License: http://www.apache.org/licenses/LICENSE-2.0.html Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: Console Classifier:
 Operating System :: OS Independent Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python Classifier: Topic :: Scientific/
@@ -10,16 +10,16 @@
 File: LICENSE Requires-Dist: typechecks<1.0.0,>=0.0.2 Requires-Dist:
 datacache<2.0.0,>=1.4.0 Requires-Dist: memoized-property>=1.0.2 Requires-Dist:
 tinytimer<1.0.0,>=0.0.0 Requires-Dist: gtfparse<3.0.0,>=2.5.0 Requires-Dist:
 serializable<1.0.0,>=0.2.1 Requires-Dist: pylint<3.0.0,>=2.17.2 [![Tests]
 (https://github.com/openvax/pyensembl/actions/workflows/tests.yml/badge.svg)]
 (https://github.com/openvax/pyensembl/actions/workflows/tests.yml) [![Coverage
 Status](https://coveralls.io/repos/github/openvax/pyensembl/
-badge.svg?branch=master)](https://coveralls.io/github/openvax/
-pyensembl?branch=master) _[_P_y_P_I_]# PyEnsembl PyEnsembl is a Python interface to
+badge.svg?branch=main)](https://coveralls.io/github/openvax/
+pyensembl?branch=main) _[_P_y_P_I_]# PyEnsembl PyEnsembl is a Python interface to
 [Ensembl](http://www.ensembl.org) reference genome metadata such as exons and
 transcripts. PyEnsembl downloads [GTF](https://en.wikipedia.org/wiki/
 Gene_transfer_format) and [FASTA](https://en.wikipedia.org/wiki/FASTA_format)
 files from the [Ensembl FTP server](ftp://ftp.ensembl.org) and loads them into
 a local database. PyEnsembl can also work with custom reference data specified
 using user-supplied GTF and FASTA files. # Example Usage ```python from
 pyensembl import EnsemblRelease # release 77 uses human reference genome GRCh38
```

### Comparing `pyensembl-2.3.8/pyensembl.egg-info/SOURCES.txt` & `pyensembl-2.3.9/pyensembl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyensembl-2.3.8/setup.py` & `pyensembl-2.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `pyensembl-2.3.8/tests/test_download_cache.py` & `pyensembl-2.3.9/tests/test_download_cache.py`

 * *Files identical despite different names*

### Comparing `pyensembl-2.3.8/tests/test_ensembl_object_properties.py` & `pyensembl-2.3.9/tests/test_ensembl_object_properties.py`

 * *Files identical despite different names*

### Comparing `pyensembl-2.3.8/tests/test_exon_id.py` & `pyensembl-2.3.9/tests/test_exon_id.py`

 * *Files identical despite different names*

### Comparing `pyensembl-2.3.8/tests/test_exon_object.py` & `pyensembl-2.3.9/tests/test_exon_object.py`

 * *Files identical despite different names*

### Comparing `pyensembl-2.3.8/tests/test_gene_ids.py` & `pyensembl-2.3.9/tests/test_gene_ids.py`

 * *Files identical despite different names*

### Comparing `pyensembl-2.3.8/tests/test_gene_names.py` & `pyensembl-2.3.9/tests/test_gene_names.py`

 * *Files identical despite different names*

### Comparing `pyensembl-2.3.8/tests/test_gene_objects.py` & `pyensembl-2.3.9/tests/test_gene_objects.py`

 * *Files identical despite different names*

### Comparing `pyensembl-2.3.8/tests/test_id_length.py` & `pyensembl-2.3.9/tests/test_id_length.py`

 * *Files identical despite different names*

### Comparing `pyensembl-2.3.8/tests/test_locus.py` & `pyensembl-2.3.9/tests/test_locus.py`

 * *Files identical despite different names*

### Comparing `pyensembl-2.3.8/tests/test_missing_genome_sources.py` & `pyensembl-2.3.9/tests/test_missing_genome_sources.py`

 * *Files identical despite different names*

### Comparing `pyensembl-2.3.8/tests/test_mouse.py` & `pyensembl-2.3.9/tests/test_mouse.py`

 * *Files identical despite different names*

### Comparing `pyensembl-2.3.8/tests/test_release_versions.py` & `pyensembl-2.3.9/tests/test_release_versions.py`

 * *Files identical despite different names*

### Comparing `pyensembl-2.3.8/tests/test_search.py` & `pyensembl-2.3.9/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `pyensembl-2.3.8/tests/test_sequence_data.py` & `pyensembl-2.3.9/tests/test_sequence_data.py`

 * *Files identical despite different names*

### Comparing `pyensembl-2.3.8/tests/test_serialization.py` & `pyensembl-2.3.9/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `pyensembl-2.3.8/tests/test_string_representation.py` & `pyensembl-2.3.9/tests/test_string_representation.py`

 * *Files identical despite different names*

### Comparing `pyensembl-2.3.8/tests/test_timings.py` & `pyensembl-2.3.9/tests/test_timings.py`

 * *Files identical despite different names*

### Comparing `pyensembl-2.3.8/tests/test_transcript_ids.py` & `pyensembl-2.3.9/tests/test_transcript_ids.py`

 * *Files identical despite different names*

### Comparing `pyensembl-2.3.8/tests/test_transcript_objects.py` & `pyensembl-2.3.9/tests/test_transcript_objects.py`

 * *Files identical despite different names*

### Comparing `pyensembl-2.3.8/tests/test_transcript_sequences.py` & `pyensembl-2.3.9/tests/test_transcript_sequences.py`

 * *Files identical despite different names*

### Comparing `pyensembl-2.3.8/tests/test_transcript_support_level.py` & `pyensembl-2.3.9/tests/test_transcript_support_level.py`

 * *Files identical despite different names*

### Comparing `pyensembl-2.3.8/tests/test_ucsc_gtf.py` & `pyensembl-2.3.9/tests/test_ucsc_gtf.py`

 * *Files identical despite different names*

