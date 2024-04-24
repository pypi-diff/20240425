# Comparing `tmp/mutwo.music-0.26.1.tar.gz` & `tmp/mutwo_music-0.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mutwo.music-0.26.1.tar", last modified: Tue Apr  9 22:04:01 2024, max compression
+gzip compressed data, was "mutwo_music-0.27.0.tar", last modified: Wed Apr 24 22:30:52 2024, max compression
```

## Comparing `mutwo.music-0.26.1.tar` & `mutwo_music-0.27.0.tar`

### file list

```diff
@@ -1,84 +1,85 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-09 22:04:01.732684 mutwo.music-0.26.1/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    35149 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2101 2024-04-09 22:04:01.732684 mutwo.music-0.26.1/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      823 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-09 22:04:01.720684 mutwo.music-0.26.1/mutwo/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-09 22:04:01.724684 mutwo.music-0.26.1/mutwo/music_converters/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      566 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_converters/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4313 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_converters/configurations.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11105 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_converters/grace_notes.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1139 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_converters/instruments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4877 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_converters/metricities.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12039 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_converters/parsers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    26267 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_converters/playing_indicators.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3443 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_converters/spectrals.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-09 22:04:01.724684 mutwo.music-0.26.1/mutwo/music_events/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      192 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_events/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8446 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_events/configurations.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10563 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_events/music.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-09 22:04:01.724684 mutwo.music-0.26.1/mutwo/music_generators/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_generators/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2359 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_generators/constants.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-09 22:04:01.724684 mutwo.music-0.26.1/mutwo/music_parameters/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1587 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    36923 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/abc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      490 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/ambituses.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2154 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/commas.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-09 22:04:01.724684 mutwo.music-0.26.1/mutwo/music_parameters/configurations/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      146 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/configurations/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2710 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/configurations/instruments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/configurations/lyrics.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1064 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/configurations/pitch_intervals.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3027 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/configurations/pitches.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      511 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/configurations/volumes.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-09 22:04:01.728684 mutwo.music-0.26.1/mutwo/music_parameters/constants/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      138 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/constants/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10201 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/constants/diatonic_pitch_classes.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      584 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/constants/instruments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4464 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/constants/pitch_intervals.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7580 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/constants/pitches.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3245 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/constants/playing_indicators.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      863 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/constants/volumes.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-09 22:04:01.728684 mutwo.music-0.26.1/mutwo/music_parameters/instruments/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      302 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/instruments/Bassoon.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      339 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/instruments/BfClarinet.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      427 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/instruments/CelticHarp.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      339 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/instruments/EfClarinet.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      298 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/instruments/Flute.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      296 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/instruments/Oboe.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      302 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/instruments/Piccolo.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      963 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/instruments/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22802 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/instruments/general.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-09 22:04:01.728684 mutwo.music-0.26.1/mutwo/music_parameters/lyrics/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1052 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/lyrics/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3357 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/lyrics/text_based_lyrics.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3467 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/notation_indicators.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23404 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/pitch_intervals.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-09 22:04:01.728684 mutwo.music-0.26.1/mutwo/music_parameters/pitches/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2451 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/pitches/CommonHarmonic.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1353 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/pitches/DirectPitch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9091 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/pitches/EqualDividedOctavePitch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    42947 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/pitches/JustIntonationPitch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1669 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/pitches/MidiPitch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2341 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/pitches/ScalePitch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24609 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/pitches/WesternPitch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1311 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/pitches/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9134 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/playing_indicators.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15358 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/scales.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8424 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_parameters/volumes.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-09 22:04:01.732684 mutwo.music-0.26.1/mutwo/music_utilities/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      341 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_utilities/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1196 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_utilities/exceptions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1597 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_utilities/indicator_collection_parsers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      645 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_utilities/tools.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-09 22:04:01.732684 mutwo.music-0.26.1/mutwo/music_version/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      144 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/mutwo/music_version/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-09 22:04:01.732684 mutwo.music-0.26.1/mutwo.music.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2101 2024-04-09 22:04:01.000000 mutwo.music-0.26.1/mutwo.music.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2759 2024-04-09 22:04:01.000000 mutwo.music-0.26.1/mutwo.music.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-09 22:04:01.000000 mutwo.music-0.26.1/mutwo.music.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      119 2024-04-09 22:04:01.000000 mutwo.music-0.26.1/mutwo.music.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2024-04-09 22:04:01.000000 mutwo.music-0.26.1/mutwo.music.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      200 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-09 22:04:01.732684 mutwo.music-0.26.1/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1843 2024-04-09 22:03:49.000000 mutwo.music-0.26.1/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 22:30:52.917789 mutwo_music-0.27.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    35149 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2101 2024-04-24 22:30:52.917789 mutwo_music-0.27.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      823 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 22:30:52.905789 mutwo_music-0.27.0/mutwo/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 22:30:52.909789 mutwo_music-0.27.0/mutwo/music_converters/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      566 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_converters/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4217 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_converters/configurations.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10581 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_converters/grace_notes.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1103 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_converters/instruments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4877 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_converters/metricities.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11805 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_converters/parsers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25199 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_converters/playing_indicators.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3443 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_converters/spectrals.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 22:30:52.909789 mutwo_music-0.27.0/mutwo/music_events/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      192 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_events/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      564 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_events/configurations.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9375 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_events/music.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 22:30:52.909789 mutwo_music-0.27.0/mutwo/music_generators/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_generators/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2359 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_generators/constants.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 22:30:52.909789 mutwo_music-0.27.0/mutwo/music_parameters/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1587 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_parameters/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    33838 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_parameters/abc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      490 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_parameters/ambituses.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2152 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_parameters/commas.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 22:30:52.913789 mutwo_music-0.27.0/mutwo/music_parameters/configurations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      146 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_parameters/configurations/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2710 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_parameters/configurations/instruments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_parameters/configurations/lyrics.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1064 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_parameters/configurations/pitch_intervals.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3027 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_parameters/configurations/pitches.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      511 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_parameters/configurations/volumes.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 22:30:52.913789 mutwo_music-0.27.0/mutwo/music_parameters/constants/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      138 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_parameters/constants/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10201 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_parameters/constants/diatonic_pitch_classes.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      584 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_parameters/constants/instruments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4464 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_parameters/constants/pitch_intervals.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7584 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_parameters/constants/pitches.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3245 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_parameters/constants/playing_indicators.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      863 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_parameters/constants/volumes.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 22:30:52.913789 mutwo_music-0.27.0/mutwo/music_parameters/instruments/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      302 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_parameters/instruments/Bassoon.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      339 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_parameters/instruments/BfClarinet.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      427 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_parameters/instruments/CelticHarp.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      339 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_parameters/instruments/EfClarinet.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      298 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_parameters/instruments/Flute.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      296 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_parameters/instruments/Oboe.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      302 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_parameters/instruments/Piccolo.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      963 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_parameters/instruments/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22674 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_parameters/instruments/general.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 22:30:52.913789 mutwo_music-0.27.0/mutwo/music_parameters/lyrics/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      814 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_parameters/lyrics/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3272 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_parameters/lyrics/text_based_lyrics.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2811 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_parameters/notation_indicators.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23172 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_parameters/pitch_intervals.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 22:30:52.917789 mutwo_music-0.27.0/mutwo/music_parameters/pitches/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2451 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_parameters/pitches/CommonHarmonic.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1200 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_parameters/pitches/DirectPitch.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8995 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_parameters/pitches/EqualDividedOctavePitch.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      850 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_parameters/pitches/FlexPitch.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    42592 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_parameters/pitches/JustIntonationPitch.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1567 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_parameters/pitches/MidiPitch.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2235 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_parameters/pitches/ScalePitch.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24450 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_parameters/pitches/WesternPitch.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1353 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_parameters/pitches/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7759 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_parameters/playing_indicators.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15468 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_parameters/scales.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9117 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_parameters/volumes.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 22:30:52.917789 mutwo_music-0.27.0/mutwo/music_utilities/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      341 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_utilities/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1196 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_utilities/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1597 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_utilities/indicator_collection_parsers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      645 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_utilities/tools.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 22:30:52.917789 mutwo_music-0.27.0/mutwo/music_version/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      144 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/mutwo/music_version/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 22:30:52.917789 mutwo_music-0.27.0/mutwo.music.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2101 2024-04-24 22:30:52.000000 mutwo_music-0.27.0/mutwo.music.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2803 2024-04-24 22:30:52.000000 mutwo_music-0.27.0/mutwo.music.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-24 22:30:52.000000 mutwo_music-0.27.0/mutwo.music.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      119 2024-04-24 22:30:52.000000 mutwo_music-0.27.0/mutwo.music.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2024-04-24 22:30:52.000000 mutwo_music-0.27.0/mutwo.music.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      200 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-24 22:30:52.917789 mutwo_music-0.27.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1843 2024-04-24 22:30:42.000000 mutwo_music-0.27.0/setup.py
```

### Comparing `mutwo.music-0.26.1/LICENSE` & `mutwo_music-0.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.1/PKG-INFO` & `mutwo_music-0.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutwo.music
-Version: 0.26.1
+Version: 0.27.0
 Summary: music extension for event based framework for generative art
 Home-page: https://github.com/mutwo-org/mutwo.music
 Author: Levin Eric Zimmermann
 Author-email: levin.eric.zimmermann@posteo.eu
 License: GPL
 Project-URL: Documentation, https://mutwo-org.github.io
 Classifier: Development Status :: 3 - Alpha
@@ -19,15 +19,15 @@
 Classifier: Topic :: Artistic Software
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Sound/Audio :: MIDI
 Requires-Python: >=3.10, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mutwo.core<2.0.0,>=1.3.0
+Requires-Dist: mutwo.core<3.0.0,>=2.0.0
 Requires-Dist: epitran<1.25,>=1.23
 Requires-Dist: sympy<2.0.0,>=1.10.1
 Requires-Dist: python-ranges<2.0.0,>=1.2.0
 Provides-Extra: testing
 Requires-Dist: pytest>=7.1.1; extra == "testing"
 
 # mutwo.music
```

### Comparing `mutwo.music-0.26.1/README.md` & `mutwo_music-0.27.0/README.md`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.1/mutwo/music_converters/__init__.py` & `mutwo_music-0.27.0/mutwo/music_converters/__init__.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.1/mutwo/music_converters/configurations.py` & `mutwo_music-0.27.0/mutwo/music_converters/configurations.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,81 +1,81 @@
 """Configure the default behaviour of :mod:`mutwo.music_converters`"""
 
 DEFAULT_PITCH_LIST_TO_SEARCH_NAME = "pitch_list"
 """Default value for :param:`pitch_list_to_search_name` parameter in
 :class:`mutwo.music_converters.MutwoParameterDictToPitchList` and
 default value for :param:`attribute_name` in
-:class:`mutwo.music_converters.SimpleEventToPitchList`."""
+:class:`mutwo.music_converters.ChrononToPitchList`."""
 
 DEFAULT_PITCH_LIST_KEYWORD_NAME = "pitch_list"
 """Default value for :param:`pitch_list_keyword_name` parameter in
 :class:`mutwo.core_converters.MutwoParameterDictToPitchList`"""
 
 DEFAULT_VOLUME_TO_SEARCH_NAME = "volume"
 """Default value for :param:`volume_to_search_name` parameter in
 :class:`mutwo.music_converters.MutwoParameterDictToVolume` and
 default value for :param:`attribute_name` in
-:class:`mutwo.music_converters.SimpleEventToVolume`."""
+:class:`mutwo.music_converters.ChrononToVolume`."""
 
 DEFAULT_VOLUME_KEYWORD_NAME = "volume"
 """Default value for :param:`volume_keyword_name` parameter in
 :class:`mutwo.core_converters.MutwoParameterDictToVolume`"""
 
 DEFAULT_INSTRUMENT_LIST_TO_SEARCH_NAME = "instrument_list"
 """Default value for :param:`instrument_list_to_search_name` parameter in
 :class:`mutwo.music_converters.MutwoParameterDictToInstrumentList` and
 default value for :param:`attribute_name` in
-:class:`mutwo.music_converters.SimpleEventToInstrumentList`."""
+:class:`mutwo.music_converters.ChrononToInstrumentList`."""
 
 DEFAULT_INSTRUMENT_LIST_KEYWORD_NAME = "instrument_list"
 """Default value for :param:`instrument_list_keyword_name` parameter in
 :class:`mutwo.core_converters.MutwoParameterDictToInstrumentList`"""
 
 DEFAULT_PLAYING_INDICATOR_COLLECTION_TO_SEARCH_NAME = "playing_indicator_collection"
 """Default value for :param:`playing_indicator_collection_to_search_name` parameter in
 :class:`mutwo.music_converters.MutwoParameterDictToPlayingIndicatorCollection` and
 default value for :param:`attribute_name` in
-:class:`mutwo.music_converters.SimpleEventToPlayingIndicatorCollection`."""
+:class:`mutwo.music_converters.ChrononToPlayingIndicatorCollection`."""
 
 DEFAULT_PLAYING_INDICATOR_COLLECTION_KEYWORD_NAME = "playing_indicator_collection"
 """Default value for :param:`playing_indicator_collection_keyword_name` parameter in
 :class:`mutwo.core_converters.MutwoParameterDictToPlayingIndicatorCollection`"""
 
 DEFAULT_NOTATION_INDICATOR_COLLECTION_TO_SEARCH_NAME = "notation_indicator_collection"
 """Default value for :param:`notation_indicator_collection_to_search_name` parameter in
 :class:`mutwo.music_converters.MutwoParameterDictToNotationIndicatorCollection` and
 default value for :param:`attribute_name` in
-:class:`mutwo.music_converters.SimpleEventToNotationIndicatorCollection`."""
+:class:`mutwo.music_converters.ChrononToNotationIndicatorCollection`."""
 
 DEFAULT_NOTATION_INDICATOR_COLLECTION_KEYWORD_NAME = "notation_indicator_collection"
 """Default value for :param:`notation_indicator_collection_keyword_name` parameter in
 :class:`mutwo.core_converters.MutwoParameterDictToNotationIndicatorCollection`"""
 
-DEFAULT_GRACE_NOTE_SEQUENTIAL_EVENT_TO_SEARCH_NAME = "grace_note_sequential_event"
-"""Default value for :param:`grace_note_sequential_event_to_search_name` parameter in
-:class:`mutwo.music_converters.MutwoParameterDictToGraceNoteSequentialEvent` and
-default value for :param:`attribute_name` in
-:class:`mutwo.music_converters.SimpleEventToGraceNoteSequentialEvent`."""
-
-DEFAULT_GRACE_NOTE_SEQUENTIAL_EVENT_KEYWORD_NAME = "grace_note_sequential_event"
-"""Default value for :param:`grace_note_sequential_event_keyword_name` parameter in
-:class:`mutwo.core_converters.MutwoParameterDictToGraceNoteSequentialEvent`"""
+DEFAULT_GRACE_NOTE_SEQUENTIAL_EVENT_TO_SEARCH_NAME = "grace_note_consecution"
+"""Default value for :param:`grace_note_consecution_to_search_name` parameter in
+:class:`mutwo.music_converters.MutwoParameterDictToGraceNoteConsecution` and
+default value for :param:`attribute_name` in
+:class:`mutwo.music_converters.ChrononToGraceNoteConsecution`."""
+
+DEFAULT_GRACE_NOTE_SEQUENTIAL_EVENT_KEYWORD_NAME = "grace_note_consecution"
+"""Default value for :param:`grace_note_consecution_keyword_name` parameter in
+:class:`mutwo.core_converters.MutwoParameterDictToGraceNoteConsecution`"""
 
 DEFAULT_AFTER_GRACE_NOTE_SEQUENTIAL_EVENT_TO_SEARCH_NAME = (
-    "after_grace_note_sequential_event"
+    "after_grace_note_consecution"
 )
-"""Default value for :param:`after_grace_note_sequential_event_to_search_name` parameter in
-:class:`mutwo.music_converters.MutwoParameterDictToAfterGraceNoteSequentialEvent` and
+"""Default value for :param:`after_grace_note_consecution_to_search_name` parameter in
+:class:`mutwo.music_converters.MutwoParameterDictToAfterGraceNoteConsecution` and
 default value for :param:`attribute_name` in
-:class:`mutwo.music_converters.SimpleEventToAfterGraceNoteSequentialEvent`."""
+:class:`mutwo.music_converters.ChrononToAfterGraceNoteConsecution`."""
 
 DEFAULT_AFTER_GRACE_NOTE_SEQUENTIAL_EVENT_KEYWORD_NAME = (
-    "after_grace_note_sequential_event"
+    "after_grace_note_consecution"
 )
-"""Default value for :param:`after_grace_note_sequential_event_keyword_name` parameter in
-:class:`mutwo.core_converters.MutwoParameterDictToAfterGraceNoteSequentialEvent`"""
+"""Default value for :param:`after_grace_note_consecution_keyword_name` parameter in
+:class:`mutwo.core_converters.MutwoParameterDictToAfterGraceNoteConsecution`"""
 
 DEFAULT_LYRIC_TO_SEARCH_NAME = "lyric"
 """Default value for :param:`lyric_to_search_name` parameter in
 :class:`mutwo.music_converters.MutwoParameterDictToLyric` and
 default value for :param:`attribute_name` in
-:class:`mutwo.music_converters.SimpleEventToLyric`."""
+:class:`mutwo.music_converters.ChrononToLyric`."""
```

### Comparing `mutwo.music-0.26.1/mutwo/music_converters/grace_notes.py` & `mutwo_music-0.27.0/mutwo/music_converters/grace_notes.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,92 +1,92 @@
 """Apply grace notes on Events"""
 
 import copy
 import typing
 
 from mutwo import core_converters
-from mutwo import core_constants
 from mutwo import core_events
+from mutwo import core_parameters
 from mutwo import music_converters
 
 __all__ = ("GraceNotesConverter",)
 
 
 class GraceNotesConverter(core_converters.abc.EventConverter):
     """Apply grace notes and after grace notes on :class:`core_events.abc.Event`.
 
     :param minima_grace_notes_duration_factor: Minimal percentage how much
-        of the initial duration of the :class:`~mutwo.core_events.SimpleEvent`
+        of the initial duration of the :class:`~mutwo.core_events.Chronon`
         shall be moved to the grace notes / after grace notes. This value has to be
-        smaller than 0.5 (so that the :class:`SimpleEvent` have a
+        smaller than 0.5 (so that the :class:`Chronon` have a
         duration > 0 if it has both: grace notes and after grace notes)
         and bigger than 0 (so that the grace notes or after grace notes
         have a duration > 0). Default to 0.12.
     :type minima_grace_notes_duration_factor: float
     :param maxima_grace_notes_duration_factor: Maxima percentage how much
-        of the initial duration of the :class:`~mutwo.core_events.SimpleEvent`
+        of the initial duration of the :class:`~mutwo.core_events.Chronon`
         shall be moved to the grace notes / after grace notes. This value has to be
-        smaller than 0.5 (so that the :class:`SimpleEvent` have a
+        smaller than 0.5 (so that the :class:`Chronon` have a
         duration > 0 if it has both: grace notes and after grace notes)
         and bigger than 0 (so that the grace notes or after grace notes
         have a duration > 0). Default to 0.25.
     :type maxima_grace_notes_duration_factor: float
     :param minima_number_of_grace_notes: For how many events in the grace
         note or after grace note container shall the
         `minima_grace_notes_duration_factor` be applied. Default to 1.
     :type minima_number_of_grace_notes: int
     :param maxima_number_of_grace_notes: For how many events in the grace
         note or after grace note container shall the
         `maxima_number_of_grace_notes` be applied. Default to 4.
     :type maxima_number_of_grace_notes: int
-    :param simple_event_to_grace_note_sequential_event: Function which
-        receives as an input a :class:`~mutwo.core_events.SimpleEvent`
-        and returns a :class:`~mutwo.core_events.SequentialEvent`.
+    :param chronon_to_grace_note_consecution: Function which
+        receives as an input a :class:`~mutwo.core_events.Chronon`
+        and returns a :class:`~mutwo.core_events.Consecution`.
         By default the function will ask the event for a
-        :attr:`~mutwo.events.music.NoteLike.grace_note_sequential_event`
-        attribute, because by default `~mutwo.events.music.NoteLike`
+        :attr:`~mutwo.music_events.NoteLike.grace_note_consecution`
+        attribute, because by default `~mutwo.music_events.NoteLike`
         objects are expected.
-    :type simple_event_to_grace_note_sequential_event: typing.Callable[[core_events.SimpleEvent], core_events.SequentialEvent[core_events.SimpleEvent]]
-    :param simple_event_to_after_grace_note_sequential_event: Function which
-        receives as an input a :class:`~mutwo.core_events.SimpleEvent`
-        and returns a :class:`~mutwo.core_events.SequentialEvent`.
+    :type chronon_to_grace_note_consecution: typing.Callable[[core_events.Chronon], core_events.Consecution[core_events.Chronon]]
+    :param chronon_to_after_grace_note_consecution: Function which
+        receives as an input a :class:`~mutwo.core_events.Chronon`
+        and returns a :class:`~mutwo.core_events.Consecution`.
         By default the function will ask the event for a
-        :attr:`~mutwo.events.music.NoteLike.grace_note_sequential_event`
-        attribute, because by default `~mutwo.events.music.NoteLike`
+        :attr:`~mutwo.music_events.NoteLike.grace_note_consecution`
+        attribute, because by default `~mutwo.music_events.NoteLike`
         objects are expected.
-    :type simple_event_to_after_grace_note_sequential_event: typing.Callable[[core_events.SimpleEvent], core_events.SequentialEvent[core_events.SimpleEvent]]
+    :type chronon_to_after_grace_note_consecution: typing.Callable[[core_events.Chronon], core_events.Consecution[core_events.Chronon]]
     """
 
     def __init__(
         self,
         minima_grace_notes_duration_factor: float = 0.12,
         maxima_grace_notes_duration_factor: float = 0.25,
         minima_number_of_grace_notes: int = 1,
         maxima_number_of_grace_notes: int = 4,
-        simple_event_to_grace_note_sequential_event: typing.Callable[
-            [core_events.SimpleEvent],
-            core_events.SequentialEvent[core_events.SimpleEvent],
-        ] = music_converters.SimpleEventToGraceNoteSequentialEvent(),
-        simple_event_to_after_grace_note_sequential_event: typing.Callable[
-            [core_events.SimpleEvent],
-            core_events.SequentialEvent[core_events.SimpleEvent],
-        ] = music_converters.SimpleEventToAfterGraceNoteSequentialEvent(),
+        chronon_to_grace_note_consecution: typing.Callable[
+            [core_events.Chronon],
+            core_events.Consecution[core_events.Chronon],
+        ] = music_converters.ChrononToGraceNoteConsecution(),
+        chronon_to_after_grace_note_consecution: typing.Callable[
+            [core_events.Chronon],
+            core_events.Consecution[core_events.Chronon],
+        ] = music_converters.ChrononToAfterGraceNoteConsecution(),
     ):
         self._test_input(
             minima_grace_notes_duration_factor,
             maxima_grace_notes_duration_factor,
             minima_number_of_grace_notes,
             maxima_number_of_grace_notes,
         )
 
-        self._simple_event_to_grace_note_sequential_event = (
-            simple_event_to_grace_note_sequential_event
+        self._chronon_to_grace_note_consecution = (
+            chronon_to_grace_note_consecution
         )
-        self._simple_event_to_after_grace_note_sequential_event = (
-            simple_event_to_after_grace_note_sequential_event
+        self._chronon_to_after_grace_note_consecution = (
+            chronon_to_after_grace_note_consecution
         )
 
         self._n_grace_notes_to_grace_note_duration_factor_envelope = (
             core_events.Envelope(
                 (
                     (minima_number_of_grace_notes, minima_grace_notes_duration_factor),
                     (maxima_number_of_grace_notes, maxima_grace_notes_duration_factor),
@@ -129,117 +129,117 @@
         try:
             assert minima_grace_notes_duration_factor > 0
         except AssertionError:
             raise ValueError(
                 "'minima_grace_notes_duration_factor' has " "to be bigger than 0!"
             )
 
-    def _get_grace_note_sequential_event(
-        self, simple_event_to_convert: core_events.SimpleEvent
-    ) -> core_events.SequentialEvent[core_events.SimpleEvent]:
-        return self._simple_event_to_grace_note_sequential_event(
-            simple_event_to_convert
+    def _get_grace_note_consecution(
+        self, chronon_to_convert: core_events.Chronon
+    ) -> core_events.Consecution[core_events.Chronon]:
+        return self._chronon_to_grace_note_consecution(
+            chronon_to_convert
         )
 
-    def _get_after_grace_note_sequential_event(
-        self, simple_event_to_convert: core_events.SimpleEvent
-    ) -> core_events.SequentialEvent[core_events.SimpleEvent]:
-        return self._simple_event_to_after_grace_note_sequential_event(
-            simple_event_to_convert
+    def _get_after_grace_note_consecution(
+        self, chronon_to_convert: core_events.Chronon
+    ) -> core_events.Consecution[core_events.Chronon]:
+        return self._chronon_to_after_grace_note_consecution(
+            chronon_to_convert
         )
 
-    def _convert_simple_event(
+    def _convert_chronon(
         self,
-        event_to_convert: core_events.SimpleEvent,
-        _: core_constants.DurationType,
-    ) -> core_events.SequentialEvent[core_events.SimpleEvent]:
-        """Convert instance of :class:`mutwo.core_events.SimpleEvent`."""
-
-        def adjust_grace_note_sequential_event(
-            grace_note_sequential_event: core_events.SequentialEvent[
-                core_events.SimpleEvent
+        event_to_convert: core_events.Chronon,
+        _: core_parameters.abc.Duration.Type,
+    ) -> core_events.Consecution[core_events.Chronon]:
+        """Convert instance of :class:`mutwo.core_events.Chronon`."""
+
+        def adjust_grace_note_consecution(
+            grace_note_consecution: core_events.Consecution[
+                core_events.Chronon
             ],
-        ) -> core_events.SequentialEvent:
-            if grace_note_sequential_event:
+        ) -> core_events.Consecution:
+            if grace_note_consecution:
                 factor_to_main_event = (
                     self._n_grace_notes_to_grace_note_duration_factor_envelope.value_at(
-                        len(grace_note_sequential_event)
+                        len(grace_note_consecution)
                     )
                 )
                 new_duration = event_to_convert.duration * factor_to_main_event
-                grace_note_sequential_event = grace_note_sequential_event.copy()
-                grace_note_sequential_event.duration = new_duration
-            return grace_note_sequential_event
+                grace_note_consecution = grace_note_consecution.copy()
+                grace_note_consecution.duration = new_duration
+            return grace_note_consecution
 
-        grace_note_sequential_event = adjust_grace_note_sequential_event(
-            self._get_grace_note_sequential_event(event_to_convert)
+        grace_note_consecution = adjust_grace_note_consecution(
+            self._get_grace_note_consecution(event_to_convert)
         )
-        after_grace_note_sequential_event = adjust_grace_note_sequential_event(
-            self._get_after_grace_note_sequential_event(event_to_convert)
+        after_grace_note_consecution = adjust_grace_note_consecution(
+            self._get_after_grace_note_consecution(event_to_convert)
         )
 
         copied_event_to_convert = copy.deepcopy(event_to_convert)
         # Remove applied grace notes / after grace notes
-        copied_event_to_convert.grace_note_sequential_event = (
-            core_events.SequentialEvent([])
+        copied_event_to_convert.grace_note_consecution = (
+            core_events.Consecution([])
         )
-        copied_event_to_convert.after_grace_note_sequential_event = (
-            core_events.SequentialEvent([])
+        copied_event_to_convert.after_grace_note_consecution = (
+            core_events.Consecution([])
         )
         copied_event_to_convert.duration -= (
-            grace_note_sequential_event.duration
-            + after_grace_note_sequential_event.duration
+            grace_note_consecution.duration
+            + after_grace_note_consecution.duration
         )
 
-        grace_note_sequential_event.append(copied_event_to_convert)
-        grace_note_sequential_event.extend(after_grace_note_sequential_event)
+        grace_note_consecution.append(copied_event_to_convert)
+        grace_note_consecution.extend(after_grace_note_consecution)
 
-        return grace_note_sequential_event
+        return grace_note_consecution
 
     def _convert_simultaneous_event(
         self,
-        simultaneous_event: core_events.SimultaneousEvent,
-        absolute_entry_delay: core_constants.DurationType,
-    ) -> tuple[core_events.SimultaneousEvent[core_events.abc.Event]]:
-        """Convert instance of :class:`mutwo.core_events.SimultaneousEvent`."""
+        simultaneous_event: core_events.Concurrence,
+        absolute_entry_delay: core_parameters.abc.Duration.Type,
+    ) -> tuple[core_events.Concurrence[core_events.abc.Event]]:
+        """Convert instance of :class:`mutwo.core_events.Concurrence`."""
 
         simultaneous_event_copied = simultaneous_event.empty_copy()
         for event in simultaneous_event:
             converted_event = self._convert_event(event, absolute_entry_delay)
-            # If we find a simple event, we shouldn't extend but append it to the
-            # the SimultaneousEvent. A converted simple event will be a
-            # SequentialEvent. The grace notes and after grace notes should
+            # If we find a chronon, we shouldn't extend but append it to the
+            # the Concurrence. A converted chronon will be a
+            # Consecution. The grace notes and after grace notes should
             # happen before and after the respective event. If we extend
-            # the whole SequentialEvent to the SimultaneousEvent the
+            # the whole Consecution to the Concurrence the
             # grace notes and after grace notes will be played simultaneously
             # with the main note, therefore we have to append them.
-            if isinstance(event, core_events.SimpleEvent):
+            if isinstance(event, core_events.Chronon):
                 simultaneous_event_copied.append(converted_event)
             else:
                 simultaneous_event_copied.extend(converted_event)
         return (simultaneous_event_copied,)
 
-    def _convert_sequential_event(
+    def _convert_consecution(
         self,
-        sequential_event: core_events.SequentialEvent,
-        absolute_entry_delay: core_constants.DurationType,
-    ) -> tuple[core_events.SequentialEvent[core_events.abc.Event]]:
-        sequential_event_copied = sequential_event.empty_copy()
-        sequential_event_copied.extend(
-            super()._convert_sequential_event(sequential_event, absolute_entry_delay)
+        consecution: core_events.Consecution,
+        absolute_entry_delay: core_parameters.abc.Duration.Type,
+    ) -> tuple[core_events.Consecution[core_events.abc.Event]]:
+        consecution_copied = consecution.empty_copy()
+        consecution_copied.extend(
+            super()._convert_consecution(consecution, absolute_entry_delay)
         )
-        return (sequential_event_copied,)
+        return (consecution_copied,)
 
     def convert(self, event_to_convert: core_events.abc.Event) -> core_events.abc.Event:
-        """Apply grace notes and after grace notes of all :class:`SimpleEvent`.
+        """Apply grace notes and after grace notes of all :class:`Chronon`.
 
         :param event_to_convert: The event which grace notes and after grace
             notes shall be converted to normal events in the upper
-            :class:`SequentialEvent`.
+            :class:`Consecution`.
         :type event_to_convert: core_events.abc.Event
         """
 
         converted_event = self._convert_event(event_to_convert, 0)
-        if isinstance(event_to_convert, core_events.SimpleEvent):
+        if isinstance(event_to_convert, core_events.Chronon):
             return converted_event
         else:
             return converted_event[0]
```

### Comparing `mutwo.music-0.26.1/mutwo/music_converters/instruments.py` & `mutwo_music-0.27.0/mutwo/music_converters/instruments.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from mutwo import core_converters
-from mutwo import core_constants
 from mutwo import core_events
 from mutwo import core_parameters
 from mutwo import music_parameters
 
 
 __all__ = ("InstrumentNoteLikeToPitchedNoteLike",)
 
@@ -15,18 +14,18 @@
         self,
         instrument_to_pitch_dict: dict[
             music_parameters.abc.Instrument, music_parameters.abc.Pitch
         ],
     ):
         self.instrument_to_pitch_dict = instrument_to_pitch_dict
 
-    def _convert_simple_event(
+    def _convert_chronon(
         self,
-        event_to_convert: core_events.SimpleEvent,
-        absolute_time: core_constants.DurationType,
+        event_to_convert: core_events.Chronon,
+        absolute_time: core_parameters.abc.Duration.Type,
     ):
         instrument = getattr(event_to_convert, "instrument", None)
         if instrument is not None:
             pitch_list = [self.instrument_to_pitch_dict[instrument]]
             return event_to_convert.copy().set_parameter("pitch_list", pitch_list)
         return event_to_convert
```

### Comparing `mutwo.music-0.26.1/mutwo/music_converters/metricities.py` & `mutwo_music-0.27.0/mutwo/music_converters/metricities.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.1/mutwo/music_converters/parsers.py` & `mutwo_music-0.27.0/mutwo/music_converters/parsers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Standardization for transformations between parameters and simple events
+"""Standardization for transformations between parameters and chronons
 
 All converters here expect by default a :class:`mutwo.music_events.NoteLike`
 (and uses the attribute names defined for the
 :class:`mutwo.music_events.NoteLike`). To adjust the used names you can change
 the values in the :mod:`mutwo.music_converters.configurations` module.
 """
 
@@ -13,86 +13,86 @@
 from mutwo import core_events
 from mutwo import music_converters
 from mutwo import music_events
 from mutwo import music_parameters
 
 
 __all__ = (
-    "SimpleEventToPitchList",
-    "SimpleEventToVolume",
-    "SimpleEventToLyric",
-    "SimpleEventToInstrumentList",
-    "SimpleEventToPlayingIndicatorCollection",
-    "SimpleEventToNotationIndicatorCollection",
-    "SimpleEventToGraceNoteSequentialEvent",
-    "SimpleEventToAfterGraceNoteSequentialEvent",
+    "ChrononToPitchList",
+    "ChrononToVolume",
+    "ChrononToLyric",
+    "ChrononToInstrumentList",
+    "ChrononToPlayingIndicatorCollection",
+    "ChrononToNotationIndicatorCollection",
+    "ChrononToGraceNoteConsecution",
+    "ChrononToAfterGraceNoteConsecution",
     "MutwoParameterDictToPitchList",
     "MutwoParameterDictToVolume",
     "MutwoParameterDictToInstrumentList",
     "MutwoParameterDictToPlayingIndicatorCollection",
     "MutwoParameterDictToNotationIndicatorCollection",
-    "MutwoParameterDictToGraceNoteSequentialEvent",
-    "MutwoParameterDictToAfterGraceNoteSequentialEvent",
+    "MutwoParameterDictToGraceNoteConsecution",
+    "MutwoParameterDictToAfterGraceNoteConsecution",
     "MutwoParameterDictToNoteLike",
 )
 
 
-class SimpleEventToPitchList(core_converters.SimpleEventToAttribute):
+class ChrononToPitchList(core_converters.ChrononToAttribute):
     def __init__(
         self,
         attribute_name: typing.Optional[str] = None,
         exception_value: list[music_parameters.abc.Pitch] = [],
     ):
         super().__init__(
             attribute_name
             or music_converters.configurations.DEFAULT_PITCH_LIST_TO_SEARCH_NAME,
             exception_value,
         )
 
 
-class SimpleEventToVolume(core_converters.SimpleEventToAttribute):
+class ChrononToVolume(core_converters.ChrononToAttribute):
     def __init__(
         self,
         attribute_name: typing.Optional[str] = None,
-        exception_value: music_parameters.abc.Volume = music_parameters.DirectVolume(0),
+        exception_value: music_parameters.abc.Volume = music_parameters.AmplitudeVolume(0),
     ):
         super().__init__(
             attribute_name
             or (music_converters.configurations.DEFAULT_VOLUME_TO_SEARCH_NAME),
             exception_value,
         )
 
 
-class SimpleEventToLyric(core_converters.SimpleEventToAttribute):
+class ChrononToLyric(core_converters.ChrononToAttribute):
     def __init__(
         self,
         attribute_name: typing.Optional[str] = None,
         exception_value: music_parameters.abc.Volume = music_parameters.DirectLyric(""),
     ):
         super().__init__(
             attribute_name
             or music_converters.configurations.DEFAULT_LYRIC_TO_SEARCH_NAME,
             exception_value,
         )
 
 
-class SimpleEventToInstrumentList(core_converters.SimpleEventToAttribute):
+class ChrononToInstrumentList(core_converters.ChrononToAttribute):
     def __init__(
         self,
         attribute_name: typing.Optional[str] = None,
         exception_value: typing.Optional[music_parameters.abc.Instrument] = [],
     ):
         super().__init__(
             attribute_name
             or music_converters.configurations.DEFAULT_INSTRUMENT_LIST_TO_SEARCH_NAME,
             exception_value,
         )
 
 
-class SimpleEventToAttributeWithDefaultValue(core_converters.SimpleEventToAttribute):
+class ChrononToAttributeWithDefaultValue(core_converters.ChrononToAttribute):
     @abc.abstractmethod
     def _get_default_exception_value(self) -> typing.Any:
         raise NotImplementedError
 
     def convert(self, *args, **kwargs) -> typing.Any:
         # If it is undefined we will use the default value.
         is_default_exception_value = self._exception_value is None
@@ -108,15 +108,15 @@
 
         if is_default_exception_value:
             self._exception_value = None
 
         return attribute
 
 
-class SimpleEventToPlayingIndicatorCollection(SimpleEventToAttributeWithDefaultValue):
+class ChrononToPlayingIndicatorCollection(ChrononToAttributeWithDefaultValue):
     def __init__(
         self,
         attribute_name: typing.Optional[str] = None,
         exception_value: typing.Optional[
             music_parameters.NotationIndicatorCollection
         ] = None,
     ):
@@ -126,15 +126,15 @@
             exception_value,
         )
 
     def _get_default_exception_value(self) -> typing.Any:
         return music_events.configurations.DEFAULT_PLAYING_INDICATORS_COLLECTION_CLASS()
 
 
-class SimpleEventToNotationIndicatorCollection(SimpleEventToAttributeWithDefaultValue):
+class ChrononToNotationIndicatorCollection(ChrononToAttributeWithDefaultValue):
     def __init__(
         self,
         attribute_name: typing.Optional[str] = None,
         exception_value: typing.Optional[
             music_parameters.NotationIndicatorCollection
         ] = None,
     ):
@@ -146,34 +146,34 @@
 
     def _get_default_exception_value(self) -> typing.Any:
         return (
             music_events.configurations.DEFAULT_NOTATION_INDICATORS_COLLECTION_CLASS()
         )
 
 
-class SimpleEventToGraceNoteSequentialEvent(core_converters.SimpleEventToAttribute):
+class ChrononToGraceNoteConsecution(core_converters.ChrononToAttribute):
     def __init__(
         self,
         attribute_name: typing.Optional[str] = None,
-        exception_value: core_events.SequentialEvent = core_events.SequentialEvent([]),
+        exception_value: core_events.Consecution = core_events.Consecution([]),
     ):
         super().__init__(
             attribute_name
             or music_converters.configurations.DEFAULT_GRACE_NOTE_SEQUENTIAL_EVENT_TO_SEARCH_NAME,
             exception_value,
         )
 
 
-class SimpleEventToAfterGraceNoteSequentialEvent(
-    core_converters.SimpleEventToAttribute
+class ChrononToAfterGraceNoteConsecution(
+    core_converters.ChrononToAttribute
 ):
     def __init__(
         self,
         attribute_name: typing.Optional[str] = None,
-        exception_value: core_events.SequentialEvent = core_events.SequentialEvent([]),
+        exception_value: core_events.Consecution = core_events.Consecution([]),
     ):
         super().__init__(
             attribute_name
             or music_converters.configurations.DEFAULT_AFTER_GRACE_NOTE_SEQUENTIAL_EVENT_TO_SEARCH_NAME,
             exception_value,
         )
 
@@ -252,73 +252,73 @@
             notation_indicator_collection_to_search_name
             or music_converters.configurations.DEFAULT_NOTATION_INDICATOR_COLLECTION_TO_SEARCH_NAME,
             notation_indicator_collection_keyword_name
             or music_converters.configurations.DEFAULT_NOTATION_INDICATOR_COLLECTION_KEYWORD_NAME,
         )
 
 
-class MutwoParameterDictToGraceNoteSequentialEvent(
+class MutwoParameterDictToGraceNoteConsecution(
     core_converters.MutwoParameterDictToKeywordArgument
 ):
     def __init__(
         self,
-        grace_note_sequential_event_to_search_name: typing.Optional[str] = None,
-        grace_note_sequential_event_keyword_name: typing.Optional[str] = None,
+        grace_note_consecution_to_search_name: typing.Optional[str] = None,
+        grace_note_consecution_keyword_name: typing.Optional[str] = None,
     ):
         super().__init__(
-            grace_note_sequential_event_to_search_name
+            grace_note_consecution_to_search_name
             or music_converters.configurations.DEFAULT_GRACE_NOTE_SEQUENTIAL_EVENT_TO_SEARCH_NAME,
-            grace_note_sequential_event_keyword_name
+            grace_note_consecution_keyword_name
             or music_converters.configurations.DEFAULT_GRACE_NOTE_SEQUENTIAL_EVENT_KEYWORD_NAME,
         )
 
 
-class MutwoParameterDictToAfterGraceNoteSequentialEvent(
+class MutwoParameterDictToAfterGraceNoteConsecution(
     core_converters.MutwoParameterDictToKeywordArgument
 ):
     def __init__(
         self,
-        after_grace_note_sequential_event_to_search_name: typing.Optional[str] = None,
-        after_grace_note_sequential_event_keyword_name: typing.Optional[str] = None,
+        after_grace_note_consecution_to_search_name: typing.Optional[str] = None,
+        after_grace_note_consecution_keyword_name: typing.Optional[str] = None,
     ):
         super().__init__(
-            after_grace_note_sequential_event_to_search_name
+            after_grace_note_consecution_to_search_name
             or music_converters.configurations.DEFAULT_AFTER_GRACE_NOTE_SEQUENTIAL_EVENT_TO_SEARCH_NAME,
-            after_grace_note_sequential_event_keyword_name
+            after_grace_note_consecution_keyword_name
             or music_converters.configurations.DEFAULT_AFTER_GRACE_NOTE_SEQUENTIAL_EVENT_KEYWORD_NAME,
         )
 
 
-class MutwoParameterDictToNoteLike(core_converters.MutwoParameterDictToSimpleEvent):
+class MutwoParameterDictToNoteLike(core_converters.MutwoParameterDictToChronon):
     """Convert a dict of mutwo parameters to a :class:`mutwo.music_events.NoteLike`
 
     :param mutwo_parameter_dict_to_keyword_argument_sequence: A sequence of
         :class:`MutwoParameterDictToKeywordArgument`.
         Default to `None`.
     :type mutwo_parameter_dict_to_keyword_argument_sequence: typing.Optional[typing.Sequence[MutwoParameterDictToKeywordArgument]]
-    :param simple_event_class: Default to :class:`mutwo.music_events.NoteLike`.
-    :type simple_event_class: typing.Type[core_events.SimpleEvent]
+    :param chronon_class: Default to :class:`mutwo.music_events.NoteLike`.
+    :type chronon_class: typing.Type[core_events.Chronon]
     """
 
     def __init__(
         self,
         mutwo_parameter_dict_to_keyword_argument_sequence: typing.Optional[
             typing.Sequence[core_converters.MutwoParameterDictToKeywordArgument]
         ] = None,
-        simple_event_class: typing.Type[
-            core_events.SimpleEvent
+        chronon_class: typing.Type[
+            core_events.Chronon
         ] = music_events.NoteLike,
     ):
         if mutwo_parameter_dict_to_keyword_argument_sequence is None:
             mutwo_parameter_dict_to_keyword_argument_sequence = (
                 core_converters.MutwoParameterDictToDuration(),
                 MutwoParameterDictToPitchList(),
                 MutwoParameterDictToVolume(),
                 MutwoParameterDictToPlayingIndicatorCollection(),
                 MutwoParameterDictToNotationIndicatorCollection(),
-                MutwoParameterDictToGraceNoteSequentialEvent(),
-                MutwoParameterDictToAfterGraceNoteSequentialEvent(),
+                MutwoParameterDictToGraceNoteConsecution(),
+                MutwoParameterDictToAfterGraceNoteConsecution(),
                 MutwoParameterDictToInstrumentList(),
             )
         super().__init__(
-            mutwo_parameter_dict_to_keyword_argument_sequence, simple_event_class
+            mutwo_parameter_dict_to_keyword_argument_sequence, chronon_class
         )
```

### Comparing `mutwo.music-0.26.1/mutwo/music_converters/playing_indicators.py` & `mutwo_music-0.27.0/mutwo/music_converters/playing_indicators.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 import typing
 
 try:
     import quicktions as fractions  # type: ignore
 except ImportError:
     import fractions  # type: ignore
 
-from mutwo import core_constants
 from mutwo import core_converters
 from mutwo import core_events
+from mutwo import core_parameters
 from mutwo import core_utilities
 from mutwo import music_converters
 from mutwo import music_parameters
 from mutwo import music_utilities
 
 
 __all__ = (
@@ -30,300 +30,289 @@
     "TrillConverter",
     "OptionalConverter",
     "PlayingIndicatorsConverter",
 )
 
 
 class PlayingIndicatorConverter(core_converters.abc.Converter):
-    """Abstract base class to apply :class:`~mutwo.music_parameters.abc.PlayingIndicator` on a :class:`~mutwo.core_events.SimpleEvent`.
+    """Abstract base class to apply :class:`~mutwo.music_parameters.abc.PlayingIndicator` on a :class:`~mutwo.core_events.Chronon`.
 
-    :param simple_event_to_playing_indicator_collection: Function to extract from a
-        :class:`mutwo.core_events.SimpleEvent` a
+    :param chronon_to_playing_indicator_collection: Function to extract from a
+        :class:`mutwo.core_events.Chronon` a
         :class:`mutwo.music_parameters.PlayingIndicatorCollection`
         object. By default it asks the Event for its
         :attr:`~mutwo.music_events.NoteLike.playing_indicator_collection`
         attribute (because by default :class:`mutwo.music_events.NoteLike`
         objects are expected).
         When using different Event classes than :class:`~mutwo.music_events.NoteLike`
         with a different name for their playing_indicator_collection property, this argument
         should be overridden. If the
         function call raises an :obj:`AttributeError` (e.g. if no playing indicator
         collection can be extracted), mutwo will build a playing indicator collection
         from :const:`~mutwo.music_events.configurations.DEFAULT_PLAYING_INDICATORS_COLLECTION_CLASS`.
-    :type simple_event_to_playing_indicator_collection: typing.Callable[[core_events.SimpleEvent], music_parameters.PlayingIndicatorCollection], optional
+    :type chronon_to_playing_indicator_collection: typing.Callable[[core_events.Chronon], music_parameters.PlayingIndicatorCollection], optional
 
     To write a new PlayingIndicatorConverter the abstract method
     :func:`_apply_playing_indicator` and the abstract properties
     `playing_indicator_name` and `default_playing_indicator` have
     to be overridden.
     """
 
     def __init__(
         self,
-        simple_event_to_playing_indicator_collection: typing.Callable[
-            [core_events.SimpleEvent],
+        chronon_to_playing_indicator_collection: typing.Callable[
+            [core_events.Chronon],
             music_parameters.PlayingIndicatorCollection,
-        ] = music_converters.SimpleEventToPlayingIndicatorCollection(),  # type: ignore
+        ] = music_converters.ChrononToPlayingIndicatorCollection(),  # type: ignore
     ):
-        self._simple_event_to_playing_indicator_collection = (
-            simple_event_to_playing_indicator_collection
+        self._chronon_to_playing_indicator_collection = (
+            chronon_to_playing_indicator_collection
         )
 
     @abc.abstractmethod
     def _apply_playing_indicator(
         self,
-        simple_event_to_convert: core_events.SimpleEvent,
+        chronon_to_convert: core_events.Chronon,
         playing_indicator: music_parameters.abc.PlayingIndicator,
-    ) -> core_events.SequentialEvent[core_events.SimpleEvent]:
+    ) -> core_events.Consecution[core_events.Chronon]:
         ...
 
     @property
     @abc.abstractmethod
     def playing_indicator_name(self) -> str:
         ...
 
     @property
     @abc.abstractmethod
     def default_playing_indicator(self) -> music_parameters.abc.PlayingIndicator:
         ...
 
     def convert(
-        self, simple_event_to_convert: core_events.SimpleEvent
-    ) -> core_events.SequentialEvent[core_events.SimpleEvent]:
-        """Apply PlayingIndicator on simple_event.
+        self, chronon_to_convert: core_events.Chronon
+    ) -> core_events.Consecution[core_events.Chronon]:
+        """Apply PlayingIndicator on chronon.
 
-        :param simple_event_to_convert: The event which shall be converted.
-        :type simple_event_to_convert: core_events.SimpleEvent
+        :param chronon_to_convert: The event which shall be converted.
+        :type chronon_to_convert: core_events.Chronon
         """
 
-        playing_indicator_collection = (
-            self._simple_event_to_playing_indicator_collection(
-                simple_event_to_convert,
-            )
+        playing_indicator_collection = self._chronon_to_playing_indicator_collection(
+            chronon_to_convert,
         )
         playing_indicator = core_utilities.call_function_except_attribute_error(
             lambda playing_indicator_collection: getattr(
                 playing_indicator_collection, self.playing_indicator_name
             ),
             playing_indicator_collection,
             self.default_playing_indicator,
         )
 
         if playing_indicator.is_active:
-            return self._apply_playing_indicator(
-                simple_event_to_convert, playing_indicator
-            )
+            return self._apply_playing_indicator(chronon_to_convert, playing_indicator)
         else:
-            return core_events.SequentialEvent([copy.deepcopy(simple_event_to_convert)])
+            return core_events.Consecution([copy.deepcopy(chronon_to_convert)])
 
 
 class ArpeggioConverter(PlayingIndicatorConverter):
-    """Apply arpeggio on :class:`~mutwo.core_events.SimpleEvent`.
+    """Apply arpeggio on :class:`~mutwo.core_events.Chronon`.
 
     :param duration_for_each_attack: Set how long each attack of the
         Arpeggio lasts. Default to 0.1.
-    :type duration_for_each_attack: constants.DurationType
-    :param simple_event_to_pitch_list: Function to extract from a
-        :class:`mutwo.core_events.SimpleEvent` a tuple that contains pitch objects
+    :type duration_for_each_attack: core_parameters.abc.Duration.Type
+    :param chronon_to_pitch_list: Function to extract from a
+        :class:`mutwo.core_events.Chronon` a tuple that contains pitch objects
         (objects that inherit from :class:`mutwo.music_parameters.abc.Pitch`).
         By default it asks the Event for its
         :attr:`~mutwo.music_events.NoteLike.pitch_list` attribute
         (because by default :class:`mutwo.music_events.NoteLike` objects are expected).
         When using different Event classes than :class:`~mutwo.music_events.NoteLike`
         with a different name for their pitch property, this argument
         should be overridden.
         If the function call raises an :obj:`AttributeError` (e.g. if no pitch can be
         extracted), mutwo will assume an event without any pitches.
-    :type simple_event_to_pitch_list: typing.Callable[[core_events.SimpleEvent], music_parameters.abc.Pitch], optional
-    :param simple_event_to_playing_indicator_collection: Function to extract from a
-        :class:`mutwo.core_events.SimpleEvent` a
+    :type chronon_to_pitch_list: typing.Callable[[core_events.Chronon], music_parameters.abc.Pitch], optional
+    :param chronon_to_playing_indicator_collection: Function to extract from a
+        :class:`mutwo.core_events.Chronon` a
         :class:`mutwo.music_parameters.PlayingIndicatorCollection`
         object. By default it asks the Event for its
         :attr:`~mutwo.music_events.NoteLike.playing_indicator_collection`
         attribute (because by default :class:`mutwo.music_events.NoteLike`
         objects are expected).
         When using different Event classes than :class:`~mutwo.music_events.NoteLike`
         with a different name for their playing_indicator_collection property, this argument
         should be overridden. If the
         function call raises an :obj:`AttributeError` (e.g. if no playing indicator
         collection can be extracted), mutwo will build a playing indicator collection
         from :const:`~mutwo.music_events.configurations.DEFAULT_PLAYING_INDICATORS_COLLECTION_CLASS`.
-    :type simple_event_to_playing_indicator_collection: typing.Callable[[core_events.SimpleEvent], music_parameters.PlayingIndicatorCollection,], optional
-    :param set_pitch_list_for_simple_event: Function which assigns
+    :type chronon_to_playing_indicator_collection: typing.Callable[[core_events.Chronon], music_parameters.PlayingIndicatorCollection,], optional
+    :param set_pitch_list_for_chronon: Function which assigns
         a list of :class:`~mutwo.music_parameters.abc.Pitch` objects to a
-        :class:`~mutwo.core_events.SimpleEvent`. By default the
+        :class:`~mutwo.core_events.Chronon`. By default the
         function assigns the passed pitches to the
         :attr:`~mutwo.music_events.NoteLike.pitch_list` attribute
         (because by default :class:`mutwo.music_events.NoteLike` objects
         are expected).
-    :type set_pitch_list_for_simple_event: typing.Callable[[core_events.SimpleEvent, list[music_parameters.abc.Pitch]], None]
+    :type set_pitch_list_for_chronon: typing.Callable[[core_events.Chronon, list[music_parameters.abc.Pitch]], None]
     """
 
     def __init__(
         self,
-        duration_for_each_attack: core_constants.DurationType = 0.1,
-        simple_event_to_pitch_list: typing.Callable[
-            [core_events.SimpleEvent], list[music_parameters.abc.Pitch]
-        ] = music_converters.SimpleEventToPitchList(),
-        simple_event_to_playing_indicator_collection: typing.Callable[
-            [core_events.SimpleEvent],
+        duration_for_each_attack: core_parameters.abc.Duration.Type = 0.1,
+        chronon_to_pitch_list: typing.Callable[
+            [core_events.Chronon], list[music_parameters.abc.Pitch]
+        ] = music_converters.ChrononToPitchList(),
+        chronon_to_playing_indicator_collection: typing.Callable[
+            [core_events.Chronon],
             music_parameters.PlayingIndicatorCollection,
-        ] = music_converters.SimpleEventToPlayingIndicatorCollection(),
-        set_pitch_list_for_simple_event: typing.Callable[
-            [core_events.SimpleEvent, list[music_parameters.abc.Pitch]], None
-        ] = lambda simple_event, pitch_list: simple_event.set_parameter(  # type: ignore
+        ] = music_converters.ChrononToPlayingIndicatorCollection(),
+        set_pitch_list_for_chronon: typing.Callable[
+            [core_events.Chronon, list[music_parameters.abc.Pitch]], None
+        ] = lambda chronon, pitch_list: chronon.set_parameter(  # type: ignore
             "pitch_list", pitch_list, set_unassigned_parameter=True
         ),
     ):
         super().__init__(
-            simple_event_to_playing_indicator_collection=simple_event_to_playing_indicator_collection
+            chronon_to_playing_indicator_collection=chronon_to_playing_indicator_collection
         )
-        self._duration_for_each_attack = (
-            core_events.configurations.UNKNOWN_OBJECT_TO_DURATION(
-                duration_for_each_attack
-            )
+        self._duration_for_each_attack = core_parameters.abc.Duration.from_any(
+            duration_for_each_attack
         )
-        self._simple_event_to_pitch_list = simple_event_to_pitch_list
-        self._set_pitch_list_for_simple_event = set_pitch_list_for_simple_event
+        self._chronon_to_pitch_list = chronon_to_pitch_list
+        self._set_pitch_list_for_chronon = set_pitch_list_for_chronon
 
     @property
     def playing_indicator_name(self) -> str:
         return "arpeggio"
 
     @property
     def default_playing_indicator(self) -> music_parameters.abc.PlayingIndicator:
         return music_parameters.Arpeggio()
 
     def _apply_playing_indicator(
         self,
-        simple_event_to_convert: core_events.SimpleEvent,
+        chronon_to_convert: core_events.Chronon,
         playing_indicator: music_parameters.Arpeggio,
-    ) -> core_events.SequentialEvent[core_events.SimpleEvent]:
-        pitch_list = list(self._simple_event_to_pitch_list(simple_event_to_convert))
+    ) -> core_events.Consecution[core_events.Chronon]:
+        pitch_list = list(self._chronon_to_pitch_list(chronon_to_convert))
 
         # sort pitches according to Arpeggio direction
         pitch_list.sort(reverse=playing_indicator.direction != "up")
 
-        converted_event: core_events.SequentialEvent[
-            core_events.SimpleEvent
-        ] = core_events.SequentialEvent(
-            [copy.copy(simple_event_to_convert) for _ in pitch_list]
-        )
+        converted_event: core_events.Consecution[
+            core_events.Chronon
+        ] = core_events.Consecution([copy.copy(chronon_to_convert) for _ in pitch_list])
 
         # apply pitches on events
         for event_index, pitch in enumerate(pitch_list):
-            self._set_pitch_list_for_simple_event(converted_event[event_index], [pitch])
+            self._set_pitch_list_for_chronon(converted_event[event_index], [pitch])
 
         # set correct duration for each event
         event_count = len(converted_event)
         duration_of_each_attack = self._duration_for_each_attack
-        if duration_of_each_attack * event_count > simple_event_to_convert.duration:
-            duration_of_each_attack = simple_event_to_convert.duration / event_count
+        if duration_of_each_attack * event_count > chronon_to_convert.duration:
+            duration_of_each_attack = chronon_to_convert.duration / event_count
 
         for event_index in range(event_count - 1):
             converted_event[event_index].duration = duration_of_each_attack
 
         converted_event[-1].duration -= (
-            converted_event.duration - simple_event_to_convert.duration
+            converted_event.duration - chronon_to_convert.duration
         )
 
         return converted_event
 
 
 class StacattoConverter(PlayingIndicatorConverter):
-    """Apply staccato on :class:`~mutwo.core_events.SimpleEvent`.
+    """Apply staccato on :class:`~mutwo.core_events.Chronon`.
 
     :param factor:
     :param allowed_articulation_name_sequence:
-    :param simple_event_to_playing_indicator_collection: Function to extract from a
-        :class:`mutwo.core_events.SimpleEvent` a
+    :param chronon_to_playing_indicator_collection: Function to extract from a
+        :class:`mutwo.core_events.Chronon` a
         :class:`mutwo.music_parameters.PlayingIndicatorCollection`
         object. By default it asks the Event for its
         :attr:`~mutwo.music_events.NoteLike.playing_indicator_collection`
         attribute (because by default :class:`mutwo.music_events.NoteLike`
         objects are expected).
         When using different Event classes than :class:`~mutwo.music_events.NoteLike`
         with a different name for their playing_indicator_collection property, this argument
         should be overridden. If the
         function call raises an :obj:`AttributeError` (e.g. if no playing indicator
         collection can be extracted), mutwo will build a playing indicator collection
         from :const:`~mutwo.music_events.configurations.DEFAULT_PLAYING_INDICATORS_COLLECTION_CLASS`.
-    :type simple_event_to_playing_indicator_collection: typing.Callable[[core_events.SimpleEvent], music_parameters.PlayingIndicatorCollection,], optional
+    :type chronon_to_playing_indicator_collection: typing.Callable[[core_events.Chronon], music_parameters.PlayingIndicatorCollection,], optional
     """
 
     def __init__(
         self,
         factor: float = 0.5,
         allowed_articulation_name_sequence: typing.Sequence[str] = ("staccato", "."),
-        simple_event_to_playing_indicator_collection: typing.Callable[
-            [core_events.SimpleEvent],
+        chronon_to_playing_indicator_collection: typing.Callable[
+            [core_events.Chronon],
             music_parameters.PlayingIndicatorCollection,
-        ] = music_converters.SimpleEventToPlayingIndicatorCollection(),
+        ] = music_converters.ChrononToPlayingIndicatorCollection(),
     ):
         self._allowed_articulation_name_sequence = allowed_articulation_name_sequence
         self._factor = factor
-        super().__init__(simple_event_to_playing_indicator_collection)
+        super().__init__(chronon_to_playing_indicator_collection)
 
     def _apply_playing_indicator(
         self,
-        simple_event_to_convert: core_events.SimpleEvent,
+        chronon_to_convert: core_events.Chronon,
         _: music_parameters.abc.PlayingIndicator,
-    ) -> core_events.SequentialEvent[core_events.SimpleEvent]:
-        duration = simple_event_to_convert.duration * self._factor
-        sequential_event = core_events.SequentialEvent(
+    ) -> core_events.Consecution[core_events.Chronon]:
+        duration = chronon_to_convert.duration * self._factor
+        consecution = core_events.Consecution(
             [
-                simple_event_to_convert.set_parameter(
-                    "duration", duration, mutate=False
-                ),
-                core_events.SimpleEvent(duration),
+                chronon_to_convert.copy().set_parameter("duration", duration),
+                core_events.Chronon(duration),
             ]
         )
-        return sequential_event
+        return consecution
 
     @property
     def playing_indicator_name(self) -> str:
         return "articulation"
 
     @property
     def default_playing_indicator(self) -> music_parameters.abc.PlayingIndicator:
         return music_parameters.Articulation()
 
 
 class ArticulationConverter(PlayingIndicatorConverter):
-    """Apply articulation on :class:`~mutwo.core_events.SimpleEvent`.
+    """Apply articulation on :class:`~mutwo.core_events.Chronon`.
 
     :param articulation_name_tuple_to_playing_indicator_converter:
     :type articulation_name_tuple_to_playing_indicator_converter: dict[tuple[str, ...], PlayingIndicatorConverter]
-    :param simple_event_to_playing_indicator_collection: Function to extract from a
-        :class:`mutwo.core_events.SimpleEvent` a
+    :param chronon_to_playing_indicator_collection: Function to extract from a
+        :class:`mutwo.core_events.Chronon` a
         :class:`mutwo.music_parameters.PlayingIndicatorCollection`
         object. By default it asks the Event for its
         :attr:`~mutwo.music_events.NoteLike.playing_indicator_collection`
         attribute (because by default :class:`mutwo.music_events.NoteLike`
         objects are expected).
         When using different Event classes than :class:`~mutwo.music_events.NoteLike`
         with a different name for their playing_indicator_collection property, this argument
         should be overridden. If the
         function call raises an :obj:`AttributeError` (e.g. if no playing indicator
         collection can be extracted), mutwo will build a playing indicator collection
         from :const:`~mutwo.music_events.configurations.DEFAULT_PLAYING_INDICATORS_COLLECTION_CLASS`.
-    :type simple_event_to_playing_indicator_collection: typing.Callable[[core_events.SimpleEvent], music_parameters.PlayingIndicatorCollection,], optional
+    :type chronon_to_playing_indicator_collection: typing.Callable[[core_events.Chronon], music_parameters.PlayingIndicatorCollection,], optional
     """
 
     def __init__(
         self,
         articulation_name_tuple_to_playing_indicator_converter: dict[
             tuple[str, ...], PlayingIndicatorConverter
         ] = {("staccato", "."): StacattoConverter()},
-        simple_event_to_playing_indicator_collection: typing.Callable[
-            [core_events.SimpleEvent],
+        chronon_to_playing_indicator_collection: typing.Callable[
+            [core_events.Chronon],
             music_parameters.PlayingIndicatorCollection,
-        ] = music_converters.SimpleEventToPlayingIndicatorCollection(),
+        ] = music_converters.ChrononToPlayingIndicatorCollection(),
     ):
-        self._logger = core_utilities.get_cls_logger(type(self))
         articulation_name_to_playing_indicator_converter = {}
         for (
             articulation_name_tuple,
             playing_indicator_converter,
         ) in articulation_name_tuple_to_playing_indicator_converter.items():
             for articulation_name in articulation_name_tuple:
                 if (
@@ -338,232 +327,228 @@
                 articulation_name_to_playing_indicator_converter.update(
                     {articulation_name: playing_indicator_converter}
                 )
 
         self._articulation_name_to_playing_indicator_converter = (
             articulation_name_to_playing_indicator_converter
         )
-        super().__init__(simple_event_to_playing_indicator_collection)
+        super().__init__(chronon_to_playing_indicator_collection)
 
     def _apply_playing_indicator(
         self,
-        simple_event_to_convert: core_events.SimpleEvent,
+        chronon_to_convert: core_events.Chronon,
         playing_indicator: music_parameters.Articulation,
-    ) -> core_events.SequentialEvent[core_events.SimpleEvent]:
+    ) -> core_events.Consecution[core_events.Chronon]:
         if (
             playing_indicator.name
             in self._articulation_name_to_playing_indicator_converter
         ):
             return self._articulation_name_to_playing_indicator_converter[
                 playing_indicator.name
-            ].convert(simple_event_to_convert)
+            ].convert(chronon_to_convert)
         else:
-            return core_events.SequentialEvent([copy.deepcopy(simple_event_to_convert)])
+            return core_events.Consecution([copy.deepcopy(chronon_to_convert)])
 
     @property
     def playing_indicator_name(self) -> str:
         return "articulation"
 
     @property
     def default_playing_indicator(self) -> music_parameters.abc.PlayingIndicator:
         return music_parameters.Articulation()
 
 
 class TrillConverter(PlayingIndicatorConverter):
-    """Apply trill on :class:`~mutwo.core_events.SimpleEvent`.
+    """Apply trill on :class:`~mutwo.core_events.Chronon`.
 
     :param trill_size:
-    :type trill_size: constants.DurationType
-    :param simple_event_to_pitch_list: Function to extract from a
-        :class:`mutwo.core_events.SimpleEvent` a tuple that contains pitch objects
+    :type trill_size: core_parameters.abc.Duration.Type
+    :param chronon_to_pitch_list: Function to extract from a
+        :class:`mutwo.core_events.Chronon` a tuple that contains pitch objects
         (objects that inherit from :class:`mutwo.music_parameters.abc.Pitch`).
         By default it asks the Event for its
         :attr:`~mutwo.music_events.NoteLike.pitch_list` attribute
         (because by default :class:`mutwo.music_events.NoteLike` objects are expected).
         When using different Event classes than :class:`~mutwo.music_events.NoteLike`
         with a different name for their pitch property, this argument
         should be overridden.
         If the function call raises an :obj:`AttributeError` (e.g. if no pitch can be
         extracted), mutwo will assume an event without any pitches.
-    :type simple_event_to_pitch_list: typing.Callable[[core_events.SimpleEvent], music_parameters.abc.Pitch], optional
-    :param simple_event_to_playing_indicator_collection: Function to extract from a
-        :class:`mutwo.core_events.SimpleEvent` a
+    :type chronon_to_pitch_list: typing.Callable[[core_events.Chronon], music_parameters.abc.Pitch], optional
+    :param chronon_to_playing_indicator_collection: Function to extract from a
+        :class:`mutwo.core_events.Chronon` a
         :class:`mutwo.music_parameters.PlayingIndicatorCollection`
         object. By default it asks the Event for its
         :attr:`~mutwo.music_events.NoteLike.playing_indicator_collection`
         attribute (because by default :class:`mutwo.music_events.NoteLike`
         objects are expected).
         When using different Event classes than :class:`~mutwo.music_events.NoteLike`
         with a different name for their playing_indicator_collection property, this argument
         should be overridden. If the
         function call raises an :obj:`AttributeError` (e.g. if no playing indicator
         collection can be extracted), mutwo will build a playing indicator collection
         from :const:`~mutwo.music_events.configurations.DEFAULT_PLAYING_INDICATORS_COLLECTION_CLASS`.
-    :type simple_event_to_playing_indicator_collection: typing.Callable[[core_events.SimpleEvent], music_parameters.PlayingIndicatorCollection,], optional
+    :type chronon_to_playing_indicator_collection: typing.Callable[[core_events.Chronon], music_parameters.PlayingIndicatorCollection,], optional
     """
 
     def __init__(
         self,
-        trill_size: core_constants.DurationType = fractions.Fraction(1, 16),
-        simple_event_to_pitch_list: typing.Callable[
-            [core_events.SimpleEvent], list[music_parameters.abc.Pitch]
-        ] = music_converters.SimpleEventToPitchList(),
-        simple_event_to_playing_indicator_collection: typing.Callable[
-            [core_events.SimpleEvent],
+        trill_size: core_parameters.abc.Duration.Type = fractions.Fraction(1, 16),
+        chronon_to_pitch_list: typing.Callable[
+            [core_events.Chronon], list[music_parameters.abc.Pitch]
+        ] = music_converters.ChrononToPitchList(),
+        chronon_to_playing_indicator_collection: typing.Callable[
+            [core_events.Chronon],
             music_parameters.PlayingIndicatorCollection,
-        ] = music_converters.SimpleEventToPlayingIndicatorCollection(),
+        ] = music_converters.ChrononToPlayingIndicatorCollection(),
     ):
-        self._trill_size = trill_size
-        self._simple_event_to_pitch_list = simple_event_to_pitch_list
-        super().__init__(simple_event_to_playing_indicator_collection)
+        self._trill_size = core_parameters.abc.Duration.from_any(trill_size)
+        self._chronon_to_pitch_list = chronon_to_pitch_list
+        super().__init__(chronon_to_playing_indicator_collection)
 
     def _apply_trill(
         self,
-        simple_event_to_convert: core_events.SimpleEvent,
+        chronon_to_convert: core_events.Chronon,
         trill: music_parameters.Trill,
         pitch_list: list[music_parameters.abc.Pitch],
-    ) -> core_events.SequentialEvent[core_events.SimpleEvent]:
-        trill_item_count = simple_event_to_convert.duration // self._trill_size
-        remaining = simple_event_to_convert.duration - (
-            trill_item_count * self._trill_size
-        )
-        sequential_event = core_events.SequentialEvent([])
+    ) -> core_events.Consecution[core_events.Chronon]:
+        trill_item_count = chronon_to_convert.duration // self._trill_size
+        remaining = chronon_to_convert.duration - (trill_item_count * self._trill_size)
+        consecution = core_events.Consecution([])
         pitch_cycle = itertools.cycle((pitch_list, trill.pitch))
         for _ in range(int(trill_item_count)):
-            simple_event = simple_event_to_convert.set_parameter(
-                "duration", self._trill_size, mutate=False
-            ).set_parameter("pitch_list", next(pitch_cycle))
-            sequential_event.append(simple_event)
-        sequential_event[-1].duration += remaining
-        return sequential_event
+            chronon = (
+                chronon_to_convert.copy()
+                .set_parameter("duration", self._trill_size)
+                .set_parameter("pitch_list", next(pitch_cycle))
+            )
+            consecution.append(chronon)
+        consecution[-1].duration += remaining
+        return consecution
 
     def _apply_playing_indicator(
         self,
-        simple_event_to_convert: core_events.SimpleEvent,
+        chronon_to_convert: core_events.Chronon,
         playing_indicator: music_parameters.Trill,
-    ) -> core_events.SequentialEvent[core_events.SimpleEvent]:
-        pitch_list = self._simple_event_to_pitch_list(simple_event_to_convert)
+    ) -> core_events.Consecution[core_events.Chronon]:
+        pitch_list = self._chronon_to_pitch_list(chronon_to_convert)
         if pitch_list:
-            return self._apply_trill(
-                simple_event_to_convert, playing_indicator, pitch_list
-            )
+            return self._apply_trill(chronon_to_convert, playing_indicator, pitch_list)
         else:
-            return core_events.SequentialEvent([copy.copy(simple_event_to_convert)])
+            return core_events.Consecution([copy.copy(chronon_to_convert)])
 
     @property
     def playing_indicator_name(self) -> str:
         return "trill"
 
     @property
     def default_playing_indicator(self) -> music_parameters.abc.PlayingIndicator:
         return music_parameters.Trill()
 
 
 class OptionalConverter(PlayingIndicatorConverter):
-    """Apply optional on :class:`~mutwo.core_events.SimpleEvent`.
+    """Apply optional on :class:`~mutwo.core_events.Chronon`.
 
     :param likelihood: A number between 0 - 1. 1 means that each optional
         note is played, 0 means no optional note is played. Default to 0.5.
     :type likelihood: float
     :param random_seed: Set inner random process. Default to 100.
     :type random_seed: int
-    :param make_rest: A function which takes the original :class:`~mutwo.core_events.SimpleEvent`
-        and returns a new `SimpleEvent` with the same duration which represents a rest.
-        By default, `mutwo` simply creates a `SimpleEvent` with the same duration.
-    :type make_rest: typing.Callable[[core_events.SimpleEvent], core_events.SimpleEvent]
-    :param simple_event_to_playing_indicator_collection: Function to extract from a
-        :class:`mutwo.core_events.SimpleEvent` a
+    :param make_rest: A function which takes the original :class:`~mutwo.core_events.Chronon`
+        and returns a new `Chronon` with the same duration which represents a rest.
+        By default, `mutwo` simply creates a `Chronon` with the same duration.
+    :type make_rest: typing.Callable[[core_events.Chronon], core_events.Chronon]
+    :param chronon_to_playing_indicator_collection: Function to extract from a
+        :class:`mutwo.core_events.Chronon` a
         :class:`mutwo.music_parameters.PlayingIndicatorCollection`
         object. By default it asks the Event for its
         :attr:`~mutwo.music_events.NoteLike.playing_indicator_collection`
         attribute (because by default :class:`mutwo.music_events.NoteLike`
         objects are expected).
         When using different Event classes than :class:`~mutwo.music_events.NoteLike`
         with a different name for their playing_indicator_collection property, this argument
         should be overridden. If the
         function call raises an :obj:`AttributeError` (e.g. if no playing indicator
         collection can be extracted), mutwo will build a playing indicator collection
         from :const:`~mutwo.music_events.configurations.DEFAULT_PLAYING_INDICATORS_COLLECTION_CLASS`.
-    :type simple_event_to_playing_indicator_collection: typing.Callable[[core_events.SimpleEvent], music_parameters.PlayingIndicatorCollection,], optional
+    :type chronon_to_playing_indicator_collection: typing.Callable[[core_events.Chronon], music_parameters.PlayingIndicatorCollection,], optional
     """
 
     def __init__(
         self,
         likelihood: float = 0.5,
         random_seed: int = 100,
         make_rest: typing.Callable[
-            [core_events.SimpleEvent], core_events.SimpleEvent
-        ] = lambda simple_event: core_events.SimpleEvent(simple_event.duration),
-        simple_event_to_playing_indicator_collection: typing.Callable[
-            [core_events.SimpleEvent],
+            [core_events.Chronon], core_events.Chronon
+        ] = lambda chronon: core_events.Chronon(chronon.duration),
+        chronon_to_playing_indicator_collection: typing.Callable[
+            [core_events.Chronon],
             music_parameters.PlayingIndicatorCollection,
-        ] = music_converters.SimpleEventToPlayingIndicatorCollection(),
+        ] = music_converters.ChrononToPlayingIndicatorCollection(),
     ):
         self._make_rest = make_rest
         self._likelihood = likelihood
         self._random = random.Random(random_seed)
-        super().__init__(simple_event_to_playing_indicator_collection)
+        super().__init__(chronon_to_playing_indicator_collection)
 
     def _apply_playing_indicator(
         self,
-        simple_event_to_convert: core_events.SimpleEvent,
+        chronon_to_convert: core_events.Chronon,
         playing_indicator: music_parameters.abc.ExplicitPlayingIndicator,
-    ) -> core_events.SequentialEvent[core_events.SimpleEvent]:
-        sequential_event = core_events.SequentialEvent([])
+    ) -> core_events.Consecution[core_events.Chronon]:
+        consecution = core_events.Consecution([])
         if playing_indicator.is_active and self._random.random() > self._likelihood:
-            rest = self._make_rest(simple_event_to_convert)
-            sequential_event.append(rest)
+            rest = self._make_rest(chronon_to_convert)
+            consecution.append(rest)
         else:
-            sequential_event.append(simple_event_to_convert.copy())
-        return sequential_event
+            consecution.append(chronon_to_convert.copy())
+        return consecution
 
     @property
     def playing_indicator_name(self) -> str:
         return "optional"
 
     @property
     def default_playing_indicator(self) -> music_parameters.abc.PlayingIndicator:
         return music_parameters.abc.ExplicitPlayingIndicator()
 
 
 class PlayingIndicatorsConverter(core_converters.abc.SymmetricalEventConverter):
     """Apply :class:`mutwo.music_parameters.abc.PlayingIndicator` on any :class:`~mutwo.core_events.abc.Event`.
 
     :param playing_indicator_converter_sequence: A sequence of :class:`PlayingIndicatorConverter` which shall
-        be applied on each :class:`~mutwo.core_events.SimpleEvent`.
+        be applied on each :class:`~mutwo.core_events.Chronon`.
     :type playing_indicator_converter_sequence: typing.Sequence[PlayingIndicatorConverter]
     """
 
     def __init__(
         self,
         playing_indicator_converter_sequence: typing.Sequence[
             PlayingIndicatorConverter
         ],
     ):
         self._playing_indicator_converter_tuple = tuple(
             playing_indicator_converter_sequence
         )
 
-    def _convert_simple_event(
+    def _convert_chronon(
         self,
-        event_to_convert: core_events.SimpleEvent,
-        _: core_constants.DurationType,
-    ) -> core_events.SequentialEvent:
-        """Convert instance of :class:`mutwo.core_events.SimpleEvent`."""
+        event_to_convert: core_events.Chronon,
+        _: core_parameters.abc.Duration.Type,
+    ) -> core_events.Consecution:
+        """Convert instance of :class:`mutwo.core_events.Chronon`."""
 
         converted_event = [event_to_convert]
 
         for playing_indicator_converter in self._playing_indicator_converter_tuple:
-            new_converted_event: list[core_events.SimpleEvent] = []
-            for simple_event in converted_event:
-                converted_simple_event = playing_indicator_converter.convert(
-                    simple_event
-                )
-                new_converted_event.extend(converted_simple_event)
+            new_converted_event: list[core_events.Chronon] = []
+            for chronon in converted_event:
+                converted_chronon = playing_indicator_converter.convert(chronon)
+                new_converted_event.extend(converted_chronon)
 
             converted_event = new_converted_event
 
-        return core_events.SequentialEvent(converted_event)
+        return core_events.Consecution(converted_event)
 
     def convert(self, event_to_convert: core_events.abc.Event) -> core_events.abc.Event:
         converted_event = self._convert_event(event_to_convert, 0)
         return converted_event
```

### Comparing `mutwo.music-0.26.1/mutwo/music_converters/spectrals.py` & `mutwo_music-0.27.0/mutwo/music_converters/spectrals.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.1/mutwo/music_events/configurations.py` & `mutwo_music-0.27.0/mutwo/music_parameters/playing_indicators.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,229 +1,239 @@
-"""Set default values for :class:`mutwo.music_events.NoteLike`."""
+"""Define playing indicators for chronons.
 
-import fractions
-import numbers
-import typing
+This submodules provides several classes to add specific musical
+playing techniques to :class:`mutwo.core_events.Chronon` objects.
+They mostly derive from traditional Western playing techniques and their
+notation. Unlike indicators of the :mod:`mutwo.music_parameters.notation_indicators`
+module, playing indicators have an effect on the played music and aren't
+merely specifications of representation. The proper way to handle
+playing  indicators should be via a :class:`PlayingIndicatorCollection`
+object that should be attached to the respective :class:`Chronon`.
+The collection contains all possible playing indicators which are defined
+in this module. :class:`mutwo.music_events.NoteLike` contain by default
+a playing indicator collection.
+
+There are basically two different types of playing indicators:
+
+1, Playing indicators which can only be on or off (for instance
+``bartok_pizzicato``, ``prall`` or ``laissez_vibrer``). They have
+a :attr:`is_active` attribute which can either be :obj:`True`
+or :obj:`False`.
+
+2. Playing indicators with one or more arguments (for instance
+:class:`Tremolo` with :attr:`flag_count` or :class:`Arpeggio` with
+:attr:`direction`). Their :attr:`is_active` attribute can't be
+set by the user and get automatically initialised depending on
+if all necessary attributes are defined (then active) or
+if any of the necessary attributes is set to :obj:`None` (then
+not active).
+
+**Example:**
+
+Set playing indicators of :class:`NoteLike`:
+
+>>> from mutwo import music_events
+>>> my_note = music_events.NoteLike('c', 1 / 4, 'mf')
+>>> my_note.playing_indicator_collection.articulation.name = "."  # add staccato
+>>> my_chord = music_events.NoteLike('c e g', 1 / 2, 'f')
+>>> my_chord.playing_indicator_collection.arpeggio.direction= "up"  # add arpeggio
+>>> my_chord.playing_indicator_collection.laissez_vibrer = True  # and laissez_vibrer
+
+Attach :class:`PlayingIndicatorCollection` to :class:`Chronon`:
+
+>>> from mutwo import core_events
+>>> from mutwo import music_parameters
+>>> my_chronon = core_events.Chronon(1)
+>>> my_chronon.playing_indicator_collection = music_parameters.PlayingIndicatorCollection()
+"""
 
-try:
-    import quicktions
-except ImportError:
-    quicktions = fractions
+import dataclasses
+import inspect
+import typing
 
-from mutwo import core_events
 from mutwo import music_parameters
-from mutwo import music_utilities
 
-DEFAULT_PLAYING_INDICATORS_COLLECTION_CLASS = (
-    music_parameters.PlayingIndicatorCollection
-)
-"""Default value for :attr:`mutwo.music_events.NoteLike.playing_indicator_collection`
-in :class:`~mutwo.music_events.NoteLike`"""
-
-DEFAULT_NOTATION_INDICATORS_COLLECTION_CLASS = (
-    music_parameters.NotationIndicatorCollection
-)
-"""Default value for :attr:`mutwo.music_events.NoteLike.notation_indicator_collection`
-in :class:`~mutwo.music_events.NoteLike`"""
-
-
-_indicator_collection_parser = music_utilities.IndicatorCollectionParser()
-
-
-def _unknown_object_to_playing_indicator_collection(
-    unknown_object: typing.Any,
-) -> list[music_parameters.PlayingIndicatorCollection]:
-    match unknown_object:
-        case None:
-            return DEFAULT_PLAYING_INDICATORS_COLLECTION_CLASS()
-        case music_parameters.PlayingIndicatorCollection():
-            return unknown_object
-        case str():
-            return _indicator_collection_parser.parse(
-                unknown_object, DEFAULT_PLAYING_INDICATORS_COLLECTION_CLASS()
-            )
-        case _:
-            raise NotImplementedError(
-                f"Can't build PlayingIndicatorCollection from '{unknown_object}'"
-            )
-
-
-UNKNOWN_OBJECT_TO_PLAYING_INDICATOR_COLLECTION = (
-    _unknown_object_to_playing_indicator_collection
-)
-"""This function is called whenever an object is assigned to
-the `playing_indicator_collection` property of :class:`mutwo.music_events.NoteLike`.
-The function is called on the object which is tried to be assigned
-to the `playing_indicator_collection` property. The function tries to return an instance
-of :class:`mutwo.music_parameters.PlayingIndicatorCollection` or an instance
-of any child class. The aim of this function is to allow syntactic
-sugar.
-"""
 
+class PlayingIndicatorCollection(
+    music_parameters.abc.IndicatorCollection[music_parameters.abc.PlayingIndicator]
+):
+    """Collection of playing indicators"""
 
-def _unknown_object_to_notation_indicator_collection(
-    unknown_object: typing.Any,
-) -> list[music_parameters.NotationIndicatorCollection]:
-    match unknown_object:
-        case None:
-            return DEFAULT_NOTATION_INDICATORS_COLLECTION_CLASS()
-        case music_parameters.NotationIndicatorCollection():
-            return unknown_object
-        case str():
-            return _indicator_collection_parser.parse(
-                unknown_object, DEFAULT_NOTATION_INDICATORS_COLLECTION_CLASS()
-            )
-        case _:
-            raise NotImplementedError(
-                f"Can't build NotationIndicatorCollection from '{unknown_object}'"
-            )
-
-
-UNKNOWN_OBJECT_TO_NOTATION_INDICATOR_COLLECTION = (
-    _unknown_object_to_notation_indicator_collection
-)
-"""This function is called when any object is assigned to
-the `notation_indicator_collection` property of :class:`mutwo.music_events.NoteLike`.
-The function is called on the object which is tried to be assigned
-to the `notation_indicator_collection` property. The function tries to return an instance
-of :class:`mutwo.music_parameters.NotationIndicatorCollection` or an instance
-of any child class. The aim of this function is to allow syntactic
-sugar.
-"""
+    def __setattr__(self, parameter_name: str, value: bool):
+        """Overriding default behaviour to allow syntactic sugar.
+
+        This method allows syntax like:
+
+            playing_indicator_collection.tie = True
+
+        which is the same as
+
+            playing_indicator_collection.tie.is_active = True
+
+        Furthermore the methods makes sure that no property
+        can actually be overridden.
+        """
+        if (playing_indicator := getattr(self, parameter_name, None)) is not None:
+            if isinstance(
+                playing_indicator, music_parameters.abc.ExplicitPlayingIndicator
+            ):
+                playing_indicator.is_active = bool(value)
+                return
+        super().__setattr__(parameter_name, value)
+
+
+r = PlayingIndicatorCollection.register
+
+# Add explicit playing indicators
+for exp in (
+    "bartok_pizzicato",
+    "breath_mark",
+    "duration_line_dashed",
+    "duration_line_triller",
+    "flageolet",
+    "glissando",
+    "laissez_vibrer",
+    "optional",
+    "prall",
+    "tie",
+):
+    r(music_parameters.abc.ExplicitPlayingIndicator, exp)
+del exp
+
+
+implicit = lambda cls: r(dataclasses.dataclass()(cls))
+
+
+# Add implicit playing indicators
+@implicit
+class Tremolo(music_parameters.abc.ImplicitPlayingIndicator):
+    flag_count: typing.Optional[int] = None
+
+
+@implicit
+class Articulation(music_parameters.abc.ImplicitPlayingIndicator):
+    name: typing.Optional[music_parameters.constants.ARTICULATION_LITERAL] = None
+
+
+@implicit
+class Arpeggio(music_parameters.abc.ImplicitPlayingIndicator):
+    direction: typing.Optional[music_parameters.constants.DIRECTION_LITERAL] = None
+
+
+@implicit
+class Pedal(music_parameters.abc.ImplicitPlayingIndicator):
+    type: typing.Optional[music_parameters.constants.PEDAL_TYPE_LITERAL] = None
+    activity: typing.Optional[bool] = True
 
 
-def _unknown_object_to_pitch_list(
-    unknown_object: typing.Any,
-) -> list[music_parameters.abc.Pitch]:
-    match unknown_object:
-        case None:
-            pitch_list = []
-        case music_parameters.abc.Pitch():
-            pitch_list = [unknown_object]
-        case str():
-            pitch_list = [
-                _string_to_pitch(pitch_indication)
-                for pitch_indication in unknown_object.split(" ")
-                if pitch_indication
-            ]
-        case fractions.Fraction() | quicktions.Fraction():
-            pitch_list = [music_parameters.JustIntonationPitch(unknown_object)]
-        case float() | int():
-            pitch_list = [music_parameters.WesternPitch(unknown_object)]
-        case _:
-            raise NotImplementedError(
-                f"Can't build pitch object from object '{unknown_object}' "
-                f"of type '{type(unknown_object)}'."
-            )
-
-    return pitch_list
-
-
-def _string_to_pitch(pitch_indication: str) -> music_parameters.abc.Pitch:
-    # assumes it is a ratio
-    if "/" in pitch_indication:
-        return music_parameters.JustIntonationPitch(pitch_indication)
-
-    # assumes it is a WesternPitch name
-    elif (
-        pitch_indication[0] in music_parameters.constants.DIATONIC_PITCH_CLASS_CONTAINER
+@implicit
+class Slur(music_parameters.abc.ImplicitPlayingIndicator):
+    activity: typing.Optional[bool] = None
+
+
+@implicit
+class StringContactPoint(music_parameters.abc.ImplicitPlayingIndicator):
+    contact_point: typing.Optional[
+        music_parameters.constants.CONTACT_POINT_LITERAL
+    ] = None
+
+
+@implicit
+class Ornamentation(music_parameters.abc.ImplicitPlayingIndicator):
+    direction: typing.Optional[music_parameters.constants.DIRECTION_LITERAL] = None
+    count: int = 1
+
+
+@implicit
+class BendAfter(music_parameters.abc.ImplicitPlayingIndicator):
+    # Content music_parameters
+    bend_amount: typing.Optional[float] = None
+    # Presentation music_parameters
+    minimum_length: typing.Optional[float] = 3
+    thickness: typing.Optional[float] = 3
+
+
+@implicit
+class ArtificalHarmonic(music_parameters.abc.ImplicitPlayingIndicator):
+    semitone_count: typing.Optional[int] = None
+
+
+@implicit
+class NaturalHarmonicNodeList(
+    list[music_parameters.NaturalHarmonic.Node], music_parameters.abc.PlayingIndicator
+):
+    """Assign natural harmonics to your note.
+
+    **Example:**
+
+    >>> from mutwo import music_events, music_parameters
+    >>> n = music_events.NoteLike('c', 4)
+    >>> n.playing_indicator_collection.natural_harmonic_node_list.is_active
+    False
+    >>> n.playing_indicator_collection.natural_harmonic_node_list.append(
+    ...     music_parameters.NaturalHarmonic(
+    ...         2,
+    ...         music_parameters.String(0, music_parameters.WesternPitch('c', 3))
+    ...     ).node_tuple[0]
+    ... )
+    >>> n.playing_indicator_collection.natural_harmonic_node_list.is_active
+    True
+    """
+
+    def __new__(
+        self,
+        natural_harmonic_list: typing.Optional[
+            list[music_parameters.NaturalHarmonic.Node]
+        ] = None,
+        harmonic_note_head_style: bool = True,
+        write_string: bool = True,
+        parenthesize_lower_note_head: bool = False,
     ):
-        if pitch_indication[-1].isdigit():
-            pitch_name, octave = pitch_indication[:-1], int(pitch_indication[-1])
-            pitch = music_parameters.WesternPitch(pitch_name, octave)
-        else:
-            pitch = music_parameters.WesternPitch(pitch_indication)
-
-        return pitch
-
-    else:
-        raise NotImplementedError(
-            f"Can't build pitch from pitch_indication '{pitch_indication}'."
-            " Supported string formats are (1) ratios divided by a forward "
-            "slash (for instance '3/2' or '4/3') and (2) names of western "
-            "pitch classes with an optional number to indicate the octave "
-            "(for instance 'c4', 'as' or 'fqs2')."
-        )
-
-
-UNKNOWN_OBJECT_TO_PITCH_LIST = _unknown_object_to_pitch_list
-"""This function converts any input parameter for the `pitch_list`
-property to a list of :class:`mutwo.music_parameters.abc.Pitch` objects.
-It is used inside :class:`mutwo.music_events.NoteLike` in order to allow
-syntactic sugar when parsing pitches to `NoteLike`. This functions
-allows the following syntax:
+        nhn_list = super().__new__(self, natural_harmonic_list or [])
+        nhn_list.write_string = write_string
+        nhn_list.harmonic_note_head_style = harmonic_note_head_style
+        nhn_list.parenthesize_lower_note_head = parenthesize_lower_note_head
+        return nhn_list
 
+    @property
+    def is_active(self) -> bool:
+        return bool(self)
 
-    >>> music_events.NoteLike('c d f') # or
-    >>> music_events.NoteLike('3/2')
 
-It can be overridden by the user if desired.
-"""
+@implicit
+class Fermata(music_parameters.abc.ImplicitPlayingIndicator):
+    type: typing.Optional[music_parameters.constants.FERMATA_TYPE_LITERAL] = None
+
+
+@implicit
+class Hairpin(music_parameters.abc.ImplicitPlayingIndicator):
+    symbol: typing.Optional[music_parameters.constants.HAIRPIN_SYMBOL_LITERAL] = None
+    niente: bool = False
+
+
+@implicit
+class Trill(music_parameters.abc.ImplicitPlayingIndicator):
+    pitch: typing.Optional[music_parameters.abc.Pitch] = None
+
+
+@implicit
+class WoodwindFingering(music_parameters.abc.ImplicitPlayingIndicator):
+    cc: typing.Optional[typing.Tuple[str, ...]] = None
+    left_hand: typing.Optional[typing.Tuple[str, ...]] = None
+    right_hand: typing.Optional[typing.Tuple[str, ...]] = None
+    instrument: str = "clarinet"
+
+
+@implicit
+class Cue(music_parameters.abc.ImplicitPlayingIndicator):
+    """Cue for electronics etc."""
+
+    index: typing.Optional[int] = None
 
 
-def _unknown_object_to_volume(volume: typing.Any) -> music_parameters.abc.Volume:
-    match volume:
-        case music_parameters.abc.Volume():
-            volume = volume
-        case numbers.Real():
-            if volume >= 0:  # type: ignore
-                volume = music_parameters.DirectVolume(volume)  # type: ignore
-            else:
-                volume = music_parameters.DecibelVolume(volume)  # type: ignore
-        case str():
-            volume = music_parameters.WesternVolume(volume)
-        case _:
-            raise TypeError(
-                "Can't initialise '{}' with value '{}' of type '{}' for argument"
-                " 'volume'. The type for 'volume' should be '{}'.".format(
-                    type(self).__name__, volume, type(volume), Volume
-                )
-            )
-    return volume
-
-
-UNKNOWN_OBJECT_TO_VOLUME = _unknown_object_to_volume
-"""This function is called when any object is assigned to
-the `volume` property of :class:`mutwo.music_events.NoteLike`.
-The function is called on the object which is tried to be assigned
-to the volume property. The function tries to return an instance
-of :class:`mutwo.music_parameters.abc.Volume` or an instance
-of any child class. The aim of this function is to allow syntactic
-sugar to the user. For instance consider the following:
-
-
-    >>> music_events.NoteLike('3/2', 'p')
-
-Here the volume property is 'p'. This is merely a string and
-not a volume object. The function `UNKNOWN_OBJECT_TO_VOLUME`
-automatically converts the string 'p' to
-`music_parameters.WesternVolume('p')`. User can override the
-default conversion routine.
-
-You can compare `mutwo.core_events.UNKNOWN_OBJECT_TO_DURATION`
-and `UNKNOWN_OBJECT_TO_PITCH` and
-`UNKNOWN_OBJECT_TO_GRACE_NOTE_SEQUENTIAL_EVENT` for similar
-functions."""
-
-
-GraceNotes = core_events.SequentialEvent[core_events.SimpleEvent]
-
-
-def _unknown_object_to_grace_note_sequential_event(
-    unknown_object: GraceNotes | core_events.SimpleEvent,
-) -> GraceNotes:
-    match unknown_object:
-        case core_events.SimpleEvent():
-            return core_events.SequentialEvent([unknown_object])
-        case core_events.SequentialEvent():
-            return unknown_object
-        case _:
-            raise TypeError(f"Can't set grace notes to {unknown_object}")
-
-
-UNKNOWN_OBJECT_TO_GRACE_NOTE_SEQUENTIAL_EVENT = (
-    _unknown_object_to_grace_note_sequential_event
-)
-"""Convert any object to a :class:`mutwo.core_events.SequentialEvent`.
-This function is used inside :class:`mutwo.music_events.NoteLike`. It
-helps to allow syntactic sugar and raises errors for unsupported types.
-It can be overridden by the user."""
+# Dynamically define __all__ in order to catch all PlayingIndicator classes
+__all__ = tuple(
+    name
+    for name, cls in globals().items()
+    if inspect.isclass(cls)
+    and music_parameters.abc.PlayingIndicator in inspect.getmro(cls)
+) + ("PlayingIndicatorCollection",)
```

### Comparing `mutwo.music-0.26.1/mutwo/music_generators/constants.py` & `mutwo_music-0.27.0/mutwo/music_generators/constants.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.1/mutwo/music_parameters/__init__.py` & `mutwo_music-0.27.0/mutwo/music_parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.1/mutwo/music_parameters/abc.py` & `mutwo_music-0.27.0/mutwo/music_parameters/abc.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,25 +11,30 @@
 from __future__ import annotations
 
 import abc
 import copy
 import dataclasses
 import functools
 import math
+import numbers
+import types
 import typing
 
 try:
     import quicktions as fractions  # type: ignore
 except ImportError:
     import fractions  # type: ignore
 
+    _fractions = None
+else:
+    import fractions as _fractions
+
 import ranges
 
 from mutwo import core_constants
-from mutwo import core_events
 from mutwo import core_parameters
 from mutwo import core_utilities
 from mutwo import music_parameters
 
 __all__ = (
     "PitchInterval",
     "Pitch",
@@ -42,268 +47,61 @@
     "Instrument",
     "PitchedInstrument",
 )
 
 
 class PitchInterval(
     core_parameters.abc.SingleNumberParameter,
-    value_name="interval",
+    value_name="cents",
     value_return_type=float,
 ):
     """Abstract base class for any pitch interval class
 
     If the user wants to define a new pitch interval class, the abstract
-    property :attr:`interval` and the abstract method `inverse`
+    property :attr:`cents` and the abstract method `inverse`
     have to be overridden.
 
-    :attr:`interval` is stored in unit `cents`.
-
     See `wikipedia entry <https://en.wikipedia.org/wiki/Cent_(music)>`_
     for definition of 'cents'.
     """
 
     def __repr__(self) -> str:
         return str(self)
 
     @abc.abstractmethod
-    def inverse(self, mutate: bool = False) -> PitchInterval:
+    def inverse(self) -> PitchInterval:
         """Makes falling interval to rising and vice versa.
 
         In `music21` the method for equal semantics is called
         `reverse <https://web.mit.edu/music21/doc/moduleReference/moduleInterval.html#music21.interval.Interval.reverse>`_.
         """
 
     def __add__(self, other: PitchInterval) -> PitchInterval:
-        return music_parameters.DirectPitchInterval(self.interval + other.interval)
+        return music_parameters.DirectPitchInterval(self.cents + other.cents)
 
     def __sub__(self, other: PitchInterval) -> PitchInterval:
-        return music_parameters.DirectPitchInterval(self.interval - other.interval)
+        return music_parameters.DirectPitchInterval(self.cents - other.cents)
 
 
 class Pitch(
     core_parameters.abc.SingleNumberParameter,
-    core_parameters.abc.ParameterWithEnvelope,
-    value_name="frequency",
+    value_name="hertz",
     value_return_type=float,
 ):
     """Abstract base class for any pitch class.
 
     If the user wants to define a new pitch class, the abstract
-    property :attr:`frequency` has to be overridden. Starting
+    property :attr:`hertz` has to be overridden. Starting
     from mutwo version = 0.46.0 the user will furthermore have
     to define an :func:`add` method.
     """
 
-    class PitchEnvelope(core_events.Envelope):
-        """Default resolution envelope class for :class:`Pitch`"""
-
-        def __init__(
-            self,
-            *args,
-            event_to_parameter: typing.Optional[
-                typing.Callable[[core_events.abc.Event], core_constants.ParameterType]
-            ] = None,
-            value_to_parameter: typing.Optional[
-                typing.Callable[
-                    [core_events.Envelope.Value], core_constants.ParameterType
-                ]
-            ] = None,
-            parameter_to_value: typing.Optional[
-                typing.Callable[
-                    [core_constants.ParameterType], core_events.Envelope.Value
-                ]
-            ] = None,
-            apply_parameter_on_event: typing.Optional[
-                typing.Callable[
-                    [core_events.abc.Event, core_constants.ParameterType], None
-                ]
-            ] = None,
-            **kwargs,
-        ):
-            event_to_parameter = event_to_parameter or self._event_to_parameter
-            value_to_parameter = value_to_parameter or self._value_to_parameter
-            apply_parameter_on_event = (
-                apply_parameter_on_event or self._apply_parameter_on_event
-            )
-            parameter_to_value = parameter_to_value or self._parameter_to_value
-
-            super().__init__(
-                *args,
-                event_to_parameter=event_to_parameter,
-                value_to_parameter=value_to_parameter,
-                parameter_to_value=parameter_to_value,
-                apply_parameter_on_event=apply_parameter_on_event,
-                **kwargs,
-            )
-
-        @classmethod
-        def frequency_and_envelope_to_pitch(
-            cls,
-            frequency: core_constants.Real,
-            envelope: typing.Optional[
-                Pitch.PitchIntervalEnvelope | typing.Sequence
-            ] = None,
-        ) -> Pitch:
-            return music_parameters.DirectPitch(frequency, envelope=envelope)
-
-        @classmethod
-        def _value_to_parameter(
-            cls,
-            value: core_events.Envelope.Value,  # type: ignore
-        ) -> core_constants.ParameterType:
-            # For inner calculation (value) cents are used instead
-            # of frequencies. In this way we can ensure that the transitions
-            # are closer to the human logarithmic hearing.
-            # See als `_parameter_to_value`.
-            frequency = (
-                Pitch.cents_to_ratio(value)
-                * music_parameters.constants.PITCH_ENVELOPE_REFERENCE_FREQUENCY
-            )
-            return cls.frequency_and_envelope_to_pitch(frequency)
-
-        @classmethod
-        def _event_to_parameter(
-            cls, event: core_events.abc.Event
-        ) -> core_constants.ParameterType:
-            if hasattr(
-                event,
-                music_parameters.configurations.DEFAULT_PITCH_ENVELOPE_PARAMETER_NAME,
-            ):
-                return getattr(
-                    event,
-                    music_parameters.configurations.DEFAULT_PITCH_ENVELOPE_PARAMETER_NAME,
-                )
-            else:
-                return cls.frequency_and_envelope_to_pitch(
-                    music_parameters.configurations.DEFAULT_CONCERT_PITCH
-                )
-
-        @classmethod
-        def _apply_parameter_on_event(
-            cls, event: core_events.abc.Event, parameter: core_constants.ParameterType
-        ):
-            setattr(
-                event,
-                music_parameters.configurations.DEFAULT_PITCH_ENVELOPE_PARAMETER_NAME,
-                parameter,
-            )
-
-        @classmethod
-        def _parameter_to_value(
-            cls, parameter: core_constants.ParameterType
-        ) -> core_constants.Real:
-            # For inner calculation (value) cents are used instead
-            # of frequencies. In this way we can ensure that the transitions
-            # are closer to the human logarithmic hearing.
-            # See als `_value_to_parameter`.
-            return Pitch.hertz_to_cents(
-                music_parameters.constants.PITCH_ENVELOPE_REFERENCE_FREQUENCY,
-                parameter.frequency,
-            )
-
-    class PitchIntervalEnvelope(core_events.RelativeEnvelope):
-        """Default envelope class for :class:`Pitch`
-
-        Resolves into :class:`Pitch.PitchEnvelope`.
-        """
-
-        def __init__(
-            self,
-            *args,
-            event_to_parameter: typing.Optional[
-                typing.Callable[[core_events.abc.Event], core_constants.ParameterType]
-            ] = None,
-            value_to_parameter: typing.Optional[
-                typing.Callable[
-                    [core_events.Envelope.Value], core_constants.ParameterType
-                ]
-            ] = None,
-            parameter_to_value: typing.Callable[
-                [core_constants.ParameterType], core_events.Envelope.Value
-            ] = lambda parameter: parameter.interval,
-            apply_parameter_on_event: typing.Optional[
-                typing.Callable[
-                    [core_events.abc.Event, core_constants.ParameterType], None
-                ]
-            ] = None,
-            base_parameter_and_relative_parameter_to_absolute_parameter: typing.Optional[
-                typing.Callable[
-                    [core_constants.ParameterType, core_constants.ParameterType],
-                    core_constants.ParameterType,
-                ]
-            ] = None,
-            **kwargs,
-        ):
-            if not event_to_parameter:
-                event_to_parameter = self._event_to_parameter
-            if not value_to_parameter:
-                value_to_parameter = self._value_to_parameter
-            if not apply_parameter_on_event:
-                apply_parameter_on_event = self._apply_parameter_on_event
-            if not base_parameter_and_relative_parameter_to_absolute_parameter:
-                base_parameter_and_relative_parameter_to_absolute_parameter = (
-                    self._base_parameter_and_relative_parameter_to_absolute_parameter
-                )
-
-            super().__init__(
-                *args,
-                event_to_parameter=event_to_parameter,
-                value_to_parameter=value_to_parameter,
-                parameter_to_value=parameter_to_value,
-                apply_parameter_on_event=apply_parameter_on_event,
-                base_parameter_and_relative_parameter_to_absolute_parameter=base_parameter_and_relative_parameter_to_absolute_parameter,
-                **kwargs,
-            )
-
-        @classmethod
-        def cents_to_pitch_interval(cls, cents: core_constants.Real) -> PitchInterval:
-            return music_parameters.DirectPitchInterval(cents)
-
-        @classmethod
-        def _event_to_parameter(
-            cls, event: core_events.abc.Event
-        ) -> core_constants.ParameterType:
-            if hasattr(
-                event,
-                music_parameters.configurations.DEFAULT_PITCH_INTERVAL_ENVELOPE_PARAMETER_NAME,
-            ):
-                return getattr(
-                    event,
-                    music_parameters.configurations.DEFAULT_PITCH_INTERVAL_ENVELOPE_PARAMETER_NAME,
-                )
-            else:
-                return cls.cents_to_pitch_interval(0)
-
-        @classmethod
-        def _value_to_parameter(
-            cls, value: core_events.Envelope.Value
-        ) -> core_constants.ParameterType:
-            return cls.cents_to_pitch_interval(value)
-
-        @classmethod
-        def _apply_parameter_on_event(
-            cls, event: core_events.abc.Event, parameter: core_constants.ParameterType
-        ):
-            setattr(
-                event,
-                music_parameters.configurations.DEFAULT_PITCH_INTERVAL_ENVELOPE_PARAMETER_NAME,
-                parameter,
-            ),
-
-        @classmethod
-        def _base_parameter_and_relative_parameter_to_absolute_parameter(
-            cls, base_parameter: Pitch, relative_parameter: PitchInterval
-        ) -> Pitch:
-            return base_parameter + relative_parameter
-
-    def __init__(
-        self,
-        envelope: typing.Optional[Pitch.PitchIntervalEnvelope | typing.Sequence] = None,
-    ):
-        self.envelope = envelope
+    Type: typing.TypeAlias = typing.Union[fractions.Fraction, float, int, str, "Pitch"]
+    """Pitch.Type hosts all types that are supported by the pitch parser
+    :func:`Pitch.from_any`."""
 
     # ###################################################################### #
     #     conversion methods between different pitch describing units        #
     # ###################################################################### #
 
     @staticmethod
     def hertz_to_cents(
@@ -382,101 +180,134 @@
         closest_midi_pitch_number = music_parameters.constants.MIDI_PITCH_NUMBER_TUPLE[
             closest_frequency_index
         ]
         difference_in_cents = Pitch.hertz_to_cents(frequency, closest_frequency)
         return float(closest_midi_pitch_number + (difference_in_cents / 100))
 
     # ###################################################################### #
+    #                            class methods                               #
+    # ###################################################################### #
+
+    @classmethod
+    def from_any(cls, object: Pitch.Type) -> Pitch:
+        builtin_fraction = _fractions.Fraction if _fractions else fractions.Fraction
+        match object:
+            case music_parameters.abc.Pitch():
+                return object
+            case str():
+                if "/" in object:  # assumes it is a ratio
+                    return music_parameters.JustIntonationPitch(object)
+                elif (  # assumes it is a WesternPitch name
+                    object[0]
+                    in music_parameters.constants.DIATONIC_PITCH_CLASS_CONTAINER
+                ):
+                    if object[-1].isdigit():
+                        pitch_name, octave = object[:-1], int(object[-1])
+                        return music_parameters.WesternPitch(pitch_name, octave)
+                    else:
+                        return music_parameters.WesternPitch(object)
+            case fractions.Fraction() | builtin_fraction():
+                return music_parameters.JustIntonationPitch(object)
+            case float() | int():
+                return music_parameters.WesternPitch(object)
+            case list() | tuple():
+                return music_parameters.FlexPitch(object)
+            case _:
+                pass
+
+        raise core_utilities.CannotParseError(object, cls)
+
+    # ###################################################################### #
     #                            public properties                           #
     # ###################################################################### #
 
     @property
     def midi_pitch_number(self) -> float:
         """The midi pitch number (from 0 to 127) of the pitch."""
-        return self.hertz_to_midi_pitch_number(self.frequency)
-
-    @core_parameters.abc.ParameterWithEnvelope.envelope.setter
-    def envelope(
-        self,
-        envelope_or_envelope_argument: typing.Optional[
-            Pitch.PitchIntervalEnvelope | typing.Sequence
-        ],
-    ):
-        if not envelope_or_envelope_argument:
-            generic_pitch_interval = self.PitchIntervalEnvelope.cents_to_pitch_interval(
-                0
-            )
-            envelope = self.PitchIntervalEnvelope([[0, generic_pitch_interval]])
-        elif isinstance(envelope_or_envelope_argument, core_events.RelativeEnvelope):
-            envelope = envelope_or_envelope_argument
-        else:
-            envelope = self.PitchIntervalEnvelope(envelope_or_envelope_argument)
-        self._envelope = envelope
+        return self.hertz_to_midi_pitch_number(self.hertz)
 
     # ###################################################################### #
     #                            comparison methods                          #
     # ###################################################################### #
 
     @abc.abstractmethod
-    def add(self, pitch_interval: PitchInterval, mutate: bool = True) -> Pitch:
+    def add(self, pitch_interval: PitchInterval) -> Pitch:
         ...
 
-    @core_utilities.add_copy_option
     def subtract(self, pitch_interval: music_parameters.abc.PitchInterval) -> Pitch:
-        return self.add(music_parameters.DirectPitchInterval(-pitch_interval.interval))  # type: ignore
+        return self.add(music_parameters.DirectPitchInterval(-pitch_interval.cents))
 
     def __add__(self, pitch_interval: PitchInterval) -> Pitch:
-        return self.add(pitch_interval, mutate=False)
+        return self.copy().add(pitch_interval)
 
     def __sub__(self, pitch_interval: PitchInterval) -> Pitch:
-        return self.subtract(pitch_interval, mutate=False)
-
-    def resolve_envelope(
-        self,
-        duration: core_constants.DurationType,
-        resolve_envelope_class: typing.Optional[type[core_events.Envelope]] = None,
-    ) -> core_events.Envelope:
-        if not resolve_envelope_class:
-            resolve_envelope_class = Pitch.PitchEnvelope
-        return super().resolve_envelope(duration, resolve_envelope_class)
+        return self.copy().subtract(pitch_interval)
 
     def get_pitch_interval(self, pitch_to_compare: Pitch) -> PitchInterval:
         """Get :class:`PitchInterval` between itself and other pitch
 
         :param pitch_to_compare: The pitch which shall be compared to
             the active pitch.
         :type pitch_to_compare: Pitch
         :return: :class:`PitchInterval` between
 
         **Example:**
 
         >>> from mutwo import music_parameters
-        >>> a4 = music_parameters.DirectPitch(frequency=440)
-        >>> a5 = music_parameters.DirectPitch(frequency=880)
+        >>> a4 = music_parameters.DirectPitch(hertz=440)
+        >>> a5 = music_parameters.DirectPitch(hertz=880)
         >>> pitch_interval = a4.get_pitch_interval(a5)
         """
 
-        cent_difference = self.ratio_to_cents(
-            pitch_to_compare.frequency / self.frequency
-        )
+        cent_difference = self.ratio_to_cents(pitch_to_compare.hertz / self.hertz)
         return music_parameters.DirectPitchInterval(cent_difference)
 
 
+class PitchList(core_parameters.abc.Parameter, list[Pitch]):
+    """PitchList provides functionality to parse objects to a list of pitches"""
+
+    Type: typing.TypeAlias = typing.Union[
+        Pitch.Type, list[Pitch], tuple[Pitch], str, types.NoneType
+    ]
+    """PitchList.Type hosts all types that are supported by the pitch
+    list parser :func:`PitchList.from_any`."""
+
+    @classmethod
+    def from_any(cls, object: Pitch.Type) -> Pitch:
+        match object:
+            case None:
+                return []
+            case list() | tuple():
+                return [Pitch.from_any(p) for p in object]
+            case str():
+                return [
+                    Pitch.from_any(pitch_indication)
+                    for pitch_indication in object.split(" ")
+                    if pitch_indication
+                ]
+            case _:
+                return [Pitch.from_any(object)]
+
+
 @functools.total_ordering  # type: ignore
 class Volume(
     core_parameters.abc.SingleNumberParameter,
-    value_name="amplitude",
+    value_name="decibel",
     value_return_type=float,
 ):
     """Abstract base class for any volume class.
 
     If the user wants to define a new volume class, the abstract
-    property :attr:`amplitude` has to be overridden.
+    property :attr:`decibel` has to be overridden.
     """
 
+    Type: typing.TypeAlias = typing.Union[core_constants.Real, str, "Volume"]
+    """Volume.Type hosts all types that are supported by the volume parser
+    :func:`Volume.from_any`."""
+
     @staticmethod
     def decibel_to_amplitude_ratio(
         decibel: core_constants.Real, reference_amplitude: core_constants.Real = 1
     ) -> float:
         """Convert decibel to amplitude ratio.
 
         :param decibel: The decibel number that shall be converted.
@@ -644,27 +475,43 @@
                 music_parameters.constants.MINIMUM_VELOCITY,
                 music_parameters.constants.MAXIMUM_VELOCITY,
             )
         )
 
         return velocity
 
+    @classmethod
+    def from_any(cls, object: Volume.Type) -> Volume:
+        match object:
+            case music_parameters.abc.Volume():
+                return object
+            case numbers.Real():
+                if object >= 0:  # type: ignore
+                    return music_parameters.AmplitudeVolume(object)  # type: ignore
+                else:
+                    return music_parameters.DirectVolume(object)  # type: ignore
+            case str():
+                return music_parameters.WesternVolume(object)
+            case list() | tuple():
+                return music_parameters.FlexVolume(object)
+            case _:
+                raise core_utilities.CannotParseError(object, cls)
+
     # properties
     @property
-    def decibel(self) -> core_constants.Real:
-        """The decibel of the volume (from -120 to 0)"""
-        return self.amplitude_ratio_to_decibel(self.amplitude)
+    def amplitude(self) -> core_constants.Real:
+        return self.decibel_to_amplitude_ratio(self.decibel)
 
     @property
     def midi_velocity(self) -> int:
         """The velocity of the volume (from 0 to 127)."""
         return self.decibel_to_midi_velocity(self.decibel)
 
 
-class PitchAmbitus(abc.ABC):
+class PitchAmbitus(core_parameters.abc.Parameter):
     """Abstract base class for all pitch ambituses.
 
     To setup a new PitchAmbitus class override the abstract method
     `pitch_to_period`.
     """
 
     def __init__(self, minima_pitch: Pitch, maxima_pitch: Pitch) -> None:
@@ -798,15 +645,15 @@
                 lambda pitch: pitch >= self.minima_pitch and pitch <= self.maxima_pitch,
                 pitch_to_filter_sequence,
             )
         )
 
 
 @dataclasses.dataclass()  # type: ignore
-class Indicator(abc.ABC):
+class Indicator(core_parameters.abc.Parameter):
     @property
     @abc.abstractmethod
     def is_active(self) -> bool:
         ...
 
     def get_arguments_dict(self) -> dict[str, typing.Any]:
         return {
@@ -860,38 +707,112 @@
             )
         )
 
 
 T = typing.TypeVar("T", PlayingIndicator, NotationIndicator)
 
 
-@dataclasses.dataclass
-class IndicatorCollection(typing.Generic[T]):
-    def get_all_indicator(self) -> tuple[T, ...]:
-        return tuple(
-            getattr(self, key)
-            for key in self.__dataclass_fields__.keys()  # type: ignore
-        )
+class IndicatorCollection(core_parameters.abc.Parameter, typing.Generic[T]):
+    """An :class:`IndicatorCollection` hosts a collection of indicators."""
+
+    Type: typing.TypeAlias = typing.Union[types.NoneType, str, "IndicatorCollection"]
+    """IndicatorCollection.Type hosts all types that are supported by the indicator
+    collection parser :func:`IndicatorCollection.from_any`."""
+
+    def __init_subclass__(cls):
+        # This makes sure, that we only register indicators at the class
+        # itself, but not at other classes (e.g. its super class or other
+        # sub classes of the same super class). It also makes sure that when
+        # we inherit from a 'IndicatorCollection', we also inherit all already
+        # registered indicators.
+        IndicatorName: typing.TypeAlias = str
+        cls._indicator_type_dict: dict[IndicatorName, typing.Type[Indicator]] = dict(
+            getattr(cls, "_indicator_type_dict", {})
+        )
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        for key, factory in self._indicator_type_dict.items():
+            setattr(self, key, factory())
+
+    def __eq__(self, other: typing.Any):
+        try:
+            indicator_dict1 = other.indicator_dict
+        except AttributeError:
+            return False
+
+        indicator_dict0 = self.indicator_dict
+
+        # Ensure we have the same indicators in both collections
+        key_set0 = set(indicator_dict0.keys())
+        key_set1 = set(indicator_dict1.keys())
+        if key_set0.difference(key_set1):
+            return False
+
+        # Finally compare all indicators themselves and check if they
+        # have the same values
+        for k in indicator_dict0.keys():
+            if indicator_dict0[k] != indicator_dict1[k]:
+                return False
 
-    def get_indicator_dict(self) -> dict[str, Indicator]:
-        return {key: getattr(self, key) for key in self.__dataclass_fields__.keys()}  # type: ignore
+        return True
+
+    @property
+    def indicator_tuple(self) -> tuple[T, ...]:
+        return tuple(getattr(self, key) for key in self._indicator_type_dict.keys())
+
+    @property
+    def indicator_dict(self) -> dict[str, Indicator]:
+        return {key: getattr(self, key) for key in self._indicator_type_dict.keys()}
+
+    @classmethod
+    def from_any(cls, object: IndicatorCollection.Type) -> IndicatorCollection:
+        from mutwo import music_utilities
+
+        match object:
+            case None:
+                return cls()
+            case cls():
+                return object
+            case str():
+                return music_utilities.IndicatorCollectionParser().parse(object, cls())
+            case _:
+                raise NotImplementedError(f"Can't build {cls.__name__} from '{object}'")
+
+    @classmethod
+    def register(
+        cls, indicator: typing.Type[Indicator], name: typing.Optional[str] = None
+    ):
+        """Register new indicator type to collection.
+
+        :param indicator: The indicator type that is registered.
+        :type indicator: typing.Type[Indicator]
+        :param name: The attribute name of the collection that points to
+            the indicator. If `None` this is automatically set to a lower
+            snake case version of the type name (e.g. 'MarginMarkup' is
+            converted to 'margin_markup'). Default to `None`.
+        :type name: typing.Optional[str] = None
+        """
+        name = name or core_utilities.camel_case_to_snake_case(indicator.__name__)
+        cls._indicator_type_dict[name] = indicator
+        return indicator
 
 
 class Lyric(
     core_parameters.abc.SingleValueParameter,
-    value_name="phonetic_representation",
+    value_name="xsampa",
     value_return_type=str,
 ):
     """Abstract base class for any spoken, sung or written text.
 
     If the user wants to define a new lyric class, the abstract
-    properties :attr:`phonetic_representation` and
+    properties :attr:`xampa` and
     :attr:`written_representation` have to be overridden.
 
-    The :attr:`phonetic_representation` should return a string of
+    The :attr:`xsampa` should return a string of
     X-SAMPA format phonemes, separated by space to indicate new words.
     Consult `wikipedia entry <https://en.wikipedia.org/wiki/X-SAMPA>`_
     for detailed information regarding X-SAMPA.
 
     The :attr:`written_representation` should return a string of
     normal written text, separated by space to indicate new words.
     """
@@ -909,17 +830,16 @@
     isn't.
     """
 
     def __init__(self, is_last_syllable: bool):
         self.is_last_syllable = is_last_syllable
 
 
-
 @dataclasses.dataclass(frozen=True)
-class Instrument(abc.ABC):
+class Instrument(core_parameters.abc.Parameter):
     """Model a musical instrument.
 
     :param name: The name of the instrument.
     :type name: str
     :param short_name: The abbreviation of the instrument.
         If set to ``None`` it will be the same like `name`.
         Default to ``None``.
```

### Comparing `mutwo.music-0.26.1/mutwo/music_parameters/commas.py` & `mutwo_music-0.27.0/mutwo/music_parameters/commas.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Abstractions of `tuning commas <https://en.wikipedia.org/wiki/Comma_(music)>`_
 
-The tuning commas are helpful for :class:`mutwo.parameters.pitches.JustIntonationPitch`
+The tuning commas are helpful for :class:`mutwo.music_parameters.JustIntonationPitch`
 which owns a :attr:`commas` attribute. By default :mod:`mutwo` makes use of commas
 defined by the
 `Helmholtz-Ellis JI Pitch Notation <https://marsbat.space/pdfs/notation.pdf>`_.
 """
 
 import functools
 import operator
```

### Comparing `mutwo.music-0.26.1/mutwo/music_parameters/configurations/instruments.py` & `mutwo_music-0.27.0/mutwo/music_parameters/configurations/instruments.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.1/mutwo/music_parameters/configurations/pitch_intervals.py` & `mutwo_music-0.27.0/mutwo/music_parameters/configurations/pitch_intervals.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.1/mutwo/music_parameters/configurations/pitches.py` & `mutwo_music-0.27.0/mutwo/music_parameters/configurations/pitches.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.1/mutwo/music_parameters/constants/diatonic_pitch_classes.py` & `mutwo_music-0.27.0/mutwo/music_parameters/constants/diatonic_pitch_classes.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.1/mutwo/music_parameters/constants/instruments.py` & `mutwo_music-0.27.0/mutwo/music_parameters/constants/instruments.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.1/mutwo/music_parameters/constants/pitch_intervals.py` & `mutwo_music-0.27.0/mutwo/music_parameters/constants/pitch_intervals.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.1/mutwo/music_parameters/constants/pitches.py` & `mutwo_music-0.27.0/mutwo/music_parameters/constants/pitches.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     DIATONIC_PITCH_CLASS_CONTAINER,
     OCTAVE_IN_CENTS,
     DIATONIC_PITCH_CLASS_NAME_PAIR_TO_COMPENSATION_IN_CENTS_DICT,
 )
 
 
 CENT_CALCULATION_CONSTANT = OCTAVE_IN_CENTS / (math.log10(2))
-"""constant used for cent calculation in mutwo.parameters.abc.Pitch"""
+"""constant used for cent calculation in mutwo.music_parameters.abc.Pitch"""
 
 ACCIDENTAL_NAME_TO_PITCH_CLASS_MODIFICATION_DICT = {
     # multiply with 2 because the difference of "1" in pitch
     # class is defined as one chromatic step (see class
     # definition of WesternPitch)
     accidental_name: accidental_value * 2
     for accidental_name, accidental_value in {
@@ -101,15 +101,15 @@
 """Lists all accidental names with falling quality. This is used
 in :class:`mutwo.music_parameters.WesternPitch` (in property
 :attr:`enharmonic_pitch_tuple`."""
 
 CHROMATIC_PITCH_CLASS_COUNT = 12
 """How many chromatic pitch classes exist"""
 
-# is used in mutwo.parameters.pitches.JustIntonationPitch
+# is used in mutwo.music_parameters.JustIntonationPitch
 DIATONIC_PITCH_NAME_CYCLE_OF_FIFTH_TUPLE = tuple("f c g d a e b".split(" "))
 """Diatonic pitch names sorted by cycle of fifths."""
 
 MIDI_PITCH_FREQUENCY_TUPLE = (
     8.175798915643705,
     8.66195721802725,
     9.177023997418985,
```

### Comparing `mutwo.music-0.26.1/mutwo/music_parameters/constants/playing_indicators.py` & `mutwo_music-0.27.0/mutwo/music_parameters/constants/playing_indicators.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.1/mutwo/music_parameters/constants/volumes.py` & `mutwo_music-0.27.0/mutwo/music_parameters/constants/volumes.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.1/mutwo/music_parameters/instruments/__init__.py` & `mutwo_music-0.27.0/mutwo/music_parameters/instruments/__init__.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.1/mutwo/music_parameters/instruments/general.py` & `mutwo_music-0.27.0/mutwo/music_parameters/instruments/general.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,22 +281,22 @@
             the ``tolerance`` parameter can help. This is a
             :class:`music_parameters.abc.PitchInterval`: if the difference
             is within the intervals range, it is still considered as equal
             and the harmonic is returned. Default to `DirectPitchInterval`
             with 2 cents.
         :type tolerance: music_parameters.abc.PitchInterval
         """
-        t_interval = abs(tolerance.interval)
+        t_interval = abs(tolerance.cents)
         g = self.harmonic_pitch_ambitus.get_pitch_variant_tuple
         h_t = self.harmonic_pitch_tuple
         return tuple(
             p
             for p in g(pitch, period)
             if any(
-                [abs(p.get_pitch_interval(h_p).interval) < t_interval for h_p in h_t]
+                [abs(p.get_pitch_interval(h_p).cents) < t_interval for h_p in h_t]
             )
         )
 
     def pitch_to_natural_harmonic_tuple(
         self,
         pitch: music_parameters.abc.Pitch,
         tolerance: music_parameters.abc.PitchInterval = music_parameters.DirectPitchInterval(
@@ -313,19 +313,19 @@
             the ``tolerance`` parameter can help. This is a
             :class:`music_parameters.abc.PitchInterval`: if the difference
             is within the intervals range, it is still considered as equal
             and the harmonic is returned. Default to `DirectPitchInterval`
             with 2 cents.
         :type tolerance: music_parameters.abc.PitchInterval
         """
-        t_interval = abs(tolerance.interval)
+        t_interval = abs(tolerance.cents)
         natural_harmonic_list = []
         for s in self.string_tuple:
             for h in s.natural_harmonic_tuple:
-                if abs((h.pitch.get_pitch_interval(pitch)).interval) < t_interval:
+                if abs((h.pitch.get_pitch_interval(pitch)).cents) < t_interval:
                     natural_harmonic_list.append(h)
         return tuple(natural_harmonic_list)
 
 
 class UnpitchedInstrument(music_parameters.abc.Instrument):
     """Model a musical instruments without any clear pitches.
 
@@ -524,15 +524,15 @@
         >>> from mutwo import music_parameters
         >>> orch = music_parameters.Orchestration(
         ...   oboe0=music_parameters.Oboe(),
         ...   oboe1=music_parameters.Oboe(),
         ...   oboe2=music_parameters.Oboe(),
         ... )
         >>> orch.get_subset('oboe0', 'oboe2')
-        Orchestration(oboe0=Oboe(name='oboe', short_name='ob.', pitch_count_range=Range[1, 2), transposition_pitch_interval=DirectPitchInterval(interval = 0)), oboe2=Oboe(name='oboe', short_name='ob.', pitch_count_range=Range[1, 2), transposition_pitch_interval=DirectPitchInterval(interval = 0)))
+        Orchestration(oboe0=Oboe(name='oboe', short_name='ob.', pitch_count_range=Range[1, 2), transposition_pitch_interval=D(0)), oboe2=Oboe(name='oboe', short_name='ob.', pitch_count_range=Range[1, 2), transposition_pitch_interval=D(0)))
         """
         return Orchestration(**{name: getattr(self, name) for name in instrument_name})
 
 
 def Orchestration(**instrument_name_to_instrument: music_parameters.abc.Instrument):
     r"""Create a name space for the instrumentation of a composition.
 
@@ -549,15 +549,15 @@
     **Example:**
 
     >>> from mutwo import music_parameters
     >>> music_parameters.Orchestration(
     ...   oboe0=music_parameters.Oboe(),
     ...   oboe1=music_parameters.Oboe(),
     ... )
-    Orchestration(oboe0=Oboe(name='oboe', short_name='ob.', pitch_count_range=Range[1, 2), transposition_pitch_interval=DirectPitchInterval(interval = 0)), oboe1=Oboe(name='oboe', short_name='ob.', pitch_count_range=Range[1, 2), transposition_pitch_interval=DirectPitchInterval(interval = 0)))
+    Orchestration(oboe0=Oboe(name='oboe', short_name='ob.', pitch_count_range=Range[1, 2), transposition_pitch_interval=D(0)), oboe1=Oboe(name='oboe', short_name='ob.', pitch_count_range=Range[1, 2), transposition_pitch_interval=D(0)))
     """
 
     instrument_name_tuple, instrument_tuple = tuple([]), tuple([])
     if instrument_name_to_instrument:
         instrument_name_tuple, instrument_tuple = zip(
             *instrument_name_to_instrument.items()
         )
```

### Comparing `mutwo.music-0.26.1/mutwo/music_parameters/lyrics/text_based_lyrics.py` & `mutwo_music-0.27.0/mutwo/music_parameters/lyrics/text_based_lyrics.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         return self._written_representation
 
     @written_representation.setter
     def written_representation(self, written_representation: str):
         self._written_representation = written_representation
 
     @property
-    def phonetic_representation(self) -> str:
+    def xsampa(self) -> str:
         word_tuple = self.written_representation.split(" ")
         return " ".join(
             ["".join(self._epitran.xsampa_list(word)) for word in word_tuple]
         )
 
 
 class LanguageBasedSyllable(music_parameters.abc.Syllable, LanguageBasedLyric):
@@ -75,22 +75,22 @@
         `mutwo.music_parameters.configurations.DEFAULT_LANGUAGE_CODE`
         will be used. Default to `None`.
     :type language_code: typing.Optional[str]
 
     **Warning:**
 
     It is a known bug that a split word (syllables) and the word
-    itself will return different values for :attr:`phonetic_representation`.
+    itself will return different values for :attr:`xsampa`.
     For instance:
 
-    >>> LanguageBasedLyric('hallo').phonetic_representation
+    >>> LanguageBasedLyric('hallo').xsampa
     'halo:'
     >>> # And now splitted to syllables:
-    >>> LanguageBasedSyllable(False, 'hal').phonetic_representation
+    >>> LanguageBasedSyllable(False, 'hal').xsampa
     'hA:l'
-    >>> LanguageBasedSyllable(True, 'lo').phonetic_representation
+    >>> LanguageBasedSyllable(True, 'lo').xsampa
     'lo:'
     """
 
     def __init__(self, is_last_syllable: bool, *args, **kwargs):
         music_parameters.abc.Syllable.__init__(self, is_last_syllable)
         LanguageBasedLyric.__init__(self, *args, **kwargs)
```

### Comparing `mutwo.music-0.26.1/mutwo/music_parameters/pitch_intervals.py` & `mutwo_music-0.27.0/mutwo/music_parameters/pitch_intervals.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,46 +11,45 @@
     "WesternPitchInterval",
 )
 
 
 class DirectPitchInterval(music_parameters.abc.PitchInterval):
     """Simple interval class which gets directly assigned by its cents value
 
-    :param interval: Defines how big or small the interval is (in cents).
-    :type interval: float
+    :param cents: Defines how big or small the interval is (in cents).
+    :type cents: float
 
     **Example:**
 
     >>> from mutwo import music_parameters
     >>> rising_octave = music_parameters.DirectPitchInterval(1200)
     >>> falling_minor_third = music_parameters.DirectPitchInterval(-300)
     """
 
-    def __init__(self, interval: float):
-        self.interval = interval
+    def __init__(self, cents: float):
+        self.cents = cents
 
     @property
-    def interval(self) -> float:
-        return self._interval
+    def cents(self) -> float:
+        return self._cents
 
-    @interval.setter
-    def interval(self, interval: float):
-        self._interval = interval
+    @cents.setter
+    def cents(self, cents: float):
+        self._cents = cents
 
-    @core_utilities.add_copy_option
-    def inverse(self, mutate: bool = False) -> DirectPitchInterval:
+    def inverse(self) -> DirectPitchInterval:
         """Makes falling interval to rising and vice versa.
 
         **Example:**
 
         >>> from mutwo import music_parameters
-        >>> music_parameters.DirectPitchInterval(700).inverse().interval
+        >>> music_parameters.DirectPitchInterval(700).inverse().cents
         -700
         """
-        self.interval = -self.interval
+        self.cents = -self.cents
         return self
 
 
 class WesternPitchInterval(music_parameters.abc.PitchInterval):
     """Model intervals by using European music theory based representations
 
     :param interval_name_or_semitone_count: Can be either an interval name
@@ -86,15 +85,14 @@
     >>> very_diminished_sixth = music_parameters.WesternPitchInterval('dddd6')
     """
 
     def __init__(
         self,
         interval_name_or_semitone_count: str | core_constants.Real = "p1",
     ):
-        self._logger = core_utilities.get_cls_logger(type(self))
         # Define mapping on the fly, so that it is only necessary to adjust
         # music_parameters.configurations.WESTERN_PITCH_INTERVAL_QUALITY_NAME_TO_ABBREVIATION_DICT
         # if user wants to use different abbreviations.
         self._abbreviation_to_western_pitch_interval_quality_name_dict = {
             abbreviation: western_pitch_interval_quality
             for western_pitch_interval_quality, abbreviation in music_parameters.configurations.WESTERN_PITCH_INTERVAL_QUALITY_NAME_TO_ABBREVIATION_DICT.items()
         }
@@ -511,25 +509,25 @@
         This excludes intervals as prime, fourth, ... which have the
         'perfect' quality.
         """
 
         return WesternPitchInterval.is_interval_type_imperfect(self.interval_type)
 
     @property
-    def interval(self) -> float:
+    def cents(self) -> float:
         cent_deviation = (
             self.interval_quality_cent_deviation + self.interval_type_cent_deviation
         )
         if self.is_interval_falling:
             cent_deviation = -cent_deviation
         return cent_deviation
 
     @property
     def semitone_count(self) -> float:
-        return self.interval // 100
+        return self.cents // 100
 
     @semitone_count.setter
     def semitone_count(self, semitone_count: core_constants.Real):
         self._set_attribute_by_interval_data(
             *self._semitone_count_to_interval_data(semitone_count)
         )
 
@@ -564,16 +562,15 @@
             ]
         )
 
     # ###################################################################### #
     #                           public methods                               #
     # ###################################################################### #
 
-    @core_utilities.add_copy_option
-    def inverse(self, mutate: bool = False) -> WesternPitchInterval:
+    def inverse(self) -> WesternPitchInterval:
         """Makes falling interval to rising and vice versa.
 
         **Example:**
 
         >>> from mutwo import music_parameters
         >>> music_parameters.WesternPitchInterval('m3').inverse()
         WesternPitchInterval('m-3')
```

### Comparing `mutwo.music-0.26.1/mutwo/music_parameters/pitches/CommonHarmonic.py` & `mutwo_music-0.27.0/mutwo/music_parameters/pitches/CommonHarmonic.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.1/mutwo/music_parameters/pitches/DirectPitch.py` & `mutwo_music-0.27.0/mutwo/music_parameters/pitches/DirectPitch.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,38 @@
 from __future__ import annotations
 
 from mutwo import core_constants
-from mutwo import core_utilities
 from mutwo import music_parameters
 
 __all__ = ("DirectPitch",)
 
 
 class DirectPitch(music_parameters.abc.Pitch):
     """A simple pitch class that gets directly initialised by its frequency.
 
-    :param frequency: The frequency of the ``DirectPitch`` object.
+    :param hertz: The hertz of the ``DirectPitch`` object.
 
     May be used when a converter class needs a pitch object, but there is
     no need or desire for a complex abstraction of the respective pitch
     (that classes like ``JustIntonationPitch`` or ``WesternPitch`` offer).
 
     **Example:**
 
     >>> from mutwo import music_parameters
     >>> my_pitch = music_parameters.DirectPitch(440)
     """
 
-    def __init__(self, frequency: core_constants.Real, *args, **kwargs):
+    def __init__(self, hertz: core_constants.Real, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self._frequency = float(frequency)
+        self._hertz = float(hertz)
 
     @property
-    def frequency(self) -> float:
+    def hertz(self) -> float:
         """The frequency of the pitch."""
-
-        return self._frequency
+        return self._hertz
 
     def __repr__(self) -> str:
-        return "DirectPitch(frequency = {})".format(self.frequency)
+        return "DirectPitch(hertz = {})".format(self.hertz)
 
-    @core_utilities.add_copy_option
-    def add(
-        self, pitch_interval: music_parameters.abc.PitchInterval, mutate: bool = False
-    ) -> DirectPitch:
-        self._frequency = self.cents_to_ratio(pitch_interval.interval) * self.frequency
+    def add(self, pitch_interval: music_parameters.abc.PitchInterval) -> DirectPitch:
+        self._hertz = self.cents_to_ratio(pitch_interval.cents) * self.hertz
         return self
```

### Comparing `mutwo.music-0.26.1/mutwo/music_parameters/pitches/EqualDividedOctavePitch.py` & `mutwo_music-0.27.0/mutwo/music_parameters/pitches/EqualDividedOctavePitch.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         self,
         pitch_interval: music_parameters.abc.PitchInterval | core_constants.Real,
     ) -> core_constants.Real:
         if isinstance(
             pitch_interval,
             music_parameters.abc.PitchInterval,
         ):
-            return pitch_interval.interval / self.n_cents_per_step
+            return pitch_interval.cents / self.n_cents_per_step
         else:
             return pitch_interval
 
     def _math(
         self,
         n_pitch_classes_difference: core_constants.Real,
         operator: typing.Callable[
@@ -173,48 +173,47 @@
 
     @property
     def n_cents_per_step(self) -> float:
         """This property describes how many cents are between two adjacent pitches."""
         return self.ratio_to_cents(self.step_factor)
 
     @property
-    def frequency(self) -> float:
+    def hertz(self) -> float:
         n_octaves_distant_to_concert_pitch = self.octave - self.concert_pitch_octave
         n_pitch_classes_distant_to_concert_pitch = (
             self.pitch_class - self.concert_pitch_pitch_class
         )
         distance_to_concert_pitch_in_cents = (
             n_octaves_distant_to_concert_pitch
             * music_parameters.constants.OCTAVE_IN_CENTS
         ) + (self.n_cents_per_step * n_pitch_classes_distant_to_concert_pitch)
         distance_to_concert_pitch_as_factor = self.cents_to_ratio(
             distance_to_concert_pitch_in_cents
         )
         return core_utilities.round_floats(
-            self.concert_pitch.frequency * distance_to_concert_pitch_as_factor,
+            self.concert_pitch.hertz* distance_to_concert_pitch_as_factor,
             music_parameters.configurations.EQUAL_DIVIDED_OCTAVE_PITCH_ROUND_FREQUENCY_DIGIT_COUNT,
         )
 
     # ###################################################################### #
     #                          public methods                                #
     # ###################################################################### #
 
-    @core_utilities.add_copy_option
-    def add(  # type: ignore
+    def add(
         self, pitch_interval: music_parameters.abc.PitchInterval | core_constants.Real
     ) -> EqualDividedOctavePitch:  # type: ignore
         """Transposes the ``EqualDividedOctavePitch`` by n_pitch_classes_difference."""
 
         n_pitch_classes_difference = self._fetch_n_pitch_classes_difference(
             pitch_interval
         )
         self._math(n_pitch_classes_difference, operator.add)
+        return self
 
-    @core_utilities.add_copy_option
-    def subtract(  # type: ignore
+    def subtract(
         self, pitch_interval: music_parameters.abc.PitchInterval | core_constants.Real
     ) -> EqualDividedOctavePitch:  # type: ignore
         """Transposes the ``EqualDividedOctavePitch`` by n_pitch_classes_difference."""
         if isinstance(
             pitch_interval,
             music_parameters.abc.PitchInterval,
         ):
```

### Comparing `mutwo.music-0.26.1/mutwo/music_parameters/pitches/JustIntonationPitch.py` & `mutwo_music-0.27.0/mutwo/music_parameters/pitches/JustIntonationPitch.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,14 @@
         ratio_or_exponent_tuple: typing.Union[
             str, fractions.Fraction, typing.Iterable[int]
         ] = "1/1",
         concert_pitch: ConcertPitch = None,
         *args,
         **kwargs,
     ):
-        self._logger = core_utilities.get_cls_logger(type(self))
         super().__init__(*args, **kwargs)
 
         if concert_pitch is None:
             concert_pitch = music_parameters.configurations.DEFAULT_CONCERT_PITCH
 
         self.exponent_tuple = self._ratio_or_fractions_argument_to_exponent_tuple(
             ratio_or_exponent_tuple
@@ -400,43 +399,43 @@
             raise NotImplementedError(
                 f"Unknown type '{type(ratio_or_exponent_tuple)}' of object "
                 f"'{ratio_or_exponent_tuple}' for 'ratio_or_exponent_tuple' "
                 "argument."
             )
         return exponent_tuple
 
-    @core_utilities.add_copy_option
     def _math(  # type: ignore
         self, other: JustIntonationPitch, operation: typing.Callable
     ) -> JustIntonationPitch:
         exponent_tuple0, exponent_tuple1 = JustIntonationPitch._adjust_exponent_lengths(
             self.exponent_tuple, other.exponent_tuple
         )
         self.exponent_tuple = tuple(
             operation(exponent0, exponent1)
             for exponent0, exponent1 in zip(exponent_tuple0, exponent_tuple1)
         )
+        return self
 
     # ###################################################################### #
     #                            magic methods                               #
     # ###################################################################### #
 
     def __eq__(self, other: typing.Any) -> bool:
         match other:
             case JustIntonationPitch():
                 return self.exponent_tuple == other.exponent_tuple
             case music_parameters.abc.PitchInterval():
-                return self.interval == other.interval
+                return self.cents == other.cents
             case _:  # pitch test
                 return super().__eq__(other)
 
     def __lt__(self, other: typing.Any) -> bool:
         match other:
             case music_parameters.abc.PitchInterval():
-                return self.interval < other.interval
+                return self.cents < other.cents
             case _:  # pitch test
                 return super().__lt__(other)
 
     def __float__(self) -> float:
         """Return the float of a JustIntonationPitch - object.
 
         These are the same:
@@ -517,16 +516,16 @@
     def concert_pitch(self, concert_pitch: ConcertPitch) -> None:
         if not isinstance(concert_pitch, music_parameters.abc.Pitch):
             concert_pitch = music_parameters.DirectPitch(concert_pitch)
 
         self._concert_pitch = concert_pitch
 
     @property
-    def frequency(self) -> float:
-        return float(self.ratio * self.concert_pitch.frequency)
+    def hertz(self) -> float:
+        return float(self.ratio * self.concert_pitch.hertz)
 
     @property
     def ratio(self) -> fractions.Fraction:
         """Return the JustIntonationPitch transformed to a Ratio.
 
         **Example:**
 
@@ -573,15 +572,15 @@
         denominator = 1
         for number, exponent in zip(self.prime_tuple, self.exponent_tuple):
             if exponent < 0:
                 denominator *= pow(number, -exponent)
         return denominator
 
     @property
-    def interval(self) -> float:
+    def cents(self) -> float:
         return self.ratio_to_cents(self.ratio)
 
     @property
     def factorised(self) -> tuple:
         """Return factorised / decomposed version of itsef.
 
         **Example:**
@@ -622,15 +621,15 @@
         return tuple(
             functools.reduce(operator.add, decomposed)
             for decomposed in numerator_denominator
         )
 
     @property
     def octave(self) -> int:
-        return int(self.interval // music_parameters.constants.OCTAVE_IN_CENTS)
+        return int(self.cents // music_parameters.constants.OCTAVE_IN_CENTS)
 
     @property
     def helmholtz_ellis_just_intonation_notation_commas(
         self,
     ) -> music_parameters.CommaCompound:
         """Commas of JustIntonationPitch."""
 
@@ -650,30 +649,30 @@
             closest_pythagorean_interval = self - type(self)(
                 functools.reduce(
                     operator.mul, self.helmholtz_ellis_just_intonation_notation_commas
                 )
             )
             closest_pythagorean_interval.normalize()
         else:
-            closest_pythagorean_interval = self.normalize(mutate=False)  # type: ignore
+            closest_pythagorean_interval = self.copy().normalize()  # type: ignore
 
         return closest_pythagorean_interval
 
     @property
     def cent_deviation_from_closest_western_pitch_class(self) -> float:
         deviation_by_helmholtz_ellis_just_intonation_notation_commas = (
             JustIntonationPitch(
                 self.helmholtz_ellis_just_intonation_notation_commas.ratio
-            ).interval
+            ).cents
         )
         closest_pythagorean_interval = self.closest_pythagorean_interval
         if len(closest_pythagorean_interval.exponent_tuple) >= 2:
             pythagorean_deviation = self.closest_pythagorean_interval.exponent_tuple[
                 1
-            ] * (JustIntonationPitch("3/2").interval - 700)
+            ] * (JustIntonationPitch("3/2").cents - 700)
         else:
             pythagorean_deviation = 0
         return (
             deviation_by_helmholtz_ellis_just_intonation_notation_commas
             + pythagorean_deviation
         )
 
@@ -964,16 +963,15 @@
         self, pitch_to_compare: music_parameters.abc.Pitch
     ) -> music_parameters.abc.PitchInterval:
         if isinstance(pitch_to_compare, JustIntonationPitch):
             return pitch_to_compare - self
         else:
             return super().get_pitch_interval(pitch_to_compare)
 
-    @core_utilities.add_copy_option
-    def register(self, octave: int) -> JustIntonationPitch:  # type: ignore
+    def register(self, octave: int) -> JustIntonationPitch:
         """Move :class:`JustIntonationPitch` to the given octave.
 
         :param octave: 0 for the octave from 1/1 to 2/1, negative values for octaves
             below 1/1 and positive values for octaves above 2/1.
         :type octave: int
 
         **Example:**
@@ -990,48 +988,48 @@
         JustIntonationPitch('3/4')
         >>> p.register(0)
         JustIntonationPitch('3/2')
         >>> p
         JustIntonationPitch('3/2')
         """
 
-        normalized_just_intonation_pitch = self.normalize(mutate=False)  # type: ignore
+        normalized_just_intonation_pitch = self.copy().normalize()  # type: ignore
         factor = 2 ** abs(octave)
         if octave < 1:
             added = type(self)(fractions.Fraction(1, factor))
         else:
             added = type(self)(fractions.Fraction(factor, 1))
         self.exponent_tuple = (normalized_just_intonation_pitch + added).exponent_tuple  # type: ignore
+        return self
 
-    @core_utilities.add_copy_option
-    def move_to_closest_register(  # type: ignore
+    def move_to_closest_register(
         self, reference: JustIntonationPitch
     ) -> JustIntonationPitch:
         reference_register = reference.octave
 
         best = None
         for adaption in range(-1, 2):
-            candidate: JustIntonationPitch = self.register(reference_register + adaption, mutate=False)  # type: ignore
-            difference = abs((candidate - reference).interval)
+            candidate: JustIntonationPitch = self.copy().register(reference_register + adaption)  # type: ignore
+            difference = abs((candidate - reference).cents)
             set_best = True
             if best and difference > best[1]:
                 set_best = False
 
             if set_best:
                 best = (candidate, difference)
 
         if best:
             self.exponent_tuple = best[0].exponent_tuple
         else:
             raise NotImplementedError(
                 f"Couldn't find closest register of '{self}' to '{reference}'."
             )
+        return self
 
-    @core_utilities.add_copy_option
-    def normalize(self, prime: int = 2) -> JustIntonationPitch:  # type: ignore
+    def normalize(self, prime: int = 2) -> JustIntonationPitch:
         """Normalize :class:`JustIntonationPitch`.
 
         :param prime: The normalization period (2 for octave,
             3 for twelfth, ...). Default to 2.
         :type prime: int
 
         **Example:**
@@ -1044,17 +1042,17 @@
         JustIntonationPitch('3/2')
         """
         ratio = self.ratio
         adjusted = type(self)._adjust_ratio(ratio, prime)
         self.exponent_tuple = self._ratio_or_fractions_argument_to_exponent_tuple(
             adjusted
         )
+        return self
 
-    @core_utilities.add_copy_option
-    def inverse(  # type: ignore
+    def inverse(
         self, axis: typing.Optional[JustIntonationPitch] = None
     ) -> JustIntonationPitch:
         """Inverse current pitch on given axis.
 
         :param axis: The :class:`JustIntonationPitch` from which the
             pitch shall be inversed.
         :type axis: JustIntonationPitch, optional
@@ -1071,16 +1069,16 @@
 
         if axis is None:
             exponent_tuple = tuple(map(lambda x: -x, self.exponent_tuple))
         else:
             distance = self - axis
             exponent_tuple = (axis - distance).exponent_tuple
         self.exponent_tuple = exponent_tuple
+        return self
 
-    @core_utilities.add_copy_option
     def add(
         self, pitch_interval: music_parameters.abc.PitchInterval
     ) -> JustIntonationPitch:
         """Add :class:`JustIntonationPitch` to current pitch.
 
         :param other: The :class:`JustIntonationPitch` to add to
             the current pitch.
@@ -1094,19 +1092,18 @@
         >>> p
         JustIntonationPitch('9/4')
         """
         if isinstance(pitch_interval, JustIntonationPitch):
             self._math(pitch_interval, operator.add)
         else:
             self.exponent_tuple = self._ratio_to_exponent_tuple(
-                self.ratio * self.cents_to_ratio(pitch_interval.interval)
+                self.ratio * self.cents_to_ratio(pitch_interval.cents)
             )
         return self
 
-    @core_utilities.add_copy_option
     def subtract(
         self, pitch_interval: music_parameters.abc.PitchInterval
     ) -> JustIntonationPitch:
         """Subtract :class:`JustIntonationPitch` from current pitch.
 
         :param other: The :class:`JustIntonationPitch` to subtract from
             the current pitch.
@@ -1121,19 +1118,18 @@
         JustIntonationPitch('3/2')
         """
 
         if isinstance(pitch_interval, JustIntonationPitch):
             self._math(pitch_interval, operator.sub)
         else:
             self.exponent_tuple = self._ratio_to_exponent_tuple(
-                self.ratio / self.cents_to_ratio(pitch_interval.interval)
+                self.ratio / self.cents_to_ratio(pitch_interval.cents)
             )
         return self
 
-    @core_utilities.add_copy_option
     def intersection(
         self, other: JustIntonationPitch, strict: bool = False
     ) -> JustIntonationPitch:
         """Make intersection with other :class:`JustIntonationPitch`.
 
         :param other: The :class:`JustIntonationPitch` to build the
             intersection with.
@@ -1189,7 +1185,8 @@
 
         intersected_exponent_tuple = tuple(
             map(
                 intersect_exponent_tuple, zip(self.exponent_tuple, other.exponent_tuple)
             )
         )
         self.exponent_tuple = intersected_exponent_tuple
+        return self
```

### Comparing `mutwo.music-0.26.1/mutwo/music_parameters/pitches/MidiPitch.py` & `mutwo_music-0.27.0/mutwo/music_parameters/pitches/MidiPitch.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-from mutwo import core_utilities
 from mutwo import music_parameters
 
 __all__ = ("MidiPitch",)
 
 
 class MidiPitch(music_parameters.abc.Pitch):
     """Pitch that is defined by its midi pitch number.
@@ -25,27 +24,26 @@
         super().__init__(*args, **kwargs)
         self._midi_pitch_number = midi_pitch_number
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}(midi_pitch_number = {self.midi_pitch_number})"
 
     @property
-    def frequency(self) -> float:
+    def hertz(self) -> float:
         difference_to_middle_a = self.midi_pitch_number - 69
         return float(440 * self.cents_to_ratio(difference_to_middle_a * 100))
 
     @property
     def midi_pitch_number(self) -> float:
         return self._midi_pitch_number
 
     @midi_pitch_number.setter
     def midi_pitch_number(self, new_midi_pitch_number: float):
         self._midi_pitch_number = new_midi_pitch_number
 
-    @core_utilities.add_copy_option
     def add(
-        self, pitch_interval: music_parameters.abc.PitchInterval, mutate: bool = False
+        self, pitch_interval: music_parameters.abc.PitchInterval
     ) -> MidiPitch:
         self.midi_pitch_number = self.hertz_to_midi_pitch_number(
-            self.cents_to_ratio(pitch_interval.interval) * self.frequency
+            self.cents_to_ratio(pitch_interval.cents) * self.hertz
         )
         return self
```

### Comparing `mutwo.music-0.26.1/mutwo/music_parameters/pitches/ScalePitch.py` & `mutwo_music-0.27.0/mutwo/music_parameters/pitches/ScalePitch.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 
 import typing
 
-from mutwo import core_utilities
 from mutwo import music_parameters
 
 __all__ = ("ScalePitch",)
 
 
 class ScalePitch(music_parameters.abc.Pitch):
     """Pitch that is defined by its scale degree, octave and reference scale.
@@ -53,19 +52,18 @@
         return (self.scale_degree, self.octave)
 
     @property
     def scale_pitch(self) -> music_parameters.abc.Pitch:
         return self.scale.scale_position_to_pitch(self.scale_position)
 
     @property
-    def frequency(self) -> float:
-        return self.scale_pitch.frequency
+    def hertz(self) -> float:
+        return self.scale_pitch.hertz
 
-    @core_utilities.add_copy_option
     def add(
-        self, pitch_interval: music_parameters.abc.PitchInterval, mutate: bool = False
+        self, pitch_interval: music_parameters.abc.PitchInterval
     ) -> ScalePitch:
-        p = self.scale_pitch.add(pitch_interval, mutate=False)
+        p = self.scale_pitch.copy().add(pitch_interval)
         if p not in self.scale.pitch_tuple:
             raise RuntimeError(f"Pitch '{p}' isn't part of reference scale.")
         self.scale_degree, self.octave = self.scale.pitch_to_scale_position(p)
         return self
```

### Comparing `mutwo.music-0.26.1/mutwo/music_parameters/pitches/WesternPitch.py` & `mutwo_music-0.27.0/mutwo/music_parameters/pitches/WesternPitch.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,14 @@
         octave: int = 4,
         concert_pitch_pitch_class: core_constants.Real = None,
         concert_pitch_octave: int = None,
         concert_pitch: ConcertPitch = None,
         *args,
         **kwargs,
     ):
-        self._logger = core_utilities.get_cls_logger(type(self))
 
         (
             pitch_class,
             pitch_class_name,
         ) = self._pitch_class_or_pitch_class_name_to_pitch_class_and_pitch_class_name(
             pitch_class_or_pitch_class_name
         )
@@ -262,15 +261,19 @@
     # ###################################################################### #
     #                         private methods                                #
     # ###################################################################### #
 
     def _parse_pitch_interval(
         self,
         pitch_interval: str | music_parameters.abc.PitchInterval | core_constants.Real,
-    ) -> music_parameters.abc.PitchInterval | core_constants.Real | music_parameters.abc.PitchInterval:
+    ) -> (
+        music_parameters.abc.PitchInterval
+        | core_constants.Real
+        | music_parameters.abc.PitchInterval
+    ):
         if isinstance(pitch_interval, str):
             pitch_interval = music_parameters.WesternPitchInterval(pitch_interval)
         elif isinstance(pitch_interval, core_constants.Real.__args__ + (int,)):
             # Only convert to western pitch interval in case the interval isn't
             # microtonal (because WesternPitchInterval doesn't support
             # microtonality). 0.001 (= 0.1 cents) are set in case for
             # floating point errors.
@@ -292,15 +295,14 @@
         )
 
     def _get_new_pitch_class_modification(
         self,
         western_pitch_interval_to_add: music_parameters.WesternPitchInterval,
         new_diatonic_pitch_class_name: str,
     ) -> fractions.Fraction:
-
         key = (self.diatonic_pitch_class_name, new_diatonic_pitch_class_name)
         if western_pitch_interval_to_add.is_interval_falling:
             key = tuple(reversed(key))
 
         added_cent_deviation = (
             western_pitch_interval_to_add.interval_quality_cent_deviation
             + music_parameters.constants.DIATONIC_PITCH_CLASS_NAME_PAIR_TO_COMPENSATION_IN_CENTS_DICT[
@@ -456,33 +458,32 @@
 
         return tuple(enharmonic_pitch_list)
 
     # ###################################################################### #
     #                          public methods                                #
     # ###################################################################### #
 
-    @core_utilities.add_copy_option
-    def add(  # type: ignore
+    def add(
         self,
         pitch_interval: str | music_parameters.abc.PitchInterval | core_constants.Real,
     ) -> WesternPitch:  # type: ignore
         pitch_interval = self._parse_pitch_interval(pitch_interval)
         if isinstance(pitch_interval, music_parameters.WesternPitchInterval):
             self._add_western_pitch_interval(pitch_interval)
         else:
             return super().add(pitch_interval)  # type: ignore
+        return self
 
-    @core_utilities.add_copy_option
-    def subtract(  # type: ignore
+    def subtract(
         self,
         pitch_interval: str | music_parameters.abc.PitchInterval | core_constants.Real,
     ) -> WesternPitch:  # type: ignore
         pitch_interval = self._parse_pitch_interval(pitch_interval)
         if isinstance(pitch_interval, music_parameters.WesternPitchInterval):
-            return self.add(pitch_interval.inverse(mutate=False))
+            return self.add(pitch_interval.copy().inverse())
         else:
             return super().subtract(pitch_interval)  # type: ignore
 
     def _get_western_pitch_interval(
         self, pitch_to_compare: music_parameters.WesternPitch
     ) -> music_parameters.WesternPitchInterval:
         # First we need to fetch the basic interval type:
@@ -561,15 +562,14 @@
                 pitch_interval.inverse()
             else:
                 pitch_interval = self._get_western_pitch_interval(pitch_to_compare)
             return pitch_interval
         else:
             return super().get_pitch_interval(pitch_to_compare)
 
-    @core_utilities.add_copy_option
     def round_to(
         self,
         allowed_division_sequence: typing.Sequence[fractions.Fraction] = (
             fractions.Fraction(1, 1),
         ),
     ) -> WesternPitch:
         """Round to closest accidental (helpful to avoid microtones).
```

### Comparing `mutwo.music-0.26.1/mutwo/music_parameters/pitches/__init__.py` & `mutwo_music-0.27.0/mutwo/music_parameters/pitches/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,19 +21,21 @@
 from .DirectPitch import *
 from .MidiPitch import *
 from .JustIntonationPitch import *
 from .CommonHarmonic import *
 from .EqualDividedOctavePitch import *
 from .WesternPitch import *
 from .ScalePitch import *
+from .FlexPitch import *
 
 
 __all__ = (
     "DirectPitch",
     "JustIntonationPitch",
     "Partial",
     "EqualDividedOctavePitch",
     "WesternPitch",
     "MidiPitch",
     "CommonHarmonic",
     "ScalePitch",
+    "FlexPitch",
 )
```

### Comparing `mutwo.music-0.26.1/mutwo/music_parameters/scales.py` & `mutwo_music-0.27.0/mutwo/music_parameters/scales.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,18 +215,18 @@
         repeating_period_repetition_count_tuple = ScaleFamily._period_repetition_count_sequence_to_period_repetition_count_tuple(
             repeating_period_repetition_count_sequence, repeating_interval_tuple
         )
 
         is_rising = ScaleFamily._is_interval_tuple_rising(repeating_interval_tuple)
 
         interval_range = (
-            repeating_interval_tuple[0].interval - repeating_interval_tuple[-1].interval
+            repeating_interval_tuple[0].cents - repeating_interval_tuple[-1].cents
         )
 
-        assert abs(interval_range) < abs(repetition_interval.interval), (
+        assert abs(interval_range) < abs(repetition_interval.cents), (
             "Repetition interval has to be bigger than "
             "ambitus of repeating interval sequence!"
         )
 
         interval_data_list = [
             (interval, weight, scale_degree, period_repetition_count)
             for interval, weight, scale_degree, period_repetition_count in zip(
@@ -236,25 +236,25 @@
                 repeating_period_repetition_count_tuple,
             )
             if interval >= min_pitch_interval and interval < max_pitch_interval
         ]
 
         for local_repetition_interval in (
             repetition_interval,
-            repetition_interval.inverse(mutate=False),
+            repetition_interval.copy().inverse(),
         ):
             last_interval_data_list = list(
                 zip(
                     repeating_interval_tuple,
                     repeating_weight_tuple,
                     repeating_scale_degree_tuple,
                     repeating_period_repetition_count_tuple,
                 )
             )
-            if local_repetition_interval.interval > 0:
+            if local_repetition_interval.cents > 0:
                 period_repetition_delta = 1
             else:
                 period_repetition_delta = -1
             while 1:
                 new_interval_data_list = []
                 is_valid = True
                 for (
@@ -406,7 +406,12 @@
     def pitch_to_scale_index(self, pitch: music_parameters.abc.Pitch) -> ScaleIndex:
         return self.pitch_tuple.index(pitch)
 
     def scale_index_to_pitch(
         self, scale_index: ScaleIndex
     ) -> music_parameters.abc.Pitch:
         return self.pitch_tuple[scale_index]
+
+    def scale_degree_to_pitch_class(
+        self, scale_degree: ScaleDegree
+    ) -> music_parameters.abc.Pitch:
+        ...
```

### Comparing `mutwo.music-0.26.1/mutwo/music_parameters/volumes.py` & `mutwo_music-0.27.0/mutwo/music_parameters/volumes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,66 +1,98 @@
 """Submodule for the parameter volume.
 
-'Volume' is defined as any object that knows a :attr:`amplitude` attribute.
+'Volume' is defined as any object that knows a :attr:`decibel` attribute.
 """
 
 import typing
 
 from mutwo import core_constants
+from mutwo import core_parameters
 from mutwo import core_utilities
 from mutwo import music_parameters
 from mutwo import music_utilities
 
-__all__ = ("DirectVolume", "DecibelVolume", "WesternVolume")
+__all__ = ("DirectVolume", "FlexVolume", "AmplitudeVolume", "WesternVolume")
 
 
 class DirectVolume(music_parameters.abc.Volume):
-    """A simple volume class that gets directly initialised by its amplitude.
+    """A simple volume class that gets directly initialised by decibel.
 
-    :param amplitude: The amplitude of the :class:`DirectVolume` object.
+    :param decibel: The decibel of the :class:`DecibelVolume` object (should be
+        from -120 to 0).
 
     May be used when a converter class needs a volume object, but there is
     no need or desire for a complex abstraction of the respective volume.
     """
 
-    def __init__(self, amplitude: core_constants.Real):
-        self._amplitude = amplitude
+    def __init__(self, decibel: core_constants.Real):
+        self._decibel = decibel
 
     @property
-    def amplitude(self) -> core_constants.Real:
-        return self._amplitude
+    def decibel(self) -> core_constants.Real:
+        return self._decibel
+
+    @decibel.setter
+    def decibel(self, decibel: core_constants.Real):
+        self._decibel = decibel
 
     def __repr__(self) -> str:
         return "{}({})".format(type(self).__name__, self.amplitude)
 
 
-class DecibelVolume(music_parameters.abc.Volume):
-    """A simple volume class that gets directly initialised by decibel.
+class FlexVolume(music_parameters.abc.Volume, core_parameters.abc.FlexParameterMixin):
+    """A flexible volume.
+
+    This can be used to create dynamically changing volumes (e.g. crescendo,
+    decrescendo, ...).
+
+    **Example:**
+
+    >>> from mutwo import music_parameters
+    >>> v = music_parameters.FlexVolume([[0, 'ff'], [1, 'ppp']])
+    """
+
+    @classmethod
+    @property
+    def parameter_name(cls) -> str:
+        return "volume"
+
+    @classmethod
+    @property
+    def default_parameter(cls) -> music_parameters.abc.Pitch:
+        return music_parameters.DirectVolume(-6)
+
+    @property
+    def decibel(self):
+        return self.value_at(0)
 
-    :param decibel: The decibel of the :class:`DecibelVolume` object (should be
-        from -120 to 0).
+
+class AmplitudeVolume(music_parameters.abc.Volume):
+    """A simple volume class that gets directly initialised by its amplitude.
+
+    :param amplitude: The amplitude of the :class:`DirectVolume` object.
 
     May be used when a converter class needs a volume object, but there is
     no need or desire for a complex abstraction of the respective volume.
     """
 
-    def __init__(self, decibel: core_constants.Real):
-        self._decibel = decibel
+    def __init__(self, amplitude: core_constants.Real):
+        self._amplitude = amplitude
 
     @property
-    def decibel(self) -> core_constants.Real:
-        return self._decibel
+    def amplitude(self) -> core_constants.Real:
+        return self._amplitude
 
-    @decibel.setter
-    def decibel(self, decibel: core_constants.Real):
-        self._decibel = decibel
+    @amplitude.setter
+    def amplitude(self, amplitude: float) -> core_constants.Real:
+        self._amplitude = amplitude
 
     @property
-    def amplitude(self) -> core_constants.Real:
-        return self.decibel_to_amplitude_ratio(self.decibel)
+    def decibel(self) -> float:
+        return self.amplitude_ratio_to_decibel(self.amplitude)
 
     def __repr__(self) -> str:
         return "{}({})".format(type(self).__name__, self.amplitude)
 
 
 class WesternVolume(music_parameters.abc.Volume):
     """Volume with a traditional Western nomenclature.
@@ -224,11 +256,7 @@
                 f"are '{music_parameters.constants.DYNAMIC_INDICATOR_TUPLE}'."
             )
         self._name = name
 
     @property
     def decibel(self) -> core_constants.Real:
         return self._dynamic_indicator_to_decibel_mapping[self.name]
-
-    @property
-    def amplitude(self) -> core_constants.Real:
-        return self.decibel_to_amplitude_ratio(self.decibel)
```

### Comparing `mutwo.music-0.26.1/mutwo/music_utilities/exceptions.py` & `mutwo_music-0.27.0/mutwo/music_utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.1/mutwo/music_utilities/indicator_collection_parsers.py` & `mutwo_music-0.27.0/mutwo/music_utilities/indicator_collection_parsers.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.1/mutwo/music_utilities/tools.py` & `mutwo_music-0.27.0/mutwo/music_utilities/tools.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.26.1/mutwo.music.egg-info/PKG-INFO` & `mutwo_music-0.27.0/mutwo.music.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutwo.music
-Version: 0.26.1
+Version: 0.27.0
 Summary: music extension for event based framework for generative art
 Home-page: https://github.com/mutwo-org/mutwo.music
 Author: Levin Eric Zimmermann
 Author-email: levin.eric.zimmermann@posteo.eu
 License: GPL
 Project-URL: Documentation, https://mutwo-org.github.io
 Classifier: Development Status :: 3 - Alpha
@@ -19,15 +19,15 @@
 Classifier: Topic :: Artistic Software
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Sound/Audio :: MIDI
 Requires-Python: >=3.10, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mutwo.core<2.0.0,>=1.3.0
+Requires-Dist: mutwo.core<3.0.0,>=2.0.0
 Requires-Dist: epitran<1.25,>=1.23
 Requires-Dist: sympy<2.0.0,>=1.10.1
 Requires-Dist: python-ranges<2.0.0,>=1.2.0
 Provides-Extra: testing
 Requires-Dist: pytest>=7.1.1; extra == "testing"
 
 # mutwo.music
```

### Comparing `mutwo.music-0.26.1/mutwo.music.egg-info/SOURCES.txt` & `mutwo_music-0.27.0/mutwo.music.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 mutwo/music_parameters/instruments/__init__.py
 mutwo/music_parameters/instruments/general.py
 mutwo/music_parameters/lyrics/__init__.py
 mutwo/music_parameters/lyrics/text_based_lyrics.py
 mutwo/music_parameters/pitches/CommonHarmonic.py
 mutwo/music_parameters/pitches/DirectPitch.py
 mutwo/music_parameters/pitches/EqualDividedOctavePitch.py
+mutwo/music_parameters/pitches/FlexPitch.py
 mutwo/music_parameters/pitches/JustIntonationPitch.py
 mutwo/music_parameters/pitches/MidiPitch.py
 mutwo/music_parameters/pitches/ScalePitch.py
 mutwo/music_parameters/pitches/WesternPitch.py
 mutwo/music_parameters/pitches/__init__.py
 mutwo/music_utilities/__init__.py
 mutwo/music_utilities/exceptions.py
```

### Comparing `mutwo.music-0.26.1/setup.py` & `mutwo_music-0.27.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         for package in setuptools.find_namespace_packages(
             include=["mutwo.*"]
         )
         if package[:5] != "tests"
     ],
     setup_requires=[],
     install_requires=[
-        "mutwo.core>=1.3.0, <2.0.0",
+        "mutwo.core>=2.0.0, <3.0.0",
         "epitran>=1.23, <1.25",
         "sympy>=1.10.1, <2.0.0",
         "python-ranges>=1.2.0, <2.0.0",
     ],
     extras_require=extras_require,
     classifiers=[
         "Development Status :: 3 - Alpha",
```

