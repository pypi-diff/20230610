# Comparing `tmp/Shark sac Korean editor-1.2.1.tar.gz` & `tmp/Shark sac Korean editor-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Shark sac Korean editor-1.2.1.tar", last modified: Sat Jun 10 07:29:41 2023, max compression
+gzip compressed data, was "Shark sac Korean editor-1.2.5.tar", last modified: Sat Jun 10 13:38:56 2023, max compression
```

## Comparing `Shark sac Korean editor-1.2.1.tar` & `Shark sac Korean editor-1.2.5.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 07:29:41.877987 Shark sac Korean editor-1.2.1/
--rw-rw-rw-   0        0        0      731 2023-06-10 07:29:41.876988 Shark sac Korean editor-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      198 2023-04-27 07:59:41.000000 Shark sac Korean editor-1.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-10 07:29:41.807956 Shark sac Korean editor-1.2.1/Shark_sac_Korean_editor.egg-info/
--rw-rw-rw-   0        0        0      731 2023-06-10 07:29:41.000000 Shark sac Korean editor-1.2.1/Shark_sac_Korean_editor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2708 2023-06-10 07:29:41.000000 Shark sac Korean editor-1.2.1/Shark_sac_Korean_editor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 07:29:41.000000 Shark sac Korean editor-1.2.1/Shark_sac_Korean_editor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-10 07:29:41.000000 Shark sac Korean editor-1.2.1/Shark_sac_Korean_editor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-10 07:29:41.823989 Shark sac Korean editor-1.2.1/modkr/
--rw-rw-rw-   0        0        0      283 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.2.1/modkr/__init__.py
--rw-rw-rw-   0        0        0     9136 2023-06-10 03:58:09.000000 Shark sac Korean editor-1.2.1/modkr/__main__.py
--rw-rw-rw-   0        0        0    10151 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.2.1/modkr/adb_handler.py
--rw-rw-rw-   0        0        0    13745 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.2.1/modkr/config_manager.py
--rw-rw-rw-   0        0        0     1510 2023-06-10 06:54:54.000000 Shark sac Korean editor-1.2.1/modkr/csv_handler.py
-drwxrwxrwx   0        0        0        0 2023-06-10 07:29:41.824985 Shark sac Korean editor-1.2.1/modkr/edits/
--rw-rw-rw-   0        0        0       67 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.2.1/modkr/edits/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 07:29:41.831269 Shark sac Korean editor-1.2.1/modkr/edits/basic/
--rw-rw-rw-   0        0        0      122 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.2.1/modkr/edits/basic/__init__.py
--rw-rw-rw-   0        0        0     9125 2023-06-10 05:12:02.000000 Shark sac Korean editor-1.2.1/modkr/edits/basic/basic_items.py
--rw-rw-rw-   0        0        0     1490 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.2.1/modkr/edits/basic/catfruit.py
--rw-rw-rw-   0        0        0     2017 2023-06-10 05:17:14.000000 Shark sac Korean editor-1.2.1/modkr/edits/basic/catseyes.py
--rw-rw-rw-   0        0        0     1702 2023-06-10 05:47:34.000000 Shark sac Korean editor-1.2.1/modkr/edits/basic/ototo_base_mats.py
--rw-rw-rw-   0        0        0     4136 2023-06-10 05:30:23.000000 Shark sac Korean editor-1.2.1/modkr/edits/basic/talent_orbs.py
--rw-rw-rw-   0        0        0    16762 2023-06-10 05:34:36.000000 Shark sac Korean editor-1.2.1/modkr/edits/basic/talent_orbs_new.py
-drwxrwxrwx   0        0        0        0 2023-06-10 07:29:41.839675 Shark sac Korean editor-1.2.1/modkr/edits/cats/
--rw-rw-rw-   0        0        0      179 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.2.1/modkr/edits/cats/__init__.py
--rw-rw-rw-   0        0        0     8978 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.2.1/modkr/edits/cats/cat_helper.py
--rw-rw-rw-   0        0        0    11473 2023-06-10 04:48:37.000000 Shark sac Korean editor-1.2.1/modkr/edits/cats/cat_id_selector.py
--rw-rw-rw-   0        0        0     3378 2023-06-10 04:40:29.000000 Shark sac Korean editor-1.2.1/modkr/edits/cats/chara_drop.py
--rw-rw-rw-   0        0        0     1081 2023-06-10 04:41:38.000000 Shark sac Korean editor-1.2.1/modkr/edits/cats/clear_cat_guide.py
--rw-rw-rw-   0        0        0     2882 2023-06-10 04:42:21.000000 Shark sac Korean editor-1.2.1/modkr/edits/cats/evolve_cats.py
--rw-rw-rw-   0        0        0     1268 2023-06-10 04:42:37.000000 Shark sac Korean editor-1.2.1/modkr/edits/cats/get_remove_cats.py
--rw-rw-rw-   0        0        0     8010 2023-06-10 04:43:44.000000 Shark sac Korean editor-1.2.1/modkr/edits/cats/talents.py
--rw-rw-rw-   0        0        0     2114 2023-06-10 07:13:45.000000 Shark sac Korean editor-1.2.1/modkr/edits/cats/upgrade_blue.py
--rw-rw-rw-   0        0        0     4660 2023-06-10 07:15:32.000000 Shark sac Korean editor-1.2.1/modkr/edits/cats/upgrade_cats.py
-drwxrwxrwx   0        0        0        0 2023-06-10 07:29:41.844203 Shark sac Korean editor-1.2.1/modkr/edits/gamototo/
--rw-rw-rw-   0        0        0       66 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.2.1/modkr/edits/gamototo/__init__.py
--rw-rw-rw-   0        0        0      333 2023-06-10 05:39:01.000000 Shark sac Korean editor-1.2.1/modkr/edits/gamototo/fix_gamatoto.py
--rw-rw-rw-   0        0        0     2878 2023-06-10 05:42:37.000000 Shark sac Korean editor-1.2.1/modkr/edits/gamototo/gamatoto_xp.py
--rw-rw-rw-   0        0        0     3430 2023-06-10 05:43:35.000000 Shark sac Korean editor-1.2.1/modkr/edits/gamototo/helpers.py
--rw-rw-rw-   0        0        0     7458 2023-06-10 05:58:12.000000 Shark sac Korean editor-1.2.1/modkr/edits/gamototo/ototo_cat_cannon.py
-drwxrwxrwx   0        0        0        0 2023-06-10 07:29:41.858925 Shark sac Korean editor-1.2.1/modkr/edits/levels/
--rw-rw-rw-   0        0        0      313 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.2.1/modkr/edits/levels/__init__.py
--rw-rw-rw-   0        0        0     1060 2023-06-10 06:06:45.000000 Shark sac Korean editor-1.2.1/modkr/edits/levels/aku.py
--rw-rw-rw-   0        0        0      516 2023-06-10 06:06:59.000000 Shark sac Korean editor-1.2.1/modkr/edits/levels/allow_filibuster_clearing.py
--rw-rw-rw-   0        0        0      815 2023-06-10 06:08:07.000000 Shark sac Korean editor-1.2.1/modkr/edits/levels/behemoth_culling.py
--rw-rw-rw-   0        0        0      644 2023-06-10 06:08:16.000000 Shark sac Korean editor-1.2.1/modkr/edits/levels/clear_tutorial.py
--rw-rw-rw-   0        0        0     1146 2023-06-10 06:08:52.000000 Shark sac Korean editor-1.2.1/modkr/edits/levels/enigma_stages.py
--rw-rw-rw-   0        0        0     6453 2023-06-10 07:03:14.000000 Shark sac Korean editor-1.2.1/modkr/edits/levels/event_stages.py
--rw-rw-rw-   0        0        0     1873 2023-06-10 06:14:29.000000 Shark sac Korean editor-1.2.1/modkr/edits/levels/gauntlet.py
--rw-rw-rw-   0        0        0     1058 2023-06-10 06:14:57.000000 Shark sac Korean editor-1.2.1/modkr/edits/levels/itf_timed_scores.py
--rw-rw-rw-   0        0        0     1481 2023-06-10 06:16:15.000000 Shark sac Korean editor-1.2.1/modkr/edits/levels/legend_quest.py
--rw-rw-rw-   0        0        0     4372 2023-06-10 06:18:36.000000 Shark sac Korean editor-1.2.1/modkr/edits/levels/main_story.py
--rw-rw-rw-   0        0        0     2350 2023-06-10 06:20:35.000000 Shark sac Korean editor-1.2.1/modkr/edits/levels/outbreaks.py
--rw-rw-rw-   0        0        0     3076 2023-06-10 07:10:43.000000 Shark sac Korean editor-1.2.1/modkr/edits/levels/story_level_id_selector.py
--rw-rw-rw-   0        0        0     1212 2023-06-10 06:25:23.000000 Shark sac Korean editor-1.2.1/modkr/edits/levels/towers.py
--rw-rw-rw-   0        0        0     8550 2023-06-10 06:32:15.000000 Shark sac Korean editor-1.2.1/modkr/edits/levels/treasures.py
--rw-rw-rw-   0        0        0     1081 2023-06-10 06:33:11.000000 Shark sac Korean editor-1.2.1/modkr/edits/levels/uncanny.py
--rw-rw-rw-   0        0        0      801 2023-06-10 06:33:22.000000 Shark sac Korean editor-1.2.1/modkr/edits/levels/unlock_aku_realm.py
-drwxrwxrwx   0        0        0        0 2023-06-10 07:29:41.870928 Shark sac Korean editor-1.2.1/modkr/edits/other/
--rw-rw-rw-   0        0        0      276 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.2.1/modkr/edits/other/__init__.py
--rw-rw-rw-   0        0        0     3940 2023-06-10 06:36:04.000000 Shark sac Korean editor-1.2.1/modkr/edits/other/cat_shrine.py
--rw-rw-rw-   0        0        0     1141 2023-06-10 06:36:40.000000 Shark sac Korean editor-1.2.1/modkr/edits/other/claim_user_rank_rewards.py
--rw-rw-rw-   0        0        0     1058 2023-06-10 06:37:11.000000 Shark sac Korean editor-1.2.1/modkr/edits/other/create_new_account.py
--rw-rw-rw-   0        0        0     2150 2023-06-10 06:38:29.000000 Shark sac Korean editor-1.2.1/modkr/edits/other/fix_elsewhere.py
--rw-rw-rw-   0        0        0      705 2023-06-10 06:40:04.000000 Shark sac Korean editor-1.2.1/modkr/edits/other/fix_time_issues.py
--rw-rw-rw-   0        0        0     3470 2023-06-10 06:41:27.000000 Shark sac Korean editor-1.2.1/modkr/edits/other/get_gold_pass.py
--rw-rw-rw-   0        0        0     7233 2023-06-10 06:43:47.000000 Shark sac Korean editor-1.2.1/modkr/edits/other/meow_medals.py
--rw-rw-rw-   0        0        0     4416 2023-06-10 06:45:55.000000 Shark sac Korean editor-1.2.1/modkr/edits/other/missions.py
--rw-rw-rw-   0        0        0      985 2023-06-10 06:46:36.000000 Shark sac Korean editor-1.2.1/modkr/edits/other/play_time.py
--rw-rw-rw-   0        0        0     4612 2023-06-10 06:47:06.000000 Shark sac Korean editor-1.2.1/modkr/edits/other/scheme_item.py
--rw-rw-rw-   0        0        0     1645 2023-06-10 06:47:33.000000 Shark sac Korean editor-1.2.1/modkr/edits/other/trade_progress.py
--rw-rw-rw-   0        0        0     1436 2023-06-10 06:48:09.000000 Shark sac Korean editor-1.2.1/modkr/edits/other/unlock_enemy_guide.py
--rw-rw-rw-   0        0        0      356 2023-06-10 06:48:20.000000 Shark sac Korean editor-1.2.1/modkr/edits/other/unlock_equip_menu.py
-drwxrwxrwx   0        0        0        0 2023-06-10 07:29:41.876988 Shark sac Korean editor-1.2.1/modkr/edits/save_management/
--rw-rw-rw-   0        0        0       56 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.2.1/modkr/edits/save_management/__init__.py
--rw-rw-rw-   0        0        0     1331 2023-06-10 06:48:57.000000 Shark sac Korean editor-1.2.1/modkr/edits/save_management/convert.py
--rw-rw-rw-   0        0        0     2718 2023-06-10 06:49:37.000000 Shark sac Korean editor-1.2.1/modkr/edits/save_management/load.py
--rw-rw-rw-   0        0        0      661 2023-06-10 06:49:54.000000 Shark sac Korean editor-1.2.1/modkr/edits/save_management/other.py
--rw-rw-rw-   0        0        0     2073 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.2.1/modkr/edits/save_management/save.py
--rw-rw-rw-   0        0        0     2208 2023-06-10 06:50:35.000000 Shark sac Korean editor-1.2.1/modkr/edits/save_management/server_upload.py
--rw-rw-rw-   0        0        0    13946 2023-06-10 05:47:12.000000 Shark sac Korean editor-1.2.1/modkr/feature_handler.py
--rw-rw-rw-   0        0        0     4841 2023-06-10 05:56:27.000000 Shark sac Korean editor-1.2.1/modkr/game_data_getter.py
--rw-rw-rw-   0        0        0    24350 2023-06-10 07:19:14.000000 Shark sac Korean editor-1.2.1/modkr/helper.py
--rw-rw-rw-   0        0        0     7470 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.2.1/modkr/item.py
--rw-rw-rw-   0        0        0     3505 2023-06-10 04:57:01.000000 Shark sac Korean editor-1.2.1/modkr/locale_handler.py
--rw-rw-rw-   0        0        0     1269 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.2.1/modkr/managed_item.py
--rw-rw-rw-   0        0        0    72179 2023-06-10 06:58:03.000000 Shark sac Korean editor-1.2.1/modkr/parse_save.py
--rw-rw-rw-   0        0        0     1301 2023-06-10 06:58:57.000000 Shark sac Korean editor-1.2.1/modkr/patcher.py
--rw-rw-rw-   0        0        0     2415 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.2.1/modkr/root_handler.py
--rw-rw-rw-   0        0        0    55884 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.2.1/modkr/serialise_save.py
--rw-rw-rw-   0        0        0    26654 2023-06-10 06:54:07.000000 Shark sac Korean editor-1.2.1/modkr/server_handler.py
--rw-rw-rw-   0        0        0     3717 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.2.1/modkr/tracker.py
--rw-rw-rw-   0        0        0     3640 2023-06-10 07:00:23.000000 Shark sac Korean editor-1.2.1/modkr/updater.py
--rw-rw-rw-   0        0        0     4515 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.2.1/modkr/user_info.py
--rw-rw-rw-   0        0        0     8297 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.2.1/modkr/user_input_handler.py
--rw-rw-rw-   0        0        0       42 2023-06-10 07:29:41.877987 Shark sac Korean editor-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0      984 2023-06-10 07:28:54.000000 Shark sac Korean editor-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 13:38:56.540459 Shark sac Korean editor-1.2.5/
+-rw-rw-rw-   0        0        0      731 2023-06-10 13:38:56.540459 Shark sac Korean editor-1.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2023-04-27 07:59:41.000000 Shark sac Korean editor-1.2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-10 13:38:56.473130 Shark sac Korean editor-1.2.5/Shark_sac_Korean_editor.egg-info/
+-rw-rw-rw-   0        0        0      731 2023-06-10 13:38:56.000000 Shark sac Korean editor-1.2.5/Shark_sac_Korean_editor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2708 2023-06-10 13:38:56.000000 Shark sac Korean editor-1.2.5/Shark_sac_Korean_editor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 13:38:56.000000 Shark sac Korean editor-1.2.5/Shark_sac_Korean_editor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-10 13:38:56.000000 Shark sac Korean editor-1.2.5/Shark_sac_Korean_editor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-10 13:38:56.489414 Shark sac Korean editor-1.2.5/modkr/
+-rw-rw-rw-   0        0        0      283 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.2.5/modkr/__init__.py
+-rw-rw-rw-   0        0        0     9136 2023-06-10 03:58:09.000000 Shark sac Korean editor-1.2.5/modkr/__main__.py
+-rw-rw-rw-   0        0        0    10151 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.2.5/modkr/adb_handler.py
+-rw-rw-rw-   0        0        0    13745 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.2.5/modkr/config_manager.py
+-rw-rw-rw-   0        0        0     1510 2023-06-10 06:54:54.000000 Shark sac Korean editor-1.2.5/modkr/csv_handler.py
+drwxrwxrwx   0        0        0        0 2023-06-10 13:38:56.490902 Shark sac Korean editor-1.2.5/modkr/edits/
+-rw-rw-rw-   0        0        0       67 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.2.5/modkr/edits/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 13:38:56.495901 Shark sac Korean editor-1.2.5/modkr/edits/basic/
+-rw-rw-rw-   0        0        0      122 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.2.5/modkr/edits/basic/__init__.py
+-rw-rw-rw-   0        0        0     9125 2023-06-10 05:12:02.000000 Shark sac Korean editor-1.2.5/modkr/edits/basic/basic_items.py
+-rw-rw-rw-   0        0        0     1490 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.2.5/modkr/edits/basic/catfruit.py
+-rw-rw-rw-   0        0        0     2017 2023-06-10 05:17:14.000000 Shark sac Korean editor-1.2.5/modkr/edits/basic/catseyes.py
+-rw-rw-rw-   0        0        0     1702 2023-06-10 05:47:34.000000 Shark sac Korean editor-1.2.5/modkr/edits/basic/ototo_base_mats.py
+-rw-rw-rw-   0        0        0     4136 2023-06-10 05:30:23.000000 Shark sac Korean editor-1.2.5/modkr/edits/basic/talent_orbs.py
+-rw-rw-rw-   0        0        0    16762 2023-06-10 05:34:36.000000 Shark sac Korean editor-1.2.5/modkr/edits/basic/talent_orbs_new.py
+drwxrwxrwx   0        0        0        0 2023-06-10 13:38:56.504871 Shark sac Korean editor-1.2.5/modkr/edits/cats/
+-rw-rw-rw-   0        0        0      179 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.2.5/modkr/edits/cats/__init__.py
+-rw-rw-rw-   0        0        0     8978 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.2.5/modkr/edits/cats/cat_helper.py
+-rw-rw-rw-   0        0        0    11473 2023-06-10 04:48:37.000000 Shark sac Korean editor-1.2.5/modkr/edits/cats/cat_id_selector.py
+-rw-rw-rw-   0        0        0     3378 2023-06-10 04:40:29.000000 Shark sac Korean editor-1.2.5/modkr/edits/cats/chara_drop.py
+-rw-rw-rw-   0        0        0     1081 2023-06-10 04:41:38.000000 Shark sac Korean editor-1.2.5/modkr/edits/cats/clear_cat_guide.py
+-rw-rw-rw-   0        0        0     2882 2023-06-10 04:42:21.000000 Shark sac Korean editor-1.2.5/modkr/edits/cats/evolve_cats.py
+-rw-rw-rw-   0        0        0     1268 2023-06-10 04:42:37.000000 Shark sac Korean editor-1.2.5/modkr/edits/cats/get_remove_cats.py
+-rw-rw-rw-   0        0        0     8010 2023-06-10 04:43:44.000000 Shark sac Korean editor-1.2.5/modkr/edits/cats/talents.py
+-rw-rw-rw-   0        0        0     2114 2023-06-10 07:13:45.000000 Shark sac Korean editor-1.2.5/modkr/edits/cats/upgrade_blue.py
+-rw-rw-rw-   0        0        0     4660 2023-06-10 07:15:32.000000 Shark sac Korean editor-1.2.5/modkr/edits/cats/upgrade_cats.py
+drwxrwxrwx   0        0        0        0 2023-06-10 13:38:56.509824 Shark sac Korean editor-1.2.5/modkr/edits/gamototo/
+-rw-rw-rw-   0        0        0       66 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.2.5/modkr/edits/gamototo/__init__.py
+-rw-rw-rw-   0        0        0      333 2023-06-10 05:39:01.000000 Shark sac Korean editor-1.2.5/modkr/edits/gamototo/fix_gamatoto.py
+-rw-rw-rw-   0        0        0     2878 2023-06-10 05:42:37.000000 Shark sac Korean editor-1.2.5/modkr/edits/gamototo/gamatoto_xp.py
+-rw-rw-rw-   0        0        0     3430 2023-06-10 05:43:35.000000 Shark sac Korean editor-1.2.5/modkr/edits/gamototo/helpers.py
+-rw-rw-rw-   0        0        0     7458 2023-06-10 13:31:26.000000 Shark sac Korean editor-1.2.5/modkr/edits/gamototo/ototo_cat_cannon.py
+drwxrwxrwx   0        0        0        0 2023-06-10 13:38:56.522619 Shark sac Korean editor-1.2.5/modkr/edits/levels/
+-rw-rw-rw-   0        0        0      313 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.2.5/modkr/edits/levels/__init__.py
+-rw-rw-rw-   0        0        0     1060 2023-06-10 06:06:45.000000 Shark sac Korean editor-1.2.5/modkr/edits/levels/aku.py
+-rw-rw-rw-   0        0        0      516 2023-06-10 06:06:59.000000 Shark sac Korean editor-1.2.5/modkr/edits/levels/allow_filibuster_clearing.py
+-rw-rw-rw-   0        0        0      815 2023-06-10 06:08:07.000000 Shark sac Korean editor-1.2.5/modkr/edits/levels/behemoth_culling.py
+-rw-rw-rw-   0        0        0      644 2023-06-10 06:08:16.000000 Shark sac Korean editor-1.2.5/modkr/edits/levels/clear_tutorial.py
+-rw-rw-rw-   0        0        0     1146 2023-06-10 06:08:52.000000 Shark sac Korean editor-1.2.5/modkr/edits/levels/enigma_stages.py
+-rw-rw-rw-   0        0        0     6453 2023-06-10 07:03:14.000000 Shark sac Korean editor-1.2.5/modkr/edits/levels/event_stages.py
+-rw-rw-rw-   0        0        0     1873 2023-06-10 06:14:29.000000 Shark sac Korean editor-1.2.5/modkr/edits/levels/gauntlet.py
+-rw-rw-rw-   0        0        0     1058 2023-06-10 06:14:57.000000 Shark sac Korean editor-1.2.5/modkr/edits/levels/itf_timed_scores.py
+-rw-rw-rw-   0        0        0     1481 2023-06-10 06:16:15.000000 Shark sac Korean editor-1.2.5/modkr/edits/levels/legend_quest.py
+-rw-rw-rw-   0        0        0     4372 2023-06-10 06:18:36.000000 Shark sac Korean editor-1.2.5/modkr/edits/levels/main_story.py
+-rw-rw-rw-   0        0        0     2350 2023-06-10 06:20:35.000000 Shark sac Korean editor-1.2.5/modkr/edits/levels/outbreaks.py
+-rw-rw-rw-   0        0        0     3076 2023-06-10 07:10:43.000000 Shark sac Korean editor-1.2.5/modkr/edits/levels/story_level_id_selector.py
+-rw-rw-rw-   0        0        0     1212 2023-06-10 06:25:23.000000 Shark sac Korean editor-1.2.5/modkr/edits/levels/towers.py
+-rw-rw-rw-   0        0        0     8550 2023-06-10 06:32:15.000000 Shark sac Korean editor-1.2.5/modkr/edits/levels/treasures.py
+-rw-rw-rw-   0        0        0     1081 2023-06-10 06:33:11.000000 Shark sac Korean editor-1.2.5/modkr/edits/levels/uncanny.py
+-rw-rw-rw-   0        0        0      801 2023-06-10 06:33:22.000000 Shark sac Korean editor-1.2.5/modkr/edits/levels/unlock_aku_realm.py
+drwxrwxrwx   0        0        0        0 2023-06-10 13:38:56.533678 Shark sac Korean editor-1.2.5/modkr/edits/other/
+-rw-rw-rw-   0        0        0      276 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.2.5/modkr/edits/other/__init__.py
+-rw-rw-rw-   0        0        0     3940 2023-06-10 06:36:04.000000 Shark sac Korean editor-1.2.5/modkr/edits/other/cat_shrine.py
+-rw-rw-rw-   0        0        0     1141 2023-06-10 06:36:40.000000 Shark sac Korean editor-1.2.5/modkr/edits/other/claim_user_rank_rewards.py
+-rw-rw-rw-   0        0        0     1058 2023-06-10 06:37:11.000000 Shark sac Korean editor-1.2.5/modkr/edits/other/create_new_account.py
+-rw-rw-rw-   0        0        0     2150 2023-06-10 06:38:29.000000 Shark sac Korean editor-1.2.5/modkr/edits/other/fix_elsewhere.py
+-rw-rw-rw-   0        0        0      705 2023-06-10 06:40:04.000000 Shark sac Korean editor-1.2.5/modkr/edits/other/fix_time_issues.py
+-rw-rw-rw-   0        0        0     3470 2023-06-10 06:41:27.000000 Shark sac Korean editor-1.2.5/modkr/edits/other/get_gold_pass.py
+-rw-rw-rw-   0        0        0     7233 2023-06-10 06:43:47.000000 Shark sac Korean editor-1.2.5/modkr/edits/other/meow_medals.py
+-rw-rw-rw-   0        0        0     4416 2023-06-10 06:45:55.000000 Shark sac Korean editor-1.2.5/modkr/edits/other/missions.py
+-rw-rw-rw-   0        0        0      985 2023-06-10 06:46:36.000000 Shark sac Korean editor-1.2.5/modkr/edits/other/play_time.py
+-rw-rw-rw-   0        0        0     4612 2023-06-10 06:47:06.000000 Shark sac Korean editor-1.2.5/modkr/edits/other/scheme_item.py
+-rw-rw-rw-   0        0        0     1645 2023-06-10 06:47:33.000000 Shark sac Korean editor-1.2.5/modkr/edits/other/trade_progress.py
+-rw-rw-rw-   0        0        0     1436 2023-06-10 06:48:09.000000 Shark sac Korean editor-1.2.5/modkr/edits/other/unlock_enemy_guide.py
+-rw-rw-rw-   0        0        0      356 2023-06-10 06:48:20.000000 Shark sac Korean editor-1.2.5/modkr/edits/other/unlock_equip_menu.py
+drwxrwxrwx   0        0        0        0 2023-06-10 13:38:56.539457 Shark sac Korean editor-1.2.5/modkr/edits/save_management/
+-rw-rw-rw-   0        0        0       56 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.2.5/modkr/edits/save_management/__init__.py
+-rw-rw-rw-   0        0        0     1331 2023-06-10 06:48:57.000000 Shark sac Korean editor-1.2.5/modkr/edits/save_management/convert.py
+-rw-rw-rw-   0        0        0     2718 2023-06-10 06:49:37.000000 Shark sac Korean editor-1.2.5/modkr/edits/save_management/load.py
+-rw-rw-rw-   0        0        0      661 2023-06-10 06:49:54.000000 Shark sac Korean editor-1.2.5/modkr/edits/save_management/other.py
+-rw-rw-rw-   0        0        0     2073 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.2.5/modkr/edits/save_management/save.py
+-rw-rw-rw-   0        0        0     2208 2023-06-10 06:50:35.000000 Shark sac Korean editor-1.2.5/modkr/edits/save_management/server_upload.py
+-rw-rw-rw-   0        0        0    13946 2023-06-10 05:47:12.000000 Shark sac Korean editor-1.2.5/modkr/feature_handler.py
+-rw-rw-rw-   0        0        0     4841 2023-06-10 05:56:27.000000 Shark sac Korean editor-1.2.5/modkr/game_data_getter.py
+-rw-rw-rw-   0        0        0    24350 2023-06-10 07:19:14.000000 Shark sac Korean editor-1.2.5/modkr/helper.py
+-rw-rw-rw-   0        0        0     7470 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.2.5/modkr/item.py
+-rw-rw-rw-   0        0        0     3505 2023-06-10 04:57:01.000000 Shark sac Korean editor-1.2.5/modkr/locale_handler.py
+-rw-rw-rw-   0        0        0     1269 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.2.5/modkr/managed_item.py
+-rw-rw-rw-   0        0        0    72179 2023-06-10 06:58:03.000000 Shark sac Korean editor-1.2.5/modkr/parse_save.py
+-rw-rw-rw-   0        0        0     1301 2023-06-10 06:58:57.000000 Shark sac Korean editor-1.2.5/modkr/patcher.py
+-rw-rw-rw-   0        0        0     2415 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.2.5/modkr/root_handler.py
+-rw-rw-rw-   0        0        0    55884 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.2.5/modkr/serialise_save.py
+-rw-rw-rw-   0        0        0    26654 2023-06-10 06:54:07.000000 Shark sac Korean editor-1.2.5/modkr/server_handler.py
+-rw-rw-rw-   0        0        0     3717 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.2.5/modkr/tracker.py
+-rw-rw-rw-   0        0        0     3640 2023-06-10 07:00:23.000000 Shark sac Korean editor-1.2.5/modkr/updater.py
+-rw-rw-rw-   0        0        0     4515 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.2.5/modkr/user_info.py
+-rw-rw-rw-   0        0        0     8297 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.2.5/modkr/user_input_handler.py
+-rw-rw-rw-   0        0        0       42 2023-06-10 13:38:56.540459 Shark sac Korean editor-1.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      984 2023-06-10 13:38:13.000000 Shark sac Korean editor-1.2.5/setup.py
```

### Comparing `Shark sac Korean editor-1.2.1/PKG-INFO` & `Shark sac Korean editor-1.2.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Shark sac Korean editor
-Version: 1.2.1
+Version: 1.2.5
 Summary: 냥코에디터 한글화
 Home-page: https://github.com/sharkwodm/koreditor
 Author: 익명
 Author-email: 
 License: MIT
 Keywords: python,template
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Shark sac Korean editor-1.2.1/Shark_sac_Korean_editor.egg-info/PKG-INFO` & `Shark sac Korean editor-1.2.5/Shark_sac_Korean_editor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Shark-sac-Korean-editor
-Version: 1.2.1
+Version: 1.2.5
 Summary: 냥코에디터 한글화
 Home-page: https://github.com/sharkwodm/koreditor
 Author: 익명
 Author-email: 
 License: MIT
 Keywords: python,template
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Shark sac Korean editor-1.2.1/Shark_sac_Korean_editor.egg-info/SOURCES.txt` & `Shark sac Korean editor-1.2.5/Shark_sac_Korean_editor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/__main__.py` & `Shark sac Korean editor-1.2.5/modkr/__main__.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/adb_handler.py` & `Shark sac Korean editor-1.2.5/modkr/adb_handler.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/config_manager.py` & `Shark sac Korean editor-1.2.5/modkr/config_manager.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/csv_handler.py` & `Shark sac Korean editor-1.2.5/modkr/csv_handler.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/basic/basic_items.py` & `Shark sac Korean editor-1.2.5/modkr/edits/basic/basic_items.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/basic/catfruit.py` & `Shark sac Korean editor-1.2.5/modkr/edits/basic/catfruit.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/basic/catseyes.py` & `Shark sac Korean editor-1.2.5/modkr/edits/basic/catseyes.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/basic/ototo_base_mats.py` & `Shark sac Korean editor-1.2.5/modkr/edits/basic/ototo_base_mats.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/basic/talent_orbs.py` & `Shark sac Korean editor-1.2.5/modkr/edits/basic/talent_orbs.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/basic/talent_orbs_new.py` & `Shark sac Korean editor-1.2.5/modkr/edits/basic/talent_orbs_new.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/cats/cat_helper.py` & `Shark sac Korean editor-1.2.5/modkr/edits/cats/cat_helper.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/cats/cat_id_selector.py` & `Shark sac Korean editor-1.2.5/modkr/edits/cats/cat_id_selector.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/cats/chara_drop.py` & `Shark sac Korean editor-1.2.5/modkr/edits/cats/chara_drop.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/cats/clear_cat_guide.py` & `Shark sac Korean editor-1.2.5/modkr/edits/cats/clear_cat_guide.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/cats/evolve_cats.py` & `Shark sac Korean editor-1.2.5/modkr/edits/cats/evolve_cats.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/cats/get_remove_cats.py` & `Shark sac Korean editor-1.2.5/modkr/edits/cats/get_remove_cats.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/cats/talents.py` & `Shark sac Korean editor-1.2.5/modkr/edits/cats/talents.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/cats/upgrade_blue.py` & `Shark sac Korean editor-1.2.5/modkr/edits/cats/upgrade_blue.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/cats/upgrade_cats.py` & `Shark sac Korean editor-1.2.5/modkr/edits/cats/upgrade_cats.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/gamototo/gamatoto_xp.py` & `Shark sac Korean editor-1.2.5/modkr/edits/gamototo/gamatoto_xp.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/gamototo/helpers.py` & `Shark sac Korean editor-1.2.5/modkr/edits/gamototo/helpers.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/gamototo/ototo_cat_cannon.py` & `Shark sac Korean editor-1.2.5/modkr/edits/gamototo/ototo_cat_cannon.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,19 +44,19 @@
         elif max_val > maxes[cannon_id][part]:
             maxes[cannon_id][part] = max_val
     return maxes
 
 
 def get_part_id_from_str(part: str) -> int:
     """Get the part id from the string"""
-    if part == "효과":
+    if part == "effect":
         return 0
-    if part == "기반":
+    if part == "foundation":
         return 1
-    if part == "스타일":
+    if part == "style":
         return 2
     return 0
 
 
 def get_max(
     part: str, cannon_id: int, cannon_maxes: dict[int, dict[int, int]]
 ) -> Optional[int]:
```

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/levels/aku.py` & `Shark sac Korean editor-1.2.5/modkr/edits/levels/aku.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/levels/allow_filibuster_clearing.py` & `Shark sac Korean editor-1.2.5/modkr/edits/levels/allow_filibuster_clearing.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/levels/behemoth_culling.py` & `Shark sac Korean editor-1.2.5/modkr/edits/levels/behemoth_culling.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/levels/clear_tutorial.py` & `Shark sac Korean editor-1.2.5/modkr/edits/levels/clear_tutorial.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/levels/enigma_stages.py` & `Shark sac Korean editor-1.2.5/modkr/edits/levels/enigma_stages.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/levels/event_stages.py` & `Shark sac Korean editor-1.2.5/modkr/edits/levels/event_stages.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/levels/gauntlet.py` & `Shark sac Korean editor-1.2.5/modkr/edits/levels/gauntlet.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/levels/itf_timed_scores.py` & `Shark sac Korean editor-1.2.5/modkr/edits/levels/itf_timed_scores.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/levels/legend_quest.py` & `Shark sac Korean editor-1.2.5/modkr/edits/levels/legend_quest.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/levels/main_story.py` & `Shark sac Korean editor-1.2.5/modkr/edits/levels/main_story.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/levels/outbreaks.py` & `Shark sac Korean editor-1.2.5/modkr/edits/levels/outbreaks.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/levels/story_level_id_selector.py` & `Shark sac Korean editor-1.2.5/modkr/edits/levels/story_level_id_selector.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/levels/towers.py` & `Shark sac Korean editor-1.2.5/modkr/edits/levels/towers.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/levels/treasures.py` & `Shark sac Korean editor-1.2.5/modkr/edits/levels/treasures.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/levels/uncanny.py` & `Shark sac Korean editor-1.2.5/modkr/edits/levels/uncanny.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/levels/unlock_aku_realm.py` & `Shark sac Korean editor-1.2.5/modkr/edits/levels/unlock_aku_realm.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/other/cat_shrine.py` & `Shark sac Korean editor-1.2.5/modkr/edits/other/cat_shrine.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/other/claim_user_rank_rewards.py` & `Shark sac Korean editor-1.2.5/modkr/edits/other/claim_user_rank_rewards.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/other/create_new_account.py` & `Shark sac Korean editor-1.2.5/modkr/edits/other/create_new_account.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/other/fix_elsewhere.py` & `Shark sac Korean editor-1.2.5/modkr/edits/other/fix_elsewhere.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/other/fix_time_issues.py` & `Shark sac Korean editor-1.2.5/modkr/edits/other/fix_time_issues.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/other/get_gold_pass.py` & `Shark sac Korean editor-1.2.5/modkr/edits/other/get_gold_pass.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/other/meow_medals.py` & `Shark sac Korean editor-1.2.5/modkr/edits/other/meow_medals.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/other/missions.py` & `Shark sac Korean editor-1.2.5/modkr/edits/other/missions.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/other/play_time.py` & `Shark sac Korean editor-1.2.5/modkr/edits/other/play_time.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/other/scheme_item.py` & `Shark sac Korean editor-1.2.5/modkr/edits/other/scheme_item.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/other/trade_progress.py` & `Shark sac Korean editor-1.2.5/modkr/edits/other/trade_progress.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/other/unlock_enemy_guide.py` & `Shark sac Korean editor-1.2.5/modkr/edits/other/unlock_enemy_guide.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/save_management/convert.py` & `Shark sac Korean editor-1.2.5/modkr/edits/save_management/convert.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/save_management/load.py` & `Shark sac Korean editor-1.2.5/modkr/edits/save_management/load.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/save_management/other.py` & `Shark sac Korean editor-1.2.5/modkr/edits/save_management/other.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/save_management/save.py` & `Shark sac Korean editor-1.2.5/modkr/edits/save_management/save.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/edits/save_management/server_upload.py` & `Shark sac Korean editor-1.2.5/modkr/edits/save_management/server_upload.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/feature_handler.py` & `Shark sac Korean editor-1.2.5/modkr/feature_handler.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/game_data_getter.py` & `Shark sac Korean editor-1.2.5/modkr/game_data_getter.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/helper.py` & `Shark sac Korean editor-1.2.5/modkr/helper.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/item.py` & `Shark sac Korean editor-1.2.5/modkr/item.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/locale_handler.py` & `Shark sac Korean editor-1.2.5/modkr/locale_handler.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/managed_item.py` & `Shark sac Korean editor-1.2.5/modkr/managed_item.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/parse_save.py` & `Shark sac Korean editor-1.2.5/modkr/parse_save.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/patcher.py` & `Shark sac Korean editor-1.2.5/modkr/patcher.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/root_handler.py` & `Shark sac Korean editor-1.2.5/modkr/root_handler.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/serialise_save.py` & `Shark sac Korean editor-1.2.5/modkr/serialise_save.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/server_handler.py` & `Shark sac Korean editor-1.2.5/modkr/server_handler.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/tracker.py` & `Shark sac Korean editor-1.2.5/modkr/tracker.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/updater.py` & `Shark sac Korean editor-1.2.5/modkr/updater.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/user_info.py` & `Shark sac Korean editor-1.2.5/modkr/user_info.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/modkr/user_input_handler.py` & `Shark sac Korean editor-1.2.5/modkr/user_input_handler.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.2.1/setup.py` & `Shark sac Korean editor-1.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 basedir = path.abspath(path.dirname(__file__))
 with open(path.join(basedir, 'README.md'), encoding='utf-8') as file:
     long_description = file.read().replace('\r\n', '\n')
 
 setup(
     name='Shark sac Korean editor',
-    version='1.2.1',
+    version='1.2.5',
     description='냥코에디터 한글화',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='익명',
     author_email='',
     url='https://github.com/sharkwodm/koreditor',
     packages=find_packages(exclude=['contrib', 'docs', 'tests']),
```

