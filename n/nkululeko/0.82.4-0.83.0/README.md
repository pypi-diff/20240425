# Comparing `tmp/nkululeko-0.82.4.tar.gz` & `tmp/nkululeko-0.83.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nkululeko-0.82.4.tar", last modified: Wed Apr 24 17:19:59 2024, max compression
+gzip compressed data, was "nkululeko-0.83.0.tar", last modified: Thu Apr 25 13:09:47 2024, max compression
```

## Comparing `nkululeko-0.82.4.tar` & `nkululeko-0.83.0.tar`

### file list

```diff
@@ -1,227 +1,227 @@
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.533017 nkululeko-0.82.4/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    17222 2024-04-24 17:12:54.000000 nkululeko-0.82.4/CHANGELOG.md
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.82.4/LICENSE
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    35950 2024-04-24 17:19:59.533017 nkululeko-0.82.4/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    17457 2024-04-24 09:02:29.000000 nkululeko-0.82.4/README.md
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.521017 nkululeko-0.82.4/data/
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.521017 nkululeko-0.82.4/data/aesdd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1513 2023-10-04 08:46:04.000000 nkululeko-0.82.4/data/aesdd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.521017 nkululeko-0.82.4/data/androids/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-08-30 12:19:59.000000 nkululeko-0.82.4/data/androids/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.521017 nkululeko-0.82.4/data/androids_orig/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-08-20 18:21:45.000000 nkululeko-0.82.4/data/androids_orig/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.521017 nkululeko-0.82.4/data/androids_test/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-09-19 12:01:52.000000 nkululeko-0.82.4/data/androids_test/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.521017 nkululeko-0.82.4/data/ased/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1566 2023-09-19 09:19:58.000000 nkululeko-0.82.4/data/ased/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.521017 nkululeko-0.82.4/data/asvp-esd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1889 2023-09-06 07:54:15.000000 nkululeko-0.82.4/data/asvp-esd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.521017 nkululeko-0.82.4/data/baved/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1899 2023-09-12 12:11:50.000000 nkululeko-0.82.4/data/baved/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.521017 nkululeko-0.82.4/data/cafe/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1520 2023-09-11 09:21:27.000000 nkululeko-0.82.4/data/cafe/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.521017 nkululeko-0.82.4/data/clac/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1202 2023-10-04 08:46:04.000000 nkululeko-0.82.4/data/clac/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.521017 nkululeko-0.82.4/data/cmu-mosei/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1805 2023-10-20 09:59:16.000000 nkululeko-0.82.4/data/cmu-mosei/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.521017 nkululeko-0.82.4/data/demos/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2058 2023-09-19 09:19:58.000000 nkululeko-0.82.4/data/demos/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.521017 nkululeko-0.82.4/data/ekorpus/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1641 2023-09-12 12:11:50.000000 nkululeko-0.82.4/data/ekorpus/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.521017 nkululeko-0.82.4/data/emns/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2073 2023-09-19 09:19:58.000000 nkululeko-0.82.4/data/emns/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.521017 nkululeko-0.82.4/data/emofilm/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1305 2023-08-23 12:21:27.000000 nkululeko-0.82.4/data/emofilm/convert_to_16k.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1736 2023-08-23 06:49:28.000000 nkululeko-0.82.4/data/emofilm/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.525017 nkululeko-0.82.4/data/emorynlp/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1686 2023-09-20 08:48:00.000000 nkululeko-0.82.4/data/emorynlp/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.525017 nkululeko-0.82.4/data/emov-db/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1777 2023-12-19 12:05:21.000000 nkululeko-0.82.4/data/emov-db/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.525017 nkululeko-0.82.4/data/emovo/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1595 2023-09-19 09:19:58.000000 nkululeko-0.82.4/data/emovo/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.525017 nkululeko-0.82.4/data/emozionalmente/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9348 2023-08-23 06:49:28.000000 nkululeko-0.82.4/data/emozionalmente/create.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.525017 nkululeko-0.82.4/data/enterface/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2429 2023-09-19 09:19:58.000000 nkululeko-0.82.4/data/enterface/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.525017 nkululeko-0.82.4/data/esd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1534 2023-09-11 09:21:27.000000 nkululeko-0.82.4/data/esd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.525017 nkululeko-0.82.4/data/gerparas/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3023 2023-10-06 16:05:03.000000 nkululeko-0.82.4/data/gerparas/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.525017 nkululeko-0.82.4/data/iemocap/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3041 2023-10-04 08:46:04.000000 nkululeko-0.82.4/data/iemocap/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.525017 nkululeko-0.82.4/data/jl/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2022 2023-10-04 08:46:04.000000 nkululeko-0.82.4/data/jl/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.525017 nkululeko-0.82.4/data/jtes/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1727 2023-10-04 08:46:04.000000 nkululeko-0.82.4/data/jtes/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.525017 nkululeko-0.82.4/data/meld/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3694 2023-09-19 09:19:58.000000 nkululeko-0.82.4/data/meld/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.525017 nkululeko-0.82.4/data/mesd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2053 2023-09-19 09:19:58.000000 nkululeko-0.82.4/data/mesd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.525017 nkululeko-0.82.4/data/mess/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1529 2023-09-19 09:19:58.000000 nkululeko-0.82.4/data/mess/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.525017 nkululeko-0.82.4/data/mlendsnd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1714 2023-12-19 12:05:21.000000 nkululeko-0.82.4/data/mlendsnd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.525017 nkululeko-0.82.4/data/msp-improv/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2328 2023-08-23 06:49:28.000000 nkululeko-0.82.4/data/msp-improv/process_database2.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.525017 nkululeko-0.82.4/data/msp-podcast/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3021 2023-08-23 06:49:28.000000 nkululeko-0.82.4/data/msp-podcast/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.525017 nkululeko-0.82.4/data/oreau2/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1557 2023-09-19 09:19:58.000000 nkululeko-0.82.4/data/oreau2/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.525017 nkululeko-0.82.4/data/portuguese/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3892 2023-09-12 12:11:50.000000 nkululeko-0.82.4/data/portuguese/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.525017 nkululeko-0.82.4/data/ravdess/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3612 2024-04-22 09:09:10.000000 nkululeko-0.82.4/data/ravdess/process_database.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3144 2023-10-06 16:05:03.000000 nkululeko-0.82.4/data/ravdess/process_database_speaker.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.525017 nkululeko-0.82.4/data/savee/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1680 2023-09-19 09:19:58.000000 nkululeko-0.82.4/data/savee/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.525017 nkululeko-0.82.4/data/shemo/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1624 2023-09-19 09:19:58.000000 nkululeko-0.82.4/data/shemo/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.525017 nkululeko-0.82.4/data/subesco/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2991 2023-09-19 09:19:58.000000 nkululeko-0.82.4/data/subesco/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.525017 nkululeko-0.82.4/data/tess/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1472 2023-09-11 09:21:27.000000 nkululeko-0.82.4/data/tess/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.525017 nkululeko-0.82.4/data/thorsten-emotional/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1142 2023-09-06 07:54:15.000000 nkululeko-0.82.4/data/thorsten-emotional/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.525017 nkululeko-0.82.4/data/urdu/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1803 2023-09-19 09:19:58.000000 nkululeko-0.82.4/data/urdu/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.525017 nkululeko-0.82.4/data/vivae/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1209 2023-09-12 12:11:50.000000 nkululeko-0.82.4/data/vivae/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.521017 nkululeko-0.82.4/docs/
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.525017 nkululeko-0.82.4/docs/source/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3070 2024-04-22 09:09:10.000000 nkululeko-0.82.4/docs/source/conf.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.521017 nkululeko-0.82.4/meta/
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.525017 nkululeko-0.82.4/meta/demos/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      617 2021-10-28 13:49:53.000000 nkululeko-0.82.4/meta/demos/demo_best_model.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.525017 nkululeko-0.82.4/meta/demos/multiple_exeriments/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      819 2024-04-24 13:07:11.000000 nkululeko-0.82.4/meta/demos/multiple_exeriments/do_experiments.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1252 2022-12-07 09:32:42.000000 nkululeko-0.82.4/meta/demos/my_experiment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1095 2022-12-15 16:06:58.000000 nkululeko-0.82.4/meta/demos/my_experiment_local.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      681 2021-10-28 13:49:53.000000 nkululeko-0.82.4/meta/demos/plot_faster_anim.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.525017 nkululeko-0.82.4/nkululeko/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       63 2023-08-31 11:56:33.000000 nkululeko-0.82.4/nkululeko/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3194 2024-02-29 11:07:44.000000 nkululeko-0.82.4/nkululeko/aug_train.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3051 2024-02-29 11:04:02.000000 nkululeko-0.82.4/nkululeko/augment.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.529017 nkululeko-0.82.4/nkululeko/augmenting/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:16:55.000000 nkululeko-0.82.4/nkululeko/augmenting/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2905 2023-12-29 16:48:37.000000 nkululeko-0.82.4/nkululeko/augmenting/augmenter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2669 2023-12-29 16:49:20.000000 nkululeko-0.82.4/nkululeko/augmenting/randomsplicer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1791 2023-09-07 11:33:33.000000 nkululeko-0.82.4/nkululeko/augmenting/randomsplicing.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3335 2023-12-19 11:16:16.000000 nkululeko-0.82.4/nkululeko/augmenting/resampler.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.529017 nkululeko-0.82.4/nkululeko/autopredict/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:02.000000 nkululeko-0.82.4/nkululeko/autopredict/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1095 2023-12-19 11:16:15.000000 nkululeko-0.82.4/nkululeko/autopredict/ap_age.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1024 2023-12-19 11:16:15.000000 nkululeko-0.82.4/nkululeko/autopredict/ap_arousal.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1039 2023-12-19 11:16:15.000000 nkululeko-0.82.4/nkululeko/autopredict/ap_dominance.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1008 2023-12-19 11:16:15.000000 nkululeko-0.82.4/nkululeko/autopredict/ap_gender.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1104 2023-12-19 11:16:16.000000 nkululeko-0.82.4/nkululeko/autopredict/ap_mos.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1137 2023-12-19 11:16:15.000000 nkululeko-0.82.4/nkululeko/autopredict/ap_pesq.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1185 2023-12-19 11:16:16.000000 nkululeko-0.82.4/nkululeko/autopredict/ap_sdr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1107 2023-12-19 11:16:15.000000 nkululeko-0.82.4/nkululeko/autopredict/ap_snr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1184 2023-12-19 11:16:15.000000 nkululeko-0.82.4/nkululeko/autopredict/ap_stoi.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1024 2023-12-19 11:16:15.000000 nkululeko-0.82.4/nkululeko/autopredict/ap_valence.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5048 2024-04-22 09:09:10.000000 nkululeko-0.82.4/nkululeko/autopredict/estimate_snr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      969 2023-09-07 11:39:39.000000 nkululeko-0.82.4/nkululeko/cacheddataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       39 2024-04-24 17:13:07.000000 nkululeko-0.82.4/nkululeko/constants.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.529017 nkululeko-0.82.4/nkululeko/data/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:06.000000 nkululeko-0.82.4/nkululeko/data/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    27650 2024-04-22 09:10:47.000000 nkululeko-0.82.4/nkululeko/data/dataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3884 2024-04-24 12:41:45.000000 nkululeko-0.82.4/nkululeko/data/dataset_csv.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3264 2024-04-22 09:09:10.000000 nkululeko-0.82.4/nkululeko/demo.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2025 2024-02-29 21:51:15.000000 nkululeko-0.82.4/nkululeko/demo_feats.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4755 2024-04-22 09:09:10.000000 nkululeko-0.82.4/nkululeko/demo_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    29576 2024-04-22 11:37:24.000000 nkululeko-0.82.4/nkululeko/experiment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2310 2024-04-22 09:09:10.000000 nkululeko-0.82.4/nkululeko/explore.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4632 2023-12-19 11:16:14.000000 nkululeko-0.82.4/nkululeko/export.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.529017 nkululeko-0.82.4/nkululeko/feat_extract/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:10.000000 nkululeko-0.82.4/nkululeko/feat_extract/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3113 2024-04-23 09:16:18.000000 nkululeko-0.82.4/nkululeko/feat_extract/feats_agender.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3346 2024-04-16 13:29:59.000000 nkululeko-0.82.4/nkululeko/feat_extract/feats_agender_agender.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11399 2024-01-24 16:15:03.000000 nkululeko-0.82.4/nkululeko/feat_extract/feats_analyser.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3162 2024-04-23 09:16:18.000000 nkululeko-0.82.4/nkululeko/feat_extract/feats_auddim.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3187 2024-04-23 09:16:18.000000 nkululeko-0.82.4/nkululeko/feat_extract/feats_audmodel.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3489 2024-04-23 09:16:18.000000 nkululeko-0.82.4/nkululeko/feat_extract/feats_clap.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5196 2024-04-24 17:12:28.000000 nkululeko-0.82.4/nkululeko/feat_extract/feats_hubert.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1622 2024-04-23 09:55:16.000000 nkululeko-0.82.4/nkululeko/feat_extract/feats_import.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2021 2023-12-19 11:16:16.000000 nkululeko-0.82.4/nkululeko/feat_extract/feats_mld.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4174 2024-04-23 10:17:00.000000 nkululeko-0.82.4/nkululeko/feat_extract/feats_mos.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3978 2024-04-24 10:46:37.000000 nkululeko-0.82.4/nkululeko/feat_extract/feats_opensmile.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4980 2024-04-23 09:16:18.000000 nkululeko-0.82.4/nkululeko/feat_extract/feats_oxbow.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3105 2024-04-23 09:16:18.000000 nkululeko-0.82.4/nkululeko/feat_extract/feats_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2829 2024-04-22 09:09:10.000000 nkululeko-0.82.4/nkululeko/feat_extract/feats_snr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3670 2024-04-23 09:59:48.000000 nkululeko-0.82.4/nkululeko/feat_extract/feats_spectra.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4803 2023-10-06 16:05:03.000000 nkululeko-0.82.4/nkululeko/feat_extract/feats_spkrec.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4528 2024-04-23 10:02:24.000000 nkululeko-0.82.4/nkululeko/feat_extract/feats_squim.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3319 2024-04-23 09:16:18.000000 nkululeko-0.82.4/nkululeko/feat_extract/feats_trill.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5285 2024-04-23 09:16:18.000000 nkululeko-0.82.4/nkululeko/feat_extract/feats_wav2vec2.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4703 2024-04-24 17:06:22.000000 nkululeko-0.82.4/nkululeko/feat_extract/feats_wavlm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4533 2024-04-23 11:35:51.000000 nkululeko-0.82.4/nkululeko/feat_extract/feats_whisper.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1448 2024-04-23 09:16:18.000000 nkululeko-0.82.4/nkululeko/feat_extract/featureset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21304 2024-04-15 13:57:11.000000 nkululeko-0.82.4/nkululeko/feat_extract/feinberg_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3976 2024-04-23 11:13:33.000000 nkululeko-0.82.4/nkululeko/feature_extractor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3474 2023-12-19 11:16:14.000000 nkululeko-0.82.4/nkululeko/file_checker.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7222 2023-12-19 11:16:14.000000 nkululeko-0.82.4/nkululeko/filter_data.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      453 2024-02-28 17:38:08.000000 nkululeko-0.82.4/nkululeko/glob_conf.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.529017 nkululeko-0.82.4/nkululeko/losses/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:16.000000 nkululeko-0.82.4/nkululeko/losses/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      976 2023-09-07 11:37:43.000000 nkululeko-0.82.4/nkululeko/losses/loss_ccc.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1309 2023-09-26 13:42:48.000000 nkululeko-0.82.4/nkululeko/losses/loss_softf1loss.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9335 2024-04-17 13:01:44.000000 nkululeko-0.82.4/nkululeko/modelrunner.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.533017 nkululeko-0.82.4/nkululeko/models/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:20.000000 nkululeko-0.82.4/nkululeko/models/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11569 2024-04-17 13:01:47.000000 nkululeko-0.82.4/nkululeko/models/model.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      378 2023-12-23 10:35:03.000000 nkululeko-0.82.4/nkululeko/models/model_bayes.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9726 2024-04-16 11:54:29.000000 nkululeko-0.82.4/nkululeko/models/model_cnn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      645 2023-09-26 13:42:48.000000 nkululeko-0.82.4/nkululeko/models/model_gmm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      573 2023-09-07 11:38:13.000000 nkululeko-0.82.4/nkululeko/models/model_knn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      580 2023-09-07 11:38:09.000000 nkululeko-0.82.4/nkululeko/models/model_knn_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      392 2023-12-19 13:57:23.000000 nkululeko-0.82.4/nkululeko/models/model_lin_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9107 2024-04-16 11:54:31.000000 nkululeko-0.82.4/nkululeko/models/model_mlp.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10083 2024-04-16 13:48:13.000000 nkululeko-0.82.4/nkululeko/models/model_mlp_regression.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      914 2024-04-17 12:17:54.000000 nkululeko-0.82.4/nkululeko/models/model_svm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      699 2024-03-21 10:56:18.000000 nkululeko-0.82.4/nkululeko/models/model_svr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      390 2023-09-07 11:38:37.000000 nkululeko-0.82.4/nkululeko/models/model_tree.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      397 2023-09-07 11:38:33.000000 nkululeko-0.82.4/nkululeko/models/model_tree_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      267 2024-03-21 10:21:07.000000 nkululeko-0.82.4/nkululeko/models/model_xgb.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      227 2023-12-14 15:14:23.000000 nkululeko-0.82.4/nkululeko/models/model_xgr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5634 2024-04-23 14:42:13.000000 nkululeko-0.82.4/nkululeko/multidb.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3354 2024-04-23 16:02:31.000000 nkululeko-0.82.4/nkululeko/nkuluflag.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1968 2024-04-23 12:35:01.000000 nkululeko-0.82.4/nkululeko/nkululeko.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    23025 2024-02-01 14:55:26.000000 nkululeko-0.82.4/nkululeko/plots.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2409 2024-04-22 09:09:10.000000 nkululeko-0.82.4/nkululeko/predict.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12427 2024-04-22 09:09:10.000000 nkululeko-0.82.4/nkululeko/reporter.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.533017 nkululeko-0.82.4/nkululeko/reporting/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-10-13 10:14:37.000000 nkululeko-0.82.4/nkululeko/reporting/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      648 2023-10-02 13:54:57.000000 nkululeko-0.82.4/nkululeko/reporting/defines.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1886 2023-12-19 13:13:44.000000 nkululeko-0.82.4/nkululeko/reporting/latex_writer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1060 2023-12-19 11:16:16.000000 nkululeko-0.82.4/nkululeko/reporting/report.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      533 2023-09-26 14:51:22.000000 nkululeko-0.82.4/nkululeko/reporting/report_item.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12670 2024-04-16 13:43:47.000000 nkululeko-0.82.4/nkululeko/reporting/reporter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      742 2024-04-16 12:21:39.000000 nkululeko-0.82.4/nkululeko/reporting/result.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2287 2024-04-22 09:09:10.000000 nkululeko-0.82.4/nkululeko/resample.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7624 2024-04-22 09:09:10.000000 nkululeko-0.82.4/nkululeko/runmanager.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4101 2024-01-31 12:20:11.000000 nkululeko-0.82.4/nkululeko/scaler.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4835 2024-02-29 11:06:43.000000 nkululeko-0.82.4/nkululeko/segment.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.533017 nkululeko-0.82.4/nkululeko/segmenting/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:24.000000 nkululeko-0.82.4/nkululeko/segmenting/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1947 2023-09-07 11:39:09.000000 nkululeko-0.82.4/nkululeko/segmenting/seg_inaspeechsegmenter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3301 2023-12-19 11:16:15.000000 nkululeko-0.82.4/nkululeko/segmenting/seg_silero.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10047 2023-09-26 13:42:49.000000 nkululeko-0.82.4/nkululeko/syllable_nuclei.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1525 2024-04-22 09:09:10.000000 nkululeko-0.82.4/nkululeko/test.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2753 2024-04-22 11:13:11.000000 nkululeko-0.82.4/nkululeko/test_predictor.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.533017 nkululeko-0.82.4/nkululeko/utils/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:28.000000 nkululeko-0.82.4/nkululeko/utils/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4021 2023-09-20 08:48:00.000000 nkululeko-0.82.4/nkululeko/utils/files.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2829 2024-04-22 09:09:10.000000 nkululeko-0.82.4/nkululeko/utils/stats.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12330 2024-03-21 11:06:05.000000 nkululeko-0.82.4/nkululeko/utils/util.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.533017 nkululeko-0.82.4/nkululeko.egg-info/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    35950 2024-04-24 17:19:59.000000 nkululeko-0.82.4/nkululeko.egg-info/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5144 2024-04-24 17:19:59.000000 nkululeko-0.82.4/nkululeko.egg-info/SOURCES.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2024-04-24 17:19:59.000000 nkululeko-0.82.4/nkululeko.egg-info/dependency_links.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      298 2024-04-24 17:19:59.000000 nkululeko-0.82.4/nkululeko.egg-info/requires.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2024-04-24 17:19:59.000000 nkululeko-0.82.4/nkululeko.egg-info/top_level.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.82.4/pyproject.toml
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1001 2024-04-24 17:19:59.533017 nkululeko-0.82.4/setup.cfg
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       57 2023-05-22 09:01:18.000000 nkululeko-0.82.4/setup.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.521017 nkululeko-0.82.4/venv/
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-24 17:19:59.533017 nkululeko-0.82.4/venv/bin/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1200 2023-12-29 19:06:16.000000 nkululeko-0.82.4/venv/bin/activate_this.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.053781 nkululeko-0.83.0/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    17290 2024-04-25 13:02:38.000000 nkululeko-0.83.0/CHANGELOG.md
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.83.0/LICENSE
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    36018 2024-04-25 13:09:47.053781 nkululeko-0.83.0/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    17457 2024-04-24 09:02:29.000000 nkululeko-0.83.0/README.md
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.041781 nkululeko-0.83.0/data/
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.041781 nkululeko-0.83.0/data/aesdd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1513 2023-10-04 08:46:04.000000 nkululeko-0.83.0/data/aesdd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.041781 nkululeko-0.83.0/data/androids/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-08-30 12:19:59.000000 nkululeko-0.83.0/data/androids/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.041781 nkululeko-0.83.0/data/androids_orig/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-08-20 18:21:45.000000 nkululeko-0.83.0/data/androids_orig/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.041781 nkululeko-0.83.0/data/androids_test/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-09-19 12:01:52.000000 nkululeko-0.83.0/data/androids_test/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.041781 nkululeko-0.83.0/data/ased/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1566 2023-09-19 09:19:58.000000 nkululeko-0.83.0/data/ased/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.041781 nkululeko-0.83.0/data/asvp-esd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1889 2023-09-06 07:54:15.000000 nkululeko-0.83.0/data/asvp-esd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.041781 nkululeko-0.83.0/data/baved/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1899 2023-09-12 12:11:50.000000 nkululeko-0.83.0/data/baved/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.041781 nkululeko-0.83.0/data/cafe/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1520 2023-09-11 09:21:27.000000 nkululeko-0.83.0/data/cafe/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.041781 nkululeko-0.83.0/data/clac/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1202 2023-10-04 08:46:04.000000 nkululeko-0.83.0/data/clac/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.041781 nkululeko-0.83.0/data/cmu-mosei/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1805 2023-10-20 09:59:16.000000 nkululeko-0.83.0/data/cmu-mosei/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.041781 nkululeko-0.83.0/data/demos/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2058 2023-09-19 09:19:58.000000 nkululeko-0.83.0/data/demos/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.041781 nkululeko-0.83.0/data/ekorpus/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1641 2023-09-12 12:11:50.000000 nkululeko-0.83.0/data/ekorpus/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.041781 nkululeko-0.83.0/data/emns/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2073 2023-09-19 09:19:58.000000 nkululeko-0.83.0/data/emns/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.041781 nkululeko-0.83.0/data/emofilm/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1305 2023-08-23 12:21:27.000000 nkululeko-0.83.0/data/emofilm/convert_to_16k.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1736 2023-08-23 06:49:28.000000 nkululeko-0.83.0/data/emofilm/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.041781 nkululeko-0.83.0/data/emorynlp/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1686 2023-09-20 08:48:00.000000 nkululeko-0.83.0/data/emorynlp/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.041781 nkululeko-0.83.0/data/emov-db/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1777 2023-12-19 12:05:21.000000 nkululeko-0.83.0/data/emov-db/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.041781 nkululeko-0.83.0/data/emovo/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1595 2023-09-19 09:19:58.000000 nkululeko-0.83.0/data/emovo/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.041781 nkululeko-0.83.0/data/emozionalmente/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9348 2023-08-23 06:49:28.000000 nkululeko-0.83.0/data/emozionalmente/create.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.041781 nkululeko-0.83.0/data/enterface/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2429 2023-09-19 09:19:58.000000 nkululeko-0.83.0/data/enterface/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.041781 nkululeko-0.83.0/data/esd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1534 2023-09-11 09:21:27.000000 nkululeko-0.83.0/data/esd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.041781 nkululeko-0.83.0/data/gerparas/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3023 2023-10-06 16:05:03.000000 nkululeko-0.83.0/data/gerparas/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.041781 nkululeko-0.83.0/data/iemocap/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3041 2023-10-04 08:46:04.000000 nkululeko-0.83.0/data/iemocap/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.041781 nkululeko-0.83.0/data/jl/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2022 2023-10-04 08:46:04.000000 nkululeko-0.83.0/data/jl/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.041781 nkululeko-0.83.0/data/jtes/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1727 2023-10-04 08:46:04.000000 nkululeko-0.83.0/data/jtes/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.041781 nkululeko-0.83.0/data/meld/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3694 2023-09-19 09:19:58.000000 nkululeko-0.83.0/data/meld/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.041781 nkululeko-0.83.0/data/mesd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2053 2023-09-19 09:19:58.000000 nkululeko-0.83.0/data/mesd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.041781 nkululeko-0.83.0/data/mess/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1529 2023-09-19 09:19:58.000000 nkululeko-0.83.0/data/mess/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.041781 nkululeko-0.83.0/data/mlendsnd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1714 2023-12-19 12:05:21.000000 nkululeko-0.83.0/data/mlendsnd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.041781 nkululeko-0.83.0/data/msp-improv/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2328 2023-08-23 06:49:28.000000 nkululeko-0.83.0/data/msp-improv/process_database2.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.041781 nkululeko-0.83.0/data/msp-podcast/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3021 2023-08-23 06:49:28.000000 nkululeko-0.83.0/data/msp-podcast/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.041781 nkululeko-0.83.0/data/oreau2/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1557 2023-09-19 09:19:58.000000 nkululeko-0.83.0/data/oreau2/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.041781 nkululeko-0.83.0/data/portuguese/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3892 2023-09-12 12:11:50.000000 nkululeko-0.83.0/data/portuguese/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.041781 nkululeko-0.83.0/data/ravdess/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3612 2024-04-22 09:09:10.000000 nkululeko-0.83.0/data/ravdess/process_database.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3144 2023-10-06 16:05:03.000000 nkululeko-0.83.0/data/ravdess/process_database_speaker.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.041781 nkululeko-0.83.0/data/savee/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1680 2023-09-19 09:19:58.000000 nkululeko-0.83.0/data/savee/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.041781 nkululeko-0.83.0/data/shemo/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1624 2023-09-19 09:19:58.000000 nkululeko-0.83.0/data/shemo/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.041781 nkululeko-0.83.0/data/subesco/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2991 2023-09-19 09:19:58.000000 nkululeko-0.83.0/data/subesco/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.045781 nkululeko-0.83.0/data/tess/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1472 2023-09-11 09:21:27.000000 nkululeko-0.83.0/data/tess/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.045781 nkululeko-0.83.0/data/thorsten-emotional/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1142 2023-09-06 07:54:15.000000 nkululeko-0.83.0/data/thorsten-emotional/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.045781 nkululeko-0.83.0/data/urdu/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1803 2023-09-19 09:19:58.000000 nkululeko-0.83.0/data/urdu/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.045781 nkululeko-0.83.0/data/vivae/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1209 2023-09-12 12:11:50.000000 nkululeko-0.83.0/data/vivae/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.041781 nkululeko-0.83.0/docs/
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.045781 nkululeko-0.83.0/docs/source/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3070 2024-04-22 09:09:10.000000 nkululeko-0.83.0/docs/source/conf.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.041781 nkululeko-0.83.0/meta/
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.045781 nkululeko-0.83.0/meta/demos/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      617 2021-10-28 13:49:53.000000 nkululeko-0.83.0/meta/demos/demo_best_model.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.045781 nkululeko-0.83.0/meta/demos/multiple_exeriments/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      819 2024-04-24 13:07:11.000000 nkululeko-0.83.0/meta/demos/multiple_exeriments/do_experiments.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1252 2022-12-07 09:32:42.000000 nkululeko-0.83.0/meta/demos/my_experiment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1095 2022-12-15 16:06:58.000000 nkululeko-0.83.0/meta/demos/my_experiment_local.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      681 2021-10-28 13:49:53.000000 nkululeko-0.83.0/meta/demos/plot_faster_anim.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.045781 nkululeko-0.83.0/nkululeko/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       63 2023-08-31 11:56:33.000000 nkululeko-0.83.0/nkululeko/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3194 2024-02-29 11:07:44.000000 nkululeko-0.83.0/nkululeko/aug_train.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3051 2024-02-29 11:04:02.000000 nkululeko-0.83.0/nkululeko/augment.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.049781 nkululeko-0.83.0/nkululeko/augmenting/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:16:55.000000 nkululeko-0.83.0/nkululeko/augmenting/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2905 2023-12-29 16:48:37.000000 nkululeko-0.83.0/nkululeko/augmenting/augmenter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2669 2023-12-29 16:49:20.000000 nkululeko-0.83.0/nkululeko/augmenting/randomsplicer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1791 2023-09-07 11:33:33.000000 nkululeko-0.83.0/nkululeko/augmenting/randomsplicing.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3335 2023-12-19 11:16:16.000000 nkululeko-0.83.0/nkululeko/augmenting/resampler.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.049781 nkululeko-0.83.0/nkululeko/autopredict/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:02.000000 nkululeko-0.83.0/nkululeko/autopredict/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1095 2023-12-19 11:16:15.000000 nkululeko-0.83.0/nkululeko/autopredict/ap_age.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1024 2023-12-19 11:16:15.000000 nkululeko-0.83.0/nkululeko/autopredict/ap_arousal.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1039 2023-12-19 11:16:15.000000 nkululeko-0.83.0/nkululeko/autopredict/ap_dominance.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1008 2023-12-19 11:16:15.000000 nkululeko-0.83.0/nkululeko/autopredict/ap_gender.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1104 2023-12-19 11:16:16.000000 nkululeko-0.83.0/nkululeko/autopredict/ap_mos.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1137 2023-12-19 11:16:15.000000 nkululeko-0.83.0/nkululeko/autopredict/ap_pesq.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1185 2023-12-19 11:16:16.000000 nkululeko-0.83.0/nkululeko/autopredict/ap_sdr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1107 2023-12-19 11:16:15.000000 nkululeko-0.83.0/nkululeko/autopredict/ap_snr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1184 2023-12-19 11:16:15.000000 nkululeko-0.83.0/nkululeko/autopredict/ap_stoi.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1024 2023-12-19 11:16:15.000000 nkululeko-0.83.0/nkululeko/autopredict/ap_valence.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5048 2024-04-22 09:09:10.000000 nkululeko-0.83.0/nkululeko/autopredict/estimate_snr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      969 2023-09-07 11:39:39.000000 nkululeko-0.83.0/nkululeko/cacheddataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       39 2024-04-25 13:02:38.000000 nkululeko-0.83.0/nkululeko/constants.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.049781 nkululeko-0.83.0/nkululeko/data/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:06.000000 nkululeko-0.83.0/nkululeko/data/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    27650 2024-04-22 09:10:47.000000 nkululeko-0.83.0/nkululeko/data/dataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3884 2024-04-24 12:41:45.000000 nkululeko-0.83.0/nkululeko/data/dataset_csv.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3264 2024-04-22 09:09:10.000000 nkululeko-0.83.0/nkululeko/demo.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2025 2024-02-29 21:51:15.000000 nkululeko-0.83.0/nkululeko/demo_feats.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4755 2024-04-22 09:09:10.000000 nkululeko-0.83.0/nkululeko/demo_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    29574 2024-04-25 13:02:38.000000 nkululeko-0.83.0/nkululeko/experiment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2310 2024-04-22 09:09:10.000000 nkululeko-0.83.0/nkululeko/explore.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4632 2023-12-19 11:16:14.000000 nkululeko-0.83.0/nkululeko/export.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.049781 nkululeko-0.83.0/nkululeko/feat_extract/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:10.000000 nkululeko-0.83.0/nkululeko/feat_extract/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3113 2024-04-23 09:16:18.000000 nkululeko-0.83.0/nkululeko/feat_extract/feats_agender.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3346 2024-04-16 13:29:59.000000 nkululeko-0.83.0/nkululeko/feat_extract/feats_agender_agender.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11399 2024-01-24 16:15:03.000000 nkululeko-0.83.0/nkululeko/feat_extract/feats_analyser.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3162 2024-04-23 09:16:18.000000 nkululeko-0.83.0/nkululeko/feat_extract/feats_auddim.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3187 2024-04-23 09:16:18.000000 nkululeko-0.83.0/nkululeko/feat_extract/feats_audmodel.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3489 2024-04-23 09:16:18.000000 nkululeko-0.83.0/nkululeko/feat_extract/feats_clap.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5196 2024-04-24 17:12:28.000000 nkululeko-0.83.0/nkululeko/feat_extract/feats_hubert.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1622 2024-04-23 09:55:16.000000 nkululeko-0.83.0/nkululeko/feat_extract/feats_import.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2021 2023-12-19 11:16:16.000000 nkululeko-0.83.0/nkululeko/feat_extract/feats_mld.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4174 2024-04-23 10:17:00.000000 nkululeko-0.83.0/nkululeko/feat_extract/feats_mos.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3978 2024-04-24 10:46:37.000000 nkululeko-0.83.0/nkululeko/feat_extract/feats_opensmile.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4980 2024-04-23 09:16:18.000000 nkululeko-0.83.0/nkululeko/feat_extract/feats_oxbow.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3105 2024-04-23 09:16:18.000000 nkululeko-0.83.0/nkululeko/feat_extract/feats_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2829 2024-04-22 09:09:10.000000 nkululeko-0.83.0/nkululeko/feat_extract/feats_snr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3670 2024-04-23 09:59:48.000000 nkululeko-0.83.0/nkululeko/feat_extract/feats_spectra.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4803 2023-10-06 16:05:03.000000 nkululeko-0.83.0/nkululeko/feat_extract/feats_spkrec.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4528 2024-04-23 10:02:24.000000 nkululeko-0.83.0/nkululeko/feat_extract/feats_squim.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3319 2024-04-23 09:16:18.000000 nkululeko-0.83.0/nkululeko/feat_extract/feats_trill.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5285 2024-04-23 09:16:18.000000 nkululeko-0.83.0/nkululeko/feat_extract/feats_wav2vec2.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4703 2024-04-24 17:06:22.000000 nkululeko-0.83.0/nkululeko/feat_extract/feats_wavlm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4533 2024-04-23 11:35:51.000000 nkululeko-0.83.0/nkululeko/feat_extract/feats_whisper.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1448 2024-04-23 09:16:18.000000 nkululeko-0.83.0/nkululeko/feat_extract/featureset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21304 2024-04-15 13:57:11.000000 nkululeko-0.83.0/nkululeko/feat_extract/feinberg_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3976 2024-04-23 11:13:33.000000 nkululeko-0.83.0/nkululeko/feature_extractor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3474 2023-12-19 11:16:14.000000 nkululeko-0.83.0/nkululeko/file_checker.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7222 2023-12-19 11:16:14.000000 nkululeko-0.83.0/nkululeko/filter_data.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      453 2024-02-28 17:38:08.000000 nkululeko-0.83.0/nkululeko/glob_conf.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.049781 nkululeko-0.83.0/nkululeko/losses/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:16.000000 nkululeko-0.83.0/nkululeko/losses/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      976 2023-09-07 11:37:43.000000 nkululeko-0.83.0/nkululeko/losses/loss_ccc.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1309 2023-09-26 13:42:48.000000 nkululeko-0.83.0/nkululeko/losses/loss_softf1loss.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9288 2024-04-25 13:02:38.000000 nkululeko-0.83.0/nkululeko/modelrunner.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.053781 nkululeko-0.83.0/nkululeko/models/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:20.000000 nkululeko-0.83.0/nkululeko/models/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11569 2024-04-17 13:01:47.000000 nkululeko-0.83.0/nkululeko/models/model.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      378 2023-12-23 10:35:03.000000 nkululeko-0.83.0/nkululeko/models/model_bayes.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9726 2024-04-16 11:54:29.000000 nkululeko-0.83.0/nkululeko/models/model_cnn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      645 2023-09-26 13:42:48.000000 nkululeko-0.83.0/nkululeko/models/model_gmm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      573 2023-09-07 11:38:13.000000 nkululeko-0.83.0/nkululeko/models/model_knn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      580 2023-09-07 11:38:09.000000 nkululeko-0.83.0/nkululeko/models/model_knn_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      392 2023-12-19 13:57:23.000000 nkululeko-0.83.0/nkululeko/models/model_lin_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9107 2024-04-16 11:54:31.000000 nkululeko-0.83.0/nkululeko/models/model_mlp.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10083 2024-04-16 13:48:13.000000 nkululeko-0.83.0/nkululeko/models/model_mlp_regression.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      914 2024-04-17 12:17:54.000000 nkululeko-0.83.0/nkululeko/models/model_svm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      699 2024-03-21 10:56:18.000000 nkululeko-0.83.0/nkululeko/models/model_svr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      390 2023-09-07 11:38:37.000000 nkululeko-0.83.0/nkululeko/models/model_tree.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      397 2023-09-07 11:38:33.000000 nkululeko-0.83.0/nkululeko/models/model_tree_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      267 2024-03-21 10:21:07.000000 nkululeko-0.83.0/nkululeko/models/model_xgb.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      227 2023-12-14 15:14:23.000000 nkululeko-0.83.0/nkululeko/models/model_xgr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5634 2024-04-23 14:42:13.000000 nkululeko-0.83.0/nkululeko/multidb.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3354 2024-04-23 16:02:31.000000 nkululeko-0.83.0/nkululeko/nkuluflag.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1968 2024-04-23 12:35:01.000000 nkululeko-0.83.0/nkululeko/nkululeko.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    23025 2024-02-01 14:55:26.000000 nkululeko-0.83.0/nkululeko/plots.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2409 2024-04-22 09:09:10.000000 nkululeko-0.83.0/nkululeko/predict.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12483 2024-04-25 13:02:38.000000 nkululeko-0.83.0/nkululeko/reporter.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.053781 nkululeko-0.83.0/nkululeko/reporting/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-10-13 10:14:37.000000 nkululeko-0.83.0/nkululeko/reporting/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      648 2023-10-02 13:54:57.000000 nkululeko-0.83.0/nkululeko/reporting/defines.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1886 2023-12-19 13:13:44.000000 nkululeko-0.83.0/nkululeko/reporting/latex_writer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1060 2023-12-19 11:16:16.000000 nkululeko-0.83.0/nkululeko/reporting/report.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      533 2023-09-26 14:51:22.000000 nkululeko-0.83.0/nkululeko/reporting/report_item.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12841 2024-04-25 13:02:38.000000 nkululeko-0.83.0/nkululeko/reporting/reporter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      742 2024-04-16 12:21:39.000000 nkululeko-0.83.0/nkululeko/reporting/result.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2287 2024-04-22 09:09:10.000000 nkululeko-0.83.0/nkululeko/resample.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7624 2024-04-22 09:09:10.000000 nkululeko-0.83.0/nkululeko/runmanager.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4101 2024-01-31 12:20:11.000000 nkululeko-0.83.0/nkululeko/scaler.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4835 2024-02-29 11:06:43.000000 nkululeko-0.83.0/nkululeko/segment.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.053781 nkululeko-0.83.0/nkululeko/segmenting/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:24.000000 nkululeko-0.83.0/nkululeko/segmenting/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1947 2023-09-07 11:39:09.000000 nkululeko-0.83.0/nkululeko/segmenting/seg_inaspeechsegmenter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3301 2023-12-19 11:16:15.000000 nkululeko-0.83.0/nkululeko/segmenting/seg_silero.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10047 2023-09-26 13:42:49.000000 nkululeko-0.83.0/nkululeko/syllable_nuclei.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1525 2024-04-22 09:09:10.000000 nkululeko-0.83.0/nkululeko/test.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3148 2024-04-25 13:02:38.000000 nkululeko-0.83.0/nkululeko/test_predictor.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.053781 nkululeko-0.83.0/nkululeko/utils/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:28.000000 nkululeko-0.83.0/nkululeko/utils/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4021 2023-09-20 08:48:00.000000 nkululeko-0.83.0/nkululeko/utils/files.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2829 2024-04-22 09:09:10.000000 nkululeko-0.83.0/nkululeko/utils/stats.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12330 2024-03-21 11:06:05.000000 nkululeko-0.83.0/nkululeko/utils/util.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.053781 nkululeko-0.83.0/nkululeko.egg-info/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    36018 2024-04-25 13:09:47.000000 nkululeko-0.83.0/nkululeko.egg-info/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5144 2024-04-25 13:09:47.000000 nkululeko-0.83.0/nkululeko.egg-info/SOURCES.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2024-04-25 13:09:47.000000 nkululeko-0.83.0/nkululeko.egg-info/dependency_links.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      298 2024-04-25 13:09:47.000000 nkululeko-0.83.0/nkululeko.egg-info/requires.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2024-04-25 13:09:47.000000 nkululeko-0.83.0/nkululeko.egg-info/top_level.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.83.0/pyproject.toml
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1001 2024-04-25 13:09:47.053781 nkululeko-0.83.0/setup.cfg
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       57 2023-05-22 09:01:18.000000 nkululeko-0.83.0/setup.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.041781 nkululeko-0.83.0/venv/
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-25 13:09:47.053781 nkululeko-0.83.0/venv/bin/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1200 2023-12-29 19:06:16.000000 nkululeko-0.83.0/venv/bin/activate_this.py
```

### Comparing `nkululeko-0.82.4/CHANGELOG.md` & `nkululeko-0.83.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changelog
 =========
 
+Version 0.83.0
+--------------
+* test module now prints out reports
+
 Version 0.82.4
 --------------
 * fixed bug in wavlm 
 
 Version 0.82.3
 --------------
 * fixed another audformat peculiarity to interprete time values as nanoseconds
```

### Comparing `nkululeko-0.82.4/LICENSE` & `nkululeko-0.83.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/PKG-INFO` & `nkululeko-0.83.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.82.4
+Version: 0.83.0
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -329,14 +329,18 @@
    year = {2022},
 }
 ```
 
 Changelog
 =========
 
+Version 0.83.0
+--------------
+* test module now prints out reports
+
 Version 0.82.4
 --------------
 * fixed bug in wavlm 
 
 Version 0.82.3
 --------------
 * fixed another audformat peculiarity to interprete time values as nanoseconds
```

### Comparing `nkululeko-0.82.4/README.md` & `nkululeko-0.83.0/README.md`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/data/aesdd/process_database.py` & `nkululeko-0.83.0/data/aesdd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/data/androids/process_database.py` & `nkululeko-0.83.0/data/androids/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/data/androids_orig/process_database.py` & `nkululeko-0.83.0/data/androids_orig/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/data/androids_test/process_database.py` & `nkululeko-0.83.0/data/androids_test/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/data/ased/process_database.py` & `nkululeko-0.83.0/data/ased/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/data/asvp-esd/process_database.py` & `nkululeko-0.83.0/data/asvp-esd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/data/baved/process_database.py` & `nkululeko-0.83.0/data/baved/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/data/cafe/process_database.py` & `nkululeko-0.83.0/data/cafe/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/data/clac/process_database.py` & `nkululeko-0.83.0/data/clac/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/data/cmu-mosei/process_database.py` & `nkululeko-0.83.0/data/cmu-mosei/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/data/demos/process_database.py` & `nkululeko-0.83.0/data/demos/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/data/ekorpus/process_database.py` & `nkululeko-0.83.0/data/ekorpus/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/data/emns/process_database.py` & `nkululeko-0.83.0/data/emns/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/data/emofilm/convert_to_16k.py` & `nkululeko-0.83.0/data/emofilm/convert_to_16k.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/data/emofilm/process_database.py` & `nkululeko-0.83.0/data/emofilm/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/data/emorynlp/process_database.py` & `nkululeko-0.83.0/data/emorynlp/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/data/emov-db/process_database.py` & `nkululeko-0.83.0/data/emov-db/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/data/emovo/process_database.py` & `nkululeko-0.83.0/data/emovo/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/data/emozionalmente/create.py` & `nkululeko-0.83.0/data/emozionalmente/create.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/data/enterface/process_database.py` & `nkululeko-0.83.0/data/enterface/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/data/esd/process_database.py` & `nkululeko-0.83.0/data/esd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/data/gerparas/process_database.py` & `nkululeko-0.83.0/data/gerparas/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/data/iemocap/process_database.py` & `nkululeko-0.83.0/data/iemocap/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/data/jl/process_database.py` & `nkululeko-0.83.0/data/jl/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/data/jtes/process_database.py` & `nkululeko-0.83.0/data/jtes/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/data/meld/process_database.py` & `nkululeko-0.83.0/data/meld/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/data/mesd/process_database.py` & `nkululeko-0.83.0/data/mesd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/data/mess/process_database.py` & `nkululeko-0.83.0/data/mess/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/data/mlendsnd/process_database.py` & `nkululeko-0.83.0/data/mlendsnd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/data/msp-improv/process_database2.py` & `nkululeko-0.83.0/data/msp-improv/process_database2.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/data/msp-podcast/process_database.py` & `nkululeko-0.83.0/data/msp-podcast/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/data/oreau2/process_database.py` & `nkululeko-0.83.0/data/oreau2/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/data/portuguese/process_database.py` & `nkululeko-0.83.0/data/portuguese/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/data/ravdess/process_database.py` & `nkululeko-0.83.0/data/ravdess/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/data/ravdess/process_database_speaker.py` & `nkululeko-0.83.0/data/ravdess/process_database_speaker.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/data/savee/process_database.py` & `nkululeko-0.83.0/data/savee/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/data/shemo/process_database.py` & `nkululeko-0.83.0/data/shemo/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/data/subesco/process_database.py` & `nkululeko-0.83.0/data/subesco/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/data/tess/process_database.py` & `nkululeko-0.83.0/data/tess/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/data/thorsten-emotional/process_database.py` & `nkululeko-0.83.0/data/thorsten-emotional/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/data/urdu/process_database.py` & `nkululeko-0.83.0/data/urdu/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/data/vivae/process_database.py` & `nkululeko-0.83.0/data/vivae/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/docs/source/conf.py` & `nkululeko-0.83.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/meta/demos/demo_best_model.py` & `nkululeko-0.83.0/meta/demos/demo_best_model.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/meta/demos/multiple_exeriments/do_experiments.py` & `nkululeko-0.83.0/meta/demos/multiple_exeriments/do_experiments.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/meta/demos/my_experiment.py` & `nkululeko-0.83.0/meta/demos/my_experiment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/meta/demos/my_experiment_local.py` & `nkululeko-0.83.0/meta/demos/my_experiment_local.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/meta/demos/plot_faster_anim.py` & `nkululeko-0.83.0/meta/demos/plot_faster_anim.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/aug_train.py` & `nkululeko-0.83.0/nkululeko/aug_train.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/augment.py` & `nkululeko-0.83.0/nkululeko/augment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/augmenting/augmenter.py` & `nkululeko-0.83.0/nkululeko/augmenting/augmenter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/augmenting/randomsplicer.py` & `nkululeko-0.83.0/nkululeko/augmenting/randomsplicer.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/augmenting/randomsplicing.py` & `nkululeko-0.83.0/nkululeko/augmenting/randomsplicing.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/augmenting/resampler.py` & `nkululeko-0.83.0/nkululeko/augmenting/resampler.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/autopredict/ap_age.py` & `nkululeko-0.83.0/nkululeko/autopredict/ap_age.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/autopredict/ap_arousal.py` & `nkululeko-0.83.0/nkululeko/autopredict/ap_arousal.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/autopredict/ap_dominance.py` & `nkululeko-0.83.0/nkululeko/autopredict/ap_dominance.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/autopredict/ap_gender.py` & `nkululeko-0.83.0/nkululeko/autopredict/ap_gender.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/autopredict/ap_mos.py` & `nkululeko-0.83.0/nkululeko/autopredict/ap_mos.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/autopredict/ap_pesq.py` & `nkululeko-0.83.0/nkululeko/autopredict/ap_pesq.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/autopredict/ap_sdr.py` & `nkululeko-0.83.0/nkululeko/autopredict/ap_sdr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/autopredict/ap_snr.py` & `nkululeko-0.83.0/nkululeko/autopredict/ap_snr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/autopredict/ap_stoi.py` & `nkululeko-0.83.0/nkululeko/autopredict/ap_stoi.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/autopredict/ap_valence.py` & `nkululeko-0.83.0/nkululeko/autopredict/ap_valence.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/autopredict/estimate_snr.py` & `nkululeko-0.83.0/nkululeko/autopredict/estimate_snr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/cacheddataset.py` & `nkululeko-0.83.0/nkululeko/cacheddataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/data/dataset.py` & `nkululeko-0.83.0/nkululeko/data/dataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/data/dataset_csv.py` & `nkululeko-0.83.0/nkululeko/data/dataset_csv.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/demo.py` & `nkululeko-0.83.0/nkululeko/demo.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/demo_feats.py` & `nkululeko-0.83.0/nkululeko/demo_feats.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/demo_predictor.py` & `nkululeko-0.83.0/nkululeko/demo_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/experiment.py` & `nkululeko-0.83.0/nkululeko/experiment.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from nkululeko.feature_extractor import FeatureExtractor
 from nkululeko.file_checker import FileChecker
 from nkululeko.filter_data import DataFilter, filter_min_dur
 from nkululeko.plots import Plots
 from nkululeko.reporting.report import Report
 from nkululeko.runmanager import Runmanager
 from nkululeko.scaler import Scaler
-from nkululeko.test_predictor import Test_predictor
+from nkululeko.test_predictor import TestPredictor
 from nkululeko.utils.util import Util
 
 
 class Experiment:
     """Main class specifying an experiment"""
 
     def __init__(self, config_obj):
@@ -668,15 +668,15 @@
             model, file, is_list, self.feature_extractor, labelEncoder, outfile
         )
         demo.run_demo()
 
     def predict_test_and_save(self, result_name):
         model = self.runmgr.get_best_model()
         model.set_testdata(self.df_test, self.feats_test)
-        test_predictor = Test_predictor(
+        test_predictor = TestPredictor(
             model, self.df_test, self.label_encoder, result_name
         )
         test_predictor.predict_and_store()
 
     def load(self, filename):
         f = open(filename, "rb")
         tmp_dict = pickle.load(f)
```

### Comparing `nkululeko-0.82.4/nkululeko/explore.py` & `nkululeko-0.83.0/nkululeko/explore.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/export.py` & `nkululeko-0.83.0/nkululeko/export.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/feat_extract/feats_agender.py` & `nkululeko-0.83.0/nkululeko/feat_extract/feats_agender.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/feat_extract/feats_agender_agender.py` & `nkululeko-0.83.0/nkululeko/feat_extract/feats_agender_agender.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/feat_extract/feats_analyser.py` & `nkululeko-0.83.0/nkululeko/feat_extract/feats_analyser.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/feat_extract/feats_auddim.py` & `nkululeko-0.83.0/nkululeko/feat_extract/feats_auddim.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/feat_extract/feats_audmodel.py` & `nkululeko-0.83.0/nkululeko/feat_extract/feats_audmodel.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/feat_extract/feats_clap.py` & `nkululeko-0.83.0/nkululeko/feat_extract/feats_clap.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/feat_extract/feats_hubert.py` & `nkululeko-0.83.0/nkululeko/feat_extract/feats_hubert.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/feat_extract/feats_import.py` & `nkululeko-0.83.0/nkululeko/feat_extract/feats_import.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/feat_extract/feats_mld.py` & `nkululeko-0.83.0/nkululeko/feat_extract/feats_mld.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/feat_extract/feats_mos.py` & `nkululeko-0.83.0/nkululeko/feat_extract/feats_mos.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/feat_extract/feats_opensmile.py` & `nkululeko-0.83.0/nkululeko/feat_extract/feats_opensmile.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/feat_extract/feats_oxbow.py` & `nkululeko-0.83.0/nkululeko/feat_extract/feats_oxbow.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/feat_extract/feats_praat.py` & `nkululeko-0.83.0/nkululeko/feat_extract/feats_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/feat_extract/feats_snr.py` & `nkululeko-0.83.0/nkululeko/feat_extract/feats_snr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/feat_extract/feats_spectra.py` & `nkululeko-0.83.0/nkululeko/feat_extract/feats_spectra.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/feat_extract/feats_spkrec.py` & `nkululeko-0.83.0/nkululeko/feat_extract/feats_spkrec.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/feat_extract/feats_squim.py` & `nkululeko-0.83.0/nkululeko/feat_extract/feats_squim.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/feat_extract/feats_trill.py` & `nkululeko-0.83.0/nkululeko/feat_extract/feats_trill.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/feat_extract/feats_wav2vec2.py` & `nkululeko-0.83.0/nkululeko/feat_extract/feats_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/feat_extract/feats_wavlm.py` & `nkululeko-0.83.0/nkululeko/feat_extract/feats_wavlm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/feat_extract/feats_whisper.py` & `nkululeko-0.83.0/nkululeko/feat_extract/feats_whisper.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/feat_extract/featureset.py` & `nkululeko-0.83.0/nkululeko/feat_extract/featureset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/feat_extract/feinberg_praat.py` & `nkululeko-0.83.0/nkululeko/feat_extract/feinberg_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/feature_extractor.py` & `nkululeko-0.83.0/nkululeko/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/file_checker.py` & `nkululeko-0.83.0/nkululeko/file_checker.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/filter_data.py` & `nkululeko-0.83.0/nkululeko/filter_data.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/losses/loss_ccc.py` & `nkululeko-0.83.0/nkululeko/losses/loss_ccc.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/losses/loss_softf1loss.py` & `nkululeko-0.83.0/nkululeko/losses/loss_softf1loss.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/modelrunner.py` & `nkululeko-0.83.0/nkululeko/modelrunner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 # modelrunner.py
 
 import pandas as pd
 
-from nkululeko.utils.util import Util
 from nkululeko import glob_conf
-import nkululeko.glob_conf as glob_conf
+from nkululeko.utils.util import Util
 
 
 class Modelrunner:
-    """
-    Class to model one run
-    """
+    """Class to model one run."""
 
     def __init__(self, df_train, df_test, feats_train, feats_test, run):
-        """Constructor setting up the dataframes
+        """Constructor setting up the dataframes.
+
         Args:
             df_train: train dataframe
             df_test: test dataframe
             feats_train: train features
             feats_train: test features
         """
         self.df_train, self.df_test, self.feats_train, self.feats_test = (
```

### Comparing `nkululeko-0.82.4/nkululeko/models/model.py` & `nkululeko-0.83.0/nkululeko/models/model.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/models/model_cnn.py` & `nkululeko-0.83.0/nkululeko/models/model_cnn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/models/model_gmm.py` & `nkululeko-0.83.0/nkululeko/models/model_gmm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/models/model_knn.py` & `nkululeko-0.83.0/nkululeko/models/model_knn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/models/model_knn_reg.py` & `nkululeko-0.83.0/nkululeko/models/model_knn_reg.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/models/model_mlp.py` & `nkululeko-0.83.0/nkululeko/models/model_mlp.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/models/model_mlp_regression.py` & `nkululeko-0.83.0/nkululeko/models/model_mlp_regression.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/models/model_svm.py` & `nkululeko-0.83.0/nkululeko/models/model_svm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/models/model_svr.py` & `nkululeko-0.83.0/nkululeko/models/model_svr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/multidb.py` & `nkululeko-0.83.0/nkululeko/multidb.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/nkuluflag.py` & `nkululeko-0.83.0/nkululeko/nkuluflag.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/nkululeko.py` & `nkululeko-0.83.0/nkululeko/nkululeko.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/plots.py` & `nkululeko-0.83.0/nkululeko/plots.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/predict.py` & `nkululeko-0.83.0/nkululeko/predict.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/reporter.py` & `nkululeko-0.83.0/nkululeko/reporter.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 """Reporter module.
 
 This module contains the Reporter class which is responsible for generating reports.
 """
 
-
 import ast
 import glob
 import json
 import math
 
 import matplotlib.pyplot as plt
 import numpy as np
 from scipy.stats import pearsonr
-from sklearn.metrics import (
-    ConfusionMatrixDisplay,
-    accuracy_score,
-    classification_report,
-    confusion_matrix,
-    mean_absolute_error,
-    mean_squared_error,
-    r2_score,
-    recall_score,
-)
+from sklearn.metrics import ConfusionMatrixDisplay
+from sklearn.metrics import accuracy_score
+from sklearn.metrics import classification_report
+from sklearn.metrics import confusion_matrix
+from sklearn.metrics import mean_absolute_error
+from sklearn.metrics import mean_squared_error
+from sklearn.metrics import r2_score
+from sklearn.metrics import recall_score
 from sklearn.utils import resample
 
 import nkululeko.glob_conf as glob_conf
 from nkululeko.reporting.defines import Header
 from nkululeko.reporting.report_item import ReportItem
 from nkululeko.result import Result
 from nkululeko.utils.util import Util
@@ -66,19 +63,17 @@
                 self.result.test = recall_score(
                     self.truths, self.preds, average="macro"
                 )
                 self.result.loss = 1 - accuracy_score(self.truths, self.preds)
             else:
                 # regression experiment
                 if self.measure == "mse":
-                    self.result.test = mean_squared_error(
-                        self.truths, self.preds)
+                    self.result.test = mean_squared_error(self.truths, self.preds)
                 elif self.measure == "mae":
-                    self.result.test = mean_absolute_error(
-                        self.truths, self.preds)
+                    self.result.test = mean_absolute_error(self.truths, self.preds)
                 elif self.measure == "ccc":
                     self.result.test = self.ccc(self.truths, self.preds)
                     if math.isnan(self.result.test):
                         self.util.debug(f"Truth: {self.truths}")
                         self.util.debug(f"Predict.: {self.preds}")
                         self.util.debug(f"Result is NAN: setting to -1")
                         self.result.test = -1
@@ -111,15 +106,15 @@
 
     This function creates a confusion matrix for each speaker in the result_df.
     The result_df should contain the columns: preds, truths and speaker.
 
     Args:
         * result_df: a pandas dataframe with columns: preds, truths and speaker
         * plot_name: a string with the name of the plot
-        * function: a string with the function to use for each speaker, 
+        * function: a string with the function to use for each speaker,
         can be 'mode' or 'mean'
 
     Returns:
         * None
     """
     # Initialize empty arrays for predictions and truths
     pred = np.zeros(0)
@@ -181,16 +176,15 @@
             ).plot(cmap="Blues")
 
         reg_res = ""
         if not self.is_classification:
             reg_res = f", {self.MEASURE}: {self.result.test:.3f}"
 
         if epoch != 0:
-            plt.title(
-                f"Confusion Matrix, UAR: {uar:.3f}{reg_res}, Epoch: {epoch}")
+            plt.title(f"Confusion Matrix, UAR: {uar:.3f}{reg_res}, Epoch: {epoch}")
         else:
             plt.title(f"Confusion Matrix, UAR: {uar:.3f}{reg_res}")
         img_path = f"{fig_dir}{plot_name}.{self.format}"
         plt.savefig(img_path)
         fig.clear()
         plt.close(fig)
         plt.savefig(img_path)
@@ -261,16 +255,15 @@
                     f"{measure}: {result:.3f}, r_2: {r2:.3f}, pcc {pcc:.3f}"
                 )
 
     def make_conf_animation(self, out_name):
         import imageio
 
         fig_dir = self.util.get_path("fig_dir")
-        filenames = glob.glob(
-            fig_dir + f"{self.util.get_plot_name()}*_?_???_cnf.png")
+        filenames = glob.glob(fig_dir + f"{self.util.get_plot_name()}*_?_???_cnf.png")
         images = []
         for filename in filenames:
             images.append(imageio.imread(filename))
         fps = self.util.config_val("PLOT", "fps", "1")
         try:
             imageio.mimsave(fig_dir + out_name, images, fps=int(fps))
         except RuntimeError as e:
@@ -318,15 +311,14 @@
     def ccc(ground_truth, prediction):
         mean_gt = np.mean(ground_truth, 0)
         mean_pred = np.mean(prediction, 0)
         var_gt = np.var(ground_truth, 0)
         var_pred = np.var(prediction, 0)
         v_pred = prediction - mean_pred
         v_gt = ground_truth - mean_gt
-        cor = sum(v_pred * v_gt) / \
-            (np.sqrt(sum(v_pred**2)) * np.sqrt(sum(v_gt**2)))
+        cor = sum(v_pred * v_gt) / (np.sqrt(sum(v_pred**2)) * np.sqrt(sum(v_gt**2)))
         sd_gt = np.std(ground_truth)
         sd_pred = np.std(prediction)
         numerator = 2 * cor * sd_gt * sd_pred
         denominator = var_gt + var_pred + (mean_gt - mean_pred) ** 2
         ccc = numerator / denominator
         return ccc
```

### Comparing `nkululeko-0.82.4/nkululeko/reporting/defines.py` & `nkululeko-0.83.0/nkululeko/reporting/defines.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/reporting/latex_writer.py` & `nkululeko-0.83.0/nkululeko/reporting/latex_writer.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/reporting/report.py` & `nkululeko-0.83.0/nkululeko/reporting/report.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/reporting/report_item.py` & `nkululeko-0.83.0/nkululeko/reporting/report_item.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/reporting/reporter.py` & `nkululeko-0.83.0/nkululeko/reporting/reporter.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,14 +51,15 @@
         self.format = self.util.config_val("PLOT", "format", "png")
         self.truths = np.asarray(truths)
         self.preds = np.asarray(preds)
         self.result = Result(0, 0, 0, 0, "unknown")
         self.run = run
         self.epoch = epoch
         self.__set_measure()
+        self.filenameadd = ""
         self.cont_to_cat = False
         if len(self.truths) > 0 and len(self.preds) > 0:
             if self.util.exp_is_classification():
                 uar, (upper, lower) = evaluate_with_conf_int(
                     self.preds,
                     unweighted_average_recall,
                     self.truths,
@@ -202,15 +203,15 @@
                 + f"(+-{up_str}/{low_str}), {reg_res}, Epoch: {epoch}"
             )
         else:
             plt.title(
                 f"Confusion Matrix, UAR: {uar_str} "
                 + f"(+-{up_str}/{low_str}) {reg_res}"
             )
-        img_path = f"{fig_dir}{plot_name}.{self.format}"
+        img_path = f"{fig_dir}{plot_name}{self.filenameadd}.{self.format}"
         plt.savefig(img_path)
         fig.clear()
         plt.close(fig)
         plt.savefig(img_path)
         plt.close(fig)
         glob_conf.report.add_item(
             ReportItem(
@@ -224,22 +225,25 @@
         res_dir = self.util.get_path("res_dir")
         rpt = (
             f"epoch: {epoch}, UAR: {uar_str}"
             + f", (+-{up_str}/{low_str}), ACC: {acc_str}"
         )
         # print(rpt)
         self.util.debug(rpt)
-        file_name = f"{res_dir}{self.util.get_exp_name()}_conf.txt"
+        file_name = f"{res_dir}{self.util.get_exp_name()}{self.filenameadd}_conf.txt"
         with open(file_name, "w") as text_file:
             text_file.write(rpt)
 
+    def set_filename_add(self, my_string):
+        self.filenameadd = f"_{my_string}"
+
     def print_results(self, epoch):
         """Print all evaluation values to text file."""
         res_dir = self.util.get_path("res_dir")
-        file_name = f"{res_dir}{self.util.get_exp_name()}_{epoch}.txt"
+        file_name = f"{res_dir}{self.util.get_exp_name()}_{epoch}{self.filenameadd}.txt"
         if self.util.exp_is_classification():
             labels = glob_conf.labels
             try:
                 rpt = classification_report(
                     self.truths,
                     self.preds,
                     target_names=labels,
```

### Comparing `nkululeko-0.82.4/nkululeko/reporting/result.py` & `nkululeko-0.83.0/nkululeko/reporting/result.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/resample.py` & `nkululeko-0.83.0/nkululeko/resample.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/runmanager.py` & `nkululeko-0.83.0/nkululeko/runmanager.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/scaler.py` & `nkululeko-0.83.0/nkululeko/scaler.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/segment.py` & `nkululeko-0.83.0/nkululeko/segment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/segmenting/seg_inaspeechsegmenter.py` & `nkululeko-0.83.0/nkululeko/segmenting/seg_inaspeechsegmenter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/segmenting/seg_silero.py` & `nkululeko-0.83.0/nkululeko/segmenting/seg_silero.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/syllable_nuclei.py` & `nkululeko-0.83.0/nkululeko/syllable_nuclei.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/test.py` & `nkululeko-0.83.0/nkululeko/test.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/test_predictor.py` & `nkululeko-0.83.0/nkululeko/test_predictor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,29 @@
-""" test_predictor.py
+"""test_predictor.py.
+
     Predict targets from a model and save as csv file.
 
 """
 
-import nkululeko.glob_conf as glob_conf
-from nkululeko.utils.util import Util
+import ast
+
+import numpy as np
 import pandas as pd
+from sklearn.preprocessing import LabelEncoder
+
 from nkululeko.data.dataset import Dataset
 from nkululeko.feature_extractor import FeatureExtractor
+import nkululeko.glob_conf as glob_conf
 from nkululeko.scaler import Scaler
-import numpy as np
-from sklearn.preprocessing import LabelEncoder
+from nkululeko.utils.util import Util
 
 
-class Test_predictor:
+class TestPredictor:
     def __init__(self, model, orig_df, labenc, name):
-        """Constructor setting up name and configuration"""
+        """Constructor setting up name and configuration."""
         self.model = model
         self.orig_df = orig_df
         self.label_encoder = labenc
         self.target = glob_conf.config["DATA"]["target"]
         self.util = Util("test_predictor")
         self.name = name
 
@@ -45,15 +49,22 @@
             predictions = self.model.get_predictions()
             df = pd.DataFrame(index=data_df.index)
             df["speaker"] = data_df["speaker"]
             df["gender"] = data_df["gender"]
             df[self.target] = labelenc.inverse_transform(predictions.tolist())
             df.to_csv(self.name)
         else:
+            test_dbs = ast.literal_eval(glob_conf.config["DATA"]["tests"])
+            test_dbs_string = "_".join(test_dbs)
             predictions = self.model.get_predictions()
+            report = self.model.predict()
+            report.set_filename_add(f"test-{test_dbs_string}")
+            self.util.print_best_results([report])
+            report.plot_confmatrix(self.util.get_plot_name(), 0)
+            report.print_results(0)
             # print(predictions)
             # df = pd.DataFrame(index=self.orig_df.index)
             # df["speaker"] = self.orig_df["speaker"]
             # df["gender"] = self.orig_df["gender"]
             # df[self.target] = self.orig_df[self.target]
             df = self.orig_df.copy()
             df["predictions"] = self.label_encoder.inverse_transform(predictions)
```

### Comparing `nkululeko-0.82.4/nkululeko/utils/files.py` & `nkululeko-0.83.0/nkululeko/utils/files.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/utils/stats.py` & `nkululeko-0.83.0/nkululeko/utils/stats.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko/utils/util.py` & `nkululeko-0.83.0/nkululeko/utils/util.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/nkululeko.egg-info/PKG-INFO` & `nkululeko-0.83.0/nkululeko.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.82.4
+Version: 0.83.0
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -329,14 +329,18 @@
    year = {2022},
 }
 ```
 
 Changelog
 =========
 
+Version 0.83.0
+--------------
+* test module now prints out reports
+
 Version 0.82.4
 --------------
 * fixed bug in wavlm 
 
 Version 0.82.3
 --------------
 * fixed another audformat peculiarity to interprete time values as nanoseconds
```

### Comparing `nkululeko-0.82.4/nkululeko.egg-info/SOURCES.txt` & `nkululeko-0.83.0/nkululeko.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/setup.cfg` & `nkululeko-0.83.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `nkululeko-0.82.4/venv/bin/activate_this.py` & `nkululeko-0.83.0/venv/bin/activate_this.py`

 * *Files identical despite different names*

