# Comparing `tmp/kailo-beewell-dashboard-0.3.3.tar.gz` & `tmp/kailo-beewell-dashboard-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kailo-beewell-dashboard-0.3.3.tar", last modified: Tue Apr 16 14:30:56 2024, max compression
+gzip compressed data, was "kailo-beewell-dashboard-0.3.4.tar", last modified: Thu Apr 25 14:18:44 2024, max compression
```

## Comparing `kailo-beewell-dashboard-0.3.3.tar` & `kailo-beewell-dashboard-0.3.4.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 ellengoddard   (501) staff       (20)        0 2024-04-16 14:30:56.379128 kailo-beewell-dashboard-0.3.3/
--rw-r--r--   0 ellengoddard   (501) staff       (20)     1070 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/LICENSE
--rw-r--r--   0 ellengoddard   (501) staff       (20)      158 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/MANIFEST.in
--rw-r--r--   0 ellengoddard   (501) staff       (20)     2744 2024-04-16 14:30:56.378890 kailo-beewell-dashboard-0.3.3/PKG-INFO
--rw-r--r--   0 ellengoddard   (501) staff       (20)     1631 2024-04-16 14:23:31.000000 kailo-beewell-dashboard-0.3.3/README.md
-drwxr-xr-x   0 ellengoddard   (501) staff       (20)        0 2024-04-16 14:30:56.323499 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/
--rw-r--r--   0 ellengoddard   (501) staff       (20)      169 2024-04-16 14:23:31.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/__init__.py
--rw-r--r--   0 ellengoddard   (501) staff       (20)     6521 2024-04-16 14:23:31.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/about_page.py
--rw-r--r--   0 ellengoddard   (501) staff       (20)     3939 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/authentication.py
--rw-r--r--   0 ellengoddard   (501) staff       (20)    15122 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/bar_charts.py
--rw-r--r--   0 ellengoddard   (501) staff       (20)     6242 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/bar_charts_text.py
-drwxr-xr-x   0 ellengoddard   (501) staff       (20)        0 2024-04-16 14:30:56.324589 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/css/
--rw-r--r--   0 ellengoddard   (501) staff       (20)     1802 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/css/static_report_style.css
--rw-r--r--   0 ellengoddard   (501) staff       (20)     3223 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/css/style.css
--rw-r--r--   0 ellengoddard   (501) staff       (20)    25957 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/explore_results.py
--rw-r--r--   0 ellengoddard   (501) staff       (20)      557 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/grammar.py
-drwxr-xr-x   0 ellengoddard   (501) staff       (20)        0 2024-04-16 14:30:56.341757 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/
--rw-r--r--   0 ellengoddard   (501) staff       (20)    61702 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/beewell_map.png
--rw-r--r--   0 ellengoddard   (501) staff       (20)   185745 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/canva_people.png
--rw-r--r--   0 ellengoddard   (501) staff       (20)    48221 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/circle_divider.png
--rw-r--r--   0 ellengoddard   (501) staff       (20)    72751 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/dashboard_home_section.png
--rw-r--r--   0 ellengoddard   (501) staff       (20)    31928 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/devices.png
--rw-r--r--   0 ellengoddard   (501) staff       (20)   550917 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/discovery-looking-researching.jpg
--rw-r--r--   0 ellengoddard   (501) staff       (20)   258283 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/home_image_3_transparent.png
--rw-r--r--   0 ellengoddard   (501) staff       (20)    92545 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/kailo_beewell_logo.png
--rw-r--r--   0 ellengoddard   (501) staff       (20)    93979 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/kailo_beewell_logo_padded.png
--rw-r--r--   0 ellengoddard   (501) staff       (20)    88360 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/kailo_systems_adapted.png
--rw-r--r--   0 ellengoddard   (501) staff       (20)   564177 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/levelling-the-ground.jpg
--rw-r--r--   0 ellengoddard   (501) staff       (20)    21040 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/northern_devon.png
-drwxr-xr-x   0 ellengoddard   (501) staff       (20)        0 2024-04-16 14:30:56.377186 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/
--rw-r--r--   0 ellengoddard   (501) staff       (20)   180897 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/choice.png
--rw-r--r--   0 ellengoddard   (501) staff       (20)   155419 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/choice_crop.png
--rw-r--r--   0 ellengoddard   (501) staff       (20)    23923 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/choose_one.png
--rw-r--r--   0 ellengoddard   (501) staff       (20)   131754 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/family.png
--rw-r--r--   0 ellengoddard   (501) staff       (20)   106617 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/family_crop.png
--rw-r--r--   0 ellengoddard   (501) staff       (20)   127520 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/free_time.png
--rw-r--r--   0 ellengoddard   (501) staff       (20)   102391 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/free_time_crop.png
--rw-r--r--   0 ellengoddard   (501) staff       (20)   129719 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/friends.png
--rw-r--r--   0 ellengoddard   (501) staff       (20)   104548 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/friends_crop.png
--rw-r--r--   0 ellengoddard   (501) staff       (20)   123168 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/future.png
--rw-r--r--   0 ellengoddard   (501) staff       (20)    98588 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/future_crop.png
--rw-r--r--   0 ellengoddard   (501) staff       (20)    21352 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/happy.png
--rw-r--r--   0 ellengoddard   (501) staff       (20)   108174 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/health.png
--rw-r--r--   0 ellengoddard   (501) staff       (20)    82741 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/health_crop.png
--rw-r--r--   0 ellengoddard   (501) staff       (20)   120585 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/home.png
--rw-r--r--   0 ellengoddard   (501) staff       (20)    95604 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/home_crop.png
--rw-r--r--   0 ellengoddard   (501) staff       (20)   121744 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/life.png
--rw-r--r--   0 ellengoddard   (501) staff       (20)    96996 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/life_crop.png
--rw-r--r--   0 ellengoddard   (501) staff       (20)    16076 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/ok.png
--rw-r--r--   0 ellengoddard   (501) staff       (20)    19823 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/sad.png
--rw-r--r--   0 ellengoddard   (501) staff       (20)   121199 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/school.png
--rw-r--r--   0 ellengoddard   (501) staff       (20)    96276 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/school_crop.png
--rw-r--r--   0 ellengoddard   (501) staff       (20)   156249 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/things.png
--rw-r--r--   0 ellengoddard   (501) staff       (20)   131030 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/things_crop.png
--rw-r--r--   0 ellengoddard   (501) staff       (20)    85100 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/thinking.png
--rw-r--r--   0 ellengoddard   (501) staff       (20)   475730 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/young-person-journey.jpg
--rw-r--r--   0 ellengoddard   (501) staff       (20)     1767 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images.py
--rw-r--r--   0 ellengoddard   (501) staff       (20)     4418 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/import_data.py
--rw-r--r--   0 ellengoddard   (501) staff       (20)     1843 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/map.py
--rw-r--r--   0 ellengoddard   (501) staff       (20)     2503 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/page_setup.py
--rw-r--r--   0 ellengoddard   (501) staff       (20)     6853 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/reshape_data.py
--rw-r--r--   0 ellengoddard   (501) staff       (20)    14456 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/response_labels.py
--rw-r--r--   0 ellengoddard   (501) staff       (20)    13118 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/reuse_text.py
--rw-r--r--   0 ellengoddard   (501) staff       (20)     2723 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/score_descriptions.py
--rw-r--r--   0 ellengoddard   (501) staff       (20)    13596 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/static_report.py
--rw-r--r--   0 ellengoddard   (501) staff       (20)     2297 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/stylable_container.py
--rw-r--r--   0 ellengoddard   (501) staff       (20)    12744 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/summary_rag.py
--rw-r--r--   0 ellengoddard   (501) staff       (20)     1077 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/switch_page_button.py
--rw-r--r--   0 ellengoddard   (501) staff       (20)    14229 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/synthesise_aggregate.py
--rw-r--r--   0 ellengoddard   (501) staff       (20)     3553 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/synthesise_demographic.py
--rw-r--r--   0 ellengoddard   (501) staff       (20)    19646 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/synthesise_responses.py
--rw-r--r--   0 ellengoddard   (501) staff       (20)    14885 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/synthesise_scores.py
--rw-r--r--   0 ellengoddard   (501) staff       (20)     3935 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/topic_labels.py
--rw-r--r--   0 ellengoddard   (501) staff       (20)     7968 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/who_took_part.py
-drwxr-xr-x   0 ellengoddard   (501) staff       (20)        0 2024-04-16 14:30:56.378570 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard.egg-info/
--rw-r--r--   0 ellengoddard   (501) staff       (20)     2744 2024-04-16 14:30:56.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard.egg-info/PKG-INFO
--rw-r--r--   0 ellengoddard   (501) staff       (20)     3561 2024-04-16 14:30:56.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard.egg-info/SOURCES.txt
--rw-r--r--   0 ellengoddard   (501) staff       (20)        1 2024-04-16 14:30:56.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard.egg-info/dependency_links.txt
--rw-r--r--   0 ellengoddard   (501) staff       (20)      308 2024-04-16 14:30:56.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard.egg-info/requires.txt
--rw-r--r--   0 ellengoddard   (501) staff       (20)       24 2024-04-16 14:30:56.000000 kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard.egg-info/top_level.txt
--rw-r--r--   0 ellengoddard   (501) staff       (20)      675 2024-04-16 14:30:27.000000 kailo-beewell-dashboard-0.3.3/pyproject.toml
--rw-r--r--   0 ellengoddard   (501) staff       (20)      728 2024-04-16 14:30:05.000000 kailo-beewell-dashboard-0.3.3/requirements.txt
--rw-r--r--   0 ellengoddard   (501) staff       (20)       38 2024-04-16 14:30:56.379181 kailo-beewell-dashboard-0.3.3/setup.cfg
--rw-r--r--   0 ellengoddard   (501) staff       (20)     1167 2024-04-16 12:15:41.000000 kailo-beewell-dashboard-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 14:18:44.973140 kailo-beewell-dashboard-0.3.4/
+-rw-rw-rw-   0        0        0     1091 2024-04-18 12:45:26.000000 kailo-beewell-dashboard-0.3.4/LICENSE
+-rw-rw-rw-   0        0        0      161 2024-04-18 12:45:26.000000 kailo-beewell-dashboard-0.3.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2854 2024-04-25 14:18:44.969529 kailo-beewell-dashboard-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1707 2024-04-25 13:49:01.000000 kailo-beewell-dashboard-0.3.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 14:18:44.507722 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/
+-rw-rw-rw-   0        0        0      199 2024-04-25 13:49:01.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/__init__.py
+-rw-rw-rw-   0        0        0     6712 2024-04-25 13:49:01.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/about_page.py
+-rw-rw-rw-   0        0        0     4065 2024-04-18 12:45:26.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/authentication.py
+-rw-rw-rw-   0        0        0    15486 2024-04-18 12:45:26.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/bar_charts.py
+-rw-rw-rw-   0        0        0     6442 2024-04-18 12:45:26.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/bar_charts_text.py
+drwxrwxrwx   0        0        0        0 2024-04-25 14:18:44.582584 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/css/
+-rw-rw-rw-   0        0        0     1898 2024-04-18 12:45:26.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/css/static_report_style.css
+-rw-rw-rw-   0        0        0     3372 2024-04-18 12:45:26.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/css/style.css
+-rw-rw-rw-   0        0        0    26660 2024-04-18 12:45:26.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/explore_results.py
+-rw-rw-rw-   0        0        0      583 2024-04-18 12:45:26.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/grammar.py
+drwxrwxrwx   0        0        0        0 2024-04-25 14:18:44.699160 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/
+-rw-rw-rw-   0        0        0    61702 2024-04-18 12:45:26.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/beewell_map.png
+-rw-rw-rw-   0        0        0   185745 2024-04-18 12:45:26.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/canva_people.png
+-rw-rw-rw-   0        0        0    48221 2024-04-18 12:45:26.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/circle_divider.png
+-rw-rw-rw-   0        0        0    72751 2024-04-18 12:45:26.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/dashboard_home_section.png
+-rw-rw-rw-   0        0        0    31928 2024-04-18 12:45:26.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/devices.png
+-rw-rw-rw-   0        0        0   550917 2024-04-18 12:45:26.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/discovery-looking-researching.jpg
+-rw-rw-rw-   0        0        0   258283 2024-04-18 12:45:26.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/home_image_3_transparent.png
+-rw-rw-rw-   0        0        0    92545 2024-04-18 12:45:26.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/kailo_beewell_logo.png
+-rw-rw-rw-   0        0        0    93979 2024-04-18 12:45:26.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/kailo_beewell_logo_padded.png
+-rw-rw-rw-   0        0        0    88360 2024-04-18 12:45:26.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/kailo_systems_adapted.png
+-rw-rw-rw-   0        0        0   564177 2024-04-18 12:45:26.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/levelling-the-ground.jpg
+-rw-rw-rw-   0        0        0    21040 2024-04-18 12:45:26.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/northern_devon.png
+drwxrwxrwx   0        0        0        0 2024-04-25 14:18:44.959020 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/
+-rw-rw-rw-   0        0        0   180897 2024-04-18 12:45:26.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/choice.png
+-rw-rw-rw-   0        0        0   155419 2024-04-18 12:45:26.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/choice_crop.png
+-rw-rw-rw-   0        0        0    23923 2024-04-18 12:45:26.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/choose_one.png
+-rw-rw-rw-   0        0        0   131754 2024-04-18 12:45:26.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/family.png
+-rw-rw-rw-   0        0        0   106617 2024-04-18 12:45:26.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/family_crop.png
+-rw-rw-rw-   0        0        0   127520 2024-04-18 12:45:26.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/free_time.png
+-rw-rw-rw-   0        0        0   102391 2024-04-18 12:45:26.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/free_time_crop.png
+-rw-rw-rw-   0        0        0   129719 2024-04-18 12:45:26.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/friends.png
+-rw-rw-rw-   0        0        0   104548 2024-04-18 12:45:26.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/friends_crop.png
+-rw-rw-rw-   0        0        0   123168 2024-04-18 12:45:26.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/future.png
+-rw-rw-rw-   0        0        0    98588 2024-04-18 12:45:26.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/future_crop.png
+-rw-rw-rw-   0        0        0    21352 2024-04-18 12:45:26.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/happy.png
+-rw-rw-rw-   0        0        0   108174 2024-04-18 12:45:26.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/health.png
+-rw-rw-rw-   0        0        0    82741 2024-04-18 12:45:26.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/health_crop.png
+-rw-rw-rw-   0        0        0   120585 2024-04-18 12:45:26.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/home.png
+-rw-rw-rw-   0        0        0    95604 2024-04-18 12:45:26.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/home_crop.png
+-rw-rw-rw-   0        0        0   121744 2024-04-18 12:45:27.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/life.png
+-rw-rw-rw-   0        0        0    96996 2024-04-18 12:45:27.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/life_crop.png
+-rw-rw-rw-   0        0        0    16076 2024-04-18 12:45:27.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/ok.png
+-rw-rw-rw-   0        0        0    19823 2024-04-18 12:45:27.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/sad.png
+-rw-rw-rw-   0        0        0   121199 2024-04-18 12:45:27.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/school.png
+-rw-rw-rw-   0        0        0    96276 2024-04-18 12:45:27.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/school_crop.png
+-rw-rw-rw-   0        0        0   156249 2024-04-18 12:45:27.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/things.png
+-rw-rw-rw-   0        0        0   131030 2024-04-18 12:45:27.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/things_crop.png
+-rw-rw-rw-   0        0        0    85100 2024-04-18 12:45:27.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/thinking.png
+-rw-rw-rw-   0        0        0   475730 2024-04-18 12:45:27.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/young-person-journey.jpg
+-rw-rw-rw-   0        0        0     1831 2024-04-18 12:45:26.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images.py
+-rw-rw-rw-   0        0        0     4532 2024-04-18 12:45:27.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/import_data.py
+-rw-rw-rw-   0        0        0     1892 2024-04-18 12:45:27.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/map.py
+-rw-rw-rw-   0        0        0     2597 2024-04-18 12:45:27.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/page_setup.py
+-rw-rw-rw-   0        0        0     7045 2024-04-18 12:45:27.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/reshape_data.py
+-rw-rw-rw-   0        0        0    14959 2024-04-18 12:45:27.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/response_labels.py
+-rw-rw-rw-   0        0        0    13381 2024-04-18 12:45:27.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/reuse_text.py
+-rw-rw-rw-   0        0        0     2779 2024-04-18 12:45:27.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/score_descriptions.py
+-rw-rw-rw-   0        0        0    14022 2024-04-18 12:45:27.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/static_report.py
+-rw-rw-rw-   0        0        0     2372 2024-04-18 12:45:27.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/stylable_container.py
+-rw-rw-rw-   0        0        0    13113 2024-04-18 12:45:27.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/summary_rag.py
+-rw-rw-rw-   0        0        0     1116 2024-04-18 12:45:27.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/switch_page_button.py
+-rw-rw-rw-   0        0        0    14611 2024-04-18 12:45:27.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/synthesise_aggregate.py
+-rw-rw-rw-   0        0        0     3651 2024-04-18 12:45:27.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/synthesise_demographic.py
+-rw-rw-rw-   0        0        0    20162 2024-04-18 12:45:27.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/synthesise_responses.py
+-rw-rw-rw-   0        0        0    15260 2024-04-18 12:45:27.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/synthesise_scores.py
+-rw-rw-rw-   0        0        0     4036 2024-04-18 12:45:27.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/topic_labels.py
+-rw-rw-rw-   0        0        0     8174 2024-04-18 12:45:27.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/who_took_part.py
+drwxrwxrwx   0        0        0        0 2024-04-25 14:18:44.964506 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard.egg-info/
+-rw-rw-rw-   0        0        0     2854 2024-04-25 14:18:43.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3561 2024-04-25 14:18:43.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 14:18:43.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      308 2024-04-25 14:18:43.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-04-25 14:18:43.000000 kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      708 2024-04-18 12:45:27.000000 kailo-beewell-dashboard-0.3.4/pyproject.toml
+-rw-rw-rw-   0        0        0      773 2024-04-18 12:45:27.000000 kailo-beewell-dashboard-0.3.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 14:18:44.974124 kailo-beewell-dashboard-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     1202 2024-04-18 12:45:27.000000 kailo-beewell-dashboard-0.3.4/setup.py
```

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/authentication.py` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/authentication.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,126 +1,126 @@
-'''
-Helper functions for user authentication
-'''
-import streamlit as st
-import os
-from django.core.wsgi import get_wsgi_application
-from django.contrib.auth import authenticate
-
-os.environ.setdefault('DJANGO_SETTINGS_MODULE', 'config.settings')
-application = get_wsgi_application()
-
-
-def get_school(username):
-    '''
-    Finds the school based on the username
-
-    Parameters
-    ----------
-    username : string
-        Django username
-    '''
-    schools = {
-        'schoola': 'School A',
-        'schoolb': 'School B',
-        'schoolc': 'School C',
-        'schoold': 'School D',
-        'schoole': 'School E',
-        'schoolf': 'School F'
-    }
-    return schools[username]
-
-
-def password_entered():
-    '''
-    Checks whether a password entered by the user is correct
-    '''
-    # Use Django to check if the username and password match record
-    user = authenticate(
-        username=st.session_state['username'],
-        password=st.session_state['password']
-        )
-    # If this succeeds, delete the username and password, and keep record
-    # of the user and school in the session state
-    if user is not None:
-        st.session_state['password_correct'] = True
-        del st.session_state['password']
-        del st.session_state['username']
-        st.session_state.user = user
-        st.session_state['school'] = get_school(str(user))
-    else:
-        st.session_state['password_correct'] = False
-
-
-def login_screen(survey_type):
-    '''
-    Produces message that is displayed on the login screen.
-
-    Parameters
-    ----------
-    survey_type : string
-        Specifies whether this is for the 'standard' or 'symbol' survey.
-    '''
-    # Login screen title
-    st.title('The #BeeWell survey')
-
-    # Compose message, with content depending on dashboard
-    message = '''
-Please enter your school username and password to login to the dashboard.'''
-
-    if survey_type == 'standard':
-        message += '''
-
-For this synthetic dashboard, we have six schools - choose a username and
-password from the following:
-* '**schoola**' and '**schoolapassword**' - n<10 for some demographic responses
-* '**schoolb**' and '**schoolbpassword**' - no SEN
-* '**schoolc**' and '**schoolcpassword**'
-* '**schoold**' and '**schooldpassword**'
-* '**schoole**' and '**schoolepassword**'
-* '**schoolf**' and '**schoolfpassword**' - no Year 10s
-'''
-    elif survey_type == 'symbol':
-        message += '''
-
-For this synthetic dashboard, we have two schools - choose a username and
-password from the following:
-* '**schoola**' and '**schoolapassword**'
-* '**schoolb**' and '**schoolbpassword**'
-'''
-
-    # Print message onto the dashboard
-    st.markdown(message)
-
-
-def check_password(survey_type):
-    '''
-    Function that returns 'True' if the user has entered the correct password
-    Stores the user to the session state, and finds the school's full name,
-    and adds that to the session state as well.
-
-    Parameters
-    ----------
-    survey_type : string
-        Specifies whether this is for the 'standard' or 'symbol' survey.
-    '''
-    # If have not yet logged in...
-    if 'password_correct' not in st.session_state:
-        # Show inputs for username and password
-        login_screen(survey_type)
-        st.text_input('Username', key='username')
-        st.text_input('Password', type='password', key='password')
-        st.write('')
-        st.button(label='Enter', on_click=password_entered)
-        return False
-    elif not st.session_state['password_correct']:
-        # Password not correct, show input boxes again and an error message
-        login_screen(survey_type)
-        st.text_input('Username', key='username')
-        st.text_input('Password', type='password', key='password')
-        st.write('')
-        st.button(label='Enter', on_click=password_entered)
-        st.error('😕 User not known or password incorrect')
-        return False
-    else:
-        # Password correct.
-        return True
+'''
+Helper functions for user authentication
+'''
+import streamlit as st
+import os
+from django.core.wsgi import get_wsgi_application
+from django.contrib.auth import authenticate
+
+os.environ.setdefault('DJANGO_SETTINGS_MODULE', 'config.settings')
+application = get_wsgi_application()
+
+
+def get_school(username):
+    '''
+    Finds the school based on the username
+
+    Parameters
+    ----------
+    username : string
+        Django username
+    '''
+    schools = {
+        'schoola': 'School A',
+        'schoolb': 'School B',
+        'schoolc': 'School C',
+        'schoold': 'School D',
+        'schoole': 'School E',
+        'schoolf': 'School F'
+    }
+    return schools[username]
+
+
+def password_entered():
+    '''
+    Checks whether a password entered by the user is correct
+    '''
+    # Use Django to check if the username and password match record
+    user = authenticate(
+        username=st.session_state['username'],
+        password=st.session_state['password']
+        )
+    # If this succeeds, delete the username and password, and keep record
+    # of the user and school in the session state
+    if user is not None:
+        st.session_state['password_correct'] = True
+        del st.session_state['password']
+        del st.session_state['username']
+        st.session_state.user = user
+        st.session_state['school'] = get_school(str(user))
+    else:
+        st.session_state['password_correct'] = False
+
+
+def login_screen(survey_type):
+    '''
+    Produces message that is displayed on the login screen.
+
+    Parameters
+    ----------
+    survey_type : string
+        Specifies whether this is for the 'standard' or 'symbol' survey.
+    '''
+    # Login screen title
+    st.title('The #BeeWell survey')
+
+    # Compose message, with content depending on dashboard
+    message = '''
+Please enter your school username and password to login to the dashboard.'''
+
+    if survey_type == 'standard':
+        message += '''
+
+For this synthetic dashboard, we have six schools - choose a username and
+password from the following:
+* '**schoola**' and '**schoolapassword**' - n<10 for some demographic responses
+* '**schoolb**' and '**schoolbpassword**' - no SEN
+* '**schoolc**' and '**schoolcpassword**'
+* '**schoold**' and '**schooldpassword**'
+* '**schoole**' and '**schoolepassword**'
+* '**schoolf**' and '**schoolfpassword**' - no Year 10s
+'''
+    elif survey_type == 'symbol':
+        message += '''
+
+For this synthetic dashboard, we have two schools - choose a username and
+password from the following:
+* '**schoola**' and '**schoolapassword**'
+* '**schoolb**' and '**schoolbpassword**'
+'''
+
+    # Print message onto the dashboard
+    st.markdown(message)
+
+
+def check_password(survey_type):
+    '''
+    Function that returns 'True' if the user has entered the correct password
+    Stores the user to the session state, and finds the school's full name,
+    and adds that to the session state as well.
+
+    Parameters
+    ----------
+    survey_type : string
+        Specifies whether this is for the 'standard' or 'symbol' survey.
+    '''
+    # If have not yet logged in...
+    if 'password_correct' not in st.session_state:
+        # Show inputs for username and password
+        login_screen(survey_type)
+        st.text_input('Username', key='username')
+        st.text_input('Password', type='password', key='password')
+        st.write('')
+        st.button(label='Enter', on_click=password_entered)
+        return False
+    elif not st.session_state['password_correct']:
+        # Password not correct, show input boxes again and an error message
+        login_screen(survey_type)
+        st.text_input('Username', key='username')
+        st.text_input('Password', type='password', key='password')
+        st.write('')
+        st.button(label='Enter', on_click=password_entered)
+        st.error('😕 User not known or password incorrect')
+        return False
+    else:
+        # Password correct.
+        return True
```

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/bar_charts.py` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/bar_charts.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,364 +1,364 @@
-'''
-Functions used to produce the two types of bar chart
-'''
-from contextlib import nullcontext
-from markdown import markdown
-import numpy as np
-import plotly.express as px
-import streamlit as st
-from .images import convert_fig_to_html
-from .grammar import lower_first
-
-
-def create_group_list(drop, page='explore'):
-    '''
-    Creates list of the pupil groups who have been excluded as n<10. This is
-    provided as a seperation function as wanted to create string depending on
-    three use cases - with the example of year group...:
-    (1) 'Year 7' pupils
-    (2) 'Year 7 and Year 9' pupils
-    (3) 'Year 7, Year 8 and Year 9' pupils (or longer)
-
-    Parameters
-    ----------
-    drop : series
-        Contains the names of the groups that had less than 10 responses
-    page : string
-        Specifies whether this is for the 'explore' page or 'demographic' page.
-        Default is the 'explore' page.
-    '''
-    # Convert to list (if not already)
-    drop = drop.to_list()
-
-    # Convert first letter to lower case (unless all are upper case)
-    drop = [lower_first(item) for item in drop]
-
-    # Generate string with appropriate grammar
-    if len(drop) == 1:
-        string = drop[0]
-    elif len(drop) == 2:
-        string = f'{drop[0]} and {drop[1]}'
-    elif len(drop) >= 3:
-        string = f'''{drop[0]}, {', '.join(drop[1:-1])} and {drop[-1]}'''
-
-    # Add pupils with appropriate grammer
-    if page == 'explore':
-        string = f'{string} pupils'
-    elif page == 'demographic':
-        string = f'pupils at {string}'
-    return string
-
-
-def survey_responses(dataset, font_size=16, output='streamlit', content=None,
-                     page='explore'):
-    '''
-    Create bar charts for each of the questions in the provided dataframe.
-    The dataframe should contain questions which all have the same set
-    of possible responses.
-
-    Parameters
-    ----------
-    df : dataframe
-        Dataframe to create plot from (e.g. chosen_result)
-    font_size : integer
-        Font size of x axis labels, y axis labels and legend text, default=16
-    output : string
-        Use of function - either for streamlit page or PDF report
-        Must be either 'streamlit' or 'pdf, default is 'streamlit.
-    content : list
-        Optional input used when output=='pdf', contains HTML for report.
-    page : string
-        Specifies whether this is for the 'explore' page or 'demographic' page.
-        Default is the 'explore' page.
-
-    Returns
-    -------
-    content : list
-        Optional return, used when output=='pdf', contains HTML for report.
-    '''
-    # Create seperate figures for each of the measures
-    for measure in dataset['measure_lab'].drop_duplicates():
-
-        # Streamlit: Create containers to visually seperate plots
-        with (st.container(border=True) if output == 'streamlit'
-              else nullcontext()):
-
-            # PDF: Create empty list to store content for PDF
-            if output == 'pdf':
-                temp_content = []
-
-            # Streamlit and PDF: Create header for plot
-            # Don't use in-built plotly title as that overlaps the legend if it
-            # spans over 2 lines
-            if output == 'streamlit':
-                st.markdown(f'**{measure.lstrip()}**')
-            elif output == 'pdf':
-                temp_content.append(
-                    f'''<p style='margin:0;'><strong>{measure}</strong></p>''')
-
-            # Filter to the relevant measure
-            df = dataset[dataset['measure_lab'] == measure]
-
-            # Check if there are any groups where n<10 overall - if one of the
-            # groups are, remove it from dataframe and print explanation
-            mask = df['cat_lab'] == 'Less than 10 responses'
-            under_10 = df[mask]
-            # Remove group from dataframe for plotting
-            df = df[~mask]
-
-            # If there were some with n<10 but still some left to plot...
-            if len(under_10.index) > 0 and len(df.index) > 0:
-                # Create explanation
-                dropped = create_group_list(under_10['group'], page)
-                kept = create_group_list(df['group'].drop_duplicates(), page)
-                explanation = f'''
-There were less than 10 responses from {dropped} so results are just
-shown for {kept}.'''
-            # Else if all groups were removed and nothing left to plot...
-            elif len(df.index) == 0:
-                dropped = create_group_list(under_10['group'], page)
-                explanation = f'''
-There were less than 10 responses from {dropped}, so no results can
-be shown.'''
-
-            # Print explanation on page for the removal of n<10 overall
-            if (len(under_10.index) > 0) or (len(df.index) == 0):
-                if output == 'streamlit':
-                    st.markdown(explanation)
-                elif output == 'pdf':
-                    temp_content.append(f'<p>{explanation}</p>')
-
-            # Create plot if there was at least one group without NaN
-            if len(df.index) > 0:
-
-                # First, check for any individual categories censored due to
-                # n<10 (this is relevant to demographic page, the explore
-                # results page won't have any)
-                # If there are any rows with NaN...
-                null_mask = df['count'].isnull()
-                if sum(null_mask) > 0:
-                    # Filter to NaN rows and get the categories as a string
-                    dropped = df.loc[null_mask, ['cat_lab', 'group']]
-                    for school in dropped['group'].drop_duplicates():
-                        dropped_string = ', '.join(dropped.loc[
-                            dropped['group'] == school, 'cat_lab'].values)
-                        # Print explanation of this censoring
-                        explanation = f'''
-Due to small sample sizes, response rates are hidden for:
-
-* {school}: {dropped_string}'''
-                        if output == 'streamlit':
-                            st.markdown(explanation)
-                        elif output == 'pdf':
-                            temp_content.append(markdown(explanation))
-
-                # Create colour map
-                unique_groups = np.unique(df['group'])
-                if (len(unique_groups) == 1):
-                    colour_map = {unique_groups[0]: '#FF6E4A'}
-                else:
-                    colour_map = {unique_groups[0]: '#ffb49a',
-                                  unique_groups[1]: '#e05a38'}
-
-                # Create figure
-                fig = px.bar(
-                    df, x='cat_lab', y='percentage',
-                    # Set colours and grouping
-                    color='group', barmode='group',
-                    color_discrete_map=colour_map,
-                    # Label bars with the percentage to 1 decimal place
-                    text_auto='.1f',
-                    # Specify what to show when hover over the bars
-                    hover_data={
-                        'cat_lab': True,
-                        'percentage': ':.1f',
-                        'count': True,
-                        'measure_lab': False,
-                        'group': False})
-
-                # Set x axis to type category, else only shows integer
-                # categories if you have a mix of numbers and strings
-                fig.update_layout(xaxis_type='category')
-
-                # Add percent sign to the numbers labelling the bars
-                fig.for_each_trace(lambda t: t.update(
-                    texttemplate=t.texttemplate + ' %'))
-
-                # Choose survey or council label for y axis, based on tick for
-                # x axis ('no response' is survey, 'no data' is council)
-                if 'No response' in df['cat_lab'].values:
-                    yaxis_title = 'Percentage of pupils<br>providing response'
-                else:
-                    yaxis_title = 'Percentage of pupils'
-
-                # Make changes to figure design...
-                fig.update_layout(
-                    # Set font size of bar labels
-                    font=dict(size=font_size),
-                    # Set x axis title, labels, colour and size
-                    xaxis=dict(
-                        title='Response',
-                        tickfont=dict(color='#05291F', size=font_size),
-                        titlefont=dict(color='#05291F', size=font_size)),
-                    # Set y axis title, labels, colour and size
-                    yaxis=dict(
-                        title=yaxis_title,
-                        titlefont=dict(color='#05291F', size=font_size),
-                        tickfont=dict(color='#05291F', size=font_size),
-                        ticksuffix='%'
-                    ),
-                    # Legend title and labels and remove interactivity
-                    legend=dict(
-                        title='Pupils',
-                        font=dict(color='#05291F', size=font_size),
-                        itemclick=False, itemdoubleclick=False),
-                    # Legend title font
-                    legend_title=dict(
-                        font=dict(color='#05291F', size=font_size)))
-
-                # Disable zooming and panning
-                fig.layout.xaxis.fixedrange = True
-                fig.layout.yaxis.fixedrange = True
-
-                # Streamlit: Create plot on streamlit app, hiding the plotly
-                # settings bar
-                if output == 'streamlit':
-                    st.plotly_chart(fig, use_container_width=True,
-                                    config={'displayModeBar': False})
-
-                # PDF: Write image to a temporary PNG file, convert that
-                # to HTML, and add the image HTML to temp_content
-                elif output == 'pdf':
-                    # Make and add HTML image tag to temp_content
-                    temp_content.append(convert_fig_to_html(
-                        fig=fig, alt_text=measure))
-
-            # Insert temp_content into a div class and add to content
-            if output == 'pdf':
-                content.append(f'''
-<div class='responses_container'>
-{''.join(temp_content)}
-</div>''')
-
-    # At the end of the loop, if PDF report, return content
-    if output == 'pdf':
-        return content
-
-
-def details_ordered_bar(school_scores, school_name, font_size=16,
-                        output='streamlit', content=None):
-    '''
-    Created ordered bar chart with the results from each school, with the
-    chosen school highlighted
-
-    Parameters
-    ----------
-    school_scores : dataframe
-        Dataframe with mean score at each school (e.g. between_schools)
-    school_name : string
-        Name of school (matching name in 'school_lab' col)
-    font_size : integer
-        Font size of x axis labels, y axis labels and legend text, default=16
-    output : string
-        Use of function - either for streamlit page or PDF report
-        Must be either 'streamlit' or 'pdf, default is 'streamlit.
-    content : list
-        Optional input used when output=='pdf', contains HTML for report.
-
-    Returns
-    -------
-    content : list
-        Optional return, used when output=='pdf', contains HTML for report.
-    '''
-    # Make a copy of the school_scores df to work on (avoid SettingCopyWarning)
-    df = school_scores.copy()
-
-    # Add colour for bar based on school
-    df['colour'] = np.where(
-        df['school_lab'] == school_name, 'Your school', 'Other schools')
-
-    # Create column with mean rounded to 2 d.p.
-    df['Mean score'] = round(df['mean'], 2)
-
-    # Plot the results, specifying colours and hover data
-    fig = px.bar(
-        df, x='school_lab', y='mean', color='colour',
-        color_discrete_map={'Your school': '#5D98AB',
-                            'Other schools': '#BFD8E0'},
-        category_orders={'colour': ['Your school', 'Other schools']},
-        hover_data={'school_lab': False, 'colour': False,
-                    'mean': False, 'Mean score': True})
-
-    # Reorder x axis so in ascending order
-    fig.update_layout(xaxis={'categoryorder': 'total ascending'})
-
-    # Set y axis limits so the first and last bars of the chart a consistent
-    # height between different plots - find 15% of range and adjust the min
-    # and max by that
-    min = df['mean'].min()
-    max = df['mean'].max()
-    adj_axis = (max - min)*0.15
-    ymin = np.max([0, (min - adj_axis)])
-    ymax = max + adj_axis
-    fig.update_layout(yaxis_range=[ymin, ymax])
-
-    # Extract lower and upper rag boundaries amd shade the RAG areas
-    # (Colours used were matched to those from the summary page)
-    lower = df['lower'].to_list()[0]
-    upper = df['upper'].to_list()[0]
-    fig.add_hrect(
-        y0=ymin, y1=lower, fillcolor='#FFCCCC', layer='below',
-        line={'color': '#9A505B'}, line_width=0.5,
-        annotation_text='Below average', annotation_position='top left')
-    fig.add_hrect(
-        y0=lower, y1=upper, fillcolor='#FFE8BF', layer='below',
-        line={'color': '#B3852A'}, line_width=0.5,
-        annotation_text='Average', annotation_position='top left')
-    fig.add_hrect(
-        y0=upper, y1=ymax, fillcolor='#B6E6B6', layer='below',
-        line={'color': '#3A8461'}, line_width=0.5,
-        annotation_text='Above average', annotation_position='top left')
-
-    # Set font size and hide x axis tick labels (but seems to be a bug that
-    # means the axis label is then above the plot, so had to use a work around
-    # of replacing the axis labels with spaces
-    fig.update_layout(
-        font=dict(size=font_size),
-        xaxis=dict(title='Northern Devon schools<br>(ordered by mean score)',
-                   tickfont=dict(color='#05291F', size=font_size),
-                   titlefont=dict(color='#05291F', size=font_size),
-                   tickvals=df['school_lab'],
-                   ticktext=[' ']*len(df['school_lab'])),
-        yaxis=dict(title='Mean score',
-                   tickfont=dict(color='#05291F', size=font_size),
-                   titlefont=dict(color='#05291F', size=font_size)),
-        legend=dict(title='School',
-                    font=dict(color='#05291F', size=font_size),
-                    itemclick=False, itemdoubleclick=False),
-        legend_title=dict(font=dict(color='#05291F', size=font_size))
-    )
-
-    # Prevent zooming and panning, remove grid, and hide plotly toolbar
-    fig.layout.xaxis.fixedrange = True
-    fig.layout.yaxis.fixedrange = True
-    fig.update_yaxes(showgrid=False)
-
-    if output == 'streamlit':
-        st.plotly_chart(fig, use_container_width=True,
-                        config={'displayModeBar': False})
-    elif output == 'pdf':
-        # Create temporary list to hold image HTML
-        temp_content = []
-
-        # Get the HTML image tag for the figure and add to temp_content
-        temp_content.append(convert_fig_to_html(
-            fig=fig, alt_text='Comparison with other schools'))
-
-        # Insert temp_content into a div class and add to content
-        content.append(f'''
-<div class='comparison_container'>
-    {''.join(temp_content)}
-</div>''')
-
-        # Return the updated content HTML
-        return content
+'''
+Functions used to produce the two types of bar chart
+'''
+from contextlib import nullcontext
+from markdown import markdown
+import numpy as np
+import plotly.express as px
+import streamlit as st
+from .images import convert_fig_to_html
+from .grammar import lower_first
+
+
+def create_group_list(drop, page='explore'):
+    '''
+    Creates list of the pupil groups who have been excluded as n<10. This is
+    provided as a seperation function as wanted to create string depending on
+    three use cases - with the example of year group...:
+    (1) 'Year 7' pupils
+    (2) 'Year 7 and Year 9' pupils
+    (3) 'Year 7, Year 8 and Year 9' pupils (or longer)
+
+    Parameters
+    ----------
+    drop : series
+        Contains the names of the groups that had less than 10 responses
+    page : string
+        Specifies whether this is for the 'explore' page or 'demographic' page.
+        Default is the 'explore' page.
+    '''
+    # Convert to list (if not already)
+    drop = drop.to_list()
+
+    # Convert first letter to lower case (unless all are upper case)
+    drop = [lower_first(item) for item in drop]
+
+    # Generate string with appropriate grammar
+    if len(drop) == 1:
+        string = drop[0]
+    elif len(drop) == 2:
+        string = f'{drop[0]} and {drop[1]}'
+    elif len(drop) >= 3:
+        string = f'''{drop[0]}, {', '.join(drop[1:-1])} and {drop[-1]}'''
+
+    # Add pupils with appropriate grammer
+    if page == 'explore':
+        string = f'{string} pupils'
+    elif page == 'demographic':
+        string = f'pupils at {string}'
+    return string
+
+
+def survey_responses(dataset, font_size=16, output='streamlit', content=None,
+                     page='explore'):
+    '''
+    Create bar charts for each of the questions in the provided dataframe.
+    The dataframe should contain questions which all have the same set
+    of possible responses.
+
+    Parameters
+    ----------
+    df : dataframe
+        Dataframe to create plot from (e.g. chosen_result)
+    font_size : integer
+        Font size of x axis labels, y axis labels and legend text, default=16
+    output : string
+        Use of function - either for streamlit page or PDF report
+        Must be either 'streamlit' or 'pdf, default is 'streamlit.
+    content : list
+        Optional input used when output=='pdf', contains HTML for report.
+    page : string
+        Specifies whether this is for the 'explore' page or 'demographic' page.
+        Default is the 'explore' page.
+
+    Returns
+    -------
+    content : list
+        Optional return, used when output=='pdf', contains HTML for report.
+    '''
+    # Create seperate figures for each of the measures
+    for measure in dataset['measure_lab'].drop_duplicates():
+
+        # Streamlit: Create containers to visually seperate plots
+        with (st.container(border=True) if output == 'streamlit'
+              else nullcontext()):
+
+            # PDF: Create empty list to store content for PDF
+            if output == 'pdf':
+                temp_content = []
+
+            # Streamlit and PDF: Create header for plot
+            # Don't use in-built plotly title as that overlaps the legend if it
+            # spans over 2 lines
+            if output == 'streamlit':
+                st.markdown(f'**{measure.lstrip()}**')
+            elif output == 'pdf':
+                temp_content.append(
+                    f'''<p style='margin:0;'><strong>{measure}</strong></p>''')
+
+            # Filter to the relevant measure
+            df = dataset[dataset['measure_lab'] == measure]
+
+            # Check if there are any groups where n<10 overall - if one of the
+            # groups are, remove it from dataframe and print explanation
+            mask = df['cat_lab'] == 'Less than 10 responses'
+            under_10 = df[mask]
+            # Remove group from dataframe for plotting
+            df = df[~mask]
+
+            # If there were some with n<10 but still some left to plot...
+            if len(under_10.index) > 0 and len(df.index) > 0:
+                # Create explanation
+                dropped = create_group_list(under_10['group'], page)
+                kept = create_group_list(df['group'].drop_duplicates(), page)
+                explanation = f'''
+There were less than 10 responses from {dropped} so results are just
+shown for {kept}.'''
+            # Else if all groups were removed and nothing left to plot...
+            elif len(df.index) == 0:
+                dropped = create_group_list(under_10['group'], page)
+                explanation = f'''
+There were less than 10 responses from {dropped}, so no results can
+be shown.'''
+
+            # Print explanation on page for the removal of n<10 overall
+            if (len(under_10.index) > 0) or (len(df.index) == 0):
+                if output == 'streamlit':
+                    st.markdown(explanation)
+                elif output == 'pdf':
+                    temp_content.append(f'<p>{explanation}</p>')
+
+            # Create plot if there was at least one group without NaN
+            if len(df.index) > 0:
+
+                # First, check for any individual categories censored due to
+                # n<10 (this is relevant to demographic page, the explore
+                # results page won't have any)
+                # If there are any rows with NaN...
+                null_mask = df['count'].isnull()
+                if sum(null_mask) > 0:
+                    # Filter to NaN rows and get the categories as a string
+                    dropped = df.loc[null_mask, ['cat_lab', 'group']]
+                    for school in dropped['group'].drop_duplicates():
+                        dropped_string = ', '.join(dropped.loc[
+                            dropped['group'] == school, 'cat_lab'].values)
+                        # Print explanation of this censoring
+                        explanation = f'''
+Due to small sample sizes, response rates are hidden for:
+
+* {school}: {dropped_string}'''
+                        if output == 'streamlit':
+                            st.markdown(explanation)
+                        elif output == 'pdf':
+                            temp_content.append(markdown(explanation))
+
+                # Create colour map
+                unique_groups = np.unique(df['group'])
+                if (len(unique_groups) == 1):
+                    colour_map = {unique_groups[0]: '#FF6E4A'}
+                else:
+                    colour_map = {unique_groups[0]: '#ffb49a',
+                                  unique_groups[1]: '#e05a38'}
+
+                # Create figure
+                fig = px.bar(
+                    df, x='cat_lab', y='percentage',
+                    # Set colours and grouping
+                    color='group', barmode='group',
+                    color_discrete_map=colour_map,
+                    # Label bars with the percentage to 1 decimal place
+                    text_auto='.1f',
+                    # Specify what to show when hover over the bars
+                    hover_data={
+                        'cat_lab': True,
+                        'percentage': ':.1f',
+                        'count': True,
+                        'measure_lab': False,
+                        'group': False})
+
+                # Set x axis to type category, else only shows integer
+                # categories if you have a mix of numbers and strings
+                fig.update_layout(xaxis_type='category')
+
+                # Add percent sign to the numbers labelling the bars
+                fig.for_each_trace(lambda t: t.update(
+                    texttemplate=t.texttemplate + ' %'))
+
+                # Choose survey or council label for y axis, based on tick for
+                # x axis ('no response' is survey, 'no data' is council)
+                if 'No response' in df['cat_lab'].values:
+                    yaxis_title = 'Percentage of pupils<br>providing response'
+                else:
+                    yaxis_title = 'Percentage of pupils'
+
+                # Make changes to figure design...
+                fig.update_layout(
+                    # Set font size of bar labels
+                    font=dict(size=font_size),
+                    # Set x axis title, labels, colour and size
+                    xaxis=dict(
+                        title='Response',
+                        tickfont=dict(color='#05291F', size=font_size),
+                        titlefont=dict(color='#05291F', size=font_size)),
+                    # Set y axis title, labels, colour and size
+                    yaxis=dict(
+                        title=yaxis_title,
+                        titlefont=dict(color='#05291F', size=font_size),
+                        tickfont=dict(color='#05291F', size=font_size),
+                        ticksuffix='%'
+                    ),
+                    # Legend title and labels and remove interactivity
+                    legend=dict(
+                        title='Pupils',
+                        font=dict(color='#05291F', size=font_size),
+                        itemclick=False, itemdoubleclick=False),
+                    # Legend title font
+                    legend_title=dict(
+                        font=dict(color='#05291F', size=font_size)))
+
+                # Disable zooming and panning
+                fig.layout.xaxis.fixedrange = True
+                fig.layout.yaxis.fixedrange = True
+
+                # Streamlit: Create plot on streamlit app, hiding the plotly
+                # settings bar
+                if output == 'streamlit':
+                    st.plotly_chart(fig, use_container_width=True,
+                                    config={'displayModeBar': False})
+
+                # PDF: Write image to a temporary PNG file, convert that
+                # to HTML, and add the image HTML to temp_content
+                elif output == 'pdf':
+                    # Make and add HTML image tag to temp_content
+                    temp_content.append(convert_fig_to_html(
+                        fig=fig, alt_text=measure))
+
+            # Insert temp_content into a div class and add to content
+            if output == 'pdf':
+                content.append(f'''
+<div class='responses_container'>
+{''.join(temp_content)}
+</div>''')
+
+    # At the end of the loop, if PDF report, return content
+    if output == 'pdf':
+        return content
+
+
+def details_ordered_bar(school_scores, school_name, font_size=16,
+                        output='streamlit', content=None):
+    '''
+    Created ordered bar chart with the results from each school, with the
+    chosen school highlighted
+
+    Parameters
+    ----------
+    school_scores : dataframe
+        Dataframe with mean score at each school (e.g. between_schools)
+    school_name : string
+        Name of school (matching name in 'school_lab' col)
+    font_size : integer
+        Font size of x axis labels, y axis labels and legend text, default=16
+    output : string
+        Use of function - either for streamlit page or PDF report
+        Must be either 'streamlit' or 'pdf, default is 'streamlit.
+    content : list
+        Optional input used when output=='pdf', contains HTML for report.
+
+    Returns
+    -------
+    content : list
+        Optional return, used when output=='pdf', contains HTML for report.
+    '''
+    # Make a copy of the school_scores df to work on (avoid SettingCopyWarning)
+    df = school_scores.copy()
+
+    # Add colour for bar based on school
+    df['colour'] = np.where(
+        df['school_lab'] == school_name, 'Your school', 'Other schools')
+
+    # Create column with mean rounded to 2 d.p.
+    df['Mean score'] = round(df['mean'], 2)
+
+    # Plot the results, specifying colours and hover data
+    fig = px.bar(
+        df, x='school_lab', y='mean', color='colour',
+        color_discrete_map={'Your school': '#5D98AB',
+                            'Other schools': '#BFD8E0'},
+        category_orders={'colour': ['Your school', 'Other schools']},
+        hover_data={'school_lab': False, 'colour': False,
+                    'mean': False, 'Mean score': True})
+
+    # Reorder x axis so in ascending order
+    fig.update_layout(xaxis={'categoryorder': 'total ascending'})
+
+    # Set y axis limits so the first and last bars of the chart a consistent
+    # height between different plots - find 15% of range and adjust the min
+    # and max by that
+    min = df['mean'].min()
+    max = df['mean'].max()
+    adj_axis = (max - min)*0.15
+    ymin = np.max([0, (min - adj_axis)])
+    ymax = max + adj_axis
+    fig.update_layout(yaxis_range=[ymin, ymax])
+
+    # Extract lower and upper rag boundaries amd shade the RAG areas
+    # (Colours used were matched to those from the summary page)
+    lower = df['lower'].to_list()[0]
+    upper = df['upper'].to_list()[0]
+    fig.add_hrect(
+        y0=ymin, y1=lower, fillcolor='#FFCCCC', layer='below',
+        line={'color': '#9A505B'}, line_width=0.5,
+        annotation_text='Below average', annotation_position='top left')
+    fig.add_hrect(
+        y0=lower, y1=upper, fillcolor='#FFE8BF', layer='below',
+        line={'color': '#B3852A'}, line_width=0.5,
+        annotation_text='Average', annotation_position='top left')
+    fig.add_hrect(
+        y0=upper, y1=ymax, fillcolor='#B6E6B6', layer='below',
+        line={'color': '#3A8461'}, line_width=0.5,
+        annotation_text='Above average', annotation_position='top left')
+
+    # Set font size and hide x axis tick labels (but seems to be a bug that
+    # means the axis label is then above the plot, so had to use a work around
+    # of replacing the axis labels with spaces
+    fig.update_layout(
+        font=dict(size=font_size),
+        xaxis=dict(title='Northern Devon schools<br>(ordered by mean score)',
+                   tickfont=dict(color='#05291F', size=font_size),
+                   titlefont=dict(color='#05291F', size=font_size),
+                   tickvals=df['school_lab'],
+                   ticktext=[' ']*len(df['school_lab'])),
+        yaxis=dict(title='Mean score',
+                   tickfont=dict(color='#05291F', size=font_size),
+                   titlefont=dict(color='#05291F', size=font_size)),
+        legend=dict(title='School',
+                    font=dict(color='#05291F', size=font_size),
+                    itemclick=False, itemdoubleclick=False),
+        legend_title=dict(font=dict(color='#05291F', size=font_size))
+    )
+
+    # Prevent zooming and panning, remove grid, and hide plotly toolbar
+    fig.layout.xaxis.fixedrange = True
+    fig.layout.yaxis.fixedrange = True
+    fig.update_yaxes(showgrid=False)
+
+    if output == 'streamlit':
+        st.plotly_chart(fig, use_container_width=True,
+                        config={'displayModeBar': False})
+    elif output == 'pdf':
+        # Create temporary list to hold image HTML
+        temp_content = []
+
+        # Get the HTML image tag for the figure and add to temp_content
+        temp_content.append(convert_fig_to_html(
+            fig=fig, alt_text='Comparison with other schools'))
+
+        # Insert temp_content into a div class and add to content
+        content.append(f'''
+<div class='comparison_container'>
+    {''.join(temp_content)}
+</div>''')
+
+        # Return the updated content HTML
+        return content
```

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/explore_results.py` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/explore_results.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,703 +1,703 @@
-'''
-Helper functions for the explore_results() section of dashboard and PDF report.
-'''
-import pandas as pd
-import numpy as np
-import streamlit as st
-from markdown import markdown
-from .bar_charts_text import create_response_description
-from .bar_charts import survey_responses, details_ordered_bar
-from .summary_rag import result_box
-from .reshape_data import filter_by_group, extract_nested_results
-from .score_descriptions import score_descriptions
-
-
-def write_page_title(output='streamlit', survey_type='standard'):
-    '''
-    Writes the title of this page/section (Explore Results), for the streamlit
-    page or for the PDF report.
-
-    Parameters
-    ----------
-    output : string
-        Specifies whether to write for 'streamlit' (default) or 'pdf'.
-    survey_type : string
-        Specifies whether this is for the 'standard' or 'symbol' survey.
-
-    Returns
-    -------
-    html_string : string
-        Optional return, used when output=='pdf', contains HTML for report.
-    '''
-    # Title
-    title = 'Explore results'
-    if output == 'streamlit':
-        st.title(title)
-    elif output == 'pdf':
-        temp_content = []
-        temp_content.append(f'''
-<h1 style='page-break-before:always;' id='explore_results'>{title}</h1>''')
-
-    # Generate the description (with some changes to the text and spacing
-    # between streamlit and the PDF report)
-    if output == 'streamlit':
-        type1 = 'page'
-        type2 = 'page'
-        line_break = ''
-    elif output == 'pdf':
-        type1 = 'section of the report'
-        type2 = 'section'
-        line_break = '<br><br>'
-    descrip = f'''
-This {type1} allows you to explore the results of pupils at your school.'''
-
-    if survey_type == 'standard':
-        descrip += f'''
-{line_break} For each survey topic, you can see (a) a breakdown of how pupils
-at your school responded to each question in that topic, and (b) a chart
-building on results from the 'Summary' {type2} that allows you to understand
-more about the comparison of your results with other schools.'''
-
-    # Add the description to the streamlit page or to the report
-    if output == 'streamlit':
-        st.markdown(descrip)
-    elif output == 'pdf':
-        temp_content.append(f'<p>{descrip}</p>')
-
-        # Then, for the PDF report, format in div and add to content list
-        html_string = f'''
-<div class='page'>
-    <div class='section_container'>
-        {''.join(temp_content)}
-    </div>
-</div>
-'''
-        return html_string
-
-
-def create_topic_dict(df):
-    '''
-    Generate dictionary of survey topics with keys as the topic labels
-    ('variable_lab') and values as the raw topic strings ('variable').
-
-    Parameters
-    ----------
-    df : pandas dataframe
-        Dataframe containing the 'variable' and 'variable_lab' columns
-
-    Returns
-    -------
-    topic_dict : dictionary
-        Dictionary to map between topic raw names and label names
-    '''
-    # Get dataframe with the unique variables and their labels
-    topic_df = df[['variable', 'variable_lab']].drop_duplicates()
-
-    # Drop topics that we don't want to appear in the dictionary
-    topic_df = topic_df[~topic_df['variable'].isin([
-            'staff_talk_score', 'home_talk_score', 'peer_talk_score'])]
-
-    # Remove the '_score' suffix from the variable names
-    topic_df['variable'] = topic_df['variable'].str.replace('_score', '')
-
-    # Convert to a dictionary
-    topic_dict = pd.Series(
-        topic_df.variable.values, index=topic_df.variable_lab).to_dict()
-
-    return topic_dict
-
-
-def choose_topic(df, include_raw_name=False):
-    '''
-    Create topic dictionary and produce selectbox for users to choose a topic
-
-    Parameters
-    ----------
-    df : Dataframe
-        Dataframe which includes columns with topic names
-    include_raw_name : Boolean
-        Whether to include the raw version of the topic name
-
-    Returns
-    -------
-    chosen_variable_lab : String
-        Full and capitalised topic name
-    chosen_variable : String
-        Raw version of topic name
-    '''
-    # Create dictionary of topics
-    topic_dict = create_topic_dict(df)
-
-    # If session state doesn't contain chosen variable, default to Autonomy
-    # If it does (i.e. set from Summary page), use that
-    if 'chosen_variable_lab' not in st.session_state:
-        st.session_state['chosen_variable_lab'] = 'Autonomy'
-
-    # Convert topics to list and find index of the session state variable
-    topic_list = list(topic_dict.keys())
-    default = topic_list.index(st.session_state['chosen_variable_lab'])
-
-    # Select topic
-    chosen_variable_lab = st.selectbox(
-        '**Topic:**', topic_dict.keys(), index=default)
-
-    # Convert from variable_lab to variable
-    chosen_variable = topic_dict[chosen_variable_lab]
-
-    if include_raw_name:
-        # Convert from variable_lab to variable
-        chosen_variable = topic_dict[chosen_variable_lab]
-        return chosen_variable_lab, chosen_variable
-    else:
-        return chosen_variable_lab
-
-
-def write_topic_intro(chosen_variable, chosen_variable_lab, df,
-                      output='streamlit', content=None):
-    '''
-    Writes the header for the topic on the Explore Results streamlit page or
-    in HTML for page of PDF report.
-    Example output:
-        Psychological Wellbeing
-        These questions are about how positive and generally happy young people
-        feel regarding their life.
-
-    Parameters
-    ----------
-    chosen_variable : string
-        Chosen variable in simple format (e.g. 'psychological_wellbeing')
-    chosen_variable_lab : string
-        Chosen variable in label format (e.g. 'Psychological wellbeing')
-    df : pandas dataframe
-        Dataframe containing the 'variable' and 'description' columns for each
-        topic.
-    output : string
-        Specifies whether to write for 'streamlit' (default) or 'pdf'.
-    content : list
-        Optional input used when output=='pdf', contains HTML for report.
-
-    Returns
-    -------
-    content : list
-        Optional return, used when output=='pdf', contains HTML for report.
-    '''
-    # Header (name of topic)
-    if output == 'streamlit':
-        st.markdown(f'''<h2 style='font-size:55px; text-align:center;'>{
-            chosen_variable_lab}</h2>''', unsafe_allow_html=True)
-    elif output == 'pdf':
-        content.append(f'''
-<h1 style='text-align:center; page-break-before:always;'
-id='{chosen_variable}'>{chosen_variable_lab}</h1>''')
-
-    # Description under header (one sentence summary of topic)
-    # Create dictionary where key is topic name and value is topic description
-    description = (df[['variable', 'description']]
-                   .drop_duplicates()
-                   .set_index('variable')
-                   .to_dict()['description'])
-
-    # Create description string
-    topic_descrip = f'''
-<p style='text-align:center;'><b>These questions are
-about {description[f'{chosen_variable}_score'].lower()}</b></p>'''
-
-    # Print that description string into streamlit page or PDF report HTML
-    if output == 'streamlit':
-        st.markdown(topic_descrip, unsafe_allow_html=True)
-    elif output == 'pdf':
-        content.append(f'{topic_descrip}<br>')
-        return content
-
-
-def write_response_section_intro(
-        chosen_variable_lab, output='streamlit', content=None, type='school'):
-    '''
-    Create the header and description for the section with the bar charts
-    showing responses from pupils to each question of a topic.
-    Example output:
-        Responses from pupils at your school
-        In this section, you can see how pupils at you school responded to
-        survey questions that relate to the topic of 'psychological wellbeing'.
-
-    Parameters
-    ----------
-    chosen_variable_lab : string
-        Chosen variable in label format (e.g. 'Psychological wellbeing')
-    output : string
-        Specifies whether to write for 'streamlit' (default) or 'pdf'.
-    content : list
-        Optional input used when output=='pdf', contains HTML for report.
-    type : string
-        Specifies whether it is a 'school' (default) or 'public' dashboard
-
-    Returns
-    -------
-    content : list
-        Optional return, used when output=='pdf', contains HTML for report.
-    '''
-    # Create phrase to use below, depending on dashboard type
-    if type == 'school':
-        phrase = 'pupils at your school'
-    elif type == 'public':
-        phrase = 'young people across Northern Devon'
-
-    # Section header (currently not used for public dashboard)
-    if type == 'school':
-        header = f'Responses from {phrase}'
-        if output == 'streamlit':
-            st.subheader(header)
-        elif output == 'pdf':
-            content.append(f'<h3>{header}</h3>')
-
-    # Section description
-    section_descrip = f'''
-In this section, you can see how {phrase} responded to survey
-questions that relate to the topic of '{chosen_variable_lab.lower()}'.'''
-    if output == 'streamlit':
-        st.markdown(section_descrip)
-    elif output == 'pdf':
-        content.append(f'<p>{section_descrip}</p>')
-        return content
-
-
-def get_chosen_result(chosen_variable, chosen_group, df, school,
-                      survey_type='standard'):
-    '''
-    Filters the dataframe with responses to each question, to just responses
-    for the chosen topic, school and group.
-
-    Parameters
-    ----------
-    chosen_variable : string
-        Name of the chosen topic
-    chosen_group : string
-        Name of the chosen group to view results by - options are
-        'For all pupils', 'By year group', 'By gender', 'By FSM' or 'By SEN'
-    df : dataframe
-        Dataframe with responses to all the questions for all topics
-    school : string
-        Name of school to get results for
-    survey_type : string
-        Specifies whether it is 'standard' (default) or 'symbol' survey
-
-    Returns
-    ----------
-    chosen_result : dataframe
-        Contains responses to each question in the chosen topic, with the
-        results extracted so they are in seperate rows and columns (rather
-        than original format where they are nested in lists)
-
-    '''
-    # Filter by the specified school and grouping
-    chosen, group_lab = filter_by_group(
-        df=df, chosen_group=chosen_group, output='explore',
-        chosen_school=school, survey_type=survey_type)
-
-    # Filter by the chosen variable
-    chosen = chosen[chosen['group'] == chosen_variable]
-
-    # Extract the nested lists in the dataframe
-    chosen_result = extract_nested_results(chosen, group_lab)
-
-    return chosen_result
-
-
-def reverse_categories(df):
-    '''
-    Resorts dataframe so categories are in reverse order, but ensuring
-    non-response is still at the end (despite it being the max value).
-
-    Parameters:
-    -----------
-    df : dataframe
-        Dataframe with question responses, to be resorted
-
-    Returns:
-    --------
-    new_df : dataframe
-        Resorted dataframe
-    '''
-    # Resort everything except for the pupils who did not respond
-    # (which is always the final category)
-    new_df = df[df['cat'] != df['cat'].max()].sort_values(by=['cat'],
-                                                          ascending=False)
-
-    # Append those non-response counts back to the end
-    new_df = pd.concat([new_df, df[df['cat'] == df['cat'].max()]])
-
-    return new_df
-
-
-def define_multiple_charts():
-    '''
-    Create a dictionary designating which topics have charts that needed to be
-    seperated, and how this should be done. This is to create seperate clusters
-    of charts (so there can be text describing one group of charts, then
-    text describing another - e.g. when they're the same topic but have
-    different sets of responses options).
-
-    Returns
-    -------
-    multiple_charts : dictionary
-        Dictionary where key is variable and value is dictionary with
-        sub-groups of topic questions
-    '''
-    multiple_charts = {
-        'optimism': {'optimism_future': ['optimism_future'],
-                     'optimism_other': ['optimism_best',
-                                        'optimism_good',
-                                        'optimism_work']},
-        'appearance': {'appearance_happy': ['appearance_happy'],
-                       'appearance_feel': ['appearance_feel']},
-        'physical': {'physical_days': ['physical_days'],
-                     'physical_hours': ['physical_hours']},
-        'places': {'places_freq': ['places_freq'],
-                   'places_barriers': ['places_barriers___1',
-                                       'places_barriers___2',
-                                       'places_barriers___3',
-                                       'places_barriers___4',
-                                       'places_barriers___5',
-                                       'places_barriers___6',
-                                       'places_barriers___7',
-                                       'places_barriers___8',
-                                       'places_barriers___9']},
-        'talk': {'talk_yesno': ['staff_talk',
-                                'home_talk',
-                                'peer_talk'],
-                 'talk_listen': ['staff_talk_listen',
-                                 'home_talk_listen',
-                                 'peer_talk_listen'],
-                 'talk_helpful': ['staff_talk_helpful',
-                                  'home_talk_helpful',
-                                  'peer_talk_helpful'],
-                 'talk_if': ['staff_talk_if',
-                             'home_talk_if',
-                             'peer_talk_if']},
-        'local_env': {'local_safe': ['local_safe'],
-                      'local_other': ['local_support',
-                                      'local_trust',
-                                      'local_neighbours',
-                                      'local_places']},
-        'future': {'future_options': ['future_options'],
-                   'future_interest': ['future_interest'],
-                   'future_support': ['future_support']}
-    }
-
-    return multiple_charts
-
-
-def create_bar_charts(chosen_variable, chosen_result,
-                      output='streamlit', content=None):
-    '''
-    Creates the section of bar charts and their accompanying text, for
-    streamlit page or PDF report.
-
-    Parameters
-    ----------
-    chosen_variable : string
-        Name of the chosen topic
-    chosen_result : dataframe
-        Contains responses to each question in the chosen topic, school + group
-    output : string
-        Specifies whether to write for 'streamlit' (default) or 'pdf'.
-    content : list
-        Optional input used when output=='pdf', contains HTML for report.
-
-    Returns
-    -------
-    content : list
-        Optional return, used when output=='pdf', contains HTML for report.
-    '''
-    # Import dictionary designating if there are sub-groups of charts
-    multiple_charts = define_multiple_charts()
-
-    # Import descriptions for the groups of stacked bar charts
-    # Note: We still import for symbol dashboard but won't use
-    response_descrip = create_response_description()
-
-    # Define which variables need to be reversed - intention was to be mostly
-    # be positive to negative - but made exceptions for social media use, where
-    # that ordering felt counter-intuitive - and for the sub-questions of
-    # autonomy where the question meaning flips between positive and negative
-    reverse = ['esteem', 'negative', 'support', 'free_like', 'local_safe',
-               'local_other', 'belong_local', 'bully']
-
-    # Create bar chart with seperate chart groups if required
-    if chosen_variable in multiple_charts:
-        # Counter as we don't want to break page before first description,
-        # but do for the later description
-        i = -1
-        var_dict = multiple_charts[chosen_variable]
-        for key, value in var_dict.items():
-            i += 1
-            # Add description
-            if key in response_descrip.keys():
-                if output == 'streamlit':
-                    st.markdown(response_descrip[key])
-                elif output == 'pdf':
-                    # Break page before description, unless it's the first.
-                    if i > 0:
-                        content.append(f'''
-<p style='page-break-before:always;'>{response_descrip[key]}</p>''')
-                    else:
-                        content.append(f'<p>{response_descrip[key]}</p>')
-
-            # Filter to questions in sub-group, reversing categories if need to
-            to_plot = chosen_result[chosen_result['measure'].isin(value)]
-            if key in reverse:
-                to_plot = reverse_categories(to_plot)
-
-            # Output the plots
-            if output == 'streamlit':
-                survey_responses(to_plot)
-            elif output == 'pdf':
-                content = survey_responses(
-                    dataset=to_plot, font_size=14,
-                    output='pdf', content=content)
-
-    # Otherwise create a single stacked bar chart
-    else:
-
-        # Add description
-        if chosen_variable in response_descrip.keys():
-            if output == 'streamlit':
-                st.markdown(response_descrip[chosen_variable])
-            elif output == 'pdf':
-                content.append(
-                    f'<p>{response_descrip[chosen_variable]}</p>')
-
-        # Reverse categories if required
-        if chosen_variable in reverse:
-            chosen_result = reverse_categories(chosen_result)
-
-        # Output the plot
-        if output == 'streamlit':
-            survey_responses(chosen_result)
-        elif output == 'pdf':
-            content = survey_responses(
-                dataset=chosen_result, font_size=14,
-                output='pdf', content=content)
-
-    if output == 'pdf':
-        return content
-
-
-def write_comparison_intro(
-        chosen_variable, chosen_variable_lab, score_descriptions,
-        output='streamlit', content=None):
-    '''
-    Write the introduction to the comparison section (heading, description
-    and RAG rating)
-
-    Parameters
-    ----------
-    chosen_variable : string
-        Chosen variable (e.g. 'autonomy')
-    chosen_variable_lab : string
-        Label for the chosen variable (e.g. 'Autonomy')
-    score_descriptions : dictionary
-        Dictionary with variable and then the appropriate descriptions for this
-        section (range of score, and interpretation of score)
-    output : string
-        Specifies whether to write for 'streamlit' (default) or 'pdf'.
-    content : list
-        Optional input used when output=='pdf', contains HTML for report.
-
-    Returns
-    -------
-    content : list
-        Optional return, used when output=='pdf', contains HTML for report.
-    '''
-    # Heading
-    heading = 'Comparison with other schools'
-    if output == 'streamlit':
-        st.subheader(heading)
-    elif output == 'pdf':
-        content.append(f'''
-<h3 style='page-break-before: always;'>{heading}</h3>''')
-
-    # Description text
-    description = f'''
-In this section, an overall score for the topic of
-'{chosen_variable_lab.lower()}' has been calculated for each pupil with
-complete responses on this question. Possible scores for each pupil on this
-topic range from {score_descriptions[chosen_variable][0]} with
-**higher scores indicating {score_descriptions[chosen_variable][1]}** -
-and vice versa for lower scores. The mean score of the pupils at you
-school is compared with pupils who completed the same survey questions at other
-schools. This allows you to see whether the typical score for pupils at your
-school is average, below average or above average.'''
-
-    # Add description to dashboard or report
-    if output == 'streamlit':
-        st.markdown(description)
-    elif output == 'pdf':
-        content.append(markdown(description))
-        return content
-
-
-def write_comparison_result(chosen_school, between_schools, group,
-                            output='streamlit', content=None):
-    '''
-    Write the introduction to the comparison section (heading, description
-    and RAG rating)
-
-    Parameters
-    ----------
-    chosen_school : string
-        Name of chosen school
-    between_schools: dataframe
-        Dataframe with scores for the chosen variable in each school
-    output : string
-        Specifies whether to write for 'streamlit' (default) or 'pdf'.
-    content : list
-        Optional input used when output=='pdf', contains HTML for report.
-    group : string
-        Pupil group
-
-    Returns
-    -------
-    content : list
-        Optional return, used when output=='pdf', contains HTML for report.
-    '''
-    # Provide title, unless looking at all pupils, in which case drop group too
-    if group != 'All':
-        description = f'''**{group}**
-
-'''
-    else:
-        group = ''
-        description = ''
-
-    # Get number of responses at school
-    school_mean = between_schools.loc[
-        between_schools['school_lab'] == chosen_school, 'mean'].to_list()[0]
-
-    # Display message if it was less than 10 (and so NaN)
-    if np.isnan(school_mean):
-        description += '''
-There were less than ten complete responses from these pupils at your school,
-so the results are not shown.
-'''
-    # Otherwise...
-    else:
-        # Get count of pupils who completed the topic questions
-        topic_count = int(between_schools.loc[
-            between_schools['school_lab'] == chosen_school,
-            'count'].to_list()[0])
-
-        # Get total responses and total schools (can just take first item as
-        # whole column will be the same value for each school)
-        total_responses = str(int(
-            between_schools['total_pupils'].to_list()[0]))
-        total_schools = str(int(
-            between_schools['group_n'].to_list()[0]))
-        description += f'''
-Your school had {topic_count} complete responses. Across
-Northern Devon, there were {total_responses} complete responses from
-{total_schools} schools. The average score for the pupils at your school,
-compared to other schools in Northern Devon, was:'''
-
-    # Add description to page
-    if output == 'streamlit':
-        st.markdown(description)
-    elif output == 'pdf':
-        content.append(markdown(description))
-
-    # If school wasn't NaN...
-    if not np.isnan(school_mean):
-        # Get RAG rating
-        devon_rag = between_schools.loc[
-            between_schools['school_lab'] == chosen_school, 'rag'].to_list()[0]
-        # Drop any schools that were NaN (i.e. n<10)
-        between_schools = between_schools[between_schools['mean'].notna()]
-        # Add the RAG result and ordered bar chart
-        if output == 'streamlit':
-            result_box(devon_rag)
-            details_ordered_bar(between_schools, chosen_school)
-        elif output == 'pdf':
-            content.append(result_box(devon_rag, 'pdf'))
-            content = details_ordered_bar(
-                school_scores=between_schools, school_name=chosen_school,
-                font_size=16, output='pdf', content=content)
-
-    if output == 'pdf':
-        return content
-
-
-def create_explore_topic_page(
-        chosen_variable_lab, topic_dict, df_scores, chosen_school,
-        chosen_group, df_prop, content):
-    '''
-    Add an explore results page with responses to a given topic to report HTML.
-
-    Parameters
-    ----------
-    chosen_variable_lab : string
-        Chosen variable in label format (e.g. 'Psychological wellbeing')
-    topic_dict : dictionary
-        Dictionary of topics where key is variable_lab and value is variable
-    df_scores : dataframe
-        Dataframe with scores for each topic
-    chosen_school : string
-        Name of the chosen school
-    chosen_group : string
-        Name of the chosen group to view results by - options are
-        'For all pupils', 'By year group', 'By gender', 'By FSM' or 'By SEN'
-    df_prop : dataframe
-        Dataframe with the proportion of pupils providing each response to each
-        survey question
-    content : list
-        Optional input used when output=='pdf', contains HTML for report.
-
-    Returns
-    -------
-    content : list
-        Optional return, used when output=='pdf', contains HTML for report.
-    '''
-    # Convert from variable_lab to variable
-    chosen_variable = topic_dict[chosen_variable_lab]
-
-    # Topic header and description
-    content = write_topic_intro(chosen_variable, chosen_variable_lab,
-                                df_scores, output='pdf', content=content)
-
-    # Section header and description
-    content = write_response_section_intro(
-        chosen_variable_lab, output='pdf', content=content)
-
-    # Get dataframe with results for the chosen variable, group and school
-    chosen_result = get_chosen_result(
-        chosen_variable, chosen_group, df_prop, chosen_school)
-
-    # Produce bar charts, plus their chart section descriptions and titles
-    content = create_bar_charts(
-        chosen_variable, chosen_result, output='pdf', content=content)
-
-    # Create dataframe based on chosen variable
-    between_schools, group_lab, order = filter_by_group(
-        df=df_scores, chosen_group=chosen_group, output='compare',
-        chosen_variable=chosen_variable+'_score')
-
-    # Write the comparison intro text
-    content = write_comparison_intro(
-        chosen_variable, chosen_variable_lab, score_descriptions,
-        output='pdf', content=content)
-
-    # Filter to each group (will just be 'all' if was for all pupils), then
-    # print the results and create the ordered bar chart for each
-    for group in order:
-        temp_content = []
-        # Filter to group and get result
-        group_result = between_schools[between_schools[group_lab] == group]
-        temp_content = write_comparison_result(
-            chosen_school, group_result, group, output='pdf',
-            content=temp_content)
-        # Insert temp_content into a div class and add to content
-        content.append(f'''
-    <div class='responses_container'>
-        {''.join(temp_content)}
-    </div>''')
-
-    return content
+'''
+Helper functions for the explore_results() section of dashboard and PDF report.
+'''
+import pandas as pd
+import numpy as np
+import streamlit as st
+from markdown import markdown
+from .bar_charts_text import create_response_description
+from .bar_charts import survey_responses, details_ordered_bar
+from .summary_rag import result_box
+from .reshape_data import filter_by_group, extract_nested_results
+from .score_descriptions import score_descriptions
+
+
+def write_page_title(output='streamlit', survey_type='standard'):
+    '''
+    Writes the title of this page/section (Explore Results), for the streamlit
+    page or for the PDF report.
+
+    Parameters
+    ----------
+    output : string
+        Specifies whether to write for 'streamlit' (default) or 'pdf'.
+    survey_type : string
+        Specifies whether this is for the 'standard' or 'symbol' survey.
+
+    Returns
+    -------
+    html_string : string
+        Optional return, used when output=='pdf', contains HTML for report.
+    '''
+    # Title
+    title = 'Explore results'
+    if output == 'streamlit':
+        st.title(title)
+    elif output == 'pdf':
+        temp_content = []
+        temp_content.append(f'''
+<h1 style='page-break-before:always;' id='explore_results'>{title}</h1>''')
+
+    # Generate the description (with some changes to the text and spacing
+    # between streamlit and the PDF report)
+    if output == 'streamlit':
+        type1 = 'page'
+        type2 = 'page'
+        line_break = ''
+    elif output == 'pdf':
+        type1 = 'section of the report'
+        type2 = 'section'
+        line_break = '<br><br>'
+    descrip = f'''
+This {type1} allows you to explore the results of pupils at your school.'''
+
+    if survey_type == 'standard':
+        descrip += f'''
+{line_break} For each survey topic, you can see (a) a breakdown of how pupils
+at your school responded to each question in that topic, and (b) a chart
+building on results from the 'Summary' {type2} that allows you to understand
+more about the comparison of your results with other schools.'''
+
+    # Add the description to the streamlit page or to the report
+    if output == 'streamlit':
+        st.markdown(descrip)
+    elif output == 'pdf':
+        temp_content.append(f'<p>{descrip}</p>')
+
+        # Then, for the PDF report, format in div and add to content list
+        html_string = f'''
+<div class='page'>
+    <div class='section_container'>
+        {''.join(temp_content)}
+    </div>
+</div>
+'''
+        return html_string
+
+
+def create_topic_dict(df):
+    '''
+    Generate dictionary of survey topics with keys as the topic labels
+    ('variable_lab') and values as the raw topic strings ('variable').
+
+    Parameters
+    ----------
+    df : pandas dataframe
+        Dataframe containing the 'variable' and 'variable_lab' columns
+
+    Returns
+    -------
+    topic_dict : dictionary
+        Dictionary to map between topic raw names and label names
+    '''
+    # Get dataframe with the unique variables and their labels
+    topic_df = df[['variable', 'variable_lab']].drop_duplicates()
+
+    # Drop topics that we don't want to appear in the dictionary
+    topic_df = topic_df[~topic_df['variable'].isin([
+            'staff_talk_score', 'home_talk_score', 'peer_talk_score'])]
+
+    # Remove the '_score' suffix from the variable names
+    topic_df['variable'] = topic_df['variable'].str.replace('_score', '')
+
+    # Convert to a dictionary
+    topic_dict = pd.Series(
+        topic_df.variable.values, index=topic_df.variable_lab).to_dict()
+
+    return topic_dict
+
+
+def choose_topic(df, include_raw_name=False):
+    '''
+    Create topic dictionary and produce selectbox for users to choose a topic
+
+    Parameters
+    ----------
+    df : Dataframe
+        Dataframe which includes columns with topic names
+    include_raw_name : Boolean
+        Whether to include the raw version of the topic name
+
+    Returns
+    -------
+    chosen_variable_lab : String
+        Full and capitalised topic name
+    chosen_variable : String
+        Raw version of topic name
+    '''
+    # Create dictionary of topics
+    topic_dict = create_topic_dict(df)
+
+    # If session state doesn't contain chosen variable, default to Autonomy
+    # If it does (i.e. set from Summary page), use that
+    if 'chosen_variable_lab' not in st.session_state:
+        st.session_state['chosen_variable_lab'] = 'Autonomy'
+
+    # Convert topics to list and find index of the session state variable
+    topic_list = list(topic_dict.keys())
+    default = topic_list.index(st.session_state['chosen_variable_lab'])
+
+    # Select topic
+    chosen_variable_lab = st.selectbox(
+        '**Topic:**', topic_dict.keys(), index=default)
+
+    # Convert from variable_lab to variable
+    chosen_variable = topic_dict[chosen_variable_lab]
+
+    if include_raw_name:
+        # Convert from variable_lab to variable
+        chosen_variable = topic_dict[chosen_variable_lab]
+        return chosen_variable_lab, chosen_variable
+    else:
+        return chosen_variable_lab
+
+
+def write_topic_intro(chosen_variable, chosen_variable_lab, df,
+                      output='streamlit', content=None):
+    '''
+    Writes the header for the topic on the Explore Results streamlit page or
+    in HTML for page of PDF report.
+    Example output:
+        Psychological Wellbeing
+        These questions are about how positive and generally happy young people
+        feel regarding their life.
+
+    Parameters
+    ----------
+    chosen_variable : string
+        Chosen variable in simple format (e.g. 'psychological_wellbeing')
+    chosen_variable_lab : string
+        Chosen variable in label format (e.g. 'Psychological wellbeing')
+    df : pandas dataframe
+        Dataframe containing the 'variable' and 'description' columns for each
+        topic.
+    output : string
+        Specifies whether to write for 'streamlit' (default) or 'pdf'.
+    content : list
+        Optional input used when output=='pdf', contains HTML for report.
+
+    Returns
+    -------
+    content : list
+        Optional return, used when output=='pdf', contains HTML for report.
+    '''
+    # Header (name of topic)
+    if output == 'streamlit':
+        st.markdown(f'''<h2 style='font-size:55px; text-align:center;'>{
+            chosen_variable_lab}</h2>''', unsafe_allow_html=True)
+    elif output == 'pdf':
+        content.append(f'''
+<h1 style='text-align:center; page-break-before:always;'
+id='{chosen_variable}'>{chosen_variable_lab}</h1>''')
+
+    # Description under header (one sentence summary of topic)
+    # Create dictionary where key is topic name and value is topic description
+    description = (df[['variable', 'description']]
+                   .drop_duplicates()
+                   .set_index('variable')
+                   .to_dict()['description'])
+
+    # Create description string
+    topic_descrip = f'''
+<p style='text-align:center;'><b>These questions are
+about {description[f'{chosen_variable}_score'].lower()}</b></p>'''
+
+    # Print that description string into streamlit page or PDF report HTML
+    if output == 'streamlit':
+        st.markdown(topic_descrip, unsafe_allow_html=True)
+    elif output == 'pdf':
+        content.append(f'{topic_descrip}<br>')
+        return content
+
+
+def write_response_section_intro(
+        chosen_variable_lab, output='streamlit', content=None, type='school'):
+    '''
+    Create the header and description for the section with the bar charts
+    showing responses from pupils to each question of a topic.
+    Example output:
+        Responses from pupils at your school
+        In this section, you can see how pupils at you school responded to
+        survey questions that relate to the topic of 'psychological wellbeing'.
+
+    Parameters
+    ----------
+    chosen_variable_lab : string
+        Chosen variable in label format (e.g. 'Psychological wellbeing')
+    output : string
+        Specifies whether to write for 'streamlit' (default) or 'pdf'.
+    content : list
+        Optional input used when output=='pdf', contains HTML for report.
+    type : string
+        Specifies whether it is a 'school' (default) or 'public' dashboard
+
+    Returns
+    -------
+    content : list
+        Optional return, used when output=='pdf', contains HTML for report.
+    '''
+    # Create phrase to use below, depending on dashboard type
+    if type == 'school':
+        phrase = 'pupils at your school'
+    elif type == 'public':
+        phrase = 'young people across Northern Devon'
+
+    # Section header (currently not used for public dashboard)
+    if type == 'school':
+        header = f'Responses from {phrase}'
+        if output == 'streamlit':
+            st.subheader(header)
+        elif output == 'pdf':
+            content.append(f'<h3>{header}</h3>')
+
+    # Section description
+    section_descrip = f'''
+In this section, you can see how {phrase} responded to survey
+questions that relate to the topic of '{chosen_variable_lab.lower()}'.'''
+    if output == 'streamlit':
+        st.markdown(section_descrip)
+    elif output == 'pdf':
+        content.append(f'<p>{section_descrip}</p>')
+        return content
+
+
+def get_chosen_result(chosen_variable, chosen_group, df, school,
+                      survey_type='standard'):
+    '''
+    Filters the dataframe with responses to each question, to just responses
+    for the chosen topic, school and group.
+
+    Parameters
+    ----------
+    chosen_variable : string
+        Name of the chosen topic
+    chosen_group : string
+        Name of the chosen group to view results by - options are
+        'For all pupils', 'By year group', 'By gender', 'By FSM' or 'By SEN'
+    df : dataframe
+        Dataframe with responses to all the questions for all topics
+    school : string
+        Name of school to get results for
+    survey_type : string
+        Specifies whether it is 'standard' (default) or 'symbol' survey
+
+    Returns
+    ----------
+    chosen_result : dataframe
+        Contains responses to each question in the chosen topic, with the
+        results extracted so they are in seperate rows and columns (rather
+        than original format where they are nested in lists)
+
+    '''
+    # Filter by the specified school and grouping
+    chosen, group_lab = filter_by_group(
+        df=df, chosen_group=chosen_group, output='explore',
+        chosen_school=school, survey_type=survey_type)
+
+    # Filter by the chosen variable
+    chosen = chosen[chosen['group'] == chosen_variable]
+
+    # Extract the nested lists in the dataframe
+    chosen_result = extract_nested_results(chosen, group_lab)
+
+    return chosen_result
+
+
+def reverse_categories(df):
+    '''
+    Resorts dataframe so categories are in reverse order, but ensuring
+    non-response is still at the end (despite it being the max value).
+
+    Parameters:
+    -----------
+    df : dataframe
+        Dataframe with question responses, to be resorted
+
+    Returns:
+    --------
+    new_df : dataframe
+        Resorted dataframe
+    '''
+    # Resort everything except for the pupils who did not respond
+    # (which is always the final category)
+    new_df = df[df['cat'] != df['cat'].max()].sort_values(by=['cat'],
+                                                          ascending=False)
+
+    # Append those non-response counts back to the end
+    new_df = pd.concat([new_df, df[df['cat'] == df['cat'].max()]])
+
+    return new_df
+
+
+def define_multiple_charts():
+    '''
+    Create a dictionary designating which topics have charts that needed to be
+    seperated, and how this should be done. This is to create seperate clusters
+    of charts (so there can be text describing one group of charts, then
+    text describing another - e.g. when they're the same topic but have
+    different sets of responses options).
+
+    Returns
+    -------
+    multiple_charts : dictionary
+        Dictionary where key is variable and value is dictionary with
+        sub-groups of topic questions
+    '''
+    multiple_charts = {
+        'optimism': {'optimism_future': ['optimism_future'],
+                     'optimism_other': ['optimism_best',
+                                        'optimism_good',
+                                        'optimism_work']},
+        'appearance': {'appearance_happy': ['appearance_happy'],
+                       'appearance_feel': ['appearance_feel']},
+        'physical': {'physical_days': ['physical_days'],
+                     'physical_hours': ['physical_hours']},
+        'places': {'places_freq': ['places_freq'],
+                   'places_barriers': ['places_barriers___1',
+                                       'places_barriers___2',
+                                       'places_barriers___3',
+                                       'places_barriers___4',
+                                       'places_barriers___5',
+                                       'places_barriers___6',
+                                       'places_barriers___7',
+                                       'places_barriers___8',
+                                       'places_barriers___9']},
+        'talk': {'talk_yesno': ['staff_talk',
+                                'home_talk',
+                                'peer_talk'],
+                 'talk_listen': ['staff_talk_listen',
+                                 'home_talk_listen',
+                                 'peer_talk_listen'],
+                 'talk_helpful': ['staff_talk_helpful',
+                                  'home_talk_helpful',
+                                  'peer_talk_helpful'],
+                 'talk_if': ['staff_talk_if',
+                             'home_talk_if',
+                             'peer_talk_if']},
+        'local_env': {'local_safe': ['local_safe'],
+                      'local_other': ['local_support',
+                                      'local_trust',
+                                      'local_neighbours',
+                                      'local_places']},
+        'future': {'future_options': ['future_options'],
+                   'future_interest': ['future_interest'],
+                   'future_support': ['future_support']}
+    }
+
+    return multiple_charts
+
+
+def create_bar_charts(chosen_variable, chosen_result,
+                      output='streamlit', content=None):
+    '''
+    Creates the section of bar charts and their accompanying text, for
+    streamlit page or PDF report.
+
+    Parameters
+    ----------
+    chosen_variable : string
+        Name of the chosen topic
+    chosen_result : dataframe
+        Contains responses to each question in the chosen topic, school + group
+    output : string
+        Specifies whether to write for 'streamlit' (default) or 'pdf'.
+    content : list
+        Optional input used when output=='pdf', contains HTML for report.
+
+    Returns
+    -------
+    content : list
+        Optional return, used when output=='pdf', contains HTML for report.
+    '''
+    # Import dictionary designating if there are sub-groups of charts
+    multiple_charts = define_multiple_charts()
+
+    # Import descriptions for the groups of stacked bar charts
+    # Note: We still import for symbol dashboard but won't use
+    response_descrip = create_response_description()
+
+    # Define which variables need to be reversed - intention was to be mostly
+    # be positive to negative - but made exceptions for social media use, where
+    # that ordering felt counter-intuitive - and for the sub-questions of
+    # autonomy where the question meaning flips between positive and negative
+    reverse = ['esteem', 'negative', 'support', 'free_like', 'local_safe',
+               'local_other', 'belong_local', 'bully']
+
+    # Create bar chart with seperate chart groups if required
+    if chosen_variable in multiple_charts:
+        # Counter as we don't want to break page before first description,
+        # but do for the later description
+        i = -1
+        var_dict = multiple_charts[chosen_variable]
+        for key, value in var_dict.items():
+            i += 1
+            # Add description
+            if key in response_descrip.keys():
+                if output == 'streamlit':
+                    st.markdown(response_descrip[key])
+                elif output == 'pdf':
+                    # Break page before description, unless it's the first.
+                    if i > 0:
+                        content.append(f'''
+<p style='page-break-before:always;'>{response_descrip[key]}</p>''')
+                    else:
+                        content.append(f'<p>{response_descrip[key]}</p>')
+
+            # Filter to questions in sub-group, reversing categories if need to
+            to_plot = chosen_result[chosen_result['measure'].isin(value)]
+            if key in reverse:
+                to_plot = reverse_categories(to_plot)
+
+            # Output the plots
+            if output == 'streamlit':
+                survey_responses(to_plot)
+            elif output == 'pdf':
+                content = survey_responses(
+                    dataset=to_plot, font_size=14,
+                    output='pdf', content=content)
+
+    # Otherwise create a single stacked bar chart
+    else:
+
+        # Add description
+        if chosen_variable in response_descrip.keys():
+            if output == 'streamlit':
+                st.markdown(response_descrip[chosen_variable])
+            elif output == 'pdf':
+                content.append(
+                    f'<p>{response_descrip[chosen_variable]}</p>')
+
+        # Reverse categories if required
+        if chosen_variable in reverse:
+            chosen_result = reverse_categories(chosen_result)
+
+        # Output the plot
+        if output == 'streamlit':
+            survey_responses(chosen_result)
+        elif output == 'pdf':
+            content = survey_responses(
+                dataset=chosen_result, font_size=14,
+                output='pdf', content=content)
+
+    if output == 'pdf':
+        return content
+
+
+def write_comparison_intro(
+        chosen_variable, chosen_variable_lab, score_descriptions,
+        output='streamlit', content=None):
+    '''
+    Write the introduction to the comparison section (heading, description
+    and RAG rating)
+
+    Parameters
+    ----------
+    chosen_variable : string
+        Chosen variable (e.g. 'autonomy')
+    chosen_variable_lab : string
+        Label for the chosen variable (e.g. 'Autonomy')
+    score_descriptions : dictionary
+        Dictionary with variable and then the appropriate descriptions for this
+        section (range of score, and interpretation of score)
+    output : string
+        Specifies whether to write for 'streamlit' (default) or 'pdf'.
+    content : list
+        Optional input used when output=='pdf', contains HTML for report.
+
+    Returns
+    -------
+    content : list
+        Optional return, used when output=='pdf', contains HTML for report.
+    '''
+    # Heading
+    heading = 'Comparison with other schools'
+    if output == 'streamlit':
+        st.subheader(heading)
+    elif output == 'pdf':
+        content.append(f'''
+<h3 style='page-break-before: always;'>{heading}</h3>''')
+
+    # Description text
+    description = f'''
+In this section, an overall score for the topic of
+'{chosen_variable_lab.lower()}' has been calculated for each pupil with
+complete responses on this question. Possible scores for each pupil on this
+topic range from {score_descriptions[chosen_variable][0]} with
+**higher scores indicating {score_descriptions[chosen_variable][1]}** -
+and vice versa for lower scores. The mean score of the pupils at you
+school is compared with pupils who completed the same survey questions at other
+schools. This allows you to see whether the typical score for pupils at your
+school is average, below average or above average.'''
+
+    # Add description to dashboard or report
+    if output == 'streamlit':
+        st.markdown(description)
+    elif output == 'pdf':
+        content.append(markdown(description))
+        return content
+
+
+def write_comparison_result(chosen_school, between_schools, group,
+                            output='streamlit', content=None):
+    '''
+    Write the introduction to the comparison section (heading, description
+    and RAG rating)
+
+    Parameters
+    ----------
+    chosen_school : string
+        Name of chosen school
+    between_schools: dataframe
+        Dataframe with scores for the chosen variable in each school
+    output : string
+        Specifies whether to write for 'streamlit' (default) or 'pdf'.
+    content : list
+        Optional input used when output=='pdf', contains HTML for report.
+    group : string
+        Pupil group
+
+    Returns
+    -------
+    content : list
+        Optional return, used when output=='pdf', contains HTML for report.
+    '''
+    # Provide title, unless looking at all pupils, in which case drop group too
+    if group != 'All':
+        description = f'''**{group}**
+
+'''
+    else:
+        group = ''
+        description = ''
+
+    # Get number of responses at school
+    school_mean = between_schools.loc[
+        between_schools['school_lab'] == chosen_school, 'mean'].to_list()[0]
+
+    # Display message if it was less than 10 (and so NaN)
+    if np.isnan(school_mean):
+        description += '''
+There were less than ten complete responses from these pupils at your school,
+so the results are not shown.
+'''
+    # Otherwise...
+    else:
+        # Get count of pupils who completed the topic questions
+        topic_count = int(between_schools.loc[
+            between_schools['school_lab'] == chosen_school,
+            'count'].to_list()[0])
+
+        # Get total responses and total schools (can just take first item as
+        # whole column will be the same value for each school)
+        total_responses = str(int(
+            between_schools['total_pupils'].to_list()[0]))
+        total_schools = str(int(
+            between_schools['group_n'].to_list()[0]))
+        description += f'''
+Your school had {topic_count} complete responses. Across
+Northern Devon, there were {total_responses} complete responses from
+{total_schools} schools. The average score for the pupils at your school,
+compared to other schools in Northern Devon, was:'''
+
+    # Add description to page
+    if output == 'streamlit':
+        st.markdown(description)
+    elif output == 'pdf':
+        content.append(markdown(description))
+
+    # If school wasn't NaN...
+    if not np.isnan(school_mean):
+        # Get RAG rating
+        devon_rag = between_schools.loc[
+            between_schools['school_lab'] == chosen_school, 'rag'].to_list()[0]
+        # Drop any schools that were NaN (i.e. n<10)
+        between_schools = between_schools[between_schools['mean'].notna()]
+        # Add the RAG result and ordered bar chart
+        if output == 'streamlit':
+            result_box(devon_rag)
+            details_ordered_bar(between_schools, chosen_school)
+        elif output == 'pdf':
+            content.append(result_box(devon_rag, 'pdf'))
+            content = details_ordered_bar(
+                school_scores=between_schools, school_name=chosen_school,
+                font_size=16, output='pdf', content=content)
+
+    if output == 'pdf':
+        return content
+
+
+def create_explore_topic_page(
+        chosen_variable_lab, topic_dict, df_scores, chosen_school,
+        chosen_group, df_prop, content):
+    '''
+    Add an explore results page with responses to a given topic to report HTML.
+
+    Parameters
+    ----------
+    chosen_variable_lab : string
+        Chosen variable in label format (e.g. 'Psychological wellbeing')
+    topic_dict : dictionary
+        Dictionary of topics where key is variable_lab and value is variable
+    df_scores : dataframe
+        Dataframe with scores for each topic
+    chosen_school : string
+        Name of the chosen school
+    chosen_group : string
+        Name of the chosen group to view results by - options are
+        'For all pupils', 'By year group', 'By gender', 'By FSM' or 'By SEN'
+    df_prop : dataframe
+        Dataframe with the proportion of pupils providing each response to each
+        survey question
+    content : list
+        Optional input used when output=='pdf', contains HTML for report.
+
+    Returns
+    -------
+    content : list
+        Optional return, used when output=='pdf', contains HTML for report.
+    '''
+    # Convert from variable_lab to variable
+    chosen_variable = topic_dict[chosen_variable_lab]
+
+    # Topic header and description
+    content = write_topic_intro(chosen_variable, chosen_variable_lab,
+                                df_scores, output='pdf', content=content)
+
+    # Section header and description
+    content = write_response_section_intro(
+        chosen_variable_lab, output='pdf', content=content)
+
+    # Get dataframe with results for the chosen variable, group and school
+    chosen_result = get_chosen_result(
+        chosen_variable, chosen_group, df_prop, chosen_school)
+
+    # Produce bar charts, plus their chart section descriptions and titles
+    content = create_bar_charts(
+        chosen_variable, chosen_result, output='pdf', content=content)
+
+    # Create dataframe based on chosen variable
+    between_schools, group_lab, order = filter_by_group(
+        df=df_scores, chosen_group=chosen_group, output='compare',
+        chosen_variable=chosen_variable+'_score')
+
+    # Write the comparison intro text
+    content = write_comparison_intro(
+        chosen_variable, chosen_variable_lab, score_descriptions,
+        output='pdf', content=content)
+
+    # Filter to each group (will just be 'all' if was for all pupils), then
+    # print the results and create the ordered bar chart for each
+    for group in order:
+        temp_content = []
+        # Filter to group and get result
+        group_result = between_schools[between_schools[group_lab] == group]
+        temp_content = write_comparison_result(
+            chosen_school, group_result, group, output='pdf',
+            content=temp_content)
+        # Insert temp_content into a div class and add to content
+        content.append(f'''
+    <div class='responses_container'>
+        {''.join(temp_content)}
+    </div>''')
+
+    return content
```

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/beewell_map.png` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/beewell_map.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/canva_people.png` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/canva_people.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/circle_divider.png` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/circle_divider.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/dashboard_home_section.png` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/dashboard_home_section.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/devices.png` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/devices.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/discovery-looking-researching.jpg` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/discovery-looking-researching.jpg`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/home_image_3_transparent.png` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/home_image_3_transparent.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/kailo_beewell_logo.png` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/kailo_beewell_logo.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/kailo_beewell_logo_padded.png` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/kailo_beewell_logo_padded.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/kailo_systems_adapted.png` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/kailo_systems_adapted.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/levelling-the-ground.jpg` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/levelling-the-ground.jpg`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/northern_devon.png` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/northern_devon.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/choice.png` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/choice.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/choice_crop.png` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/choice_crop.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/choose_one.png` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/choose_one.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/family.png` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/family.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/family_crop.png` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/family_crop.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/free_time.png` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/free_time.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/free_time_crop.png` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/free_time_crop.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/friends.png` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/friends.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/friends_crop.png` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/friends_crop.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/future.png` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/future.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/future_crop.png` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/future_crop.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/happy.png` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/happy.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/health.png` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/health.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/health_crop.png` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/health_crop.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/home.png` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/home.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/home_crop.png` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/home_crop.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/life.png` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/life.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/life_crop.png` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/life_crop.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/ok.png` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/ok.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/sad.png` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/sad.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/school.png` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/school.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/school_crop.png` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/school_crop.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/things.png` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/things.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/symbol_survey/things_crop.png` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/symbol_survey/things_crop.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/thinking.png` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/thinking.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images/young-person-journey.jpg` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images/young-person-journey.jpg`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/images.py` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/images.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-'''
-Helper functions for working with image files
-'''
-from tempfile import NamedTemporaryFile
-import base64
-from importlib.resources import files
-
-
-def convert_fig_to_html(fig, alt_text):
-    '''
-    Convert plotly fig to HTML by saving it as a temporary PNG file, and then
-    importing that and converting it to HTML which can produce the figure.
-
-    Parameters
-    ----------
-    fig : plotly figure object
-        Figure to be converted
-    alt_text : string
-        Alternative text for the figure
-
-    Returns
-    -------
-    img_tag : string
-        HTML to generate image
-    '''
-    # Adjust the layout so the figure proportions fit in the PDF report and are
-    # similar to streamlit, with automargin to ensure labels aren't cut off
-    fig.update_layout(
-        height=411,
-        width=600,
-        xaxis=dict(automargin=True),
-        yaxis=dict(automargin=True))
-
-    # Write image to a temporary file, then open again and convert to HTML
-    with NamedTemporaryFile(suffix='.png') as temp:
-        fig.write_image(temp)
-        temp.seek(0)
-        data_uri = base64.b64encode(
-            open(temp.name, 'rb').read()).decode('utf-8')
-
-    # Generate the image tag, inserting the HTML for the figure
-    img_tag = f'''
-<img src='data:image/png;base64,{data_uri}' alt='{alt_text}'>'''
-
-    return img_tag
-
-
-def get_image_path(filename):
-    '''
-    Get path for image in the kailo-beewell-dashboard package
-
-    Parameters
-    ----------
-    filename: string
-        Name of the image file within the package (e.g. 'image.png')
-
-    Returns
-    -------
-    img_path : string
-        Path to image within the package
-    '''
-    img_path = str(files('kailo_beewell_dashboard')
-                   .joinpath(f'images/{filename}'))
-    return img_path
+'''
+Helper functions for working with image files
+'''
+from tempfile import NamedTemporaryFile
+import base64
+from importlib.resources import files
+
+
+def convert_fig_to_html(fig, alt_text):
+    '''
+    Convert plotly fig to HTML by saving it as a temporary PNG file, and then
+    importing that and converting it to HTML which can produce the figure.
+
+    Parameters
+    ----------
+    fig : plotly figure object
+        Figure to be converted
+    alt_text : string
+        Alternative text for the figure
+
+    Returns
+    -------
+    img_tag : string
+        HTML to generate image
+    '''
+    # Adjust the layout so the figure proportions fit in the PDF report and are
+    # similar to streamlit, with automargin to ensure labels aren't cut off
+    fig.update_layout(
+        height=411,
+        width=600,
+        xaxis=dict(automargin=True),
+        yaxis=dict(automargin=True))
+
+    # Write image to a temporary file, then open again and convert to HTML
+    with NamedTemporaryFile(suffix='.png') as temp:
+        fig.write_image(temp)
+        temp.seek(0)
+        data_uri = base64.b64encode(
+            open(temp.name, 'rb').read()).decode('utf-8')
+
+    # Generate the image tag, inserting the HTML for the figure
+    img_tag = f'''
+<img src='data:image/png;base64,{data_uri}' alt='{alt_text}'>'''
+
+    return img_tag
+
+
+def get_image_path(filename):
+    '''
+    Get path for image in the kailo-beewell-dashboard package
+
+    Parameters
+    ----------
+    filename: string
+        Name of the image file within the package (e.g. 'image.png')
+
+    Returns
+    -------
+    img_path : string
+        Path to image within the package
+    '''
+    img_path = str(files('kailo_beewell_dashboard')
+                   .joinpath(f'images/{filename}'))
+    return img_path
```

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/import_data.py` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/import_data.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,114 +1,114 @@
-'''
-Helper function for importing the data from TiDB Cloud
-'''
-import numpy as np
-import pandas as pd
-import streamlit as st
-from tempfile import NamedTemporaryFile
-import pymysql
-
-
-def get_df(query, conn):
-    '''
-    Get data from the connected SQL database
-
-    Parameters:
-    -----------
-    query : string
-        SQL query
-    conn : connection object
-        Connection to the SQL database
-
-    Returns:
-    --------
-    df : pandas DataFrame
-        Dataframe produced from the query
-    '''
-    cursor = conn.cursor()
-    cursor.execute(query)
-    columns = [desc[0] for desc in cursor.description]
-    df = pd.DataFrame(cursor.fetchall(), columns=columns)
-    return df
-
-
-def import_tidb_data(survey_type):
-    '''
-    Imports all the datasets from TiDB Cloud, fixes any data type issues, and
-    saves the datasets to the session state.
-
-    Parameters
-    ----------
-    survey_type : string
-        Designates whether to import for 'standard' or 'symbol' survey
-    '''
-    # Define the session state variables (keys) and TIDB datasets (values)
-    if survey_type == 'standard':
-        items = {'scores_rag': 'standard_school_aggregate_scores_rag',
-                 'responses': 'standard_school_aggregate_responses',
-                 'counts': 'standard_school_overall_counts',
-                 'demographic': 'standard_school_aggregate_demographic'}
-    elif survey_type == 'symbol':
-        items = {'responses': 'symbol_school_aggregate_responses',
-                 'counts': 'symbol_school_overall_counts',
-                 'demographic': 'symbol_school_aggregate_demographic'}
-
-    # First, check if everything is in the session state - if so, don't need to
-    # connect, but if missing stuff, will want to connect
-    if not all([x in st.session_state for x in items.keys()]):
-
-        # Create temporary PEM file for setting up the connection
-        with NamedTemporaryFile(suffix='.pem') as temp:
-
-            # Write the temporary file
-            temp.write(st.secrets.tidb.root_cert.encode('utf-8'))
-
-            # Temporary file have pointer to current position in file - as we
-            # have just written, the pointer is at the end of the last write,
-            # so if you don't seek, you would read from the end of the file and
-            # find nothing
-            temp.seek(0)
-
-            # Set up connection manually, providing the temporary PEM file
-            # (as cannot use st.connection() without providing tempfile name
-            # in secrets)
-            conn = pymysql.connect(
-                host=st.secrets.tidb.host,
-                user=st.secrets.tidb.username,
-                password=st.secrets.tidb.password,
-                database=st.secrets.tidb.database,
-                port=st.secrets.tidb.port,
-                ssl_verify_cert=False,
-                ssl_verify_identity=False,
-                ssl_ca=temp.name
-            )
-
-            # Loop through each of the items
-            for key, value in items.items():
-
-                # Check if it is in the session state, and if not...
-                if key not in st.session_state:
-
-                    # Import data from TIDB cloud
-                    df = get_df(f'SELECT * FROM {value}', conn)
-
-                    # If dataset is scores with RAG ratings, convert
-                    # columns to numeric, and string 'nan' to actual np.nan
-                    if key == 'scores_rag':
-                        to_fix = ['mean', 'count', 'total_pupils',
-                                  'group_n', 'group_wt_mean', 'group_wt_std',
-                                  'lower', 'upper']
-                        for col in to_fix:
-                            df[col] = pd.to_numeric(df[col], errors='ignore')
-                        df['rag'] = df['rag'].replace('nan', np.nan)
-
-                    # If dataset is demographic, convert n_responses to numeric
-                    if key == 'demographic':
-                        df['n_responses'] = pd.to_numeric(df['n_responses'],
-                                                          errors='ignore')
-
-                    # If dataset is counts, convert counts to numeric
-                    if key == 'counts':
-                        df['count'] = pd.to_numeric(df['count'],
-                                                    errors='ignore')
-                    # Save into the session state
-                    st.session_state[key] = df
+'''
+Helper function for importing the data from TiDB Cloud
+'''
+import numpy as np
+import pandas as pd
+import streamlit as st
+from tempfile import NamedTemporaryFile
+import pymysql
+
+
+def get_df(query, conn):
+    '''
+    Get data from the connected SQL database
+
+    Parameters:
+    -----------
+    query : string
+        SQL query
+    conn : connection object
+        Connection to the SQL database
+
+    Returns:
+    --------
+    df : pandas DataFrame
+        Dataframe produced from the query
+    '''
+    cursor = conn.cursor()
+    cursor.execute(query)
+    columns = [desc[0] for desc in cursor.description]
+    df = pd.DataFrame(cursor.fetchall(), columns=columns)
+    return df
+
+
+def import_tidb_data(survey_type):
+    '''
+    Imports all the datasets from TiDB Cloud, fixes any data type issues, and
+    saves the datasets to the session state.
+
+    Parameters
+    ----------
+    survey_type : string
+        Designates whether to import for 'standard' or 'symbol' survey
+    '''
+    # Define the session state variables (keys) and TIDB datasets (values)
+    if survey_type == 'standard':
+        items = {'scores_rag': 'standard_school_aggregate_scores_rag',
+                 'responses': 'standard_school_aggregate_responses',
+                 'counts': 'standard_school_overall_counts',
+                 'demographic': 'standard_school_aggregate_demographic'}
+    elif survey_type == 'symbol':
+        items = {'responses': 'symbol_school_aggregate_responses',
+                 'counts': 'symbol_school_overall_counts',
+                 'demographic': 'symbol_school_aggregate_demographic'}
+
+    # First, check if everything is in the session state - if so, don't need to
+    # connect, but if missing stuff, will want to connect
+    if not all([x in st.session_state for x in items.keys()]):
+
+        # Create temporary PEM file for setting up the connection
+        with NamedTemporaryFile(suffix='.pem') as temp:
+
+            # Write the temporary file
+            temp.write(st.secrets.tidb.root_cert.encode('utf-8'))
+
+            # Temporary file have pointer to current position in file - as we
+            # have just written, the pointer is at the end of the last write,
+            # so if you don't seek, you would read from the end of the file and
+            # find nothing
+            temp.seek(0)
+
+            # Set up connection manually, providing the temporary PEM file
+            # (as cannot use st.connection() without providing tempfile name
+            # in secrets)
+            conn = pymysql.connect(
+                host=st.secrets.tidb.host,
+                user=st.secrets.tidb.username,
+                password=st.secrets.tidb.password,
+                database=st.secrets.tidb.database,
+                port=st.secrets.tidb.port,
+                ssl_verify_cert=False,
+                ssl_verify_identity=False,
+                ssl_ca=temp.name
+            )
+
+            # Loop through each of the items
+            for key, value in items.items():
+
+                # Check if it is in the session state, and if not...
+                if key not in st.session_state:
+
+                    # Import data from TIDB cloud
+                    df = get_df(f'SELECT * FROM {value}', conn)
+
+                    # If dataset is scores with RAG ratings, convert
+                    # columns to numeric, and string 'nan' to actual np.nan
+                    if key == 'scores_rag':
+                        to_fix = ['mean', 'count', 'total_pupils',
+                                  'group_n', 'group_wt_mean', 'group_wt_std',
+                                  'lower', 'upper']
+                        for col in to_fix:
+                            df[col] = pd.to_numeric(df[col], errors='ignore')
+                        df['rag'] = df['rag'].replace('nan', np.nan)
+
+                    # If dataset is demographic, convert n_responses to numeric
+                    if key == 'demographic':
+                        df['n_responses'] = pd.to_numeric(df['n_responses'],
+                                                          errors='ignore')
+
+                    # If dataset is counts, convert counts to numeric
+                    if key == 'counts':
+                        df['count'] = pd.to_numeric(df['count'],
+                                                    errors='ignore')
+                    # Save into the session state
+                    st.session_state[key] = df
```

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/page_setup.py` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/page_setup.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-'''
-Helper functions for setting up the page and page formatting.
-'''
-import base64
-import streamlit as st
-from importlib.resources import files
-
-
-def page_logo():
-    '''
-    Create logo to go above the pages in the sidebar
-    '''
-    # Set up logo for display in markdown, which we use instead of st.image()
-    # to allow inline display and alt_text
-    img_path = str(files('kailo_beewell_dashboard')
-                   .joinpath('images/kailo_beewell_logo_padded.png'))
-    file = open(img_path, 'rb')
-    contents = file.read()
-    url = base64.b64encode(contents).decode('utf-8')
-    file.close()
-
-    # Display logo
-    st.markdown(f'''
-<style>
-    [data-testid='stSidebarNav'] {{
-        background-image: url('data:image/png;base64,{url}');
-        background-repeat: no-repeat;
-        padding-top: 110px; /* Move page names down */
-        background-position: 0px 50px; /* Move image down */
-        background-size: 240px;
-    }}
-</style>
-''', unsafe_allow_html=True)
-
-
-def page_setup(type):
-    '''
-    Set up page to standard conditions, with layout as specified
-
-    Parameters
-    ----------
-    type : string
-        Survey type - 'standard', 'symbol', or 'public'
-    '''
-    # Set up streamlit page parameters
-    st.set_page_config(
-        page_title='#BeeWell School Dashboard',
-        page_icon='🐝',
-        initial_sidebar_state='expanded',
-        layout='centered',
-        menu_items={'About': f'''
-{type.capitalize()} #BeeWell survey dashboard for North Devon and Torridge in
-2023/24 as part of Kailo.'''})
-
-    # Import CSS style
-    css_path = str(files('kailo_beewell_dashboard').joinpath('css/style.css'))
-    with open(css_path) as css:
-        st.markdown(f'<style>{css.read()}</style>', unsafe_allow_html=True)
-
-    # Add page logo
-    page_logo()
-
-
-def blank_lines(n):
-    '''
-    Create blank lines on the page of the dashboard
-
-    Parameters
-    ----------
-    n : int
-        Number of blank lines to create
-    '''
-    counter = 0
-    while counter < n:
-        st.text('')
-        counter += 1
-
-
-def page_footer(school):
-    '''
-    Create a footer for each page
-
-    Parameters
-    ----------
-    school : string
-        Name of the chosen school for this dashboard
-    '''
-    blank_lines(2)
-    st.divider()
-    st.markdown(f'''
-<p style='font-size: 12px;'>
-This dashboard shows results for pupils at {school}. If you have any
-questions, you can get in touch with the Kailo team by emailing
-kailobeewell@dartington.org.uk.''', unsafe_allow_html=True)
+'''
+Helper functions for setting up the page and page formatting.
+'''
+import base64
+import streamlit as st
+from importlib.resources import files
+
+
+def page_logo():
+    '''
+    Create logo to go above the pages in the sidebar
+    '''
+    # Set up logo for display in markdown, which we use instead of st.image()
+    # to allow inline display and alt_text
+    img_path = str(files('kailo_beewell_dashboard')
+                   .joinpath('images/kailo_beewell_logo_padded.png'))
+    file = open(img_path, 'rb')
+    contents = file.read()
+    url = base64.b64encode(contents).decode('utf-8')
+    file.close()
+
+    # Display logo
+    st.markdown(f'''
+<style>
+    [data-testid='stSidebarNav'] {{
+        background-image: url('data:image/png;base64,{url}');
+        background-repeat: no-repeat;
+        padding-top: 110px; /* Move page names down */
+        background-position: 0px 50px; /* Move image down */
+        background-size: 240px;
+    }}
+</style>
+''', unsafe_allow_html=True)
+
+
+def page_setup(type):
+    '''
+    Set up page to standard conditions, with layout as specified
+
+    Parameters
+    ----------
+    type : string
+        Survey type - 'standard', 'symbol', or 'public'
+    '''
+    # Set up streamlit page parameters
+    st.set_page_config(
+        page_title='#BeeWell School Dashboard',
+        page_icon='🐝',
+        initial_sidebar_state='expanded',
+        layout='centered',
+        menu_items={'About': f'''
+{type.capitalize()} #BeeWell survey dashboard for North Devon and Torridge in
+2023/24 as part of Kailo.'''})
+
+    # Import CSS style
+    css_path = str(files('kailo_beewell_dashboard').joinpath('css/style.css'))
+    with open(css_path) as css:
+        st.markdown(f'<style>{css.read()}</style>', unsafe_allow_html=True)
+
+    # Add page logo
+    page_logo()
+
+
+def blank_lines(n):
+    '''
+    Create blank lines on the page of the dashboard
+
+    Parameters
+    ----------
+    n : int
+        Number of blank lines to create
+    '''
+    counter = 0
+    while counter < n:
+        st.text('')
+        counter += 1
+
+
+def page_footer(school):
+    '''
+    Create a footer for each page
+
+    Parameters
+    ----------
+    school : string
+        Name of the chosen school for this dashboard
+    '''
+    blank_lines(2)
+    st.divider()
+    st.markdown(f'''
+<p style='font-size: 12px;'>
+This dashboard shows results for pupils at {school}. If you have any
+questions, you can get in touch with the Kailo team by emailing
+kailobeewell@dartington.org.uk.''', unsafe_allow_html=True)
```

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/reshape_data.py` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/reshape_data.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,192 +1,192 @@
-'''
-Helper functions for reshaping data or extracting a certain element from the
-data, often used across multiple different pages
-'''
-import pandas as pd
-from ast import literal_eval
-import numpy as np
-
-
-def filter_by_group(df, chosen_group, output, chosen_school=None,
-                    chosen_variable=None, survey_type='standard'):
-    '''
-    Filter dataframe so just contains rows relevant for chosen group (either
-    results from all pupils, or from the two chosen groups) and school
-
-    Parameters
-    ----------
-    df : dataframe
-        Dataframe to be filtered
-    chosen_group : string
-        The group for results to be viewed by - one of: 'For all pupils',
-        'By year group', 'By gender', 'By FSM', or 'By SEN'
-    output : string
-        Defines where data will be used - either 'explore' or 'summary'
-    chosen_school : string
-        Optional input, name of a school to filter to as well
-    chosen_variable : string
-        Optional input, name of a variable to filter to as well
-    survey_type : string
-        Designates whether this filtering is for 'standard' or 'symbol' survey
-
-    Returns
-    -------
-    Depends on chosen output
-    '''
-    # Set default values
-    year_group = ['All']
-    gender = ['All']
-    fsm = ['All']
-    sen = ['All']
-
-    # These are default values that each page will need to avoid errors
-    # (explore uses it - it could use any of them - and summary doesn't)
-    if output == 'explore':
-        group_lab = 'year_group_lab'
-    elif output == 'summary':
-        group_lab = None
-        order = None
-    elif output == 'compare':
-        group_lab = 'year_group_lab'
-        order = ['All']
-
-    # Depending on chosen breakdown, alter one of the above variables
-    # If the chosen group was All, then no changes are made, as this is default
-    if chosen_group == 'By year group':
-        group_lab = 'year_group_lab'
-        if survey_type == 'standard':
-            year_group = ['Year 8', 'Year 10']
-            order = ['Year 8', 'Year 10']
-        elif survey_type == 'symbol':
-            year_group = ['Year 7', 'Year 8', 'Year 9', 'Year 10', 'Year 11']
-            order = ['Year 7', 'Year 8', 'Year 9', 'Year 10', 'Year 11']
-    elif chosen_group == 'By gender':
-        group_lab = 'gender_lab'
-        gender = ['Girl', 'Boy']
-        order = ['Girl', 'Boy']
-    elif chosen_group == 'By FSM':
-        group_lab = 'fsm_lab'
-        fsm = ['FSM', 'Non-FSM']
-        order = ['FSM', 'Non-FSM']
-    elif chosen_group == 'By SEN':
-        group_lab = 'sen_lab'
-        sen = ['SEN', 'Non-SEN']
-        order = ['SEN', 'Non-SEN']
-
-    # Filter to chosen group (exc. SEN filter for symbol survey)
-    chosen = df[
-        (df['year_group_lab'].isin(year_group)) &
-        (df['gender_lab'].isin(gender)) &
-        (df['fsm_lab'].isin(fsm))]
-    if survey_type == 'standard':
-        chosen = chosen[chosen['sen_lab'].isin(sen)]
-
-    # Filter to chosen school, if relevant
-    if chosen_school is not None:
-        chosen = chosen[chosen['school_lab'] == chosen_school]
-
-    # Filter to chosen variable, if relevant
-    if chosen_variable is not None:
-        chosen = chosen[chosen['variable'] == chosen_variable]
-
-    # Return the relevant results for the given output
-    if output == 'explore':
-        return chosen, group_lab
-    elif output == 'summary':
-        return chosen, group_lab, order
-    elif output == 'compare':
-        return chosen, group_lab, order
-
-
-def extract_nested_results(chosen, group_lab=None, plot_group=False):
-    '''
-    Extract lists of results that were stored in dataframe.
-    e.g. ['Yes', 'No'], [20, 80], [2, 8] in the original data will become
-    seperate columns with [Yes, 20, 2] and [No, 80, 8]
-
-    Parameters
-    ----------
-    chosen : dataframe
-        Dataframe with the nested lists to be extracted
-    group_lab : string
-        Name of chosen group (e.g. gender_lab, fsm_lab) - optional input,
-        default None.
-    plot_group : boolean
-        Whether there is a plot_group column to include - default False.
-    '''
-    # Initalise empty list to store rows
-    df_list = []
-
-    # Loop through each of the rows in the dataframe
-    for index, row in chosen.iterrows():
-
-        # Extract results as long as it isn't NaN (e.g. NaN when n<10)
-        if ~np.isnan(row.n_responses):
-            # Literal_eval means the string lists become actual lists
-            df = pd.DataFrame(
-                zip(literal_eval(row['cat'].replace('nan', 'None')),
-                    literal_eval(row['cat_lab']),
-                    literal_eval(row['percentage'].replace('nan', 'None')),
-                    literal_eval(row['count'].replace('nan', 'None'))),
-                columns=['cat', 'cat_lab', 'percentage', 'count'])
-            # Replace NaN with max number so stays at end of sequence
-            df['cat'] = df['cat'].fillna(df['cat'].max()+1)
-            # Add the string columns (no extraction needed)
-            df['measure'] = row['measure']
-            df['measure_lab'] = row['measure_lab']
-            if group_lab is not None:
-                df['group'] = row[group_lab]
-            if plot_group:
-                df['plot_group'] = row['plot_group']
-            df_list.append(df)
-
-        # As we still want a bar when n<10, we create a record still but label
-        # it to indicate n<10
-        else:
-            df = row.to_frame().T[['measure', 'measure_lab']]
-            if group_lab is not None:
-                df['group'] = row[group_lab]
-            if plot_group:
-                df['plot_group'] = row['plot_group']
-            df['cat'] = 0
-            df['cat_lab'] = 'Less than 10 responses'
-            df['count'] = np.nan
-            df['percentage'] = 100
-            df_list.append(df)
-
-    # Combine into a single dataframe
-    chosen_result = pd.concat(df_list)
-
-    return chosen_result
-
-
-def get_school_size(counts, school, survey_type='standard'):
-    '''
-    Get the total pupil number for a given school
-
-    Parameters
-    ----------
-    counts : dataframe
-        Dataframe containing the count of pupils at each school
-    school : string
-        Name of the school
-    survey_type : string
-        Designates whether this filtering is for 'standard' or 'symbol' survey
-
-    Returns
-    -------
-    school_size : integer
-        Total number of pupils at school (who answered at least one question)
-    '''
-    # Filter to relevant school
-    school_counts = counts.loc[counts['school_lab'] == school]
-
-    # Find total school size
-    df = school_counts[(school_counts['year_group_lab'] == 'All') &
-                       (school_counts['gender_lab'] == 'All') &
-                       (school_counts['fsm_lab'] == 'All')]
-    if survey_type == 'standard':
-        df = df[df['sen_lab'] == 'All']
-    school_size = df['count'].values[0].astype(int)
-
-    return school_size
+'''
+Helper functions for reshaping data or extracting a certain element from the
+data, often used across multiple different pages
+'''
+import pandas as pd
+from ast import literal_eval
+import numpy as np
+
+
+def filter_by_group(df, chosen_group, output, chosen_school=None,
+                    chosen_variable=None, survey_type='standard'):
+    '''
+    Filter dataframe so just contains rows relevant for chosen group (either
+    results from all pupils, or from the two chosen groups) and school
+
+    Parameters
+    ----------
+    df : dataframe
+        Dataframe to be filtered
+    chosen_group : string
+        The group for results to be viewed by - one of: 'For all pupils',
+        'By year group', 'By gender', 'By FSM', or 'By SEN'
+    output : string
+        Defines where data will be used - either 'explore' or 'summary'
+    chosen_school : string
+        Optional input, name of a school to filter to as well
+    chosen_variable : string
+        Optional input, name of a variable to filter to as well
+    survey_type : string
+        Designates whether this filtering is for 'standard' or 'symbol' survey
+
+    Returns
+    -------
+    Depends on chosen output
+    '''
+    # Set default values
+    year_group = ['All']
+    gender = ['All']
+    fsm = ['All']
+    sen = ['All']
+
+    # These are default values that each page will need to avoid errors
+    # (explore uses it - it could use any of them - and summary doesn't)
+    if output == 'explore':
+        group_lab = 'year_group_lab'
+    elif output == 'summary':
+        group_lab = None
+        order = None
+    elif output == 'compare':
+        group_lab = 'year_group_lab'
+        order = ['All']
+
+    # Depending on chosen breakdown, alter one of the above variables
+    # If the chosen group was All, then no changes are made, as this is default
+    if chosen_group == 'By year group':
+        group_lab = 'year_group_lab'
+        if survey_type == 'standard':
+            year_group = ['Year 8', 'Year 10']
+            order = ['Year 8', 'Year 10']
+        elif survey_type == 'symbol':
+            year_group = ['Year 7', 'Year 8', 'Year 9', 'Year 10', 'Year 11']
+            order = ['Year 7', 'Year 8', 'Year 9', 'Year 10', 'Year 11']
+    elif chosen_group == 'By gender':
+        group_lab = 'gender_lab'
+        gender = ['Girl', 'Boy']
+        order = ['Girl', 'Boy']
+    elif chosen_group == 'By FSM':
+        group_lab = 'fsm_lab'
+        fsm = ['FSM', 'Non-FSM']
+        order = ['FSM', 'Non-FSM']
+    elif chosen_group == 'By SEN':
+        group_lab = 'sen_lab'
+        sen = ['SEN', 'Non-SEN']
+        order = ['SEN', 'Non-SEN']
+
+    # Filter to chosen group (exc. SEN filter for symbol survey)
+    chosen = df[
+        (df['year_group_lab'].isin(year_group)) &
+        (df['gender_lab'].isin(gender)) &
+        (df['fsm_lab'].isin(fsm))]
+    if survey_type == 'standard':
+        chosen = chosen[chosen['sen_lab'].isin(sen)]
+
+    # Filter to chosen school, if relevant
+    if chosen_school is not None:
+        chosen = chosen[chosen['school_lab'] == chosen_school]
+
+    # Filter to chosen variable, if relevant
+    if chosen_variable is not None:
+        chosen = chosen[chosen['variable'] == chosen_variable]
+
+    # Return the relevant results for the given output
+    if output == 'explore':
+        return chosen, group_lab
+    elif output == 'summary':
+        return chosen, group_lab, order
+    elif output == 'compare':
+        return chosen, group_lab, order
+
+
+def extract_nested_results(chosen, group_lab=None, plot_group=False):
+    '''
+    Extract lists of results that were stored in dataframe.
+    e.g. ['Yes', 'No'], [20, 80], [2, 8] in the original data will become
+    seperate columns with [Yes, 20, 2] and [No, 80, 8]
+
+    Parameters
+    ----------
+    chosen : dataframe
+        Dataframe with the nested lists to be extracted
+    group_lab : string
+        Name of chosen group (e.g. gender_lab, fsm_lab) - optional input,
+        default None.
+    plot_group : boolean
+        Whether there is a plot_group column to include - default False.
+    '''
+    # Initalise empty list to store rows
+    df_list = []
+
+    # Loop through each of the rows in the dataframe
+    for index, row in chosen.iterrows():
+
+        # Extract results as long as it isn't NaN (e.g. NaN when n<10)
+        if ~np.isnan(row.n_responses):
+            # Literal_eval means the string lists become actual lists
+            df = pd.DataFrame(
+                zip(literal_eval(row['cat'].replace('nan', 'None')),
+                    literal_eval(row['cat_lab']),
+                    literal_eval(row['percentage'].replace('nan', 'None')),
+                    literal_eval(row['count'].replace('nan', 'None'))),
+                columns=['cat', 'cat_lab', 'percentage', 'count'])
+            # Replace NaN with max number so stays at end of sequence
+            df['cat'] = df['cat'].fillna(df['cat'].max()+1)
+            # Add the string columns (no extraction needed)
+            df['measure'] = row['measure']
+            df['measure_lab'] = row['measure_lab']
+            if group_lab is not None:
+                df['group'] = row[group_lab]
+            if plot_group:
+                df['plot_group'] = row['plot_group']
+            df_list.append(df)
+
+        # As we still want a bar when n<10, we create a record still but label
+        # it to indicate n<10
+        else:
+            df = row.to_frame().T[['measure', 'measure_lab']]
+            if group_lab is not None:
+                df['group'] = row[group_lab]
+            if plot_group:
+                df['plot_group'] = row['plot_group']
+            df['cat'] = 0
+            df['cat_lab'] = 'Less than 10 responses'
+            df['count'] = np.nan
+            df['percentage'] = 100
+            df_list.append(df)
+
+    # Combine into a single dataframe
+    chosen_result = pd.concat(df_list)
+
+    return chosen_result
+
+
+def get_school_size(counts, school, survey_type='standard'):
+    '''
+    Get the total pupil number for a given school
+
+    Parameters
+    ----------
+    counts : dataframe
+        Dataframe containing the count of pupils at each school
+    school : string
+        Name of the school
+    survey_type : string
+        Designates whether this filtering is for 'standard' or 'symbol' survey
+
+    Returns
+    -------
+    school_size : integer
+        Total number of pupils at school (who answered at least one question)
+    '''
+    # Filter to relevant school
+    school_counts = counts.loc[counts['school_lab'] == school]
+
+    # Find total school size
+    df = school_counts[(school_counts['year_group_lab'] == 'All') &
+                       (school_counts['gender_lab'] == 'All') &
+                       (school_counts['fsm_lab'] == 'All')]
+    if survey_type == 'standard':
+        df = df[df['sen_lab'] == 'All']
+    school_size = df['count'].values[0].astype(int)
+
+    return school_size
```

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/reuse_text.py` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/reuse_text.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,263 +1,263 @@
-'''
-Dictionary with large sections of descriptive text - mainly text that is from
-the About page (some of which goes on PDF report introduction) - but also
-includes caveat about comparisons (from PDF report introduction and from
-various pages of dashboard like summary and explore results). These are also
-text that are reused between different versions of the dashboard (e.g. standard
-and symbol).
-'''
-
-reuse_text = {
-
-    # Introduction for the About page
-    'about_intro': '''
-This page has lots of helpful information about the research projects (Kailo
-and #BeeWell), as well as advice on using and accessing this dashboard, and
-some background information around young people's wellbeing.''',
-
-    # Description of the Kailo project
-    'kailo': '''
-Our aim is to help local communities, young people and public service
-partnerships better understand and address the root causes (and wider
-determinants) of young people's mental health.
-
-We're made up of leading academics, designers and practitioners, dedicated to
-working alongside communities in specific localities. Together, we will test
-and co-design evidence-based responses (in a 'framework') to these root causes,
-over the next four years.
-
-Our model is formed of three key stages:
-* **Early Discovery** - here, we build strong and trusted relationships with
-local partners with an aim to understand what matters locally thus, forming
-communities around youth- and community-centred priorities
-* **Deeper Discovery and Codesign** - this stage, which we're in currently,
-sees us codesign systemic responses to social determinants.
-* **Prototyping, Implementation and Testing** - this is where the learning is
-applied, integrating the codesigned responses with the local system,
-prototyping them and making iterative refinements along the way.
-
-To find out more about Kailo, check out our site: https://kailo.community/''',
-
-    # Sample (used for public and standard school dashboard)
-    'sample': '''
-This year, pupils in Years 8 and 10 at **seven secondary schools** from across
-North Devon and Torridge completed the standard version of the #BeeWell survey.
-A symbol version of the survey was also completed by pupils in Years 7 to 11
-from **two non-mainstream schools** in Northern Devon.''',
-
-    # Sample (used for symbol school dashboard)
-    'sample_symbol': '''
-This years, pupils in Years 7 to 11 at **two non-mainstream schools** in North
-Devon and Torridge completed the symbol version of the #BeeWell survey. A
-longer, standard version of the survey was also completed by pupils in Years
-8 and 10 at **seven mainstream secondary schools** in Northern Devon.''',
-
-    # Content of the standard survey
-    'standard_content': '''
-The survey contained questions to measure wellbeing and the factors that might
-impact it. Survey topics included:
-* 🌱 **Feelings about life** - autonomy, life satisfaction, optimism
-* 🧍 **Thoughts and feelings about self** - psychological wellbeing,
-self-esteem, stress, feelings around appearance
-* 😟 **Feeling down** - negative affect, loneliness, supporting own wellbeing
-* 🧘‍♂️ **Health and routines** - sleep, physical activity
-* 🕰️ **Free time** - social media use, places to go and things to do
-* 🧑‍🤝‍🧑 **Relationships** - talking about feelings, acceptance, school
-connection, support from staff, support from parents/carers, experiences of
-discrimintation, support from friends, relative wealth and bulllying
-* 🏠 **Environment** - feelings about home and local area, including future work
-and education opportunities, and climate change
-* 👨‍👩‍👧‍👦 **Demographics and experiences** - gender, transgender, sexual
-orientation, neurodivergence, family background, care experience and young
-carers''',
-
-    # Design of standard survey
-    'standard_design': '''
-The survey delivered in Northern Devon was adapted from the first #BeeWell
-survey in Greater Manchester. That survey was developed through engagements
-with over 150 young people from 15 different schools to understand what
-wellbeing means to young people, what influences their wellbeing, and what
-makes them thrive.
-
-In Devon, we have adapted the survey to help it reflect the
-priorities of young people in this area. Topics were based on conversations
-across North Devon and Torridge with 195 young people and over 100 local actors
-including: system leaders, practitioners, and people at 45 organisations
-working with young people and broader communities. We have spoken with young
-people and school staff in Northern Devon, as well as researchers and public
-health professionals, amongst others, to choose, adapt and/or develop
-appropriate questions for the survey. We'd like to extend our thanks to
-everyone who supported this process.''',
-
-    # Design of the symbol survey
-    'symbol_design': '''
-The survey delivered in Northern Devon is the same as that first designed and
-delivered by the #BeeWell team in Greater Manchester. They worked with staff
-in special school settings to co-design a symbol version of the #BeeWell survey
-that would be accessible to young people with severe learning difficulties or
-profound and multiple learning disabilities. Using The Children's Society's
-'Good Childhood Index' for inspiration, they created a 10-item survey using the
-Widgit symbol system with simplified response options.''',
-
-    # Other #BeeWell sites
-    'other_beewell_sites': '''
-#BeeWell surveys have also been completed by pupils at schools in Hampshire,
-Greater Manchester, the London borough of Havering, and Milton Keynes.
-
-In 2023-24, **over 38,000 young people** completed a survey, with **nearly 300
-schools** having now taken part in #BeeWell.
-
-You can find out more about other sites at https://beewellprogramme.org/.''',
-
-    # Data used to create the dashboard (standard dashboard)
-    'standard_data': '''
-This dashboard presents the results from pupils at your school who completed
-the survey. To give context to these results, we've added comparisons against
-pupils from schools across Northern Devon.
-
-The survey responses were combined with data shared by the local authority such
-as free school meal eligibility and special education needs to give further
-insight into responses.''',
-
-    # Data used to create the dashboard (symbol dashboard)
-    'symbol_data': '''
-This dashboard presents the results from pupils at your school who completed
-the survey.
-
-The survey responses were combined with data shared by the local authority such
-as free school meal eligibility and special education needs to give further
-insight into responses.''',
-
-    # Data used to create the dashboard (public dashboard)
-    'public_data': '''
-This dashboard presents results from pupils at mainstream and non-mainstream
-schools who completed the survey.
-
-The survey responses were combined with data shared by the local authority such
-as free school meal eligibility and special education needs to give further
-insight into responses.''',
-
-    # How to use the results from this report
-    'how_to_use_results': '''
-These data can provide a useful starting point for discussions about the needs
-of your school population and priority areas for development and improvement.
-It can also be useful in considering areas of strengths and/or helping pupils
-reflect on their positive qualities.
-
-Data in your #BeeWell report may be useful in indicating progress against
-targets in your School Improvement Plan or help to identify future target
-areas. It may help to identify areas of priority for staff training or be used
-as context when considering academic data for participating year groups. It can
-also be used as independent evidence in the context of an Ofsted inspection.
-
-Finally, young people consulted during the set-up of #BeeWell in Greater
-Manchester felt strongly that pupils should be included in discussions around
-feedback, particularly to plan activities and approaches to raise awareness of
-strengths or difficulties the #BeeWell survey may highlight. They suggested
-involving a range of students (not just those involved in school councils) in
-planning how to raise awareness about wellbeing and to support the needs of
-young people.''',
-
-    # Viewing dashboard on different devices
-    'view_devices': '''
-Yes - this dashboard will resize so you should be able to access it on a range
-of devices (computer/laptop, tablet, phone, etc).''',
-
-    # Will there be support for interpreting and actioning on results?
-    'dashboard_support': '''
-Yes - Child Outcomes Research Consortium (CORC) has been funded to provide
-seminars and 1:1 support to schools in Northern Devon, to help you understand
-how to navigate the dashboard, interpret results, and suggest feedback in the
-development of action plans. You should receive information about this via
-email, but if you have not or have any questions, please contact us at
-kailobeewell@dartington.org.uk.''',
-
-    # Context of what already know about YP wellbeing
-    'wellbeing_context': '''
-* The peak age of onset of mental health difficulties is 14.5 years.<sup>[1]
-</sup>
-* Mental health and wellbeing in adolescence predicts adult health, labour
-market and other important outcomes.<sup>[2]</sup>
-* The wellbeing of adolescents has decreased in the last two decades, while the
-prevalence of mental health difficulties among them has increased.<sup>[3,4]
-</sup>
-* A recent international study ranked the UK’s young people fourth from bottom
-across nearly 80 countries in terms of life satisfaction.<sup>[5,6]</sup>
-* Young people’s mental health and wellbeing can be influenced by multiple
-drivers, including their health and routines, hobbies and entertainment,
-relationships, school, environment and society, and how they feel about their
-future.<sup>[7]</sup>
-
-<p style='font-size: 12px;'>
-References:<br>
-[1] Solmi, M. et al (2021). Age at onset of mental disorders worldwide:
-large-scale meta-analysis of 192 epidemiological studies. Molecular Psychiatry,
-Online First. Available at: https://www.nature.com/articles/s41380-021-01161-7
-<br>
-[2] Goodman A, Joshi H, Nasim B, Tyler C (2015). Social and emotional skills in
-childhood and their long-term effects on adult life. London: EIF. Available at:
-https://www.eif.org.uk/report/social-and-emotional-skills-in-childhood-and-thei
-r-long-term-effects-on-adult-life.<br>
-[3] Children’s Society (2021). The Good Childhood Report 2021. London:
-Children's Society. Available at: https://www.childrenssociety.org.uk/informati
-on/professionals/resources/good-childhood-report-2021<br>
-[4] NHS Digital (2021). Mental health of children and young people in England,
-2021 – wave 2 follow up to the 2017 survey. London: NHS Digital. Available at:
-https://digital.nhs.uk/data-and-information/publications/statistical/mental-hea
-lth-of-children-and-young-people-in-england/2021-follow-up-to-the-2017-survey
-<br>
-[5] Office for Economic Cooperation and Development (2019). Programme for
-International Student Assessment (PISA) results. Paris: OECD. Available at:
-https://www.oecd.org/publications/pisa-2018-results-volume-iii-acd78851-en.htm
-<br>
-[6] Marquez J, Long, E (2021). A Global Decline in Adolescents' Subjective
-Well-Being: a Comparative Study Exploring Patterns of Change in the Life
-Satisfaction of 15-Year-Old Students in 46 Countries. Child Ind Res 14,
-1251–1292 (2021). Available at: https://doi.org/10.1007/s12187-020-09788-8<br>
-[7] #BeeWell Programme Team (2021). #BeeWell survey. Manchester: University of
-Manchester. Available at: https://gmbeewell.org/wp-content/uploads/2021/09/BeeW
-ell-Questionnaires-Booklet.pdf</p>'''
-}
-
-
-def caution_comparing(type):
-    '''
-    Produce section of text providing caution for when making comparisons
-    between schools.
-
-    Parameters
-    ----------
-    type : string
-        Whether this is for 'school' or 'area' dashboard
-
-    Returns
-    -------
-    statement : string
-        Text on caution when comparing
-    '''
-    if type == 'school':
-        unit = 'schools'
-        participants = 'pupils'
-    elif type == 'area':
-        unit = 'areas'
-        participants = 'young people'
-    statement = f'''
-Always be mindful when making comparisons between different {unit}. There are
-a number of factors that could explain differences in scores (whether you are
-above average, average, or below average). These include:
-
-* Random chance ('one-off' findings).
-* Differences in the socio-economic characteristics of {participants} and the
-areas where they live (e.g. income, education, ethnicity, access to services
-and amenities).
-* The number of {participants} taking part - {unit} that are much smaller are
-more likely to have more "extreme" results (i.e. above or below average),
-whilst {unit} with a larger number of {participants} who took part are more
-likely to see average results.
-
-It's also worth noting that the score will only include results from
-{participants} who completed each of the questions used to calculate that
-topic, and so does not include any reflection of results from {participants}
-who did not complete some or all of the questions for that topic.
-'''
-    return statement
+'''
+Dictionary with large sections of descriptive text - mainly text that is from
+the About page (some of which goes on PDF report introduction) - but also
+includes caveat about comparisons (from PDF report introduction and from
+various pages of dashboard like summary and explore results). These are also
+text that are reused between different versions of the dashboard (e.g. standard
+and symbol).
+'''
+
+reuse_text = {
+
+    # Introduction for the About page
+    'about_intro': '''
+This page has lots of helpful information about the research projects (Kailo
+and #BeeWell), as well as advice on using and accessing this dashboard, and
+some background information around young people's wellbeing.''',
+
+    # Description of the Kailo project
+    'kailo': '''
+Our aim is to help local communities, young people and public service
+partnerships better understand and address the root causes (and wider
+determinants) of young people's mental health.
+
+We're made up of leading academics, designers and practitioners, dedicated to
+working alongside communities in specific localities. Together, we will test
+and co-design evidence-based responses (in a 'framework') to these root causes,
+over the next four years.
+
+Our model is formed of three key stages:
+* **Early Discovery** - here, we build strong and trusted relationships with
+local partners with an aim to understand what matters locally thus, forming
+communities around youth- and community-centred priorities
+* **Deeper Discovery and Codesign** - this stage, which we're in currently,
+sees us codesign systemic responses to social determinants.
+* **Prototyping, Implementation and Testing** - this is where the learning is
+applied, integrating the codesigned responses with the local system,
+prototyping them and making iterative refinements along the way.
+
+To find out more about Kailo, check out our site: https://kailo.community/''',
+
+    # Sample (used for public and standard school dashboard)
+    'sample': '''
+This year, pupils in Years 8 and 10 at **seven secondary schools** from across
+North Devon and Torridge completed the standard version of the #BeeWell survey.
+A symbol version of the survey was also completed by pupils in Years 7 to 11
+from **two non-mainstream schools** in Northern Devon.''',
+
+    # Sample (used for symbol school dashboard)
+    'sample_symbol': '''
+This years, pupils in Years 7 to 11 at **two non-mainstream schools** in North
+Devon and Torridge completed the symbol version of the #BeeWell survey. A
+longer, standard version of the survey was also completed by pupils in Years
+8 and 10 at **seven mainstream secondary schools** in Northern Devon.''',
+
+    # Content of the standard survey
+    'standard_content': '''
+The survey contained questions to measure wellbeing and the factors that might
+impact it. Survey topics included:
+* 🌱 **Feelings about life** - autonomy, life satisfaction, optimism
+* 🧍 **Thoughts and feelings about self** - psychological wellbeing,
+self-esteem, stress, feelings around appearance
+* 😟 **Feeling down** - negative affect, loneliness, supporting own wellbeing
+* 🧘‍♂️ **Health and routines** - sleep, physical activity
+* 🕰️ **Free time** - social media use, places to go and things to do
+* 🧑‍🤝‍🧑 **Relationships** - talking about feelings, acceptance, school
+connection, support from staff, support from parents/carers, experiences of
+discrimintation, support from friends, relative wealth and bulllying
+* 🏠 **Environment** - feelings about home and local area, including future work
+and education opportunities, and climate change
+* 👨‍👩‍👧‍👦 **Demographics and experiences** - gender, transgender, sexual
+orientation, neurodivergence, family background, care experience and young
+carers''',
+
+    # Design of standard survey
+    'standard_design': '''
+The survey delivered in Northern Devon was adapted from the first #BeeWell
+survey in Greater Manchester. That survey was developed through engagements
+with over 150 young people from 15 different schools to understand what
+wellbeing means to young people, what influences their wellbeing, and what
+makes them thrive.
+
+In Devon, we have adapted the survey to help it reflect the
+priorities of young people in this area. Topics were based on conversations
+across North Devon and Torridge with 195 young people and over 100 local actors
+including: system leaders, practitioners, and people at 45 organisations
+working with young people and broader communities. We have spoken with young
+people and school staff in Northern Devon, as well as researchers and public
+health professionals, amongst others, to choose, adapt and/or develop
+appropriate questions for the survey. We'd like to extend our thanks to
+everyone who supported this process.''',
+
+    # Design of the symbol survey
+    'symbol_design': '''
+The survey delivered in Northern Devon is the same as that first designed and
+delivered by the #BeeWell team in Greater Manchester. They worked with staff
+in special school settings to co-design a symbol version of the #BeeWell survey
+that would be accessible to young people with severe learning difficulties or
+profound and multiple learning disabilities. Using The Children's Society's
+'Good Childhood Index' for inspiration, they created a 10-item survey using the
+Widgit symbol system with simplified response options.''',
+
+    # Other #BeeWell sites
+    'other_beewell_sites': '''
+#BeeWell surveys have also been completed by pupils at schools in Hampshire,
+Greater Manchester, the London borough of Havering, and Milton Keynes.
+
+In 2023-24, **over 38,000 young people** completed a survey, with **nearly 300
+schools** having now taken part in #BeeWell.
+
+You can find out more about other sites at https://beewellprogramme.org/.''',
+
+    # Data used to create the dashboard (standard dashboard)
+    'standard_data': '''
+This dashboard presents the results from pupils at your school who completed
+the survey. To give context to these results, we've added comparisons against
+pupils from schools across Northern Devon.
+
+The survey responses were combined with data shared by the local authority such
+as free school meal eligibility and special education needs to give further
+insight into responses.''',
+
+    # Data used to create the dashboard (symbol dashboard)
+    'symbol_data': '''
+This dashboard presents the results from pupils at your school who completed
+the survey.
+
+The survey responses were combined with data shared by the local authority such
+as free school meal eligibility and special education needs to give further
+insight into responses.''',
+
+    # Data used to create the dashboard (public dashboard)
+    'public_data': '''
+This dashboard presents results from pupils at mainstream and non-mainstream
+schools who completed the survey.
+
+The survey responses were combined with data shared by the local authority such
+as free school meal eligibility and special education needs to give further
+insight into responses.''',
+
+    # How to use the results from this report
+    'how_to_use_results': '''
+These data can provide a useful starting point for discussions about the needs
+of your school population and priority areas for development and improvement.
+It can also be useful in considering areas of strengths and/or helping pupils
+reflect on their positive qualities.
+
+Data in your #BeeWell report may be useful in indicating progress against
+targets in your School Improvement Plan or help to identify future target
+areas. It may help to identify areas of priority for staff training or be used
+as context when considering academic data for participating year groups. It can
+also be used as independent evidence in the context of an Ofsted inspection.
+
+Finally, young people consulted during the set-up of #BeeWell in Greater
+Manchester felt strongly that pupils should be included in discussions around
+feedback, particularly to plan activities and approaches to raise awareness of
+strengths or difficulties the #BeeWell survey may highlight. They suggested
+involving a range of students (not just those involved in school councils) in
+planning how to raise awareness about wellbeing and to support the needs of
+young people.''',
+
+    # Viewing dashboard on different devices
+    'view_devices': '''
+Yes - this dashboard will resize so you should be able to access it on a range
+of devices (computer/laptop, tablet, phone, etc).''',
+
+    # Will there be support for interpreting and actioning on results?
+    'dashboard_support': '''
+Yes - Child Outcomes Research Consortium (CORC) has been funded to provide
+seminars and 1:1 support to schools in Northern Devon, to help you understand
+how to navigate the dashboard, interpret results, and suggest feedback in the
+development of action plans. You should receive information about this via
+email, but if you have not or have any questions, please contact us at
+kailobeewell@dartington.org.uk.''',
+
+    # Context of what already know about YP wellbeing
+    'wellbeing_context': '''
+* The peak age of onset of mental health difficulties is 14.5 years.<sup>[1]
+</sup>
+* Mental health and wellbeing in adolescence predicts adult health, labour
+market and other important outcomes.<sup>[2]</sup>
+* The wellbeing of adolescents has decreased in the last two decades, while the
+prevalence of mental health difficulties among them has increased.<sup>[3,4]
+</sup>
+* A recent international study ranked the UK’s young people fourth from bottom
+across nearly 80 countries in terms of life satisfaction.<sup>[5,6]</sup>
+* Young people’s mental health and wellbeing can be influenced by multiple
+drivers, including their health and routines, hobbies and entertainment,
+relationships, school, environment and society, and how they feel about their
+future.<sup>[7]</sup>
+
+<p style='font-size: 12px;'>
+References:<br>
+[1] Solmi, M. et al (2021). Age at onset of mental disorders worldwide:
+large-scale meta-analysis of 192 epidemiological studies. Molecular Psychiatry,
+Online First. Available at: https://www.nature.com/articles/s41380-021-01161-7
+<br>
+[2] Goodman A, Joshi H, Nasim B, Tyler C (2015). Social and emotional skills in
+childhood and their long-term effects on adult life. London: EIF. Available at:
+https://www.eif.org.uk/report/social-and-emotional-skills-in-childhood-and-thei
+r-long-term-effects-on-adult-life.<br>
+[3] Children’s Society (2021). The Good Childhood Report 2021. London:
+Children's Society. Available at: https://www.childrenssociety.org.uk/informati
+on/professionals/resources/good-childhood-report-2021<br>
+[4] NHS Digital (2021). Mental health of children and young people in England,
+2021 – wave 2 follow up to the 2017 survey. London: NHS Digital. Available at:
+https://digital.nhs.uk/data-and-information/publications/statistical/mental-hea
+lth-of-children-and-young-people-in-england/2021-follow-up-to-the-2017-survey
+<br>
+[5] Office for Economic Cooperation and Development (2019). Programme for
+International Student Assessment (PISA) results. Paris: OECD. Available at:
+https://www.oecd.org/publications/pisa-2018-results-volume-iii-acd78851-en.htm
+<br>
+[6] Marquez J, Long, E (2021). A Global Decline in Adolescents' Subjective
+Well-Being: a Comparative Study Exploring Patterns of Change in the Life
+Satisfaction of 15-Year-Old Students in 46 Countries. Child Ind Res 14,
+1251–1292 (2021). Available at: https://doi.org/10.1007/s12187-020-09788-8<br>
+[7] #BeeWell Programme Team (2021). #BeeWell survey. Manchester: University of
+Manchester. Available at: https://gmbeewell.org/wp-content/uploads/2021/09/BeeW
+ell-Questionnaires-Booklet.pdf</p>'''
+}
+
+
+def caution_comparing(type):
+    '''
+    Produce section of text providing caution for when making comparisons
+    between schools.
+
+    Parameters
+    ----------
+    type : string
+        Whether this is for 'school' or 'area' dashboard
+
+    Returns
+    -------
+    statement : string
+        Text on caution when comparing
+    '''
+    if type == 'school':
+        unit = 'schools'
+        participants = 'pupils'
+    elif type == 'area':
+        unit = 'areas'
+        participants = 'young people'
+    statement = f'''
+Always be mindful when making comparisons between different {unit}. There are
+a number of factors that could explain differences in scores (whether you are
+above average, average, or below average). These include:
+
+* Random chance ('one-off' findings).
+* Differences in the socio-economic characteristics of {participants} and the
+areas where they live (e.g. income, education, ethnicity, access to services
+and amenities).
+* The number of {participants} taking part - {unit} that are much smaller are
+more likely to have more "extreme" results (i.e. above or below average),
+whilst {unit} with a larger number of {participants} who took part are more
+likely to see average results.
+
+It's also worth noting that the score will only include results from
+{participants} who completed each of the questions used to calculate that
+topic, and so does not include any reflection of results from {participants}
+who did not complete some or all of the questions for that topic.
+'''
+    return statement
```

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/score_descriptions.py` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/score_descriptions.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-'''
-Dictionary with simple descriptions to support score interpretation
-For each score, we have a list where the first item is the score range
-and the second item is the interpretation of what higher scores indicate.
-'''
-
-score_descriptions = {
-    'autonomy': ['6 to 20', 'higher levels of autonomy'],
-    'life_satisfaction': ['0 to 10', 'higher levels of life satisfaction'],
-    'optimism': ['4 to 20', 'higher levels of optimism'],
-    'wellbeing': ['7 to 35', 'higher levels of psychological wellbeing'],
-    'esteem': ['5 to 20', 'higher levels of self-esteem'],
-    'stress': ['0 to 16', '''
-that pupils are feeling lower levels of stress, and better able to cope with
-stress'''],
-    'appearance': ['0 to 10', 'pupils feel happier about their appearance'],
-    'negative': ['0 to 20', 'less negative affect'],
-    'lonely': ['1 to 5', 'lower levels of loneliness'],
-    'support': ['2 to 8', '''
-pupils feel more able to support themselves when feeling down'''],
-    'sleep': ['0 to 1', 'pupils feel they get enough sleep'],
-    'physical': ['0 to 840', 'higher levels of physical activity'],
-    'free_like': ['1 to 5', '''
-pupils feel that they are more often able to do things that they like in their
-free time'''],
-    'media': ['0 to 8', 'less time spent on social media'],
-    'places': ['1 to 4', '''
-pupils feel there are activities/places in their local area that they would
-choose to or want to go to'''],
-    'talk': ['3 to 12', '''
-pupils feel more positively about talking with others when feeling down'''],
-    'accept': ['4 to 16', 'higher levels of perceived acceptance by others'],
-    'school_belong': ['1 to 5', 'higher levels of school connection'],
-    'staff_relationship': ['4 to 20', '''
-higher levels of perceived support from staff'''],
-    'home_relationship': [' 4 to 20', '''
-higher levels of perceived support at home'''],
-    'home_happy': ['0 to 10', '''
-higher levels of happiness with the home environment'''],
-    'local_env': ['5 to 25', '''
-pupils feel more positively about their local area'''],
-    'discrim': ['1 to 2', 'fewer experiences of discrimination'],
-    'belong_local': ['1 to 4', '''
-greater feelings of belonging in the local area'''],
-    'wealth': ['0 to 1', '''
-pupils feel their family has similar wealth as their friends (as opposed to
-feeling they are richer or poorer)'''],
-    'future': ['3 to 12', '''
-pupils feel more positively about future work, education and/or training
-opportunities in their local area'''],
-    'climate': ['1 to 4', '''
-lower levels of worrying about the impact of climate change on their
-future'''],
-    'social': ['4 to 20', 'higher levels of perceived social support'],
-    'bully': ['3 to 12', 'there to be less bullying']
-}
+'''
+Dictionary with simple descriptions to support score interpretation
+For each score, we have a list where the first item is the score range
+and the second item is the interpretation of what higher scores indicate.
+'''
+
+score_descriptions = {
+    'autonomy': ['6 to 20', 'higher levels of autonomy'],
+    'life_satisfaction': ['0 to 10', 'higher levels of life satisfaction'],
+    'optimism': ['4 to 20', 'higher levels of optimism'],
+    'wellbeing': ['7 to 35', 'higher levels of psychological wellbeing'],
+    'esteem': ['5 to 20', 'higher levels of self-esteem'],
+    'stress': ['0 to 16', '''
+that pupils are feeling lower levels of stress, and better able to cope with
+stress'''],
+    'appearance': ['0 to 10', 'pupils feel happier about their appearance'],
+    'negative': ['0 to 20', 'less negative affect'],
+    'lonely': ['1 to 5', 'lower levels of loneliness'],
+    'support': ['2 to 8', '''
+pupils feel more able to support themselves when feeling down'''],
+    'sleep': ['0 to 1', 'pupils feel they get enough sleep'],
+    'physical': ['0 to 840', 'higher levels of physical activity'],
+    'free_like': ['1 to 5', '''
+pupils feel that they are more often able to do things that they like in their
+free time'''],
+    'media': ['0 to 8', 'less time spent on social media'],
+    'places': ['1 to 4', '''
+pupils feel there are activities/places in their local area that they would
+choose to or want to go to'''],
+    'talk': ['3 to 12', '''
+pupils feel more positively about talking with others when feeling down'''],
+    'accept': ['4 to 16', 'higher levels of perceived acceptance by others'],
+    'school_belong': ['1 to 5', 'higher levels of school connection'],
+    'staff_relationship': ['4 to 20', '''
+higher levels of perceived support from staff'''],
+    'home_relationship': [' 4 to 20', '''
+higher levels of perceived support at home'''],
+    'home_happy': ['0 to 10', '''
+higher levels of happiness with the home environment'''],
+    'local_env': ['5 to 25', '''
+pupils feel more positively about their local area'''],
+    'discrim': ['1 to 2', 'fewer experiences of discrimination'],
+    'belong_local': ['1 to 4', '''
+greater feelings of belonging in the local area'''],
+    'wealth': ['0 to 1', '''
+pupils feel their family has similar wealth as their friends (as opposed to
+feeling they are richer or poorer)'''],
+    'future': ['3 to 12', '''
+pupils feel more positively about future work, education and/or training
+opportunities in their local area'''],
+    'climate': ['1 to 4', '''
+lower levels of worrying about the impact of climate change on their
+future'''],
+    'social': ['4 to 20', 'higher levels of perceived social support'],
+    'bully': ['3 to 12', 'there to be less bullying']
+}
```

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/static_report.py` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/static_report.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,426 +1,426 @@
-'''
-Function to generate a non-interactive PDF version of the dashboard as a
-temporary file that can then be downloaded from the dashboard
-'''
-import base64
-from .images import get_image_path
-from importlib.resources import files
-from markdown import markdown
-import os
-from .reshape_data import get_school_size
-from .reuse_text import reuse_text, caution_comparing
-from .summary_rag import summary_intro, summary_table
-from .explore_results import (
-    create_bar_charts,
-    create_explore_topic_page,
-    create_topic_dict,
-    get_chosen_result,
-    write_page_title)
-from .who_took_part import (
-    create_demographic_page_intro,
-    demographic_headers,
-    demographic_plots)
-
-
-def logo_html():
-    '''
-    Generates HTML string to create logo as displayed on cover page of reports.
-
-    Returns
-    -------
-    img_tag : string
-        HTML to generate the logo
-    '''
-    # Encode image
-    img_path = get_image_path('kailo_beewell_logo_padded.png')
-    data_uri = base64.b64encode(open(img_path, 'rb').read()).decode('utf-8')
-    # Insert into HTML image tag
-    img_tag = f'''
-<img src='data:image/png;base64,{data_uri}' alt='Kailo #BeeWell logo'
-style='width:300px; height:182px;'>'''
-    return img_tag
-
-
-def illustration_html():
-    '''
-    Generates DIV element containing illustration as displayed on cover page of
-    reports.
-
-    Returns
-    -------
-    illustration : string
-        HTML to generate div containing the illustration
-    '''
-    # Encode image
-    img_path = get_image_path('home_image_3_transparent.png')
-    data_uri = base64.b64encode(open(img_path, 'rb').read()).decode('utf-8')
-    # Insert into HTML image tag
-    img_tag = f'''
-<img src='data:image/png;base64,{data_uri}' alt='Kailo illustration'
-style='width:650px; height:192px;'>'''
-    # Insert into div
-    illustration = f'''
-<div style='width:100%; position:absolute; bottom:0;'>
-    {img_tag}
-</div>'''
-    return illustration
-
-
-def structure_report(pdf_title, content):
-    '''
-    Inserts the provided HTML into the structure of the report - PDF title,
-    importing and reading the CSS style, and inserting the content of report
-
-    Parameters
-    ----------
-    pdf_title : string
-        Title for the pdf file
-    content : string
-        HTML content of the report
-
-    Returns
-    -------
-    html_content : string
-        HTML to produce the styled report
-    '''
-    # Remove the final temporary image file
-    if os.path.exists('report/temp_image.png'):
-        os.remove('report/temp_image.png')
-
-    # Import the CSS stylesheet
-    css_path = str(files('kailo_beewell_dashboard')
-                   .joinpath('css/static_report_style.css'))
-    with open(css_path) as css:
-        css_style = css.read()
-
-    html_content = f'''
-<!DOCTYPE html>
-<html>
-<head>
-    <title>{pdf_title}</title>
-    <style>
-        {css_style}
-    </style>
-</head>
-<body>
-    {''.join(content)}
-</body>
-</html>
-'''
-    return html_content
-
-
-def create_static_report(chosen_school, chosen_group, df_scores, df_prop,
-                         counts, dem_prop, pdf_title):
-    '''
-    Generate a static PDF report for the chosen school and group, with all
-    the key information and figures from the dashboard
-
-    Parameters
-    ----------
-    chosen_school : string
-        Name of the chosen school
-    chosen_group : string
-        Name of the chosen group to view results by - options are
-        'For all pupils', 'By year group', 'By gender', 'By FSM' or 'By SEN'
-    df_scores : dataframe
-        Dataframe with aggregate scores and RAG for each topic
-    df_prop : dataframe
-        Dataframe with proportion of each response to each survey question
-    counts : dataframe
-        Dataframe with the counts of pupils at each school
-    dem_prop : dataframe
-        Dataframe with proportion of each reponse to the demographic questions
-    pdf_title : string
-        Title for the PDF file
-    '''
-    ##########
-    # Set-up #
-    ##########
-
-    # Create empty list to fill with HTML content for PDF report
-    content = []
-
-    # Get dictionaries which will use later on and for table of contents
-    # Create dictionary of topics
-    topic_dict = create_topic_dict(df_scores)
-    # Create header dictionary for the demographic section
-    dem_header_dict = demographic_headers()
-
-    # Get school size
-    school_size = get_school_size(counts, chosen_school)
-
-    ##############
-    # Title page #
-    ##############
-
-    # Add logo
-    content.append(logo_html())
-
-    # Get group name with only first character modified to lower case
-    group_lower_first = chosen_group[0].lower() + chosen_group[1:]
-
-    # Title and introduction
-    title_page = f'''
-<div class='section_container'>
-    <h1 style='text-align:center;'>The #BeeWell Survey</h1>
-    <p style='text-align:center; font-weight:bold;'>Thank you for taking
-    part in the #BeeWell survey delivered by Kailo.</p>
-    <p>The results from pupils at your school can be explored using the
-    interactive dashboard at
-    https://synthetic-beewell-kailo-standard-school-dashboard.streamlit.app/.
-    This report has been downloaded from that dashboard.<br><br>
-    There are four reports available - these have results: (a) from all
-    pupils, (b) by gender, (c) by free school meal (FSM) eligibility, and
-    (d) by year group.<br><br>
-    This report contains the results <b>{group_lower_first}</b> for
-    <b>{chosen_school}</b>.</p>
-</div>'''
-    content.append(title_page)
-
-    # Add illustration
-    content.append(illustration_html())
-
-    ################
-    # Introduction #
-    ################
-
-    # Heading
-    content.append('''<h1 style='page-break-before:always;'>
-                   Introduction</h1>''')
-
-    # Using the report (duplicate text with About.py)
-    content.append('<h2>How to use this report</h2>')
-    content.append(markdown(reuse_text['how_to_use_results']))
-
-    # Comparison warning (duplicate text with Explore results.py)
-    content.append('<h2>Comparing between schools</h2>')
-    content.append(markdown(caution_comparing(type='school')))
-
-    #####################
-    # Table of contents #
-    #####################
-
-    # Get all of the explore results pages as lines for the table of contents
-    explore_results_pages = []
-    for key, value in topic_dict.items():
-        line = f'''<li><a href='#{value}'>{key}</a></li>'''
-        explore_results_pages.append(line)
-
-    # Get the demographic headers as lines for the table of contents
-    demographic_pages = []
-    for key, value in dem_header_dict.items():
-        line = f'''<li><a href='#{key}'>{value}</a></li>'''
-        demographic_pages.append(line)
-
-    content.append(f'''
-<div>
-    <h1 style='page-break-before:always;'>Table of Contents</h1>
-    <ul>
-        <li><a href='#summary'>Summary</a> - See a simple overview of
-            results from pupils at your school, compared with other
-            schools</li>
-        <br>
-        <li><a href='#explore_results'>Explore results</a> - Explore how
-            your pupils responded to each survey question, and see further
-            information on how the summary page's comparison to other
-            schools was generated
-            <ul>{''.join(explore_results_pages)}</ul>
-        </li>
-        <br>
-        <li><a href='#who_took_part'>Who took part</a> - See the
-            characteristics of the pupils who took part in the survey
-            <ul>{''.join(demographic_pages)}</ul>
-        </li>
-    </ul>
-</div>
-''')
-
-    ################
-    # Summary page #
-    ################
-
-    # Summary cover page with guide to RAG ratings
-    content.append(summary_intro(school_size, 'pdf'))
-
-    # Summary grid with RAG ratings for each topic
-    content = summary_table(
-        df_scores, chosen_group, chosen_school, 'pdf', content)
-
-    ###########################
-    # Explore results section #
-    ###########################
-
-    # Create cover page with title and introduction
-    content.append(write_page_title(output='pdf'))
-
-    # Create pages for all of the topics
-    for chosen_variable_lab in topic_dict.keys():
-        content = create_explore_topic_page(
-            chosen_variable_lab, topic_dict, df_scores, chosen_school,
-            chosen_group, df_prop, content)
-
-    #########################
-    # Who took part section #
-    #########################
-
-    # Create cover page with title and introduction
-    content.append(create_demographic_page_intro(school_size, 'pdf'))
-
-    # Create pages with plots for each measure
-    content = demographic_plots(
-        dem_prop=dem_prop, chosen_school=chosen_school,
-        chosen_group='Compared with other schools in Northern Devon',
-        output='pdf', content=content)
-
-    ######################
-    # Create HTML report #
-    ######################
-
-    html_content = structure_report(pdf_title, content)
-
-    return html_content
-
-
-def create_static_symbol_report(
-        chosen_school,  df_prop, counts, dem_prop, pdf_title):
-    '''
-    Generate a static symbol survey PDF report for the chosen school and group,
-    with all the key information and figures from the dashboard
-
-    Parameters
-    ----------
-    chosen_school : string
-        Name of the chosen school
-    df_prop : dataframe
-        Dataframe with proportion of each response to each survey question
-    counts : dataframe
-        Dataframe with the counts of pupils at each school
-    dem_prop : dataframe
-        Dataframe with proportion of each reponse to the demographic questions
-    pdf_title : string
-        Title for the PDF file
-    '''
-    ##########
-    # Set-up #
-    ##########
-    # Create empty list to fill with HTML content for PDF report
-    content = []
-
-    # Create dictionary with groups and labels to use in table of contents
-    survey_groups = {'all': 'For all pupils',
-                     'year': 'By year group',
-                     'gender': 'By gender',
-                     'fsm': 'By FSM'}
-
-    # Get school size
-    school_size = get_school_size(counts, chosen_school, 'symbol')
-
-    ##############
-    # Title page #
-    ##############
-
-    # Add logo
-    content.append(logo_html())
-
-    # Title and introduction
-    title_page = f'''
-<div class='section_container'>
-    <h1 style='text-align:center;'>The #BeeWell Survey</h1>
-    <p style='text-align:center; font-weight:bold;'>Thank you for taking
-    part in the #BeeWell survey delivered by Kailo.</p>
-    <p>The results from pupils at your school can be explored using the
-    interactive dashboard at
-    https://synthetic-beewell-kailo-standard-school-dashboard.streamlit.app/.
-    This report has been downloaded from that dashboard.<br><br>
-    This report contains the results for <b>{chosen_school}</b>.</p>
-</div>'''
-    content.append(title_page)
-
-    # Add illustration
-    content.append(illustration_html())
-
-    ################
-    # Introduction #
-    ################
-
-    # Heading
-    content.append('''<h1 style='page-break-before:always;'>
-                   Introduction</h1>''')
-
-    # Using the report (duplicate text with About.py)
-    content.append('<h2>How to use this report</h2>')
-    content.append(markdown(caution_comparing(type='school')))
-
-    #####################
-    # Table of contents #
-    #####################
-
-    # Get all of the explore results pages as lines for the table of contents
-    explore_results_pages = []
-    for key, value in survey_groups.items():
-        line = f'''<li><a href='#{key}'>{value}</a></li>'''
-        explore_results_pages.append(line)
-
-    # Get the demographic headers as lines for the table of contents
-
-    content.append(f'''
-<div>
-    <h1>Table of Contents</h1>
-    <ul>
-        <li><a href='#explore_results'>Explore results</a> - Explore how
-            your pupils responded to each survey question
-            <ul>{''.join(explore_results_pages)}</ul>
-        </li>
-        <br>
-        <li><a href='#who_took_part'>Who took part</a> - See the
-            characteristics of the pupils who took part in the survey
-        </li>
-    </ul>
-</div>
-''')
-
-    ###########################
-    # Explore results section #
-    ###########################
-
-    # Create cover page with title and introduction
-    content.append(write_page_title(output='pdf', survey_type='symbol'))
-
-    # Create pages with plots for each measure
-    chosen_variable = 'symbol'
-    df_prop['group'] = chosen_variable
-    for key, value in survey_groups.items():
-        # Add title for that group
-        content.append(f'''
-<h2 id='{key}'; style='page-break-before:always;'>Explore
-results {value[0].lower() + value[1:]}</h2>''')
-        # Get results for that school and group
-        chosen_result = get_chosen_result(
-            chosen_variable, chosen_group=value, df=df_prop,
-            school=chosen_school, survey_type='symbol')
-        # Add bar charts to the HTML
-        content = create_bar_charts(
-            chosen_variable, chosen_result, output='pdf', content=content)
-
-    #########################
-    # Who took part section #
-    #########################
-
-    # Create cover page with title and introduction
-    content.append(create_demographic_page_intro(school_size, 'pdf'))
-
-    # Create pages with plots for each measure
-    dem_prop['plot_group'] = dem_prop['measure']
-    content = demographic_plots(
-        dem_prop=dem_prop, chosen_school=chosen_school,
-        chosen_group='For your school', output='pdf', content=content,
-        survey_type='symbol')
-
-    ######################
-    # Create HTML report #
-    ######################
-
-    html_content = structure_report(pdf_title, content)
-
-    return html_content
+'''
+Function to generate a non-interactive PDF version of the dashboard as a
+temporary file that can then be downloaded from the dashboard
+'''
+import base64
+from .images import get_image_path
+from importlib.resources import files
+from markdown import markdown
+import os
+from .reshape_data import get_school_size
+from .reuse_text import reuse_text, caution_comparing
+from .summary_rag import summary_intro, summary_table
+from .explore_results import (
+    create_bar_charts,
+    create_explore_topic_page,
+    create_topic_dict,
+    get_chosen_result,
+    write_page_title)
+from .who_took_part import (
+    create_demographic_page_intro,
+    demographic_headers,
+    demographic_plots)
+
+
+def logo_html():
+    '''
+    Generates HTML string to create logo as displayed on cover page of reports.
+
+    Returns
+    -------
+    img_tag : string
+        HTML to generate the logo
+    '''
+    # Encode image
+    img_path = get_image_path('kailo_beewell_logo_padded.png')
+    data_uri = base64.b64encode(open(img_path, 'rb').read()).decode('utf-8')
+    # Insert into HTML image tag
+    img_tag = f'''
+<img src='data:image/png;base64,{data_uri}' alt='Kailo #BeeWell logo'
+style='width:300px; height:182px;'>'''
+    return img_tag
+
+
+def illustration_html():
+    '''
+    Generates DIV element containing illustration as displayed on cover page of
+    reports.
+
+    Returns
+    -------
+    illustration : string
+        HTML to generate div containing the illustration
+    '''
+    # Encode image
+    img_path = get_image_path('home_image_3_transparent.png')
+    data_uri = base64.b64encode(open(img_path, 'rb').read()).decode('utf-8')
+    # Insert into HTML image tag
+    img_tag = f'''
+<img src='data:image/png;base64,{data_uri}' alt='Kailo illustration'
+style='width:650px; height:192px;'>'''
+    # Insert into div
+    illustration = f'''
+<div style='width:100%; position:absolute; bottom:0;'>
+    {img_tag}
+</div>'''
+    return illustration
+
+
+def structure_report(pdf_title, content):
+    '''
+    Inserts the provided HTML into the structure of the report - PDF title,
+    importing and reading the CSS style, and inserting the content of report
+
+    Parameters
+    ----------
+    pdf_title : string
+        Title for the pdf file
+    content : string
+        HTML content of the report
+
+    Returns
+    -------
+    html_content : string
+        HTML to produce the styled report
+    '''
+    # Remove the final temporary image file
+    if os.path.exists('report/temp_image.png'):
+        os.remove('report/temp_image.png')
+
+    # Import the CSS stylesheet
+    css_path = str(files('kailo_beewell_dashboard')
+                   .joinpath('css/static_report_style.css'))
+    with open(css_path) as css:
+        css_style = css.read()
+
+    html_content = f'''
+<!DOCTYPE html>
+<html>
+<head>
+    <title>{pdf_title}</title>
+    <style>
+        {css_style}
+    </style>
+</head>
+<body>
+    {''.join(content)}
+</body>
+</html>
+'''
+    return html_content
+
+
+def create_static_report(chosen_school, chosen_group, df_scores, df_prop,
+                         counts, dem_prop, pdf_title):
+    '''
+    Generate a static PDF report for the chosen school and group, with all
+    the key information and figures from the dashboard
+
+    Parameters
+    ----------
+    chosen_school : string
+        Name of the chosen school
+    chosen_group : string
+        Name of the chosen group to view results by - options are
+        'For all pupils', 'By year group', 'By gender', 'By FSM' or 'By SEN'
+    df_scores : dataframe
+        Dataframe with aggregate scores and RAG for each topic
+    df_prop : dataframe
+        Dataframe with proportion of each response to each survey question
+    counts : dataframe
+        Dataframe with the counts of pupils at each school
+    dem_prop : dataframe
+        Dataframe with proportion of each reponse to the demographic questions
+    pdf_title : string
+        Title for the PDF file
+    '''
+    ##########
+    # Set-up #
+    ##########
+
+    # Create empty list to fill with HTML content for PDF report
+    content = []
+
+    # Get dictionaries which will use later on and for table of contents
+    # Create dictionary of topics
+    topic_dict = create_topic_dict(df_scores)
+    # Create header dictionary for the demographic section
+    dem_header_dict = demographic_headers()
+
+    # Get school size
+    school_size = get_school_size(counts, chosen_school)
+
+    ##############
+    # Title page #
+    ##############
+
+    # Add logo
+    content.append(logo_html())
+
+    # Get group name with only first character modified to lower case
+    group_lower_first = chosen_group[0].lower() + chosen_group[1:]
+
+    # Title and introduction
+    title_page = f'''
+<div class='section_container'>
+    <h1 style='text-align:center;'>The #BeeWell Survey</h1>
+    <p style='text-align:center; font-weight:bold;'>Thank you for taking
+    part in the #BeeWell survey delivered by Kailo.</p>
+    <p>The results from pupils at your school can be explored using the
+    interactive dashboard at
+    https://synthetic-beewell-kailo-standard-school-dashboard.streamlit.app/.
+    This report has been downloaded from that dashboard.<br><br>
+    There are four reports available - these have results: (a) from all
+    pupils, (b) by gender, (c) by free school meal (FSM) eligibility, and
+    (d) by year group.<br><br>
+    This report contains the results <b>{group_lower_first}</b> for
+    <b>{chosen_school}</b>.</p>
+</div>'''
+    content.append(title_page)
+
+    # Add illustration
+    content.append(illustration_html())
+
+    ################
+    # Introduction #
+    ################
+
+    # Heading
+    content.append('''<h1 style='page-break-before:always;'>
+                   Introduction</h1>''')
+
+    # Using the report (duplicate text with About.py)
+    content.append('<h2>How to use this report</h2>')
+    content.append(markdown(reuse_text['how_to_use_results']))
+
+    # Comparison warning (duplicate text with Explore results.py)
+    content.append('<h2>Comparing between schools</h2>')
+    content.append(markdown(caution_comparing(type='school')))
+
+    #####################
+    # Table of contents #
+    #####################
+
+    # Get all of the explore results pages as lines for the table of contents
+    explore_results_pages = []
+    for key, value in topic_dict.items():
+        line = f'''<li><a href='#{value}'>{key}</a></li>'''
+        explore_results_pages.append(line)
+
+    # Get the demographic headers as lines for the table of contents
+    demographic_pages = []
+    for key, value in dem_header_dict.items():
+        line = f'''<li><a href='#{key}'>{value}</a></li>'''
+        demographic_pages.append(line)
+
+    content.append(f'''
+<div>
+    <h1 style='page-break-before:always;'>Table of Contents</h1>
+    <ul>
+        <li><a href='#summary'>Summary</a> - See a simple overview of
+            results from pupils at your school, compared with other
+            schools</li>
+        <br>
+        <li><a href='#explore_results'>Explore results</a> - Explore how
+            your pupils responded to each survey question, and see further
+            information on how the summary page's comparison to other
+            schools was generated
+            <ul>{''.join(explore_results_pages)}</ul>
+        </li>
+        <br>
+        <li><a href='#who_took_part'>Who took part</a> - See the
+            characteristics of the pupils who took part in the survey
+            <ul>{''.join(demographic_pages)}</ul>
+        </li>
+    </ul>
+</div>
+''')
+
+    ################
+    # Summary page #
+    ################
+
+    # Summary cover page with guide to RAG ratings
+    content.append(summary_intro(school_size, 'pdf'))
+
+    # Summary grid with RAG ratings for each topic
+    content = summary_table(
+        df_scores, chosen_group, chosen_school, 'pdf', content)
+
+    ###########################
+    # Explore results section #
+    ###########################
+
+    # Create cover page with title and introduction
+    content.append(write_page_title(output='pdf'))
+
+    # Create pages for all of the topics
+    for chosen_variable_lab in topic_dict.keys():
+        content = create_explore_topic_page(
+            chosen_variable_lab, topic_dict, df_scores, chosen_school,
+            chosen_group, df_prop, content)
+
+    #########################
+    # Who took part section #
+    #########################
+
+    # Create cover page with title and introduction
+    content.append(create_demographic_page_intro(school_size, 'pdf'))
+
+    # Create pages with plots for each measure
+    content = demographic_plots(
+        dem_prop=dem_prop, chosen_school=chosen_school,
+        chosen_group='Compared with other schools in Northern Devon',
+        output='pdf', content=content)
+
+    ######################
+    # Create HTML report #
+    ######################
+
+    html_content = structure_report(pdf_title, content)
+
+    return html_content
+
+
+def create_static_symbol_report(
+        chosen_school,  df_prop, counts, dem_prop, pdf_title):
+    '''
+    Generate a static symbol survey PDF report for the chosen school and group,
+    with all the key information and figures from the dashboard
+
+    Parameters
+    ----------
+    chosen_school : string
+        Name of the chosen school
+    df_prop : dataframe
+        Dataframe with proportion of each response to each survey question
+    counts : dataframe
+        Dataframe with the counts of pupils at each school
+    dem_prop : dataframe
+        Dataframe with proportion of each reponse to the demographic questions
+    pdf_title : string
+        Title for the PDF file
+    '''
+    ##########
+    # Set-up #
+    ##########
+    # Create empty list to fill with HTML content for PDF report
+    content = []
+
+    # Create dictionary with groups and labels to use in table of contents
+    survey_groups = {'all': 'For all pupils',
+                     'year': 'By year group',
+                     'gender': 'By gender',
+                     'fsm': 'By FSM'}
+
+    # Get school size
+    school_size = get_school_size(counts, chosen_school, 'symbol')
+
+    ##############
+    # Title page #
+    ##############
+
+    # Add logo
+    content.append(logo_html())
+
+    # Title and introduction
+    title_page = f'''
+<div class='section_container'>
+    <h1 style='text-align:center;'>The #BeeWell Survey</h1>
+    <p style='text-align:center; font-weight:bold;'>Thank you for taking
+    part in the #BeeWell survey delivered by Kailo.</p>
+    <p>The results from pupils at your school can be explored using the
+    interactive dashboard at
+    https://synthetic-beewell-kailo-standard-school-dashboard.streamlit.app/.
+    This report has been downloaded from that dashboard.<br><br>
+    This report contains the results for <b>{chosen_school}</b>.</p>
+</div>'''
+    content.append(title_page)
+
+    # Add illustration
+    content.append(illustration_html())
+
+    ################
+    # Introduction #
+    ################
+
+    # Heading
+    content.append('''<h1 style='page-break-before:always;'>
+                   Introduction</h1>''')
+
+    # Using the report (duplicate text with About.py)
+    content.append('<h2>How to use this report</h2>')
+    content.append(markdown(caution_comparing(type='school')))
+
+    #####################
+    # Table of contents #
+    #####################
+
+    # Get all of the explore results pages as lines for the table of contents
+    explore_results_pages = []
+    for key, value in survey_groups.items():
+        line = f'''<li><a href='#{key}'>{value}</a></li>'''
+        explore_results_pages.append(line)
+
+    # Get the demographic headers as lines for the table of contents
+
+    content.append(f'''
+<div>
+    <h1>Table of Contents</h1>
+    <ul>
+        <li><a href='#explore_results'>Explore results</a> - Explore how
+            your pupils responded to each survey question
+            <ul>{''.join(explore_results_pages)}</ul>
+        </li>
+        <br>
+        <li><a href='#who_took_part'>Who took part</a> - See the
+            characteristics of the pupils who took part in the survey
+        </li>
+    </ul>
+</div>
+''')
+
+    ###########################
+    # Explore results section #
+    ###########################
+
+    # Create cover page with title and introduction
+    content.append(write_page_title(output='pdf', survey_type='symbol'))
+
+    # Create pages with plots for each measure
+    chosen_variable = 'symbol'
+    df_prop['group'] = chosen_variable
+    for key, value in survey_groups.items():
+        # Add title for that group
+        content.append(f'''
+<h2 id='{key}'; style='page-break-before:always;'>Explore
+results {value[0].lower() + value[1:]}</h2>''')
+        # Get results for that school and group
+        chosen_result = get_chosen_result(
+            chosen_variable, chosen_group=value, df=df_prop,
+            school=chosen_school, survey_type='symbol')
+        # Add bar charts to the HTML
+        content = create_bar_charts(
+            chosen_variable, chosen_result, output='pdf', content=content)
+
+    #########################
+    # Who took part section #
+    #########################
+
+    # Create cover page with title and introduction
+    content.append(create_demographic_page_intro(school_size, 'pdf'))
+
+    # Create pages with plots for each measure
+    dem_prop['plot_group'] = dem_prop['measure']
+    content = demographic_plots(
+        dem_prop=dem_prop, chosen_school=chosen_school,
+        chosen_group='For your school', output='pdf', content=content,
+        survey_type='symbol')
+
+    ######################
+    # Create HTML report #
+    ######################
+
+    html_content = structure_report(pdf_title, content)
+
+    return html_content
```

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/stylable_container.py` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/stylable_container.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-'''
-Generic function to produce stylised containers and then specific function
-for producing the stylised header containers used on the About page
-'''
-import streamlit as st
-from .page_setup import blank_lines
-
-
-def stylable_container(key, css_styles):
-    '''
-    This function is copied from streamlit-extras. It creates inserts a
-    container in the app that we are able to style using CSS.
-
-    Parameters
-    ----------
-    key : str
-        The unique key associated with container
-    css_styles : str | list[str]
-        The CSS styles to apply to the container elements. This can be a single
-        CSS block or a list of CSS blocks.
-
-    Returns:
-    container
-        A container object. Elements can be added to this container using
-        either the 'with' notation or by calling methods directly on the
-        returned object.
-    '''
-    # If CSS style provided is a string, insert it into a list
-    if isinstance(css_styles, str):
-        css_styles = [css_styles]
-
-    # Remove unneeded spacing that is added by the style markdown:
-    css_styles.append('''
-> div:first-child {
-    margin-bottom: -1rem;
-}
-''')
-
-    # Use provided CSS to write the full CSS to style the container
-    style_text = '<style>'
-    for style in css_styles:
-        style_text += f'''
-div[data-testid="stVerticalBlock"]:has(> div.element-container > div.stMarkdown
-> div[data-testid="stMarkdownContainer"] > p > span.{key}) {style}'''
-    style_text += f'''
-</style>
-<span class="{key}"></span>'''
-
-    # Produce the container and apply style
-    container = st.container()
-    container.markdown(style_text, unsafe_allow_html=True)
-    return container
-
-
-def header_container(key, text, colour):
-    '''
-    Create a stylised container for the About page to container a header
-
-    Args:
-        key (str): Key for container type
-        text (str): Header text
-        colour (str): HEX colour code for background of container
-    '''
-    blank_lines(2)
-    with stylable_container(
-            key=key,
-            css_styles=f'''
-{{
-    background-color: {colour};
-    border-radius: 0.5rem;
-    padding: 0px
-}}''',):
-        # Add header in markdown so can add some blank space to start of line
-        st.markdown(f'<h2>&nbsp&nbsp{text}</hr>', unsafe_allow_html=True)
-        blank_lines(1)
+'''
+Generic function to produce stylised containers and then specific function
+for producing the stylised header containers used on the About page
+'''
+import streamlit as st
+from .page_setup import blank_lines
+
+
+def stylable_container(key, css_styles):
+    '''
+    This function is copied from streamlit-extras. It creates inserts a
+    container in the app that we are able to style using CSS.
+
+    Parameters
+    ----------
+    key : str
+        The unique key associated with container
+    css_styles : str | list[str]
+        The CSS styles to apply to the container elements. This can be a single
+        CSS block or a list of CSS blocks.
+
+    Returns:
+    container
+        A container object. Elements can be added to this container using
+        either the 'with' notation or by calling methods directly on the
+        returned object.
+    '''
+    # If CSS style provided is a string, insert it into a list
+    if isinstance(css_styles, str):
+        css_styles = [css_styles]
+
+    # Remove unneeded spacing that is added by the style markdown:
+    css_styles.append('''
+> div:first-child {
+    margin-bottom: -1rem;
+}
+''')
+
+    # Use provided CSS to write the full CSS to style the container
+    style_text = '<style>'
+    for style in css_styles:
+        style_text += f'''
+div[data-testid="stVerticalBlock"]:has(> div.element-container > div.stMarkdown
+> div[data-testid="stMarkdownContainer"] > p > span.{key}) {style}'''
+    style_text += f'''
+</style>
+<span class="{key}"></span>'''
+
+    # Produce the container and apply style
+    container = st.container()
+    container.markdown(style_text, unsafe_allow_html=True)
+    return container
+
+
+def header_container(key, text, colour):
+    '''
+    Create a stylised container for the About page to container a header
+
+    Args:
+        key (str): Key for container type
+        text (str): Header text
+        colour (str): HEX colour code for background of container
+    '''
+    blank_lines(2)
+    with stylable_container(
+            key=key,
+            css_styles=f'''
+{{
+    background-color: {colour};
+    border-radius: 0.5rem;
+    padding: 0px
+}}''',):
+        # Add header in markdown so can add some blank space to start of line
+        st.markdown(f'<h2>&nbsp&nbsp{text}</hr>', unsafe_allow_html=True)
+        blank_lines(1)
```

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/summary_rag.py` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/summary_rag.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,369 +1,369 @@
-'''
-Helper functions for the summary page, and for the production of the 'RAG'
-boxes which are also use on the 'Explore Results' page
-'''
-import pandas as pd
-import streamlit as st
-import numpy as np
-from markdown import markdown
-from .page_setup import blank_lines
-from .reshape_data import filter_by_group
-from .stylable_container import stylable_container
-from .switch_page_button import switch_page
-
-
-def create_rag_container(text, background, font, output='streamlit', key=None):
-    '''
-    Generates a streamlit or HTML container with the specified background and
-    font colours, including the text provided, and with class of 'result_box'
-    if its the HTML container
-
-    Parameters
-    ----------
-    text : string
-        Text to go in the container.
-    background : string
-        Background colour.
-    font : string
-        Font colour.
-    output : string
-        Specifies whether to write for 'streamlit' (default) or 'pdf'.
-    key : string
-        Optional input. Key for the container.
-
-    Returns
-    -------
-    html_string : string
-        HTML string, to be appended to the content for the report
-    '''
-    if output == 'streamlit':
-        with stylable_container(
-            key=key,
-            css_styles=f'''{{
-                background-color: {background};
-                border-radius: 0.5rem;
-                padding: 0px}}''',):
-            blank_lines(1)
-            st.markdown(f'''<p style='text-align: center; color: {font};'>
-                        {text}</p>''', unsafe_allow_html=True)
-            blank_lines(1)
-
-    elif output == 'pdf':
-        html_string = f'''
-    <div class='result_box' style='background: {background}; color: {font}'>
-        <p>{text}</p>
-    </div>'''
-        return html_string
-
-
-def result_box(rag, output='streamlit'):
-    '''
-    Creates a result box with the RAG rating
-
-    Parameters
-    ----------
-    rag : string
-        Result from comparison with other schools - either 'below', 'average',
-        'above', or np.nan
-    output : string
-        Specifies whether to write for 'streamlit' (default) or 'pdf'.
-
-    Returns
-    -------
-    html_string : string
-        HTML string, to be appended to the content for the report
-    '''
-    # Find text and colours depending on RAG rating
-    if rag == 'below':
-        rag_text = 'Below average'
-        background = '#FFCCCC'
-        font = '#95444B'
-    elif rag == 'average':
-        rag_text = 'Average'
-        background = '#FFE8BF'
-        font = '#AA7A18'
-    elif rag == 'above':
-        rag_text = 'Above average'
-        background = '#B6E6B6'
-        font = '#2B7C47'
-    elif pd.isnull(rag):
-        rag_text = 'n < 10'
-        background = '#DCE4FF'
-        font = '#19539A'
-
-    # Create for streamlit or PDF
-    if output == 'streamlit':
-        create_rag_container(rag_text, background, font, output, key=rag)
-    elif output == 'pdf':
-        return create_rag_container(rag_text, background, font, output)
-
-
-def rag_intro_column(rag, rag_descrip, output='streamlit'):
-    '''
-    Generate a row for the introduction to the summary section, with a RAG
-    box and description of that box across 2 columns.
-
-    Parameters
-    ----------
-    rag : string
-        RAG performance - either 'above', 'average', 'below', or np.nan
-    rag_descrip : string
-        Description of the RAG rating
-    output : string
-        Specifies whether to write for 'streamlit' (default) or 'pdf'.
-
-    Returns
-    -------
-    html_string : string
-        Section of HTML that creates the RAG introductory columns
-    '''
-    # Streamlit version
-    if output == 'streamlit':
-        cols = st.columns(2)
-        with cols[0]:
-            result_box(rag)
-        with cols[1]:
-            st.markdown(rag_descrip)
-
-    # PDF version
-    elif output == 'pdf':
-        rag_box = result_box(rag, output='pdf')
-        html_string = f'''
-<div class='row'>
-    <div class='column2' style='margin-top:0.5em;'>
-        {rag_box}
-    </div>
-    <div class='column2'>
-        {rag_descrip}
-    </div>
-</div>
-'''
-        return html_string
-
-
-def summary_intro(school_size, output='streamlit'):
-    '''
-    Creates the introduction for the summary section
-
-    Parameters
-    ----------
-    school_size : integer
-        Total number of pupils at school (who answered at least one question)
-    output : string
-        Specifies whether to write for 'streamlit' (default) or 'pdf'
-
-    Returns
-    -------
-    html_string : string
-        Optional return, if output=='pdf', contains HTML for summary cover page
-    '''
-    # For PDF report, create temporary list to store HTML for page
-    if output == 'pdf':
-        temp_content = []
-
-    # Write title for this section
-    title = '''Summary of your school's results'''
-    if output == 'streamlit':
-        st.title(title)
-        st.subheader('Introduction')
-    elif output == 'pdf':
-        temp_content.append(f'''<h1 style='page-break-before:always;'
-                            id='summary'>{title}</h1>''')
-
-    # Write introductory sentence for summary section
-    descrip = f'''
-At your school, a total of {school_size} pupils took part in the #BeeWell
-survey. This page shows how the answers of pupils at your school compare with
-pupils from other schools in Northern Devon.'''
-    if output == 'streamlit':
-        st.markdown(descrip)
-    elif output == 'pdf':
-        temp_content.append(f'<p>{descrip}</p>')
-
-    # Write interpretation of each of the rag boxes
-    rag_descrip_below = '''
-This means that average scores for students in your school are **worse** than
-average scores for pupils at other schools.'''
-    rag_descrip_average = '''
-This means that average scores for students in your school are **similar** to
-average scores for pupils at other schools.'''
-    rag_descrip_above = '''
-This means that average scores for students in your school are **better** than
-average scores for pupils at other schools.'''
-    rag_descrip_small = '''
-This means that **less than ten** students in your school completed questions
-for this topic, so the results cannot be shown.'''
-    if output == 'streamlit':
-        rag_intro_column('below', rag_descrip_below)
-        rag_intro_column('average', rag_descrip_average)
-        rag_intro_column('above', rag_descrip_above)
-        rag_intro_column(np.nan, rag_descrip_small)
-    elif output == 'pdf':
-        temp_content.append(
-            rag_intro_column('below', markdown(rag_descrip_below), 'pdf'))
-        temp_content.append(
-            rag_intro_column('average', markdown(rag_descrip_average), 'pdf'))
-        temp_content.append(
-            rag_intro_column('above', markdown(rag_descrip_above), 'pdf'))
-        temp_content.append(
-            rag_intro_column(np.nan, markdown(rag_descrip_small), 'pdf'))
-
-    # Write caveat re: sample size
-    caveat = f'''
-*Please note that  although a total of {school_size} pupils took part, the
-topic summaries below are based only on responses from pupils who completed all
-the questions of a given topic. The count of pupils who completed a topic is
-available on each topic's "Explore results" page. However, the other figures
-on the "Explore results" page present data from all pupils who took part.*'''
-    if output == 'streamlit':
-        st.markdown(caveat)
-    elif output == 'pdf':
-        temp_content.append(markdown(caveat))
-
-    # For PDF report, format into section container and return
-    if output == 'pdf':
-        html_string = f'''
-    <div class='page'>
-        <div class='summary_cover'>
-            {''.join(temp_content)}
-        </div>
-    </div>
-    '''
-        return html_string
-
-
-def summary_table(df_scores, chosen_group, chosen_school,
-                  output='streamlit', content=None):
-    '''
-    Produce the summary RAG table using rows and columns, for streamlit page
-    or PDF report.
-
-    Parameters
-    ----------
-    df_scores : dataframe
-        Dataframe containing the RAG ratings for each topic for each school
-    chosen_group : string
-        The group for results to be viewed by - one of: 'For all pupils',
-        'By year group', 'By gender', 'By FSM', or 'By SEN'
-    chosen_school : string
-        Name of chosen school
-    output : string
-        Specifies whether to write for 'streamlit' (default) or 'pdf'
-    content : list
-        Optional input used when output=='pdf', contains HTML for report.
-
-    Returns
-    -------
-    content : list
-        Optional return, used when output=='pdf', contains HTML for report.
-    '''
-    # Filter by chosen grouping and school
-    chosen, pivot_var, order = filter_by_group(
-        df=df_scores, chosen_group=chosen_group, output='summary',
-        chosen_school=chosen_school)
-
-    # Filter to variable relevant for summary page
-    chosen = chosen[~chosen['variable'].isin([
-        'birth_you_age_score', 'overall_count', 'staff_talk_score',
-        'home_talk_score', 'peer_talk_score'])]
-
-    if chosen_group != 'For all pupils':
-        # Pivot from wide to long whilst maintaining row order
-        chosen = pd.pivot_table(
-            chosen[['variable_lab', pivot_var, 'rag', 'description']],
-            values='rag', index=['variable_lab', 'description'],
-            columns=pivot_var,
-            aggfunc='sum', sort=False).reset_index().replace(0, np.nan)
-        # Reorder columns
-        chosen = chosen[['variable_lab'] + order + ['description']]
-    else:
-        chosen = chosen[['variable_lab', 'rag', 'description']]
-
-    # Extract description (was used for hover over button but that didn't
-    # work with CSS styling presently)
-    # description = chosen['description']
-    chosen = chosen.drop('description', axis=1)
-
-    # Set number of columns
-    ncol = len(chosen.columns)
-
-    # Rename columns if in the dataframe
-    colnames = {'variable_lab': 'Topic',
-                'rag': 'All pupils'}
-    chosen = chosen.rename(columns=colnames)
-
-    # Add the headings for each column for Streamlit
-    if output == 'streamlit':
-        # Set up columns
-        cols = st.columns([0.3, 0.35, 0.35])
-        # For column names in chosen, write that name in a column
-        for i in range(ncol):
-            with cols[i]:
-                st.markdown(f'''
-<p style='text-align: center; font-weight: bold; font-size: 22px;'>
-{chosen.columns[i]}</p>''', unsafe_allow_html=True)
-
-    # Add the headings for each column for PDF:
-    elif output == 'pdf':
-        # Create temporary list for the column headings
-        temp_headings = list()
-        # Create series of strings with HTML code for each column
-        for i in range(ncol):
-            temp_headings.append(f'''
-<div class='column{ncol}'>
-    <p style='text-align:center; font-weight:bold;'>{chosen.columns[i]}</p>
-</div>''')
-        # Combine into a single HTML string
-        content.append(f'''
-<div class='row'>
-    {''.join(temp_headings)}
-</div>''')
-
-    # Add the topics and RAG results in Streamlit:
-    if output == 'streamlit':
-        # For each row of dataframe, create streamlit columns and write data
-        # from cell
-        st.divider()
-        for index, row in chosen.iterrows():
-            cols = st.columns([0.3, 0.35, 0.35])
-            st.divider()
-            for i in range(ncol):
-                # Create topic button or score
-                with cols[i]:
-                    if ((row.iloc[i] in ['below', 'average', 'above']) |
-                            pd.isnull(row.iloc[i])):
-                        result_box(row.iloc[i])
-                    else:
-                        # Create button that, if clicked, changes to details
-                        if st.button(row.iloc[i]):
-                            st.session_state['chosen_variable_lab'] = (
-                                row.iloc[i])
-                            switch_page('explore results')
-
-    # Add the topics and RAG results in PDF:
-    if output == 'pdf':
-        for index, row in chosen.iterrows():
-            content.append('<hr>')
-            # Create temporary list to store the HTML for this row
-            temp_row = list()
-            for i in range(ncol):
-                # Create RAG button HTML
-                if ((row.iloc[i] in ['below', 'average', 'above']) |
-                        pd.isnull(row.iloc[i])):
-                    row_value = result_box(row.iloc[i], 'pdf')
-                # Create topic name HTML
-                else:
-                    row_value = f'''
-<p style='text-align:center;'>{row.iloc[i]}</p>'''
-                # Insert that into the column DIV element
-                temp_row.append(f'''
-<div class='column{ncol}'>
-    {row_value}
-</div>''')
-            # Insert that row into the overall HTML content
-            content.append(f'''
-<div class='row'>
-    {''.join(temp_row)}
-</div>''')
-
-        return content
+'''
+Helper functions for the summary page, and for the production of the 'RAG'
+boxes which are also use on the 'Explore Results' page
+'''
+import pandas as pd
+import streamlit as st
+import numpy as np
+from markdown import markdown
+from .page_setup import blank_lines
+from .reshape_data import filter_by_group
+from .stylable_container import stylable_container
+from .switch_page_button import switch_page
+
+
+def create_rag_container(text, background, font, output='streamlit', key=None):
+    '''
+    Generates a streamlit or HTML container with the specified background and
+    font colours, including the text provided, and with class of 'result_box'
+    if its the HTML container
+
+    Parameters
+    ----------
+    text : string
+        Text to go in the container.
+    background : string
+        Background colour.
+    font : string
+        Font colour.
+    output : string
+        Specifies whether to write for 'streamlit' (default) or 'pdf'.
+    key : string
+        Optional input. Key for the container.
+
+    Returns
+    -------
+    html_string : string
+        HTML string, to be appended to the content for the report
+    '''
+    if output == 'streamlit':
+        with stylable_container(
+            key=key,
+            css_styles=f'''{{
+                background-color: {background};
+                border-radius: 0.5rem;
+                padding: 0px}}''',):
+            blank_lines(1)
+            st.markdown(f'''<p style='text-align: center; color: {font};'>
+                        {text}</p>''', unsafe_allow_html=True)
+            blank_lines(1)
+
+    elif output == 'pdf':
+        html_string = f'''
+    <div class='result_box' style='background: {background}; color: {font}'>
+        <p>{text}</p>
+    </div>'''
+        return html_string
+
+
+def result_box(rag, output='streamlit'):
+    '''
+    Creates a result box with the RAG rating
+
+    Parameters
+    ----------
+    rag : string
+        Result from comparison with other schools - either 'below', 'average',
+        'above', or np.nan
+    output : string
+        Specifies whether to write for 'streamlit' (default) or 'pdf'.
+
+    Returns
+    -------
+    html_string : string
+        HTML string, to be appended to the content for the report
+    '''
+    # Find text and colours depending on RAG rating
+    if rag == 'below':
+        rag_text = 'Below average'
+        background = '#FFCCCC'
+        font = '#95444B'
+    elif rag == 'average':
+        rag_text = 'Average'
+        background = '#FFE8BF'
+        font = '#AA7A18'
+    elif rag == 'above':
+        rag_text = 'Above average'
+        background = '#B6E6B6'
+        font = '#2B7C47'
+    elif pd.isnull(rag):
+        rag_text = 'n < 10'
+        background = '#DCE4FF'
+        font = '#19539A'
+
+    # Create for streamlit or PDF
+    if output == 'streamlit':
+        create_rag_container(rag_text, background, font, output, key=rag)
+    elif output == 'pdf':
+        return create_rag_container(rag_text, background, font, output)
+
+
+def rag_intro_column(rag, rag_descrip, output='streamlit'):
+    '''
+    Generate a row for the introduction to the summary section, with a RAG
+    box and description of that box across 2 columns.
+
+    Parameters
+    ----------
+    rag : string
+        RAG performance - either 'above', 'average', 'below', or np.nan
+    rag_descrip : string
+        Description of the RAG rating
+    output : string
+        Specifies whether to write for 'streamlit' (default) or 'pdf'.
+
+    Returns
+    -------
+    html_string : string
+        Section of HTML that creates the RAG introductory columns
+    '''
+    # Streamlit version
+    if output == 'streamlit':
+        cols = st.columns(2)
+        with cols[0]:
+            result_box(rag)
+        with cols[1]:
+            st.markdown(rag_descrip)
+
+    # PDF version
+    elif output == 'pdf':
+        rag_box = result_box(rag, output='pdf')
+        html_string = f'''
+<div class='row'>
+    <div class='column2' style='margin-top:0.5em;'>
+        {rag_box}
+    </div>
+    <div class='column2'>
+        {rag_descrip}
+    </div>
+</div>
+'''
+        return html_string
+
+
+def summary_intro(school_size, output='streamlit'):
+    '''
+    Creates the introduction for the summary section
+
+    Parameters
+    ----------
+    school_size : integer
+        Total number of pupils at school (who answered at least one question)
+    output : string
+        Specifies whether to write for 'streamlit' (default) or 'pdf'
+
+    Returns
+    -------
+    html_string : string
+        Optional return, if output=='pdf', contains HTML for summary cover page
+    '''
+    # For PDF report, create temporary list to store HTML for page
+    if output == 'pdf':
+        temp_content = []
+
+    # Write title for this section
+    title = '''Summary of your school's results'''
+    if output == 'streamlit':
+        st.title(title)
+        st.subheader('Introduction')
+    elif output == 'pdf':
+        temp_content.append(f'''<h1 style='page-break-before:always;'
+                            id='summary'>{title}</h1>''')
+
+    # Write introductory sentence for summary section
+    descrip = f'''
+At your school, a total of {school_size} pupils took part in the #BeeWell
+survey. This page shows how the answers of pupils at your school compare with
+pupils from other schools in Northern Devon.'''
+    if output == 'streamlit':
+        st.markdown(descrip)
+    elif output == 'pdf':
+        temp_content.append(f'<p>{descrip}</p>')
+
+    # Write interpretation of each of the rag boxes
+    rag_descrip_below = '''
+This means that average scores for students in your school are **worse** than
+average scores for pupils at other schools.'''
+    rag_descrip_average = '''
+This means that average scores for students in your school are **similar** to
+average scores for pupils at other schools.'''
+    rag_descrip_above = '''
+This means that average scores for students in your school are **better** than
+average scores for pupils at other schools.'''
+    rag_descrip_small = '''
+This means that **less than ten** students in your school completed questions
+for this topic, so the results cannot be shown.'''
+    if output == 'streamlit':
+        rag_intro_column('below', rag_descrip_below)
+        rag_intro_column('average', rag_descrip_average)
+        rag_intro_column('above', rag_descrip_above)
+        rag_intro_column(np.nan, rag_descrip_small)
+    elif output == 'pdf':
+        temp_content.append(
+            rag_intro_column('below', markdown(rag_descrip_below), 'pdf'))
+        temp_content.append(
+            rag_intro_column('average', markdown(rag_descrip_average), 'pdf'))
+        temp_content.append(
+            rag_intro_column('above', markdown(rag_descrip_above), 'pdf'))
+        temp_content.append(
+            rag_intro_column(np.nan, markdown(rag_descrip_small), 'pdf'))
+
+    # Write caveat re: sample size
+    caveat = f'''
+*Please note that  although a total of {school_size} pupils took part, the
+topic summaries below are based only on responses from pupils who completed all
+the questions of a given topic. The count of pupils who completed a topic is
+available on each topic's "Explore results" page. However, the other figures
+on the "Explore results" page present data from all pupils who took part.*'''
+    if output == 'streamlit':
+        st.markdown(caveat)
+    elif output == 'pdf':
+        temp_content.append(markdown(caveat))
+
+    # For PDF report, format into section container and return
+    if output == 'pdf':
+        html_string = f'''
+    <div class='page'>
+        <div class='summary_cover'>
+            {''.join(temp_content)}
+        </div>
+    </div>
+    '''
+        return html_string
+
+
+def summary_table(df_scores, chosen_group, chosen_school,
+                  output='streamlit', content=None):
+    '''
+    Produce the summary RAG table using rows and columns, for streamlit page
+    or PDF report.
+
+    Parameters
+    ----------
+    df_scores : dataframe
+        Dataframe containing the RAG ratings for each topic for each school
+    chosen_group : string
+        The group for results to be viewed by - one of: 'For all pupils',
+        'By year group', 'By gender', 'By FSM', or 'By SEN'
+    chosen_school : string
+        Name of chosen school
+    output : string
+        Specifies whether to write for 'streamlit' (default) or 'pdf'
+    content : list
+        Optional input used when output=='pdf', contains HTML for report.
+
+    Returns
+    -------
+    content : list
+        Optional return, used when output=='pdf', contains HTML for report.
+    '''
+    # Filter by chosen grouping and school
+    chosen, pivot_var, order = filter_by_group(
+        df=df_scores, chosen_group=chosen_group, output='summary',
+        chosen_school=chosen_school)
+
+    # Filter to variable relevant for summary page
+    chosen = chosen[~chosen['variable'].isin([
+        'birth_you_age_score', 'overall_count', 'staff_talk_score',
+        'home_talk_score', 'peer_talk_score'])]
+
+    if chosen_group != 'For all pupils':
+        # Pivot from wide to long whilst maintaining row order
+        chosen = pd.pivot_table(
+            chosen[['variable_lab', pivot_var, 'rag', 'description']],
+            values='rag', index=['variable_lab', 'description'],
+            columns=pivot_var,
+            aggfunc='sum', sort=False).reset_index().replace(0, np.nan)
+        # Reorder columns
+        chosen = chosen[['variable_lab'] + order + ['description']]
+    else:
+        chosen = chosen[['variable_lab', 'rag', 'description']]
+
+    # Extract description (was used for hover over button but that didn't
+    # work with CSS styling presently)
+    # description = chosen['description']
+    chosen = chosen.drop('description', axis=1)
+
+    # Set number of columns
+    ncol = len(chosen.columns)
+
+    # Rename columns if in the dataframe
+    colnames = {'variable_lab': 'Topic',
+                'rag': 'All pupils'}
+    chosen = chosen.rename(columns=colnames)
+
+    # Add the headings for each column for Streamlit
+    if output == 'streamlit':
+        # Set up columns
+        cols = st.columns([0.3, 0.35, 0.35])
+        # For column names in chosen, write that name in a column
+        for i in range(ncol):
+            with cols[i]:
+                st.markdown(f'''
+<p style='text-align: center; font-weight: bold; font-size: 22px;'>
+{chosen.columns[i]}</p>''', unsafe_allow_html=True)
+
+    # Add the headings for each column for PDF:
+    elif output == 'pdf':
+        # Create temporary list for the column headings
+        temp_headings = list()
+        # Create series of strings with HTML code for each column
+        for i in range(ncol):
+            temp_headings.append(f'''
+<div class='column{ncol}'>
+    <p style='text-align:center; font-weight:bold;'>{chosen.columns[i]}</p>
+</div>''')
+        # Combine into a single HTML string
+        content.append(f'''
+<div class='row'>
+    {''.join(temp_headings)}
+</div>''')
+
+    # Add the topics and RAG results in Streamlit:
+    if output == 'streamlit':
+        # For each row of dataframe, create streamlit columns and write data
+        # from cell
+        st.divider()
+        for index, row in chosen.iterrows():
+            cols = st.columns([0.3, 0.35, 0.35])
+            st.divider()
+            for i in range(ncol):
+                # Create topic button or score
+                with cols[i]:
+                    if ((row.iloc[i] in ['below', 'average', 'above']) |
+                            pd.isnull(row.iloc[i])):
+                        result_box(row.iloc[i])
+                    else:
+                        # Create button that, if clicked, changes to details
+                        if st.button(row.iloc[i]):
+                            st.session_state['chosen_variable_lab'] = (
+                                row.iloc[i])
+                            switch_page('explore results')
+
+    # Add the topics and RAG results in PDF:
+    if output == 'pdf':
+        for index, row in chosen.iterrows():
+            content.append('<hr>')
+            # Create temporary list to store the HTML for this row
+            temp_row = list()
+            for i in range(ncol):
+                # Create RAG button HTML
+                if ((row.iloc[i] in ['below', 'average', 'above']) |
+                        pd.isnull(row.iloc[i])):
+                    row_value = result_box(row.iloc[i], 'pdf')
+                # Create topic name HTML
+                else:
+                    row_value = f'''
+<p style='text-align:center;'>{row.iloc[i]}</p>'''
+                # Insert that into the column DIV element
+                temp_row.append(f'''
+<div class='column{ncol}'>
+    {row_value}
+</div>''')
+            # Insert that row into the overall HTML content
+            content.append(f'''
+<div class='row'>
+    {''.join(temp_row)}
+</div>''')
+
+        return content
```

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/synthesise_aggregate.py` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/synthesise_aggregate.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,382 +1,382 @@
-'''
-Functions which aggregate pupil-level data - as part of several files
-which provide functions for synthesis (creation and aggregation) of data
-for the dashboard.
-'''
-import numpy as np
-import pandas as pd
-import re
-
-
-def results_by_site_and_group(
-        data, agg_func, no_pupils, response_col=None, labels=None,
-        group_type='standard', site_col='school_lab'):
-    '''
-    Aggregate results for all possible sites (schools or areas) and groups
-    (setting result to 0 or NaN if no pupils from a particular group are
-    present).
-
-    Parameters
-    ----------
-    data : pandas dataframe
-        Pupil-level survey responses, with their school and demographics
-    agg_func : function
-        Method for aggregating the dataset
-    no_pupils: pandas dataframe
-        Output of agg_func() where all counts are set to 0 and other results
-        set to NaN, to be used in cases where there are no pupils of a
-        particular group (e.g. no FSM / SEN / Year 8)
-    response_col : list
-        Optional argument used when agg_func is aggregate_proportions(). It is
-        the list of columns that we want to aggregate.
-    labels : dictionary
-        Optional argument used when agg_func is aggregate_proportions(). It is
-        a dictionary with all possible questions as keys, then values are
-        another dictionary where keys are all the possible numeric (or nan)
-        answers to the question, and values are relevant label for each answer.
-    group_type : string
-        Links to the type of demographic groupings performed. Either
-        'standard', 'symbol' or 'none' - default is standard.
-    site_col: string
-        Name of column with site - e.g. 'school_lab' (default), 'msoa'.
-
-    Returns
-    -------
-    result : pandas DataFrame
-        Dataframe where each row has the aggregation results, along with
-        the relevant school and pupil groups used in that calculation
-    '''
-
-    # Initialise list to store results
-    result_list = list()
-
-    # Define the groups that we want to aggregate by - when providing a filter,
-    # first value is the name of the category and the second is the variable
-    if group_type == 'standard':
-        groups = [
-            'All',
-            ['Year 8', 'year_group_lab'],
-            ['Year 10', 'year_group_lab'],
-            ['Girl', 'gender_lab'],
-            ['Boy', 'gender_lab'],
-            ['FSM', 'fsm_lab'],
-            ['Non-FSM', 'fsm_lab'],
-            ['SEN', 'sen_lab'],
-            ['Non-SEN', 'sen_lab']]
-    elif group_type == 'symbol':
-        groups = [
-            'All',
-            ['Year 7', 'year_group_lab'],
-            ['Year 8', 'year_group_lab'],
-            ['Year 9', 'year_group_lab'],
-            ['Year 10', 'year_group_lab'],
-            ['Year 11', 'year_group_lab'],
-            ['Girl', 'gender_lab'],
-            ['Boy', 'gender_lab'],
-            ['FSM', 'fsm_lab'],
-            ['Non-FSM', 'fsm_lab']]
-    elif group_type == 'none':
-        groups = ['All']
-
-    # For each of the sites (which we know will all be present at least once
-    # as we base the site list on the dataset itself)
-    sites = data[site_col].dropna().drop_duplicates().sort_values()
-    for site in sites:
-
-        # For each the groupings
-        for group in groups:
-
-            # Find results for that site. If group is not equal to all,
-            # then apply additional filters
-            to_agg = data[data[site_col] == site]
-            if group != 'All':
-                to_agg = to_agg[to_agg[group[1]] == group[0]]
-
-            # If the dataframe is empty (i.e. you applied a filter but there
-            # were no students matching that filter) then set to the no_pupils
-            # df. Otherwise, aggregate the data using the provided function
-            if len(to_agg.index) == 0:
-                res = no_pupils.copy()
-            else:
-                if response_col is None:
-                    res = agg_func(to_agg)
-                else:
-                    res = agg_func(
-                        data=to_agg, response_col=response_col, labels=labels)
-
-            # Specify what site it was
-            res[site_col] = site
-
-            # Set each group as all, replacing one if filter used
-            if group_type != 'none':
-                res['year_group_lab'] = 'All'
-                res['gender_lab'] = 'All'
-                res['fsm_lab'] = 'All'
-                if group_type == 'standard':
-                    res['sen_lab'] = 'All'
-                if group != 'All':
-                    res[group[1]] = group[0]
-
-            # Append results to list
-            result_list.append(res)
-
-    # Combine all the results into a single dataframe
-    result = pd.concat(result_list)
-    return result
-
-
-def aggregate_scores(df):
-    '''
-    Aggregate the score columns in the provided dataset, finding the mean and
-    count of non-NaN
-
-    Parameters:
-    -----------
-    df : dataframe
-        Dataframe with rows for each pupils and containing the score columns
-
-    Returns:
-    -------
-    res : dataframe
-        Dataframe with mean and count for each score
-    '''
-    # Make a list of the columns that provide a score
-    score_col = [col for col in df.columns if col.endswith('_score')]
-
-    res = pd.DataFrame({
-        # Find mean for each score column, ignoring NaN
-        'mean': df[score_col].mean(),
-        # Count non-NaN so we know the number of pupils used in the mea
-        'count': df[score_col].count()}).rename_axis('variable').reset_index()
-    return res
-
-
-def convert_boolean(true_list, false_list, mask):
-    '''
-    Conditionally replace values of boolean list from one list when True and
-    another when False.
-
-    Parameters
-    ----------
-    true_list : list
-        Contains values to use if True
-    false_list : list
-        Contains values to use if False
-    mask : list
-        Boolean list
-    '''
-    iter_true = iter(true_list)
-    iter_false = iter(false_list)
-    return [next(iter_true) if item else next(iter_false) for item in mask]
-
-
-def aggregate_proportions(data, response_col, labels, hide_low_response=False):
-    '''
-    Aggregates each of the columns provided by response_col, for the chosen
-    dataset.
-
-    This function uses the known possible values for each column, it counts
-    occurences of each (inc. number missing) and makes the answer as a single
-    dataframe row, where counts and percentages and categories are stored as
-    lists within cells of that row. The function returns a dataframe containing
-    all of those rows. It is designed to based on all possible values rather
-    than only on values present - else e.g. if no-one responded 3, you could
-    have a function that just returns counts of responses to 1, 2 and 4, which
-    would then create issues when we try and plot the data.
-
-    For the branching question (talking about feelings), the value counts are
-    calculated from a subset of the data (as the no response should only be
-    from those who branched onto that question, and not those who branched onto
-    the other question (or never answered the first branching question)).
-
-    Parameters
-    ----------
-    data : dataframe
-        Dataframe with rows for each pupil and including all the response_col
-    response_col : list
-        List of columns that we want to aggregate
-    labels : dictionary
-        Dictionary with all possible questions as keys, then values are another
-        dictionary where keys are all the possible numeric (or nan) answers to
-        the question, and values are the relevant label for each answer.
-    hide_low_response : boolean
-        Whether to hide responses when a response option gets less than 10
-        responses (rather than norm elsewhere, which is just requiring 10
-        responses to the entire item rather than to each response option)
-
-    Returns
-    -------
-    pd.concat(rows): dataframe
-        Dataframe with the aggregate responses to each of the response_col
-    '''
-    # Initialise list to store rows of the dataframe
-    rows = list()
-
-    # Loop through the columns of interest
-    for col_lab in response_col:
-
-        # Find the name of the numeric version of the column
-        col = col_lab.replace('_lab', '')
-
-        # Identify if column is branching from "yes" to talking with someone
-        if any([substring in col for substring in ['talk_listen',
-                                                   'talk_helpful']]):
-            # Get the prefix (staff, home or peer)
-            prefix = re.sub('_talk_listen|_talk_helpful', '', col)
-            # Filter the data to only those who said they talked with them
-            # (branch)
-            data_subset = data[data[f'{prefix}_talk'] == 1]
-            # Find value counts
-            value_counts = data_subset[col].value_counts(dropna=False)
-
-        # Identify if the column is branching from "no" to talking with someone
-        elif 'talk_if' in col:
-            # Get the prefix (staff, home or peer)
-            prefix = re.sub('_talk_if', '', col)
-            # Filter the data to only those who said they didn't talk to them
-            # (branch)
-            data_subset = data[data[f'{prefix}_talk'] == 0]
-            # Find value counts
-            value_counts = data_subset[col].value_counts(dropna=False)
-
-        # For any other columns, no subsetting of the data is required
-        else:
-            # Find value counts
-            value_counts = data[col].value_counts(dropna=False)
-
-        # Get all possible category values and labels from dictionary
-        cat = list(labels[col].keys())
-        cat_lab = list(labels[col].values())
-
-        # Initalise list for storing counts
-        counts = []
-        # For each of the possible values in labels - if the value was present,
-        # extract from the counts series, but if not, set count to 0
-        for value in labels[col].keys():
-            if value in value_counts.index:
-                counts.append(value_counts[value])
-            else:
-                counts.append(0)
-
-        # Convert list of counts to list of percentages, and create rounded
-        # version
-        percentages = [(x/sum(counts))*100 for x in counts]
-
-        # If True to hide when individual response options are n<10
-        if hide_low_response:
-            # Create mask which is TRUE when responses where n>=10 (ignoring
-            # final option (non-response) which we don't mind being n<10)
-            mask = [x >= 10 for x in counts[:-1]]
-
-            # If all >=10, keep non-response
-            if all(mask):
-                mask += [True]
-            # If any option is <10, also hide non-response (else could deduce)
-            else:
-                mask += [False]
-
-            # Use mask to set values to NaN
-            counts = convert_boolean(
-                counts, np.full(len(counts), np.nan), mask)
-            percentages = convert_boolean(
-                percentages, np.full(len(percentages), np.nan), mask)
-
-        # Create dataframe row using the calculated data
-        # Use np.nansum() so it ignores NaN when calculating sum
-        df_row = pd.DataFrame({
-            'cat': [cat],
-            'cat_lab': [cat_lab],
-            'count': [counts],
-            'percentage': [percentages],
-            'measure': col,
-            'n_responses': np.nansum(counts)
-        })
-        # Append to list
-        rows.append(df_row)
-
-    # Combine into a single dataframe and return
-    return pd.concat(rows)
-
-
-def aggregate_counts(df):
-    '''
-    Aggregates the provided dataframe by finding the total people in it.
-
-    Parameters
-    ----------
-    df : Dataframe
-        Dataframe with row for each pupil and columns that include the school
-        and groups needed by results_by_site_and_group()
-
-    Returns
-    -------
-    res : Dataframe
-        Dataframe with the count of pupils in each school and group
-    '''
-    res = pd.DataFrame({
-        'count': [len(df.index)]
-    })
-    return res
-
-
-def aggregate_demographic(data, response_col, labels):
-    '''
-    Aggregates the demographic data by school and group (seperate to
-    results_by_school_and_group() as we want to aggregate by school v.s. all
-    others rather than for each school, and as we don't want to break down
-    results any further by any demographic characteristics)
-
-    Parameters
-    ----------
-    data : dataframe
-        Dataframe containing pupil-level demographic data
-    response_col : array
-        List of demographic columns to be aggregated
-    labels : dictionary
-        Dictionary with response options for each variable
-
-    Returns
-    -------
-    result : dataframe
-        Dataframe with % responses to demographic questions, for each school,
-        compared with all other schools
-    '''
-    # Initialise list to store results
-    result_list = list()
-
-    # For each of the schools (which we know will all be present at least once
-    # as we base the school list on the dataset itself)
-    schools = data['school_lab'].dropna().drop_duplicates().sort_values()
-    for school in schools:
-
-        # Add label identifying the school as being the current one or now
-        data['school_group'] = np.where(data['school_lab'] == school, 1, 0)
-
-        # Loop through each of those groups (current school vs. other schools)
-        for group in [1, 0]:
-
-            # Filter to the group and then aggregate the data
-            to_agg = data[data['school_group'] == group]
-            res = aggregate_proportions(
-                data=to_agg, response_col=response_col, labels=labels,
-                hide_low_response=True)
-
-            # Label with the group
-            res['school_lab'] = school
-            res['school_group'] = group
-
-            # Append results to list
-            result_list.append(res)
-
-    # Combine all the results into a single dataframe
-    result = pd.concat(result_list)
-
-    # Hide results where n<10 overall (in addition to item-level already done)
-    result.loc[result['n_responses'] < 10,
-               ['count', 'percentage', 'n_responses']] = np.nan
-
-    # Add labels that can use in figures
-    result['school_group_lab'] = np.where(
-        result['school_group'] == 1, 'Your school', 'Other schools')
-
-    return result
+'''
+Functions which aggregate pupil-level data - as part of several files
+which provide functions for synthesis (creation and aggregation) of data
+for the dashboard.
+'''
+import numpy as np
+import pandas as pd
+import re
+
+
+def results_by_site_and_group(
+        data, agg_func, no_pupils, response_col=None, labels=None,
+        group_type='standard', site_col='school_lab'):
+    '''
+    Aggregate results for all possible sites (schools or areas) and groups
+    (setting result to 0 or NaN if no pupils from a particular group are
+    present).
+
+    Parameters
+    ----------
+    data : pandas dataframe
+        Pupil-level survey responses, with their school and demographics
+    agg_func : function
+        Method for aggregating the dataset
+    no_pupils: pandas dataframe
+        Output of agg_func() where all counts are set to 0 and other results
+        set to NaN, to be used in cases where there are no pupils of a
+        particular group (e.g. no FSM / SEN / Year 8)
+    response_col : list
+        Optional argument used when agg_func is aggregate_proportions(). It is
+        the list of columns that we want to aggregate.
+    labels : dictionary
+        Optional argument used when agg_func is aggregate_proportions(). It is
+        a dictionary with all possible questions as keys, then values are
+        another dictionary where keys are all the possible numeric (or nan)
+        answers to the question, and values are relevant label for each answer.
+    group_type : string
+        Links to the type of demographic groupings performed. Either
+        'standard', 'symbol' or 'none' - default is standard.
+    site_col: string
+        Name of column with site - e.g. 'school_lab' (default), 'msoa'.
+
+    Returns
+    -------
+    result : pandas DataFrame
+        Dataframe where each row has the aggregation results, along with
+        the relevant school and pupil groups used in that calculation
+    '''
+
+    # Initialise list to store results
+    result_list = list()
+
+    # Define the groups that we want to aggregate by - when providing a filter,
+    # first value is the name of the category and the second is the variable
+    if group_type == 'standard':
+        groups = [
+            'All',
+            ['Year 8', 'year_group_lab'],
+            ['Year 10', 'year_group_lab'],
+            ['Girl', 'gender_lab'],
+            ['Boy', 'gender_lab'],
+            ['FSM', 'fsm_lab'],
+            ['Non-FSM', 'fsm_lab'],
+            ['SEN', 'sen_lab'],
+            ['Non-SEN', 'sen_lab']]
+    elif group_type == 'symbol':
+        groups = [
+            'All',
+            ['Year 7', 'year_group_lab'],
+            ['Year 8', 'year_group_lab'],
+            ['Year 9', 'year_group_lab'],
+            ['Year 10', 'year_group_lab'],
+            ['Year 11', 'year_group_lab'],
+            ['Girl', 'gender_lab'],
+            ['Boy', 'gender_lab'],
+            ['FSM', 'fsm_lab'],
+            ['Non-FSM', 'fsm_lab']]
+    elif group_type == 'none':
+        groups = ['All']
+
+    # For each of the sites (which we know will all be present at least once
+    # as we base the site list on the dataset itself)
+    sites = data[site_col].dropna().drop_duplicates().sort_values()
+    for site in sites:
+
+        # For each the groupings
+        for group in groups:
+
+            # Find results for that site. If group is not equal to all,
+            # then apply additional filters
+            to_agg = data[data[site_col] == site]
+            if group != 'All':
+                to_agg = to_agg[to_agg[group[1]] == group[0]]
+
+            # If the dataframe is empty (i.e. you applied a filter but there
+            # were no students matching that filter) then set to the no_pupils
+            # df. Otherwise, aggregate the data using the provided function
+            if len(to_agg.index) == 0:
+                res = no_pupils.copy()
+            else:
+                if response_col is None:
+                    res = agg_func(to_agg)
+                else:
+                    res = agg_func(
+                        data=to_agg, response_col=response_col, labels=labels)
+
+            # Specify what site it was
+            res[site_col] = site
+
+            # Set each group as all, replacing one if filter used
+            if group_type != 'none':
+                res['year_group_lab'] = 'All'
+                res['gender_lab'] = 'All'
+                res['fsm_lab'] = 'All'
+                if group_type == 'standard':
+                    res['sen_lab'] = 'All'
+                if group != 'All':
+                    res[group[1]] = group[0]
+
+            # Append results to list
+            result_list.append(res)
+
+    # Combine all the results into a single dataframe
+    result = pd.concat(result_list)
+    return result
+
+
+def aggregate_scores(df):
+    '''
+    Aggregate the score columns in the provided dataset, finding the mean and
+    count of non-NaN
+
+    Parameters:
+    -----------
+    df : dataframe
+        Dataframe with rows for each pupils and containing the score columns
+
+    Returns:
+    -------
+    res : dataframe
+        Dataframe with mean and count for each score
+    '''
+    # Make a list of the columns that provide a score
+    score_col = [col for col in df.columns if col.endswith('_score')]
+
+    res = pd.DataFrame({
+        # Find mean for each score column, ignoring NaN
+        'mean': df[score_col].mean(),
+        # Count non-NaN so we know the number of pupils used in the mea
+        'count': df[score_col].count()}).rename_axis('variable').reset_index()
+    return res
+
+
+def convert_boolean(true_list, false_list, mask):
+    '''
+    Conditionally replace values of boolean list from one list when True and
+    another when False.
+
+    Parameters
+    ----------
+    true_list : list
+        Contains values to use if True
+    false_list : list
+        Contains values to use if False
+    mask : list
+        Boolean list
+    '''
+    iter_true = iter(true_list)
+    iter_false = iter(false_list)
+    return [next(iter_true) if item else next(iter_false) for item in mask]
+
+
+def aggregate_proportions(data, response_col, labels, hide_low_response=False):
+    '''
+    Aggregates each of the columns provided by response_col, for the chosen
+    dataset.
+
+    This function uses the known possible values for each column, it counts
+    occurences of each (inc. number missing) and makes the answer as a single
+    dataframe row, where counts and percentages and categories are stored as
+    lists within cells of that row. The function returns a dataframe containing
+    all of those rows. It is designed to based on all possible values rather
+    than only on values present - else e.g. if no-one responded 3, you could
+    have a function that just returns counts of responses to 1, 2 and 4, which
+    would then create issues when we try and plot the data.
+
+    For the branching question (talking about feelings), the value counts are
+    calculated from a subset of the data (as the no response should only be
+    from those who branched onto that question, and not those who branched onto
+    the other question (or never answered the first branching question)).
+
+    Parameters
+    ----------
+    data : dataframe
+        Dataframe with rows for each pupil and including all the response_col
+    response_col : list
+        List of columns that we want to aggregate
+    labels : dictionary
+        Dictionary with all possible questions as keys, then values are another
+        dictionary where keys are all the possible numeric (or nan) answers to
+        the question, and values are the relevant label for each answer.
+    hide_low_response : boolean
+        Whether to hide responses when a response option gets less than 10
+        responses (rather than norm elsewhere, which is just requiring 10
+        responses to the entire item rather than to each response option)
+
+    Returns
+    -------
+    pd.concat(rows): dataframe
+        Dataframe with the aggregate responses to each of the response_col
+    '''
+    # Initialise list to store rows of the dataframe
+    rows = list()
+
+    # Loop through the columns of interest
+    for col_lab in response_col:
+
+        # Find the name of the numeric version of the column
+        col = col_lab.replace('_lab', '')
+
+        # Identify if column is branching from "yes" to talking with someone
+        if any([substring in col for substring in ['talk_listen',
+                                                   'talk_helpful']]):
+            # Get the prefix (staff, home or peer)
+            prefix = re.sub('_talk_listen|_talk_helpful', '', col)
+            # Filter the data to only those who said they talked with them
+            # (branch)
+            data_subset = data[data[f'{prefix}_talk'] == 1]
+            # Find value counts
+            value_counts = data_subset[col].value_counts(dropna=False)
+
+        # Identify if the column is branching from "no" to talking with someone
+        elif 'talk_if' in col:
+            # Get the prefix (staff, home or peer)
+            prefix = re.sub('_talk_if', '', col)
+            # Filter the data to only those who said they didn't talk to them
+            # (branch)
+            data_subset = data[data[f'{prefix}_talk'] == 0]
+            # Find value counts
+            value_counts = data_subset[col].value_counts(dropna=False)
+
+        # For any other columns, no subsetting of the data is required
+        else:
+            # Find value counts
+            value_counts = data[col].value_counts(dropna=False)
+
+        # Get all possible category values and labels from dictionary
+        cat = list(labels[col].keys())
+        cat_lab = list(labels[col].values())
+
+        # Initalise list for storing counts
+        counts = []
+        # For each of the possible values in labels - if the value was present,
+        # extract from the counts series, but if not, set count to 0
+        for value in labels[col].keys():
+            if value in value_counts.index:
+                counts.append(value_counts[value])
+            else:
+                counts.append(0)
+
+        # Convert list of counts to list of percentages, and create rounded
+        # version
+        percentages = [(x/sum(counts))*100 for x in counts]
+
+        # If True to hide when individual response options are n<10
+        if hide_low_response:
+            # Create mask which is TRUE when responses where n>=10 (ignoring
+            # final option (non-response) which we don't mind being n<10)
+            mask = [x >= 10 for x in counts[:-1]]
+
+            # If all >=10, keep non-response
+            if all(mask):
+                mask += [True]
+            # If any option is <10, also hide non-response (else could deduce)
+            else:
+                mask += [False]
+
+            # Use mask to set values to NaN
+            counts = convert_boolean(
+                counts, np.full(len(counts), np.nan), mask)
+            percentages = convert_boolean(
+                percentages, np.full(len(percentages), np.nan), mask)
+
+        # Create dataframe row using the calculated data
+        # Use np.nansum() so it ignores NaN when calculating sum
+        df_row = pd.DataFrame({
+            'cat': [cat],
+            'cat_lab': [cat_lab],
+            'count': [counts],
+            'percentage': [percentages],
+            'measure': col,
+            'n_responses': np.nansum(counts)
+        })
+        # Append to list
+        rows.append(df_row)
+
+    # Combine into a single dataframe and return
+    return pd.concat(rows)
+
+
+def aggregate_counts(df):
+    '''
+    Aggregates the provided dataframe by finding the total people in it.
+
+    Parameters
+    ----------
+    df : Dataframe
+        Dataframe with row for each pupil and columns that include the school
+        and groups needed by results_by_site_and_group()
+
+    Returns
+    -------
+    res : Dataframe
+        Dataframe with the count of pupils in each school and group
+    '''
+    res = pd.DataFrame({
+        'count': [len(df.index)]
+    })
+    return res
+
+
+def aggregate_demographic(data, response_col, labels):
+    '''
+    Aggregates the demographic data by school and group (seperate to
+    results_by_school_and_group() as we want to aggregate by school v.s. all
+    others rather than for each school, and as we don't want to break down
+    results any further by any demographic characteristics)
+
+    Parameters
+    ----------
+    data : dataframe
+        Dataframe containing pupil-level demographic data
+    response_col : array
+        List of demographic columns to be aggregated
+    labels : dictionary
+        Dictionary with response options for each variable
+
+    Returns
+    -------
+    result : dataframe
+        Dataframe with % responses to demographic questions, for each school,
+        compared with all other schools
+    '''
+    # Initialise list to store results
+    result_list = list()
+
+    # For each of the schools (which we know will all be present at least once
+    # as we base the school list on the dataset itself)
+    schools = data['school_lab'].dropna().drop_duplicates().sort_values()
+    for school in schools:
+
+        # Add label identifying the school as being the current one or now
+        data['school_group'] = np.where(data['school_lab'] == school, 1, 0)
+
+        # Loop through each of those groups (current school vs. other schools)
+        for group in [1, 0]:
+
+            # Filter to the group and then aggregate the data
+            to_agg = data[data['school_group'] == group]
+            res = aggregate_proportions(
+                data=to_agg, response_col=response_col, labels=labels,
+                hide_low_response=True)
+
+            # Label with the group
+            res['school_lab'] = school
+            res['school_group'] = group
+
+            # Append results to list
+            result_list.append(res)
+
+    # Combine all the results into a single dataframe
+    result = pd.concat(result_list)
+
+    # Hide results where n<10 overall (in addition to item-level already done)
+    result.loc[result['n_responses'] < 10,
+               ['count', 'percentage', 'n_responses']] = np.nan
+
+    # Add labels that can use in figures
+    result['school_group_lab'] = np.where(
+        result['school_group'] == 1, 'Your school', 'Other schools')
+
+    return result
```

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/synthesise_demographic.py` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/synthesise_demographic.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,98 +1,98 @@
-'''
-Functions which focus on demographic data - as part of several files
-which provide functions for synthesis (creation and aggregation) of data
-for the dashboard.
-'''
-from collections import defaultdict
-from .synthesise_responses import add_keys
-
-
-def add_standard_demographic_groups(df):
-    '''
-    Adds a 'plot_group' column providing demographic topic group for each item
-    in 'measure', for the standard survey demographic responses / data.
-
-    Parameters
-    ----------
-    df : Dataframe
-        Dataframe containing 'measure' column, which we want to add
-        'plot_group' column to.
-    '''
-    # Initialise dictionary of groups
-    groups = defaultdict(str)
-
-    # Specify group for each measure, adding to the groups dictionary
-    add_keys(groups, 'year_group', ['year_group'])
-    add_keys(groups, 'fsm', ['fsm'])
-    add_keys(groups, 'ethnicity', ['ethnicity'])
-    add_keys(groups, 'english_additional', ['english_additional'])
-    add_keys(groups, 'gender', ['gender', 'transgender'])
-    add_keys(groups, 'care_experience', ['care_experience'])
-    add_keys(groups, 'young_carer', ['young_carer'])
-    add_keys(groups, 'neuro', ['sen', 'neurodivergent'])
-    add_keys(groups, 'birth', ['birth_parent1', 'birth_parent2',
-                               'birth_you', 'birth_you_age'])
-    add_keys(groups, 'sexual_orientation', ['sexual_orientation'])
-
-    # Add groups to the dataframe
-    df['plot_group'] = df['measure'].map(groups)
-    return df
-
-
-def add_standard_demographic_response_labels(df):
-    '''
-    Adds labels for each of the demographic survey questions / data in the
-    standard survey
-
-    Parameters
-    ----------
-    df : dataframe
-        Dataframe containing 'measure' column which we want to add labels to
-    '''
-    # Define labels
-    labels = {
-        'gender': 'Gender',
-        'transgender': 'Do you consider yourself to be transgender?',
-        'sexual_orientation': 'Sexual orientation',
-        'neurodivergent': 'Do you identify as neurodivergent?',
-        'young_carer': '''In the last year, have you regularly taken on caring
-    responsibilities for a family member - e.g. due to illness, disability,
-    mental health condition or drug/alcohol dependency?''',
-        'care_experience': '''Are you or have you ever been in care (living in
-    a foster placement, residential placement, or private/kinship care)?''',
-        'birth_parent1': 'Was birth parent 1 born outside the UK?',
-        'birth_parent2': 'Was birth parent 2 born outside the UK?',
-        'birth_you': 'Were you born outside the UK?',
-        'year_group': 'Year group',
-        'fsm': 'Free school meals',
-        'sen': 'Special educational needs',
-        'ethnicity': 'Ethnicity',
-        'english_additional': 'English as an additional language'}
-
-    # Add labels to the dataframe
-    df['measure_lab'] = df['measure'].map(labels)
-    return df
-
-
-def add_symbol_demographic_response_labels(df):
-    '''
-    Adds labels for each of the demographic survey questions / data in the
-    symbol survey
-
-    Parameters
-    ----------
-    df : dataframe
-        Dataframe containing 'measure' column which we want to add labels to
-    '''
-    # Define labels
-    labels = {
-        'gender': 'Gender',
-        'year_group': 'Year group',
-        'fsm': 'Free school meals',
-        'sen': 'Special educational needs',
-        'ethnicity': 'Ethnicity',
-        'english_additional': 'English as an additional language'}
-
-    # Add labels to the dataframe
-    df['measure_lab'] = df['measure'].map(labels)
-    return df
+'''
+Functions which focus on demographic data - as part of several files
+which provide functions for synthesis (creation and aggregation) of data
+for the dashboard.
+'''
+from collections import defaultdict
+from .synthesise_responses import add_keys
+
+
+def add_standard_demographic_groups(df):
+    '''
+    Adds a 'plot_group' column providing demographic topic group for each item
+    in 'measure', for the standard survey demographic responses / data.
+
+    Parameters
+    ----------
+    df : Dataframe
+        Dataframe containing 'measure' column, which we want to add
+        'plot_group' column to.
+    '''
+    # Initialise dictionary of groups
+    groups = defaultdict(str)
+
+    # Specify group for each measure, adding to the groups dictionary
+    add_keys(groups, 'year_group', ['year_group'])
+    add_keys(groups, 'fsm', ['fsm'])
+    add_keys(groups, 'ethnicity', ['ethnicity'])
+    add_keys(groups, 'english_additional', ['english_additional'])
+    add_keys(groups, 'gender', ['gender', 'transgender'])
+    add_keys(groups, 'care_experience', ['care_experience'])
+    add_keys(groups, 'young_carer', ['young_carer'])
+    add_keys(groups, 'neuro', ['sen', 'neurodivergent'])
+    add_keys(groups, 'birth', ['birth_parent1', 'birth_parent2',
+                               'birth_you', 'birth_you_age'])
+    add_keys(groups, 'sexual_orientation', ['sexual_orientation'])
+
+    # Add groups to the dataframe
+    df['plot_group'] = df['measure'].map(groups)
+    return df
+
+
+def add_standard_demographic_response_labels(df):
+    '''
+    Adds labels for each of the demographic survey questions / data in the
+    standard survey
+
+    Parameters
+    ----------
+    df : dataframe
+        Dataframe containing 'measure' column which we want to add labels to
+    '''
+    # Define labels
+    labels = {
+        'gender': 'Gender',
+        'transgender': 'Do you consider yourself to be transgender?',
+        'sexual_orientation': 'Sexual orientation',
+        'neurodivergent': 'Do you identify as neurodivergent?',
+        'young_carer': '''In the last year, have you regularly taken on caring
+    responsibilities for a family member - e.g. due to illness, disability,
+    mental health condition or drug/alcohol dependency?''',
+        'care_experience': '''Are you or have you ever been in care (living in
+    a foster placement, residential placement, or private/kinship care)?''',
+        'birth_parent1': 'Was birth parent 1 born outside the UK?',
+        'birth_parent2': 'Was birth parent 2 born outside the UK?',
+        'birth_you': 'Were you born outside the UK?',
+        'year_group': 'Year group',
+        'fsm': 'Free school meals',
+        'sen': 'Special educational needs',
+        'ethnicity': 'Ethnicity',
+        'english_additional': 'English as an additional language'}
+
+    # Add labels to the dataframe
+    df['measure_lab'] = df['measure'].map(labels)
+    return df
+
+
+def add_symbol_demographic_response_labels(df):
+    '''
+    Adds labels for each of the demographic survey questions / data in the
+    symbol survey
+
+    Parameters
+    ----------
+    df : dataframe
+        Dataframe containing 'measure' column which we want to add labels to
+    '''
+    # Define labels
+    labels = {
+        'gender': 'Gender',
+        'year_group': 'Year group',
+        'fsm': 'Free school meals',
+        'sen': 'Special educational needs',
+        'ethnicity': 'Ethnicity',
+        'english_additional': 'English as an additional language'}
+
+    # Add labels to the dataframe
+    df['measure_lab'] = df['measure'].map(labels)
+    return df
```

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/synthesise_responses.py` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/synthesise_responses.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,516 +1,516 @@
-'''
-Functions analysing responses to each question - as part of several files
-which provide functions for synthesis (creation and aggregation) of data
-for the dashboard.
-'''
-from collections import defaultdict
-import numpy as np
-from .response_labels import (
-    create_response_label_dict, create_symbol_response_label_dict)
-from .synthesise_aggregate import (
-    aggregate_proportions, results_by_site_and_group)
-
-
-def aggregate_standard_responses(df, site_col):
-    '''
-    Aggregate responses to standard survey (non-demographic), using functions
-    including aggregate_proportions() and results_by_site_and_group().
-
-    Parameters
-    ----------
-    df : dataframe
-        Pupil-level survey responses
-    site_col : string
-        Name of column with site to group by (e.g. 'school_lab', 'site')
-    '''
-    # Make list of columns that we want to count responses for
-    # These are lab columns, but with demographic items removed
-    response_col = [col for col in df.columns if (
-        col.endswith('_lab') and col not in [
-            'school_lab', 'gender_lab', 'transgender_lab',
-            'sexual_orientation_lab', 'neurodivergent_lab',
-            'birth_parent1_lab', 'birth_parent2_lab', 'birth_you_lab',
-            'birth_you_age_lab', 'young_carer_lab', 'care_experience_lab',
-            'year_group_lab', 'fsm_lab', 'sen_lab', 'ethnicity_lab',
-            'english_additional_lab'])]
-
-    # Import dictionary which contains the response options for each question,
-    # for which we want to know the answers to
-    labels = create_response_label_dict()
-
-    # Add 'NaN': 'No response' to each of the dictionaries
-    # They are stored as dictionary of dictionaries, so we loop through and
-    # update each one
-    for key, value in labels.items():
-        value.update({np.nan: 'No response'})
-
-    # Create version where every question has count 0, to use when there is no
-    # pupils of a particular group (ie. no-one in certain FSM/SEN/gender/year)
-    no_pupils = aggregate_proportions(
-        data=df, response_col=response_col, labels=labels)
-    no_pupils[['count', 'percentage', 'n_responses']] = 0
-
-    # Find results of aggregation for each pupil group
-    result = results_by_site_and_group(
-        data=df, agg_func=aggregate_proportions, no_pupils=no_pupils,
-        response_col=response_col, labels=labels, group_type='standard',
-        site_col=site_col)
-
-    # Hide results where n<10
-    result.loc[result['n_responses'] < 10,
-               ['count', 'percentage', 'n_responses']] = np.nan
-
-    return result
-
-
-def aggregate_symbol_responses(df, site_col):
-    '''
-    Aggregate responses to symbol survey (non-demographic), using functions
-    including aggregate_proportions() and results_by_site_and_group().
-
-    Parameters
-    ----------
-    df : dataframe
-        Pupil-level survey responses
-    site_col : string
-        Name of column with site to group by (e.g. 'school_lab', 'site')
-    '''
-    # Make list of columns that we want to count responses for
-    # These are lab columns, but with demographic items removed
-    response_col = [col for col in df.columns if (
-        col.endswith('_lab') and col not in [
-            'gender_lab', 'year_group_lab', 'fsm_lab', 'sen_lab',
-            'ethnicity_lab', 'english_additional_lab', 'school_lab'])]
-
-    # Import dictionary which contains the response options for each question,
-    # for which we want to know the answers to
-    labels = create_symbol_response_label_dict()
-
-    # Add 'NaN': 'No response' to each of the dictionaries
-    # They are stored as dictionary of dictionaries, so we loop through and
-    # update each one
-    for key, value in labels.items():
-        value.update({np.nan: 'No response'})
-
-    # Create version where every question has count 0, to use when a school has
-    # no pupils of a particular subgroup (i.e. no-one in certain
-    # FSM/SEN/gender/year)
-    no_pupils = aggregate_proportions(
-        data=df, response_col=response_col, labels=labels)
-    no_pupils[['count', 'percentage', 'n_responses']] = 0
-
-    # Find results of aggregation for each pupil group
-    result = results_by_site_and_group(
-        data=df, agg_func=aggregate_proportions, no_pupils=no_pupils,
-        response_col=response_col, labels=labels, group_type='symbol',
-        site_col=site_col)
-
-    # Hide results where n<10
-    result.loc[result['n_responses'] < 10,
-               ['count', 'percentage', 'n_responses']] = np.nan
-
-    return result
-
-
-def add_keys(groups, value, keys):
-    '''
-    Add multiple keys with the same value to the dictionary
-
-    Parameters
-    ----------
-    groups: defaultdict
-        Dictionary with measure as key and group as value
-    value : string
-        Value for all the keys
-    keys : array
-        Array with the keys
-    '''
-    groups.update(dict.fromkeys(keys, value))
-
-
-def add_standard_topic_groups(df):
-    '''
-    Adds a 'group' column providing topic group for each item in 'measure',
-    for the standard survey responses
-
-    Parameters
-    ----------
-    df : Dataframe
-        Dataframe containing 'measure' column, which we want to add 'group'
-        column to
-    '''
-    # Initialise dictionary of groups
-    groups = defaultdict(str)
-
-    # Specify group for each measure, adding to the groups dictionary
-    add_keys(groups, 'autonomy', [
-        'autonomy_pressure',
-        'autonomy_express',
-        'autonomy_decide',
-        'autonomy_told',
-        'autonomy_myself',
-        'autonomy_choice'])
-    add_keys(groups, 'life_satisfaction', ['life_satisfaction'])
-    add_keys(groups, 'optimism', [
-        'optimism_future',
-        'optimism_best',
-        'optimism_good',
-        'optimism_work'])
-    add_keys(groups, 'wellbeing', [
-        'wellbeing_optimistic',
-        'wellbeing_useful',
-        'wellbeing_relaxed',
-        'wellbeing_problems',
-        'wellbeing_thinking',
-        'wellbeing_close',
-        'wellbeing_mind'])
-    add_keys(groups, 'esteem', [
-        'esteem_satisfied',
-        'esteem_qualities',
-        'esteem_well',
-        'esteem_value',
-        'esteem_good'])
-    add_keys(groups, 'stress', [
-        'stress_control',
-        'stress_overcome',
-        'stress_confident',
-        'stress_way'])
-    add_keys(groups, 'appearance', ['appearance_happy', 'appearance_feel'])
-    add_keys(groups, 'negative', [
-        'negative_lonely',
-        'negative_unhappy',
-        'negative_like',
-        'negative_cry',
-        'negative_school',
-        'negative_worry',
-        'negative_sleep',
-        'negative_wake',
-        'negative_shy',
-        'negative_scared'])
-    add_keys(groups, 'lonely', ['lonely'])
-    add_keys(groups, 'support', ['support_ways', 'support_look'])
-
-    add_keys(groups, 'sleep', ['sleep'])
-    add_keys(groups, 'physical', ['physical_days', 'physical_hours'])
-    add_keys(groups, 'free_like', ['free_like'])
-    add_keys(groups, 'media', ['media_hours'])
-    add_keys(groups, 'places', [
-        'places_freq',
-        'places_barriers___1',
-        'places_barriers___2',
-        'places_barriers___3',
-        'places_barriers___4',
-        'places_barriers___5',
-        'places_barriers___6',
-        'places_barriers___7',
-        'places_barriers___8',
-        'places_barriers___9'])
-    add_keys(groups, 'school_belong', ['school_belong'])
-    add_keys(groups, 'staff_relationship', [
-        'staff_interest', 'staff_believe', 'staff_best', 'staff_listen'])
-
-    add_keys(groups, 'talk', [
-        'staff_talk', 'staff_talk_listen',
-        'staff_talk_helpful', 'staff_talk_if',
-        'home_talk', 'home_talk_listen', 'home_talk_helpful', 'home_talk_if',
-        'peer_talk', 'peer_talk_listen', 'peer_talk_helpful', 'peer_talk_if'])
-    add_keys(groups, 'accept', [
-        'accept_staff', 'accept_home', 'accept_local', 'accept_peer'])
-
-    add_keys(groups, 'home_relationship', [
-        'home_interest', 'home_believe', 'home_best', 'home_listen'])
-    add_keys(groups, 'home_happy', ['home_happy'])
-
-    add_keys(groups, 'local_env', [
-        'local_safe', 'local_support', 'local_trust', 'local_neighbours',
-        'local_places'])
-    add_keys(groups, 'discrim', [
-        'discrim_race', 'discrim_gender', 'discrim_orientation',
-        'discrim_disability', 'discrim_faith'])
-    add_keys(groups, 'belong_local', ['belong_local'])
-    add_keys(groups, 'wealth', ['wealth'])
-    add_keys(groups, 'future', ['future_options', 'future_interest',
-                                'future_support'])
-    add_keys(groups, 'climate', ['climate'])
-    add_keys(groups, 'social', [
-        'social_along', 'social_time', 'social_support', 'social_hard'])
-    add_keys(groups, 'bully', ['bully_physical', 'bully_other', 'bully_cyber'])
-
-    # Add groups to the dataframe
-    df['group'] = df['measure'].map(groups)
-    return df
-
-
-def add_standard_response_labels(df):
-    '''
-    Adds labels for each of the survey questions (non-demographic) in the
-    standard survey
-
-    Parameters
-    ----------
-    df : dataframe
-        Dataframe containing 'measure' column which we want to add labels to
-    '''
-    # Define labels
-    labels = {
-        'autonomy_pressure': '''
-I feel pressured in my life''',
-        'autonomy_express': '''
-I generally feel free to express my ideas and opinions''',
-        'autonomy_decide': '''
-I feel like I am free to decide for myself how to live my life''',
-        'autonomy_told': '''
-In my daily life I often have to do what I am told''',
-        'autonomy_myself': '''
-I feel I can pretty much be myself in daily situations''',
-        'autonomy_choice': '''
-I have enough choice about how I spend my time''',
-        'life_satisfaction': '''
-Overall, how satisfied are you with your life nowadays?''',
-        'optimism_future': '''
-I am optimistic about my future''',
-        'optimism_best': '''
-In uncertain times, I expect the best''',
-        'optimism_good': '''
-I think good things are going to happen to me''',
-        'optimism_work': '''
-I believe that things will work out, no matter how difficult they seem''',
-        'wellbeing_optimistic': '''
-I've been feeling optimistic about the future''',
-        'wellbeing_useful': '''
-I've been feeling useful''',
-        'wellbeing_relaxed': '''
-I've been feeling relaxed''',
-        'wellbeing_problems': '''
-I've been dealing with problems well''',
-        'wellbeing_thinking': '''
-I've been thinking clearly''',
-        'wellbeing_close': '''
-I've been feeling close to other people''',
-        'wellbeing_mind': '''
-I've been able to make up my own mind about things''',
-        'esteem_satisfied': '''
-On the whole, I am satisfied with myself''',
-        'esteem_qualities': '''
-I feel that I have a number of good qualities''',
-        'esteem_well': '''
-I am able to do things as well as most other people''',
-        'esteem_value': '''
-I am a person of value''',
-        'esteem_good': '''
-I feel good about myself''',
-        'stress_control': '''
-Felt you were unable to control the important things in your life''',
-        'stress_overcome': '''
-Felt that difficulties were piling up so high that you could not overcome
-them''',
-        'stress_confident': '''
-Felt confident about your ability to handle your personal problems''',
-        'stress_way': '''
-Felt that things were going your way''',
-        'appearance_happy': '''
-How happy are you with your appearance (the way that you look)?''',
-        'appearance_feel': '''
-My appearance affects how I feel about myself''',
-        'negative_lonely': '''
-I feel lonely''',
-        'negative_unhappy': '''
-I am unhappy''',
-        'negative_like': '''
-Nobody likes me''',
-        'negative_cry': '''
-I cry a lot''',
-        'negative_school': '''
-I worry when I am at school''',
-        'negative_worry': '''
-I worry a lot''',
-        'negative_sleep': '''
-I have problems sleeping''',
-        'negative_wake': '''
-I wake up in the night''',
-        'negative_shy': '''
-I am shy''',
-        'negative_scared': '''
-I feel scared''',
-        'lonely': '''
-How often do you feel lonely?''',
-        'support_ways': '''
-I have ways to support myself (e.g. to cope, or help myself feel better)''',
-        'support_look': '''
-I know where to look for advice on how to support myself''',
-        'sleep': '''
-Is the amount of sleep you normally get enough for you to feel awake and
-concentrate on your school work during the day?''',
-        'physical_days': '''
-How many days in a usual week are you physically active?''',
-        'physical_hours': '''
-How long on average do you spend being physically active?''',
-        'free_like': '''
-How often can you do things that you like in your free time?''',
-        'media_hours': '''
-On a normal weekday during term time, how much time do you spend on social
-media?''',
-        'places_freq': '''
-How many activities/places are there in your local area, that you choose to or
-would want to go to in your free time?''',
-        'places_barriers___1': '''
-There's nothing to do''',
-        'places_barriers___2': '''
-I'm unable to get there and back''',
-        'places_barriers___3': '''
-It's too expensive (to get there or take part)''',
-        'places_barriers___4': '''
-Poor weather''',
-        'places_barriers___5': '''
-I have no-one to go with''',
-        'places_barriers___6': '''
-It's too busy''',
-        'places_barriers___7': '''
-I feel uncomfortable/anxious about other people who might be there''',
-        'places_barriers___8': '''
-My parents/carers don't allow me to go''',
-        'places_barriers___9': '''
-Other''',
-        'school_belong': '''
-I feel that I belong/belonged at my school''',
-        'staff_interest': '''
-At school there is an adult who... is interested in my schoolwork''',
-        'staff_believe': '''
-At school there is an adult who... believes that I will be a success''',
-        'staff_best': '''
-At school there is an adult who... wants me to do my best''',
-        'staff_listen': '''
-At school there is an adult who... listens to me when I have something to
-say''',
-        'staff_talk': '''
-Talked about feeling down with... an adult at school''',
-        'staff_talk_listen': '''
-Did you feel listened to when you spoke with... an adult at school''',
-        'staff_talk_helpful': '''
-Did you receive advice that you found helpful from... an adult at school''',
-        'staff_talk_if': '''
-How would you feel about speaking with... an adult at school''',
-        'accept_staff': '''
-Adults at your school''',
-        'home_interest': '''
-At home there is an adult who... is interested in my schoolwork''',
-        'home_believe': '''
-At home there is an adult who... believes that I will be a success''',
-        'home_best': '''
-At home there is an adult who... wants me to do my best''',
-        'home_listen': '''
-At home there is an adult who... listens to me when I have something to say''',
-        'home_talk': '''
-Talked about feeling down with... one of your parents/carers''',
-        'home_talk_listen': '''
-Did you feel listened to when you spoke with... one of your parents/carers''',
-        'home_talk_helpful': '''
-Did you receive advice that you found helpful from... one of your
-parents/carers''',
-        'home_talk_if': '''
-How would you feel about speaking with... one of your parents/carers''',
-        'accept_home': '''
-Your parents/carers''',
-        'home_happy': '''
-How happy are you with the home that you live in?''',
-        'local_safe': '''
-How safe do you feel when in your local area?''',
-        'local_support': '''
-People around here support each other with their wellbeing''',
-        'local_trust': '''
-You can trust people around here''',
-        'local_neighbours': '''
-I could ask for help or a favour from neighbours''',
-        'local_places': '''
-There are good places to spend your free time (e.g., leisure centres, parks,
-shops)''',
-        'discrim_race': '''
-How often do people make you feel bad because of... your race, skin colour or
-where you were born?''',
-        'discrim_gender': '''
-How often do people make you feel bad because of... your gender?''',
-        'discrim_orientation': '''
-How often do people make you feel bad because of... your sexual
-orientation?''',
-        'discrim_disability': '''
-How often do people make you feel bad because of... disability?''',
-        'discrim_faith': '''
-How often do people make you feel bad because of... your religion/faith?''',
-        'belong_local': '''
-I feel like I belong in my local area''',
-        'accept_local': '''
-People in your local area''',
-        'wealth': '''
-Compared to your friends, is your family richer, poorer or about the same?''',
-        'future_options': '''
-How many options are available?''',
-        'future_interest': '''
-How do you feel about the options available?''',
-        'future_support': '''
-Do you feel (or think you would feel) supported to explore options that
-interest you, even if no-one else around you has done them before?''',
-        'climate': '''
-How often do you worry about the impact of climate change on your future?''',
-        'social_along': '''
-I get along with people around me''',
-        'social_time': '''
-People like to spend time with me''',
-        'social_support': '''
-I feel supported by my friends''',
-        'social_hard': '''
-My friends care about me when times are hard (for example if I am sick or have
-done something wrong)''',
-        'bully_physical': '''
-How often do you get physically bullied at school? By this we mean getting hit,
-pushed around, threatened, or having belongings stolen.''',
-        'bully_other': '''
-How often do you get bullied in other ways at school? By this we mean insults,
-slurs, name calling, threats, getting left out or excluded by others, or having
-rumours spread about you on purpose.''',
-        'bully_cyber': '''
-How often do you get cyber-bullied? By this we mean someone sending mean text
-or online messages about you, creating a website making fun of you, posting
-pictures that make you look bad online, or sharing them with others.''',
-        'peer_talk': '''
-Talked about feeling down with... another person your age''',
-        'peer_talk_listen': '''
-Did you feel listened to when you spoke with... another person your age''',
-        'peer_talk_helpful': '''
-Did you receive advice that you found helpful from... another person your
-age''',
-        'peer_talk_if': '''
-How would you feel about speaking with... another person your age''',
-        'accept_peer': '''
-Other people your age'''}
-
-    # Add labels to the dataframe
-    df['measure_lab'] = df['measure'].map(labels)
-    return df
-
-
-def add_symbol_response_labels(df):
-    '''
-    Adds labels for each of the survey questions (non-demographic) in the
-    symbol survey
-
-    Parameters
-    ----------
-    df : dataframe
-        Dataframe containing 'measure' column which we want to add labels to
-    '''
-    # Define labels
-    labels = {
-        'symbol_family': 'How do you feel about your family?',
-        'symbol_home': 'How do you feel about your home?',
-        'symbol_friends': 'How do you feel about your friends?',
-        'symbol_choice': (
-            'How do you feel about how much choice you have in life?'),
-        'symbol_things': 'How do you feel about the things that you have?',
-        'symbol_health': 'How do you feel about your health?',
-        'symbol_future': 'How do you feel about your future?',
-        'symbol_school': 'How do you feel about your school?',
-        'symbol_free': 'How do you feel about your free time?',
-        'symbol_life': 'How do you feel about your life?'}
-    # Add labels to the dataframe
-    df['measure_lab'] = df['measure'].map(labels)
-    return df
+'''
+Functions analysing responses to each question - as part of several files
+which provide functions for synthesis (creation and aggregation) of data
+for the dashboard.
+'''
+from collections import defaultdict
+import numpy as np
+from .response_labels import (
+    create_response_label_dict, create_symbol_response_label_dict)
+from .synthesise_aggregate import (
+    aggregate_proportions, results_by_site_and_group)
+
+
+def aggregate_standard_responses(df, site_col):
+    '''
+    Aggregate responses to standard survey (non-demographic), using functions
+    including aggregate_proportions() and results_by_site_and_group().
+
+    Parameters
+    ----------
+    df : dataframe
+        Pupil-level survey responses
+    site_col : string
+        Name of column with site to group by (e.g. 'school_lab', 'site')
+    '''
+    # Make list of columns that we want to count responses for
+    # These are lab columns, but with demographic items removed
+    response_col = [col for col in df.columns if (
+        col.endswith('_lab') and col not in [
+            'school_lab', 'gender_lab', 'transgender_lab',
+            'sexual_orientation_lab', 'neurodivergent_lab',
+            'birth_parent1_lab', 'birth_parent2_lab', 'birth_you_lab',
+            'birth_you_age_lab', 'young_carer_lab', 'care_experience_lab',
+            'year_group_lab', 'fsm_lab', 'sen_lab', 'ethnicity_lab',
+            'english_additional_lab'])]
+
+    # Import dictionary which contains the response options for each question,
+    # for which we want to know the answers to
+    labels = create_response_label_dict()
+
+    # Add 'NaN': 'No response' to each of the dictionaries
+    # They are stored as dictionary of dictionaries, so we loop through and
+    # update each one
+    for key, value in labels.items():
+        value.update({np.nan: 'No response'})
+
+    # Create version where every question has count 0, to use when there is no
+    # pupils of a particular group (ie. no-one in certain FSM/SEN/gender/year)
+    no_pupils = aggregate_proportions(
+        data=df, response_col=response_col, labels=labels)
+    no_pupils[['count', 'percentage', 'n_responses']] = 0
+
+    # Find results of aggregation for each pupil group
+    result = results_by_site_and_group(
+        data=df, agg_func=aggregate_proportions, no_pupils=no_pupils,
+        response_col=response_col, labels=labels, group_type='standard',
+        site_col=site_col)
+
+    # Hide results where n<10
+    result.loc[result['n_responses'] < 10,
+               ['count', 'percentage', 'n_responses']] = np.nan
+
+    return result
+
+
+def aggregate_symbol_responses(df, site_col):
+    '''
+    Aggregate responses to symbol survey (non-demographic), using functions
+    including aggregate_proportions() and results_by_site_and_group().
+
+    Parameters
+    ----------
+    df : dataframe
+        Pupil-level survey responses
+    site_col : string
+        Name of column with site to group by (e.g. 'school_lab', 'site')
+    '''
+    # Make list of columns that we want to count responses for
+    # These are lab columns, but with demographic items removed
+    response_col = [col for col in df.columns if (
+        col.endswith('_lab') and col not in [
+            'gender_lab', 'year_group_lab', 'fsm_lab', 'sen_lab',
+            'ethnicity_lab', 'english_additional_lab', 'school_lab'])]
+
+    # Import dictionary which contains the response options for each question,
+    # for which we want to know the answers to
+    labels = create_symbol_response_label_dict()
+
+    # Add 'NaN': 'No response' to each of the dictionaries
+    # They are stored as dictionary of dictionaries, so we loop through and
+    # update each one
+    for key, value in labels.items():
+        value.update({np.nan: 'No response'})
+
+    # Create version where every question has count 0, to use when a school has
+    # no pupils of a particular subgroup (i.e. no-one in certain
+    # FSM/SEN/gender/year)
+    no_pupils = aggregate_proportions(
+        data=df, response_col=response_col, labels=labels)
+    no_pupils[['count', 'percentage', 'n_responses']] = 0
+
+    # Find results of aggregation for each pupil group
+    result = results_by_site_and_group(
+        data=df, agg_func=aggregate_proportions, no_pupils=no_pupils,
+        response_col=response_col, labels=labels, group_type='symbol',
+        site_col=site_col)
+
+    # Hide results where n<10
+    result.loc[result['n_responses'] < 10,
+               ['count', 'percentage', 'n_responses']] = np.nan
+
+    return result
+
+
+def add_keys(groups, value, keys):
+    '''
+    Add multiple keys with the same value to the dictionary
+
+    Parameters
+    ----------
+    groups: defaultdict
+        Dictionary with measure as key and group as value
+    value : string
+        Value for all the keys
+    keys : array
+        Array with the keys
+    '''
+    groups.update(dict.fromkeys(keys, value))
+
+
+def add_standard_topic_groups(df):
+    '''
+    Adds a 'group' column providing topic group for each item in 'measure',
+    for the standard survey responses
+
+    Parameters
+    ----------
+    df : Dataframe
+        Dataframe containing 'measure' column, which we want to add 'group'
+        column to
+    '''
+    # Initialise dictionary of groups
+    groups = defaultdict(str)
+
+    # Specify group for each measure, adding to the groups dictionary
+    add_keys(groups, 'autonomy', [
+        'autonomy_pressure',
+        'autonomy_express',
+        'autonomy_decide',
+        'autonomy_told',
+        'autonomy_myself',
+        'autonomy_choice'])
+    add_keys(groups, 'life_satisfaction', ['life_satisfaction'])
+    add_keys(groups, 'optimism', [
+        'optimism_future',
+        'optimism_best',
+        'optimism_good',
+        'optimism_work'])
+    add_keys(groups, 'wellbeing', [
+        'wellbeing_optimistic',
+        'wellbeing_useful',
+        'wellbeing_relaxed',
+        'wellbeing_problems',
+        'wellbeing_thinking',
+        'wellbeing_close',
+        'wellbeing_mind'])
+    add_keys(groups, 'esteem', [
+        'esteem_satisfied',
+        'esteem_qualities',
+        'esteem_well',
+        'esteem_value',
+        'esteem_good'])
+    add_keys(groups, 'stress', [
+        'stress_control',
+        'stress_overcome',
+        'stress_confident',
+        'stress_way'])
+    add_keys(groups, 'appearance', ['appearance_happy', 'appearance_feel'])
+    add_keys(groups, 'negative', [
+        'negative_lonely',
+        'negative_unhappy',
+        'negative_like',
+        'negative_cry',
+        'negative_school',
+        'negative_worry',
+        'negative_sleep',
+        'negative_wake',
+        'negative_shy',
+        'negative_scared'])
+    add_keys(groups, 'lonely', ['lonely'])
+    add_keys(groups, 'support', ['support_ways', 'support_look'])
+
+    add_keys(groups, 'sleep', ['sleep'])
+    add_keys(groups, 'physical', ['physical_days', 'physical_hours'])
+    add_keys(groups, 'free_like', ['free_like'])
+    add_keys(groups, 'media', ['media_hours'])
+    add_keys(groups, 'places', [
+        'places_freq',
+        'places_barriers___1',
+        'places_barriers___2',
+        'places_barriers___3',
+        'places_barriers___4',
+        'places_barriers___5',
+        'places_barriers___6',
+        'places_barriers___7',
+        'places_barriers___8',
+        'places_barriers___9'])
+    add_keys(groups, 'school_belong', ['school_belong'])
+    add_keys(groups, 'staff_relationship', [
+        'staff_interest', 'staff_believe', 'staff_best', 'staff_listen'])
+
+    add_keys(groups, 'talk', [
+        'staff_talk', 'staff_talk_listen',
+        'staff_talk_helpful', 'staff_talk_if',
+        'home_talk', 'home_talk_listen', 'home_talk_helpful', 'home_talk_if',
+        'peer_talk', 'peer_talk_listen', 'peer_talk_helpful', 'peer_talk_if'])
+    add_keys(groups, 'accept', [
+        'accept_staff', 'accept_home', 'accept_local', 'accept_peer'])
+
+    add_keys(groups, 'home_relationship', [
+        'home_interest', 'home_believe', 'home_best', 'home_listen'])
+    add_keys(groups, 'home_happy', ['home_happy'])
+
+    add_keys(groups, 'local_env', [
+        'local_safe', 'local_support', 'local_trust', 'local_neighbours',
+        'local_places'])
+    add_keys(groups, 'discrim', [
+        'discrim_race', 'discrim_gender', 'discrim_orientation',
+        'discrim_disability', 'discrim_faith'])
+    add_keys(groups, 'belong_local', ['belong_local'])
+    add_keys(groups, 'wealth', ['wealth'])
+    add_keys(groups, 'future', ['future_options', 'future_interest',
+                                'future_support'])
+    add_keys(groups, 'climate', ['climate'])
+    add_keys(groups, 'social', [
+        'social_along', 'social_time', 'social_support', 'social_hard'])
+    add_keys(groups, 'bully', ['bully_physical', 'bully_other', 'bully_cyber'])
+
+    # Add groups to the dataframe
+    df['group'] = df['measure'].map(groups)
+    return df
+
+
+def add_standard_response_labels(df):
+    '''
+    Adds labels for each of the survey questions (non-demographic) in the
+    standard survey
+
+    Parameters
+    ----------
+    df : dataframe
+        Dataframe containing 'measure' column which we want to add labels to
+    '''
+    # Define labels
+    labels = {
+        'autonomy_pressure': '''
+I feel pressured in my life''',
+        'autonomy_express': '''
+I generally feel free to express my ideas and opinions''',
+        'autonomy_decide': '''
+I feel like I am free to decide for myself how to live my life''',
+        'autonomy_told': '''
+In my daily life I often have to do what I am told''',
+        'autonomy_myself': '''
+I feel I can pretty much be myself in daily situations''',
+        'autonomy_choice': '''
+I have enough choice about how I spend my time''',
+        'life_satisfaction': '''
+Overall, how satisfied are you with your life nowadays?''',
+        'optimism_future': '''
+I am optimistic about my future''',
+        'optimism_best': '''
+In uncertain times, I expect the best''',
+        'optimism_good': '''
+I think good things are going to happen to me''',
+        'optimism_work': '''
+I believe that things will work out, no matter how difficult they seem''',
+        'wellbeing_optimistic': '''
+I've been feeling optimistic about the future''',
+        'wellbeing_useful': '''
+I've been feeling useful''',
+        'wellbeing_relaxed': '''
+I've been feeling relaxed''',
+        'wellbeing_problems': '''
+I've been dealing with problems well''',
+        'wellbeing_thinking': '''
+I've been thinking clearly''',
+        'wellbeing_close': '''
+I've been feeling close to other people''',
+        'wellbeing_mind': '''
+I've been able to make up my own mind about things''',
+        'esteem_satisfied': '''
+On the whole, I am satisfied with myself''',
+        'esteem_qualities': '''
+I feel that I have a number of good qualities''',
+        'esteem_well': '''
+I am able to do things as well as most other people''',
+        'esteem_value': '''
+I am a person of value''',
+        'esteem_good': '''
+I feel good about myself''',
+        'stress_control': '''
+Felt you were unable to control the important things in your life''',
+        'stress_overcome': '''
+Felt that difficulties were piling up so high that you could not overcome
+them''',
+        'stress_confident': '''
+Felt confident about your ability to handle your personal problems''',
+        'stress_way': '''
+Felt that things were going your way''',
+        'appearance_happy': '''
+How happy are you with your appearance (the way that you look)?''',
+        'appearance_feel': '''
+My appearance affects how I feel about myself''',
+        'negative_lonely': '''
+I feel lonely''',
+        'negative_unhappy': '''
+I am unhappy''',
+        'negative_like': '''
+Nobody likes me''',
+        'negative_cry': '''
+I cry a lot''',
+        'negative_school': '''
+I worry when I am at school''',
+        'negative_worry': '''
+I worry a lot''',
+        'negative_sleep': '''
+I have problems sleeping''',
+        'negative_wake': '''
+I wake up in the night''',
+        'negative_shy': '''
+I am shy''',
+        'negative_scared': '''
+I feel scared''',
+        'lonely': '''
+How often do you feel lonely?''',
+        'support_ways': '''
+I have ways to support myself (e.g. to cope, or help myself feel better)''',
+        'support_look': '''
+I know where to look for advice on how to support myself''',
+        'sleep': '''
+Is the amount of sleep you normally get enough for you to feel awake and
+concentrate on your school work during the day?''',
+        'physical_days': '''
+How many days in a usual week are you physically active?''',
+        'physical_hours': '''
+How long on average do you spend being physically active?''',
+        'free_like': '''
+How often can you do things that you like in your free time?''',
+        'media_hours': '''
+On a normal weekday during term time, how much time do you spend on social
+media?''',
+        'places_freq': '''
+How many activities/places are there in your local area, that you choose to or
+would want to go to in your free time?''',
+        'places_barriers___1': '''
+There's nothing to do''',
+        'places_barriers___2': '''
+I'm unable to get there and back''',
+        'places_barriers___3': '''
+It's too expensive (to get there or take part)''',
+        'places_barriers___4': '''
+Poor weather''',
+        'places_barriers___5': '''
+I have no-one to go with''',
+        'places_barriers___6': '''
+It's too busy''',
+        'places_barriers___7': '''
+I feel uncomfortable/anxious about other people who might be there''',
+        'places_barriers___8': '''
+My parents/carers don't allow me to go''',
+        'places_barriers___9': '''
+Other''',
+        'school_belong': '''
+I feel that I belong/belonged at my school''',
+        'staff_interest': '''
+At school there is an adult who... is interested in my schoolwork''',
+        'staff_believe': '''
+At school there is an adult who... believes that I will be a success''',
+        'staff_best': '''
+At school there is an adult who... wants me to do my best''',
+        'staff_listen': '''
+At school there is an adult who... listens to me when I have something to
+say''',
+        'staff_talk': '''
+Talked about feeling down with... an adult at school''',
+        'staff_talk_listen': '''
+Did you feel listened to when you spoke with... an adult at school''',
+        'staff_talk_helpful': '''
+Did you receive advice that you found helpful from... an adult at school''',
+        'staff_talk_if': '''
+How would you feel about speaking with... an adult at school''',
+        'accept_staff': '''
+Adults at your school''',
+        'home_interest': '''
+At home there is an adult who... is interested in my schoolwork''',
+        'home_believe': '''
+At home there is an adult who... believes that I will be a success''',
+        'home_best': '''
+At home there is an adult who... wants me to do my best''',
+        'home_listen': '''
+At home there is an adult who... listens to me when I have something to say''',
+        'home_talk': '''
+Talked about feeling down with... one of your parents/carers''',
+        'home_talk_listen': '''
+Did you feel listened to when you spoke with... one of your parents/carers''',
+        'home_talk_helpful': '''
+Did you receive advice that you found helpful from... one of your
+parents/carers''',
+        'home_talk_if': '''
+How would you feel about speaking with... one of your parents/carers''',
+        'accept_home': '''
+Your parents/carers''',
+        'home_happy': '''
+How happy are you with the home that you live in?''',
+        'local_safe': '''
+How safe do you feel when in your local area?''',
+        'local_support': '''
+People around here support each other with their wellbeing''',
+        'local_trust': '''
+You can trust people around here''',
+        'local_neighbours': '''
+I could ask for help or a favour from neighbours''',
+        'local_places': '''
+There are good places to spend your free time (e.g., leisure centres, parks,
+shops)''',
+        'discrim_race': '''
+How often do people make you feel bad because of... your race, skin colour or
+where you were born?''',
+        'discrim_gender': '''
+How often do people make you feel bad because of... your gender?''',
+        'discrim_orientation': '''
+How often do people make you feel bad because of... your sexual
+orientation?''',
+        'discrim_disability': '''
+How often do people make you feel bad because of... disability?''',
+        'discrim_faith': '''
+How often do people make you feel bad because of... your religion/faith?''',
+        'belong_local': '''
+I feel like I belong in my local area''',
+        'accept_local': '''
+People in your local area''',
+        'wealth': '''
+Compared to your friends, is your family richer, poorer or about the same?''',
+        'future_options': '''
+How many options are available?''',
+        'future_interest': '''
+How do you feel about the options available?''',
+        'future_support': '''
+Do you feel (or think you would feel) supported to explore options that
+interest you, even if no-one else around you has done them before?''',
+        'climate': '''
+How often do you worry about the impact of climate change on your future?''',
+        'social_along': '''
+I get along with people around me''',
+        'social_time': '''
+People like to spend time with me''',
+        'social_support': '''
+I feel supported by my friends''',
+        'social_hard': '''
+My friends care about me when times are hard (for example if I am sick or have
+done something wrong)''',
+        'bully_physical': '''
+How often do you get physically bullied at school? By this we mean getting hit,
+pushed around, threatened, or having belongings stolen.''',
+        'bully_other': '''
+How often do you get bullied in other ways at school? By this we mean insults,
+slurs, name calling, threats, getting left out or excluded by others, or having
+rumours spread about you on purpose.''',
+        'bully_cyber': '''
+How often do you get cyber-bullied? By this we mean someone sending mean text
+or online messages about you, creating a website making fun of you, posting
+pictures that make you look bad online, or sharing them with others.''',
+        'peer_talk': '''
+Talked about feeling down with... another person your age''',
+        'peer_talk_listen': '''
+Did you feel listened to when you spoke with... another person your age''',
+        'peer_talk_helpful': '''
+Did you receive advice that you found helpful from... another person your
+age''',
+        'peer_talk_if': '''
+How would you feel about speaking with... another person your age''',
+        'accept_peer': '''
+Other people your age'''}
+
+    # Add labels to the dataframe
+    df['measure_lab'] = df['measure'].map(labels)
+    return df
+
+
+def add_symbol_response_labels(df):
+    '''
+    Adds labels for each of the survey questions (non-demographic) in the
+    symbol survey
+
+    Parameters
+    ----------
+    df : dataframe
+        Dataframe containing 'measure' column which we want to add labels to
+    '''
+    # Define labels
+    labels = {
+        'symbol_family': 'How do you feel about your family?',
+        'symbol_home': 'How do you feel about your home?',
+        'symbol_friends': 'How do you feel about your friends?',
+        'symbol_choice': (
+            'How do you feel about how much choice you have in life?'),
+        'symbol_things': 'How do you feel about the things that you have?',
+        'symbol_health': 'How do you feel about your health?',
+        'symbol_future': 'How do you feel about your future?',
+        'symbol_school': 'How do you feel about your school?',
+        'symbol_free': 'How do you feel about your free time?',
+        'symbol_life': 'How do you feel about your life?'}
+    # Add labels to the dataframe
+    df['measure_lab'] = df['measure'].map(labels)
+    return df
```

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/synthesise_scores.py` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/synthesise_scores.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,375 +1,375 @@
-'''
-Functions analysing scores for each topic - as part of several files
-which provide functions for synthesis (creation and aggregation) of data
-for the dashboard.
-'''
-import math
-import numpy as np
-import pandas as pd
-
-
-def sum_score(df):
-    '''
-    Find the sum of the provided columns. If any of the required columns
-    contain, NaN, it will just return NaN as the result
-
-    Parameters
-    ----------
-    df : pandas DataFrame
-        Dataframe just containing the columns you want to sum
-    '''
-    # Convert to numeric, find sum and return
-    return df.sum(axis=1, skipna=False)
-
-
-def reverse_score(scores, min, max):
-    '''
-    Reverse scores in the provided array, based on the known min and max of the
-    scale of the scores. NaN will remain as NaN.
-
-    Parameters
-    ----------
-    scores : array
-        Array with scores to be reversed
-    min : int
-        Minimum possible score
-    max : int
-        Maximum possible score
-
-
-    Returns
-    -------
-    Array with scores reversed
-    '''
-    return [max + min - x for x in scores]
-
-
-def calculate_scores(data):
-    '''
-    Creates scores for each pupil in the provided dataframe, for each of the
-    survey topics. Note, when referring to where scores are "set to positive"
-    or "in a positive direction" or a "negative directioN", this refers to
-    whether the maximum score is a positive or negative outcome.
-
-    Parameters
-    ----------
-    data : pandas dataframe
-        Pupil-level survey responses
-
-    Returns
-    -------
-    data : pandas dataframe
-        Pupil-level survey responses with the addition of topic scores
-    '''
-    # Gender, transgender, sexual orientation, neurodivergence, and yes/no
-    # of whether born in UK are not converted to scores
-
-    # Autonomy
-    # Reverse score on two questions in negative direction
-    data['autonomy_pressure_rev'] = reverse_score(
-        data['autonomy_pressure'], min=1, max=5)
-    data['autonomy_told_rev'] = reverse_score(
-        data['autonomy_told'], min=1, max=5)
-    # Sum questions
-    data['autonomy_score'] = sum_score(
-        data[['autonomy_pressure_rev',
-              'autonomy_express',
-              'autonomy_decide',
-              'autonomy_told_rev',
-              'autonomy_myself',
-              'autonomy_choice']])
-    # Drop the temporary columns created to support score calculation
-    data = data.drop(['autonomy_pressure_rev', 'autonomy_told_rev'], axis=1)
-
-    # Life satisfaction requires no changes
-    data['life_satisfaction_score'] = data['life_satisfaction']
-
-    # Optimism
-    data['optimism_score'] = sum_score(
-        data[['optimism_future', 'optimism_best', 'optimism_good',
-              'optimism_work']])
-
-    # Psychological wellbeing
-    data['wellbeing_score'] = sum_score(
-        data[['wellbeing_optimistic', 'wellbeing_useful', 'wellbeing_relaxed',
-              'wellbeing_problems', 'wellbeing_thinking', 'wellbeing_close',
-              'wellbeing_mind']])
-
-    # Self-esteem requires reversed scoring
-    data['esteem_score'] = sum_score(
-        data[['esteem_satisfied', 'esteem_qualities', 'esteem_well',
-              'esteem_value', 'esteem_good']].apply(
-                lambda x: reverse_score(x, min=1, max=4)))
-
-    # Stress
-    # First, I calculate score as in GM - that was a negative direction, so
-    # we have to change the two positive direction options to the negative
-    data['stress_confident_rev'] = reverse_score(
-        data['stress_confident'], min=1, max=5)
-    data['stress_way_rev'] = reverse_score(data['stress_way'], min=1, max=5)
-    data['stress_score'] = sum_score(
-        data[['stress_control', 'stress_overcome', 'stress_confident_rev',
-              'stress_way_rev']] - 1)
-    # Drop the temporary columns created to support score calculation
-    data = data.drop(['stress_confident_rev', 'stress_way_rev'], axis=1)
-    # We are setting all scores to positive - so reverse the final score
-    data['stress_score'] = reverse_score(data['stress_score'], min=0, max=16)
-
-    # Appearance uses first question, excluding 'prefer not to say'
-    data['appearance_score'] = data['appearance_happy'].replace(11, np.nan)
-
-    # Negative affect requires numbering to start at 0
-    data['negative_score'] = sum_score(
-        data[['negative_lonely', 'negative_unhappy', 'negative_like',
-              'negative_cry', 'negative_school', 'negative_worry',
-              'negative_sleep', 'negative_wake', 'negative_shy',
-              'negative_scared']] - 1)
-    # We are setting all scores to positive - so reverse the final score
-    data['negative_score'] = reverse_score(
-        data['negative_score'], min=0, max=20)
-
-    # Loneliness requires reversed scoring (eg. 1 often or always becomes 5)
-    # to match GM - but we are setting all scores to positive - so leave as is
-    data['lonely_score'] = data['lonely']
-
-    # Supporting your wellbeing - reversed so its in the positive direction
-    data['support_score'] = sum_score(data[['support_ways', 'support_look']])
-    data['support_score'] = reverse_score(data['support_score'], min=2, max=8)
-
-    # Sleep is based on proportion answering 1/Yes so no change required
-    data['sleep_score'] = data['sleep']
-
-    # Physical activity multiplies days by avg time per day (which is in min)
-    data['physical_score'] = data['physical_days']*data['physical_hours']
-
-    # Free time/time use - reversed so its in the positive direction
-    data['free_like_score'] = reverse_score(data['free_like'], min=1, max=5)
-
-    # Use of social media requires scores of 0-8 (rather than 1-9)
-    # Then we reverse it so it's in the positive direction
-    data['media_score'] = data['media_hours'] - 1
-    data['media_score'] = reverse_score(data['media_score'], min=0, max=8)
-
-    # Places to go and things to do (unchanged as that is simplest)
-    data['places_score'] = data['places_freq']
-
-    # Talking with people about feeling down
-    # If answer yes, it is the average of their listen (1-4) and helpful (1-3
-    # but rescaled to 1-4) questions, giving a total of 1-4. If answer no, it
-    # is just their answer to comfortable (1-4). The scores for staff, home and
-    # peer are then summed, creating an overall score of 3-12.
-    for prefix in ['staff', 'home', 'peer']:
-        # Create the help/listen scores (see it takes the average through /2)
-        data[f'{prefix}_talk_listen_helpful'] = (
-            data[f'{prefix}_talk_listen'] +
-            data[f'{prefix}_talk_helpful'].map({1: 1, 2: 2.5, 3: 4})) / 2
-        # Create score column where choosen "help/listen" or "if" depending on
-        # answer to talk
-        data[f'{prefix}_talk_score'] = np.where(
-            data[f'{prefix}_talk'] == 1,
-            data[f'{prefix}_talk_listen_helpful'],
-            data[f'{prefix}_talk_if'])
-    # Create overall score from sum of staff, home and peer scores
-    data['talk_score'] = (data['staff_talk_score'] +
-                          data['home_talk_score'] +
-                          data['peer_talk_score'])
-    # Drop columns that were used to calculate scores
-    data = data.drop(['staff_talk_listen_helpful',
-                      'home_talk_listen_helpful',
-                      'peer_talk_listen_helpful'], axis=1)
-
-    # Acceptance
-    data['accept_score'] = sum_score(
-        data[['accept_staff', 'accept_home', 'accept_local', 'accept_peer']])
-
-    # School connection
-    data['school_belong_score'] = data['school_belong']
-
-    # Relationships with staff
-    data['staff_relationship_score'] = sum_score(
-        data[['staff_interest', 'staff_believe',
-              'staff_best', 'staff_listen']])
-
-    # Relationship with parents/carers
-    data['home_relationship_score'] = sum_score(
-        data[['home_interest', 'home_believe', 'home_best', 'home_listen']])
-
-    # Home environment
-    data['home_happy_score'] = data['home_happy']
-
-    # Caring responsibilities and care experience aren't converted to scores
-
-    # Local environment
-    # First question has four responses and one "don't know" (which convert to
-    # np.nan). We rescale to range from 1 to 5 to match remaining questions
-    # which have 1,2,3,4,5 as responses
-    data['local_safe_rescaled'] = data['local_safe'].map({
-        1: 1,
-        2: 2 + 1/3,
-        3: 3 + 2/3,
-        4: 5,
-        5: np.nan})
-    data['local_env_score'] = sum_score(
-        data[['local_safe_rescaled', 'local_support', 'local_trust',
-              'local_neighbours', 'local_places']])
-    data = data.drop('local_safe_rescaled', axis=1)
-    # We then reverse the score so it is in the positive direction
-    data['local_env_score'] = reverse_score(
-        data['local_env_score'], min=5, max=25)
-
-    # Discrimination
-    # Proportion who respond often or always / some of the time / occassionally
-    # to any of the five questions. They're not required to have responded to
-    # all five, just need to have given one of those responses to at least one
-    # of those questions.
-    # Identify relevant columns
-    discrim_col = ['discrim_race', 'discrim_gender', 'discrim_orientation',
-                   'discrim_disability', 'discrim_faith']
-    # Find if any of them are one of those responses
-    # If true, set to 1. If false, set to 2. This is because true is the
-    # negative outcome whilst false is the positive outcome (so set to higher
-    # score). We use 1 and 2 rather than 0 and 1 as often the score for a
-    # school will fall fairly low in the synthetic data, and when 0 is the
-    # minimum, the minimum bar doesn't show on the plot and there's no x axis
-    # ticks to explain
-    data['discrim_score'] = (
-        data[discrim_col].isin([1, 2, 3]).any(axis=1).map({True: 1, False: 2}))
-    # Set to NaN if all responses were NaN
-    data.loc[data[discrim_col].isnull().all(axis=1), 'discrim_score'] = np.nan
-
-    # Belonging - reverse so its in the positive direction
-    data['belong_local_score'] = reverse_score(
-        data['belong_local'], min=1, max=4)
-
-    # Relative wealth
-    # Proportion who feel about the same as friends, excluding "don't know"
-    data['wealth_score'] = data['wealth'].map({1: 0, 2: 0, 3: 1, 4: np.nan})
-
-    # Work, education and training opportunities
-    # Rescale future options so 1-5 (matching future interest and support)
-    # For all, setting the "unsure" option to np.nan
-    data['future_score'] = (
-        data['future_options'].map({
-            1: 1,
-            2: 2.5,
-            3: 4,
-            4: np.nan}) +
-        data['future_interest'].replace(5, np.nan) +
-        data['future_support'].replace(5, np.nan)
-    )
-
-    # Climate change
-    data['climate_score'] = data['climate']
-
-    # Friendships and social support
-    data['social_score'] = sum_score(data[['social_along', 'social_time',
-                                           'social_support', 'social_hard']])
-
-    # Bullying
-    data['bully_score'] = sum_score(data[['bully_physical', 'bully_other',
-                                          'bully_cyber']])
-    # Reverse so it's in the positive direction
-    data['bully_score'] = reverse_score(data['bully_score'], min=3, max=12)
-
-    return (data)
-
-
-def score_descriptives(values, counts):
-    '''
-    This function uses site-level data. Using the mean and count from each
-    group, it calculates the weighted mean and weighted standard deviation
-    of scores across the groups. It returns this, alongside a count of the
-    pupils and groups included.
-
-    Additional information about weighted standard deviation:
-    This normalises weights so they sum 1 (and so they can't all be 0).
-    It returns the biased variance and is like a weighted version of np.std().
-    For small samples, may want to alter to unbiased variance.
-    Based on: https://stackoverflow.com/questions/2413522/weighted-standard-
-    deviation-in-numpy
-
-    Parameters
-    ----------
-    values : pandas series
-        Dataframe column with the mean scores in each group, NaN removed
-    counts: pandas series
-        Dataframe column with the count of pupils in each group, NaN removed
-
-    Returns
-    -------
-    result : pandas Series
-        Series with each of the calculations, where index if the name of the
-        calculation
-    '''
-    # Check for NaN
-    if values.isnull().any():
-        raise ValueError('There must be no NaN in the values column.')
-    if counts.isnull().any():
-        raise ValueError('There must be no NaN in the counts column.')
-
-    # Weighted mean
-    average = np.average(values, weights=counts)
-    # Weighted std
-    variance = np.average((values-average)**2, weights=counts)
-    std = math.sqrt(variance)
-
-    # Total sample size
-    n_pupils = counts.sum(skipna=True)
-    # Total number of groups
-    n_groups = counts.count()
-
-    # Combine into a series
-    result = pd.Series(
-        [n_pupils, n_groups, average, std],
-        index=['total_pupils', 'group_n', 'group_wt_mean', 'group_wt_std'])
-    return result
-
-
-def create_rag_ratings(df):
-    '''
-    Generate rag ratings (above, average, below) based on scores
-
-    Parameters
-    ----------
-    df : dataframe
-        Contains scores by site, and potentially by pupil group too
-
-    Result:
-    -------
-    rag : dataframe
-        Dataframe with scores by site, with additional columns providing RAG
-        ratings and descriptives of the score distribution that were used to
-        generate the RAG
-    '''
-    # Get name of grouping columns (assumes only columns in the dataframe
-    # are those with mean and count, the site (msoa or school), and then that
-    # all other columns are what scores are grouped by) - i.e. just 'variable'
-    # for area maps, or 'variable' plus the demographic columns
-    score_groups = [e for e in list(df.columns) if e not in [
-        'mean', 'count', 'msoa', 'school_lab']]
-
-    # Filter to non-nan rows (as other rows can't/won't be used in calculation)
-    non_nan = df[~(df['mean'].isnull()) & ~(df['count'].isnull())]
-
-    # Groupby variable and return number of sites, weighted mean + SD
-    wt_mean = (non_nan
-               .groupby(score_groups)
-               .apply(lambda x: score_descriptives(x['mean'], x['count']))
-               .reset_index())
-
-    # Add the record of the weighted mean and SD back to the site-level results
-    rag = pd.merge(df, wt_mean, how='left', on=score_groups)
-
-    # Find 1 SD above and below mean
-    rag['lower'] = rag['group_wt_mean'] - rag['group_wt_std']
-    rag['upper'] = rag['group_wt_mean'] + rag['group_wt_std']
-
-    # Create RAG column based on whether scores were past lower lower and
-    # upper boundaries we generated
-    conditions = [(rag['mean'] <= rag['lower']),
-                  (rag['mean'] > rag['lower']) & (rag['mean'] < rag['upper']),
-                  (rag['mean'] >= rag['upper'])]
-    choices = ['below', 'average', 'above']
-    rag.loc[:, 'rag'] = np.select(conditions, choices, default=np.nan)
-
-    return rag
+'''
+Functions analysing scores for each topic - as part of several files
+which provide functions for synthesis (creation and aggregation) of data
+for the dashboard.
+'''
+import math
+import numpy as np
+import pandas as pd
+
+
+def sum_score(df):
+    '''
+    Find the sum of the provided columns. If any of the required columns
+    contain, NaN, it will just return NaN as the result
+
+    Parameters
+    ----------
+    df : pandas DataFrame
+        Dataframe just containing the columns you want to sum
+    '''
+    # Convert to numeric, find sum and return
+    return df.sum(axis=1, skipna=False)
+
+
+def reverse_score(scores, min, max):
+    '''
+    Reverse scores in the provided array, based on the known min and max of the
+    scale of the scores. NaN will remain as NaN.
+
+    Parameters
+    ----------
+    scores : array
+        Array with scores to be reversed
+    min : int
+        Minimum possible score
+    max : int
+        Maximum possible score
+
+
+    Returns
+    -------
+    Array with scores reversed
+    '''
+    return [max + min - x for x in scores]
+
+
+def calculate_scores(data):
+    '''
+    Creates scores for each pupil in the provided dataframe, for each of the
+    survey topics. Note, when referring to where scores are "set to positive"
+    or "in a positive direction" or a "negative directioN", this refers to
+    whether the maximum score is a positive or negative outcome.
+
+    Parameters
+    ----------
+    data : pandas dataframe
+        Pupil-level survey responses
+
+    Returns
+    -------
+    data : pandas dataframe
+        Pupil-level survey responses with the addition of topic scores
+    '''
+    # Gender, transgender, sexual orientation, neurodivergence, and yes/no
+    # of whether born in UK are not converted to scores
+
+    # Autonomy
+    # Reverse score on two questions in negative direction
+    data['autonomy_pressure_rev'] = reverse_score(
+        data['autonomy_pressure'], min=1, max=5)
+    data['autonomy_told_rev'] = reverse_score(
+        data['autonomy_told'], min=1, max=5)
+    # Sum questions
+    data['autonomy_score'] = sum_score(
+        data[['autonomy_pressure_rev',
+              'autonomy_express',
+              'autonomy_decide',
+              'autonomy_told_rev',
+              'autonomy_myself',
+              'autonomy_choice']])
+    # Drop the temporary columns created to support score calculation
+    data = data.drop(['autonomy_pressure_rev', 'autonomy_told_rev'], axis=1)
+
+    # Life satisfaction requires no changes
+    data['life_satisfaction_score'] = data['life_satisfaction']
+
+    # Optimism
+    data['optimism_score'] = sum_score(
+        data[['optimism_future', 'optimism_best', 'optimism_good',
+              'optimism_work']])
+
+    # Psychological wellbeing
+    data['wellbeing_score'] = sum_score(
+        data[['wellbeing_optimistic', 'wellbeing_useful', 'wellbeing_relaxed',
+              'wellbeing_problems', 'wellbeing_thinking', 'wellbeing_close',
+              'wellbeing_mind']])
+
+    # Self-esteem requires reversed scoring
+    data['esteem_score'] = sum_score(
+        data[['esteem_satisfied', 'esteem_qualities', 'esteem_well',
+              'esteem_value', 'esteem_good']].apply(
+                lambda x: reverse_score(x, min=1, max=4)))
+
+    # Stress
+    # First, I calculate score as in GM - that was a negative direction, so
+    # we have to change the two positive direction options to the negative
+    data['stress_confident_rev'] = reverse_score(
+        data['stress_confident'], min=1, max=5)
+    data['stress_way_rev'] = reverse_score(data['stress_way'], min=1, max=5)
+    data['stress_score'] = sum_score(
+        data[['stress_control', 'stress_overcome', 'stress_confident_rev',
+              'stress_way_rev']] - 1)
+    # Drop the temporary columns created to support score calculation
+    data = data.drop(['stress_confident_rev', 'stress_way_rev'], axis=1)
+    # We are setting all scores to positive - so reverse the final score
+    data['stress_score'] = reverse_score(data['stress_score'], min=0, max=16)
+
+    # Appearance uses first question, excluding 'prefer not to say'
+    data['appearance_score'] = data['appearance_happy'].replace(11, np.nan)
+
+    # Negative affect requires numbering to start at 0
+    data['negative_score'] = sum_score(
+        data[['negative_lonely', 'negative_unhappy', 'negative_like',
+              'negative_cry', 'negative_school', 'negative_worry',
+              'negative_sleep', 'negative_wake', 'negative_shy',
+              'negative_scared']] - 1)
+    # We are setting all scores to positive - so reverse the final score
+    data['negative_score'] = reverse_score(
+        data['negative_score'], min=0, max=20)
+
+    # Loneliness requires reversed scoring (eg. 1 often or always becomes 5)
+    # to match GM - but we are setting all scores to positive - so leave as is
+    data['lonely_score'] = data['lonely']
+
+    # Supporting your wellbeing - reversed so its in the positive direction
+    data['support_score'] = sum_score(data[['support_ways', 'support_look']])
+    data['support_score'] = reverse_score(data['support_score'], min=2, max=8)
+
+    # Sleep is based on proportion answering 1/Yes so no change required
+    data['sleep_score'] = data['sleep']
+
+    # Physical activity multiplies days by avg time per day (which is in min)
+    data['physical_score'] = data['physical_days']*data['physical_hours']
+
+    # Free time/time use - reversed so its in the positive direction
+    data['free_like_score'] = reverse_score(data['free_like'], min=1, max=5)
+
+    # Use of social media requires scores of 0-8 (rather than 1-9)
+    # Then we reverse it so it's in the positive direction
+    data['media_score'] = data['media_hours'] - 1
+    data['media_score'] = reverse_score(data['media_score'], min=0, max=8)
+
+    # Places to go and things to do (unchanged as that is simplest)
+    data['places_score'] = data['places_freq']
+
+    # Talking with people about feeling down
+    # If answer yes, it is the average of their listen (1-4) and helpful (1-3
+    # but rescaled to 1-4) questions, giving a total of 1-4. If answer no, it
+    # is just their answer to comfortable (1-4). The scores for staff, home and
+    # peer are then summed, creating an overall score of 3-12.
+    for prefix in ['staff', 'home', 'peer']:
+        # Create the help/listen scores (see it takes the average through /2)
+        data[f'{prefix}_talk_listen_helpful'] = (
+            data[f'{prefix}_talk_listen'] +
+            data[f'{prefix}_talk_helpful'].map({1: 1, 2: 2.5, 3: 4})) / 2
+        # Create score column where choosen "help/listen" or "if" depending on
+        # answer to talk
+        data[f'{prefix}_talk_score'] = np.where(
+            data[f'{prefix}_talk'] == 1,
+            data[f'{prefix}_talk_listen_helpful'],
+            data[f'{prefix}_talk_if'])
+    # Create overall score from sum of staff, home and peer scores
+    data['talk_score'] = (data['staff_talk_score'] +
+                          data['home_talk_score'] +
+                          data['peer_talk_score'])
+    # Drop columns that were used to calculate scores
+    data = data.drop(['staff_talk_listen_helpful',
+                      'home_talk_listen_helpful',
+                      'peer_talk_listen_helpful'], axis=1)
+
+    # Acceptance
+    data['accept_score'] = sum_score(
+        data[['accept_staff', 'accept_home', 'accept_local', 'accept_peer']])
+
+    # School connection
+    data['school_belong_score'] = data['school_belong']
+
+    # Relationships with staff
+    data['staff_relationship_score'] = sum_score(
+        data[['staff_interest', 'staff_believe',
+              'staff_best', 'staff_listen']])
+
+    # Relationship with parents/carers
+    data['home_relationship_score'] = sum_score(
+        data[['home_interest', 'home_believe', 'home_best', 'home_listen']])
+
+    # Home environment
+    data['home_happy_score'] = data['home_happy']
+
+    # Caring responsibilities and care experience aren't converted to scores
+
+    # Local environment
+    # First question has four responses and one "don't know" (which convert to
+    # np.nan). We rescale to range from 1 to 5 to match remaining questions
+    # which have 1,2,3,4,5 as responses
+    data['local_safe_rescaled'] = data['local_safe'].map({
+        1: 1,
+        2: 2 + 1/3,
+        3: 3 + 2/3,
+        4: 5,
+        5: np.nan})
+    data['local_env_score'] = sum_score(
+        data[['local_safe_rescaled', 'local_support', 'local_trust',
+              'local_neighbours', 'local_places']])
+    data = data.drop('local_safe_rescaled', axis=1)
+    # We then reverse the score so it is in the positive direction
+    data['local_env_score'] = reverse_score(
+        data['local_env_score'], min=5, max=25)
+
+    # Discrimination
+    # Proportion who respond often or always / some of the time / occassionally
+    # to any of the five questions. They're not required to have responded to
+    # all five, just need to have given one of those responses to at least one
+    # of those questions.
+    # Identify relevant columns
+    discrim_col = ['discrim_race', 'discrim_gender', 'discrim_orientation',
+                   'discrim_disability', 'discrim_faith']
+    # Find if any of them are one of those responses
+    # If true, set to 1. If false, set to 2. This is because true is the
+    # negative outcome whilst false is the positive outcome (so set to higher
+    # score). We use 1 and 2 rather than 0 and 1 as often the score for a
+    # school will fall fairly low in the synthetic data, and when 0 is the
+    # minimum, the minimum bar doesn't show on the plot and there's no x axis
+    # ticks to explain
+    data['discrim_score'] = (
+        data[discrim_col].isin([1, 2, 3]).any(axis=1).map({True: 1, False: 2}))
+    # Set to NaN if all responses were NaN
+    data.loc[data[discrim_col].isnull().all(axis=1), 'discrim_score'] = np.nan
+
+    # Belonging - reverse so its in the positive direction
+    data['belong_local_score'] = reverse_score(
+        data['belong_local'], min=1, max=4)
+
+    # Relative wealth
+    # Proportion who feel about the same as friends, excluding "don't know"
+    data['wealth_score'] = data['wealth'].map({1: 0, 2: 0, 3: 1, 4: np.nan})
+
+    # Work, education and training opportunities
+    # Rescale future options so 1-5 (matching future interest and support)
+    # For all, setting the "unsure" option to np.nan
+    data['future_score'] = (
+        data['future_options'].map({
+            1: 1,
+            2: 2.5,
+            3: 4,
+            4: np.nan}) +
+        data['future_interest'].replace(5, np.nan) +
+        data['future_support'].replace(5, np.nan)
+    )
+
+    # Climate change
+    data['climate_score'] = data['climate']
+
+    # Friendships and social support
+    data['social_score'] = sum_score(data[['social_along', 'social_time',
+                                           'social_support', 'social_hard']])
+
+    # Bullying
+    data['bully_score'] = sum_score(data[['bully_physical', 'bully_other',
+                                          'bully_cyber']])
+    # Reverse so it's in the positive direction
+    data['bully_score'] = reverse_score(data['bully_score'], min=3, max=12)
+
+    return (data)
+
+
+def score_descriptives(values, counts):
+    '''
+    This function uses site-level data. Using the mean and count from each
+    group, it calculates the weighted mean and weighted standard deviation
+    of scores across the groups. It returns this, alongside a count of the
+    pupils and groups included.
+
+    Additional information about weighted standard deviation:
+    This normalises weights so they sum 1 (and so they can't all be 0).
+    It returns the biased variance and is like a weighted version of np.std().
+    For small samples, may want to alter to unbiased variance.
+    Based on: https://stackoverflow.com/questions/2413522/weighted-standard-
+    deviation-in-numpy
+
+    Parameters
+    ----------
+    values : pandas series
+        Dataframe column with the mean scores in each group, NaN removed
+    counts: pandas series
+        Dataframe column with the count of pupils in each group, NaN removed
+
+    Returns
+    -------
+    result : pandas Series
+        Series with each of the calculations, where index if the name of the
+        calculation
+    '''
+    # Check for NaN
+    if values.isnull().any():
+        raise ValueError('There must be no NaN in the values column.')
+    if counts.isnull().any():
+        raise ValueError('There must be no NaN in the counts column.')
+
+    # Weighted mean
+    average = np.average(values, weights=counts)
+    # Weighted std
+    variance = np.average((values-average)**2, weights=counts)
+    std = math.sqrt(variance)
+
+    # Total sample size
+    n_pupils = counts.sum(skipna=True)
+    # Total number of groups
+    n_groups = counts.count()
+
+    # Combine into a series
+    result = pd.Series(
+        [n_pupils, n_groups, average, std],
+        index=['total_pupils', 'group_n', 'group_wt_mean', 'group_wt_std'])
+    return result
+
+
+def create_rag_ratings(df):
+    '''
+    Generate rag ratings (above, average, below) based on scores
+
+    Parameters
+    ----------
+    df : dataframe
+        Contains scores by site, and potentially by pupil group too
+
+    Result:
+    -------
+    rag : dataframe
+        Dataframe with scores by site, with additional columns providing RAG
+        ratings and descriptives of the score distribution that were used to
+        generate the RAG
+    '''
+    # Get name of grouping columns (assumes only columns in the dataframe
+    # are those with mean and count, the site (msoa or school), and then that
+    # all other columns are what scores are grouped by) - i.e. just 'variable'
+    # for area maps, or 'variable' plus the demographic columns
+    score_groups = [e for e in list(df.columns) if e not in [
+        'mean', 'count', 'msoa', 'school_lab']]
+
+    # Filter to non-nan rows (as other rows can't/won't be used in calculation)
+    non_nan = df[~(df['mean'].isnull()) & ~(df['count'].isnull())]
+
+    # Groupby variable and return number of sites, weighted mean + SD
+    wt_mean = (non_nan
+               .groupby(score_groups)
+               .apply(lambda x: score_descriptives(x['mean'], x['count']))
+               .reset_index())
+
+    # Add the record of the weighted mean and SD back to the site-level results
+    rag = pd.merge(df, wt_mean, how='left', on=score_groups)
+
+    # Find 1 SD above and below mean
+    rag['lower'] = rag['group_wt_mean'] - rag['group_wt_std']
+    rag['upper'] = rag['group_wt_mean'] + rag['group_wt_std']
+
+    # Create RAG column based on whether scores were past lower lower and
+    # upper boundaries we generated
+    conditions = [(rag['mean'] <= rag['lower']),
+                  (rag['mean'] > rag['lower']) & (rag['mean'] < rag['upper']),
+                  (rag['mean'] >= rag['upper'])]
+    choices = ['below', 'average', 'above']
+    rag.loc[:, 'rag'] = np.select(conditions, choices, default=np.nan)
+
+    return rag
```

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/topic_labels.py` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/topic_labels.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,101 +1,101 @@
-'''
-Dictionaries with names and descriptions used for each of the survey topics
-'''
-
-topic_name_dict = {
-    'autonomy_score': 'Autonomy',
-    'life_satisfaction_score': 'Life satisfaction',
-    'optimism_score': 'Optimism',
-    'wellbeing_score': 'Psychological wellbeing',
-    'esteem_score': 'Self-esteem',
-    'stress_score': 'Stress and coping',
-    'appearance_score': 'Feelings around appearance',
-    'negative_score': 'Negative affect',
-    'lonely_score': 'Loneliness',
-    'support_score': 'Supporting own wellbeing',
-    'sleep_score': 'Sleep',
-    'physical_score': 'Physical activity',
-    'free_like_score': 'Free time',
-    'media_score': 'Social media use',
-    'places_score': 'Places to go and things to do',
-    'talk_score': 'Talking about feelings',
-    'accept_score': 'Acceptance',
-    'school_belong_score': 'School connection',
-    'staff_relationship_score': 'Support from staff',
-    'home_relationship_score': 'Support from parents/carers',
-    'home_happy_score': 'Home environment',
-    'local_env_score': 'Local environment',
-    'discrim_score': 'Discrimination',
-    'belong_local_score': 'Local connection',
-    'wealth_score': 'Relative wealth',
-    'future_score': 'Future opportunities',
-    'climate_score': 'Climate change',
-    'social_score': 'Support from friends',
-    'bully_score': 'Bullying'
-}
-
-topic_description_dict = {
-    'autonomy_score': '''
-How 'in control' young people feel of their life''',
-    'life_satisfaction_score': '''
-How satisfied young people feel with their life''',
-    'optimism_score': '''
-Young people's hopefulness and confidence for the future''',
-    'wellbeing_score': '''
-How positive and generally happy young people feel regarding their life''',
-    'esteem_score': '''
-How much young people value themselves''',
-    'stress_score': '''
-Managing stress levels and coping with difficulties''',
-    'appearance_score': '''
-Young people's feelings around the way that they look''',
-    'negative_score': '''
-The frequency with which young people experience emotional difficulties''',
-    'lonely_score': '''
-How often young people feel lonely''',
-    'support_score': '''
-Young people's knowledge on supporting themselves and looking for advice''',
-    'sleep_score': '''
-How much sleep young people get''',
-    'physical_score': '''
-How physically active young people are''',
-    'free_like_score': '''
-How often young people can do things that they like in their free time''',
-    'media_score': '''
-How much time young people spend on social media''',
-    'places_score': '''
-Whether young people feel there are places to go and things to do in their
-free time''',
-    'talk_score': '''
-How positively/negatively young people feel about talking with others about
-feeling down''',
-    'accept_score': '''
-Whether young people feel accepted by different groups of people in their
-life''',
-    'school_belong_score': '''
-Feelings of belonging at school''',
-    'staff_relationship_score': '''
-The support received from adults at school''',
-    'home_relationship_score': '''
-The support received from adults at home''',
-    'home_happy_score': '''
-Young people's feelings regarding the home that they live in''',
-    'local_env_score': '''
-How young people feel regarding the area where they live''',
-    'discrim_score': '''
-Whether young people feel discriminated against''',
-    'belong_local_score': '''
-Young people's feelings of belonging in their local area''',
-    'wealth_score': '''
-Whether young people feel their family is richer, poorer or the same as their
-friends''',
-    'future_score': '''
-How young people feel regarding the future options for work, education or
-training in their local area''',
-    'climate_score': '''
-Worries regarding climate change''',
-    'social_score': '''
-The support young people receive from their peers''',
-    'bully_score': '''
-The frequency with which young people experience different types of bullying'''
-}
+'''
+Dictionaries with names and descriptions used for each of the survey topics
+'''
+
+topic_name_dict = {
+    'autonomy_score': 'Autonomy',
+    'life_satisfaction_score': 'Life satisfaction',
+    'optimism_score': 'Optimism',
+    'wellbeing_score': 'Psychological wellbeing',
+    'esteem_score': 'Self-esteem',
+    'stress_score': 'Stress and coping',
+    'appearance_score': 'Feelings around appearance',
+    'negative_score': 'Negative affect',
+    'lonely_score': 'Loneliness',
+    'support_score': 'Supporting own wellbeing',
+    'sleep_score': 'Sleep',
+    'physical_score': 'Physical activity',
+    'free_like_score': 'Free time',
+    'media_score': 'Social media use',
+    'places_score': 'Places to go and things to do',
+    'talk_score': 'Talking about feelings',
+    'accept_score': 'Acceptance',
+    'school_belong_score': 'School connection',
+    'staff_relationship_score': 'Support from staff',
+    'home_relationship_score': 'Support from parents/carers',
+    'home_happy_score': 'Home environment',
+    'local_env_score': 'Local environment',
+    'discrim_score': 'Discrimination',
+    'belong_local_score': 'Local connection',
+    'wealth_score': 'Relative wealth',
+    'future_score': 'Future opportunities',
+    'climate_score': 'Climate change',
+    'social_score': 'Support from friends',
+    'bully_score': 'Bullying'
+}
+
+topic_description_dict = {
+    'autonomy_score': '''
+How 'in control' young people feel of their life''',
+    'life_satisfaction_score': '''
+How satisfied young people feel with their life''',
+    'optimism_score': '''
+Young people's hopefulness and confidence for the future''',
+    'wellbeing_score': '''
+How positive and generally happy young people feel regarding their life''',
+    'esteem_score': '''
+How much young people value themselves''',
+    'stress_score': '''
+Managing stress levels and coping with difficulties''',
+    'appearance_score': '''
+Young people's feelings around the way that they look''',
+    'negative_score': '''
+The frequency with which young people experience emotional difficulties''',
+    'lonely_score': '''
+How often young people feel lonely''',
+    'support_score': '''
+Young people's knowledge on supporting themselves and looking for advice''',
+    'sleep_score': '''
+How much sleep young people get''',
+    'physical_score': '''
+How physically active young people are''',
+    'free_like_score': '''
+How often young people can do things that they like in their free time''',
+    'media_score': '''
+How much time young people spend on social media''',
+    'places_score': '''
+Whether young people feel there are places to go and things to do in their
+free time''',
+    'talk_score': '''
+How positively/negatively young people feel about talking with others about
+feeling down''',
+    'accept_score': '''
+Whether young people feel accepted by different groups of people in their
+life''',
+    'school_belong_score': '''
+Feelings of belonging at school''',
+    'staff_relationship_score': '''
+The support received from adults at school''',
+    'home_relationship_score': '''
+The support received from adults at home''',
+    'home_happy_score': '''
+Young people's feelings regarding the home that they live in''',
+    'local_env_score': '''
+How young people feel regarding the area where they live''',
+    'discrim_score': '''
+Whether young people feel discriminated against''',
+    'belong_local_score': '''
+Young people's feelings of belonging in their local area''',
+    'wealth_score': '''
+Whether young people feel their family is richer, poorer or the same as their
+friends''',
+    'future_score': '''
+How young people feel regarding the future options for work, education or
+training in their local area''',
+    'climate_score': '''
+Worries regarding climate change''',
+    'social_score': '''
+The support young people receive from their peers''',
+    'bully_score': '''
+The frequency with which young people experience different types of bullying'''
+}
```

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard/who_took_part.py` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard/who_took_part.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,206 +1,206 @@
-'''
-Helper functions for the 'Who took part' section of the dashboard and report
-'''
-from markdown import markdown
-import streamlit as st
-from .reshape_data import extract_nested_results
-from .bar_charts import survey_responses
-from .bar_charts_text import create_response_description
-
-
-def create_demographic_page_intro(school_size, output='streamlit'):
-    '''
-    Creates the title and introductory paragraph for the 'Who took part'
-    demographic section of the dashboard/report
-
-    Parameters
-    ----------
-    school_size : integer
-        Total number of pupils who completed at least one question at school
-    output : string
-        Specifies whether to write for 'streamlit' (default) or 'pdf'.
-
-    Returns
-    -------
-    html_string : string
-        Optional return, used when output=='pdf', contains HTML for report.
-    '''
-    # Title
-    title = 'Who took part?'
-
-    # Introductory paragraph
-    if output == 'streamlit':
-        type = 'page'
-    elif output == 'pdf':
-        type = 'section'
-    description = f'''
-There were {school_size} pupils at your school who took part in the #BeeWell
-survey. This {type} describes the sample of pupils who completed the survey.'''
-
-    # Write to streamlit dashboard
-    if output == 'streamlit':
-        st.title(title)
-        st.markdown(description)
-    # Write to PDF report
-    elif output == 'pdf':
-        html_string = f'''
-<div class='page'>
-    <div class='section_container'>
-        <h1 style='page-break-before:always;' id='who_took_part'>{title}</h1>
-        <p>{description}</p>
-    </div>
-</div>'''
-        return html_string
-
-
-def demographic_headers(survey_type='standard'):
-    '''
-    Creates dictionary of headers for the demographic section
-
-    Parameters
-    ----------
-    survey_type : string
-        Specifies whether this is for standard or symbol survey dashboard
-
-    Returns
-    -------
-    header_dict : dictionary
-        Dictionary where key is a variable name, and value is the header
-    '''
-    if survey_type == 'standard':
-        header_dict = {
-            'year_group': 'Year group',
-            'fsm': 'Eligible for free school meals (FSM)',
-            'gender': 'Gender and transgender',
-            'sexual_orientation': 'Sexual orientation',
-            'care_experience': 'Care experience',
-            'young_carer': 'Young carers',
-            'neuro': 'Special educational needs and neurodivergence',
-            'ethnicity': 'Ethnicity',
-            'english_additional': 'English as an additional language',
-            'birth': 'Background'}
-    elif survey_type == 'symbol':
-        header_dict = {
-            'gender': 'Gender',
-            'year_group': 'Year group',
-            'fsm': 'Eligible for free school meals (FSM)',
-            'ethnicity': 'Ethnicity',
-            'english_additional': 'English as an additional language'}
-    return header_dict
-
-
-def demographic_plots(
-        dem_prop, chosen_school=None, chosen_group=None,
-        group_lab='school_group_lab', output='streamlit', content=None,
-        survey_type='standard', dashboard_type='school'):
-    '''
-    Creates the plots for the Who Took Part page/section, with the relevant
-    headers and descriptions, for the streamlit dashboard or PDF report.
-
-    Parameters
-    ----------
-    dem_prop : dataframe
-        Dataframe with proportion of each responses to demographic questions
-    chosen_school : string
-        Optional input for school dashboard - name of the chosen school
-    chosen_group : string
-        Optional input for school dashboard - specifies whether to make plots
-        'For your school' or 'Compared with other schools in Northern Devon'.
-        Will do the latter unless you input 'For your school'.
-    group_lab : string
-        Name of chosen group  - default is school_group_lab.
-    output : string
-        Specifies whether to write for 'streamlit' (default) or 'pdf'.
-    content : list
-        Optional input used when output=='pdf', contains HTML for report.
-    survey_type : string
-        Specifies whether this is for 'standard' (default) or 'symbol'
-        survey dashboard.
-    dashboard_type : string
-        Specifies whether this is for 'school' (default) or 'area' dashboard.
-
-    Returns
-    -------
-    content : list
-        Optional return, used when output=='pdf', contains HTML for report.
-    '''
-    # If its for a school dashboard
-    if dashboard_type == 'school':
-        # Filter to results from current school
-        chosen = dem_prop[dem_prop['school_lab'] == chosen_school]
-        # If only looking at that school, drop the comparator school group data
-        if chosen_group == 'For your school':
-            chosen = chosen[chosen['school_group'] == 1]
-        # Extract the nested lists in the dataframe
-        chosen_result = extract_nested_results(
-            chosen=chosen, group_lab=group_lab, plot_group=True)
-    # For area dashboard, less pre-processing required...
-    else:
-        # Extract the nested lists in the dataframe
-        chosen_result = extract_nested_results(
-            chosen=dem_prop, group_lab=group_lab, plot_group=True)
-
-    # Generate titles and descriptions for the standard survey, and list of
-    # header sections
-    if survey_type == 'standard':
-        # Import descriptions for the charts
-        response_descrip = create_response_description()
-        # Import headers
-        dem_header_dict = demographic_headers(survey_type)
-        header_list = dem_header_dict.keys()
-    # We don't want section titles and descriptions for the symbol survey
-    # so just create list to loop through based on measure names
-    elif survey_type == 'symbol':
-        header_list = chosen_result['measure'].unique()
-
-    # Loop through each of the groups of plots
-    # This plots measures in loops, basing printed text on the measure names
-    # and basing the titles of groups on the group names (which differs to the
-    # survey responses page, which bases printed text on group names)
-    for plot_group in header_list:
-
-        # Add the title for that group for standard survey
-        if survey_type == 'standard':
-            if output == 'streamlit':
-                st.header(dem_header_dict[plot_group])
-            elif output == 'pdf':
-                content.append(f'''<h1 style='page-break-before:always;'
-                            id='{plot_group}'>
-                            {dem_header_dict[plot_group]}</h1>''')
-
-        # Find the measures in that group
-        measures = chosen_result.loc[
-            chosen_result['plot_group'] == plot_group,
-            'measure'].drop_duplicates()
-
-        # Loop through the measures
-        # Include a counter used for PDF report, as in report we want to
-        # break page before description, unless it is the first description
-        i = -1
-        for measure in measures:
-            i += 1
-
-            # Add descriptive text if there is any for standard survey
-            if survey_type == 'standard':
-                if measure in response_descrip.keys():
-                    if output == 'streamlit':
-                        st.markdown(response_descrip[measure])
-                    elif output == 'pdf':
-                        if i > 0:
-                            content.append(f'''
-    <p style='page-break-before:always;'>{markdown(response_descrip[measure])}
-    </p>''')
-                        else:
-                            content.append(f'''
-    <p>{markdown(response_descrip[measure])}</p>''')
-
-            # Filter data for that measure and produce plot
-            to_plot = chosen_result[chosen_result['measure'] == measure]
-            if output == 'streamlit':
-                survey_responses(to_plot, page='demographic')
-            elif output == 'pdf':
-                content = survey_responses(to_plot, font_size=14, output='pdf',
-                                           content=content, page='demographic')
-
-    if output == 'pdf':
-        return content
+'''
+Helper functions for the 'Who took part' section of the dashboard and report
+'''
+from markdown import markdown
+import streamlit as st
+from .reshape_data import extract_nested_results
+from .bar_charts import survey_responses
+from .bar_charts_text import create_response_description
+
+
+def create_demographic_page_intro(school_size, output='streamlit'):
+    '''
+    Creates the title and introductory paragraph for the 'Who took part'
+    demographic section of the dashboard/report
+
+    Parameters
+    ----------
+    school_size : integer
+        Total number of pupils who completed at least one question at school
+    output : string
+        Specifies whether to write for 'streamlit' (default) or 'pdf'.
+
+    Returns
+    -------
+    html_string : string
+        Optional return, used when output=='pdf', contains HTML for report.
+    '''
+    # Title
+    title = 'Who took part?'
+
+    # Introductory paragraph
+    if output == 'streamlit':
+        type = 'page'
+    elif output == 'pdf':
+        type = 'section'
+    description = f'''
+There were {school_size} pupils at your school who took part in the #BeeWell
+survey. This {type} describes the sample of pupils who completed the survey.'''
+
+    # Write to streamlit dashboard
+    if output == 'streamlit':
+        st.title(title)
+        st.markdown(description)
+    # Write to PDF report
+    elif output == 'pdf':
+        html_string = f'''
+<div class='page'>
+    <div class='section_container'>
+        <h1 style='page-break-before:always;' id='who_took_part'>{title}</h1>
+        <p>{description}</p>
+    </div>
+</div>'''
+        return html_string
+
+
+def demographic_headers(survey_type='standard'):
+    '''
+    Creates dictionary of headers for the demographic section
+
+    Parameters
+    ----------
+    survey_type : string
+        Specifies whether this is for standard or symbol survey dashboard
+
+    Returns
+    -------
+    header_dict : dictionary
+        Dictionary where key is a variable name, and value is the header
+    '''
+    if survey_type == 'standard':
+        header_dict = {
+            'year_group': 'Year group',
+            'fsm': 'Eligible for free school meals (FSM)',
+            'gender': 'Gender and transgender',
+            'sexual_orientation': 'Sexual orientation',
+            'care_experience': 'Care experience',
+            'young_carer': 'Young carers',
+            'neuro': 'Special educational needs and neurodivergence',
+            'ethnicity': 'Ethnicity',
+            'english_additional': 'English as an additional language',
+            'birth': 'Background'}
+    elif survey_type == 'symbol':
+        header_dict = {
+            'gender': 'Gender',
+            'year_group': 'Year group',
+            'fsm': 'Eligible for free school meals (FSM)',
+            'ethnicity': 'Ethnicity',
+            'english_additional': 'English as an additional language'}
+    return header_dict
+
+
+def demographic_plots(
+        dem_prop, chosen_school=None, chosen_group=None,
+        group_lab='school_group_lab', output='streamlit', content=None,
+        survey_type='standard', dashboard_type='school'):
+    '''
+    Creates the plots for the Who Took Part page/section, with the relevant
+    headers and descriptions, for the streamlit dashboard or PDF report.
+
+    Parameters
+    ----------
+    dem_prop : dataframe
+        Dataframe with proportion of each responses to demographic questions
+    chosen_school : string
+        Optional input for school dashboard - name of the chosen school
+    chosen_group : string
+        Optional input for school dashboard - specifies whether to make plots
+        'For your school' or 'Compared with other schools in Northern Devon'.
+        Will do the latter unless you input 'For your school'.
+    group_lab : string
+        Name of chosen group  - default is school_group_lab.
+    output : string
+        Specifies whether to write for 'streamlit' (default) or 'pdf'.
+    content : list
+        Optional input used when output=='pdf', contains HTML for report.
+    survey_type : string
+        Specifies whether this is for 'standard' (default) or 'symbol'
+        survey dashboard.
+    dashboard_type : string
+        Specifies whether this is for 'school' (default) or 'area' dashboard.
+
+    Returns
+    -------
+    content : list
+        Optional return, used when output=='pdf', contains HTML for report.
+    '''
+    # If its for a school dashboard
+    if dashboard_type == 'school':
+        # Filter to results from current school
+        chosen = dem_prop[dem_prop['school_lab'] == chosen_school]
+        # If only looking at that school, drop the comparator school group data
+        if chosen_group == 'For your school':
+            chosen = chosen[chosen['school_group'] == 1]
+        # Extract the nested lists in the dataframe
+        chosen_result = extract_nested_results(
+            chosen=chosen, group_lab=group_lab, plot_group=True)
+    # For area dashboard, less pre-processing required...
+    else:
+        # Extract the nested lists in the dataframe
+        chosen_result = extract_nested_results(
+            chosen=dem_prop, group_lab=group_lab, plot_group=True)
+
+    # Generate titles and descriptions for the standard survey, and list of
+    # header sections
+    if survey_type == 'standard':
+        # Import descriptions for the charts
+        response_descrip = create_response_description()
+        # Import headers
+        dem_header_dict = demographic_headers(survey_type)
+        header_list = dem_header_dict.keys()
+    # We don't want section titles and descriptions for the symbol survey
+    # so just create list to loop through based on measure names
+    elif survey_type == 'symbol':
+        header_list = chosen_result['measure'].unique()
+
+    # Loop through each of the groups of plots
+    # This plots measures in loops, basing printed text on the measure names
+    # and basing the titles of groups on the group names (which differs to the
+    # survey responses page, which bases printed text on group names)
+    for plot_group in header_list:
+
+        # Add the title for that group for standard survey
+        if survey_type == 'standard':
+            if output == 'streamlit':
+                st.header(dem_header_dict[plot_group])
+            elif output == 'pdf':
+                content.append(f'''<h1 style='page-break-before:always;'
+                            id='{plot_group}'>
+                            {dem_header_dict[plot_group]}</h1>''')
+
+        # Find the measures in that group
+        measures = chosen_result.loc[
+            chosen_result['plot_group'] == plot_group,
+            'measure'].drop_duplicates()
+
+        # Loop through the measures
+        # Include a counter used for PDF report, as in report we want to
+        # break page before description, unless it is the first description
+        i = -1
+        for measure in measures:
+            i += 1
+
+            # Add descriptive text if there is any for standard survey
+            if survey_type == 'standard':
+                if measure in response_descrip.keys():
+                    if output == 'streamlit':
+                        st.markdown(response_descrip[measure])
+                    elif output == 'pdf':
+                        if i > 0:
+                            content.append(f'''
+    <p style='page-break-before:always;'>{markdown(response_descrip[measure])}
+    </p>''')
+                        else:
+                            content.append(f'''
+    <p>{markdown(response_descrip[measure])}</p>''')
+
+            # Filter data for that measure and produce plot
+            to_plot = chosen_result[chosen_result['measure'] == measure]
+            if output == 'streamlit':
+                survey_responses(to_plot, page='demographic')
+            elif output == 'pdf':
+                content = survey_responses(to_plot, font_size=14, output='pdf',
+                                           content=content, page='demographic')
+
+    if output == 'pdf':
+        return content
```

### Comparing `kailo-beewell-dashboard-0.3.3/kailo_beewell_dashboard.egg-info/SOURCES.txt` & `kailo-beewell-dashboard-0.3.4/kailo_beewell_dashboard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.3/pyproject.toml` & `kailo-beewell-dashboard-0.3.4/pyproject.toml`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-[tool.poetry]
-name = "kailo-beewell-dashboard"
-version = "0.3.2"
-description = ""
-authors = ["ellengoddard <ellenamaliaa@gmail.com>"]
-license = "MIT"
-readme = "README.md"
-
-[tool.poetry.dependencies]
-python = ">=3.12,<3.13"
-pip = "24.0"
-numpy = "1.26.0"
-pandas = "2.1.1"
-plotly = "5.9.0"
-pymysql = "1.1.0"
-markdown = "3.5.2"
-kaleido = "0.2.1"
-weasyprint = "60.2"
-django = "4.2.9"
-ipykernel = "6.29.0"
-streamlit = ">=1.32.2"
-twine = "5.0.0"
-sphinx = "7.2.6"
-sphinx-rtd-theme = "2.0.0"
-myst-parser = "2.0.0"
-sphinx-autoapi = "3.0.0"
-matplotlib = "3.8.3"
-setuptools = "69.1.1"
-wheel = "0.42.0"
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "kailo-beewell-dashboard"
+version = "0.3.2"
+description = ""
+authors = ["ellengoddard <ellenamaliaa@gmail.com>"]
+license = "MIT"
+readme = "README.md"
+
+[tool.poetry.dependencies]
+python = ">=3.12,<3.13"
+pip = "24.0"
+numpy = "1.26.0"
+pandas = "2.1.1"
+plotly = "5.9.0"
+pymysql = "1.1.0"
+markdown = "3.5.2"
+kaleido = "0.2.1"
+weasyprint = "60.2"
+django = "4.2.9"
+ipykernel = "6.29.0"
+streamlit = ">=1.32.2"
+twine = "5.0.0"
+sphinx = "7.2.6"
+sphinx-rtd-theme = "2.0.0"
+myst-parser = "2.0.0"
+sphinx-autoapi = "3.0.0"
+matplotlib = "3.8.3"
+setuptools = "69.1.1"
+wheel = "0.42.0"
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `kailo-beewell-dashboard-0.3.3/requirements.txt` & `kailo-beewell-dashboard-0.3.4/requirements.txt`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-# For package installation
-pip==24.0
-
-# For data processing
-numpy==1.26.0
-pandas==2.1.1
-
-# To create plots
-plotly==5.9.0
-
-# To link with TiDB Cloud
-PyMySQL==1.1.0
-
-# To convert markdown text to HTML for PDF report
-markdown==3.5.2
-
-# For image export for the PDF report
-kaleido==0.2.1
-
-# To convert HTML report to PDF report
-weasyprint==60.2
-
-# For user authentication
-django==4.2.9
-
-# To run jupyter notebooks
-ipykernel==6.29.0
-
-# To create a streamlit dashboard
-streamlit>=1.32.2
-
-# To upload package to PYPI
-twine==5.0.0
-
-# To produce readthedocs
-sphinx==7.2.6
-sphinx-rtd-theme==2.0.0
-myst-parser==2.0.0
-sphinx-autoapi==3.0.0
-
-# To generate previews of figures in notebooks
-matplotlib==3.8.3
-
-setuptools==69.1.1
-wheel==0.42.0
+# For package installation
+pip==24.0
+
+# For data processing
+numpy==1.26.0
+pandas==2.1.1
+
+# To create plots
+plotly==5.9.0
+
+# To link with TiDB Cloud
+PyMySQL==1.1.0
+
+# To convert markdown text to HTML for PDF report
+markdown==3.5.2
+
+# For image export for the PDF report
+kaleido==0.2.1
+
+# To convert HTML report to PDF report
+weasyprint==60.2
+
+# For user authentication
+django==4.2.9
+
+# To run jupyter notebooks
+ipykernel==6.29.0
+
+# To create a streamlit dashboard
+streamlit>=1.32.2
+
+# To upload package to PYPI
+twine==5.0.0
+
+# To produce readthedocs
+sphinx==7.2.6
+sphinx-rtd-theme==2.0.0
+myst-parser==2.0.0
+sphinx-autoapi==3.0.0
+
+# To generate previews of figures in notebooks
+matplotlib==3.8.3
+
+setuptools==69.1.1
+wheel==0.42.0
```

