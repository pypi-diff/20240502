# Comparing `tmp/python_ndev_blizzardapi-0.2.1.tar.gz` & `tmp/python_ndev_blizzardapi-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_ndev_blizzardapi-0.2.1.tar", last modified: Tue Apr 30 14:03:57 2024, max compression
+gzip compressed data, was "python_ndev_blizzardapi-0.2.2.tar", last modified: Thu May  2 05:10:52 2024, max compression
```

## Comparing `python_ndev_blizzardapi-0.2.1.tar` & `python_ndev_blizzardapi-0.2.2.tar`

### file list

```diff
@@ -1,84 +1,87 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 14:03:57.028385 python_ndev_blizzardapi-0.2.1/
--rw-rw-rw-   0        0        0      134 2023-07-14 20:43:22.000000 python_ndev_blizzardapi-0.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3319 2024-04-30 14:03:57.026382 python_ndev_blizzardapi-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     2522 2023-07-23 03:28:03.000000 python_ndev_blizzardapi-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-30 14:03:56.308329 python_ndev_blizzardapi-0.2.1/blizzardAPI/
--rw-rw-rw-   0        0        0      161 2023-03-11 02:36:09.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/__init__.py
--rw-rw-rw-   0        0        0     5073 2024-04-30 13:47:44.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/api.py
-drwxrwxrwx   0        0        0        0 2024-04-30 14:03:56.322861 python_ndev_blizzardapi-0.2.1/blizzardAPI/battlenet/
--rw-rw-rw-   0        0        0       25 2023-03-10 03:36:02.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/battlenet/__init__.py
--rw-rw-rw-   0        0        0      458 2023-07-30 21:32:26.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/battlenet/battlenet_api.py
--rw-rw-rw-   0        0        0     1539 2023-07-30 21:32:29.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/battlenet/battlenet_oauth.py
--rw-rw-rw-   0        0        0     1475 2023-07-30 21:32:30.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/blizzard_api.py
-drwxrwxrwx   0        0        0        0 2024-04-30 14:03:56.332909 python_ndev_blizzardapi-0.2.1/blizzardAPI/tests/
--rw-rw-rw-   0        0        0        0 2023-06-21 22:10:25.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/tests/__init__.py
--rw-rw-rw-   0        0        0     3330 2023-07-23 02:33:06.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2024-04-30 14:03:56.342000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/
--rw-rw-rw-   0        0        0       25 2023-03-10 03:36:02.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 14:03:56.752368 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/
--rw-rw-rw-   0        0        0     5007 2023-07-07 03:47:18.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/__init__.py
--rw-rw-rw-   0        0        0     3905 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/achievement.py
--rw-rw-rw-   0        0        0     1580 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/auction_house.py
--rw-rw-rw-   0        0        0     3224 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/azerite_essence.py
--rw-rw-rw-   0        0        0     2166 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/connected_realm.py
--rw-rw-rw-   0        0        0     4876 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/covenant.py
--rw-rw-rw-   0        0        0     6308 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/creature.py
--rw-rw-rw-   0        0        0     2447 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/guild_crest.py
--rw-rw-rw-   0        0        0     1546 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/heirloom.py
--rw-rw-rw-   0        0        0     6064 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/item.py
--rw-rw-rw-   0        0        0     6036 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/journal.py
--rw-rw-rw-   0        0        0      693 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/media.py
--rw-rw-rw-   0        0        0     4290 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/modified_crafting.py
--rw-rw-rw-   0        0        0     1781 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/mount.py
--rw-rw-rw-   0        0        0     2293 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/mythic_keystone_affix.py
--rw-rw-rw-   0        0        0     4799 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/mythic_keystone_dungeon.py
--rw-rw-rw-   0        0        0     2196 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/mythic_keystone_leaderboard.py
--rw-rw-rw-   0        0        0     1261 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/mythic_raid_leaderboard.py
--rw-rw-rw-   0        0        0     3863 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/pet.py
--rw-rw-rw-   0        0        0     2919 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/playable_class.py
--rw-rw-rw-   0        0        0     1461 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/playable_race.py
--rw-rw-rw-   0        0        0     2292 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/playable_specialization.py
--rw-rw-rw-   0        0        0     1523 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/power_type.py
--rw-rw-rw-   0        0        0     5416 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/profession.py
--rw-rw-rw-   0        0        0     4051 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/pvp_season.py
--rw-rw-rw-   0        0        0     2353 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/pvp_tier.py
--rw-rw-rw-   0        0        0     5645 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/quest.py
--rw-rw-rw-   0        0        0     2246 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/realm.py
--rw-rw-rw-   0        0        0     1631 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/region.py
--rw-rw-rw-   0        0        0     3173 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/reputation.py
--rw-rw-rw-   0        0        0     2304 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/spell.py
--rw-rw-rw-   0        0        0     5321 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/talent.py
--rw-rw-rw-   0        0        0     3918 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/tech_talent.py
--rw-rw-rw-   0        0        0     1467 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/title.py
--rw-rw-rw-   0        0        0      969 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/token.py
--rw-rw-rw-   0        0        0     1602 2023-06-22 04:12:53.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/toy.py
-drwxrwxrwx   0        0        0        0 2024-04-30 14:03:57.007340 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/profile_data/
--rw-rw-rw-   0        0        0     3200 2023-07-17 17:14:22.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/profile_data/__init__.py
--rw-rw-rw-   0        0        0     7875 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/profile_data/account_profile.py
--rw-rw-rw-   0        0        0     2230 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/profile_data/character_achievements.py
--rw-rw-rw-   0        0        0     1644 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/profile_data/character_appearance.py
--rw-rw-rw-   0        0        0     4904 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/profile_data/character_collections.py
--rw-rw-rw-   0        0        0     3478 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/profile_data/character_encounters.py
--rw-rw-rw-   0        0        0     1373 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/profile_data/character_equipment.py
--rw-rw-rw-   0        0        0     1386 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/profile_data/character_hunter_pets.py
--rw-rw-rw-   0        0        0     1274 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/profile_data/character_media.py
--rw-rw-rw-   0        0        0     2842 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/profile_data/character_mythic_keystone_profile.py
--rw-rw-rw-   0        0        0     1306 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/profile_data/character_professions.py
--rw-rw-rw-   0        0        0     2507 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/profile_data/character_profile.py
--rw-rw-rw-   0        0        0     2776 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/profile_data/character_pvp.py
--rw-rw-rw-   0        0        0     2488 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/profile_data/character_quests.py
--rw-rw-rw-   0        0        0     1387 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/profile_data/character_reputations.py
--rw-rw-rw-   0        0        0     1252 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/profile_data/character_soulbinds.py
--rw-rw-rw-   0        0        0     1415 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/profile_data/character_specializations.py
--rw-rw-rw-   0        0        0     1381 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/profile_data/character_statistics.py
--rw-rw-rw-   0        0        0     1273 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/profile_data/character_titles.py
--rw-rw-rw-   0        0        0     4096 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/profile_data/guild.py
--rw-rw-rw-   0        0        0      533 2023-07-17 03:21:56.000000 python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/wow_api.py
-drwxrwxrwx   0        0        0        0 2024-04-30 14:03:57.023874 python_ndev_blizzardapi-0.2.1/python_ndev_blizzardapi.egg-info/
--rw-rw-rw-   0        0        0     3319 2024-04-30 14:03:56.000000 python_ndev_blizzardapi-0.2.1/python_ndev_blizzardapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3864 2024-04-30 14:03:56.000000 python_ndev_blizzardapi-0.2.1/python_ndev_blizzardapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 14:03:56.000000 python_ndev_blizzardapi-0.2.1/python_ndev_blizzardapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-04-30 14:03:56.000000 python_ndev_blizzardapi-0.2.1/python_ndev_blizzardapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-30 14:03:56.000000 python_ndev_blizzardapi-0.2.1/python_ndev_blizzardapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-30 14:03:57.029414 python_ndev_blizzardapi-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1033 2024-04-30 13:51:32.000000 python_ndev_blizzardapi-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 05:10:52.683742 python_ndev_blizzardapi-0.2.2/
+-rw-rw-rw-   0        0        0      134 2023-07-14 20:43:22.000000 python_ndev_blizzardapi-0.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3319 2024-05-02 05:10:52.680742 python_ndev_blizzardapi-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2522 2023-07-23 03:28:03.000000 python_ndev_blizzardapi-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 05:10:52.365224 python_ndev_blizzardapi-0.2.2/blizzardAPI/
+-rw-rw-rw-   0        0        0      162 2024-05-02 04:36:51.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/__init__.py
+-rw-rw-rw-   0        0        0     6075 2024-05-02 04:33:15.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/api.py
+drwxrwxrwx   0        0        0        0 2024-05-02 05:10:52.375227 python_ndev_blizzardapi-0.2.2/blizzardAPI/battlenet/
+-rw-rw-rw-   0        0        0       25 2023-03-10 03:36:02.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/battlenet/__init__.py
+-rw-rw-rw-   0        0        0      458 2023-07-30 21:32:26.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/battlenet/battlenet_api.py
+-rw-rw-rw-   0        0        0     1539 2023-07-30 21:32:29.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/battlenet/battlenet_oauth.py
+-rw-rw-rw-   0        0        0     1475 2023-07-30 21:32:30.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/blizzard_api.py
+drwxrwxrwx   0        0        0        0 2024-05-02 05:10:52.380224 python_ndev_blizzardapi-0.2.2/blizzardAPI/exceptions/
+-rw-rw-rw-   0        0        0       22 2024-05-02 04:30:03.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/exceptions/__init__.py
+-rw-rw-rw-   0        0        0     2464 2024-05-02 04:20:05.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/exceptions/handler.py
+drwxrwxrwx   0        0        0        0 2024-05-02 05:10:52.386225 python_ndev_blizzardapi-0.2.2/blizzardAPI/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-21 22:10:25.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/tests/__init__.py
+-rw-rw-rw-   0        0        0     3330 2023-07-23 02:33:06.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2024-05-02 05:10:52.393228 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/
+-rw-rw-rw-   0        0        0       25 2023-03-10 03:36:02.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 05:10:52.510253 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/
+-rw-rw-rw-   0        0        0     5007 2023-07-07 03:47:18.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/__init__.py
+-rw-rw-rw-   0        0        0     3905 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/achievement.py
+-rw-rw-rw-   0        0        0     1580 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/auction_house.py
+-rw-rw-rw-   0        0        0     3224 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/azerite_essence.py
+-rw-rw-rw-   0        0        0     2166 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/connected_realm.py
+-rw-rw-rw-   0        0        0     4876 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/covenant.py
+-rw-rw-rw-   0        0        0     6308 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/creature.py
+-rw-rw-rw-   0        0        0     2447 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/guild_crest.py
+-rw-rw-rw-   0        0        0     1546 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/heirloom.py
+-rw-rw-rw-   0        0        0     6064 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/item.py
+-rw-rw-rw-   0        0        0     6036 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/journal.py
+-rw-rw-rw-   0        0        0      693 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/media.py
+-rw-rw-rw-   0        0        0     4290 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/modified_crafting.py
+-rw-rw-rw-   0        0        0     1781 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/mount.py
+-rw-rw-rw-   0        0        0     2293 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/mythic_keystone_affix.py
+-rw-rw-rw-   0        0        0     4799 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/mythic_keystone_dungeon.py
+-rw-rw-rw-   0        0        0     2196 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/mythic_keystone_leaderboard.py
+-rw-rw-rw-   0        0        0     1261 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/mythic_raid_leaderboard.py
+-rw-rw-rw-   0        0        0     3863 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/pet.py
+-rw-rw-rw-   0        0        0     2919 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/playable_class.py
+-rw-rw-rw-   0        0        0     1461 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/playable_race.py
+-rw-rw-rw-   0        0        0     2292 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/playable_specialization.py
+-rw-rw-rw-   0        0        0     1523 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/power_type.py
+-rw-rw-rw-   0        0        0     5416 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/profession.py
+-rw-rw-rw-   0        0        0     4051 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/pvp_season.py
+-rw-rw-rw-   0        0        0     2353 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/pvp_tier.py
+-rw-rw-rw-   0        0        0     5645 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/quest.py
+-rw-rw-rw-   0        0        0     2246 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/realm.py
+-rw-rw-rw-   0        0        0     1631 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/region.py
+-rw-rw-rw-   0        0        0     3173 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/reputation.py
+-rw-rw-rw-   0        0        0     2304 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/spell.py
+-rw-rw-rw-   0        0        0     5321 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/talent.py
+-rw-rw-rw-   0        0        0     3918 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/tech_talent.py
+-rw-rw-rw-   0        0        0     1467 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/title.py
+-rw-rw-rw-   0        0        0      969 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/token.py
+-rw-rw-rw-   0        0        0     1602 2023-06-22 04:12:53.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/toy.py
+drwxrwxrwx   0        0        0        0 2024-05-02 05:10:52.665231 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/profile_data/
+-rw-rw-rw-   0        0        0     3200 2023-07-17 17:14:22.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/profile_data/__init__.py
+-rw-rw-rw-   0        0        0     7875 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/profile_data/account_profile.py
+-rw-rw-rw-   0        0        0     2230 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/profile_data/character_achievements.py
+-rw-rw-rw-   0        0        0     1644 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/profile_data/character_appearance.py
+-rw-rw-rw-   0        0        0     4904 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/profile_data/character_collections.py
+-rw-rw-rw-   0        0        0     3478 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/profile_data/character_encounters.py
+-rw-rw-rw-   0        0        0     1373 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/profile_data/character_equipment.py
+-rw-rw-rw-   0        0        0     1386 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/profile_data/character_hunter_pets.py
+-rw-rw-rw-   0        0        0     1274 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/profile_data/character_media.py
+-rw-rw-rw-   0        0        0     2842 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/profile_data/character_mythic_keystone_profile.py
+-rw-rw-rw-   0        0        0     1306 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/profile_data/character_professions.py
+-rw-rw-rw-   0        0        0     2507 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/profile_data/character_profile.py
+-rw-rw-rw-   0        0        0     2776 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/profile_data/character_pvp.py
+-rw-rw-rw-   0        0        0     2488 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/profile_data/character_quests.py
+-rw-rw-rw-   0        0        0     1387 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/profile_data/character_reputations.py
+-rw-rw-rw-   0        0        0     1252 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/profile_data/character_soulbinds.py
+-rw-rw-rw-   0        0        0     1415 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/profile_data/character_specializations.py
+-rw-rw-rw-   0        0        0     1381 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/profile_data/character_statistics.py
+-rw-rw-rw-   0        0        0     1273 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/profile_data/character_titles.py
+-rw-rw-rw-   0        0        0     4096 2024-04-25 15:36:13.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/profile_data/guild.py
+-rw-rw-rw-   0        0        0      533 2023-07-17 03:21:56.000000 python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/wow_api.py
+drwxrwxrwx   0        0        0        0 2024-05-02 05:10:52.678230 python_ndev_blizzardapi-0.2.2/python_ndev_blizzardapi.egg-info/
+-rw-rw-rw-   0        0        0     3319 2024-05-02 05:10:52.000000 python_ndev_blizzardapi-0.2.2/python_ndev_blizzardapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3933 2024-05-02 05:10:52.000000 python_ndev_blizzardapi-0.2.2/python_ndev_blizzardapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 05:10:52.000000 python_ndev_blizzardapi-0.2.2/python_ndev_blizzardapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-02 05:10:52.000000 python_ndev_blizzardapi-0.2.2/python_ndev_blizzardapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-02 05:10:52.000000 python_ndev_blizzardapi-0.2.2/python_ndev_blizzardapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-02 05:10:52.683742 python_ndev_blizzardapi-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1033 2024-05-02 03:54:30.000000 python_ndev_blizzardapi-0.2.2/setup.py
```

### Comparing `python_ndev_blizzardapi-0.2.1/PKG-INFO` & `python_ndev_blizzardapi-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-ndev-blizzardapi
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python module created to integrate your Python project with the Blizzard API
 Home-page: https://github.com/natanrmaia/python-ndev-blizzardapi
 Author: natanrmaia
 Author-email: contato@natanael.dev.br
 Project-URL: Documentation, https://python-ndev-blizzardapi.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/natanrmaia/python-ndev-blizzardapi
 Project-URL: Bug Reports, https://github.com/natanrmaia/python-ndev-blizzardapi/issues
```

### Comparing `python_ndev_blizzardapi-0.2.1/README.md` & `python_ndev_blizzardapi-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/api.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/profession.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,139 +1,186 @@
-import requests, os, importlib, inspect
+from typing import Dict, Optional, Any
+from ...api import API
 
-class API:
+class Profession(API):
 
     def __init__(self, client_id, client_secret):
+        super().__init__(client_id, client_secret)
 
-        """ API Keys """
-        self.client_id      = client_id         # <--- self.client_id
-        self.client_secret  = client_secret     # <--- self.client_secret
-        self.access_token   = None              # <--- self.access_token
+    def get_professions_index(self, **kwargs: Any) -> Dict:
+        """
+        This function will return the index of professions from the API.
+
+        Requested API:
+            /data/wow/profession/index
+
+        Returns:
+            A dictionary of the professions index.
+        """
 
-        """ API URLs for regions (US, EU, KR, TW) """
-        self.api_url        = 'https://{0}.api.blizzard.com{1}'
-        self.oauth_url      = 'https://{0}.battle.net{1}'
+        api = '/data/wow/profession/index'
 
-        """ API URLs for regions (CN) """
-        self.api_url_cn     = 'https://gateway.battlenet.com.cn{0}'
-        self.oauth_url_cn   = 'https://www.battlenet.com.cn{0}'
+        query_params = {
+            'namespace': 'static',
+        }
+
+        query_params.update(kwargs)
 
-        """ Session """
-        self.session        = requests.Session()
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
-    def format_url(self, region, api, format_url='api'):
+    def get_profession(self, profession_id: int, **kwargs: Any) -> Dict:
         """
-        It takes a region, an api, and a format_url, and returns a url
+        This function will return the details of a specific profession from the API.
+
+        Requested API:
+            /data/wow/profession/{professionId}
+
+        Args:
+            profession_id: The ID of the profession you want to retrieve.
 
-        :param region: The region of the server you want to connect to
-        :param api: The API you want to call
-        :param format_url: This is the type of URL you want to format, defaults to api (optional) Options: api, oauth
-        :return: The url is being returned.
+        Returns:
+            A dictionary of the profession details.
+
+        Raises:
+            ValueError: If the profession ID is not valid.
         """
 
-        if format_url == 'api':
-            if region == 'cn':
-                url = self.api_url_cn.format(api)
-            else:
-                url = self.api_url.format(region, api)
+        if profession_id is None:
+            raise ValueError('Profession ID cannot be None.')
+
+        api = f'/data/wow/profession/{profession_id}'
 
-        elif format_url == 'oauth':
-            if region == 'cn':
-                url = self.oauth_url_cn.format(api)
-            else:
-                url = self.oauth_url.format(region, api)
+        query_params = {
+            'namespace': 'static',
+        }
 
-        else:
-            raise ValueError('format_url must be either api or oauth')
+        query_params.update(kwargs)
 
-        return url
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
-    def get_client_token(self, region):
+    def get_profession_media(self, profession_id: int, **kwargs: Any) -> Dict:
         """
-        It takes no parameters, and returns the access token
+        This function will return the media of a specific profession from the API.
+
+        Requested API:
+            /data/wow/media/profession/{professionId}
 
-        :return: The access token is being returned.
+        Args:
+            profession_id: The ID of the profession you want to retrieve.
+
+        Returns:
+            A dictionary of the profession media.
+
+        Raises:
+            ValueError: If the profession ID is not valid.
         """
-        url = self.format_url(region, '/oauth/token', 'oauth')
-        data = {
-            'grant_type': 'client_credentials',
+
+        if profession_id is None:
+            raise ValueError('Profession ID cannot be None.')
+
+        api = f'/data/wow/media/profession/{profession_id}'
+
+        query_params = {
+            'namespace': 'static',
         }
-        response = self.session.post(url, data=data, auth=(self.client_id, self.client_secret))
 
-        return self.response_handler(response)
+        query_params.update(kwargs)
+
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
-    def response_handler(self, response):
+    def get_profession_skill_tier(self, profession_id: int, skill_tier_id: int, **kwargs: Any) -> Dict:
         """
-        It takes a response object, and returns the response object's json() method
+        This function will return the details of a specific profession skill tier from the API.
+
+        Requested API:
+            /data/wow/profession/{professionId}/skill-tier/{skillTierId}
+
+        Args:
+            profession_id: The ID of the profession you want to retrieve.
+            skill_tier_id: The ID of the skill tier you want to retrieve.
 
-        :param response: The response object returned by the request
-        :return: The response.json() method will convert the JSON string into a Python dictionary.
+        Returns:
+            A dictionary of the profession skill tier details.
+
+        Raises:
+            ValueError: If the profession ID is not valid.
+            ValueError: If the skill tier ID is not valid.
         """
 
-        if response.status_code != 200:
-            msg = 'The response code was {0}. Error: {1}'.format(response.status_code, response.text)
-            raise ValueError(msg)
+        if profession_id is None:
+            raise ValueError('Profession ID cannot be None.')
 
-        return response.json()
+        if skill_tier_id is None:
+            raise ValueError('Skill tier ID cannot be None.')
 
-    def request_handler(self, url, region, query_params):
 
-        if self.access_token is None:
-            client_token = self.get_client_token(region)
-            self.access_token = client_token['access_token']
+        api = f'/data/wow/profession/{profession_id}/skill-tier/{skill_tier_id}'
 
-        if query_params.get('access_token') is None:
-            query_params['access_token'] = self.access_token
+        query_params = {
+            'namespace': 'static',
+        }
 
-        response = self.session.get(url, params=query_params)
+        query_params.update(kwargs)
 
-        return self.response_handler(response)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
-    def get_api(self, **kwargs):
+    def get_recipe(self, recipe_id: int, **kwargs: Any) -> Dict:
         """
-        It takes a region, an api, and query_params, and returns the response
+        This function will return the details of a specific recipe from the API.
 
-        :param region: The region of the server you want to connect to
-        :param api: The API you want to call
-        :param query_params: The query parameters you want to pass to the API (optional)
-        :return: The response is being returned.
-        """
+        Requested API:
+            /data/wow/recipe/{recipeId}
 
-        region          = kwargs.get('region')  or 'us'
-        api             = kwargs.get('api')     or None
-        query_params    = kwargs.get('query_params') or None
+        Args:
+            region: The region of the API you want to access.
+            recipe_id: The ID of the recipe you want to retrieve.
+            locale: The locale of the API you want to access.
 
-        if query_params is None:
-            query_params = {}
+        Returns:
+            A dictionary of the recipe details.
 
-        if 'access_token' not in query_params or query_params['access_token'] is None:
-            query_params['access_token'] = self.access_token
+        Raises:
+            ValueError: If the recipe ID is not valid.
+        """
 
-        if 'locale' not in query_params:
-            query_params['locale'] = ''
-        elif query_params['locale'] is None:
-            query_params['locale'] = ''
+        if recipe_id is None:
+            raise ValueError('Recipe ID cannot be None.')
 
-        if api is None:
-            raise ValueError('api cannot be None')
+        api = f'/data/wow/recipe/{recipe_id}'
 
-        query_params['namespace'] = '{}-{}'.format(query_params['namespace'], region)
+        query_params = {
+            'namespace': 'static',
+        }
 
-        url = self.format_url(region, api)
+        query_params.update(kwargs)
 
-        return self.request_handler(url, region, query_params)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
 
-    def get_oauth(self, region, api, query_params=None):
+    def get_recipe_media(self, recipe_id: int, **kwargs: Any) -> Dict:
         """
-        It takes a region, an api, and query_params, and returns the response
+        This function will return the media of a specific recipe from the API.
+
+        Requested API:
+            /data/wow/media/recipe/{recipeId}
+
+        Args:
+            recipe_id: The ID of the recipe you want to retrieve.
+
+        Returns:
+            A dictionary of the recipe media.
 
-        :param region: The region of the server you want to connect to
-        :param api: The API you want to call
-        :param query_params: The query parameters you want to pass to the API (optional)
-        :return: The response is being returned.
+        Raises:
+            ValueError: If the recipe ID is not valid.
         """
-        if query_params is None:
-            query_params = {}
 
-        url = self.format_url(region, api, 'oauth')
+        if recipe_id is None:
+            raise ValueError('Recipe ID cannot be None.')
+
+        api = f'/data/wow/media/recipe/{recipe_id}'
+
+        query_params = {
+            'namespace': 'static',
+        }
+
+        query_params.update(kwargs)
 
-        return self.request_handler(url, region, query_params)
+        return super().get_api(api=api, query_params=query_params, **kwargs)
```

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/battlenet/battlenet_oauth.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/battlenet/battlenet_oauth.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/blizzard_api.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/blizzard_api.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/tests/conftest.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/__init__.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/__init__.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/achievement.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/achievement.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/auction_house.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/auction_house.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/azerite_essence.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/azerite_essence.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/connected_realm.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/connected_realm.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/covenant.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/covenant.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/creature.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/creature.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/guild_crest.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/guild_crest.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/heirloom.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/heirloom.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/item.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/item.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/journal.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/journal.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/media.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/media.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/modified_crafting.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/modified_crafting.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/mount.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/mount.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/mythic_keystone_affix.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/mythic_keystone_affix.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/mythic_keystone_dungeon.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/mythic_keystone_dungeon.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/mythic_keystone_leaderboard.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/mythic_keystone_leaderboard.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/mythic_raid_leaderboard.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/mythic_raid_leaderboard.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/pet.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/pet.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/playable_class.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/playable_class.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/playable_race.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/playable_race.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/playable_specialization.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/playable_specialization.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/power_type.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/power_type.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/pvp_season.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/pvp_season.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/pvp_tier.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/pvp_tier.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/quest.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/quest.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/realm.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/realm.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/region.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/region.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/reputation.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/reputation.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/spell.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/spell.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/talent.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/talent.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/tech_talent.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/tech_talent.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/title.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/title.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/token.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/token.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/game_data/toy.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/game_data/toy.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/profile_data/__init__.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/profile_data/__init__.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/profile_data/account_profile.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/profile_data/account_profile.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/profile_data/character_achievements.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/profile_data/character_achievements.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/profile_data/character_appearance.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/profile_data/character_appearance.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/profile_data/character_collections.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/profile_data/character_collections.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/profile_data/character_encounters.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/profile_data/character_encounters.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/profile_data/character_equipment.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/profile_data/character_equipment.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/profile_data/character_hunter_pets.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/profile_data/character_hunter_pets.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/profile_data/character_media.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/profile_data/character_media.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/profile_data/character_mythic_keystone_profile.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/profile_data/character_mythic_keystone_profile.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/profile_data/character_professions.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/profile_data/character_professions.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/profile_data/character_profile.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/profile_data/character_profile.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/profile_data/character_pvp.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/profile_data/character_pvp.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/profile_data/character_quests.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/profile_data/character_quests.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/profile_data/character_reputations.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/profile_data/character_reputations.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/profile_data/character_soulbinds.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/profile_data/character_soulbinds.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/profile_data/character_specializations.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/profile_data/character_specializations.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/profile_data/character_statistics.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/profile_data/character_statistics.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/profile_data/character_titles.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/profile_data/character_titles.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/profile_data/guild.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/profile_data/guild.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/blizzardAPI/world_of_warcraft/wow_api.py` & `python_ndev_blizzardapi-0.2.2/blizzardAPI/world_of_warcraft/wow_api.py`

 * *Files identical despite different names*

### Comparing `python_ndev_blizzardapi-0.2.1/python_ndev_blizzardapi.egg-info/PKG-INFO` & `python_ndev_blizzardapi-0.2.2/python_ndev_blizzardapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-ndev-blizzardapi
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python module created to integrate your Python project with the Blizzard API
 Home-page: https://github.com/natanrmaia/python-ndev-blizzardapi
 Author: natanrmaia
 Author-email: contato@natanael.dev.br
 Project-URL: Documentation, https://python-ndev-blizzardapi.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/natanrmaia/python-ndev-blizzardapi
 Project-URL: Bug Reports, https://github.com/natanrmaia/python-ndev-blizzardapi/issues
```

### Comparing `python_ndev_blizzardapi-0.2.1/python_ndev_blizzardapi.egg-info/SOURCES.txt` & `python_ndev_blizzardapi-0.2.2/python_ndev_blizzardapi.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 setup.py
 blizzardAPI/__init__.py
 blizzardAPI/api.py
 blizzardAPI/blizzard_api.py
 blizzardAPI/battlenet/__init__.py
 blizzardAPI/battlenet/battlenet_api.py
 blizzardAPI/battlenet/battlenet_oauth.py
+blizzardAPI/exceptions/__init__.py
+blizzardAPI/exceptions/handler.py
 blizzardAPI/tests/__init__.py
 blizzardAPI/tests/conftest.py
 blizzardAPI/world_of_warcraft/__init__.py
 blizzardAPI/world_of_warcraft/wow_api.py
 blizzardAPI/world_of_warcraft/game_data/__init__.py
 blizzardAPI/world_of_warcraft/game_data/achievement.py
 blizzardAPI/world_of_warcraft/game_data/auction_house.py
```

### Comparing `python_ndev_blizzardapi-0.2.1/setup.py` & `python_ndev_blizzardapi-0.2.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="python-ndev-blizzardapi",
-    version="0.2.1",
+    version="0.2.2",
     packages=find_packages(),
     install_requires=[
         "requests>=2.28.2",
         "python-dotenv>=1.0.0",
     ],
     author="natanrmaia",
     author_email="contato@natanael.dev.br",
```

