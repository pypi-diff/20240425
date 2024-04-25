# Comparing `tmp/magenpy-0.1.1.tar.gz` & `tmp/magenpy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magenpy-0.1.1.tar", last modified: Fri Apr 12 15:50:55 2024, max compression
+gzip compressed data, was "magenpy-0.1.2.tar", last modified: Thu Apr 25 18:52:52 2024, max compression
```

## Comparing `magenpy-0.1.1.tar` & `magenpy-0.1.2.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:50:55.109618 magenpy-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     7898 2024-04-12 15:50:46.000000 magenpy-0.1.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-12 15:50:46.000000 magenpy-0.1.1/CITATION.md
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-12 15:50:46.000000 magenpy-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-12 15:50:46.000000 magenpy-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-04-12 15:50:55.109618 magenpy-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-12 15:50:46.000000 magenpy-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:50:55.093618 magenpy-0.1.1/bin/
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-12 15:50:46.000000 magenpy-0.1.1/bin/magenpy_ld
--rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-04-12 15:50:46.000000 magenpy-0.1.1/bin/magenpy_simulate
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:50:55.097618 magenpy-0.1.1/magenpy/
--rw-r--r--   0 runner    (1001) docker     (127)    12137 2024-04-12 15:50:46.000000 magenpy-0.1.1/magenpy/AnnotationMatrix.py
--rw-r--r--   0 runner    (1001) docker     (127)    44598 2024-04-12 15:50:46.000000 magenpy-0.1.1/magenpy/GWADataLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)    35031 2024-04-12 15:50:46.000000 magenpy-0.1.1/magenpy/GenotypeMatrix.py
--rw-r--r--   0 runner    (1001) docker     (127)    54443 2024-04-12 15:50:46.000000 magenpy-0.1.1/magenpy/LDMatrix.py
--rw-r--r--   0 runner    (1001) docker     (127)    13870 2024-04-12 15:50:46.000000 magenpy-0.1.1/magenpy/SampleTable.py
--rw-r--r--   0 runner    (1001) docker     (127)    25669 2024-04-12 15:50:46.000000 magenpy-0.1.1/magenpy/SumstatsTable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-12 15:50:46.000000 magenpy-0.1.1/magenpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:50:55.097618 magenpy-0.1.1/magenpy/config/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-12 15:50:46.000000 magenpy-0.1.1/magenpy/config/paths.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:50:55.101618 magenpy-0.1.1/magenpy/data/
--rw-r--r--   0 runner    (1001) docker     (127)  1514113 2024-04-12 15:50:46.000000 magenpy-0.1.1/magenpy/data/1000G_eur_chr22.bed
--rw-r--r--   0 runner    (1001) docker     (127)   569420 2024-04-12 15:50:46.000000 magenpy-0.1.1/magenpy/data/1000G_eur_chr22.bim
--rw-r--r--   0 runner    (1001) docker     (127)     9450 2024-04-12 15:50:46.000000 magenpy-0.1.1/magenpy/data/1000G_eur_chr22.fam
--rw-r--r--   0 runner    (1001) docker     (127)   435206 2024-04-12 15:50:46.000000 magenpy-0.1.1/magenpy/data/ukb_height_chr22.fastGWA.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:50:55.101618 magenpy-0.1.1/magenpy/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 15:50:46.000000 magenpy-0.1.1/magenpy/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-12 15:50:46.000000 magenpy-0.1.1/magenpy/parsers/annotation_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-04-12 15:50:46.000000 magenpy-0.1.1/magenpy/parsers/misc_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-04-12 15:50:46.000000 magenpy-0.1.1/magenpy/parsers/plink_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)    15145 2024-04-12 15:50:46.000000 magenpy-0.1.1/magenpy/parsers/sumstats_parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:50:55.101618 magenpy-0.1.1/magenpy/plot/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 15:50:46.000000 magenpy-0.1.1/magenpy/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-04-12 15:50:46.000000 magenpy-0.1.1/magenpy/plot/gwa.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-12 15:50:46.000000 magenpy-0.1.1/magenpy/plot/ld.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:50:55.101618 magenpy-0.1.1/magenpy/simulation/
--rw-r--r--   0 runner    (1001) docker     (127)     4521 2024-04-12 15:50:46.000000 magenpy-0.1.1/magenpy/simulation/AnnotatedPhenotypeSimulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-04-12 15:50:46.000000 magenpy-0.1.1/magenpy/simulation/MultiCohortPhenotypeSimulator.py
--rw-r--r--   0 runner    (1001) docker     (127)    15558 2024-04-12 15:50:46.000000 magenpy-0.1.1/magenpy/simulation/PhenotypeSimulator.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 15:50:46.000000 magenpy-0.1.1/magenpy/simulation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:50:55.101618 magenpy-0.1.1/magenpy/stats/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 15:50:46.000000 magenpy-0.1.1/magenpy/stats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:50:55.101618 magenpy-0.1.1/magenpy/stats/gwa/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 15:50:46.000000 magenpy-0.1.1/magenpy/stats/gwa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13874 2024-04-12 15:50:46.000000 magenpy-0.1.1/magenpy/stats/gwa/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:50:55.105618 magenpy-0.1.1/magenpy/stats/h2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 15:50:46.000000 magenpy-0.1.1/magenpy/stats/h2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-12 15:50:46.000000 magenpy-0.1.1/magenpy/stats/h2/ldsc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:50:55.105618 magenpy-0.1.1/magenpy/stats/ld/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 15:50:46.000000 magenpy-0.1.1/magenpy/stats/ld/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8174 2024-04-12 15:50:46.000000 magenpy-0.1.1/magenpy/stats/ld/c_utils.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    22432 2024-04-12 15:50:46.000000 magenpy-0.1.1/magenpy/stats/ld/estimator.py
--rw-r--r--   0 runner    (1001) docker     (127)    18884 2024-04-12 15:50:46.000000 magenpy-0.1.1/magenpy/stats/ld/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:50:55.105618 magenpy-0.1.1/magenpy/stats/score/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 15:50:46.000000 magenpy-0.1.1/magenpy/stats/score/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-04-12 15:50:46.000000 magenpy-0.1.1/magenpy/stats/score/score.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-12 15:50:46.000000 magenpy-0.1.1/magenpy/stats/score/score_cpp.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-12 15:50:46.000000 magenpy-0.1.1/magenpy/stats/score/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:50:55.105618 magenpy-0.1.1/magenpy/stats/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 15:50:46.000000 magenpy-0.1.1/magenpy/stats/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 15:50:46.000000 magenpy-0.1.1/magenpy/stats/transforms/genotype.py
--rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-04-12 15:50:46.000000 magenpy-0.1.1/magenpy/stats/transforms/phenotype.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:50:55.105618 magenpy-0.1.1/magenpy/stats/variant/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 15:50:46.000000 magenpy-0.1.1/magenpy/stats/variant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-04-12 15:50:46.000000 magenpy-0.1.1/magenpy/stats/variant/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:50:55.105618 magenpy-0.1.1/magenpy/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 15:50:46.000000 magenpy-0.1.1/magenpy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-12 15:50:46.000000 magenpy-0.1.1/magenpy/utils/compute_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-12 15:50:46.000000 magenpy-0.1.1/magenpy/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-12 15:50:46.000000 magenpy-0.1.1/magenpy/utils/executors.py
--rw-r--r--   0 runner    (1001) docker     (127)    17719 2024-04-12 15:50:46.000000 magenpy-0.1.1/magenpy/utils/model_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-12 15:50:46.000000 magenpy-0.1.1/magenpy/utils/system_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:50:55.105618 magenpy-0.1.1/magenpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-04-12 15:50:55.000000 magenpy-0.1.1/magenpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-12 15:50:55.000000 magenpy-0.1.1/magenpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 15:50:55.000000 magenpy-0.1.1/magenpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 15:50:54.000000 magenpy-0.1.1/magenpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-12 15:50:55.000000 magenpy-0.1.1/magenpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-12 15:50:55.000000 magenpy-0.1.1/magenpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-12 15:50:46.000000 magenpy-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-12 15:50:46.000000 magenpy-0.1.1/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-12 15:50:46.000000 magenpy-0.1.1/requirements-optional.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 15:50:46.000000 magenpy-0.1.1/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-12 15:50:46.000000 magenpy-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 15:50:55.109618 magenpy-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-12 15:50:46.000000 magenpy-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:50:55.105618 magenpy-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-12 15:50:46.000000 magenpy-0.1.1/tests/test_gdl.py
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-12 15:50:46.000000 magenpy-0.1.1/tests/test_ld.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-12 15:50:46.000000 magenpy-0.1.1/tests/test_simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:52.805313 magenpy-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     8300 2024-04-25 18:52:40.000000 magenpy-0.1.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-25 18:52:40.000000 magenpy-0.1.2/CITATION.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-25 18:52:40.000000 magenpy-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-25 18:52:40.000000 magenpy-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-04-25 18:52:52.805313 magenpy-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-25 18:52:40.000000 magenpy-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:52.793313 magenpy-0.1.2/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-25 18:52:40.000000 magenpy-0.1.2/bin/magenpy_ld
+-rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-04-25 18:52:40.000000 magenpy-0.1.2/bin/magenpy_simulate
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:52.793313 magenpy-0.1.2/magenpy/
+-rw-r--r--   0 runner    (1001) docker     (127)    12137 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/AnnotationMatrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44598 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/GWADataLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35031 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/GenotypeMatrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55339 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/LDMatrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13870 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/SampleTable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25688 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/SumstatsTable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:52.793313 magenpy-0.1.2/magenpy/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/config/paths.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:52.797313 magenpy-0.1.2/magenpy/data/
+-rw-r--r--   0 runner    (1001) docker     (127)  1514113 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/data/1000G_eur_chr22.bed
+-rw-r--r--   0 runner    (1001) docker     (127)   569420 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/data/1000G_eur_chr22.bim
+-rw-r--r--   0 runner    (1001) docker     (127)     9450 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/data/1000G_eur_chr22.fam
+-rw-r--r--   0 runner    (1001) docker     (127)   435206 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/data/ukb_height_chr22.fastGWA.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:52.801313 magenpy-0.1.2/magenpy/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/parsers/annotation_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/parsers/misc_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/parsers/plink_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15145 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/parsers/sumstats_parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:52.801313 magenpy-0.1.2/magenpy/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8831 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/plot/gwa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/plot/ld.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:52.801313 magenpy-0.1.2/magenpy/simulation/
+-rw-r--r--   0 runner    (1001) docker     (127)     4521 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/simulation/AnnotatedPhenotypeSimulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/simulation/MultiCohortPhenotypeSimulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15558 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/simulation/PhenotypeSimulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/simulation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:52.801313 magenpy-0.1.2/magenpy/stats/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/stats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:52.801313 magenpy-0.1.2/magenpy/stats/gwa/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/stats/gwa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13874 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/stats/gwa/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:52.801313 magenpy-0.1.2/magenpy/stats/h2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/stats/h2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/stats/h2/ldsc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:52.801313 magenpy-0.1.2/magenpy/stats/ld/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/stats/ld/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8174 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/stats/ld/c_utils.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    22432 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/stats/ld/estimator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18884 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/stats/ld/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:52.805313 magenpy-0.1.2/magenpy/stats/score/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/stats/score/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/stats/score/score.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/stats/score/score_cpp.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/stats/score/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:52.805313 magenpy-0.1.2/magenpy/stats/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/stats/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/stats/transforms/genotype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/stats/transforms/phenotype.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:52.805313 magenpy-0.1.2/magenpy/stats/variant/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/stats/variant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/stats/variant/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:52.805313 magenpy-0.1.2/magenpy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/utils/compute_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/utils/executors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17719 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/utils/model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-25 18:52:40.000000 magenpy-0.1.2/magenpy/utils/system_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:52.805313 magenpy-0.1.2/magenpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-04-25 18:52:52.000000 magenpy-0.1.2/magenpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-25 18:52:52.000000 magenpy-0.1.2/magenpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 18:52:52.000000 magenpy-0.1.2/magenpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 18:52:52.000000 magenpy-0.1.2/magenpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-25 18:52:52.000000 magenpy-0.1.2/magenpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-25 18:52:52.000000 magenpy-0.1.2/magenpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-25 18:52:40.000000 magenpy-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-25 18:52:40.000000 magenpy-0.1.2/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-25 18:52:40.000000 magenpy-0.1.2/requirements-optional.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 18:52:40.000000 magenpy-0.1.2/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-25 18:52:40.000000 magenpy-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 18:52:52.805313 magenpy-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-25 18:52:40.000000 magenpy-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:52.805313 magenpy-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-25 18:52:40.000000 magenpy-0.1.2/tests/test_gdl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-25 18:52:40.000000 magenpy-0.1.2/tests/test_ld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-25 18:52:40.000000 magenpy-0.1.2/tests/test_simulation.py
```

### Comparing `magenpy-0.1.1/CHANGELOG.md` & `magenpy-0.1.2/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,28 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.1.2] - 2024-04-24
+
+### Changed
+
+- Fixed `manhattan` plot implementation to support various new features.
+- Added a warning when accessing `csr_matrix` property of `LDMatrix` when it hasn't been loaded
+previously.
+
+### Added
+
+- `reset_mask` method for magenpy `LDMatrix`.
+- `Dockerfile`s for both `cli` and `jupyter` modes.
+- A helper script to convert LD matrices from old format to new format.
+
 ## [0.1.1] - 2024-04-12
 
 ### Changed
 
 - Fixed bugs in how covariates are processed in `SampleTable`.
 - Fixed bugs / issues in implementation of GWAS with `xarray` backend.
 - Streamlined implementation of `manhattan` plotting function.
```

### Comparing `magenpy-0.1.1/CITATION.md` & `magenpy-0.1.2/CITATION.md`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.1/LICENSE` & `magenpy-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.1/PKG-INFO` & `magenpy-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magenpy
-Version: 0.1.1
+Version: 0.1.2
 Summary: Modeling and Analysis of Statistical Genetics data in python
 Home-page: https://github.com/shz9/magenpy
 Author: Shadi Zabad
 Author-email: shadi.zabad@mail.mcgill.ca
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `magenpy-0.1.1/README.md` & `magenpy-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.1/bin/magenpy_ld` & `magenpy-0.1.2/bin/magenpy_ld`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.1/bin/magenpy_simulate` & `magenpy-0.1.2/bin/magenpy_simulate`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.1/magenpy/AnnotationMatrix.py` & `magenpy-0.1.2/magenpy/AnnotationMatrix.py`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.1/magenpy/GWADataLoader.py` & `magenpy-0.1.2/magenpy/GWADataLoader.py`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.1/magenpy/GenotypeMatrix.py` & `magenpy-0.1.2/magenpy/GenotypeMatrix.py`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.1/magenpy/LDMatrix.py` & `magenpy-0.1.2/magenpy/LDMatrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import zarr
 import os.path as osp
 import numpy as np
 import pandas as pd
+import warnings
 from scipy.sparse import csr_matrix, identity, triu, diags
 from .utils.model_utils import quantize, dequantize
 
 
 class LDMatrix(object):
     """
     A class that represents Linkage-Disequilibrium (LD) matrices, which record
@@ -708,35 +709,40 @@
 
         """
         return np.diff(self.indptr)
 
     @property
     def n_neighbors(self):
         """
-        The number of variants in the LD window for each SNP.
-
         !!! seealso "See Also"
             * [window_size][magenpy.LDMatrix.LDMatrix.window_size]
 
         !!! note
             This includes the variant itself if the matrix is in memory and is symmetric.
 
+        :return: The number of variants in the LD window for each SNP.
+
         """
         return self.window_size()
 
     @property
     def csr_matrix(self):
         """
-        :return: The in-memory CSR matrix object.
-
         ..note ::
             If the LD matrix is not in-memory, then it'll be loaded using default settings.
+            This means that the matrix will be loaded as upper-triangular matrix with
+            default data type. To customize the loading, call the `.load(...)` method before
+            accessing the CSR matrix in this way.
 
+        :return: The in-memory CSR matrix object.
         """
         if self._mat is None:
+            warnings.warn("> Warning: Loading LD matrix with default settings. "
+                          "To customize, call the `.load(...)` method before invoking `.csr_matrix`.",
+                          stacklevel=2)
             self.load()
         return self._mat
 
     @property
     def data(self):
         """
         :return: The `data` array of the sparse `CSR` matrix, containing the entries of the LD matrix.
@@ -829,15 +835,28 @@
         else:
             self._mask = mask
 
         # If the data is already in memory, reload:
         if self.in_memory:
             self.load(force_reload=True,
                       return_symmetric=self.is_symmetric,
-                      fill_diag=self.is_symmetric)
+                      fill_diag=self.is_symmetric,
+                      dtype=self.dtype)
+
+    def reset_mask(self):
+        """
+        Reset the mask to its default value (None).
+        """
+        self._mask = None
+
+        if self.in_memory:
+            self.load(force_reload=True,
+                      return_symmetric=self.is_symmetric,
+                      fill_diag=self.is_symmetric,
+                      dtype=self.dtype)
 
     def to_snp_table(self, col_subset=None):
         """
         :param col_subset: The subset of columns to add to the table. If None, it returns
         all available columns.
 
         :return: A `pandas` dataframe of the SNP attributes and metadata for variants
@@ -1405,32 +1424,32 @@
                 raise ValueError(f"Invalid LD Matrix: Dimensions for attribute {attr} are not aligned!")
 
         # TODO: Add other sanity checks here?
 
         return True
 
     def __getstate__(self):
-        return self.store.path, self.in_memory, self.is_symmetric, self._mask
+        return self.store.path, self.in_memory, self.is_symmetric, self._mask, self.dtype
 
     def __setstate__(self, state):
 
-        path, in_mem, is_symmetric, mask = state
+        path, in_mem, is_symmetric, mask, dtype = state
 
         self._zg = zarr.open_group(path, mode='r')
         self.in_memory = in_mem
         self.is_symmetric = is_symmetric
         self._mat = None
         self.index = 0
         self._mask = None
 
         if mask is not None:
             self.set_mask(mask)
 
         if in_mem:
-            self.load(return_symmetric=is_symmetric, fill_diag=is_symmetric)
+            self.load(return_symmetric=is_symmetric, fill_diag=is_symmetric, dtype=dtype)
 
     def __len__(self):
         return self.n_snps
 
     def __getitem__(self, index):
         return self.get_row(index)
```

### Comparing `magenpy-0.1.1/magenpy/SampleTable.py` & `magenpy-0.1.2/magenpy/SampleTable.py`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.1/magenpy/SumstatsTable.py` & `magenpy-0.1.2/magenpy/SumstatsTable.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,15 +306,15 @@
             * [pval][magenpy.SumstatsTable.SumstatsTable.pval]
 
         :return: The p-value from the association test of each variant on the phenotype.
         """
         return self.pval
 
     @property
-    def log10_p_value(self):
+    def negative_log10_p_value(self):
         """
         :return: The negative log10 of the p-value (-log10(p_value)) of association
         test of each variant on the phenotype.
         """
         return -np.log10(self.pval)
 
     @property
@@ -619,15 +619,15 @@
         for col in non_present_cols:
 
             if col == 'Z':
                 table['Z'] = self.z_score
             elif col == 'PVAL':
                 table['PVAL'] = self.p_value
             elif col == 'LOG10_PVAL':
-                table['LOG10_PVAL'] = self.log10_p_value
+                table['NLOG10_PVAL'] = self.negative_log10_p_value
             elif col == 'CHISQ':
                 table['CHISQ'] = self.get_chisq_statistic()
             elif col == 'MAF_VAR':
                 table['MAF_VAR'] = self.maf_var
             elif col == 'STD_BETA':
                 table['STD_BETA'] = self.get_snp_pseudo_corr()
             else:
```

### Comparing `magenpy-0.1.1/magenpy/__init__.py` & `magenpy-0.1.2/magenpy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from .simulation.PhenotypeSimulator import PhenotypeSimulator
 
 # Data utilities:
 
 from .utils.data_utils import *
 
-__version__ = '0.1.1'
+__version__ = '0.1.2'
 __release_date__ = 'April 2024'
 
 
 config = configparser.ConfigParser()
 config.read(glob.glob(osp.join(osp.dirname(__file__), 'config/*.ini')))
```

### Comparing `magenpy-0.1.1/magenpy/data/1000G_eur_chr22.bed` & `magenpy-0.1.2/magenpy/data/1000G_eur_chr22.bed`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.1/magenpy/data/1000G_eur_chr22.bim` & `magenpy-0.1.2/magenpy/data/1000G_eur_chr22.bim`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.1/magenpy/data/1000G_eur_chr22.fam` & `magenpy-0.1.2/magenpy/data/1000G_eur_chr22.fam`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.1/magenpy/data/ukb_height_chr22.fastGWA.gz` & `magenpy-0.1.2/magenpy/data/ukb_height_chr22.fastGWA.gz`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.1/magenpy/parsers/annotation_parsers.py` & `magenpy-0.1.2/magenpy/parsers/annotation_parsers.py`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.1/magenpy/parsers/misc_parsers.py` & `magenpy-0.1.2/magenpy/parsers/misc_parsers.py`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.1/magenpy/parsers/plink_parsers.py` & `magenpy-0.1.2/magenpy/parsers/plink_parsers.py`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.1/magenpy/parsers/sumstats_parsers.py` & `magenpy-0.1.2/magenpy/parsers/sumstats_parsers.py`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.1/magenpy/plot/gwa.py` & `magenpy-0.1.2/magenpy/plot/gwa.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,118 +1,167 @@
 from typing import Union
 from ..GWADataLoader import GWADataLoader
 from ..SumstatsTable import SumstatsTable
 import matplotlib.pylab as plt
+import pandas as pd
 import numpy as np
 
 
-def manhattan(input_data: Union[GWADataLoader, SumstatsTable],
-              y=None,
-              y_label=None,
+def manhattan(input_data: Union[GWADataLoader, SumstatsTable, pd.DataFrame],
+              x_col=None,
+              y_col='NLOG10_PVAL',
               scatter_kwargs=None,
-              #highlight_snps=None,
-              #highlight_snps_kwargs=None,
+              highlight_snps=None,
+              highlight_snps_kwargs=None,
               chrom_sep_color='#f0f0f0',
               add_bonf_line=True,
               bonf_line_kwargs=None):
 
     """
     Generate Manhattan plot where the x-axis is the genomic position (in BP)
     and the y-axis is the -log10(p-value) or some other statistic of the user's choice.
 
-    TODO: Add functionality to highlight certain SNPs or markers on the plot.
-    TODO: Allow the user to plot other statistics on the y-axis.
-
-    :param input_data: An instance of `SumstatsTable` or `GWADataLoader` from which data about the
-    positions of the SNPs will be extracted.
-    :param y: An optional vector of values to plot on the y-axis. If not provided, the -log10(p-value)
-    will be plotted by default.
-    :param y_label: A label for the quantity or statistic that will be plotted on the y-axis.
-    :param chrom_sep_color: The color for the chromosome separator block.
+    :param input_data: An instance of `SumstatsTable` / `GWADataLoader` or a `pandas.DataFrame` from
+    which data about the positions of the SNPs and their statistics will be extracted. If `x_col` and `y_col` are
+    not provided, the function will assume that the input data contains columns named 'POS' and 'NLOG10_PVAL',
+    for the position in base pairs and the -log10(p-value) respectively.
+    :param x_col: The column name in the input data that contains the x-axis values. Defaults to None. If the
+    user passes `GWADataLoader` or `SumstatsTable` objects, we attempt to extract the x-axis
+    values from the 'POS' (position in base pairs) column.
+    :param y_col: The column name in the input data that contains the y-axis values (default: 'NLOG10_PVAL').
     :param scatter_kwargs: A dictionary of keyword arguments to pass to the `plt.scatter` function.
     This can be used to customize the appearance of the points on the scatter plot.
+    :param highlight_snps: A list or array of SNP rsIDs to highlight on the scatter plot.
+    :param highlight_snps_kwargs: A dictionary of keyword arguments to pass to the `plt.scatter` function
+    to customize the appearance of the highlighted SNPs.
+    :param chrom_sep_color: The color for the chromosome separator block.
     :param add_bonf_line: If True, add a line indicating the Bonferroni significance threshold.
     :param bonf_line_kwargs: The color of the Bonferroni significance threshold line.
 
     """
 
+    # -------------------------------------------------------
+    # Process the input data:
+
     if isinstance(input_data, SumstatsTable):
-        pos = {c: ss.bp_pos for c, ss in input_data.split_by_chromosome().items()}
+        if x_col is None:
+            x_col = 'POS'
+        input_data = {c: ss.to_table(col_subset=('CHR', 'SNP', x_col, y_col))
+                      for c, ss in input_data.split_by_chromosome().items()}
     elif isinstance(input_data, GWADataLoader):
-        pos = {c: ss.bp_pos for c, ss in input_data.sumstats_table.items()}
+        if x_col is None:
+            x_col = 'POS'
+        input_data = input_data.to_summary_statistics_table(col_subset=('CHR', 'SNP', x_col, y_col),
+                                                            per_chromosome=True)
+    elif isinstance(input_data, pd.DataFrame):
+
+        # Sanity checks:
+        assert 'CHR' in input_data.columns, "The input data must contain a column named 'CHR'."
+
+        # If the x-axis column is not provided, we assume that the user wishes to plot the
+        # variant rank on the x-axis.
+        if x_col is not None:
+            assert x_col in input_data.columns, f"The input data must contain a column named '{x_col}'."
+        else:
+            x_col = 'Variant order'
+            input_data['Variant order'] = np.arange(1, input_data.shape[0] + 1)
+
+        assert y_col in input_data.columns, f"The input data must contain a column named '{y_col}'."
+
+        if highlight_snps is not None:
+            assert 'SNP' in input_data.columns
+
+        input_data = {c: ss for c, ss in input_data.groupby('CHR')}
     else:
-        raise ValueError("The input data must be an instance of `SumstatsTable` or `GWADataLoader`.")
+        raise ValueError("The input data must be an instance of `SumstatsTable`, `GWADataLoader` "
+                         "or a `pandas.DataFrame`.")
+
+    # -------------------------------------------------------
+    # Process the SNPs to be highlighted:
+
+    if highlight_snps is not None:
+        if isinstance(highlight_snps, list):
+            highlight_snps = np.array(highlight_snps)
+
+        highlight_snps = {c: np.in1d(p['SNP'], highlight_snps) for c, p in input_data.items()}
 
     # -------------------------------------------------------
     # Add custom scatter plot arguments (if not provided)
     if scatter_kwargs is None:
         scatter_kwargs = {'marker': '.', 'alpha': 0.3, 'color': '#808080'}
     else:
         # Only update the keys that are not already present in the dictionary:
         scatter_kwargs = {**scatter_kwargs, **{'marker': '.', 'alpha': 0.3, 'color': '#808080'}}
 
+    if highlight_snps is not None:
+        if highlight_snps_kwargs is None:
+            highlight_snps_kwargs = {'marker': 'o', 'color': 'red', 'zorder': 2}
+        else:
+            # Only update the keys that are not already present in the dictionary:
+            highlight_snps_kwargs = {**highlight_snps_kwargs, **{'marker': 'o', 'color': 'red', 'zorder': 2}}
+
     # Add custom Bonferroni line arguments (if not provided)
     if bonf_line_kwargs is None:
         bonf_line_kwargs = {'color': '#b06a7a', 'ls': '--', 'zorder': 1}
     else:
         # Only update the keys that are not already present in the dictionary:
         bonf_line_kwargs = {**bonf_line_kwargs, **{'color': '#b06a7a', 'ls': '--', 'zorder': 1}}
 
     # -------------------------------------------------------
 
-    starting_pos = 0
-    ticks = []
-    chrom_spacing = .1*min([p.max() - p.min() for c, p in pos.items()])
-
-    if y is None:
-        # If the values for the Y-axis are not provided,
-        # we assume that the user wishes to plot a standard Manhattan plot
-        # with -log10(p_value) on the Y-axis.
-
-        if add_bonf_line:
-            # Add Bonferroni significance threshold line:
-            plt.axhline(-np.log10(0.05 / 1e6), bonf_line_kwargs)
+    if y_col == 'NLOG10_PVAL' and add_bonf_line:
+        # Add Bonferroni significance threshold line:
+        plt.axhline(-np.log10(0.05 / 1e6), **bonf_line_kwargs)
 
-        if isinstance(input_data, SumstatsTable):
-            y = {c: ss.log10_p_value for c, ss in input_data.split_by_chromosome().items()}
-        else:
-            y = {c: ss.log10_p_value for c, ss in input_data.sumstats_table.items()}
+    # -------------------------------------------------------
+    # Iterate through chromosomes and generate scatter plots:
 
-        y_label = "$-log_{10}$(p-value)"
+    starting_pos = 0
+    ticks = []
+    chrom_spacing = .1*min([p[x_col].max() - p[x_col].min() for c, p in input_data.items()])
 
-    unique_chr = sorted(list(pos.keys()))
+    unique_chr = sorted(list(input_data.keys()))
 
     for i, c in enumerate(unique_chr):
 
-        min_pos = pos[c].min()
-        max_pos = pos[c].max()
+        min_pos = input_data[c][x_col].min()
+        max_pos = input_data[c][x_col].max()
 
         xmin = min_pos + starting_pos
         xmax = max_pos + starting_pos
+
         if i % 2 == 1:
             plt.axvspan(xmin=xmin, xmax=xmax, zorder=0, color=chrom_sep_color)
 
         ticks.append((xmin + xmax) / 2)
 
-        plt.scatter(pos[c] + starting_pos,
-                    y[c],
-                    scatter_kwargs)
-
-        #if hl_snps is not None:
-        #    plt.scatter((pos + starting_pos)[hl_snps[c]], y[c][hl_snps[c]],
-        #                c=hl_snp_color, alpha=snp_alpha, label=hl_snp_label,
-        #                marker=hl_snp_marker)
+        plt.scatter(input_data[c][x_col] + starting_pos,
+                    input_data[c][y_col],
+                    **scatter_kwargs)
+
+        if highlight_snps is not None:
+            plt.scatter((input_data[c][x_col] + starting_pos)[highlight_snps[c]],
+                        input_data[c][y_col][highlight_snps[c]],
+                        **highlight_snps_kwargs)
 
         starting_pos += max_pos + chrom_spacing
 
     plt.xticks(ticks, unique_chr)
 
-    plt.xlabel("Genomic Position")
-    plt.ylabel(y_label)
+    if x_col == 'POS':
+        x_col = 'Genomic Position (BP)'
+
+    plt.xlabel(x_col)
+
+    if y_col == 'NLOG10_PVAL':
+        y_col = "$-log_{10}$(p-value)"
+    elif y_col == 'PVAL':
+        y_col = "p-value"
 
+    plt.ylabel(y_col)
     plt.tight_layout()
 
 
 def qq_plot(input_data: Union[GWADataLoader, SumstatsTable],
             statistic='p_value'):
     """
     Generate a quantile-quantile (QQ) plot for the GWAS summary statistics.
@@ -125,18 +174,19 @@
     """
 
     import scipy.stats as stats
 
     if statistic == 'p_value':
 
         if isinstance(input_data, SumstatsTable):
-            p_val = input_data.log10_p_value
+            p_val = input_data.negative_log10_p_value
             m = input_data.m
         elif isinstance(input_data, GWADataLoader):
-            p_val = np.concatenate([ss.log10_p_value for ss in input_data.sumstats_table.values()])
+            p_val = np.concatenate([ss.negative_log10_p_value
+                                    for ss in input_data.sumstats_table.values()])
             m = input_data.m
         else:
             raise ValueError("The input data must be an instance of `SumstatsTable` or `GWADataLoader`.")
 
         plt.scatter(-np.log10(np.arange(1, m + 1) / m), np.sort(p_val)[::-1])
 
         line = np.linspace(0., p_val.max() + 0.1*p_val.max())
```

### Comparing `magenpy-0.1.1/magenpy/plot/ld.py` & `magenpy-0.1.2/magenpy/plot/ld.py`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.1/magenpy/simulation/AnnotatedPhenotypeSimulator.py` & `magenpy-0.1.2/magenpy/simulation/AnnotatedPhenotypeSimulator.py`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.1/magenpy/simulation/MultiCohortPhenotypeSimulator.py` & `magenpy-0.1.2/magenpy/simulation/MultiCohortPhenotypeSimulator.py`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.1/magenpy/simulation/PhenotypeSimulator.py` & `magenpy-0.1.2/magenpy/simulation/PhenotypeSimulator.py`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.1/magenpy/stats/gwa/utils.py` & `magenpy-0.1.2/magenpy/stats/gwa/utils.py`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.1/magenpy/stats/h2/ldsc.py` & `magenpy-0.1.2/magenpy/stats/h2/ldsc.py`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.1/magenpy/stats/ld/c_utils.pyx` & `magenpy-0.1.2/magenpy/stats/ld/c_utils.pyx`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.1/magenpy/stats/ld/estimator.py` & `magenpy-0.1.2/magenpy/stats/ld/estimator.py`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.1/magenpy/stats/ld/utils.py` & `magenpy-0.1.2/magenpy/stats/ld/utils.py`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.1/magenpy/stats/score/score.hpp` & `magenpy-0.1.2/magenpy/stats/score/score.hpp`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.1/magenpy/stats/score/score_cpp.pyx` & `magenpy-0.1.2/magenpy/stats/score/score_cpp.pyx`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.1/magenpy/stats/score/utils.py` & `magenpy-0.1.2/magenpy/stats/score/utils.py`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.1/magenpy/stats/transforms/genotype.py` & `magenpy-0.1.2/magenpy/stats/transforms/genotype.py`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.1/magenpy/stats/transforms/phenotype.py` & `magenpy-0.1.2/magenpy/stats/transforms/phenotype.py`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.1/magenpy/stats/variant/utils.py` & `magenpy-0.1.2/magenpy/stats/variant/utils.py`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.1/magenpy/utils/compute_utils.py` & `magenpy-0.1.2/magenpy/utils/compute_utils.py`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.1/magenpy/utils/data_utils.py` & `magenpy-0.1.2/magenpy/utils/data_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import os.path as osp
 
 
 def tgp_eur_data_path():
     """
-    Return the path of the attached 1000G genotype data for
+    :return: The path of the attached 1000G genotype data for
     European samples (N=378) and a subset of chromosome 22 (p=15938)
     """
     return osp.join(osp.dirname(osp.dirname(__file__)), 'data/1000G_eur_chr22')
 
 
 def ukb_height_sumstats_path():
     """
-    Return the path of the attached GWAS summary statistics file
+    :return: The path of the attached GWAS summary statistics file
     for standing height. The file contains summary statistics for
     HapMap3 variants on CHR22 and is a snapshot of the summary statistics
     published on the fastGWA database:
     https://yanglab.westlake.edu.cn/data/fastgwa_data/UKB/50.v1.1.fastGWA.gz
     """
     return osp.join(osp.dirname(osp.dirname(__file__)), 'data/ukb_height_chr22.fastGWA.gz')
```

### Comparing `magenpy-0.1.1/magenpy/utils/executors.py` & `magenpy-0.1.2/magenpy/utils/executors.py`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.1/magenpy/utils/model_utils.py` & `magenpy-0.1.2/magenpy/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.1/magenpy/utils/system_utils.py` & `magenpy-0.1.2/magenpy/utils/system_utils.py`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.1/magenpy.egg-info/PKG-INFO` & `magenpy-0.1.2/magenpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magenpy
-Version: 0.1.1
+Version: 0.1.2
 Summary: Modeling and Analysis of Statistical Genetics data in python
 Home-page: https://github.com/shz9/magenpy
 Author: Shadi Zabad
 Author-email: shadi.zabad@mail.mcgill.ca
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `magenpy-0.1.1/magenpy.egg-info/SOURCES.txt` & `magenpy-0.1.2/magenpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.1/setup.py` & `magenpy-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 with open("requirements-docs.txt") as fp:
     docs_requires = fp.read().strip().split("\n")
 
 # ------------------------------------------------------
 
 setup(
     name="magenpy",
-    version="0.1.1",
+    version="0.1.2",
     author="Shadi Zabad",
     author_email="shadi.zabad@mail.mcgill.ca",
     description="Modeling and Analysis of Statistical Genetics data in python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/shz9/magenpy",
     classifiers=[
```

### Comparing `magenpy-0.1.1/tests/test_gdl.py` & `magenpy-0.1.2/tests/test_gdl.py`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.1/tests/test_ld.py` & `magenpy-0.1.2/tests/test_ld.py`

 * *Files identical despite different names*

### Comparing `magenpy-0.1.1/tests/test_simulation.py` & `magenpy-0.1.2/tests/test_simulation.py`

 * *Files identical despite different names*

