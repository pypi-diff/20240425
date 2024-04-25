# Comparing `tmp/python-ndev-blizzardapi-0.1.2.tar.gz` & `tmp/python_ndev_blizzardapi-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-ndev-blizzardapi-0.1.2.tar", last modified: Fri Oct 20 15:21:56 2023, max compression
+gzip compressed data, was "python_ndev_blizzardapi-0.2.0.tar", last modified: Thu Apr 25 15:48:11 2024, max compression
```

## Comparing `python-ndev-blizzardapi-0.1.2.tar` & `python_ndev_blizzardapi-0.2.0.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxrwxrwx   0        0        0        0 2023-10-20 15:21:56.352808 python-ndev-blizzardapi-0.1.2/
--rw-rw-rw-   0        0        0      134 2023-07-14 20:43:22.000000 python-ndev-blizzardapi-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3319 2023-10-20 15:21:56.351808 python-ndev-blizzardapi-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2522 2023-07-23 03:28:03.000000 python-ndev-blizzardapi-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-10-20 15:21:56.249419 python-ndev-blizzardapi-0.1.2/blizzardAPI/
--rw-rw-rw-   0        0        0      161 2023-03-11 02:36:09.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/__init__.py
--rw-rw-rw-   0        0        0     4981 2023-06-24 20:44:02.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/api.py
-drwxrwxrwx   0        0        0        0 2023-10-20 15:21:56.252920 python-ndev-blizzardapi-0.1.2/blizzardAPI/battlenet/
--rw-rw-rw-   0        0        0       25 2023-03-10 03:36:02.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/battlenet/__init__.py
--rw-rw-rw-   0        0        0      458 2023-07-30 21:32:26.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/battlenet/battlenet_api.py
--rw-rw-rw-   0        0        0     1539 2023-07-30 21:32:29.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/battlenet/battlenet_oauth.py
--rw-rw-rw-   0        0        0     1475 2023-07-30 21:32:30.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/blizzard_api.py
-drwxrwxrwx   0        0        0        0 2023-10-20 15:21:56.255420 python-ndev-blizzardapi-0.1.2/blizzardAPI/tests/
--rw-rw-rw-   0        0        0        0 2023-06-21 22:10:25.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/tests/__init__.py
--rw-rw-rw-   0        0        0     3330 2023-07-23 02:33:06.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2023-10-20 15:21:56.257933 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/
--rw-rw-rw-   0        0        0       25 2023-03-10 03:36:02.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-20 15:21:56.312623 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/
--rw-rw-rw-   0        0        0     5007 2023-07-07 03:47:18.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/__init__.py
--rw-rw-rw-   0        0        0     3970 2023-07-06 00:16:58.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/achievement.py
--rw-rw-rw-   0        0        0     1598 2023-06-24 14:53:05.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/auction_house.py
--rw-rw-rw-   0        0        0     3244 2023-06-24 15:40:05.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/azerite_essence.py
--rw-rw-rw-   0        0        0     2189 2023-07-06 00:26:16.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/connected_realm.py
--rw-rw-rw-   0        0        0     4911 2023-06-24 20:41:51.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/covenant.py
--rw-rw-rw-   0        0        0     6408 2023-06-28 23:16:44.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/creature.py
--rw-rw-rw-   0        0        0     2462 2023-06-25 21:15:45.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/guild_crest.py
--rw-rw-rw-   0        0        0     1556 2023-06-25 21:25:28.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/heirloom.py
--rw-rw-rw-   0        0        0     6104 2023-07-06 00:19:27.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/item.py
--rw-rw-rw-   0        0        0     6076 2023-07-06 00:28:07.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/journal.py
--rw-rw-rw-   0        0        0      698 2023-06-29 12:06:44.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/media.py
--rw-rw-rw-   0        0        0     4331 2023-06-29 17:55:54.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/modified_crafting.py
--rw-rw-rw-   0        0        0     1796 2023-06-29 18:10:53.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/mount.py
--rw-rw-rw-   0        0        0     2312 2023-06-30 11:44:37.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/mythic_keystone_affix.py
--rw-rw-rw-   0        0        0     4838 2023-06-30 15:19:13.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/mythic_keystone_dungeon.py
--rw-rw-rw-   0        0        0     2210 2023-06-30 15:24:41.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/mythic_keystone_leaderboard.py
--rw-rw-rw-   0        0        0     1278 2023-06-30 15:35:33.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/mythic_raid_leaderboard.py
--rw-rw-rw-   0        0        0     3893 2023-06-30 15:46:57.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/pet.py
--rw-rw-rw-   0        0        0     2943 2023-06-30 16:07:58.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/playable_class.py
--rw-rw-rw-   0        0        0     1471 2023-06-30 16:17:21.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/playable_race.py
--rw-rw-rw-   0        0        0     2307 2023-06-30 16:44:46.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/playable_specialization.py
--rw-rw-rw-   0        0        0     1541 2023-06-30 16:54:12.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/power_type.py
--rw-rw-rw-   0        0        0     5454 2023-07-06 00:28:33.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/profession.py
--rw-rw-rw-   0        0        0     4076 2023-07-06 00:03:47.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/pvp_season.py
--rw-rw-rw-   0        0        0     2368 2023-07-06 00:29:20.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/pvp_tier.py
--rw-rw-rw-   0        0        0     5685 2023-07-06 00:33:30.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/quest.py
--rw-rw-rw-   0        0        0     2261 2023-07-06 03:02:36.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/realm.py
--rw-rw-rw-   0        0        0     1641 2023-07-07 02:36:20.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/region.py
--rw-rw-rw-   0        0        0     3193 2023-07-07 03:49:33.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/reputation.py
--rw-rw-rw-   0        0        0     2319 2023-07-07 03:41:57.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/spell.py
--rw-rw-rw-   0        0        0     5356 2023-07-07 03:06:25.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/talent.py
--rw-rw-rw-   0        0        0     3943 2023-07-06 03:10:04.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/tech_talent.py
--rw-rw-rw-   0        0        0     1477 2023-06-29 23:35:12.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/title.py
--rw-rw-rw-   0        0        0      974 2023-06-24 00:46:18.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/token.py
--rw-rw-rw-   0        0        0     1602 2023-06-22 04:12:53.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/toy.py
-drwxrwxrwx   0        0        0        0 2023-10-20 15:21:56.343292 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/profile_data/
--rw-rw-rw-   0        0        0     3200 2023-07-17 17:14:22.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/profile_data/__init__.py
--rw-rw-rw-   0        0        0     7961 2023-07-17 03:32:41.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/profile_data/account_profile.py
--rw-rw-rw-   0        0        0     2276 2023-07-17 16:20:59.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/profile_data/character_achievements.py
--rw-rw-rw-   0        0        0     1657 2023-07-17 16:22:25.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/profile_data/character_appearance.py
--rw-rw-rw-   0        0        0     4945 2023-07-18 00:30:42.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/profile_data/character_collections.py
--rw-rw-rw-   0        0        0     3525 2023-07-18 01:14:59.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/profile_data/character_encounters.py
--rw-rw-rw-   0        0        0     1386 2023-07-18 01:57:55.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/profile_data/character_equipment.py
--rw-rw-rw-   0        0        0     1399 2023-07-18 11:48:06.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/profile_data/character_hunter_pets.py
--rw-rw-rw-   0        0        0     1287 2023-07-19 03:15:49.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/profile_data/character_media.py
--rw-rw-rw-   0        0        0     2888 2023-07-21 00:06:36.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/profile_data/character_mythic_keystone_profile.py
--rw-rw-rw-   0        0        0     1319 2023-07-22 13:00:46.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/profile_data/character_professions.py
--rw-rw-rw-   0        0        0     2537 2023-07-22 13:51:31.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/profile_data/character_profile.py
--rw-rw-rw-   0        0        0     2806 2023-07-22 14:20:08.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/profile_data/character_pvp.py
--rw-rw-rw-   0        0        0     2518 2023-07-22 14:58:23.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/profile_data/character_quests.py
--rw-rw-rw-   0        0        0     1400 2023-07-22 15:29:49.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/profile_data/character_reputations.py
--rw-rw-rw-   0        0        0     1265 2023-07-22 15:32:24.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/profile_data/character_soulbinds.py
--rw-rw-rw-   0        0        0     1428 2023-07-22 15:56:06.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/profile_data/character_specializations.py
--rw-rw-rw-   0        0        0     1394 2023-07-22 18:15:13.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/profile_data/character_statistics.py
--rw-rw-rw-   0        0        0     1286 2023-07-23 02:16:19.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/profile_data/character_titles.py
--rw-rw-rw-   0        0        0     4160 2023-07-23 02:27:49.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/profile_data/guild.py
--rw-rw-rw-   0        0        0      533 2023-07-17 03:21:56.000000 python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/wow_api.py
-drwxrwxrwx   0        0        0        0 2023-10-20 15:21:56.349812 python-ndev-blizzardapi-0.1.2/python_ndev_blizzardapi.egg-info/
--rw-rw-rw-   0        0        0     3319 2023-10-20 15:21:56.000000 python-ndev-blizzardapi-0.1.2/python_ndev_blizzardapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3864 2023-10-20 15:21:56.000000 python-ndev-blizzardapi-0.1.2/python_ndev_blizzardapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-20 15:21:56.000000 python-ndev-blizzardapi-0.1.2/python_ndev_blizzardapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-10-20 15:21:56.000000 python-ndev-blizzardapi-0.1.2/python_ndev_blizzardapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-10-20 15:21:56.000000 python-ndev-blizzardapi-0.1.2/python_ndev_blizzardapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-10-20 15:21:56.352808 python-ndev-blizzardapi-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1033 2023-10-20 15:14:43.000000 python-ndev-blizzardapi-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 15:48:11.533158 python_ndev_blizzardapi-0.2.0/
+-rw-rw-rw-   0        0        0      134 2023-07-14 20:43:22.000000 python_ndev_blizzardapi-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3319 2024-04-25 15:48:11.530162 python_ndev_blizzardapi-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2522 2023-07-23 03:28:03.000000 python_ndev_blizzardapi-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 15:48:11.318582 python_ndev_blizzardapi-0.2.0/blizzardAPI/
+-rw-rw-rw-   0        0        0      161 2023-03-11 02:36:09.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/__init__.py
+-rw-rw-rw-   0        0        0     4981 2023-06-24 20:44:02.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/api.py
+drwxrwxrwx   0        0        0        0 2024-04-25 15:48:11.327098 python_ndev_blizzardapi-0.2.0/blizzardAPI/battlenet/
+-rw-rw-rw-   0        0        0       25 2023-03-10 03:36:02.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/battlenet/__init__.py
+-rw-rw-rw-   0        0        0      458 2023-07-30 21:32:26.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/battlenet/battlenet_api.py
+-rw-rw-rw-   0        0        0     1539 2023-07-30 21:32:29.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/battlenet/battlenet_oauth.py
+-rw-rw-rw-   0        0        0     1475 2023-07-30 21:32:30.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/blizzard_api.py
+drwxrwxrwx   0        0        0        0 2024-04-25 15:48:11.331101 python_ndev_blizzardapi-0.2.0/blizzardAPI/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-21 22:10:25.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/tests/__init__.py
+-rw-rw-rw-   0        0        0     3330 2023-07-23 02:33:06.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2024-04-25 15:48:11.337099 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/
+-rw-rw-rw-   0        0        0       25 2023-03-10 03:36:02.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 15:48:11.442625 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/
+-rw-rw-rw-   0        0        0     5007 2023-07-07 03:47:18.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/__init__.py
+-rw-rw-rw-   0        0        0     3905 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/achievement.py
+-rw-rw-rw-   0        0        0     1580 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/auction_house.py
+-rw-rw-rw-   0        0        0     3224 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/azerite_essence.py
+-rw-rw-rw-   0        0        0     2166 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/connected_realm.py
+-rw-rw-rw-   0        0        0     4876 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/covenant.py
+-rw-rw-rw-   0        0        0     6308 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/creature.py
+-rw-rw-rw-   0        0        0     2447 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/guild_crest.py
+-rw-rw-rw-   0        0        0     1546 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/heirloom.py
+-rw-rw-rw-   0        0        0     6064 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/item.py
+-rw-rw-rw-   0        0        0     6036 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/journal.py
+-rw-rw-rw-   0        0        0      693 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/media.py
+-rw-rw-rw-   0        0        0     4290 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/modified_crafting.py
+-rw-rw-rw-   0        0        0     1781 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/mount.py
+-rw-rw-rw-   0        0        0     2293 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/mythic_keystone_affix.py
+-rw-rw-rw-   0        0        0     4799 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/mythic_keystone_dungeon.py
+-rw-rw-rw-   0        0        0     2196 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/mythic_keystone_leaderboard.py
+-rw-rw-rw-   0        0        0     1261 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/mythic_raid_leaderboard.py
+-rw-rw-rw-   0        0        0     3863 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/pet.py
+-rw-rw-rw-   0        0        0     2919 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/playable_class.py
+-rw-rw-rw-   0        0        0     1461 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/playable_race.py
+-rw-rw-rw-   0        0        0     2292 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/playable_specialization.py
+-rw-rw-rw-   0        0        0     1523 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/power_type.py
+-rw-rw-rw-   0        0        0     5416 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/profession.py
+-rw-rw-rw-   0        0        0     4051 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/pvp_season.py
+-rw-rw-rw-   0        0        0     2353 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/pvp_tier.py
+-rw-rw-rw-   0        0        0     5645 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/quest.py
+-rw-rw-rw-   0        0        0     2246 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/realm.py
+-rw-rw-rw-   0        0        0     1631 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/region.py
+-rw-rw-rw-   0        0        0     3173 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/reputation.py
+-rw-rw-rw-   0        0        0     2304 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/spell.py
+-rw-rw-rw-   0        0        0     5321 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/talent.py
+-rw-rw-rw-   0        0        0     3918 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/tech_talent.py
+-rw-rw-rw-   0        0        0     1467 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/title.py
+-rw-rw-rw-   0        0        0      969 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/token.py
+-rw-rw-rw-   0        0        0     1602 2023-06-22 04:12:53.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/toy.py
+drwxrwxrwx   0        0        0        0 2024-04-25 15:48:11.506156 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/profile_data/
+-rw-rw-rw-   0        0        0     3200 2023-07-17 17:14:22.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/profile_data/__init__.py
+-rw-rw-rw-   0        0        0     7875 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/profile_data/account_profile.py
+-rw-rw-rw-   0        0        0     2230 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/profile_data/character_achievements.py
+-rw-rw-rw-   0        0        0     1644 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/profile_data/character_appearance.py
+-rw-rw-rw-   0        0        0     4904 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/profile_data/character_collections.py
+-rw-rw-rw-   0        0        0     3478 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/profile_data/character_encounters.py
+-rw-rw-rw-   0        0        0     1373 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/profile_data/character_equipment.py
+-rw-rw-rw-   0        0        0     1386 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/profile_data/character_hunter_pets.py
+-rw-rw-rw-   0        0        0     1274 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/profile_data/character_media.py
+-rw-rw-rw-   0        0        0     2842 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/profile_data/character_mythic_keystone_profile.py
+-rw-rw-rw-   0        0        0     1306 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/profile_data/character_professions.py
+-rw-rw-rw-   0        0        0     2507 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/profile_data/character_profile.py
+-rw-rw-rw-   0        0        0     2776 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/profile_data/character_pvp.py
+-rw-rw-rw-   0        0        0     2488 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/profile_data/character_quests.py
+-rw-rw-rw-   0        0        0     1387 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/profile_data/character_reputations.py
+-rw-rw-rw-   0        0        0     1252 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/profile_data/character_soulbinds.py
+-rw-rw-rw-   0        0        0     1415 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/profile_data/character_specializations.py
+-rw-rw-rw-   0        0        0     1381 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/profile_data/character_statistics.py
+-rw-rw-rw-   0        0        0     1273 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/profile_data/character_titles.py
+-rw-rw-rw-   0        0        0     4096 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/profile_data/guild.py
+-rw-rw-rw-   0        0        0      533 2023-07-17 03:21:56.000000 python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/wow_api.py
+drwxrwxrwx   0        0        0        0 2024-04-25 15:48:11.528155 python_ndev_blizzardapi-0.2.0/python_ndev_blizzardapi.egg-info/
+-rw-rw-rw-   0        0        0     3319 2024-04-25 15:48:11.000000 python_ndev_blizzardapi-0.2.0/python_ndev_blizzardapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3864 2024-04-25 15:48:11.000000 python_ndev_blizzardapi-0.2.0/python_ndev_blizzardapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 15:48:11.000000 python_ndev_blizzardapi-0.2.0/python_ndev_blizzardapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-04-25 15:48:11.000000 python_ndev_blizzardapi-0.2.0/python_ndev_blizzardapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-25 15:48:11.000000 python_ndev_blizzardapi-0.2.0/python_ndev_blizzardapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 15:48:11.533158 python_ndev_blizzardapi-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1033 2024-04-25 15:38:43.000000 python_ndev_blizzardapi-0.2.0/setup.py
```

### Comparing `python-ndev-blizzardapi-0.1.2/PKG-INFO` & `python_ndev_blizzardapi-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-ndev-blizzardapi
-Version: 0.1.2
+Version: 0.2.0
 Summary: Python module created to integrate your Python project with the Blizzard API
 Home-page: https://github.com/natanrmaia/python-ndev-blizzardapi
 Author: natanrmaia
 Author-email: contato@natanael.dev.br
 Project-URL: Documentation, https://python-ndev-blizzardapi.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/natanrmaia/python-ndev-blizzardapi
 Project-URL: Bug Reports, https://github.com/natanrmaia/python-ndev-blizzardapi/issues
```

### Comparing `python-ndev-blizzardapi-0.1.2/README.md` & `python_ndev_blizzardapi-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/api.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/api.py`

 * *Files identical despite different names*

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/battlenet/battlenet_oauth.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/battlenet/battlenet_oauth.py`

 * *Files identical despite different names*

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/blizzard_api.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/blizzard_api.py`

 * *Files identical despite different names*

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/tests/conftest.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/__init__.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/__init__.py`

 * *Files identical despite different names*

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/achievement.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/achievement.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,27 +22,27 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
-    
+        return super().get_api(api=api, query_params=query_params, **kwargs)
+
     def get_achievement_category(self, achievement_category_id: int, **kwargs: Any) -> Dict:
         """
         This function retrieves information about a specific achievement category in the World of Warcraft
         game.
-        
+
         Requested API:
             /data/wow/achievement-category/{achievement_category_id}
 
         Args:
             achievement_category_id: The ID of the achievement category.
-        
+
         Returns:
             A dictionary of the achievement category.
 
         Raises:
             ValueError: If achievement_category_id is not provided.
         """
 
@@ -53,35 +53,35 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
-    
+        return super().get_api(api=api, query_params=query_params, **kwargs)
+
     def get_achievement_index(self, **kwargs: Any) -> Dict:
         """
         This function will return the index of achievements from the API.
 
         Requested API:
             /data/wow/achievement/index
-        
+
         Returns:
             A dictionary of the achievement index.
         """
 
         api = '/data/wow/achievement/index'
 
         query_params = {
             'namespace': 'static',
         }
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
-    
+        return super().get_api(api=api, query_params=query_params, **kwargs)
+
     def get_achievement(self, achievement_id: int, **kwargs: Any) -> Dict:
         """
         This function retrieves information about a specific achievement in the World of Warcraft game.
 
         Requested API:
             /data/wow/achievement/{achievement_id}
 
@@ -100,16 +100,16 @@
 
         api = f'/data/wow/achievement/{achievement_id}'
 
         query_params = {
             'namespace': 'static',
         }
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
-    
+        return super().get_api(api=api, query_params=query_params, **kwargs)
+
     def get_achievement_media(self, achievement_id: int, **kwargs: Any) -> Dict:
         """
         This function retrieves the media for a specific achievement in the API.
 
         Requested API:
             /data/wow/media/achievement/{achievement_id}
 
@@ -128,8 +128,8 @@
 
         api = f'/data/wow/media/achievement/{achievement_id}'
 
         query_params = {
             'namespace': 'static',
         }
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/auction_house.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/auction_house.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,18 +27,18 @@
             raise ValueError('connected_realm_id is required')
 
         api = f'/data/wow/connected-realm/{connected_realm_id}/auctions'
 
         query_params = {
             'namespace': 'dynamic',
         }
-        
+
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_commodities(self, **kwargs: Any) -> Dict:
         """
         This function will return the commodities from the API.
 
         Requested API:
             /data/wow/auctions/commodities
@@ -51,8 +51,8 @@
 
         query_params = {
             'namespace': 'dynamic',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/azerite_essence.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/azerite_essence.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_azerite_essence(self, azerite_essence_id: int, **kwargs: Any) -> Dict:
         """
         This function will return the azerite essence from the API.
 
         Requested API:
             /data/wow/azerite-essence/{azerite_essence_id}
@@ -51,15 +51,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_azerite_essence_search(self, **kwargs: Any) -> Dict:
             """
             This function will return the azerite essence search from the API.
 
             Requested API:
                 /data/wow/search/azerite-essence
@@ -72,15 +72,15 @@
 
             query_params = {
                 'namespace': 'static',
             }
 
             query_params.update(kwargs)
 
-            return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+            return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_azerite_essence_media(self, azerite_essence_id: int, **kwargs: Any) -> Dict:
             """
             This function will return the azerite essence media from the API.
 
             Requested API:
                 /data/wow/media/azerite-essence/{azerite_essence_id}
@@ -103,8 +103,8 @@
 
             query_params = {
                 'namespace': 'static',
             }
 
             query_params.update(kwargs)
 
-            return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+            return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/connected_realm.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/connected_realm.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 
         api = '/data/wow/connected-realm/index'
 
         query_params = {
             'namespace': 'dynamic',
         }
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
-    
+        return super().get_api(api=api, query_params=query_params, **kwargs)
+
     def get_connected_realm(self, connected_realm_id: int, **kwargs: Any) -> Dict:
         """
         This function will return the connected realm from the API.
 
         Requested API:
             /data/wow/connected-realm/{connected_realm_id}
 
@@ -48,16 +48,16 @@
 
         api = f'/data/wow/connected-realm/{connected_realm_id}'
 
         query_params = {
             'namespace': 'dynamic',
         }
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
-    
+        return super().get_api(api=api, query_params=query_params, **kwargs)
+
     def get_connected_realm_search(self, **kwargs: Any) -> Dict:
         """
         This function will return the connected realm search from the API.
 
         Requested API:
             /data/wow/search/connected-realm
 
@@ -70,8 +70,8 @@
 
         api = '/data/wow/search/connected-realm'
 
         query_params = {
             'namespace': 'dynamic',
         }
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/covenant.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/covenant.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
         api = '/data/wow/covenant/index'
 
         query_params = {
             'namespace': 'static',
         }
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_covenant(self, covenant_id: int, **kwargs: Any) -> Dict:
         """
         tThis function retrieves information about a specific covenant in the World of Warcraft from the API.
 
         Requested API:
             /data/wow/covenant/{covenant_id}
@@ -47,15 +47,15 @@
 
         api = f'/data/wow/covenant/{covenant_id}'
 
         query_params = {
             'namespace': 'static',
         }
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_covenant_media(self, covenant_id: int, **kwargs: Any) -> Dict:
         """
         This function retrieves media for a specific covenant in the World of Warcraft from the API.
 
         Requested API:
             /data/wow/media/covenant/{covenant_id}
@@ -75,15 +75,15 @@
 
         api = f'/data/wow/media/covenant/{covenant_id}'
 
         query_params = {
             'namespace': 'static',
         }
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_soulbind_index(self, **kwargs: Any) -> Dict:
         """
         This function will return the index of soulbinds from the API.
 
         Requested API:
             /data/wow/covenant/soulbind/index
@@ -94,15 +94,15 @@
 
         api = '/data/wow/covenant/soulbind/index'
 
         query_params = {
             'namespace': 'static',
         }
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_soulbind(self, soulbind_id: int, **kwargs: Any) -> Dict:
         """
         This function retrieves information about a specific soulbind in the World of Warcraft from the API.
 
         Requested API:
             /data/wow/covenant/soulbind/{soulbind_id}
@@ -122,15 +122,15 @@
 
         api = f'/data/wow/covenant/soulbind/{soulbind_id}'
 
         query_params = {
             'namespace': 'static',
         }
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_conduit_index(self, **kwargs: Any) -> Dict:
         """
         This function will return the index of conduits from the API.
 
         Requested API:
             /data/wow/covenant/conduit/index
@@ -141,15 +141,15 @@
 
         api = '/data/wow/covenant/conduit/index'
 
         query_params = {
             'namespace': 'static',
         }
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_conduit(self, conduit_id: int, **kwargs: Any) -> Dict:
         """
         This function retrieves information about a specific conduit in the World of Warcraft from the API.
 
         Requested API:
             /data/wow/covenant/conduit/{conduit_id}
@@ -169,8 +169,8 @@
 
         api = f'/data/wow/covenant/conduit/{conduit_id}'
 
         query_params = {
             'namespace': 'static',
         }
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/creature.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/creature.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,27 +21,27 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
-    
+        return super().get_api(api=api, query_params=query_params, **kwargs)
+
     def get_creature_family(self, creature_family_id: int, **kwargs: Any) -> Dict:
         """
         This function retrieves information about a specific creature family in the World of Warcraft
         game.
-        
+
         Requested API:
             /data/wow/creature-family/{creature_family_id}
 
         Args:
             creature_family_id: The ID of the creature family.
-        
+
         Returns:
             A dictionary of the creature family.
 
         Raises:
             ValueError: If creature_family_id is not provided.
         """
 
@@ -52,16 +52,16 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
-    
+        return super().get_api(api=api, query_params=query_params, **kwargs)
+
     def get_creature_types_index(self, **kwargs: Any) -> Dict:
         """
         This function will return the index of creature types from the API.
 
         Requested API:
             /data/wow/creature-type/index
 
@@ -73,27 +73,27 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
-    
+        return super().get_api(api=api, query_params=query_params, **kwargs)
+
     def get_creature_type(self, creature_type_id: int, **kwargs: Any) -> Dict:
         """
         This function retrieves information about a specific creature type in the World of Warcraft
         game.
-        
+
         Requested API:
             /data/wow/creature-type/{creature_type_id}
 
         Args:
             creature_type_id: The ID of the creature type.
-        
+
         Returns:
             A dictionary of the creature type.
 
         Raises:
             ValueError: If creature_type_id is not provided.
         """
 
@@ -104,16 +104,16 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
-    
+        return super().get_api(api=api, query_params=query_params, **kwargs)
+
     def get_creature(self, creature_id: int, **kwargs: Any) -> Dict:
         """
         This function retrieves information about a specific creature in the World of Warcraft game.
 
         Requested API:
             /data/wow/creature/{creature_id}
 
@@ -134,16 +134,16 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
-    
+        return super().get_api(api=api, query_params=query_params, **kwargs)
+
     def get_creature_search(self, **kwargs: Any) -> Dict:
         """
         This function searches for creatures with the given search parameters.
 
         Requested API:
             /data/wow/search/creature
 
@@ -155,16 +155,16 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
-    
+        return super().get_api(api=api, query_params=query_params, **kwargs)
+
     def get_creature_display_media(self, creature_display_id: int, **kwargs: Any) -> Dict:
         """
         This function retrieves the media for a specific creature display.
 
         Requested API:
             /data/wow/media/creature-display/{creature_display_id}
 
@@ -185,16 +185,16 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
-    
+        return super().get_api(api=api, query_params=query_params, **kwargs)
+
     def get_creature_family_media(self, creature_family_id: int, **kwargs: Any) -> Dict:
         """
         This function retrieves the media for a specific creature family.
 
         Requested API:
             /data/wow/media/creature-family/{creature_family_id}
 
@@ -215,8 +215,8 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/guild_crest.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/guild_crest.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
         api = '/data/wow/guild-crest/index'
 
         query_params = {
             'namespace': 'static',
         }
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_guild_crest_border_media(self, border_id: int, **kwargs: Any) -> Dict:
         """
         This function retrieves information about a specific guild crest border from the API.
 
         Requested API:
            /data/wow/media/guild-crest/border/{border_id}
@@ -49,15 +49,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_guild_crest_emblem_media(self, emblem_id: int, **kwargs: Any) -> Dict:
         """
         This function retrieves information about a specific guild crest emblem from the API.
 
         Requested API:
             /data/wow/media/guild-crest/emblem/{emblem_id}
@@ -79,8 +79,8 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/heirloom.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/heirloom.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_heirloom(self, heirloom_id: int, **kwargs: Any) -> Dict:
         """
         This function retrieves information about a specific heirloom in the World of Warcraft
         game.
 
         Requested API:
@@ -52,8 +52,8 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/item.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/item.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_item_class(self, item_class_id: int, **kwargs: Any) -> Dict:
         """
         This function retrieves information about a specific item class in the World of Warcraft
         game.
 
         Requested API:
@@ -52,15 +52,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_item_sets_index(self, **kwargs: Any) -> Dict:
         """
         This function will return the index of item sets from the API.
 
         Requested API:
             /data/wow/item-set/index
@@ -73,15 +73,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_item_set(self, item_set_id: int, **kwargs: Any) -> Dict:
         """
         This function retrieves information about a specific item set from the API.
 
         Requested API:
             /data/wow/item-set/{item_set_id}
@@ -103,15 +103,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_item_subclass(self, item_class_id: int, item_subclass_id: int, **kwargs: Any) -> Dict:
         """
         This function retrieves information about a specific item subclass from the API.
 
         Requested API:
             /data/wow/item-class/{item_class_id}/item-subclass/{item_subclass_id}
@@ -136,15 +136,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_item(self, item_id: int, **kwargs: Any) -> Dict:
         """
         This function retrieves information about a specific item from the API.
 
         Requested API:
             /data/wow/item/{item_id}
@@ -166,15 +166,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
 
     def get_item_media(self, item_id: int, **kwargs: Any) -> Dict:
         """
         This function retrieves media information about a specific item from the API.
 
         Requested API:
@@ -197,15 +197,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_item_search(self, **kwargs: Any) -> Dict:
         """
         This function will perform a search of items from the API.
 
         Requested API:
             /data/wow/search/item
@@ -218,8 +218,8 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/journal.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/journal.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_journal_expansion(self, journal_expansion_id: int, **kwargs: Any) -> Dict:
         """
         This function retrieves information about a specific expansion in the World of Warcraft
         game.
 
         Requested API:
@@ -52,15 +52,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_journal_encounters_index(self, **kwargs: Any) -> Dict:
         """
         This function will return the index of encounters from the API.
 
         Requested API:
             /data/wow/journal-encounter/index
@@ -73,15 +73,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_journal_encounter(self, journal_encounter_id: int, **kwargs: Any) -> Dict:
         """
         This function retrieves information about a specific encounter in the World of Warcraft
         game.
 
         Requested API:
@@ -104,15 +104,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_journal_encounter_search(self, **kwargs: Any) -> Dict:
         """
         This function will perform a search of encounters from the API.
 
         Requested API:
             /data/wow/search/journal-encounter
@@ -125,15 +125,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_journal_instances_index(self, **kwargs: Any) -> Dict:
         """
         This function will return the index of instances from the API.
 
         Requested API:
             /data/wow/journal-instance/index
@@ -146,15 +146,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_journal_instance(self, journal_instance_id: int, **kwargs: Any) -> Dict:
         """
         This function retrieves information about a specific instance from the API.
 
         Requested API:
             /data/wow/journal-instance/{journal_instance_id}
@@ -176,15 +176,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_journal_instance_media(self, journal_instance_id: int, **kwargs: Any) -> Dict:
         """
         This function retrieves media for a specific instance from API.
 
         Requested API:
             /data/wow/media/journal-instance/{journal_instance_id}
@@ -206,8 +206,8 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/media.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/media.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,8 +21,8 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/modified_crafting.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/modified_crafting.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
-    
+        return super().get_api(api=api, query_params=query_params, **kwargs)
+
     def get_modified_crafting_category_index(self, **kwargs: Any) -> Dict:
         """
         This function will return the index of modified crafting category from the API.
 
         Requested API:
             /data/wow/modified-crafting/category/index
 
@@ -42,16 +42,16 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
-    
+        return super().get_api(api=api, query_params=query_params, **kwargs)
+
     def get_modified_crafting_category(self, modified_crafting_category_id: int, **kwargs: Any) -> Dict:
         """
         This function retrieves information about a specific modified crafting category in the World of Warcraft
         game.
 
         Requested API:
             /data/wow/modified-crafting/category/{modified_crafting_category_id}
@@ -73,16 +73,16 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
-    
+        return super().get_api(api=api, query_params=query_params, **kwargs)
+
     def get_modified_crafting_reagent_slot_type_index(self, **kwargs: Any) -> Dict:
         """
         This function will return the index of modified crafting reagent slot type from the API.
 
         Requested API:
             /data/wow/modified-crafting/reagent-slot-type/index
 
@@ -94,16 +94,16 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
-    
+        return super().get_api(api=api, query_params=query_params, **kwargs)
+
     def get_modified_crafting_reagent_slot_type(self, modified_crafting_reagent_slot_type_id: int, **kwargs: Any) -> Dict:
         """
         This function retrieves information about a specific modified crafting reagent slot type in the World of Warcraft
         game.
 
         Requested API:
             /data/wow/modified-crafting/reagent-slot-type/{modified_crafting_reagent_slot_type_id}
@@ -125,8 +125,8 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/mount.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/mount.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_mount(self, mount_id: int, **kwargs: Any) -> Dict:
         """
         This function will return the details of a specific mount from the API.
 
         Requested API:
             /data/wow/mount/{mountId}
@@ -45,15 +45,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_mount_search(self, **kwargs: Any) -> Dict:
         """
         This function will search for mounts that match the given search query.
 
         Requested API:
             /data/wow/search/mount
@@ -66,8 +66,8 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/mythic_keystone_affix.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/mythic_keystone_affix.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict, Optional, Any
 from ...api import API
 
 class MythicKeystoneAffix(API):
-    
+
     def __init__(self, client_id, client_secret):
         super().__init__(client_id, client_secret)
 
     def get_mythic_keystone_affixes_index(self, **kwargs: Any) -> Dict:
         """
         This function will return the index of mythic keystone affixes from the API.
 
@@ -21,15 +21,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_mythic_keystone_affix(self, keystone_affix_id: int, **kwargs: Any) -> Dict:
         """
         This function will return the details of a specific mythic keystone affix from the API.
 
         Requested API:
             /data/wow/keystone-affix/{keystoneAffixId}
@@ -45,15 +45,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_mythic_keystone_affix_media(self, keystone_affix_id: int, **kwargs: Any) -> Dict:
         """
         This function will return the media of a specific mythic keystone affix from the API.
 
         Requested API:
             /data/wow/media/keystone-affix/{keystoneAffixId}
@@ -69,8 +69,8 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/mythic_keystone_dungeon.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/mythic_keystone_dungeon.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict, Optional, Any
 from ...api import API
 
 class MythicKeystoneDungeon(API):
-    
+
     def __init__(self, client_id, client_secret):
         super().__init__(client_id, client_secret)
 
     def get_mythic_keystone_dungeons_index(self, **kwargs: Any) -> Dict:
         """
         This function will return the index of mythic keystone dungeons from the API.
 
@@ -21,15 +21,15 @@
 
         query_params = {
             'namespace': 'dynamic',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_mythic_keystone_dungeon(self, dungeon_id: int,  **kwargs: Any) -> Dict:
         """
         This function will return the details of a specific mythic keystone dungeon from the API.
 
         Requested API:
             /data/wow/mythic-keystone/dungeon/{dungeonId}
@@ -45,15 +45,15 @@
 
         query_params = {
             'namespace': 'dynamic',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_mythic_keystone_index(self, **kwargs: Any) -> Dict:
         """
         This function will return the index of mythic keystones from the API.
 
         Requested API:
             /data/wow/mythic-keystone/index
@@ -66,15 +66,15 @@
 
         query_params = {
             'namespace': 'dynamic',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_mythic_keystone_period_index(self, **kwargs: Any) -> Dict:
         """
         This function will return the index of mythic keystone periods from the API.
 
         Requested API:
             /data/wow/mythic-keystone/period/index
@@ -87,15 +87,15 @@
 
         query_params = {
             'namespace': 'dynamic',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_mythic_keystone_period(self, period_id: int, **kwargs: Any) -> Dict:
         """
         This function will return the details of a specific mythic keystone period from the API.
 
         Requested API:
             /data/wow/mythic-keystone/period/{periodId}
@@ -111,15 +111,15 @@
 
         query_params = {
             'namespace': 'dynamic',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_mythic_keystone_seasons_index(self, **kwargs: Any) -> Dict:
         """
         This function will return the index of mythic keystone seasons from the API.
 
         Requested API:
             /data/wow/mythic-keystone/season/index
@@ -132,15 +132,15 @@
 
         query_params = {
             'namespace': 'dynamic',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_mythic_keystone_season(self, season_id: int, **kwargs: Any) -> Dict:
         """
         This function will return the details of a specific mythic keystone season from the API.
 
         Requested API:
             /data/wow/mythic-keystone/season/{seasonId}
@@ -156,8 +156,8 @@
 
         query_params = {
             'namespace': 'dynamic',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/mythic_keystone_leaderboard.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/mythic_keystone_leaderboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict, Optional, Any
 from ...api import API
 
 class MythicKeystoneLeaderboard(API):
-    
+
     def __init__(self, client_id, client_secret):
         super().__init__(client_id, client_secret)
 
     def get_mythic_keystone_leaderboards_index(self, connected_realm_id: int,  **kwargs: Any) -> Dict:
         """
         This function will return the index of mythic keystone leaderboards from the API.
 
@@ -24,15 +24,15 @@
 
         query_params = {
             'namespace': 'dynamic',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_mythic_keystone_leaderboard(self, connected_realm_id: int, dungeon_id: int, period: int, **kwargs: Any) -> Dict:
         """
         This function will return the details of a specific mythic keystone leaderboard from the API.
 
         Requested API:
             /data/wow/connected-realm/{connectedRealmId}/mythic-leaderboard/{dungeonId}/period/{period}
@@ -50,8 +50,8 @@
 
         query_params = {
             'namespace': 'dynamic',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/mythic_raid_leaderboard.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/mythic_raid_leaderboard.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # BEGIN: abpxx6d04wxr
 from typing import Dict, Optional, Any
 from ...api import API
 
 class MythicRaidLeaderboard(API):
-    
+
     def __init__(self, client_id, client_secret):
         super().__init__(client_id, client_secret)
 
 
     def get_mythic_raid_leaderboard(self, raid: str, faction: str, **kwargs: Any) -> Dict:
         """
         This function will return the details of a specific mythic raid leaderboard from the API.
@@ -21,20 +21,20 @@
 
         Returns:
             A dictionary of the mythic raid leaderboard details.
         """
 
         if raid is None:
             raise ValueError('raid is required')
-        
+
         if faction is None:
             raise ValueError('faction is required')
 
         api = f'/data/wow/leaderboard/hall-of-fame/{raid}/{faction}'
 
         query_params = {
             'namespace': 'dynamic',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/pet.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/pet.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_pet(self, pet_id: int, **kwargs: Any) -> Dict:
         """
         This function will return the details of a specific pet from the API.
 
         Requested API:
             /data/wow/pet/{petId}
@@ -45,15 +45,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_pet_media(self, pet_id: int, **kwargs: Any) -> Dict:
         """
         This function will return the media of a specific pet from the API.
 
         Requested API:
             /data/wow/media/pet/{petId}
@@ -69,15 +69,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_pet_abilities_index(self, **kwargs: Any) -> Dict:
         """
         This function will return the index of pet abilities from the API.
 
         Requested API:
             /data/wow/pet-ability/index
@@ -90,15 +90,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_pet_ability(self, pet_ability_id: int, **kwargs: Any) -> Dict:
         """
         This function will return the details of a specific pet ability from the API.
 
         Requested API:
             /data/wow/pet-ability/{petAbilityId}
@@ -114,15 +114,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_pet_ability_media(self, pet_ability_id: int, **kwargs: Any) -> Dict:
         """
         This function will return the media of a specific pet ability from the API.
 
         Requested API:
             /data/wow/media/pet-ability/{petAbilityId}
@@ -138,8 +138,8 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/playable_class.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/playable_class.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_playable_class(self, class_id: int, **kwargs: Any) -> Dict:
         """
         This function will return the details of a specific playable class from the API.
 
         Requested API:
             /data/wow/playable-class/{classId}
@@ -45,15 +45,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_playable_class_media(self, playable_class_id: int, **kwargs: Any) -> Dict:
         """
         This function will return the media of a specific playable class from the API.
 
         Requested API:
             /data/wow/media/playable-class/{playableClassId}
@@ -69,16 +69,16 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
-    
+        return super().get_api(api=api, query_params=query_params, **kwargs)
+
     def get_pvp_talent_slots(self, class_id: int, **kwargs: Any) -> Dict:
         """
         This function will return the PvP talent slots of a specific playable class from the API.
 
         Requested API:
             /data/wow/playable-class/{classId}/pvp-talent-slots
 
@@ -93,8 +93,8 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/playable_race.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/playable_race.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_playable_race(self, playable_race_id: int, **kwargs: Any) -> Dict:
         """
         This function will return the details of a specific playable race from the API.
 
         Requested API:
             /data/wow/playable-race/{playableRaceId}
@@ -46,8 +46,8 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/playable_specialization.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/playable_specialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_playable_specialization(self, spec_id: int, **kwargs: Any) -> Dict:
         """
         This function will return the details of a specific playable specialization from the API.
 
         Requested API:
             /data/wow/playable-specialization/{specId}
@@ -45,15 +45,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_playable_specialization_media(self, spec_id: int,  **kwargs: Any) -> Dict:
         """
         This function will return the media of a specific playable specialization from the API.
 
         Requested API:
             /data/wow/media/playable-specialization/{specId}
@@ -69,8 +69,8 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/power_type.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/power_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,26 +21,26 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_power_type(self, power_type_id: int, **kwargs: Any) -> Dict:
         """
         This function will return the power type from the API.
 
         Requested API:
             /data/wow/power-type/{power_type_id}
 
         Args:
             power_type_id: The ID of the power type.
-        
+
         Returns:
             A dict of the requested power type.
 
         Raises:
             ValueError: If power_type_id is not provided.
         """
 
@@ -51,8 +51,8 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/profession.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/profession.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_profession(self, profession_id: int, **kwargs: Any) -> Dict:
         """
         This function will return the details of a specific profession from the API.
 
         Requested API:
             /data/wow/profession/{professionId}
@@ -51,15 +51,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_profession_media(self, profession_id: int, **kwargs: Any) -> Dict:
         """
         This function will return the media of a specific profession from the API.
 
         Requested API:
             /data/wow/media/profession/{professionId}
@@ -81,15 +81,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_profession_skill_tier(self, profession_id: int, skill_tier_id: int, **kwargs: Any) -> Dict:
         """
         This function will return the details of a specific profession skill tier from the API.
 
         Requested API:
             /data/wow/profession/{professionId}/skill-tier/{skillTierId}
@@ -104,28 +104,28 @@
         Raises:
             ValueError: If the profession ID is not valid.
             ValueError: If the skill tier ID is not valid.
         """
 
         if profession_id is None:
             raise ValueError('Profession ID cannot be None.')
-        
+
         if skill_tier_id is None:
             raise ValueError('Skill tier ID cannot be None.')
 
 
         api = f'/data/wow/profession/{profession_id}/skill-tier/{skill_tier_id}'
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_recipe(self, recipe_id: int, **kwargs: Any) -> Dict:
         """
         This function will return the details of a specific recipe from the API.
 
         Requested API:
             /data/wow/recipe/{recipeId}
@@ -149,15 +149,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_recipe_media(self, recipe_id: int, **kwargs: Any) -> Dict:
         """
         This function will return the media of a specific recipe from the API.
 
         Requested API:
             /data/wow/media/recipe/{recipeId}
@@ -179,8 +179,8 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/pvp_season.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/pvp_season.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
         query_params = {
             'namespace': 'dynamic',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_pvp_season(self, pvp_season_id: int, **kwargs: Any) -> Dict:
         """
         This function retrieves information about a specific PvP season from the API.
 
         Requested API:
             /data/wow/pvp-season/{pvp_season_id}
@@ -51,15 +51,15 @@
 
         query_params = {
             'namespace': 'dynamic',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_pvp_leaderboards_index(self, pvp_season_id: int, **kwargs: Any) -> Dict:
         """
         This function will return the index of PvP leaderboards from the API.
 
         Requested API:
             /data/wow/pvp-season/{pvp_season_id}/pvp-leaderboard/index
@@ -75,15 +75,15 @@
 
         query_params = {
             'namespace': 'dynamic',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_pvp_leaderboard(self, pvp_season_id: int, pvp_bracket: str, **kwargs: Any) -> Dict:
         """
         This function retrieves information about a specific PvP leaderboard from the API.
 
         Requested API:
             /data/wow/pvp-season/{pvp_season_id}/pvp-leaderboard/{pvp_bracket}
@@ -109,15 +109,15 @@
 
         query_params = {
             'namespace': 'dynamic',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_pvp_rewards_index(self, pvp_season_id: int, **kwargs: Any) -> Dict:
         """
         This function will return the index of PvP rewards from the API.
 
         Requested API:
             /data/wow/pvp-season/{pvp_season_id}/pvp-reward/index
@@ -133,8 +133,8 @@
 
         query_params = {
             'namespace': 'dynamic',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/pvp_tier.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/pvp_tier.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_pvp_tier(self, pvp_tier_id: int, **kwargs: Any) -> Dict:
         """
         This function retrieves information about a specific PvP tier from the API.
 
         Requested API:
             /data/wow/pvp-tier/{pvp_tier_id}
@@ -52,15 +52,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_pvp_tier_media(self, pvp_tier_id: int, **kwargs: Any) -> Dict:
         """
         This function retrieves media information about a specific PvP tier from the API.
 
         Requested API:
             /data/wow/media/pvp-tier/{pvp_tier_id}
@@ -82,8 +82,8 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/quest.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/quest.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_quest(self, quest_id: int, **kwargs: Any) -> Dict:
         """
         This function retrieves information about a specific quest from the API.
 
         Requested API:
             /data/wow/quest/{quest_id}
@@ -52,15 +52,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_quest_categories_index(self, **kwargs: Any) -> Dict:
         """
         This function will return the index of quest categories from the API.
 
         Requested API:
             /data/wow/quest/category/index
@@ -73,15 +73,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_quest_category(self, quest_category_id: int, **kwargs: Any) -> Dict:
         """
         This function retrieves information about a specific quest category from the API.
 
         Requested API:
             /data/wow/quest/category/{quest_category_id}
@@ -103,15 +103,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_quest_areas_index(self, **kwargs: Any) -> Dict:
         """
         This function will return the index of quest areas from the API.
 
         Requested API:
             /data/wow/quest/area/index
@@ -125,15 +125,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_quest_area(self, quest_area_id: int, **kwargs: Any) -> Dict:
         """
         This function retrieves information about a specific quest area from the API.
 
         Requested API:
             /data/wow/quest/area/{quest_area_id}
@@ -155,15 +155,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_quest_types_index(self, **kwargs: Any) -> Dict:
         """
         This function will return the index of quest types from the API.
 
         Requested API:
             /data/wow/quest/type/index
@@ -176,15 +176,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_quest_type(self, quest_type_id: int, **kwargs: Any) -> Dict:
         """
         This function retrieves information about a specific quest type from the API.
 
         Requested API:
             /data/wow/quest/type/{quest_type_id}
@@ -206,8 +206,8 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/realm.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/realm.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
         query_params = {
             'namespace': 'dynamic',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_realm(self, realm_slug: str, **kwargs: Any) -> Dict:
         """
         This function retrieves information about a specific realm from the API.
 
         Requested API:
             /data/wow/realm/{realmSlug}
@@ -52,15 +52,15 @@
 
         query_params = {
             'namespace': 'dynamic',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_realm_search(self, search: str, **kwargs: Any) -> Dict:
         """
         This function retrieves information about a specific realm from the API.
 
         Requested API:
             /data/wow/search/realm
@@ -82,8 +82,8 @@
 
         query_params = {
             'namespace': 'dynamic',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/region.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/region.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
         query_params = {
             'namespace': 'dynamic',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_region(self, region_id: int, **kwargs: Any) -> Dict:
         """
         This function retrieves information about a specific region from the API.
 
         Requested API:
             /data/wow/region/{region_id}
@@ -56,8 +56,8 @@
 
         query_params = {
             'namespace': 'dynamic',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/reputation.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/reputation.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_reputation_faction(self, reputation_faction_id: int, **kwargs: Any) -> Dict:
         """
         This function retrieves information about a specific reputation faction from the API.
 
         Requested API:
             /data/wow/reputation-faction/{reputation_faction_id}
@@ -51,15 +51,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_reputation_tiers_index(self, **kwargs: Any) -> Dict:
         """
         This function will return the index of reputation tiers from the API.
 
         Requested API:
             /data/wow/reputation-tiers/index
@@ -72,15 +72,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_reputation_tiers(self, reputation_tiers_id: int, **kwargs: Any) -> Dict:
         """
         This function retrieves information about a specific reputation tier from the API.
 
         Requested API:
             /data/wow/reputation-tiers/{reputation_tiers_id}
@@ -102,8 +102,8 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/spell.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/spell.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_spell_media(self, spell_id: int, **kwargs: Any) -> Dict:
         """
         This function retrieves media information about a specific spell from the API.
 
         Requested API:
             /data/wow/media/spell/{spellId}
@@ -61,15 +61,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_spell_search(self, **kwargs: Any) -> Dict:
         """
         This function searches for spells from the API.
 
         Requested API:
             /data/wow/search/spell
@@ -85,8 +85,8 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/talent.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/talent.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_talent_tree(self, talent_tree_id: int, spec_id: int, **kwargs: Any) -> Dict:
         """
         This function retrieves information about a specific talent tree from the API.
 
         Requested API:
             /data/wow/talent-tree/{talent_tree_id}/playable-specialization/{spec_id}
@@ -55,15 +55,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_talent_tree_nodes(self, talent_tree_id: int, **kwargs: Any) -> Dict:
         """
         This function retrieves information about a specific talent tree nodes from the API.
 
         Requested API:
             /data/wow/talent-tree/{talent_tree_id}
@@ -85,15 +85,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_talents_index(self, **kwargs: Any) -> Dict:
         """
         This function will return the index of talents from the API.
 
         Requested API:
             /data/wow/talent/index
@@ -106,15 +106,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_talent(self, talent_id: int, **kwargs: Any) -> Dict:
         """
         This function retrieves information about a specific talent from the API.
 
         Requested API:
             /data/wow/talent/{talent_id}
@@ -136,15 +136,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_pvp_talents_index(self, **kwargs: Any) -> Dict:
         """
         This function will return the index of PvP talents from the API.
 
         Requested API:
             /data/wow/pvp-talent/index
@@ -157,15 +157,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_pvp_talent(self, pvp_talent_id: int, **kwargs: Any) -> Dict:
         """
         This function retrieves information about a specific PvP talent from the API.
 
         Requested API:
             /data/wow/pvp-talent/{pvp_talent_id}
@@ -187,8 +187,8 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/tech_talent.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/tech_talent.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_tech_talent_tree(self, tech_talent_tree_id: int, **kwargs: Any) -> Dict:
         """
         This function retrieves information about a specific Tech Talent Tree from the API.
 
         Requested API:
             /data/wow/tech-talent-tree/{tech_talent_tree_id}
@@ -52,15 +52,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_tech_talent_index(self, **kwargs: Any) -> Dict:
         """
         This function will return the index of Tech Talent from the API.
 
         Requested API:
             /data/wow/tech-talent/index
@@ -73,15 +73,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_tech_talent(self, tech_talent_id: int, **kwargs: Any) -> Dict:
         """
         This function retrieves information about a specific Tech Talent from the API.
 
         Requested API:
             /data/wow/tech-talent/{tech_talent_id}
@@ -103,15 +103,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_tech_talent_media(self, tech_talent_id: int, **kwargs: Any) -> Dict:
         """
         This function retrieves media information about a specific Tech Talent from the API.
 
         Requested API:
             /data/wow/media/tech-talent/{tech_talent_id}
@@ -133,8 +133,8 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/title.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/title.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
     def get_title(self, title_id: int, **kwargs: Any) -> Dict:
         """
         This function retrieves information about a specific title from the API.
 
         Requested API:
             /data/wow/title/{title_id}
@@ -52,8 +52,8 @@
 
         query_params = {
             'namespace': 'static',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/token.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/token.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,8 +28,8 @@
 
         query_params = {
             'namespace': 'dynamic',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(region=region, api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(region=region, api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/game_data/toy.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/game_data/toy.py`

 * *Files identical despite different names*

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/profile_data/__init__.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/profile_data/__init__.py`

 * *Files identical despite different names*

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/profile_data/account_profile.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/profile_data/account_profile.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,18 +7,18 @@
         super().__init__(client_id, client_secret)
 
     def get_account_profile_summary(self, access_token: Any, **kwargs: Any) -> Dict:
         """
         Returns the account profile summary from the API.
         Because this endpoint provides data about the current logged-in user's World of Warcraft account, it requires an access token with the wow.profile scope acquired via the Authorization Code Flow.
 
-        Args: 
-            access_token: The access token of the API endpoint you want to use. 
-        
-        Return: 
+        Args:
+            access_token: The access token of the API endpoint you want to use.
+
+        Return:
             The account profile summary.
 
         Raises:
             ValueError: If access_token is not provided.
         """
 
         api = '/profile/user/wow'
@@ -29,16 +29,16 @@
         query_params = {
             'namespace': 'profile',
             'access_token': access_token,
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
-    
+        return super().get_api(api=api, query_params=query_params, **kwargs)
+
     def get_protected_account_profile_summary(self, access_token: Any, realm_id: int, character_id: int,**kwargs: Any) -> Dict:
         """
         Returns the protected account profile summary from the API.
         Because this endpoint provides data about the current logged-in user's World of Warcraft account, it requires an access token with the wow.profile scope acquired via the Authorization Code Flow.
 
         Args:
             access_token: The access token of the API endpoint you want to use.
@@ -54,30 +54,30 @@
             ValueError: If character_id is not provided.
         """
 
         api = f'/profile/user/wow/protected-character/{realm_id}-{character_id}'
 
         if access_token is None:
             raise ValueError('access_token is required')
-        
+
         if realm_id is None:
             raise ValueError('realm_id is required')
-        
+
         if character_id is None:
             raise ValueError('character_id is required')
 
         query_params = {
             'namespace': 'profile',
             'access_token': access_token,
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
-    
+        return super().get_api(api=api, query_params=query_params, **kwargs)
+
     def get_account_collections_index(self, access_token: Any, **kwargs: Any) -> Dict:
         """
         Returns the account collections index from the API.
         Because this endpoint provides data about the current logged-in user's World of Warcraft account, it requires an access token with the wow.profile scope acquired via the Authorization Code Flow.
 
         Args:
             access_token: The access token of the API endpoint you want to use.
@@ -97,16 +97,16 @@
         query_params = {
             'namespace': 'profile',
             'access_token': access_token,
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
-    
+        return super().get_api(api=api, query_params=query_params, **kwargs)
+
     def get_account_mounts_collection_summary(self, access_token: Any, **kwargs: Any) -> Dict:
         """
         Returns the account mounts collection summary from the API.
         Because this endpoint provides data about the current logged-in user's World of Warcraft account, it requires an access token with the wow.profile scope acquired via the Authorization Code Flow.
 
         Args:
             access_token: The access token of the API endpoint you want to use.
@@ -126,16 +126,16 @@
         query_params = {
             'namespace': 'profile',
             'access_token': access_token,
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
-    
+        return super().get_api(api=api, query_params=query_params, **kwargs)
+
     def get_account_pets_collection_summary(self, access_token: Any, **kwargs: Any) -> Dict:
         """
         Returns the account pets collection summary from the API.
         Because this endpoint provides data about the current logged-in user's World of Warcraft account, it requires an access token with the wow.profile scope acquired via the Authorization Code Flow.
 
         Args:
             access_token: The access token of the API endpoint you want to use.
@@ -155,16 +155,16 @@
         query_params = {
             'namespace': 'profile',
             'access_token': access_token,
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
-    
+        return super().get_api(api=api, query_params=query_params, **kwargs)
+
     def get_account_toys_collection_summary(self, access_token: Any, **kwargs: Any) -> Dict:
         """
         Returns the account toys collection index from the API.
         Because this endpoint provides data about the current logged-in user's World of Warcraft account, it requires an access token with the wow.profile scope acquired via the Authorization Code Flow.
 
         Args:
             access_token: The access token of the API endpoint you want to use.
@@ -184,16 +184,16 @@
         query_params = {
             'namespace': 'profile',
             'access_token': access_token,
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
-    
+        return super().get_api(api=api, query_params=query_params, **kwargs)
+
     def get_account_heirlooms_collection_summary(self, access_token: Any, **kwargs: Any) -> Dict:
         """
         Returns the account heirlooms collection index from the API.
         Because this endpoint provides data about the current logged-in user's World of Warcraft account, it requires an access token with the wow.profile scope acquired via the Authorization Code Flow.
 
         Args:
             access_token: The access token of the API endpoint you want to use.
@@ -213,8 +213,8 @@
         query_params = {
             'namespace': 'profile',
             'access_token': access_token,
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/profile_data/character_achievements.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/profile_data/character_achievements.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,39 +22,39 @@
         Raises:
             ValueError: If access_token is not provided.
             ValueError: If realm_slug is not provided.
             ValueError: If character_name is not provided.
         """
 
         api = f'/profile/wow/character/{realm_slug}/{character_name}/achievements'
-        
+
         if realm_slug is None:
             raise ValueError('realm_slug is required')
-        
+
         if character_name is None:
             raise ValueError('character_name is required')
 
         query_params = {
             'namespace': 'profile',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
-    
+        return super().get_api(api=api, query_params=query_params, **kwargs)
+
     def get_character_achievements_statistics(self, realm_slug: str, character_name: str, **kwargs: Any) -> Dict:
 
         api = f'/profile/wow/character/{realm_slug}/{character_name}/achievements/statistics'
-        
+
         if realm_slug is None:
             raise ValueError('realm_slug is required')
-        
+
         if character_name is None:
             raise ValueError('character_name is required')
 
         query_params = {
             'namespace': 'profile',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/profile_data/character_appearance.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/profile_data/character_appearance.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,20 +23,20 @@
             ValueError: If access_token is not provided.
             ValueError: If realm_slug is not provided.
             ValueError: If character_name is not provided.
         """
 
         if realm_slug is None:
             raise ValueError('realm_slug is required')
-        
+
         if character_name is None:
             raise ValueError('character_name is required')
 
         api = f'/profile/wow/character/{realm_slug}/{character_name}/appearance'
 
         query_params = {
             'namespace': 'profile',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/profile_data/character_collections.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/profile_data/character_collections.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 
         query_params = {
             'namespace': 'profile',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
-    
+        return super().get_api(api=api, query_params=query_params, **kwargs)
+
     def get_character_mounts_collection_summary(self, realm_slug: str, character_name: str, **kwargs: Any) -> Dict:
         """
         Returns a summary of the mounts a character has obtained.
 
         Args:
             realm_slug: The realm slug of the character you want to get the mounts collection summary from.
             character_name: The character name of the character you want to get the mounts collection summary from.
@@ -51,16 +51,16 @@
 
         query_params = {
             'namespace': 'profile',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
-    
+        return super().get_api(api=api, query_params=query_params, **kwargs)
+
     def get_character_pets_collection_summary(self, realm_slug: str, character_name: str, **kwargs: Any) -> Dict:
         """
         Returns a summary of the pets a character has obtained.
 
         Args:
             realm_slug: The realm slug of the character you want to get the pets collection summary from.
             character_name: The character name of the character you want to get the pets collection summary from.
@@ -77,16 +77,16 @@
 
         query_params = {
             'namespace': 'profile',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
-    
+        return super().get_api(api=api, query_params=query_params, **kwargs)
+
     def get_character_toys_collection_summary(self, realm_slug: str, character_name: str, **kwargs: Any) -> Dict:
         """
         Returns a summary of the toys a character has obtained.
 
         Args:
             realm_slug: The realm slug of the character you want to get the toys collection summary from.
             character_name: The character name of the character you want to get the toys collection summary from.
@@ -103,16 +103,16 @@
 
         query_params = {
             'namespace': 'profile',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
-    
+        return super().get_api(api=api, query_params=query_params, **kwargs)
+
     def get_character_heirlooms_collection_summary(self, realm_slug: str, character_name: str, **kwargs: Any) -> Dict:
         """
         Returns a summary of the heirlooms a character has obtained.
 
         Args:
             realm_slug: The realm slug of the character you want to get the heirlooms collection summary from.
             character_name: The character name of the character you want to get the heirlooms collection summary from.
@@ -129,8 +129,8 @@
 
         query_params = {
             'namespace': 'profile',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/profile_data/character_encounters.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/profile_data/character_encounters.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,28 +20,28 @@
         Raises:
             ValueError: If realm_slug is not provided.
             ValueError: If character_name is not provided.
         """
 
         if realm_slug is None:
             raise ValueError('realm_slug is required')
-        
+
         if character_name is None:
             raise ValueError('character_name is required')
 
         api = f'/profile/wow/character/{realm_slug}/{character_name}/encounters'
 
         query_params = {
             'namespace': 'profile',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
-    
+        return super().get_api(api=api, query_params=query_params, **kwargs)
+
     def get_character_dungeons(self, realm_slug: str, character_name: str, **kwargs: Any) -> Dict:
         """
         Returns the character dungeons from the API.
 
         Args:
             realm_slug: The realm slug of the character you want to get the dungeons from.
             character_name: The character name of the character you want to get the dungeons from.
@@ -52,28 +52,28 @@
         Raises:
             ValueError: If realm_slug is not provided.
             ValueError: If character_name is not provided.
         """
 
         if realm_slug is None:
             raise ValueError('realm_slug is required')
-        
+
         if character_name is None:
             raise ValueError('character_name is required')
 
         api = f'/profile/wow/character/{realm_slug}/{character_name}/encounters/dungeons'
 
         query_params = {
             'namespace': 'profile',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
-    
+        return super().get_api(api=api, query_params=query_params, **kwargs)
+
     def get_character_raids(self, realm_slug: str, character_name: str, **kwargs: Any) -> Dict:
         """
         Returns the character raids from the API.
 
         Args:
             realm_slug: The realm slug of the character you want to get the raids from.
             character_name: The character name of the character you want to get the raids from.
@@ -84,20 +84,20 @@
         Raises:
             ValueError: If realm_slug is not provided.
             ValueError: If character_name is not provided.
         """
 
         if realm_slug is None:
             raise ValueError('realm_slug is required')
-        
+
         if character_name is None:
             raise ValueError('character_name is required')
 
         api = f'/profile/wow/character/{realm_slug}/{character_name}/encounters/raids'
 
         query_params = {
             'namespace': 'profile',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/profile_data/character_equipment.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/profile_data/character_equipment.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,20 +20,20 @@
         Raises:
             ValueError: If realm_slug is not provided.
             ValueError: If character_name is not provided.
         """
 
         if realm_slug is None:
             raise ValueError('realm_slug is required')
-        
+
         if character_name is None:
             raise ValueError('character_name is required')
 
         api = f'/profile/wow/character/{realm_slug}/{character_name}/equipment'
 
         query_params = {
             'namespace': 'profile',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/profile_data/character_hunter_pets.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/profile_data/character_hunter_pets.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,20 +20,20 @@
         Raises:
             ValueError: If realm_slug is not provided.
             ValueError: If character_name is not provided.
         """
 
         if realm_slug is None:
             raise ValueError('realm_slug is required')
-        
+
         if character_name is None:
             raise ValueError('character_name is required')
 
         api = f'/profile/wow/character/{realm_slug}/{character_name}/hunter-pets'
 
         query_params = {
             'namespace': 'profile',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/profile_data/character_media.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/profile_data/character_statistics.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 from typing import Optional, Dict, Any
 from ...api import API
 
-class CharacterMedia(API):
+class CharacterStatistics(API):
     def __init__(self, client_id, client_secret):
         super().__init__(client_id, client_secret)
 
-    def get_character_media_summary(self, realm_slug: str, character_name: str, **kwargs: Any) -> Dict:
+    def get_character_statistics_summary(self, realm_slug: str, character_name: str, **kwargs: Any) -> Dict:
         """
-        Returns the character media summary from the API.
+        Returns the character statistics summary from the API.
 
         Args:
-            realm_slug: The realm slug of the character you want to get the media summary from.
-            character_name: The character name of the character you want to get the media summary from.
+            access_token: The access token of the API endpoint you want to use.
+            realm_slug: The realm slug of the character you want to get the statistics summary from.
+            character_name: The character name of the character you want to get the statistics summary from.
 
         Return:
-            The character media summary.
+            The character statistics summary.
 
         Raises:
             ValueError: If realm_slug is not provided.
-            ValueError: If character_name is not provided.
+            ValueError: If character_name is not provided.C
         """
 
         if realm_slug is None:
             raise ValueError('realm_slug is required')
-        
+
         if character_name is None:
             raise ValueError('character_name is required')
 
-        api = f'/profile/wow/character/{realm_slug}/{character_name}/character-media'
+        api = f'/profile/wow/character/{realm_slug}/{character_name}/statistics'
 
         query_params = {
             'namespace': 'profile',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/profile_data/character_mythic_keystone_profile.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/profile_data/character_mythic_keystone_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,28 +19,28 @@
         Raises:
             ValueError: If realm_slug is not provided.
             ValueError: If character_name is not provided.
         """
 
         if realm_slug is None:
             raise ValueError('realm_slug is required')
-        
+
         if character_name is None:
             raise ValueError('character_name is required')
 
         api = f'/profile/wow/character/{realm_slug}/{character_name}/mythic-keystone-profile'
 
         query_params = {
             'namespace': 'profile',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
-    
+        return super().get_api(api=api, query_params=query_params, **kwargs)
+
     def get_character_mythic_keystone_season_details(self, realm_slug: str, character_name: str, season_id: int, **kwargs: Any) -> Dict:
         """
         Returns the character mythic keystone season details from the API.
 
         Args:
             realm_slug: The realm slug of the character you want to get the mythic keystone season details from.
             character_name: The character name of the character you want to get the mythic keystone season details from.
@@ -53,24 +53,23 @@
             ValueError: If realm_slug is not provided.
             ValueError: If character_name is not provided.
             ValueError: If season_id is not provided.
         """
 
         if realm_slug is None:
             raise ValueError('realm_slug is required')
-        
+
         if character_name is None:
             raise ValueError('character_name is required')
-        
+
         if season_id is None:
             raise ValueError('season_id is required')
 
         api = f'/profile/wow/character/{realm_slug}/{character_name}/mythic-keystone-profile/season/{season_id}'
 
         query_params = {
             'namespace': 'profile',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
-        
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/profile_data/character_professions.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/profile_data/character_professions.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,20 +19,20 @@
         Raises:
             ValueError: If realm_slug is not provided.
             ValueError: If character_name is not provided.
         """
 
         if realm_slug is None:
             raise ValueError('realm_slug is required')
-        
+
         if character_name is None:
             raise ValueError('character_name is required')
 
         api = f'/profile/wow/character/{realm_slug}/{character_name}/professions'
 
         query_params = {
             'namespace': 'profile',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/profile_data/character_profile.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/profile_data/character_profile.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,28 +20,28 @@
         Raises:
             ValueError: If realm_slug is not provided.
             ValueError: If character_name is not provided.
         """
 
         if realm_slug is None:
             raise ValueError('realm_slug is required')
-        
+
         if character_name is None:
             raise ValueError('character_name is required')
 
         api = f'/profile/wow/character/{realm_slug}/{character_name}'
 
         query_params = {
             'namespace': 'profile',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
-    
+        return super().get_api(api=api, query_params=query_params, **kwargs)
+
     def get_character_profile_status(self, realm_slug: str, character_name: str, **kwargs: Any) -> Dict:
         """
         Returns the character profile status from the API.
 
         Args:
             access_token: The access token of the API endpoint you want to use.
             realm_slug: The realm slug of the character you want to get the profile status from.
@@ -53,20 +53,20 @@
         Raises:
             ValueError: If realm_slug is not provided.
             ValueError: If character_name is not provided.
         """
 
         if realm_slug is None:
             raise ValueError('realm_slug is required')
-        
+
         if character_name is None:
             raise ValueError('character_name is required')
 
         api = f'/profile/wow/character/{realm_slug}/{character_name}/status'
 
         query_params = {
             'namespace': 'profile',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/profile_data/character_pvp.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/profile_data/character_pvp.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,31 +22,31 @@
             ValueError: If realm_slug is not provided.
             ValueError: If character_name is not provided.
             ValueError: If bracket is not provided.
         """
 
         if realm_slug is None:
             raise ValueError('realm_slug is required')
-        
+
         if character_name is None:
             raise ValueError('character_name is required')
 
         if bracket is None:
             raise ValueError('bracket is required')
 
         api = f'/profile/wow/character/{realm_slug}/{character_name}/pvp-bracket/{bracket}'
 
         query_params = {
             'namespace': 'profile',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
-    
+        return super().get_api(api=api, query_params=query_params, **kwargs)
+
     def get_character_pvp_summary(self, realm_slug: str, character_name: str, **kwargs: Any) -> Dict:
         """
         Returns the character pvp summary from the API.
 
         Args:
             access_token: The access token of the API endpoint you want to use.
             realm_slug: The realm slug of the character you want to get the pvp summary from.
@@ -58,20 +58,20 @@
         Raises:
             ValueError: If realm_slug is not provided.
             ValueError: If character_name is not provided.
         """
 
         if realm_slug is None:
             raise ValueError('realm_slug is required')
-        
+
         if character_name is None:
             raise ValueError('character_name is required')
 
         api = f'/profile/wow/character/{realm_slug}/{character_name}/pvp-summary'
 
         query_params = {
             'namespace': 'profile',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/profile_data/character_quests.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/profile_data/character_quests.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,28 +20,28 @@
         Raises:
             ValueError: If realm_slug is not provided.
             ValueError: If character_name is not provided.
         """
 
         if realm_slug is None:
             raise ValueError('realm_slug is required')
-        
+
         if character_name is None:
             raise ValueError('character_name is required')
 
         api = f'/profile/wow/character/{realm_slug}/{character_name}/quests'
 
         query_params = {
             'namespace': 'profile',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
-    
+        return super().get_api(api=api, query_params=query_params, **kwargs)
+
     def get_character_completed_quests(self, realm_slug: str, character_name: str, **kwargs: Any) -> Dict:
         """
         Returns the character completed quests from the API.
 
         Args:
             access_token: The access token of the API endpoint you want to use.
             realm_slug: The realm slug of the character you want to get the completed quests from.
@@ -53,20 +53,20 @@
         Raises:
             ValueError: If realm_slug is not provided.
             ValueError: If character_name is not provided.
         """
 
         if realm_slug is None:
             raise ValueError('realm_slug is required')
-        
+
         if character_name is None:
             raise ValueError('character_name is required')
 
         api = f'/profile/wow/character/{realm_slug}/{character_name}/quests/completed'
 
         query_params = {
             'namespace': 'profile',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/profile_data/character_reputations.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/profile_data/character_reputations.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,20 +20,20 @@
         Raises:
             ValueError: If realm_slug is not provided.
             ValueError: If character_name is not provided.
         """
 
         if realm_slug is None:
             raise ValueError('realm_slug is required')
-        
+
         if character_name is None:
             raise ValueError('character_name is required')
 
         api = f'/profile/wow/character/{realm_slug}/{character_name}/reputations'
 
         query_params = {
             'namespace': 'profile',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/profile_data/character_soulbinds.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/profile_data/character_soulbinds.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,20 +19,20 @@
         Raises:
             ValueError: If realm_slug is not provided.
             ValueError: If character_name is not provided.
         """
 
         if realm_slug is None:
             raise ValueError('realm_slug is required')
-        
+
         if character_name is None:
             raise ValueError('character_name is required')
 
         api = f'/profile/wow/character/{realm_slug}/{character_name}/soulbinds'
 
         query_params = {
             'namespace': 'profile',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/profile_data/character_specializations.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/profile_data/character_specializations.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,20 +20,20 @@
         Raises:
             ValueError: If realm_slug is not provided.
             ValueError: If character_name is not provided.
         """
 
         if realm_slug is None:
             raise ValueError('realm_slug is required')
-        
+
         if character_name is None:
             raise ValueError('character_name is required')
 
         api = f'/profile/wow/character/{realm_slug}/{character_name}/specializations'
 
         query_params = {
             'namespace': 'profile',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/profile_data/character_statistics.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/profile_data/character_titles.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 from typing import Optional, Dict, Any
 from ...api import API
 
-class CharacterStatistics(API):
+class CharacterTitles(API):
     def __init__(self, client_id, client_secret):
         super().__init__(client_id, client_secret)
 
-    def get_character_statistics_summary(self, realm_slug: str, character_name: str, **kwargs: Any) -> Dict:
+    def get_character_titles_summary(self, realm_slug: str, character_name: str, **kwargs: Any) -> Dict:
         """
-        Returns the character statistics summary from the API.
+        Returns the character titles summary from the API.
 
         Args:
-            access_token: The access token of the API endpoint you want to use.
-            realm_slug: The realm slug of the character you want to get the statistics summary from.
-            character_name: The character name of the character you want to get the statistics summary from.
+            realm_slug: The realm slug of the character you want to get the titles summary from.
+            character_name: The character name of the character you want to get the titles summary from.
 
         Return:
-            The character statistics summary.
+            The character titles summary.
 
         Raises:
             ValueError: If realm_slug is not provided.
-            ValueError: If character_name is not provided.C
+            ValueError: If character_name is not provided.
         """
 
         if realm_slug is None:
             raise ValueError('realm_slug is required')
-        
+
         if character_name is None:
             raise ValueError('character_name is required')
 
-        api = f'/profile/wow/character/{realm_slug}/{character_name}/statistics'
+        api = f'/profile/wow/character/{realm_slug}/{character_name}/titles'
 
         query_params = {
             'namespace': 'profile',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/profile_data/character_titles.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/profile_data/character_media.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 from typing import Optional, Dict, Any
 from ...api import API
 
-class CharacterTitles(API):
+class CharacterMedia(API):
     def __init__(self, client_id, client_secret):
         super().__init__(client_id, client_secret)
 
-    def get_character_titles_summary(self, realm_slug: str, character_name: str, **kwargs: Any) -> Dict:
+    def get_character_media_summary(self, realm_slug: str, character_name: str, **kwargs: Any) -> Dict:
         """
-        Returns the character titles summary from the API.
+        Returns the character media summary from the API.
 
         Args:
-            realm_slug: The realm slug of the character you want to get the titles summary from.
-            character_name: The character name of the character you want to get the titles summary from.
+            realm_slug: The realm slug of the character you want to get the media summary from.
+            character_name: The character name of the character you want to get the media summary from.
 
         Return:
-            The character titles summary.
+            The character media summary.
 
         Raises:
             ValueError: If realm_slug is not provided.
             ValueError: If character_name is not provided.
         """
 
         if realm_slug is None:
             raise ValueError('realm_slug is required')
-        
+
         if character_name is None:
             raise ValueError('character_name is required')
 
-        api = f'/profile/wow/character/{realm_slug}/{character_name}/titles'
+        api = f'/profile/wow/character/{realm_slug}/{character_name}/character-media'
 
         query_params = {
             'namespace': 'profile',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/profile_data/guild.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/profile_data/guild.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,28 +19,28 @@
         Raises:
             ValueError: If realm_slug is not provided.
             ValueError: If guild_slug is not provided.
         """
 
         if realm_slug is None:
             raise ValueError('realm_slug is required')
-        
+
         if guild_slug is None:
             raise ValueError('guild_slug is required')
 
         api = f'/data/wow/guild/{realm_slug}/{guild_slug}'
 
         query_params = {
             'namespace': 'profile',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
-    
+        return super().get_api(api=api, query_params=query_params, **kwargs)
+
     def get_guild_activity(self, realm_slug: str, guild_slug: str, **kwargs: Any) -> Dict:
         """
         Returns the guild activity from the API.
 
         Args:
             realm_slug: The realm slug of the guild you want to get the activity from.
             guild_slug: The guild name of the guild you want to get the activity from.
@@ -51,28 +51,28 @@
         Raises:
             ValueError: If realm_slug is not provided.
             ValueError: If guild_slug is not provided.
         """
 
         if realm_slug is None:
             raise ValueError('realm_slug is required')
-        
+
         if guild_slug is None:
             raise ValueError('guild_slug is required')
 
         api = f'/data/wow/guild/{realm_slug}/{guild_slug}/activity'
 
         query_params = {
             'namespace': 'profile',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
-    
+        return super().get_api(api=api, query_params=query_params, **kwargs)
+
     def get_guild_achievements(self, realm_slug: str, guild_slug: str, **kwargs: Any) -> Dict:
         """
         Returns the guild achievements from the API.
 
         Args:
             realm_slug: The realm slug of the guild you want to get the achievements from.
             guild_slug: The guild name of the guild you want to get the achievements from.
@@ -83,28 +83,28 @@
         Raises:
             ValueError: If realm_slug is not provided.
             ValueError: If guild_slug is not provided.
         """
 
         if realm_slug is None:
             raise ValueError('realm_slug is required')
-        
+
         if guild_slug is None:
             raise ValueError('guild_slug is required')
 
         api = f'/data/wow/guild/{realm_slug}/{guild_slug}/achievements'
 
         query_params = {
             'namespace': 'profile',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
-    
+        return super().get_api(api=api, query_params=query_params, **kwargs)
+
     def get_guild_roster(self, realm_slug: str, guild_slug: str, **kwargs: Any) -> Dict:
         """
         Returns the guild roster from the API.
 
         Args:
             realm_slug: The realm slug of the guild you want to get the roster from.
             guild_slug: The guild name of the guild you want to get the roster from.
@@ -115,20 +115,20 @@
         Raises:
             ValueError: If realm_slug is not provided.
             ValueError: If guild_slug is not provided.
         """
 
         if realm_slug is None:
             raise ValueError('realm_slug is required')
-        
+
         if guild_slug is None:
             raise ValueError('guild_slug is required')
 
         api = f'/data/wow/guild/{realm_slug}/{guild_slug}/roster'
 
         query_params = {
             'namespace': 'profile',
         }
 
         query_params.update(kwargs)
 
-        return super().get_api(api=api, query_params=query_params, kwargs=kwargs)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python-ndev-blizzardapi-0.1.2/blizzardAPI/world_of_warcraft/wow_api.py` & `python_ndev_blizzardapi-0.2.0/blizzardAPI/world_of_warcraft/wow_api.py`

 * *Files identical despite different names*

### Comparing `python-ndev-blizzardapi-0.1.2/python_ndev_blizzardapi.egg-info/PKG-INFO` & `python_ndev_blizzardapi-0.2.0/python_ndev_blizzardapi.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-ndev-blizzardapi
-Version: 0.1.2
+Version: 0.2.0
 Summary: Python module created to integrate your Python project with the Blizzard API
 Home-page: https://github.com/natanrmaia/python-ndev-blizzardapi
 Author: natanrmaia
 Author-email: contato@natanael.dev.br
 Project-URL: Documentation, https://python-ndev-blizzardapi.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/natanrmaia/python-ndev-blizzardapi
 Project-URL: Bug Reports, https://github.com/natanrmaia/python-ndev-blizzardapi/issues
```

### Comparing `python-ndev-blizzardapi-0.1.2/python_ndev_blizzardapi.egg-info/SOURCES.txt` & `python_ndev_blizzardapi-0.2.0/python_ndev_blizzardapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-ndev-blizzardapi-0.1.2/setup.py` & `python_ndev_blizzardapi-0.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="python-ndev-blizzardapi",
-    version="0.1.2",
+    version="0.2.0",
     packages=find_packages(),
     install_requires=[
         "requests>=2.28.2",
         "python-dotenv>=1.0.0",
     ],
     author="natanrmaia",
     author_email="contato@natanael.dev.br",
```

