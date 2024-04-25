# Comparing `tmp/enkacard-3.3.4.tar.gz` & `tmp/enkacard-3.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enkacard-3.3.4.tar", max compression
+gzip compressed data, was "enkacard-3.3.5.tar", max compression
```

## Comparing `enkacard-3.3.4.tar` & `enkacard-3.3.5.tar`

### file list

```diff
@@ -1,94 +1,94 @@
--rw-r--r--   0        0        0      313 2022-12-17 00:40:06.925303 enkacard-3.3.4/enkacard/enc_error.py
--rw-r--r--   0        0        0    10179 2024-04-18 22:10:58.709561 enkacard-3.3.4/enkacard/encbanner.py
--rw-r--r--   0        0        0     5145 2024-02-29 17:57:35.626280 enkacard-3.3.4/enkacard/enkatools.py
--rw-r--r--   0        0        0 11514084 2022-07-25 21:33:51.994087 enkacard-3.3.4/enkacard/src/assets/font/Genshin_Impact.ttf
--rw-r--r--   0        0        0    79268 2023-04-05 20:05:44.281954 enkacard-3.3.4/enkacard/src/assets/font/GSEnochian.ttf
--rw-r--r--   0        0        0     9259 2024-03-12 11:19:40.666625 enkacard-3.3.4/enkacard/src/generator/__pycache__/akasha_rank.cpython-311.pyc
--rw-r--r--   0        0        0     8281 2024-04-21 10:27:04.570454 enkacard-3.3.4/enkacard/src/generator/__pycache__/akasha_rank.cpython-312.pyc
--rw-r--r--   0        0        0    10680 2024-03-12 11:19:40.669627 enkacard-3.3.4/enkacard/src/generator/__pycache__/profile_teample_one.cpython-311.pyc
--rw-r--r--   0        0        0    11042 2024-04-21 10:27:04.572453 enkacard-3.3.4/enkacard/src/generator/__pycache__/profile_teample_one.cpython-312.pyc
--rw-r--r--   0        0        0     9363 2024-03-12 11:19:41.167913 enkacard-3.3.4/enkacard/src/generator/__pycache__/profile_teample_two.cpython-311.pyc
--rw-r--r--   0        0        0     9742 2024-04-21 10:32:16.720190 enkacard-3.3.4/enkacard/src/generator/__pycache__/profile_teample_two.cpython-312.pyc
--rw-r--r--   0        0        0    13080 2024-03-12 11:19:40.487430 enkacard-3.3.4/enkacard/src/generator/__pycache__/teample_one.cpython-311.pyc
--rw-r--r--   0        0        0    13342 2024-04-21 10:27:04.189857 enkacard-3.3.4/enkacard/src/generator/__pycache__/teample_one.cpython-312.pyc
--rw-r--r--   0        0        0    17916 2024-03-12 11:19:40.680148 enkacard-3.3.4/enkacard/src/generator/__pycache__/teample_two.cpython-311.pyc
--rw-r--r--   0        0        0    17976 2024-04-21 10:27:04.574456 enkacard-3.3.4/enkacard/src/generator/__pycache__/teample_two.cpython-312.pyc
--rw-r--r--   0        0        0     3819 2024-04-25 09:34:17.037508 enkacard-3.3.4/enkacard/src/generator/akasha_rank.py
--rw-r--r--   0        0        0    13628 2024-03-12 11:19:40.636054 enkacard-3.3.4/enkacard/src/generator/one/__pycache__/artifact.cpython-311.pyc
--rw-r--r--   0        0        0    13604 2024-04-21 10:27:04.559942 enkacard-3.3.4/enkacard/src/generator/one/__pycache__/artifact.cpython-312.pyc
--rw-r--r--   0        0        0     4882 2024-03-12 11:19:40.631536 enkacard-3.3.4/enkacard/src/generator/one/__pycache__/background.cpython-311.pyc
--rw-r--r--   0        0        0     4942 2024-04-21 10:27:04.555438 enkacard-3.3.4/enkacard/src/generator/one/__pycache__/background.cpython-312.pyc
--rw-r--r--   0        0        0     2798 2024-03-12 11:19:40.648579 enkacard-3.3.4/enkacard/src/generator/one/__pycache__/constant.cpython-311.pyc
--rw-r--r--   0        0        0     2820 2024-04-21 10:27:04.562946 enkacard-3.3.4/enkacard/src/generator/one/__pycache__/constant.cpython-312.pyc
--rw-r--r--   0        0        0     2356 2024-03-12 11:19:40.660102 enkacard-3.3.4/enkacard/src/generator/one/__pycache__/prop.cpython-311.pyc
--rw-r--r--   0        0        0     2346 2024-04-21 10:27:04.567946 enkacard-3.3.4/enkacard/src/generator/one/__pycache__/prop.cpython-312.pyc
--rw-r--r--   0        0        0     3475 2024-03-12 11:19:40.651579 enkacard-3.3.4/enkacard/src/generator/one/__pycache__/skill.cpython-311.pyc
--rw-r--r--   0        0        0     3470 2024-04-21 10:27:04.563945 enkacard-3.3.4/enkacard/src/generator/one/__pycache__/skill.cpython-312.pyc
--rw-r--r--   0        0        0    11270 2024-03-12 11:19:40.656100 enkacard-3.3.4/enkacard/src/generator/one/__pycache__/stat.cpython-311.pyc
--rw-r--r--   0        0        0    10678 2024-04-21 10:27:04.566946 enkacard-3.3.4/enkacard/src/generator/one/__pycache__/stat.cpython-312.pyc
--rw-r--r--   0        0        0     6516 2024-03-12 11:19:40.640055 enkacard-3.3.4/enkacard/src/generator/one/__pycache__/weapon.cpython-311.pyc
--rw-r--r--   0        0        0     6799 2024-04-21 10:27:04.561946 enkacard-3.3.4/enkacard/src/generator/one/__pycache__/weapon.cpython-312.pyc
--rw-r--r--   0        0        0     6657 2023-12-10 18:28:18.819703 enkacard-3.3.4/enkacard/src/generator/one/artifact.py
--rw-r--r--   0        0        0     2363 2023-12-03 21:02:32.344488 enkacard-3.3.4/enkacard/src/generator/one/background.py
--rw-r--r--   0        0        0     1235 2023-12-10 20:39:47.204162 enkacard-3.3.4/enkacard/src/generator/one/constant.py
--rw-r--r--   0        0        0      869 2023-12-01 21:40:04.470207 enkacard-3.3.4/enkacard/src/generator/one/prop.py
--rw-r--r--   0        0        0     1378 2023-12-21 20:00:52.547008 enkacard-3.3.4/enkacard/src/generator/one/skill.py
--rw-r--r--   0        0        0     5749 2023-12-07 00:50:46.885608 enkacard-3.3.4/enkacard/src/generator/one/stat.py
--rw-r--r--   0        0        0     2989 2023-12-23 01:15:33.050226 enkacard-3.3.4/enkacard/src/generator/one/weapon.py
--rw-r--r--   0        0        0     6132 2024-01-06 15:22:38.238244 enkacard-3.3.4/enkacard/src/generator/profile_teample_one.py
--rw-r--r--   0        0        0     5229 2024-04-21 10:32:11.269924 enkacard-3.3.4/enkacard/src/generator/profile_teample_two.py
--rw-r--r--   0        0        0     6711 2023-12-21 20:25:56.721897 enkacard-3.3.4/enkacard/src/generator/teample_one.py
--rw-r--r--   0        0        0     9909 2024-01-06 15:59:41.426611 enkacard-3.3.4/enkacard/src/generator/teample_two.py
--rw-r--r--   0        0        0    12705 2024-03-12 11:19:41.160400 enkacard-3.3.4/enkacard/src/generator/two/__pycache__/artifact.cpython-311.pyc
--rw-r--r--   0        0        0    12704 2024-04-21 10:27:04.967692 enkacard-3.3.4/enkacard/src/generator/two/__pycache__/artifact.cpython-312.pyc
--rw-r--r--   0        0        0     5973 2024-03-12 11:19:41.156399 enkacard-3.3.4/enkacard/src/generator/two/__pycache__/background.cpython-311.pyc
--rw-r--r--   0        0        0     6096 2024-04-21 10:27:04.963691 enkacard-3.3.4/enkacard/src/generator/two/__pycache__/background.cpython-312.pyc
--rw-r--r--   0        0        0     3475 2024-03-12 11:19:41.165913 enkacard-3.3.4/enkacard/src/generator/two/__pycache__/skill.cpython-311.pyc
--rw-r--r--   0        0        0     3470 2024-04-21 10:27:04.971200 enkacard-3.3.4/enkacard/src/generator/two/__pycache__/skill.cpython-312.pyc
--rw-r--r--   0        0        0     7278 2024-03-12 11:19:41.163914 enkacard-3.3.4/enkacard/src/generator/two/__pycache__/stat.cpython-311.pyc
--rw-r--r--   0        0        0     6910 2024-04-21 10:27:04.970200 enkacard-3.3.4/enkacard/src/generator/two/__pycache__/stat.cpython-312.pyc
--rw-r--r--   0        0        0     6377 2023-12-18 23:30:42.003393 enkacard-3.3.4/enkacard/src/generator/two/artifact.py
--rw-r--r--   0        0        0     3034 2023-12-17 22:37:02.037270 enkacard-3.3.4/enkacard/src/generator/two/background.py
--rw-r--r--   0        0        0     1368 2023-12-21 20:52:29.332377 enkacard-3.3.4/enkacard/src/generator/two/skill.py
--rw-r--r--   0        0        0     3346 2023-12-21 19:58:52.526652 enkacard-3.3.4/enkacard/src/generator/two/stat.py
--rw-r--r--   0        0        0     7501 2024-03-12 11:19:40.462381 enkacard-3.3.4/enkacard/src/modal/__pycache__/enkacardCread.cpython-311.pyc
--rw-r--r--   0        0        0     5542 2024-04-21 10:27:04.184354 enkacard-3.3.4/enkacard/src/modal/__pycache__/enkacardCread.cpython-312.pyc
--rw-r--r--   0        0        0     2072 2024-03-12 11:19:39.704683 enkacard-3.3.4/enkacard/src/modal/__pycache__/enkaToolsModel.cpython-311.pyc
--rw-r--r--   0        0        0     1604 2024-04-21 10:27:03.631178 enkacard-3.3.4/enkacard/src/modal/__pycache__/enkaToolsModel.cpython-312.pyc
--rw-r--r--   0        0        0     2553 2024-03-12 11:14:42.124404 enkacard-3.3.4/enkacard/src/modal/enkacardCread.py
--rw-r--r--   0        0        0      771 2023-12-17 22:08:52.342906 enkacard-3.3.4/enkacard/src/modal/enkaToolsModel.py
--rw-r--r--   0        0        0    59616 2023-12-25 12:23:22.739379 enkacard-3.3.4/enkacard/src/pickle_cashe/data_characters.pkz
--rw-r--r--   0        0        0        0 2023-12-25 12:23:29.173879 enkacard-3.3.4/enkacard/src/pickle_cashe/data_characters.pkz~
--rw-r--r--   0        0        0    10697 2024-03-12 11:19:40.352607 enkacard-3.3.4/enkacard/src/utils/__pycache__/affixes.cpython-311.pyc
--rw-r--r--   0        0        0     9733 2024-04-21 10:27:03.963075 enkacard-3.3.4/enkacard/src/utils/__pycache__/affixes.cpython-312.pyc
--rw-r--r--   0        0        0     7570 2024-03-12 11:19:40.683655 enkacard-3.3.4/enkacard/src/utils/__pycache__/diagram.cpython-311.pyc
--rw-r--r--   0        0        0     5714 2024-04-21 10:27:04.576454 enkacard-3.3.4/enkacard/src/utils/__pycache__/diagram.cpython-312.pyc
--rw-r--r--   0        0        0     9027 2024-03-12 11:19:40.448351 enkacard-3.3.4/enkacard/src/utils/__pycache__/git.cpython-311.pyc
--rw-r--r--   0        0        0     8437 2024-04-21 10:27:04.160338 enkacard-3.3.4/enkacard/src/utils/__pycache__/git.cpython-312.pyc
--rw-r--r--   0        0        0     6844 2024-03-12 11:19:40.348101 enkacard-3.3.4/enkacard/src/utils/__pycache__/options.cpython-311.pyc
--rw-r--r--   0        0        0     5947 2024-04-21 10:27:03.960076 enkacard-3.3.4/enkacard/src/utils/__pycache__/options.cpython-312.pyc
--rw-r--r--   0        0        0    11433 2024-03-12 11:19:40.451353 enkacard-3.3.4/enkacard/src/utils/__pycache__/pickle_cashe.cpython-311.pyc
--rw-r--r--   0        0        0     9513 2024-04-21 10:27:04.163336 enkacard-3.3.4/enkacard/src/utils/__pycache__/pickle_cashe.cpython-312.pyc
--rw-r--r--   0        0        0    33153 2024-03-12 11:19:40.497955 enkacard-3.3.4/enkacard/src/utils/__pycache__/pill.cpython-311.pyc
--rw-r--r--   0        0        0    29897 2024-04-21 10:27:04.197863 enkacard-3.3.4/enkacard/src/utils/__pycache__/pill.cpython-312.pyc
--rw-r--r--   0        0        0     1552 2024-03-12 11:19:40.457867 enkacard-3.3.4/enkacard/src/utils/__pycache__/translation.cpython-311.pyc
--rw-r--r--   0        0        0     1494 2024-04-21 10:27:04.183353 enkacard-3.3.4/enkacard/src/utils/__pycache__/translation.cpython-312.pyc
--rw-r--r--   0        0        0    18462 2023-11-30 22:40:24.144568 enkacard-3.3.4/enkacard/src/utils/affixes.py
--rw-r--r--   0        0        0     3501 2024-04-18 22:05:34.318028 enkacard-3.3.4/enkacard/src/utils/diagram.py
--rw-r--r--   0        0        0     1317 2024-03-12 11:19:40.127631 enkacard-3.3.4/enkacard/src/utils/enkanetwork_update/__pycache__/config.cpython-311.pyc
--rw-r--r--   0        0        0     1281 2024-04-25 09:25:21.427292 enkacard-3.3.4/enkacard/src/utils/enkanetwork_update/__pycache__/config.cpython-312.pyc
--rw-r--r--   0        0        0    18978 2024-03-12 11:19:39.931560 enkacard-3.3.4/enkacard/src/utils/enkanetwork_update/__pycache__/enka_update.cpython-311.pyc
--rw-r--r--   0        0        0    15771 2024-04-25 09:29:12.217664 enkacard-3.3.4/enkacard/src/utils/enkanetwork_update/__pycache__/enka_update.cpython-312.pyc
--rw-r--r--   0        0        0     1044 2024-03-12 11:19:40.123621 enkacard-3.3.4/enkacard/src/utils/enkanetwork_update/__pycache__/pathfinding.cpython-311.pyc
--rw-r--r--   0        0        0     1006 2024-04-25 09:19:48.951886 enkacard-3.3.4/enkacard/src/utils/enkanetwork_update/__pycache__/pathfinding.cpython-312.pyc
--rw-r--r--   0        0        0     1510 2024-04-25 09:25:17.101442 enkacard-3.3.4/enkacard/src/utils/enkanetwork_update/config.py
--rw-r--r--   0        0        0    11477 2024-04-25 09:31:54.863565 enkacard-3.3.4/enkacard/src/utils/enkanetwork_update/enka_update.py
--rw-r--r--   0        0        0      537 2024-04-25 09:17:51.407630 enkacard-3.3.4/enkacard/src/utils/enkanetwork_update/pathfinding.py
--rw-r--r--   0        0        0     5722 2023-12-25 11:21:01.889033 enkacard-3.3.4/enkacard/src/utils/git.py
--rw-r--r--   0        0        0     3977 2024-04-18 22:11:07.156131 enkacard-3.3.4/enkacard/src/utils/options.py
--rw-r--r--   0        0        0     6868 2023-12-13 21:43:08.363154 enkacard-3.3.4/enkacard/src/utils/pickle_cashe.py
--rw-r--r--   0        0        0    17229 2023-12-23 00:44:36.688489 enkacard-3.3.4/enkacard/src/utils/pill.py
--rw-r--r--   0        0        0     1852 2023-04-05 20:09:26.777243 enkacard-3.3.4/enkacard/src/utils/translation.py
--rw-r--r--   0        0        0      875 2024-04-25 09:34:05.419397 enkacard-3.3.4/pyproject.toml
--rw-r--r--   0        0        0     3699 2023-12-23 16:26:14.431089 enkacard-3.3.4/README.md
--rw-r--r--   0        0        0     4648 1970-01-01 00:00:00.000000 enkacard-3.3.4/PKG-INFO
+-rw-r--r--   0        0        0      313 2022-12-17 00:40:06.925303 enkacard-3.3.5/enkacard/enc_error.py
+-rw-r--r--   0        0        0    10179 2024-04-18 22:10:58.709561 enkacard-3.3.5/enkacard/encbanner.py
+-rw-r--r--   0        0        0     5145 2024-02-29 17:57:35.626280 enkacard-3.3.5/enkacard/enkatools.py
+-rw-r--r--   0        0        0 11514084 2022-07-25 21:33:51.994087 enkacard-3.3.5/enkacard/src/assets/font/Genshin_Impact.ttf
+-rw-r--r--   0        0        0    79268 2023-04-05 20:05:44.281954 enkacard-3.3.5/enkacard/src/assets/font/GSEnochian.ttf
+-rw-r--r--   0        0        0     9259 2024-03-12 11:19:40.666625 enkacard-3.3.5/enkacard/src/generator/__pycache__/akasha_rank.cpython-311.pyc
+-rw-r--r--   0        0        0     8281 2024-04-21 10:27:04.570454 enkacard-3.3.5/enkacard/src/generator/__pycache__/akasha_rank.cpython-312.pyc
+-rw-r--r--   0        0        0    10680 2024-03-12 11:19:40.669627 enkacard-3.3.5/enkacard/src/generator/__pycache__/profile_teample_one.cpython-311.pyc
+-rw-r--r--   0        0        0    11042 2024-04-21 10:27:04.572453 enkacard-3.3.5/enkacard/src/generator/__pycache__/profile_teample_one.cpython-312.pyc
+-rw-r--r--   0        0        0     9363 2024-03-12 11:19:41.167913 enkacard-3.3.5/enkacard/src/generator/__pycache__/profile_teample_two.cpython-311.pyc
+-rw-r--r--   0        0        0     9742 2024-04-21 10:32:16.720190 enkacard-3.3.5/enkacard/src/generator/__pycache__/profile_teample_two.cpython-312.pyc
+-rw-r--r--   0        0        0    13080 2024-03-12 11:19:40.487430 enkacard-3.3.5/enkacard/src/generator/__pycache__/teample_one.cpython-311.pyc
+-rw-r--r--   0        0        0    13342 2024-04-21 10:27:04.189857 enkacard-3.3.5/enkacard/src/generator/__pycache__/teample_one.cpython-312.pyc
+-rw-r--r--   0        0        0    17916 2024-03-12 11:19:40.680148 enkacard-3.3.5/enkacard/src/generator/__pycache__/teample_two.cpython-311.pyc
+-rw-r--r--   0        0        0    17976 2024-04-21 10:27:04.574456 enkacard-3.3.5/enkacard/src/generator/__pycache__/teample_two.cpython-312.pyc
+-rw-r--r--   0        0        0     3819 2024-04-25 09:34:17.037508 enkacard-3.3.5/enkacard/src/generator/akasha_rank.py
+-rw-r--r--   0        0        0    13628 2024-03-12 11:19:40.636054 enkacard-3.3.5/enkacard/src/generator/one/__pycache__/artifact.cpython-311.pyc
+-rw-r--r--   0        0        0    13604 2024-04-21 10:27:04.559942 enkacard-3.3.5/enkacard/src/generator/one/__pycache__/artifact.cpython-312.pyc
+-rw-r--r--   0        0        0     4882 2024-03-12 11:19:40.631536 enkacard-3.3.5/enkacard/src/generator/one/__pycache__/background.cpython-311.pyc
+-rw-r--r--   0        0        0     4942 2024-04-21 10:27:04.555438 enkacard-3.3.5/enkacard/src/generator/one/__pycache__/background.cpython-312.pyc
+-rw-r--r--   0        0        0     2798 2024-03-12 11:19:40.648579 enkacard-3.3.5/enkacard/src/generator/one/__pycache__/constant.cpython-311.pyc
+-rw-r--r--   0        0        0     2820 2024-04-21 10:27:04.562946 enkacard-3.3.5/enkacard/src/generator/one/__pycache__/constant.cpython-312.pyc
+-rw-r--r--   0        0        0     2356 2024-03-12 11:19:40.660102 enkacard-3.3.5/enkacard/src/generator/one/__pycache__/prop.cpython-311.pyc
+-rw-r--r--   0        0        0     2346 2024-04-21 10:27:04.567946 enkacard-3.3.5/enkacard/src/generator/one/__pycache__/prop.cpython-312.pyc
+-rw-r--r--   0        0        0     3475 2024-03-12 11:19:40.651579 enkacard-3.3.5/enkacard/src/generator/one/__pycache__/skill.cpython-311.pyc
+-rw-r--r--   0        0        0     3470 2024-04-21 10:27:04.563945 enkacard-3.3.5/enkacard/src/generator/one/__pycache__/skill.cpython-312.pyc
+-rw-r--r--   0        0        0    11270 2024-03-12 11:19:40.656100 enkacard-3.3.5/enkacard/src/generator/one/__pycache__/stat.cpython-311.pyc
+-rw-r--r--   0        0        0    10678 2024-04-21 10:27:04.566946 enkacard-3.3.5/enkacard/src/generator/one/__pycache__/stat.cpython-312.pyc
+-rw-r--r--   0        0        0     6516 2024-03-12 11:19:40.640055 enkacard-3.3.5/enkacard/src/generator/one/__pycache__/weapon.cpython-311.pyc
+-rw-r--r--   0        0        0     6799 2024-04-21 10:27:04.561946 enkacard-3.3.5/enkacard/src/generator/one/__pycache__/weapon.cpython-312.pyc
+-rw-r--r--   0        0        0     6657 2023-12-10 18:28:18.819703 enkacard-3.3.5/enkacard/src/generator/one/artifact.py
+-rw-r--r--   0        0        0     2363 2023-12-03 21:02:32.344488 enkacard-3.3.5/enkacard/src/generator/one/background.py
+-rw-r--r--   0        0        0     1235 2023-12-10 20:39:47.204162 enkacard-3.3.5/enkacard/src/generator/one/constant.py
+-rw-r--r--   0        0        0      869 2023-12-01 21:40:04.470207 enkacard-3.3.5/enkacard/src/generator/one/prop.py
+-rw-r--r--   0        0        0     1378 2023-12-21 20:00:52.547008 enkacard-3.3.5/enkacard/src/generator/one/skill.py
+-rw-r--r--   0        0        0     5749 2023-12-07 00:50:46.885608 enkacard-3.3.5/enkacard/src/generator/one/stat.py
+-rw-r--r--   0        0        0     2989 2023-12-23 01:15:33.050226 enkacard-3.3.5/enkacard/src/generator/one/weapon.py
+-rw-r--r--   0        0        0     6132 2024-01-06 15:22:38.238244 enkacard-3.3.5/enkacard/src/generator/profile_teample_one.py
+-rw-r--r--   0        0        0     5229 2024-04-21 10:32:11.269924 enkacard-3.3.5/enkacard/src/generator/profile_teample_two.py
+-rw-r--r--   0        0        0     6711 2023-12-21 20:25:56.721897 enkacard-3.3.5/enkacard/src/generator/teample_one.py
+-rw-r--r--   0        0        0     9909 2024-01-06 15:59:41.426611 enkacard-3.3.5/enkacard/src/generator/teample_two.py
+-rw-r--r--   0        0        0    12705 2024-03-12 11:19:41.160400 enkacard-3.3.5/enkacard/src/generator/two/__pycache__/artifact.cpython-311.pyc
+-rw-r--r--   0        0        0    12704 2024-04-21 10:27:04.967692 enkacard-3.3.5/enkacard/src/generator/two/__pycache__/artifact.cpython-312.pyc
+-rw-r--r--   0        0        0     5973 2024-03-12 11:19:41.156399 enkacard-3.3.5/enkacard/src/generator/two/__pycache__/background.cpython-311.pyc
+-rw-r--r--   0        0        0     6096 2024-04-21 10:27:04.963691 enkacard-3.3.5/enkacard/src/generator/two/__pycache__/background.cpython-312.pyc
+-rw-r--r--   0        0        0     3475 2024-03-12 11:19:41.165913 enkacard-3.3.5/enkacard/src/generator/two/__pycache__/skill.cpython-311.pyc
+-rw-r--r--   0        0        0     3470 2024-04-21 10:27:04.971200 enkacard-3.3.5/enkacard/src/generator/two/__pycache__/skill.cpython-312.pyc
+-rw-r--r--   0        0        0     7278 2024-03-12 11:19:41.163914 enkacard-3.3.5/enkacard/src/generator/two/__pycache__/stat.cpython-311.pyc
+-rw-r--r--   0        0        0     6910 2024-04-21 10:27:04.970200 enkacard-3.3.5/enkacard/src/generator/two/__pycache__/stat.cpython-312.pyc
+-rw-r--r--   0        0        0     6377 2023-12-18 23:30:42.003393 enkacard-3.3.5/enkacard/src/generator/two/artifact.py
+-rw-r--r--   0        0        0     3034 2023-12-17 22:37:02.037270 enkacard-3.3.5/enkacard/src/generator/two/background.py
+-rw-r--r--   0        0        0     1368 2023-12-21 20:52:29.332377 enkacard-3.3.5/enkacard/src/generator/two/skill.py
+-rw-r--r--   0        0        0     3346 2023-12-21 19:58:52.526652 enkacard-3.3.5/enkacard/src/generator/two/stat.py
+-rw-r--r--   0        0        0     7501 2024-03-12 11:19:40.462381 enkacard-3.3.5/enkacard/src/modal/__pycache__/enkacardCread.cpython-311.pyc
+-rw-r--r--   0        0        0     5542 2024-04-21 10:27:04.184354 enkacard-3.3.5/enkacard/src/modal/__pycache__/enkacardCread.cpython-312.pyc
+-rw-r--r--   0        0        0     2072 2024-03-12 11:19:39.704683 enkacard-3.3.5/enkacard/src/modal/__pycache__/enkaToolsModel.cpython-311.pyc
+-rw-r--r--   0        0        0     1604 2024-04-21 10:27:03.631178 enkacard-3.3.5/enkacard/src/modal/__pycache__/enkaToolsModel.cpython-312.pyc
+-rw-r--r--   0        0        0     2553 2024-03-12 11:14:42.124404 enkacard-3.3.5/enkacard/src/modal/enkacardCread.py
+-rw-r--r--   0        0        0      771 2023-12-17 22:08:52.342906 enkacard-3.3.5/enkacard/src/modal/enkaToolsModel.py
+-rw-r--r--   0        0        0    59616 2023-12-25 12:23:22.739379 enkacard-3.3.5/enkacard/src/pickle_cashe/data_characters.pkz
+-rw-r--r--   0        0        0        0 2023-12-25 12:23:29.173879 enkacard-3.3.5/enkacard/src/pickle_cashe/data_characters.pkz~
+-rw-r--r--   0        0        0    10697 2024-03-12 11:19:40.352607 enkacard-3.3.5/enkacard/src/utils/__pycache__/affixes.cpython-311.pyc
+-rw-r--r--   0        0        0     9733 2024-04-21 10:27:03.963075 enkacard-3.3.5/enkacard/src/utils/__pycache__/affixes.cpython-312.pyc
+-rw-r--r--   0        0        0     7570 2024-03-12 11:19:40.683655 enkacard-3.3.5/enkacard/src/utils/__pycache__/diagram.cpython-311.pyc
+-rw-r--r--   0        0        0     5714 2024-04-21 10:27:04.576454 enkacard-3.3.5/enkacard/src/utils/__pycache__/diagram.cpython-312.pyc
+-rw-r--r--   0        0        0     9027 2024-03-12 11:19:40.448351 enkacard-3.3.5/enkacard/src/utils/__pycache__/git.cpython-311.pyc
+-rw-r--r--   0        0        0     8437 2024-04-21 10:27:04.160338 enkacard-3.3.5/enkacard/src/utils/__pycache__/git.cpython-312.pyc
+-rw-r--r--   0        0        0     6844 2024-03-12 11:19:40.348101 enkacard-3.3.5/enkacard/src/utils/__pycache__/options.cpython-311.pyc
+-rw-r--r--   0        0        0     5947 2024-04-21 10:27:03.960076 enkacard-3.3.5/enkacard/src/utils/__pycache__/options.cpython-312.pyc
+-rw-r--r--   0        0        0    11433 2024-03-12 11:19:40.451353 enkacard-3.3.5/enkacard/src/utils/__pycache__/pickle_cashe.cpython-311.pyc
+-rw-r--r--   0        0        0     9513 2024-04-21 10:27:04.163336 enkacard-3.3.5/enkacard/src/utils/__pycache__/pickle_cashe.cpython-312.pyc
+-rw-r--r--   0        0        0    33153 2024-03-12 11:19:40.497955 enkacard-3.3.5/enkacard/src/utils/__pycache__/pill.cpython-311.pyc
+-rw-r--r--   0        0        0    29897 2024-04-21 10:27:04.197863 enkacard-3.3.5/enkacard/src/utils/__pycache__/pill.cpython-312.pyc
+-rw-r--r--   0        0        0     1552 2024-03-12 11:19:40.457867 enkacard-3.3.5/enkacard/src/utils/__pycache__/translation.cpython-311.pyc
+-rw-r--r--   0        0        0     1494 2024-04-21 10:27:04.183353 enkacard-3.3.5/enkacard/src/utils/__pycache__/translation.cpython-312.pyc
+-rw-r--r--   0        0        0    18462 2023-11-30 22:40:24.144568 enkacard-3.3.5/enkacard/src/utils/affixes.py
+-rw-r--r--   0        0        0     3501 2024-04-18 22:05:34.318028 enkacard-3.3.5/enkacard/src/utils/diagram.py
+-rw-r--r--   0        0        0     1317 2024-03-12 11:19:40.127631 enkacard-3.3.5/enkacard/src/utils/enkanetwork_update/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0        0        0     1281 2024-04-25 09:25:21.427292 enkacard-3.3.5/enkacard/src/utils/enkanetwork_update/__pycache__/config.cpython-312.pyc
+-rw-r--r--   0        0        0    18978 2024-03-12 11:19:39.931560 enkacard-3.3.5/enkacard/src/utils/enkanetwork_update/__pycache__/enka_update.cpython-311.pyc
+-rw-r--r--   0        0        0    15771 2024-04-25 09:29:12.217664 enkacard-3.3.5/enkacard/src/utils/enkanetwork_update/__pycache__/enka_update.cpython-312.pyc
+-rw-r--r--   0        0        0     1044 2024-03-12 11:19:40.123621 enkacard-3.3.5/enkacard/src/utils/enkanetwork_update/__pycache__/pathfinding.cpython-311.pyc
+-rw-r--r--   0        0        0     1006 2024-04-25 09:19:48.951886 enkacard-3.3.5/enkacard/src/utils/enkanetwork_update/__pycache__/pathfinding.cpython-312.pyc
+-rw-r--r--   0        0        0     1510 2024-04-25 09:25:17.101442 enkacard-3.3.5/enkacard/src/utils/enkanetwork_update/config.py
+-rw-r--r--   0        0        0    11477 2024-04-25 09:31:54.863565 enkacard-3.3.5/enkacard/src/utils/enkanetwork_update/enka_update.py
+-rw-r--r--   0        0        0      537 2024-04-25 09:17:51.407630 enkacard-3.3.5/enkacard/src/utils/enkanetwork_update/pathfinding.py
+-rw-r--r--   0        0        0     5722 2023-12-25 11:21:01.889033 enkacard-3.3.5/enkacard/src/utils/git.py
+-rw-r--r--   0        0        0     3977 2024-04-18 22:11:07.156131 enkacard-3.3.5/enkacard/src/utils/options.py
+-rw-r--r--   0        0        0     6868 2023-12-13 21:43:08.363154 enkacard-3.3.5/enkacard/src/utils/pickle_cashe.py
+-rw-r--r--   0        0        0    17229 2023-12-23 00:44:36.688489 enkacard-3.3.5/enkacard/src/utils/pill.py
+-rw-r--r--   0        0        0     1852 2023-04-05 20:09:26.777243 enkacard-3.3.5/enkacard/src/utils/translation.py
+-rw-r--r--   0        0        0      870 2024-04-25 10:05:30.157601 enkacard-3.3.5/pyproject.toml
+-rw-r--r--   0        0        0     3699 2023-12-23 16:26:14.431089 enkacard-3.3.5/README.md
+-rw-r--r--   0        0        0     4631 1970-01-01 00:00:00.000000 enkacard-3.3.5/PKG-INFO
```

### Comparing `enkacard-3.3.4/enkacard/encbanner.py` & `enkacard-3.3.5/enkacard/encbanner.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/enkatools.py` & `enkacard-3.3.5/enkacard/enkatools.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/assets/font/Genshin_Impact.ttf` & `enkacard-3.3.5/enkacard/src/assets/font/Genshin_Impact.ttf`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/assets/font/GSEnochian.ttf` & `enkacard-3.3.5/enkacard/src/assets/font/GSEnochian.ttf`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/generator/__pycache__/akasha_rank.cpython-311.pyc` & `enkacard-3.3.5/enkacard/src/generator/__pycache__/akasha_rank.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/generator/__pycache__/akasha_rank.cpython-312.pyc` & `enkacard-3.3.5/enkacard/src/generator/__pycache__/akasha_rank.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/generator/__pycache__/profile_teample_one.cpython-311.pyc` & `enkacard-3.3.5/enkacard/src/generator/__pycache__/profile_teample_one.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/generator/__pycache__/profile_teample_one.cpython-312.pyc` & `enkacard-3.3.5/enkacard/src/generator/__pycache__/profile_teample_one.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/generator/__pycache__/profile_teample_two.cpython-311.pyc` & `enkacard-3.3.5/enkacard/src/generator/__pycache__/profile_teample_two.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/generator/__pycache__/profile_teample_two.cpython-312.pyc` & `enkacard-3.3.5/enkacard/src/generator/__pycache__/profile_teample_two.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/generator/__pycache__/teample_one.cpython-311.pyc` & `enkacard-3.3.5/enkacard/src/generator/__pycache__/teample_one.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/generator/__pycache__/teample_one.cpython-312.pyc` & `enkacard-3.3.5/enkacard/src/generator/__pycache__/teample_one.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/generator/__pycache__/teample_two.cpython-311.pyc` & `enkacard-3.3.5/enkacard/src/generator/__pycache__/teample_two.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/generator/__pycache__/teample_two.cpython-312.pyc` & `enkacard-3.3.5/enkacard/src/generator/__pycache__/teample_two.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/generator/akasha_rank.py` & `enkacard-3.3.5/enkacard/src/generator/akasha_rank.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/generator/one/__pycache__/artifact.cpython-311.pyc` & `enkacard-3.3.5/enkacard/src/generator/one/__pycache__/artifact.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/generator/one/__pycache__/artifact.cpython-312.pyc` & `enkacard-3.3.5/enkacard/src/generator/one/__pycache__/artifact.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/generator/one/__pycache__/background.cpython-311.pyc` & `enkacard-3.3.5/enkacard/src/generator/one/__pycache__/background.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/generator/one/__pycache__/background.cpython-312.pyc` & `enkacard-3.3.5/enkacard/src/generator/one/__pycache__/background.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/generator/one/__pycache__/constant.cpython-311.pyc` & `enkacard-3.3.5/enkacard/src/generator/one/__pycache__/constant.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/generator/one/__pycache__/constant.cpython-312.pyc` & `enkacard-3.3.5/enkacard/src/generator/one/__pycache__/constant.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/generator/one/__pycache__/prop.cpython-311.pyc` & `enkacard-3.3.5/enkacard/src/generator/one/__pycache__/prop.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/generator/one/__pycache__/prop.cpython-312.pyc` & `enkacard-3.3.5/enkacard/src/generator/one/__pycache__/prop.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/generator/one/__pycache__/skill.cpython-311.pyc` & `enkacard-3.3.5/enkacard/src/generator/one/__pycache__/skill.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/generator/one/__pycache__/skill.cpython-312.pyc` & `enkacard-3.3.5/enkacard/src/generator/one/__pycache__/skill.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/generator/one/__pycache__/stat.cpython-311.pyc` & `enkacard-3.3.5/enkacard/src/generator/one/__pycache__/stat.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/generator/one/__pycache__/stat.cpython-312.pyc` & `enkacard-3.3.5/enkacard/src/generator/one/__pycache__/stat.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/generator/one/__pycache__/weapon.cpython-311.pyc` & `enkacard-3.3.5/enkacard/src/generator/one/__pycache__/weapon.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/generator/one/__pycache__/weapon.cpython-312.pyc` & `enkacard-3.3.5/enkacard/src/generator/one/__pycache__/weapon.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/generator/one/artifact.py` & `enkacard-3.3.5/enkacard/src/generator/one/artifact.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/generator/one/background.py` & `enkacard-3.3.5/enkacard/src/generator/one/background.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/generator/one/constant.py` & `enkacard-3.3.5/enkacard/src/generator/one/constant.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/generator/one/prop.py` & `enkacard-3.3.5/enkacard/src/generator/one/prop.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/generator/one/skill.py` & `enkacard-3.3.5/enkacard/src/generator/one/skill.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/generator/one/stat.py` & `enkacard-3.3.5/enkacard/src/generator/one/stat.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/generator/one/weapon.py` & `enkacard-3.3.5/enkacard/src/generator/one/weapon.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/generator/profile_teample_one.py` & `enkacard-3.3.5/enkacard/src/generator/profile_teample_one.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/generator/profile_teample_two.py` & `enkacard-3.3.5/enkacard/src/generator/profile_teample_two.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/generator/teample_one.py` & `enkacard-3.3.5/enkacard/src/generator/teample_one.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/generator/teample_two.py` & `enkacard-3.3.5/enkacard/src/generator/teample_two.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/generator/two/__pycache__/artifact.cpython-311.pyc` & `enkacard-3.3.5/enkacard/src/generator/two/__pycache__/artifact.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/generator/two/__pycache__/artifact.cpython-312.pyc` & `enkacard-3.3.5/enkacard/src/generator/two/__pycache__/artifact.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/generator/two/__pycache__/background.cpython-311.pyc` & `enkacard-3.3.5/enkacard/src/generator/two/__pycache__/background.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/generator/two/__pycache__/background.cpython-312.pyc` & `enkacard-3.3.5/enkacard/src/generator/two/__pycache__/background.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/generator/two/__pycache__/skill.cpython-311.pyc` & `enkacard-3.3.5/enkacard/src/generator/two/__pycache__/skill.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/generator/two/__pycache__/skill.cpython-312.pyc` & `enkacard-3.3.5/enkacard/src/generator/two/__pycache__/skill.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/generator/two/__pycache__/stat.cpython-311.pyc` & `enkacard-3.3.5/enkacard/src/generator/two/__pycache__/stat.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/generator/two/__pycache__/stat.cpython-312.pyc` & `enkacard-3.3.5/enkacard/src/generator/two/__pycache__/stat.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/generator/two/artifact.py` & `enkacard-3.3.5/enkacard/src/generator/two/artifact.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/generator/two/background.py` & `enkacard-3.3.5/enkacard/src/generator/two/background.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/generator/two/skill.py` & `enkacard-3.3.5/enkacard/src/generator/two/skill.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/generator/two/stat.py` & `enkacard-3.3.5/enkacard/src/generator/two/stat.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/modal/__pycache__/enkacardCread.cpython-311.pyc` & `enkacard-3.3.5/enkacard/src/modal/__pycache__/enkacardCread.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/modal/__pycache__/enkacardCread.cpython-312.pyc` & `enkacard-3.3.5/enkacard/src/modal/__pycache__/enkacardCread.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/modal/__pycache__/enkaToolsModel.cpython-311.pyc` & `enkacard-3.3.5/enkacard/src/modal/__pycache__/enkaToolsModel.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/modal/__pycache__/enkaToolsModel.cpython-312.pyc` & `enkacard-3.3.5/enkacard/src/modal/__pycache__/enkaToolsModel.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/modal/enkacardCread.py` & `enkacard-3.3.5/enkacard/src/modal/enkacardCread.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/modal/enkaToolsModel.py` & `enkacard-3.3.5/enkacard/src/modal/enkaToolsModel.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/pickle_cashe/data_characters.pkz` & `enkacard-3.3.5/enkacard/src/pickle_cashe/data_characters.pkz`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/utils/__pycache__/affixes.cpython-311.pyc` & `enkacard-3.3.5/enkacard/src/utils/__pycache__/affixes.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/utils/__pycache__/affixes.cpython-312.pyc` & `enkacard-3.3.5/enkacard/src/utils/__pycache__/affixes.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/utils/__pycache__/diagram.cpython-311.pyc` & `enkacard-3.3.5/enkacard/src/utils/__pycache__/diagram.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/utils/__pycache__/diagram.cpython-312.pyc` & `enkacard-3.3.5/enkacard/src/utils/__pycache__/diagram.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/utils/__pycache__/git.cpython-311.pyc` & `enkacard-3.3.5/enkacard/src/utils/__pycache__/git.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/utils/__pycache__/git.cpython-312.pyc` & `enkacard-3.3.5/enkacard/src/utils/__pycache__/git.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/utils/__pycache__/options.cpython-311.pyc` & `enkacard-3.3.5/enkacard/src/utils/__pycache__/options.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/utils/__pycache__/options.cpython-312.pyc` & `enkacard-3.3.5/enkacard/src/utils/__pycache__/options.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/utils/__pycache__/pickle_cashe.cpython-311.pyc` & `enkacard-3.3.5/enkacard/src/utils/__pycache__/pickle_cashe.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/utils/__pycache__/pickle_cashe.cpython-312.pyc` & `enkacard-3.3.5/enkacard/src/utils/__pycache__/pickle_cashe.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/utils/__pycache__/pill.cpython-311.pyc` & `enkacard-3.3.5/enkacard/src/utils/__pycache__/pill.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/utils/__pycache__/pill.cpython-312.pyc` & `enkacard-3.3.5/enkacard/src/utils/__pycache__/pill.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/utils/__pycache__/translation.cpython-311.pyc` & `enkacard-3.3.5/enkacard/src/utils/__pycache__/translation.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/utils/__pycache__/translation.cpython-312.pyc` & `enkacard-3.3.5/enkacard/src/utils/__pycache__/translation.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/utils/affixes.py` & `enkacard-3.3.5/enkacard/src/utils/affixes.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/utils/diagram.py` & `enkacard-3.3.5/enkacard/src/utils/diagram.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/utils/enkanetwork_update/__pycache__/config.cpython-311.pyc` & `enkacard-3.3.5/enkacard/src/utils/enkanetwork_update/__pycache__/config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/utils/enkanetwork_update/__pycache__/config.cpython-312.pyc` & `enkacard-3.3.5/enkacard/src/utils/enkanetwork_update/__pycache__/config.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/utils/enkanetwork_update/__pycache__/enka_update.cpython-311.pyc` & `enkacard-3.3.5/enkacard/src/utils/enkanetwork_update/__pycache__/enka_update.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/utils/enkanetwork_update/__pycache__/enka_update.cpython-312.pyc` & `enkacard-3.3.5/enkacard/src/utils/enkanetwork_update/__pycache__/enka_update.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/utils/enkanetwork_update/__pycache__/pathfinding.cpython-311.pyc` & `enkacard-3.3.5/enkacard/src/utils/enkanetwork_update/__pycache__/pathfinding.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/utils/enkanetwork_update/__pycache__/pathfinding.cpython-312.pyc` & `enkacard-3.3.5/enkacard/src/utils/enkanetwork_update/__pycache__/pathfinding.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/utils/enkanetwork_update/config.py` & `enkacard-3.3.5/enkacard/src/utils/enkanetwork_update/config.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/utils/enkanetwork_update/enka_update.py` & `enkacard-3.3.5/enkacard/src/utils/enkanetwork_update/enka_update.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/utils/enkanetwork_update/pathfinding.py` & `enkacard-3.3.5/enkacard/src/utils/enkanetwork_update/pathfinding.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/utils/git.py` & `enkacard-3.3.5/enkacard/src/utils/git.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/utils/options.py` & `enkacard-3.3.5/enkacard/src/utils/options.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/utils/pickle_cashe.py` & `enkacard-3.3.5/enkacard/src/utils/pickle_cashe.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/utils/pill.py` & `enkacard-3.3.5/enkacard/src/utils/pill.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/enkacard/src/utils/translation.py` & `enkacard-3.3.5/enkacard/src/utils/translation.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/pyproject.toml` & `enkacard-3.3.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "enkacard"
-version = "3.3.4"
+version = "3.3.5"
 description = "An asynchronous module and API that allows you to connect to your bot the generation of Genshin character cards from the Enka.Network website."
 authors = ["None"]
 
 readme = 'README.md'  # Поддерживаются файлы в формате Markdown
 
 repository = "https://github.com/DEViantUA/EnkaCard"
 homepage = "https://github.com/DEViantUA/EnkaCard"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 Pillow = "*"
-"enkanetworkv2.py" = "^2.0.0"
+"enkanetworkv2.py" = "*"
 cachetools = "*"
 asyncache  = "*"
 numpy = "*"
 more-itertools = "*"
 pydantic = "*"
 aiofiles = "*"
 matplotlib = "*"
```

### Comparing `enkacard-3.3.4/README.md` & `enkacard-3.3.5/README.md`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.4/PKG-INFO` & `enkacard-3.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: enkacard
-Version: 3.3.4
+Version: 3.3.5
 Summary: An asynchronous module and API that allows you to connect to your bot the generation of Genshin character cards from the Enka.Network website.
 Home-page: https://github.com/DEViantUA/EnkaCard
 Author: None
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Pillow
 Requires-Dist: aiofiles
 Requires-Dist: asyncache
 Requires-Dist: cachetools
-Requires-Dist: enkanetworkv2.py (>=2.0.0,<3.0.0)
+Requires-Dist: enkanetworkv2.py
 Requires-Dist: matplotlib
 Requires-Dist: more-itertools
 Requires-Dist: numpy
 Requires-Dist: pydantic
 Requires-Dist: python-magic (>=0.4.27,<0.5.0) ; sys_platform == "windows"
 Requires-Dist: python-magic-bin (>=0.4.14,<0.5.0) ; sys_platform == "windows"
 Project-URL: Repository, https://github.com/DEViantUA/EnkaCard
```

