# Comparing `tmp/Shark sac Korean editor-1.1.1.tar.gz` & `tmp/Shark sac Korean editor-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Shark sac Korean editor-1.1.1.tar", last modified: Thu Jun  8 13:52:53 2023, max compression
+gzip compressed data, was "Shark sac Korean editor-1.1.2.tar", last modified: Sat Jun 10 07:21:07 2023, max compression
```

## Comparing `Shark sac Korean editor-1.1.1.tar` & `Shark sac Korean editor-1.1.2.tar`

### file list

```diff
@@ -1,97 +1,98 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 13:52:53.407198 Shark sac Korean editor-1.1.1/
--rw-rw-rw-   0        0        0      731 2023-06-08 13:52:53.407198 Shark sac Korean editor-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      198 2023-04-27 07:59:41.000000 Shark sac Korean editor-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 13:52:53.338556 Shark sac Korean editor-1.1.1/Shark_sac_Korean_editor.egg-info/
--rw-rw-rw-   0        0        0      731 2023-06-08 13:52:53.000000 Shark sac Korean editor-1.1.1/Shark_sac_Korean_editor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2689 2023-06-08 13:52:53.000000 Shark sac Korean editor-1.1.1/Shark_sac_Korean_editor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 13:52:53.000000 Shark sac Korean editor-1.1.1/Shark_sac_Korean_editor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-08 13:52:53.000000 Shark sac Korean editor-1.1.1/Shark_sac_Korean_editor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-08 13:52:53.354627 Shark sac Korean editor-1.1.1/modkr/
--rw-rw-rw-   0        0        0      281 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/__init__.py
--rw-rw-rw-   0        0        0     9149 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/__main__.py
--rw-rw-rw-   0        0        0    10240 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/adb_handler.py
--rw-rw-rw-   0        0        0    13764 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/config_manager.py
--rw-rw-rw-   0        0        0     1501 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/csv_handler.py
-drwxrwxrwx   0        0        0        0 2023-06-08 13:52:53.355623 Shark sac Korean editor-1.1.1/modkr/edits/
--rw-rw-rw-   0        0        0       67 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 13:52:53.361501 Shark sac Korean editor-1.1.1/modkr/edits/basic/
--rw-rw-rw-   0        0        0      122 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/basic/__init__.py
--rw-rw-rw-   0        0        0     8976 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/basic/basic_items.py
--rw-rw-rw-   0        0        0     1490 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/basic/catfruit.py
--rw-rw-rw-   0        0        0     1931 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/basic/catseyes.py
--rw-rw-rw-   0        0        0     1647 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/basic/ototo_base_mats.py
--rw-rw-rw-   0        0        0     4041 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/basic/talent_orbs.py
--rw-rw-rw-   0        0        0    16755 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/basic/talent_orbs_new.py
-drwxrwxrwx   0        0        0        0 2023-06-08 13:52:53.370337 Shark sac Korean editor-1.1.1/modkr/edits/cats/
--rw-rw-rw-   0        0        0      179 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/cats/__init__.py
--rw-rw-rw-   0        0        0     8994 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/cats/cat_helper.py
--rw-rw-rw-   0        0        0    11449 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/cats/cat_id_selector.py
--rw-rw-rw-   0        0        0     3262 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/cats/chara_drop.py
--rw-rw-rw-   0        0        0     1083 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/cats/clear_cat_guide.py
--rw-rw-rw-   0        0        0     2883 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/cats/evolve_cats.py
--rw-rw-rw-   0        0        0     1277 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/cats/get_remove_cats.py
--rw-rw-rw-   0        0        0     8065 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/cats/talents.py
--rw-rw-rw-   0        0        0     1900 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/cats/upgrade_blue.py
--rw-rw-rw-   0        0        0     4634 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/cats/upgrade_cats.py
-drwxrwxrwx   0        0        0        0 2023-06-08 13:52:53.373830 Shark sac Korean editor-1.1.1/modkr/edits/gamototo/
--rw-rw-rw-   0        0        0       66 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/gamototo/__init__.py
--rw-rw-rw-   0        0        0      333 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/gamototo/fix_gamatoto.py
--rw-rw-rw-   0        0        0     2835 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/gamototo/gamatoto_xp.py
--rw-rw-rw-   0        0        0     3399 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/gamototo/helpers.py
--rw-rw-rw-   0        0        0     4130 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/gamototo/ototo_cat_cannon.py
-drwxrwxrwx   0        0        0        0 2023-06-08 13:52:53.389190 Shark sac Korean editor-1.1.1/modkr/edits/levels/
--rw-rw-rw-   0        0        0      313 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/levels/__init__.py
--rw-rw-rw-   0        0        0     1057 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/levels/aku.py
--rw-rw-rw-   0        0        0      516 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/levels/allow_filibuster_clearing.py
--rw-rw-rw-   0        0        0      869 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/levels/behemoth_culling.py
--rw-rw-rw-   0        0        0      650 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/levels/clear_tutorial.py
--rw-rw-rw-   0        0        0     1121 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/levels/enigma_stages.py
--rw-rw-rw-   0        0        0     6389 2023-06-08 13:45:09.000000 Shark sac Korean editor-1.1.1/modkr/edits/levels/event_stages.py
--rw-rw-rw-   0        0        0     2062 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/levels/gauntlet.py
--rw-rw-rw-   0        0        0     1056 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/levels/itf_timed_scores.py
--rw-rw-rw-   0        0        0     1481 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/levels/legend_quest.py
--rw-rw-rw-   0        0        0     4451 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/levels/main_story.py
--rw-rw-rw-   0        0        0     2361 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/levels/outbreaks.py
--rw-rw-rw-   0        0        0     3106 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/levels/story_level_id_selector.py
--rw-rw-rw-   0        0        0     1227 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/levels/towers.py
--rw-rw-rw-   0        0        0     8576 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/levels/treasures.py
--rw-rw-rw-   0        0        0     1082 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/levels/uncanny.py
--rw-rw-rw-   0        0        0      802 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/levels/unlock_aku_realm.py
-drwxrwxrwx   0        0        0        0 2023-06-08 13:52:53.401219 Shark sac Korean editor-1.1.1/modkr/edits/other/
--rw-rw-rw-   0        0        0      276 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/other/__init__.py
--rw-rw-rw-   0        0        0     3913 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/other/cat_shrine.py
--rw-rw-rw-   0        0        0     1124 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/other/claim_user_rank_rewards.py
--rw-rw-rw-   0        0        0     1054 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/other/create_new_account.py
--rw-rw-rw-   0        0        0     2236 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/other/fix_elsewhere.py
--rw-rw-rw-   0        0        0      698 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/other/fix_time_issues.py
--rw-rw-rw-   0        0        0     3510 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/other/get_gold_pass.py
--rw-rw-rw-   0        0        0     7142 2023-06-08 13:49:33.000000 Shark sac Korean editor-1.1.1/modkr/edits/other/meow_medals.py
--rw-rw-rw-   0        0        0     4384 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/other/missions.py
--rw-rw-rw-   0        0        0     1016 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/other/play_time.py
--rw-rw-rw-   0        0        0     4568 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/other/scheme_item.py
--rw-rw-rw-   0        0        0     1657 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/other/trade_progress.py
--rw-rw-rw-   0        0        0     1426 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/other/unlock_enemy_guide.py
--rw-rw-rw-   0        0        0      356 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/other/unlock_equip_menu.py
-drwxrwxrwx   0        0        0        0 2023-06-08 13:52:53.406199 Shark sac Korean editor-1.1.1/modkr/edits/save_management/
--rw-rw-rw-   0        0        0       56 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/save_management/__init__.py
--rw-rw-rw-   0        0        0     1308 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/save_management/convert.py
--rw-rw-rw-   0        0        0     2795 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/save_management/load.py
--rw-rw-rw-   0        0        0      661 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/save_management/other.py
--rw-rw-rw-   0        0        0     2049 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/save_management/save.py
--rw-rw-rw-   0        0        0     1906 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/save_management/server_upload.py
--rw-rw-rw-   0        0        0    13855 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/feature_handler.py
--rw-rw-rw-   0        0        0     6664 2023-06-08 13:50:04.000000 Shark sac Korean editor-1.1.1/modkr/game_data_getter.py
--rw-rw-rw-   0        0        0    23001 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/helper.py
--rw-rw-rw-   0        0        0     7075 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/item.py
--rw-rw-rw-   0        0        0     3505 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/locale_handler.py
--rw-rw-rw-   0        0        0     1269 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/managed_item.py
--rw-rw-rw-   0        0        0    66980 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/parse_save.py
--rw-rw-rw-   0        0        0     1301 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/patcher.py
--rw-rw-rw-   0        0        0     2450 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/root_handler.py
--rw-rw-rw-   0        0        0    53823 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/serialise_save.py
--rw-rw-rw-   0        0        0    25211 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/server_handler.py
--rw-rw-rw-   0        0        0     3717 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/tracker.py
--rw-rw-rw-   0        0        0     3544 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/updater.py
--rw-rw-rw-   0        0        0     8297 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/user_input_handler.py
--rw-rw-rw-   0        0        0       42 2023-06-08 13:52:53.407198 Shark sac Korean editor-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      984 2023-06-08 13:51:19.000000 Shark sac Korean editor-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 07:21:07.499626 Shark sac Korean editor-1.1.2/
+-rw-rw-rw-   0        0        0      731 2023-06-10 07:21:07.499626 Shark sac Korean editor-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2023-04-27 07:59:41.000000 Shark sac Korean editor-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-10 07:21:07.433697 Shark sac Korean editor-1.1.2/Shark_sac_Korean_editor.egg-info/
+-rw-rw-rw-   0        0        0      731 2023-06-10 07:21:07.000000 Shark sac Korean editor-1.1.2/Shark_sac_Korean_editor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2708 2023-06-10 07:21:07.000000 Shark sac Korean editor-1.1.2/Shark_sac_Korean_editor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 07:21:07.000000 Shark sac Korean editor-1.1.2/Shark_sac_Korean_editor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-10 07:21:07.000000 Shark sac Korean editor-1.1.2/Shark_sac_Korean_editor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-10 07:21:07.449997 Shark sac Korean editor-1.1.2/modkr/
+-rw-rw-rw-   0        0        0      283 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.1.2/modkr/__init__.py
+-rw-rw-rw-   0        0        0     9136 2023-06-10 03:58:09.000000 Shark sac Korean editor-1.1.2/modkr/__main__.py
+-rw-rw-rw-   0        0        0    10151 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.1.2/modkr/adb_handler.py
+-rw-rw-rw-   0        0        0    13745 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.1.2/modkr/config_manager.py
+-rw-rw-rw-   0        0        0     1510 2023-06-10 06:54:54.000000 Shark sac Korean editor-1.1.2/modkr/csv_handler.py
+drwxrwxrwx   0        0        0        0 2023-06-10 07:21:07.451337 Shark sac Korean editor-1.1.2/modkr/edits/
+-rw-rw-rw-   0        0        0       67 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.1.2/modkr/edits/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 07:21:07.456112 Shark sac Korean editor-1.1.2/modkr/edits/basic/
+-rw-rw-rw-   0        0        0      122 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.1.2/modkr/edits/basic/__init__.py
+-rw-rw-rw-   0        0        0     9125 2023-06-10 05:12:02.000000 Shark sac Korean editor-1.1.2/modkr/edits/basic/basic_items.py
+-rw-rw-rw-   0        0        0     1490 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.1.2/modkr/edits/basic/catfruit.py
+-rw-rw-rw-   0        0        0     2017 2023-06-10 05:17:14.000000 Shark sac Korean editor-1.1.2/modkr/edits/basic/catseyes.py
+-rw-rw-rw-   0        0        0     1702 2023-06-10 05:47:34.000000 Shark sac Korean editor-1.1.2/modkr/edits/basic/ototo_base_mats.py
+-rw-rw-rw-   0        0        0     4136 2023-06-10 05:30:23.000000 Shark sac Korean editor-1.1.2/modkr/edits/basic/talent_orbs.py
+-rw-rw-rw-   0        0        0    16762 2023-06-10 05:34:36.000000 Shark sac Korean editor-1.1.2/modkr/edits/basic/talent_orbs_new.py
+drwxrwxrwx   0        0        0        0 2023-06-10 07:21:07.465287 Shark sac Korean editor-1.1.2/modkr/edits/cats/
+-rw-rw-rw-   0        0        0      179 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.1.2/modkr/edits/cats/__init__.py
+-rw-rw-rw-   0        0        0     8978 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.1.2/modkr/edits/cats/cat_helper.py
+-rw-rw-rw-   0        0        0    11473 2023-06-10 04:48:37.000000 Shark sac Korean editor-1.1.2/modkr/edits/cats/cat_id_selector.py
+-rw-rw-rw-   0        0        0     3378 2023-06-10 04:40:29.000000 Shark sac Korean editor-1.1.2/modkr/edits/cats/chara_drop.py
+-rw-rw-rw-   0        0        0     1081 2023-06-10 04:41:38.000000 Shark sac Korean editor-1.1.2/modkr/edits/cats/clear_cat_guide.py
+-rw-rw-rw-   0        0        0     2882 2023-06-10 04:42:21.000000 Shark sac Korean editor-1.1.2/modkr/edits/cats/evolve_cats.py
+-rw-rw-rw-   0        0        0     1268 2023-06-10 04:42:37.000000 Shark sac Korean editor-1.1.2/modkr/edits/cats/get_remove_cats.py
+-rw-rw-rw-   0        0        0     8010 2023-06-10 04:43:44.000000 Shark sac Korean editor-1.1.2/modkr/edits/cats/talents.py
+-rw-rw-rw-   0        0        0     2114 2023-06-10 07:13:45.000000 Shark sac Korean editor-1.1.2/modkr/edits/cats/upgrade_blue.py
+-rw-rw-rw-   0        0        0     4660 2023-06-10 07:15:32.000000 Shark sac Korean editor-1.1.2/modkr/edits/cats/upgrade_cats.py
+drwxrwxrwx   0        0        0        0 2023-06-10 07:21:07.468300 Shark sac Korean editor-1.1.2/modkr/edits/gamototo/
+-rw-rw-rw-   0        0        0       66 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.1.2/modkr/edits/gamototo/__init__.py
+-rw-rw-rw-   0        0        0      333 2023-06-10 05:39:01.000000 Shark sac Korean editor-1.1.2/modkr/edits/gamototo/fix_gamatoto.py
+-rw-rw-rw-   0        0        0     2878 2023-06-10 05:42:37.000000 Shark sac Korean editor-1.1.2/modkr/edits/gamototo/gamatoto_xp.py
+-rw-rw-rw-   0        0        0     3430 2023-06-10 05:43:35.000000 Shark sac Korean editor-1.1.2/modkr/edits/gamototo/helpers.py
+-rw-rw-rw-   0        0        0     7458 2023-06-10 05:58:12.000000 Shark sac Korean editor-1.1.2/modkr/edits/gamototo/ototo_cat_cannon.py
+drwxrwxrwx   0        0        0        0 2023-06-10 07:21:07.482726 Shark sac Korean editor-1.1.2/modkr/edits/levels/
+-rw-rw-rw-   0        0        0      313 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.1.2/modkr/edits/levels/__init__.py
+-rw-rw-rw-   0        0        0     1060 2023-06-10 06:06:45.000000 Shark sac Korean editor-1.1.2/modkr/edits/levels/aku.py
+-rw-rw-rw-   0        0        0      516 2023-06-10 06:06:59.000000 Shark sac Korean editor-1.1.2/modkr/edits/levels/allow_filibuster_clearing.py
+-rw-rw-rw-   0        0        0      815 2023-06-10 06:08:07.000000 Shark sac Korean editor-1.1.2/modkr/edits/levels/behemoth_culling.py
+-rw-rw-rw-   0        0        0      644 2023-06-10 06:08:16.000000 Shark sac Korean editor-1.1.2/modkr/edits/levels/clear_tutorial.py
+-rw-rw-rw-   0        0        0     1146 2023-06-10 06:08:52.000000 Shark sac Korean editor-1.1.2/modkr/edits/levels/enigma_stages.py
+-rw-rw-rw-   0        0        0     6453 2023-06-10 07:03:14.000000 Shark sac Korean editor-1.1.2/modkr/edits/levels/event_stages.py
+-rw-rw-rw-   0        0        0     1873 2023-06-10 06:14:29.000000 Shark sac Korean editor-1.1.2/modkr/edits/levels/gauntlet.py
+-rw-rw-rw-   0        0        0     1058 2023-06-10 06:14:57.000000 Shark sac Korean editor-1.1.2/modkr/edits/levels/itf_timed_scores.py
+-rw-rw-rw-   0        0        0     1481 2023-06-10 06:16:15.000000 Shark sac Korean editor-1.1.2/modkr/edits/levels/legend_quest.py
+-rw-rw-rw-   0        0        0     4372 2023-06-10 06:18:36.000000 Shark sac Korean editor-1.1.2/modkr/edits/levels/main_story.py
+-rw-rw-rw-   0        0        0     2350 2023-06-10 06:20:35.000000 Shark sac Korean editor-1.1.2/modkr/edits/levels/outbreaks.py
+-rw-rw-rw-   0        0        0     3076 2023-06-10 07:10:43.000000 Shark sac Korean editor-1.1.2/modkr/edits/levels/story_level_id_selector.py
+-rw-rw-rw-   0        0        0     1212 2023-06-10 06:25:23.000000 Shark sac Korean editor-1.1.2/modkr/edits/levels/towers.py
+-rw-rw-rw-   0        0        0     8550 2023-06-10 06:32:15.000000 Shark sac Korean editor-1.1.2/modkr/edits/levels/treasures.py
+-rw-rw-rw-   0        0        0     1081 2023-06-10 06:33:11.000000 Shark sac Korean editor-1.1.2/modkr/edits/levels/uncanny.py
+-rw-rw-rw-   0        0        0      801 2023-06-10 06:33:22.000000 Shark sac Korean editor-1.1.2/modkr/edits/levels/unlock_aku_realm.py
+drwxrwxrwx   0        0        0        0 2023-06-10 07:21:07.494688 Shark sac Korean editor-1.1.2/modkr/edits/other/
+-rw-rw-rw-   0        0        0      276 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.1.2/modkr/edits/other/__init__.py
+-rw-rw-rw-   0        0        0     3940 2023-06-10 06:36:04.000000 Shark sac Korean editor-1.1.2/modkr/edits/other/cat_shrine.py
+-rw-rw-rw-   0        0        0     1141 2023-06-10 06:36:40.000000 Shark sac Korean editor-1.1.2/modkr/edits/other/claim_user_rank_rewards.py
+-rw-rw-rw-   0        0        0     1058 2023-06-10 06:37:11.000000 Shark sac Korean editor-1.1.2/modkr/edits/other/create_new_account.py
+-rw-rw-rw-   0        0        0     2150 2023-06-10 06:38:29.000000 Shark sac Korean editor-1.1.2/modkr/edits/other/fix_elsewhere.py
+-rw-rw-rw-   0        0        0      705 2023-06-10 06:40:04.000000 Shark sac Korean editor-1.1.2/modkr/edits/other/fix_time_issues.py
+-rw-rw-rw-   0        0        0     3470 2023-06-10 06:41:27.000000 Shark sac Korean editor-1.1.2/modkr/edits/other/get_gold_pass.py
+-rw-rw-rw-   0        0        0     7233 2023-06-10 06:43:47.000000 Shark sac Korean editor-1.1.2/modkr/edits/other/meow_medals.py
+-rw-rw-rw-   0        0        0     4416 2023-06-10 06:45:55.000000 Shark sac Korean editor-1.1.2/modkr/edits/other/missions.py
+-rw-rw-rw-   0        0        0      985 2023-06-10 06:46:36.000000 Shark sac Korean editor-1.1.2/modkr/edits/other/play_time.py
+-rw-rw-rw-   0        0        0     4612 2023-06-10 06:47:06.000000 Shark sac Korean editor-1.1.2/modkr/edits/other/scheme_item.py
+-rw-rw-rw-   0        0        0     1645 2023-06-10 06:47:33.000000 Shark sac Korean editor-1.1.2/modkr/edits/other/trade_progress.py
+-rw-rw-rw-   0        0        0     1436 2023-06-10 06:48:09.000000 Shark sac Korean editor-1.1.2/modkr/edits/other/unlock_enemy_guide.py
+-rw-rw-rw-   0        0        0      356 2023-06-10 06:48:20.000000 Shark sac Korean editor-1.1.2/modkr/edits/other/unlock_equip_menu.py
+drwxrwxrwx   0        0        0        0 2023-06-10 07:21:07.499626 Shark sac Korean editor-1.1.2/modkr/edits/save_management/
+-rw-rw-rw-   0        0        0       56 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.1.2/modkr/edits/save_management/__init__.py
+-rw-rw-rw-   0        0        0     1331 2023-06-10 06:48:57.000000 Shark sac Korean editor-1.1.2/modkr/edits/save_management/convert.py
+-rw-rw-rw-   0        0        0     2718 2023-06-10 06:49:37.000000 Shark sac Korean editor-1.1.2/modkr/edits/save_management/load.py
+-rw-rw-rw-   0        0        0      661 2023-06-10 06:49:54.000000 Shark sac Korean editor-1.1.2/modkr/edits/save_management/other.py
+-rw-rw-rw-   0        0        0     2073 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.1.2/modkr/edits/save_management/save.py
+-rw-rw-rw-   0        0        0     2208 2023-06-10 06:50:35.000000 Shark sac Korean editor-1.1.2/modkr/edits/save_management/server_upload.py
+-rw-rw-rw-   0        0        0    13946 2023-06-10 05:47:12.000000 Shark sac Korean editor-1.1.2/modkr/feature_handler.py
+-rw-rw-rw-   0        0        0     4841 2023-06-10 05:56:27.000000 Shark sac Korean editor-1.1.2/modkr/game_data_getter.py
+-rw-rw-rw-   0        0        0    24350 2023-06-10 07:19:14.000000 Shark sac Korean editor-1.1.2/modkr/helper.py
+-rw-rw-rw-   0        0        0     7470 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.1.2/modkr/item.py
+-rw-rw-rw-   0        0        0     3505 2023-06-10 04:57:01.000000 Shark sac Korean editor-1.1.2/modkr/locale_handler.py
+-rw-rw-rw-   0        0        0     1269 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.1.2/modkr/managed_item.py
+-rw-rw-rw-   0        0        0    72179 2023-06-10 06:58:03.000000 Shark sac Korean editor-1.1.2/modkr/parse_save.py
+-rw-rw-rw-   0        0        0     1301 2023-06-10 06:58:57.000000 Shark sac Korean editor-1.1.2/modkr/patcher.py
+-rw-rw-rw-   0        0        0     2415 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.1.2/modkr/root_handler.py
+-rw-rw-rw-   0        0        0    55884 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.1.2/modkr/serialise_save.py
+-rw-rw-rw-   0        0        0    26654 2023-06-10 06:54:07.000000 Shark sac Korean editor-1.1.2/modkr/server_handler.py
+-rw-rw-rw-   0        0        0     3717 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.2/modkr/tracker.py
+-rw-rw-rw-   0        0        0     3640 2023-06-10 07:00:23.000000 Shark sac Korean editor-1.1.2/modkr/updater.py
+-rw-rw-rw-   0        0        0     4515 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.1.2/modkr/user_info.py
+-rw-rw-rw-   0        0        0     8297 2023-06-09 08:08:58.000000 Shark sac Korean editor-1.1.2/modkr/user_input_handler.py
+-rw-rw-rw-   0        0        0       42 2023-06-10 07:21:07.499626 Shark sac Korean editor-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      984 2023-06-10 07:20:10.000000 Shark sac Korean editor-1.1.2/setup.py
```

### Comparing `Shark sac Korean editor-1.1.1/PKG-INFO` & `Shark sac Korean editor-1.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Shark sac Korean editor
-Version: 1.1.1
+Version: 1.1.2
 Summary: 냥코에디터 한글화
 Home-page: https://github.com/sharkwodm/koreditor
 Author: 익명
 Author-email: 
 License: MIT
 Keywords: python,template
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Shark sac Korean editor-1.1.1/Shark_sac_Korean_editor.egg-info/PKG-INFO` & `Shark sac Korean editor-1.1.2/Shark_sac_Korean_editor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Shark-sac-Korean-editor
-Version: 1.1.1
+Version: 1.1.2
 Summary: 냥코에디터 한글화
 Home-page: https://github.com/sharkwodm/koreditor
 Author: 익명
 Author-email: 
 License: MIT
 Keywords: python,template
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Shark sac Korean editor-1.1.1/Shark_sac_Korean_editor.egg-info/SOURCES.txt` & `Shark sac Korean editor-1.1.2/Shark_sac_Korean_editor.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 modkr/parse_save.py
 modkr/patcher.py
 modkr/root_handler.py
 modkr/serialise_save.py
 modkr/server_handler.py
 modkr/tracker.py
 modkr/updater.py
+modkr/user_info.py
 modkr/user_input_handler.py
 modkr/edits/__init__.py
 modkr/edits/basic/__init__.py
 modkr/edits/basic/basic_items.py
 modkr/edits/basic/catfruit.py
 modkr/edits/basic/catseyes.py
 modkr/edits/basic/ototo_base_mats.py
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/__main__.py` & `Shark sac Korean editor-1.1.2/modkr/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     feature_handler,
     game_data_getter,
     helper,
     parse_save,
     patcher,
     serialise_save,
     server_handler,
-    tracker,
+    user_info,
     updater,
     user_input_handler,
     root_handler,
     locale_handler,
 )
 from .edits.levels import clear_tutorial
 
@@ -37,22 +37,21 @@
         new=helper.WHITE,
     )
     local_version = updater.get_local_version()
 
     print()
     if "b" in local_version:
         helper.colored_text(
+            locale_manager.search_key("beta_message"),
             base=helper.RED,
             new=helper.WHITE,
         )
     print()
     helper.colored_text(
         f"{locale_manager.search_key('thanks_title')}\n"
-        + f"{locale_manager.search_key('thanks_title2')}\n"
-        + f"{locale_manager.search_key('blacklist')}\n"
         + f"{locale_manager.search_key('lethal_thanks')}\n"
         + f"{locale_manager.search_key('beeven_cse_thanks')}\n"
         + f"{locale_manager.search_key('support_thanks')}\n"
         + locale_manager.search_key("discord_thanks"),
         base=helper.GREEN,
         new=helper.WHITE,
     )
@@ -60,14 +59,15 @@
 
 def check_update() -> None:
     """Check if there is an update available and if so, ask the user if they want to update"""
     version_info = updater.get_version_info()
     locale_manager = locale_handler.LocalManager.from_config()
     if version_info is None:
         helper.colored_text(
+            locale_manager.search_key("update_check_failed"), base=helper.RED
         )
         return
     stable_ver, pre_release_ver = version_info
 
     local_version = updater.get_local_version()
 
     helper.colored_text(
@@ -80,24 +80,23 @@
         helper.colored_text(
             f" &|& {locale_manager.search_key('latest_pre_release_version') % pre_release_ver}",
             base=helper.CYAN,
             new=helper.WHITE,
             end="",
         )
     print()
-   
+
+
 def main():
     """Main function"""
 
-    item_tracker = tracker.Tracker()
-
     if config_manager.get_config_value_category(
         "SERVER", "WIPE_TRACKED_ITEMS_ON_START"
     ):
-        item_tracker.reset_tracker()
+        user_info.UserInfo.clear_all_items()
     game_data_getter.check_remove_handler()
 
     check_updates = config_manager.get_config_value_category(
         "START_UP", "CHECK_FOR_UPDATES"
     )
     show_start = not config_manager.get_config_value_category(
         "START_UP", "HIDE_START_TEXT"
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/adb_handler.py` & `Shark sac Korean editor-1.1.2/modkr/adb_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -220,50 +220,50 @@
             helper.RED,
         )
         return
 
     adb_path = find_adb_path()
     if not adb_path:
         adb_path = input(
-            "adb가 포함된 폴더의 경로를 입력하세요: 다운로드 링크: https://dl.google.com/android/repository/platform-tools-latest-windows.zip:"
+            "Please enter the path to the folder than contains adb: download link here: https://dl.google.com/android/repository/platform-tools-latest-windows.zip:"
         )
         if os.path.isfile(adb_path):
             adb_path = os.path.dirname(adb_path)
 
     print(f"Adding {adb_path} to your path environment variable")
     backup = os.environ["PATH"]
     backup_path = os.path.join(config_manager.get_app_data_folder(), "path_backup.txt")
     helper.write_file_string(backup_path, backup)
     helper.colored_text(
-        f"이전 PATH 환경 변수가 다음에 백업되었습니다.&{backup_path}&"
+        f"Your old PATH environment variable has been backed up to &{backup_path}&"
     )
     subprocess.run(f'setx PATH "{adb_path};%PATH%"', shell=True, check=True, text=True)
-    print("경로에 adb를 성공적으로 추가했습니다.")
+    print("Successfully added adb to path")
 
 
 def adb_err_handler(err: ADBException):
     """Handle ADB errors"""
     if err.exception_type in (
         ADBExceptionTypes.NO_DEVICE,
         ADBExceptionTypes.DEVICE_OFFLINE,
     ):
         helper.colored_text(
-            "오류: adb 연결이 있는 장치를 찾을 수 없습니다. 하나를 연결하고 다시 시도하십시오. (장치가 감지될 때까지 약 1분 정도 기다려야 할 수 있습니다.)",
+            "Error: No device with an adb connection can be found, please connect one and try again. (You may have to wait aprox 1min for the device to be detected)",
             base=helper.RED,
         )
         adb_reboot()
     elif err.exception_type == ADBExceptionTypes.PATH_NOT_FOUND:
         helper.colored_text(
-            '오류: SAVE_DATA를 찾을 수 없습니다. 게임에 로드되었는지 확인하고 "시작"을 클릭한 후 다시 시도하세요..',
+            'Error: SAVE_DATA couldn\'t be located, please make sure you have loaded into the game and clicked "START" and try again.',
             base=helper.RED,
         )
     elif err.exception_type == ADBExceptionTypes.ADB_NOT_INSTALLED:
         add_adb = (
             user_input_handler.colored_input(
-                "오류, adb가 Path 환경 변수에 없습니다. github의 readme에 자습서가 있습니다. 지금 경로에 adb를 추가하시겠습니까?(&y&/&n&):"
+                "Error, adb is not in your Path environment variable. There is a tutorial in the github's readme. Would you like to try to add adb to your path now?(&y&/&n&):"
             )
             == "y"
         )
         if add_adb:
             add_to_path()
             print("Please re-run the editor to try again")
     elif err.exception_type == ADBExceptionTypes.MORE_THAN_ONE_DEVICE:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/config_manager.py` & `Shark sac Korean editor-1.1.2/modkr/config_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -251,19 +251,19 @@
 
 def edit_editor_settings(_: Any) -> None:
     """
     Edit the editor settings
     """
     locale_manager = locale_handler.LocalManager.from_config()
     options = [
-        "최대 비활성화",
-        "금지 경고 표시",
-        "카테고리 보기",
-        "기능 선택 설명 표시",
-        "데이터만 가져오기",
+        "DISABLE_MAXES",
+        "SHOW_BAN_WARNING",
+        "SHOW_CATEGORIES",
+        "SHOW_FEATURE_SELECT_EXPLANATION",
+        "ONLY_GET_EN_DATA",
     ]
     option_values = [get_config_value_category("EDITOR", option) for option in options]
     ids = user_input_handler.select_not_inc(options, "select", option_values)
     for option_id in ids:
         option_name = options[option_id]
         current_value = option_values[option_id]
         if current_value:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/csv_handler.py` & `Shark sac Korean editor-1.1.2/modkr/csv_handler.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 from typing import Any
 
 
 def remove_pkcs7_padding(data: bytes) -> bytes:
     """Remove pkcs7 padding from data."""
 
     if len(data) % 16 != 0:
-        raise Exception("Invalid data length")
+        raise Exception("잘못된 데이터 길이")
 
     padding_length = data[-1]
     if padding_length > 16:
-        raise Exception("Invalid padding length")
+        raise Exception("잘못된 패딩 길이")
     if data[-padding_length:] != bytes([padding_length] * padding_length):
-        raise Exception("Invalid padding")
+        raise Exception("잘못된 패딩")
 
     return data[:-padding_length]
 
 
 def remove_comments(data: str) -> str:
     """Remove in-line comments from data."""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/basic/basic_items.py` & `Shark sac Korean editor-1.1.2/modkr/edits/basic/basic_items.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     """Handler for editing cat food"""
 
     cat_food = item.IntItem(
         name="통조림",
         value=item.Int(save_stats["cat_food"]["Value"]),
         max_value=45000,
         bannable=item.Bannable(
-            managed_item.ManagedItemType.CATFOOD,
+            managed_item.ManagedItemType.CATFOOD, save_stats["inquiry_code"]
         ),
     )
     cat_food.edit()
     save_stats["cat_food"]["Value"] = cat_food.get_value()
     return save_stats
 
 
@@ -49,32 +49,34 @@
     """Handler for editing rare tickets"""
 
     rare_tickets = item.IntItem(
         name="레어 티켓",
         value=item.Int(save_stats["rare_tickets"]["Value"]),
         max_value=299,
         bannable=item.Bannable(
-            work_around='&희귀 티켓을 직접 편집하는 대신 "일반 티켓 최대 거래 진행" 전환 기능을 대신 사용하십시오! 훨씬 더 안전합니다.',
+            inquiry_code=save_stats["inquiry_code"],
+            work_around='&Instead of editing rare tickets directly, use the "Normal Ticket Max Trade Progress" conversion feature instead! It is much more safe.',
             type=managed_item.ManagedItemType.RARE_TICKET,
         ),
     )
     rare_tickets.edit()
     save_stats["rare_tickets"]["Value"] = rare_tickets.get_value()
     return save_stats
 
 
 def edit_platinum_tickets(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Handler for editing platinum tickets"""
 
     platinum_tickets = item.IntItem(
-        name="플래티넘 티켓",
+        name="플레티넘 티켓",
         value=item.Int(save_stats["platinum_tickets"]["Value"]),
         max_value=9,
         bannable=item.Bannable(
-            work_around="&플래티넘 티켓을 편집하는 대신 플래티넘 샤드를 편집하세요! 그들은 훨씬 더 안전합니다. 10 플래티넘 조각 = 1 플래티넘 티켓",
+            inquiry_code=save_stats["inquiry_code"],
+            work_around="&플래티넘 티켓을 편집하는 대신 플래티넘 조각를 편집하세요! 그들은 훨씬 더 안전합니다. 10 플래티넘 조각 = 1 플래티넘 티켓",
             type=managed_item.ManagedItemType.PLATINUM_TICKET,
         ),
     )
     platinum_tickets.edit()
     save_stats["platinum_tickets"]["Value"] = platinum_tickets.get_value()
     return save_stats
 
@@ -122,19 +124,19 @@
 
 def edit_battle_items(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Handler for editing battle items"""
 
     battle_items = item.IntItemGroup.from_lists(
         names=[
             "스피드 업",
-            "보물 레이더",
-            "부자 냥코고양이",
-            "고양이 cpu",
-            "고양이 직업",
-            "고양이 스나이퍼",
+            "트레저 레이더",
+            "고양이 도령",
+            "야옹컴[cpu]",
+            "고양이 박사",
+            "스냥이퍼",
         ],
         values=save_stats["battle_items"],
         maxes=9999,
         group_name="배틀 아이템",
     )
     battle_items.edit()
     save_stats["battle_items"] = battle_items.get_values()
@@ -142,46 +144,46 @@
     return save_stats
 
 
 def edit_engineers(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Handler for editing ototo engineers"""
 
     engineers = item.IntItem(
-        name="오토토",
+        name="오토토 조수",
         value=item.Int(save_stats["engineers"]["Value"]),
         max_value=5,
     )
     engineers.edit()
     save_stats["engineers"]["Value"] = engineers.get_value()
     return save_stats
 
 
 def edit_catamins(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Handler for editing catamins"""
 
     catamins = item.IntItemGroup.from_lists(
         names=[
-            "고양이 드링크 A",
-            "고양이 드링크 B",
-            "고양이 드링크 C",
+            "드링크 A",
+            "드링크 B",
+            "드링크 C",
         ],
         values=save_stats["catamins"],
         maxes=9999,
-        group_name="Catamins",
+        group_name="드링크",
     )
     catamins.edit()
     save_stats["catamins"] = catamins.get_values()
     return save_stats
 
 
 def edit_inquiry_code(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Handler for editing the inquiry code"""
 
     print(
-        "경고: 문의 코드 편집은 자신이 무엇을 하고 있는지 알고 있는 경우에만 수행해야 합니다! 올바르게 수행하지 않으면 게임 내에서 다른 오류가 발생하기 때문입니다!"
+        "⚠️경고: 문의 코드 편집은 자신이 무엇을 하고 있는지 알고 있는 경우에만 수행해야 합니다! 올바르게 수행하지 않으면 게임 내에서 다른 오류가 발생하기 때문입니다!"
     )
     inquiry_code = item.StrItem(
         name="문의 코드",
         value=save_stats["inquiry_code"],
     )
     inquiry_code.edit()
     save_stats["inquiry_code"] = inquiry_code.get_value()
@@ -214,15 +216,15 @@
     return save_stats
 
 
 def edit_token(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Handler for editing the password-refresh-token"""
 
     print(
-        "경고: 토큰 편집은 수행 중인 작업을 알고 있는 경우에만 수행해야 합니다! 올바르게 수행하지 않으면 게임 내에서 다른 오류가 발생하기 때문입니다!"
+        "⚠️경고: 토큰 편집은 수행 중인 작업을 알고 있는 경우에만 수행해야 합니다! 올바르게 수행하지 않으면 게임 내에서 다른 오류가 발생하기 때문입니다!"
     )
     token = item.StrItem(
         name="Token",
         value=save_stats["token"],
     )
     token.edit()
     save_stats["token"] = token.get_value()
@@ -237,15 +239,15 @@
     return save_stats
 
 
 def edit_challenge_battle(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Handler for editing the score of the challenge battle"""
 
     challenge_battle = item.IntItem(
-        name="도전 전투",
+        name="Challenge Battle",
         value=item.Int(save_stats["challenge"]["Score"]["Value"]),
         max_value=None,
     )
     challenge_battle.edit()
     save_stats["challenge"]["Score"]["Value"] = challenge_battle.get_value()
     save_stats["challenge"]["Cleared"]["Value"] = 1
     return save_stats
@@ -255,14 +257,15 @@
     """Handler for editing legend tickets"""
 
     legend_tickets = item.IntItem(
         name="레전드 티켓",
         value=item.Int(save_stats["legend_tickets"]["Value"]),
         max_value=4,
         bannable=item.Bannable(
+            inquiry_code=save_stats["inquiry_code"],
             type=managed_item.ManagedItemType.LEGEND_TICKET,
         ),
     )
     legend_tickets.edit()
     save_stats["legend_tickets"]["Value"] = legend_tickets.get_value()
     return save_stats
 
@@ -270,14 +273,14 @@
 def edit_dojo_score(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Handler for editing the dojo score"""
 
     if not save_stats["dojo_data"]:
         save_stats["dojo_data"] = {0: {0: 0}}
 
     dojo_score = item.IntItem(
-        name="랭킹 점수",
+        name="도장 점수",
         value=item.Int(save_stats["dojo_data"][0][0]),
         max_value=None,
     )
     dojo_score.edit()
     save_stats["dojo_data"][0][0] = dojo_score.get_value()
     return save_stats
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/basic/catfruit.py` & `Shark sac Korean editor-1.1.2/modkr/edits/basic/catfruit.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/basic/catseyes.py` & `Shark sac Korean editor-1.1.2/modkr/edits/basic/catseyes.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 def get_catseye_ids(is_jp: bool) -> list[int]:
     """Get the catseye ids"""
 
     file_data = game_data_getter.get_file_latest("DataLocal", "Gatyaitembuy.csv", is_jp)
     if file_data is None:
-        helper.error_text("Failed to get catseye ids")
+        helper.error_text("캣츠아이 ID를 가져오지 못했습니다.s")
         return []
     items = helper.parse_int_list_list(
         csv_handler.parse_csv(
             file_data.decode("utf-8"),
             ",",
         )[1:]
     )
@@ -28,34 +28,34 @@
 
 
 def get_catseye_names(is_jp: bool) -> list[str]:
     """Get the catseye names"""
 
     file_data = game_data_getter.get_file_latest("resLocal", "GatyaitemName.csv", is_jp)
     if file_data is None:
-        helper.error_text("Failed to get catseye names")
+        helper.error_text("캣츠아이 이름을 가져오지 못했습니다.")
         return []
     item_names = csv_handler.parse_csv(
         file_data.decode("utf-8"),
         helper.get_text_splitter(is_jp),
     )
     catseye_names: list[str] = []
     for catseye_id in get_catseye_ids(is_jp):
         try:
             catseye_names.append(item_names[catseye_id][0])
         except IndexError:
-            helper.error_text(f"Failed to get catseye name for {catseye_id}")
+            helper.error_text(f"에 대한 캣츠아이 이름을 가져오지 못했습니다. {catseye_id}")
     return catseye_names
 
 
 def edit_catseyes(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Handler for editing catseyes"""
 
     catseyes = item.IntItemGroup.from_lists(
         names=get_catseye_names(helper.check_data_is_jp(save_stats)),
         values=save_stats["catseyes"],
         maxes=9999,
-        group_name="Catseyes",
+        group_name="캣츠아이",
     )
     catseyes.edit()
     save_stats["catseyes"] = catseyes.get_values()
     return save_stats
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/basic/ototo_base_mats.py` & `Shark sac Korean editor-1.1.2/modkr/edits/basic/ototo_base_mats.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 
 
 def get_base_mats_names(is_jp: bool) -> list[str]:
     """Get the base material names"""
 
     file_data = game_data_getter.get_file_latest("resLocal", "GatyaitemName.csv", is_jp)
     if file_data is None:
-        helper.error_text("Failed to get base material names")
+        helper.error_text("기본 재료 이름을 가져오지 못했습니다.")
         return []
     item_names = csv_handler.parse_csv(
         file_data.decode("utf-8"),
         delimeter=helper.get_text_splitter(is_jp),
     )
     file_data = game_data_getter.get_file_latest("DataLocal", "Gatyaitembuy.csv", is_jp)
     if file_data is None:
-        helper.error_text("Failed to get gatya item buy data")
+        helper.error_text("재료 아이템 구매 데이터를 가져오지 못했습니다.")
         return []
     all_items = helper.parse_int_list_list(
         csv_handler.parse_csv(
             file_data.decode("utf-8"),
         )
     )[1:]
     base_mat_indexes: dict[int, str] = {}
@@ -39,12 +39,12 @@
 def edit_base_mats(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Handler for editing base materials"""
 
     base_mats = item.IntItemGroup.from_lists(
         names=get_base_mats_names(helper.check_data_is_jp(save_stats)),
         values=save_stats["base_materials"],
         maxes=9999,
-        group_name="Base Materials",
+        group_name="오토토 재료",
     )
     base_mats.edit()
     save_stats["base_materials"] = base_mats.get_values()
     return save_stats
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/basic/talent_orbs.py` & `Shark sac Korean editor-1.1.2/modkr/edits/basic/talent_orbs.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 from ... import helper, user_input_handler
 
 
 def edit_all_orbs(save_stats: dict[str, Any], orb_list: list[str]) -> dict[str, Any]:
     """Handler for editing all talent orbs"""
 
     val = user_input_handler.colored_input(
-        "모든 재능 구슬의 값을 무엇으로 설정하시겠습니까?:"
+        "모든 본능 오브의 값을 무엇으로 설정하시겠습니까?:"
     )
     val = helper.check_int_max(val)
     if val is None:
         print("오류 숫자를 입력하십시오")
         return save_stats
 
     for orb in orb_list:
         try:
             orb_id = orb_list.index(orb)
         except ValueError:
             continue
         save_stats["talent_orbs"][orb_id] = val
 
-    helper.colored_text(f"모든 재능 오브를 다음으로 설정 &{val}&")
+    helper.colored_text(f"모든 본능 오브를 다음으로 설정 &{val}&")
     return save_stats
 
 
 def edit_talent_orbs(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Handler for editing talent orbs"""
 
     orb_list = get_talent_orbs_types()
@@ -39,60 +39,60 @@
         text = "orbs" if amount != 1 else "orb"
         try:
             helper.colored_text(f"&{amount}& {orb_list[orb]} {text}")
         except IndexError:
             helper.colored_text(f"&{amount}& Unknown {orb} {text}")
 
     orbs_str = user_input_handler.colored_input(
-        "원하는 구의 이름을 입력합니다. &공백&로 구분된 여러 오브 이름을 입력하여 한 번에 여러 개를 편집하거나 &all&을 입력하여 편집할 모든 재능 오브를 선택할 수 있습니다.):"
+        "원하는 오브의 이름을 입력합니다. &공백&로 구분된 여러 구 이름을 입력하여 한 번에 여러 개를 편집하거나 &all&을 입력하여 편집할 모든 재능 구를 선택할 수 있습니다(예: &엔젤 a 거대한 레드 d 강한 블랙 b 내성&):"
     ).split(" ")
     if orbs_str[0] == "all":
         return edit_all_orbs(save_stats, orb_list)
     length = len(orbs_str) // 3
     orbs_to_set: list[int] = []
 
     for i in range(length):
         orb_name = " ".join(orbs_str[i * 3 : i * 3 + 3]).lower()
         orb_name = orb_name.replace("angle", "angel").title()
         try:
             orbs_to_set.append(orb_list.index(orb_name))
         except ValueError:
             helper.colored_text(
-                f"Error orb &{orb_name}& does not exist or is not recognized"
+                f"오류 오브 &{orb_name}& 존재하지 않거나 인식되지 않음"
             )
 
     for orb_id in orbs_to_set:
         name = orb_list[orb_id]
         val = helper.check_int_max(
             user_input_handler.colored_input(
-                f"What do you want to set the value of &{name}& to?:"
+                f"어떤 값을 설정하시겠습니까? &{name}& to?:"
             )
         )
         if val is None:
-            print("Error please enter a number")
+            print("오류 숫자를 입력하십시오")
             continue
         talent_orbs[orb_id] = val
     save_stats["talent_orbs"] = talent_orbs
 
     return save_stats
 
 
 ATTRIBUTES = [
-    "빨간색",
+    "빨간 적",
     "떠있는 적",
-    "검정",
-    "메탈",
+    "검은 적",
+    "메탈 적",
     "천사",
-    "에이리언",
+    "에일리언",
     "좀비",
 ]
 EFFECTS = [
     "공격",
     "방어",
-    "강한",
+    "데미지 경감",
     "엄청난",
     "내성",
 ]
 GRADES = [
     "D",
     "C",
     "B",
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/basic/talent_orbs_new.py` & `Shark sac Korean editor-1.1.2/modkr/edits/basic/talent_orbs_new.py`

 * *Files 1% similar despite different names*

```diff
@@ -368,25 +368,25 @@
 
         all_grades_str = "&,& ".join(all_grades)
         all_attributes_str = "&,& ".join(all_attributes)
         all_effects_str = "&,& ".join(all_effects)
 
         help_text = f"""Help:
 사용 가능한 등급: &{all_grades_str}&
-사용 가능한 속성:&{all_attributes_str}&
+사용 가능한 속성: &{all_attributes_str}&
 사용 가능한 효과: &{all_effects_str}&
 &참고: 모든 속성에 대해 모든 등급과 효과를 사용할 수 있는 것은 아닙니다.&
 예시 입력:
-    &aku& - &모든 aku& 오브 선택합니다
-    &red s& - &s& 등급의 모든 빨간색 &오브 선택합니다
-    &에일리언 d 공격& - &공격&을 증가시키는 &d& 등급의 &에일리언 &오브를 선택합니다.
+    &aku& - &all aku& 오브들 선택
+    &red s& - &s& 등급의 모든 빨간색 &orb 선택
+    &에일리언 d 공격& - &공격력&을 증가시키는 &d& 등급의 &에일리언 &orb를 선택합니다.
 전환할 수 있으므로 다음과 같은 작업도 수행할 수 있습니다.
-    &d 외계인 공격&
+    &d 에일리언 공격&
     &빨간색&
-    &공격 d 외계인&
+    &공격 d 에일리언&
 &all& 오브를 선택하려면 다음을 입력하십시오.
     &*&
 &여러 선택&을 수행하려면 다음과 같이 &쉼표&로 구분하십시오.
     &s 블랙 터프&,&d 레드 매시브&,&플로팅&
 """
         helper.colored_text(help_text)
 
@@ -432,30 +432,30 @@
 
         orb_selection = list(set(orb_selection))
         orb_selection.sort(key=lambda orb: orb.raw_orb_info.orb_id)
         orb_selection.sort(key=lambda orb: orb.raw_orb_info.grade_id)
         orb_selection.sort(key=lambda orb: orb.raw_orb_info.effect_id)
         orb_selection.sort(key=lambda orb: orb.raw_orb_info.attribute_id)
 
-        print("오브 선택:")
+        print("선택한 오브:")
         for orb in orb_selection:
             helper.colored_text((orb.to_colortext()))
 
         individual = (
-            input("구의 양을 개별적으로 수정하시겠습니까? 아니면 한꺼번에? [한번에a](i/a)") == "i"
+            input("오브의 양을 개별적으로 수정하시겠습니까? 아니면 한꺼번에? (i/a)") == "i"
         )
         if individual:
             for orb in orb_selection:
                 orb_id = orb.raw_orb_info.orb_id
                 try:
                     orb_count = self.orbs[orb_id].count
                 except KeyError:
                     orb_count = 0
                 orb_count = user_input_handler.colored_input(
-                    f"금액을 무엇으로 설정하시겠습니까? {orb.to_colortext()} to? (현재 &{orb_count}&) (&q& 종료하다):"
+                    f"금액을 무엇으로 설정하시겠습니까? {orb.to_colortext()} to? (현재 &{orb_count}&) (&q& 종료 하가위한):"
                 )
                 if orb_count == "q":
                     break
                 orb_count = helper.check_int_max(orb_count)
                 if orb_count is None:
                     continue
 
@@ -489,12 +489,12 @@
         save_stats (dict[str, Any]): The save_stats to edit the orbs in
 
     Returns:
         dict[str, Any]: The edited save_stats
     """
     save_orbs = SaveOrbs.from_save_stats(save_stats)
     if save_orbs is None:
-        print("Failed to load orbs")
+        print("오브를 로드하지 못했습니다.")
         return save_stats
     save_orbs.edit()
     save_orbs.save(save_stats)
     return save_stats
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/cats/cat_helper.py` & `Shark sac Korean editor-1.1.2/modkr/edits/cats/cat_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Helper for cats"""
 from typing import Any, Optional
 
 from ... import csv_handler, game_data_getter, helper
 from ..levels import main_story, uncanny
 
 TYPES = [
-    "노멀",
-    "레어",
-    "희귀",
-    "슈퍼레어",
-    "울트라 슈퍼 레어",
-    "레전드 레어",
+    "Normal",
+    "Special",
+    "Rare",
+    "Super Rare",
+    "Uber Super Rare",
+    "Legend Rare",
 ]
 
 
 def get_level_cap_increase_amount(cat_base_level: int) -> int:
     """
     Get the amount of levels to increase the level cap by
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/cats/cat_id_selector.py` & `Shark sac Korean editor-1.1.2/modkr/edits/cats/cat_id_selector.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 def select_cats(save_stats: dict[str, Any], current: bool = True) -> list[int]:
     """Select cats"""
 
     options: dict[str, Callable[[dict[str, Any]], list[int]]] = {
         "현재 잠금 해제된 고양이 선택": select_current_cats,
         "특정 희귀도의 고양이 선택": select_cats_rarity,
         "특정 고양이 ID 선택": select_cats_range,
-        "특정 가챠 배너의 고양이 선택": select_cats_gatya_banner,
+        "특정 뽑기 배너의 고양이 선택": select_cats_gatya_banner,
         "모든 고양이 선택": get_all_cats,
         "고양이 이름으로 검색": select_cat_names,
         "획득 가능한 모든 고양이 선택": select_cats_obtainable,
     }
     if not current:
         del options["현재 잠금 해제된 고양이 선택"]
 
@@ -75,29 +75,29 @@
 
 
 def select_cats_range(save_stats: dict[str, Any]) -> list[int]:
     """Select cats in a range"""
 
     ids = user_input_handler.get_range(
         user_input_handler.colored_input(
-            "고양이 ID를 입력하십시오(ID를 찾으려면 &냥코id사이트.kro.kr 에서 를 조회하십시오)(모든 범위를 얻으려면 &all&을 입력할 수 있습니다(예: &1&-&50& 또는 공백으로 구분된 ID(예: &5 4 7&)).:"
+            "고양이 ID를 입력하십시오(ID를 찾으려면 냥코id사이트.kro.kr에서 조회하십시오)(&all&을 입력하여 범위(예: &1&-&50& 또는 공백으로 구분된 ID(예: &5 4 7&)를 얻을 수 있음):"
         ),
         length=len(save_stats["cats"]),
     )
     return ids
 
 
 def select_cats_gatya_banner(save_stats: dict[str, Any]) -> list[int]:
     """Select cats for a specific gacha banner"""
     is_jp = helper.is_jp(save_stats)
     file_data = game_data_getter.get_file_latest(
         "DataLocal", "GatyaDataSetR1.csv", is_jp
     )
     if file_data is None:
-        helper.colored_text("개다레 배너를 가져오지 못했습니다.")
+        helper.colored_text("Failed to get gatya banners")
         return []
     data = helper.parse_int_list_list(csv_handler.parse_csv(file_data.decode("utf-8")))
     ids = user_input_handler.get_range(
         user_input_handler.colored_input(
             "가챠배너 아이디 입력 (원하는 가챠배너 조회 후 상단의 이미지 클릭 후 파일명 마지막 자리 찾기 (예. royal fest = 602))(&all& 입력하시면 모두 받으실 수 있습니다. 범위(예: &1&-&50&) 또는 공백으로 구분된 ID(예: &5 4 7&):"
         ),
         length=len(data),
@@ -124,41 +124,41 @@
 
     Returns:
         list[int]: cat ids
     """
     all_names = get_cat_names(save_stats)
     if all_names is None:
         return []
-    name = user_input_handler.colored_input("고양이 이름 입력:")
+    name = user_input_handler.colored_input("고양이 이름 입력[영어로]:")
     found_names = search_cat_names(name, all_names)
     found_names = filter_cat_names(found_names)
     if not found_names:
         print("해당 이름을 가진 고양이를 찾을 수 없습니다.")
         return []
 
     cat_ids: list[int] = []
     cat_ids_str: list[str] = []
     cat_names: list[str] = []
     for cat_name, cat_id, _ in found_names:
         cat_ids.append(cat_id)
         cat_name = cat_name.replace("&", "\\&")
         cat_names.append(cat_name)
-        cat_ids_str.append(f"고양이id: &{cat_id}&")
+        cat_ids_str.append(f"고양이 아이디: &{cat_id}&")
 
-    print("선택할 고양이의 인덱스 선택 (고양이 id 자체가 아님):")
+    print("선택할 고양이의 인덱스 선택(고양이 ID 자체가 아님):")
     indexes = user_input_handler.select_not_inc(
         cat_names, mode="select", extra_data=cat_ids_str
     )
     selected_ids: list[int] = []
     for index in indexes:
         try:
             selected_ids.append(cat_ids[index])
         except IndexError:
             helper.colored_text(
-                f"Option is too high: {index} - Make sure to select the index on the left rather than the cat id",
+                f"옵션이 너무 높음: {index} -고양이 ID가 아닌 왼쪽의 인덱스를 선택해야 합니다.",
                 helper.RED,
             )
     return selected_ids
 
 
 def get_cat_by_form_and_id(
     all_names: list[tuple[str, int, int]], cat_id: int, form_id: int
@@ -267,15 +267,15 @@
         Optional[list[tuple[str, int, int]]]: cat names and ids
     """
 
     is_jp = helper.is_jp(save_stats)
 
     path = game_data_getter.get_path("resLocal", "", is_jp)
     if path is None:
-        helper.colored_text("Failed to get cat names", helper.RED)
+        helper.colored_text("고양이 이름을 가져오지 못했습니다.", helper.RED)
         return None
     file_path_dir = os.path.dirname(helper.get_file(path))
     helper.create_dirs(file_path_dir)
     if len(helper.find_files_in_dir(file_path_dir, "Unit_Explanation")) < len(
         save_stats["cats"]
     ):
         helper.colored_text(
@@ -326,15 +326,15 @@
     Returns:
         list[int]: obtainability of cats (0 = not obtainable, 1 = obtainable)
     """
     file_data = game_data_getter.get_file_latest(
         "DataLocal", "nyankoPictureBookData.csv", helper.is_jp(save_stats)
     )
     if file_data is None:
-        helper.colored_text("Failed to get obtainability", helper.RED)
+        helper.colored_text("획득 가능성을 얻지 못했습니다.", helper.RED)
         return []
     data = helper.parse_int_list_list(csv_handler.parse_csv(file_data.decode("utf-8")))
     is_obtainable = helper.copy_first_n(data, 0)
     return is_obtainable
 
 
 def get_obtainable_cats(save_stats: dict[str, Any]) -> list[int]:
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/cats/chara_drop.py` & `Shark sac Korean editor-1.1.2/modkr/edits/cats/chara_drop.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     """handler for editing treasure ids"""
 
     unit_drops_stats = save_stats["unit_drops"]
     data = get_data(helper.check_data_is_jp(save_stats))
 
     usr_t_ids = user_input_handler.get_range(
         user_input_handler.colored_input(
-            "Enter treasures ids (Look up item drop cats battle cats to find ids)(You can enter &all& to get all, a range e.g &1&-&50&, or ids separate by spaces e.g &5 4 7&):"
+            "보물 ID를 입력하세요(id를 찾으려면 항목 드롭 고양이 전투 고양이를 조회하세요)(모든 항목을 얻으려면 &all&을 입력할 수 있습니다. 범위(예: &1&-&50&, 또는 공백으로 구분된 ID(예: &5 4 7&)):"
         ),
         all_ids=data["t_ids"],
     )
 
     unit_drops_stats = set_t_ids_val(unit_drops_stats, data, usr_t_ids)
 
     save_stats["unit_drops"] = unit_drops_stats
@@ -41,34 +41,34 @@
 
 
 def get_character_drops(save_stats: dict[str, Any]) -> dict[str, Any]:
     """handler for getting character drops"""
 
     flag_t_ids = (
         user_input_handler.colored_input(
-            "보물 ID를 선택하시겠습니까? &(1)&, 또는 고양이 ID? &(2)&:"
+            "보물 ID &(1)& 또는 고양이 ID를 선택하시겠습니까? &(2)&:ㅍㅍ"
         )
         == "1"
     )
 
     if flag_t_ids:
         save_stats = set_t_ids(save_stats)
     else:
         save_stats = set_c_ids(save_stats)
-    print("Successfully set unit drops")
+    print("성공적으로 유닛 드랍 설정")
 
     return save_stats
 
 
 def get_data(is_jp: bool) -> dict[str, Any]:
     """gets all of the cat ids and treasure ids that can be dropped"""
 
     file_data = game_data_getter.get_file_latest("DataLocal", "drop_chara.csv", is_jp)
     if file_data is None:
-        helper.error_text("Failed to get drop_chara.csv")
+        helper.error_text("drop_chara.csv를 가져오지 못했습니다.")
         return {"t_ids": [], "c_ids": [], "indexes": []}
     character_data = helper.parse_int_list_list(
         csv_handler.parse_csv(file_data.decode("utf-8"))[1:]
     )
 
     treasure_ids = helper.copy_first_n(character_data, 0)
     indexes = helper.copy_first_n(character_data, 1)
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/cats/clear_cat_guide.py` & `Shark sac Korean editor-1.1.2/modkr/edits/cats/clear_cat_guide.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 
 
 def collect_cat_guide(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Collect cat guide for cats"""
 
     ids = cat_id_selector.select_cats(save_stats)
 
-    save_stats = cat_guide_ids(save_stats, ids, 1, "수집된")
+    save_stats = cat_guide_ids(save_stats, ids, 1, "collected")
     return save_stats
 
 
 def remove_cat_guide(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Remove cat guide for cats"""
 
     ids = cat_id_selector.select_cats(save_stats)
 
-    save_stats = cat_guide_ids(save_stats, ids, 0, "제거된")
+    save_stats = cat_guide_ids(save_stats, ids, 0, "removed")
     return save_stats
 
 
 def cat_guide_ids(
     save_stats: dict[str, Any], ids: list[int], val: int, string: str
 ) -> dict[str, Any]:
     """Clear cat guide for a set of cat ids"""
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/cats/evolve_cats.py` & `Shark sac Korean editor-1.1.2/modkr/edits/cats/evolve_cats.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,41 +8,41 @@
 def get_evolve(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Handler for evolving cats"""
 
     cat_ids = cat_id_selector.select_cats(save_stats)
     return evolve_handler_ids(
         save_stats=save_stats,
         val=2,
-        string="설정",
+        string="set",
         ids=cat_ids,
         forced=False,
     )
 
 
 def get_evolve_forced(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Handler for evolving cats without the form check"""
 
     cat_ids = cat_id_selector.select_cats(save_stats)
     return evolve_handler_ids(
         save_stats=save_stats,
         val=2,
-        string="설정",
+        string="set",
         ids=cat_ids,
         forced=True,
     )
 
 
 def remove_evolve(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Handler for de-evolving cats"""
 
     cat_ids = cat_id_selector.select_cats(save_stats)
     return evolve_handler_ids(
         save_stats=save_stats,
         val=0,
-        string="제거",
+        string="removed",
         ids=cat_ids,
         forced=True,
     )
 
 
 def evolve_handler(
     save_stats: dict[str, Any], val: int, string: str, forced: bool
@@ -89,9 +89,9 @@
         zip(evolves, save_stats["current_forms"])
     ):
         save_stats["current_forms"][cat_id] = max(unlocked_flag, current_flag)
 
     flags_evolved = [0 if form == 1 else form for form in evolves]
     save_stats["unlocked_forms"] = flags_evolved
 
-    print(f"성공적인 {string}고양이의 진정한 형태")
+    print(f"성공적으로 {string} 고양이의 진정한 형태")
     return save_stats
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/cats/get_remove_cats.py` & `Shark sac Korean editor-1.1.2/modkr/edits/cats/get_remove_cats.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,29 +9,29 @@
     """Handler to get cats"""
 
     cat_ids = cat_id_selector.select_cats(save_stats, False)
 
     save_stats = get_cat_ids(
         save_stats=save_stats,
         val=1,
-        string="얻다",
+        string="gave",
         ids=cat_ids,
     )
     return save_stats
 
 
 def remove_cats(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Handler to remove cats"""
 
     cat_ids = cat_id_selector.select_cats(save_stats, False)
 
     save_stats = get_cat_ids(
         save_stats=save_stats,
         val=0,
-        string="제거",
+        string="removed",
         ids=cat_ids,
     )
     return save_stats
 
 
 def get_cat_ids(
     save_stats: dict[str, Any], val: int, string: str, ids: list[int]
@@ -43,12 +43,12 @@
     cats = save_stats["cats"]
     seen_cats = save_stats["gatya_seen_cats"]
 
     for cat_id in ids:
         cats[cat_id] = val
         seen_cats[cat_id] = val
 
-    save_stats["냥코캐릭터"] = cats
+    save_stats["cats"] = cats
     save_stats["gatya_seen_cats"] = seen_cats
     save_stats["menu_unlocks"][2] = 1
-    print(f"성공 {string} 냥코캐릭터")
+    print(f"성공적으로 {string} 고양이")
     return save_stats
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/cats/talents.py` & `Shark sac Korean editor-1.1.2/modkr/edits/cats/talents.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 def get_talent_data(save_stats: dict[str, Any]) -> Optional[dict[Any, Any]]:
     """Get talent data for all cats"""
 
     file_data = game_data_getter.get_file_latest(
         "DataLocal", "SkillAcquisition.csv", helper.check_data_is_jp(save_stats)
     )
     if file_data is None:
-        helper.error_text("재능 데이터를 가져오지 못했습니다.")
+        helper.error_text("본능 데이터를 가져오지 못했습니다.")
         return None
     talent_data_raw = helper.parse_int_list_list(
         csv_handler.parse_csv(
             file_data.decode("utf-8"),
         )
     )
     file_data = game_data_getter.get_file_latest(
         "resLocal", "SkillDescriptions.csv", helper.check_data_is_jp(save_stats)
     )
     if file_data is None:
-        helper.error_text("재능 이름을 가져오지 못했습니다.")
+        helper.error_text("본능 이름을 가져오지 못했습니다.")
         return None
     talent_names = csv_handler.parse_csv(
         file_data.decode("utf-8"),
         helper.get_text_splitter(helper.check_data_is_jp(save_stats)),
     )
     columns = helper.int_to_str_ls(talent_data_raw[0])
     new_talent_data: dict[Any, Any] = {}
@@ -69,32 +69,27 @@
 
 
 def find_order(
     cat_talents: list[dict[str, Any]], cat_talent_data: dict[str, Any]
 ) -> list[str]:
     """Find what talent slot each letter corresponds to"""
 
-    letters = [
-        "A",
-        "B",
-        "C",
-        "D",
-        "E",
-        "F",
-    ]
+    letters = ["A", "B", "C", "D", "E", "F", "G", "H"]
     letter_order: list[str] = []
 
-    for i, talent in enumerate(cat_talents):
-        if i == 0:
-            continue
+    for talent in cat_talents:
         talent_id = talent["id"]
         for letter in letters:
-            ability_id = int(cat_talent_data[f"abilityID_{letter}"])
+            key = f"abilityID_{letter}"
+            if key not in cat_talent_data:
+                continue
+            ability_id = int(cat_talent_data[key])
             if ability_id == talent_id:
                 letter_order.append(letter)
+                break
     return letter_order
 
 
 def get_cat_talents(
     cat_talents: list[dict[str, Any]], cat_talent_data: dict[str, Any]
 ) -> dict[Any, Any]:
     """Get the name and max value of each talent for a specific cat"""
@@ -130,15 +125,15 @@
     return cat_talents_levels
 
 
 def max_all_talents(save_stats: dict[str, Any]):
     """Max all talents for all cats"""
     max_all = (
         user_input_handler.colored_input(
-            "재능을 최대화하거나 재능을 재설정하고 싶습니까? (&m&/&r&):"
+            "Do you want to max talents or reset talents? (&m&/&r&):"
         )
         == "m"
     )
     if not max_all:
         return remove_all_talents(save_stats)
     talents = save_stats["talents"]
 
@@ -150,18 +145,18 @@
     cat_talents_levels: list[int] = []
     for cat_id in ids:
         if cat_id not in talents or cat_id not in talent_data:
             continue
         cat_talents = talents[cat_id]
         cat_talents_levels = get_talent_levels(talent_data, talents, cat_id)
         for i, cat_talent_level in enumerate(cat_talents_levels):
-            cat_talents[i + 1]["level"] = cat_talent_level
+            cat_talents[i]["level"] = cat_talent_level
         save_stats["talents"] = talents
 
-    print("재능을 성공적으로 설정")
+    print("본능을 성공적으로 설정")
     return save_stats
 
 
 def remove_all_talents(save_stats: dict[str, Any]) -> dict[str, Any]:
     """
     Remove all talents for all cats
 
@@ -181,18 +176,18 @@
     cat_talents_levels: list[int] = []
     for cat_id in ids:
         if cat_id not in talents or cat_id not in talent_data:
             continue
         cat_talents = talents[cat_id]
         cat_talents_levels = get_talent_levels(talent_data, talents, cat_id)
         for i in range(len(cat_talents_levels)):
-            cat_talents[i + 1]["level"] = 0
+            cat_talents[i]["level"] = 0
         save_stats["talents"] = talents
 
-    print("재능을 성공적으로 제거했습니다.")
+    print("본능을 성공적으로 제거했습니다.")
     return save_stats
 
 
 def edit_talents_individual(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Handler for editing talents"""
 
     talents = save_stats["talents"]
@@ -203,39 +198,39 @@
         return save_stats
     for cat_id in ids:
         cat_talents_levels: list[int] = []
         if cat_id not in talents or cat_id not in talent_data:
             # don't spam the user with messages if they selected alot of ids at once
             if len(ids) < 20:
                 helper.colored_text(
-                    f"오류 고양이 &{cat_id}&에 재능이 없습니다.",
+                    f"Error cat &{cat_id}& does not have any talents",
                     helper.RED,
                     helper.WHITE,
                 )
             continue
         cat_talent_data = talent_data[cat_id]
         cat_talents = talents[cat_id]
         cat_talent_data_formatted = get_cat_talents(cat_talents, cat_talent_data)
         names: list[str] = []
         maxes: list[int] = []
         for talent_index, cat_talent_formatted in cat_talent_data_formatted.items():
             names.append(cat_talent_formatted["name"])
-            cat_talents_levels.append(cat_talents[talent_index + 1]["level"])
+            cat_talents_levels.append(cat_talents[talent_index]["level"])
             maxes.append(cat_talent_formatted["max"])
-        helper.colored_text(f"고양이 &{cat_id}&가 선택되었습니다.:")
+        helper.colored_text(f"Cat &{cat_id}& is selected:")
         cat_talents_levels_g = item.IntItemGroup.from_lists(
             names=names,
             values=cat_talents_levels,
             maxes=maxes,
             group_name="Talents",
         )
         cat_talents_levels_g.edit()
         cat_talents_levels = cat_talents_levels_g.get_values()
         for i, cat_talent_level in enumerate(cat_talents_levels):
-            cat_talents[i + 1]["level"] = cat_talent_level
+            cat_talents[i]["level"] = cat_talent_level
 
         talents[cat_id] = cat_talents
 
         save_stats["talents"] = talents
 
-    print("재능을 성공적으로 설정")
+    print("본능을 성공적으로 설정")
     return save_stats
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/cats/upgrade_blue.py` & `Shark sac Korean editor-1.1.2/modkr/edits/cats/upgrade_blue.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 """Handler for upgrading the blue upgrades"""
 from typing import Any
 
 from ... import helper, user_input_handler
 from . import upgrade_cats
 
 TYPES = [
-    "Power",
-    "Range",
-    "Charge",
-    "Efficiency",
-    "Wallet",
-    "Health",
-    "Research",
-    "Accounting",
-    "Study",
-    "Energy",
+    "냥코 대포 공격력",
+    "냥코 대포 사정거리",
+    "냥코 대포 충전",
+    "일 고양이의 의 호율",
+    "일 고양이의 의 지갑",
+    "성 체력",
+    "연구력",
+    "회계력",
+    "공부력",
+    "통솔력",
 ]
 
 
 def upgrade_blue_ids(save_stats: dict[str, Any], ids: list[int]) -> dict[str, Any]:
     """Upgrade blue upgrades for a set of ids"""
 
     save_stats["blue_upgrades"] = upgrade_cats.upgrade_handler(
         data=save_stats["blue_upgrades"],
         ids=ids,
-        item_name="upgrade",
+        item_name="업그레이드",
         save_stats=save_stats,
     )
     save_stats = upgrade_cats.set_user_popups(save_stats)
-    print("Successfully set special skills")
+    print("특수 기술을 성공적으로 설정")
     return save_stats
 
 
 def upgrade_blue(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Handler for editing blue upgrades"""
 
     levels = save_stats["blue_upgrades"]
@@ -41,20 +41,20 @@
         "Plus": [levels["Plus"][0]] + levels["Plus"][2:],
     }
 
     levels_removed_formated: list[str] = []
     for base, plus in zip(levels_removed["Base"], levels_removed["Plus"]):
         levels_removed_formated.append(f"{base + 1}+{plus}")
 
-    print("What do you want to upgrade:")
+    print("무엇을 업그레이드하고 싶습니까?:\n⚠️1만이상숫자넣지마십시요")
     helper.colored_list(TYPES, extra_data=levels_removed_formated)
 
     total = len(TYPES) + 1
     ids = user_input_handler.colored_input(
-        f"{total}. &All at once&\nEnter a number from 1 to {total} (You can enter multiple values separated by spaces to edit multiple at once):"
+        f"{total}. &한 번에&\n1부터 숫자를 입력하세요.{total} (공백으로 구분된 여러 값을 입력하여 한 번에 여러 값을 편집할 수 있습니다.):"
     ).split(" ")
     ids = user_input_handler.create_all_list_not_inc(ids, 11)
     ids = helper.parse_int_list(ids, -1)
     new_ids: list[int] = []
     for blue_id in ids:
         if blue_id > 0:
             blue_id += 1
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/cats/upgrade_cats.py` & `Shark sac Korean editor-1.1.2/modkr/edits/cats/upgrade_cats.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,36 +75,36 @@
     ids = helper.check_cat_ids(ids, save_stats)
 
     base = data["Base"]
     plus = data["Plus"]
     individual = True
     if len(ids) > 1:
         individual = user_input_handler.ask_if_individual(
-            f"냥코의 업그레이드{item_name}"
+            f"각각의 업그레이드 {item_name}"
         )
     first = True
     base_lvl = None
     plus_lvl = None
     for cat_id in ids:
         if not individual and first:
             levels = get_plus_base(
                 user_input_handler.colored_input(
-                    '냥코 캐릭터 기본 수준 다음에 "&+&" 다음에 플러스 수준을 입력합니다(예: 5&+&12). 기본 레벨을 무시하려면 &+&12 를 입력 하시구 플러스 레벨을 무시하려면 &5+&를 입력하십시오. 올강레벨(예제:30+70):\n'
+                    '냥코 캐릭터 기본 수준 다음에 "&+&" 다음에 플러스 수준을 입력합니다(예: 5&+&12). 기본 레벨을 무시하려면 &+&12 를 입력 하시구 플러스 레벨을 무시하려면 5&+&를 입력하십시오. 올강레벨(예제:90+90)\n냥코지갑 [예제:10000]:\n'
                 )
             )
             base_lvl = levels[0]
             plus_lvl = levels[1]
             first = False
         elif individual:
             helper.colored_text(
-                f"냥코캐릭터 id의 현재 업그레이드 레벨&{cat_id}& is &{base[cat_id]+1}&+&{plus[cat_id]}&"
+                f"냥코id의 현재 업그레이드 레벨 &{cat_id}& is &{base[cat_id]+1}&+&{plus[cat_id]}&"
             )
             levels = get_plus_base(
                 user_input_handler.colored_input(
-                    f'냥코캐릭터 대한 기준 레벨을 입력합니다.{item_name}: &{cat_id}&"&+&"그런 다음 플러스 수준뒤에 , 예: 5&+&12. 기본 레벨을 무시하려면 &+&12를 수행하고 플러스 레벨을 무시하려면 &+&5를 수행하십시오.\n'
+                    f'냥코에 대한 기준 레벨을 입력합니다. {item_name}: &{cat_id}& "&+&" 다음에 플러스 레벨이 옵니다(예: 5&+&12). 기본 레벨을 무시하려면 &+&12를 수행하고 플러스 레벨을 무시하려면 5&+&를 수행하십시오.\n'
                 )
             )
             base_lvl = levels[0]
             plus_lvl = levels[1]
         if base_lvl is not None:
             if base_lvl > 0:
                 base_lvl = helper.clamp(base_lvl, 0, 50000)
@@ -120,14 +120,14 @@
 
 def upgrade_cats_ids(save_stats: dict[str, Any], ids: list[int]) -> dict[str, Any]:
     """Upgrade cats by ids"""
 
     save_stats["cat_upgrades"] = upgrade_handler(
         data=save_stats["cat_upgrades"],
         ids=ids,
-        item_name="cat",
+        item_name="고양이",
         save_stats=save_stats,
     )
     save_stats = set_user_popups(save_stats)
     # save_stats = set_level_caps(save_stats)
     print("고양이 레벨을 성공적으로 설정했습니다.")
     return save_stats
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/gamototo/gamatoto_xp.py` & `Shark sac Korean editor-1.1.2/modkr/edits/gamototo/gamatoto_xp.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def get_boundaries(is_jp: bool) -> Optional[list[int]]:
     """Get the xp requirements for each level"""
 
     file_data = game_data_getter.get_file_latest(
         "DataLocal", "GamatotoExpedition.csv", is_jp
     )
     if file_data is None:
-        helper.error_text("Failed to get gamatoto xp requirements")
+        helper.error_text("가마토토 경험치 요구 사항을 가져오지 못했습니다.")
         return None
     boundaries = file_data.decode("utf-8").splitlines()
     previous = 0
     xp_requirements: list[int] = []
     previous = 0
     for line in boundaries:
         requirement = int(line.split(",")[0])
@@ -62,18 +62,18 @@
     gamatoto_xp = save_stats["gamatoto_xp"]
 
     data = get_level_from_xp(gamatoto_xp["Value"], helper.check_data_is_jp(save_stats))
     if data is None:
         return save_stats
     level = data["level"]
 
-    helper.colored_text(f"Gamatoto xp: &{gamatoto_xp['Value']}&\nLevel: &{level}&")
+    helper.colored_text(f"가마토토 경험치: &{gamatoto_xp['Value']}&\n레벨: &{level}&")
     raw = (
         user_input_handler.colored_input(
-            "가마토토 경험치를 편집하시겠습니까?(&1&)또는 레벨(&2&)?:"
+            "가마토토 경험치(&1&) 또는 레벨(&2&)을 편집하시겠습니까?:"
         )
         == "1"
     )
 
     if raw:
         gam_xp = item.IntItem(
             name="가마토토 경험치",
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/gamototo/helpers.py` & `Shark sac Korean editor-1.1.2/modkr/edits/gamototo/helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     else:
         country_code = "en"
 
     file_data = game_data_getter.get_file_latest(
         "resLocal", f"GamatotoExpedition_Members_name_{country_code}.csv", is_jp
     )
     if file_data is None:
-        helper.error_text("Failed to get gamatoto helper data")
+        helper.error_text("가마토토 도우미 데이터를 가져오지 못했습니다.")
         return None
     data = file_data.decode("utf-8").splitlines()[1:]
     helpers: dict[str, Any] = {}
     for line in data:
         line_data = line.split(helper.get_text_splitter(is_jp))
         if len(line_data) < 5:
             break
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/levels/aku.py` & `Shark sac Korean editor-1.1.2/modkr/edits/levels/aku.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,9 +23,9 @@
         aku["clear_amount"][0][0][stage_index] = 1
         for i in range(stage_index):
             aku["clear_amount"][0][0][i] = 1
         for i in range(stage_index + 1, 49):
             aku["clear_amount"][0][0][i] = 0
 
     save_stats["aku"]["Value"] = aku
-    helper.colored_text("aku 단계를 성공적으로 설정했습니다.")
+    helper.colored_text("마계 단계를 성공적으로 설정했습니다.")
     return save_stats
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/levels/allow_filibuster_clearing.py` & `Shark sac Korean editor-1.1.2/modkr/edits/levels/allow_filibuster_clearing.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/levels/behemoth_culling.py` & `Shark sac Korean editor-1.1.2/modkr/edits/levels/behemoth_culling.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,13 +10,13 @@
 
     stage_data = save_stats["behemoth_culling"]
     lengths = stage_data["Lengths"]
 
     ids = []
     ids = user_input_handler.get_range(
         user_input_handler.colored_input(
-            "베헤모스 컬링 ID를 입력하세요. (예) &0& = &가프라의 숨겨진 숲&, &1& = &아쉬비니 사막&) (&all&을 입력하여 모두 가져오거나 범위(예: 1-49) 또는 공백으로 구분된 ID(예: &5 4 7&)를 가져올 수 있습니다.):"
+            "거대 컬링 ID 입력(예: &0& = &가프라의 숨겨진 숲&, &1& = &아시비니 사막&)(&all&을 입력하면 범위(예: 1-49, 또는 공백으로 구분된 ID(예: &5 4 7&)를 얻을 수 있음):"
         ),
         lengths["total"],
     )
     save_stats["behemoth_culling"] = event_stages.stage_handler(stage_data, ids, 0)
     return save_stats
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/levels/clear_tutorial.py` & `Shark sac Korean editor-1.1.2/modkr/edits/levels/clear_tutorial.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 def clear_tutorial(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Handler for clearing the tutorial"""
 
     save_stats["tutorial_cleared"]["Value"] = 1
     if save_stats["story_chapters"]["Chapter Progress"][0] == 0:
         save_stats["story_chapters"]["Chapter Progress"][0] = 1
     save_stats["story_chapters"]["Times Cleared"][0][0] = 1
-    print("튜토리얼을 클리어했습니다")
+    print("튜토리얼을 클리어했다")
 
     return save_stats
 
 
 def is_tutorial_cleared(save_stats: dict[str, Any]) -> bool:
     """Check if the tutorial is cleared"""
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/levels/enigma_stages.py` & `Shark sac Korean editor-1.1.2/modkr/edits/levels/enigma_stages.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,9 +33,9 @@
         data["stage_id"] = abs_id
         data["decoding_status"] = 2
         data["start_time"] = int(time.time())
         enigma_stages["stages"].append(data)
 
     save_stats["enigma_data"] = enigma_stages
 
-    print("Successfully edited enigma stages")
+    print("수수께끼 단계를 성공적으로 편집했습니다.")
     return save_stats
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/levels/event_stages.py` & `Shark sac Korean editor-1.1.2/modkr/edits/levels/event_stages.py`

 * *Files 13% similar despite different names*

```diff
@@ -111,51 +111,51 @@
     first = True
     stars = 0
     stage_data_edit = stage_data
     for stage_id in ids:
         if not individual and first:
             stars = helper.check_int(
                 user_input_handler.colored_input(
-                    f"별/크라운의 수를 입력하세요. (max &{lengths['stars']}&):"
+                    f"별/크라운의 수를 입력하십시오(최대 &{lengths['stars']}&):"
                 )
             )
             if stars is None:
-                print("Please enter a valid number")
+                print("유효한 숫자를 입력하세요.")
                 break
             stars = helper.clamp(stars, 0, lengths["stars"])
             first = False
         elif individual:
             stars = helper.check_int(
                 user_input_handler.colored_input(
-                    f"하위 장에 대한 별/크라운의 수를 입력하십시오. &{stage_id}& (max &{lengths['stars']}&):"
+                    f"하위 장에 대한 별/크라운의 수를 입력하십시오. &{stage_id}& (최대 &{lengths['stars']}&):"
                 )
             )
             if stars is None:
-                print("Please enter a valid number")
+                print("유효한 숫자를 입력하세요.")
                 break
             stars = helper.clamp(stars, 0, lengths["stars"])
         stage_id += offset
         stage_data_edit = stage_data
         stage_data_edit = set_stage_data(
             stage_data_edit, stage_id, stars, lengths, unlock_next
         )
 
-    print("Successfully set subchapters")
+    print("성공적으로 하위 챕터 설정")
 
     return stage_data_edit
 
 
 def stories_of_legend(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Handler for clearing stories of legend"""
 
     stage_data = save_stats["event_stages"]
 
     ids = user_input_handler.get_range(
         user_input_handler.colored_input(
-            "하위 챕터 ID 입력 (e.g &1& = legend begins, &2& = passion land)(You can enter &all& to get all, a range e.g &1&-&49&, or ids separate by spaces e.g &5 4 7&):"
+            "하위 챕터 ID 입력(예: &1& = 범례 시작, &2& = 열정의 땅)(모든 범위를 가져오려면 &all&을 입력할 수 있습니다. 예: &1&-&49& 또는 공백으로 구분된 ID(예: &5 4 7&):"
         ),
         50,
     )
     offset = -1
     save_stats["event_stages"] = stage_handler(stage_data, ids, offset)
     save_stats["event_stages"], save_stats["medals"] = set_medals(
         save_stats["event_stages"],
@@ -171,15 +171,15 @@
     """Handler for clearing event stages"""
 
     stage_data = save_stats["event_stages"]
     lengths = stage_data["Lengths"]
 
     ids = user_input_handler.get_range(
         user_input_handler.colored_input(
-            "하위 챕터 ID 입력 (&이벤트 출시 주문 전투 고양이&를 조회하여 ID를 찾습니다.)(예: &1&-&50& 또는 공백으로 구분된 ID(예: &5 4 7&)를 모두 가져오려면 &all&을 입력할 수 있습니다.):"
+            "하위 챕터 ID를 입력하십시오(ID를 찾으려면 &이벤트 출시 순서 전투 고양이& 조회)(&all&을 입력하여 범위(예: &1&-&50&, 또는 공백으로 구분된 ID(예: &5 4 7&)를 얻을 수 있음):"
         ),
         lengths["total"] - 400,
     )
     offset = 400
     save_stats["event_stages"] = stage_handler(stage_data, ids, offset)
     save_stats["event_stages"], save_stats["medals"] = set_medals(
         save_stats["event_stages"],
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/levels/gauntlet.py` & `Shark sac Korean editor-1.1.2/modkr/edits/levels/gauntlet.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     stage_data = save_stats["gauntlets"]
     lengths = stage_data["Lengths"]
 
     ids = []
     ids = user_input_handler.get_range(
         user_input_handler.colored_input(
-            "건틀릿 ID 입력 (찾아보기 및 이벤트 릴리스 전투 고양이를 주문하고 이벤트를 스크롤하여 건틀릿 ​​ID를 찾으십시오.) (&all&을 입력하여 모두 가져오거나 범위(예: 1-49) 또는 공백으로 구분된 ID(예: &5 4 7&)를 가져올 수 있습니다.):"
+            "Enter gauntlet ids (Look up &Event Release Order battle cats& and scroll past the &events& to find &gauntlet& ids) (You can enter &all& to get all, a range e.g 1-49, or ids separate by spaces e.g &5 4 7&):"
         ),
         lengths["total"],
     )
     save_stats["gauntlets"] = event_stages.stage_handler(stage_data, ids, 0)
     base_addr = meow_medals.BaseMapIds.GAUNTLETS.value
     save_stats["gauntlets"], save_stats["medals"] = event_stages.set_medals(
         save_stats["gauntlets"],
@@ -36,13 +36,13 @@
 
     stage_data = save_stats["collab_gauntlets"]
     lengths = stage_data["Lengths"]
 
     ids = []
     ids = user_input_handler.get_range(
         user_input_handler.colored_input(
-            "콜라보 건틀릿 ID 입력 (&이벤트& 및 &건틀릿& 과거를 지나 &콜라보 건틀렛& ID를 찾으려면 &이벤트 출시 순서 전투 고양이&를 찾아 스크롤하십시오.) (&all&을 입력하여 모두 가져오거나 범위(예: 1-49) 또는 공백으로 구분된 ID(예: &5 4 7&)를 가져올 수 있습니다.):"
+            "Enter collab gauntlet ids (Look up &Event Release Order battle cats& and scroll past the &events& and past &gauntlet& to find &Collaboration Gauntlet& ids) (You can enter &all& to get all, a range e.g 1-49, or ids separate by spaces e.g &5 4 7&):"
         ),
         lengths["total"],
     )
     save_stats["collab_gauntlets"] = event_stages.stage_handler(stage_data, ids, 0)
     return save_stats
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/levels/itf_timed_scores.py` & `Shark sac Korean editor-1.1.2/modkr/edits/levels/itf_timed_scores.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,19 +16,19 @@
     return scores
 
 
 def timed_scores(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Handler for setting into the future timed scores"""
 
     scores = save_stats["itf_timed_scores"]
-    print("다음 장의 점수를 입력하세요.:")
+    print("다음 장의 점수를 입력하십시오.")
     usr_scores = item.IntItemGroup.from_lists(
         names=main_story.CHAPTERS[3:6],
         values=None,
         maxes=9999,
-        group_name="미래의 시간 초과 점수",
+        group_name="미래편 시간 초과 점수",
     )
     usr_scores.edit()
     save_stats["itf_timed_scores"] = set_scores(scores, usr_scores.get_values_none())
 
     print("시간 제한 점수를 성공적으로 설정했습니다.")
     return save_stats
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/levels/legend_quest.py` & `Shark sac Korean editor-1.1.2/modkr/edits/levels/legend_quest.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/levels/main_story.py` & `Shark sac Korean editor-1.1.2/modkr/edits/levels/main_story.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 from typing import Any
 
 
 from ... import helper
 from . import story_level_id_selector
 
 CHAPTERS = [
-    "고양이 제국 1",
-    "고양이 제국 2",
-    "고양이 제국 3",
+    "세계편 1",
+    "세계편 2",
+    "세계편 3",
     "미래편 1",
     "미래편 2",
     "미래편 3",
-    "코스모스의 고양이들 1",
-    "코스모스의 고양이들 2",
-    "코스모스의 고양이들 3",
+    "우주편 1",
+    "우주편 2",
+    "우주편 3",
 ]
 
 
 def clear_specific_level_ids(
     save_stats: dict[str, Any], chapter_id: int, progress: int
 ) -> dict[str, Any]:
     """Clear specific levels in a chapter"""
@@ -103,15 +103,15 @@
 
 def clear_each(save_stats: dict[str, Any]):
     """Clear stages for each chapter"""
 
     chapter_ids = story_level_id_selector.select_specific_chapters()
 
     for chapter_id in chapter_ids:
-        helper.colored_text(f"Chapter: &{chapter_id+1}& : &{CHAPTERS[chapter_id]}&")
+        helper.colored_text(f"챕터: &{chapter_id+1}& : &{CHAPTERS[chapter_id]}&")
         formatted_id = format_story_id(chapter_id)
         progress = story_level_id_selector.select_level_progress(
             chapter_id, get_total_stages(save_stats, formatted_id)
         )
         save_stats = clear_specific_level_ids(save_stats, formatted_id, progress)
     helper.colored_text("메인 스토리 챕터를 성공적으로 설정")
     return save_stats
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/levels/outbreaks.py` & `Shark sac Korean editor-1.1.2/modkr/edits/levels/outbreaks.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,28 +51,28 @@
     """Handler for editting outbreaks"""
 
     outbreaks = save_stats["outbreaks"]
     current_outbreaks = save_stats["current_outbreaks"]
 
     clear = (
         user_input_handler.colored_input(
-            "아웃브레이크를 지우거나 지우지 않으시겠습니까? (&c&/&u&): "
+            "좀비스테이지를 지우거나 지우지 않으시겠습니까? (&c&/&u&): "
         )
         == "c"
     )
 
     available_chapters = get_available_chapters(outbreaks)
 
-    print("What chapter do you want to edit:")
+    print("편집할 챕터:")
     ids = user_input_handler.select_not_inc(
         options=available_chapters,
-        mode="바이러스을 소멸시키다?",
+        mode="에 대한 발병을 제거합니까?",
     )
     ids = helper.check_clamp(ids, len(available_chapters) + 1, 0, 0)
     ids = main_story.format_story_ids(ids)
     outbreaks, current_outbreaks = set_outbreaks(
         outbreaks, current_outbreaks, ids, clear
     )
     save_stats["outbreaks"] = outbreaks
     save_stats["current_outbreaks"] = current_outbreaks
-    print("확산을 성공적으로 설정")
+    print("청소를 성공적으로 설정")
     return save_stats
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/levels/story_level_id_selector.py` & `Shark sac Korean editor-1.1.2/modkr/edits/levels/story_level_id_selector.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from . import main_story
 
 
 def select_specific_chapters() -> list[int]:
     """Select specific levels"""
 
     print("어떤 챕터를 선택하시겠습니까?")
-    ids = user_input_handler.select_not_inc(main_story.CHAPTERS, "클리어")
+    ids = user_input_handler.select_not_inc(main_story.CHAPTERS, "clear")
     return ids
 
 
 def get_option():
     """Get option"""
 
     options = [
@@ -44,33 +44,33 @@
 
 def select_specific_levels(chapter_id: Optional[int], total: int) -> list[int]:
     """Select specific levels"""
 
     print("어떤 수준을 선택하시겠습니까?")
     if chapter_id is not None:
         helper.colored_text(
-            f"챕터: &{chapter_id+1}& : &{main_story.CHAPTERS[chapter_id]}&"
+            f"Chapter: &{chapter_id+1}& : &{main_story.CHAPTERS[chapter_id]}&"
         )
     ids = user_input_handler.get_range_ids(
-        "Level ids (e.g &1&=한국, &2&=몽골)", total
+        "레벨 ID(예: &1&=한국, &2&=몽골)", total
     )
     ids = helper.check_clamp(ids, total, 1, -1)
     return ids
 
 
 def select_levels_up_to(chapter_id: Optional[int], total: int) -> list[int]:
     """Select levels up to a certain level"""
 
     print("어떤 수준을 선택하시겠습니까?")
     if chapter_id is not None:
         helper.colored_text(
-            f"챕터: &{chapter_id+1}& : &{main_story.CHAPTERS[chapter_id]}&"
+            f"Chapter: &{chapter_id+1}& : &{main_story.CHAPTERS[chapter_id]}&"
         )
     stage_id = user_input_handler.get_int(
-        f"최대 삭제/해제하려는 단계 ID를 입력하세요. (그리고 포함) (예: &1&=korea 삭제됨, &2&=korea &and& mongolia 삭제됨, &{total}&=all)?:"
+        f"원하는단계 단계 ID를 최대(및 포함)까지 입력하세요(예: &1&=한국 클리어, &2&=한국 &또는& 몽골 클리어, &{total}&=all)?:"
     )
     stage_id = helper.clamp(stage_id, 1, total)
     return list(range(0, stage_id))
 
 
 def select_all(total: int) -> list[int]:
     """Select all levels"""
@@ -82,20 +82,20 @@
     chapter_id: Optional[int], total: int, examples: Optional[list[str]] = None
 ) -> int:
     """Select level progress"""
 
     if examples is None:
         examples = [
             "한국",
-            "몽골리아",
+            "몽골",
         ]
 
     print("어떤 레벨까지 클리어하고 싶나요?")
     if chapter_id is not None:
         helper.colored_text(
             f"챕터: &{chapter_id+1}& : &{main_story.CHAPTERS[chapter_id]}&"
         )
     progress = user_input_handler.get_int(
-        f"클리어할려는 스테이지 ID를 입력하세요./노클리어 (e.g &1&={examples[0]} 클리어, &2&={examples[0]} &and& {examples[1]} 클리어, &{total}&=올클리어, &0&=노클리어 모두)?:"
+        f"원하는 단계 ID를 입력하세요.클리어/언클리어 (e.g &1&={examples[0]} 클리어, &2&={examples[0]} &또는& {examples[1]} 클리어, &{total}&=all, &0&=언클리어 all)?:"
     )
     progress = helper.clamp(progress, 0, total)
     return progress
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/levels/towers.py` & `Shark sac Korean editor-1.1.2/modkr/edits/levels/towers.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         "Value": stage_data,
         "Lengths": {"stars": stage_data["stars"], "stages": stage_data["stages"]},
     }
 
     ids = []
     ids = user_input_handler.get_range(
         user_input_handler.colored_input(
-            "타워 ID 입력 (&이벤트 출시 순서 전투 고양이&를 찾아 스크롤하여 &이벤트& and &건틀릿& &탑& ID 찾기) (&all&을 입력하여 &1&-&49&와 같은 범위 또는 &5 4 7&와 같이 공백으로 구분된 ID를 모두 가져올 수 있습니다.):"
+            "타워 ID를 입력합니다(&이벤트 출시 순서 전투 고양이&를 찾아 &이벤트& 및 &장갑?&을 지나 스크롤하여 &타워& ID를 찾습니다)(&all&을 입력하여 범위(예: &1&-&49&, 또는 공백으로 구분된 ID(예: &5 4 7&)): "
         ),
         stage_data["Value"]["total"],
     )
     save_stats["tower"]["progress"] = event_stages.stage_handler(
         stage_data, ids, 0, False
     )["Value"]
     save_stats["tower"]["progress"]["total"] = stage_data["Value"]["total"]
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/levels/treasures.py` & `Shark sac Korean editor-1.1.2/modkr/edits/levels/treasures.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,26 +20,26 @@
             file_data.decode("utf-8"),
         )
     )[11:22]
     file_data = game_data_getter.get_file_latest(
         "DataLocal", "treasureData1.csv", is_jp
     )
     if file_data is None:
-        helper.error_text("가져오지 못했습니다 treasureData1.csv")
+        helper.error_text("가져오지 못했습니다. treasureData1.csv")
         return None
     itf_treasures = helper.parse_int_list_list(
         csv_handler.parse_csv(
             file_data.decode("utf-8"),
         )
     )[11:22]
     file_data = game_data_getter.get_file_latest(
         "DataLocal", "treasureData2_0.csv", is_jp
     )
     if file_data is None:
-        helper.error_text("가져오지 못했습니다 treasureData2_0.csv")
+        helper.error_text("가져오지 못했습니다. treasureData2_0.csv")
         return None
     cotc_treasures = helper.parse_int_list_list(
         csv_handler.parse_csv(
             file_data.decode("utf-8"),
         )
     )[11:22]
 
@@ -68,39 +68,39 @@
     else:
         country_code = "en"
 
     file_data = game_data_getter.get_file_latest(
         "resLocal", f"Treasure3_0_{country_code}.csv", is_jp
     )
     if file_data is None:
-        helper.error_text(f"가져오지 못했습니다 Treasure3_0_{country_code}.csv")
+        helper.error_text(f"가져오지 못했습니다. Treasure3_0_{country_code}.csv")
         return None
     eoc_names = csv_handler.parse_csv(
         file_data.decode("utf-8"),
         delimeter=helper.get_text_splitter(is_jp),
     )[:11]
 
     file_data = game_data_getter.get_file_latest(
         "resLocal", f"Treasure3_1_AfterFirstEncounter_{country_code}.csv", is_jp
     )
     if file_data is None:
         helper.error_text(
-            f"가져오지 못했습니다 Treasure3_1_AfterFirstEncounter_{country_code}.csv"
+            f"가져오지 못했습니다. Treasure3_1_AfterFirstEncounter_{country_code}.csv"
         )
         return None
     itf_names = csv_handler.parse_csv(
         file_data.decode("utf-8"),
         delimeter=helper.get_text_splitter(is_jp),
     )[:11]
 
     file_data = game_data_getter.get_file_latest(
         "resLocal", f"Treasure3_2_0_{country_code}.csv", is_jp
     )
     if file_data is None:
-        helper.error_text(f"가져오지 못했습니다 Treasure3_2_0_{country_code}.csv")
+        helper.error_text(f"가져오지 못했습니다. Treasure3_2_0_{country_code}.csv")
         return None
     cotc_names = csv_handler.parse_csv(
         file_data.decode("utf-8"),
         delimeter=helper.get_text_splitter(is_jp),
     )[:11]
 
     names.append(helper.copy_first_n(eoc_names, 0))
@@ -171,24 +171,24 @@
     """Handler for editing treasure groups"""
 
     treasure_grps = get_treasure_groups(helper.check_data_is_jp(save_stats))
     if treasure_grps is None:
         return save_stats
     treasures_stats = save_stats["treasures"]
 
-    ids = user_input_handler.select_not_inc(main_story.CHAPTERS, "선택하다")
+    ids = user_input_handler.select_not_inc(main_story.CHAPTERS, "설정")
 
     for chapter_id in ids:
         helper.colored_text(f"챕터: &{main_story.CHAPTERS[chapter_id]}&")
         type_id = chapter_id // 3
         if chapter_id > 2:
             chapter_id += 1
         names = treasure_grps["names"][type_id]
         treasure_levels = [-1] * len(names)
-        helper.colored_text("&0& = 없음, &1& = 못한, &2& = 노멀, &3& = 우수한")
+        helper.colored_text("&0& = 없음, &1& = 낮음, &2& = 보통, &3& = 높음")
         treasure_levels = item.IntItemGroup.from_lists(
             names=names,
             values=None,
             maxes=None,
             group_name="보물",
         )
         treasure_levels.edit()
@@ -217,17 +217,17 @@
         stage_ids = story_level_id_selector.select_levels(chapter_id, choice)
         treasure_data = [-1] * 48
         treasure_data = user_input_handler.handle_all_at_once(
             stage_ids,
             False,
             treasure_data,
             list(range(1, 49)),
-            "보물 레벨",
-            "스테이지",
-            "(&0&=없음, &1&=못한, &2&=노멀, &3&=우수한)",
+            "treasure level",
+            "stage",
+            "(&0&=없음, &1&=열등, &2&=정상, &3&=우수)",
         )
         treasure_stats = set_specific_treasures(
             treasure_stats, treasure_data, chapter_id
         )
     save_stats["treasures"] = treasure_stats
     print("성공적으로 보물 설정")
     return save_stats
@@ -246,17 +246,17 @@
         chapter_id = main_story.format_story_id(chapter_id)
         if i == 0:
             treasure_data = user_input_handler.handle_all_at_once(
                 stage_ids,
                 True,
                 treasure_data,
                 list(range(0, 48)),
-                "보물 레벨",
-                "스테이지",
-                "(&0&=none없음, &1&=못한, &2&=노멀, &3&=우수한)",
+                "treasure level",
+                "stage",
+                "(&0&=없음, &1&=열등, &2&=정상, &3&=우수)",
             )
         treasure_stats = set_specific_treasures(
             treasure_stats, treasure_data, chapter_id
         )
     save_stats["treasures"] = treasure_stats
     print("성공적으로 보물 설정")
     return save_stats
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/levels/uncanny.py` & `Shark sac Korean editor-1.1.2/modkr/edits/levels/uncanny.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     """Handler for editting uncanny legends"""
     stage_data = save_stats["uncanny"]
     lengths = stage_data["Lengths"]
 
     ids = []
     ids = user_input_handler.get_range(
         user_input_handler.colored_input(
-            "단계 ID 입력(예: &1& = 새 범례, &2& = 여기 드래곤)(모든 범위를 가져오려면 &all&을 입력할 수 있습니다. 예: &1&-&49& 또는 공백으로 구분된 ID(예: &5 4 7&)):"
+            "단계 ID 입력(예: &1& = 새 범례, &2& = 여기 드래곤)(모든 범위를 가져오려면 &all&을 입력할 수 있습니다. 예: &1&-&49& 또는 공백으로 구분된 ID(예: &5 4 7&):"
         ),
         lengths["total"],
     )
     save_stats["uncanny"] = event_stages.stage_handler(stage_data, ids, -1)
 
     return save_stats
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/levels/unlock_aku_realm.py` & `Shark sac Korean editor-1.1.2/modkr/edits/levels/unlock_aku_realm.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,9 +20,9 @@
         save_stats["event_stages"] = event_stages.set_stage_data(
             save_stats["event_stages"],
             stage_id + offset,
             1,
             save_stats["event_stages"]["Lengths"],
             True,
         )
-    helper.colored_text("&마계 영역이 성공적으로 잠금 해제되었습니다..")
+    helper.colored_text("&마계 영역이 성공적으로 잠금 해제되었습니다.")
     return save_stats
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/other/cat_shrine.py` & `Shark sac Korean editor-1.1.2/modkr/edits/other/cat_shrine.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         is_jp (bool): If the save file is japanese
 
     Returns:
         list[int]: The xp requirements for each level
     """
     file_data = game_data_getter.get_file_latest("resLocal", "jinja_level.csv", is_jp)
     if file_data is None:
-        helper.error_text("Failed to get jinja level data")
+        helper.error_text("신전 레벨 데이터를 가져오지 못했습니다.")
         return None
     boundaries = file_data.decode("utf-8").splitlines()
     xp_requirements: list[int] = []
     counter = 0
     for line in boundaries:
         requirement = int(line.split(helper.get_text_splitter(is_jp))[0])
         counter += requirement
@@ -86,33 +86,33 @@
     shrine_xp = save_stats["cat_shrine"]["xp_offering"]
 
     data = get_level_from_xp(shrine_xp, helper.check_data_is_jp(save_stats))
     if data is None:
         return save_stats
     level = data["level"]
 
-    helper.colored_text(f"신전 경험치: &{shrine_xp}&\n레벨: &{level}&")
+    helper.colored_text(f"신사 경험치: &{shrine_xp}&\n레벨: &{level}&")
     raw = (
         user_input_handler.colored_input(
-            "신전 경험치(&1&) 또는 레벨(&2&)을 편집하시겠습니까?:"
+            "신사 경험치를 편집하시겠습니까?(&1&) 또는 레벨(&2&)?:"
         )
         == "1"
     )
 
     if raw:
         cat_shrine_xp = item.IntItem(
-            name="신전 경험치",
+            name="신사 경험치",
             value=item.Int(shrine_xp),
             max_value=None,
         )
         cat_shrine_xp.edit()
         shrine_xp = int(cat_shrine_xp.get_value())
     else:
         shrine_level = item.IntItem(
-            name="신전 레벨",
+            name="신사 레벨",
             value=item.Int(level),
             max_value=data["max_level"],
         )
         shrine_level.edit()
         shrine_xp = get_xp_from_level(
             int(shrine_level.get_value()), helper.check_data_is_jp(save_stats)
         )
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/other/create_new_account.py` & `Shark sac Korean editor-1.1.2/modkr/edits/other/create_new_account.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from . import fix_elsewhere
 from ... import helper, server_handler
 
 
 def create_new_account(save_stats: dict[str, Any]):
     """Create a new account"""
 
-    helper.colored_text("Creating a new inquiry code and token...", helper.GREEN)
+    helper.colored_text("새 조회 코드 및 토큰 생성 중...", helper.GREEN)
 
     save_stats["inquiry_code"] = server_handler.get_inquiry_code()
     save_stats["token"] = "0" * 40
     save_stats = fix_elsewhere.fix_elsewhere(save_stats, force_mi=True)
 
     return save_stats
 
@@ -24,14 +24,14 @@
 
     Args:
         save_stats (dict[str, Any]): The save stats
 
     Returns:
         dict[str, Any]: The save stats
     """
-    helper.colored_text("Creating a new inquiry code and token...", helper.GREEN)
+    helper.colored_text("새 조회 코드 및 토큰 생성 중...", helper.GREEN)
 
     save_stats["inquiry_code"] = server_handler.get_inquiry_code()
     save_stats["token"] = "0" * 40
     save_stats = fix_elsewhere.fix_elsewhere(save_stats, force_mi=True, text=False)
 
     return save_stats
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/other/fix_elsewhere.py` & `Shark sac Korean editor-1.1.2/modkr/edits/other/fix_elsewhere.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Fix the elsewhere issue and unban an account"""
 import json
 import os
 from typing import Any
 
 
-from ... import helper, adb_handler, server_handler, tracker
+from ... import helper, adb_handler, server_handler, user_info
 
 
 def edit_cache(password: str, token: str, save_stats: dict[str, Any]) -> bool:
     """Edit the cache file in /data/data/jp.co.ponos.battlecats/files/cache/ to add the token and password"""
 
     data = {"password": password, "token": token}
     data_s = json.dumps(data)
@@ -26,33 +26,33 @@
         )
     except adb_handler.ADBException:
         success = False
     os.remove(local_path)
     return success
 
 
-def fix_elsewhere(save_stats: dict[str, Any], force_mi: bool = False, text: bool = True) -> dict[str, Any]:
+def fix_elsewhere(
+    save_stats: dict[str, Any], force_mi: bool = False, text: bool = True
+) -> dict[str, Any]:
     """Handler for fixing the elsewhere issue and unban an account"""
 
-    helper.colored_text("Getting account password...", helper.GREEN)
+    helper.colored_text("계정 비밀번호 얻기...", helper.GREEN)
     original_iq = save_stats["inquiry_code"]
     data = server_handler.check_gen_token(save_stats)
     token = data["token"]
     inquiry_code = data["inquiry_code"]
-    password_refresh_data = data["password_refresh_data"]
     if token is None:
-        helper.colored_text("Failed to get auth token", helper.RED)
+        helper.colored_text("인증 토큰을 가져오지 못했습니다.", helper.RED)
         return save_stats
-    edit_cache(password_refresh_data["password"], token, save_stats)
     if original_iq != inquiry_code or force_mi:
-        item_tracker = tracker.Tracker()
-        item_tracker.reset_tracker()
+        info = user_info.UserInfo(inquiry_code)
+        info.clear_managed_items()
         server_handler.update_managed_items(
             save_stats["inquiry_code"], token, save_stats
         )
     if text:
         helper.colored_text(
-            "완료!\n재생을 누르면 금지 메시지가 표시될 수 있습니다. 그럴 경우 재생을 다시 누르면 사라집니다.\n계속하려면 Enter를 누르십시오...(변경 사항을 저장해야 합니다.)",
+            "완료!\n재생을 누르면 금지 메시지가 표시될 수 있습니다. 그럴 경우 재생을 다시 누르면 사라집니다.\n계속하려면 엔터키를 누르십시오...(변경 사항을 저장해야 합니다.)",
             helper.DARK_YELLOW,
         )
         input()
     return save_stats
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/other/fix_time_issues.py` & `Shark sac Korean editor-1.1.2/modkr/edits/other/fix_time_issues.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,12 +15,12 @@
     """
     save_stats["third_time"] = helper.get_iso_time()
 
     save_stats["time_stamp"] = helper.get_time()
     save_stats["time_stamp_4"] = helper.get_time()
 
     helper.colored_text(
-        "시간 문제를 성공적으로 수정했습니다 &(이 작업을 수행하려면 두 장치의 장치 시간이 정확해야 합니다!)&",
+        "시간 문제를 성공적으로 수정했습니다 &(이 작업을 수행하려면 두 기기의 기기 시간이 모두 정확해야 합니다!)&",
         helper.GREEN,
         helper.RED,
     )
     return save_stats
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/other/get_gold_pass.py` & `Shark sac Korean editor-1.1.2/modkr/edits/other/get_gold_pass.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,26 +93,28 @@
     return random.randint(1, 2**16 - 1)
 
 
 def get_gold_pass(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Give the gold pass"""
 
     officer_id = user_input_handler.colored_input(
-        "원하는 회원코드 ID& 입력 (&랜덤 id&에 ​​대해 &엔터&를 누르고, &-1&을 입력하여 골드 패스를 &제거&):"
+        "원하는 &임원 ID&를 입력하세요.:"
     )
     if officer_id == "":
         officer_id = get_random_officer_id()
+    elif officer_id == "-1":
+        officer_id = -1
     else:
         officer_id = helper.check_int_max(officer_id)
 
     if officer_id is None:
         officer_id = 0
 
     if officer_id == -1:
         save_stats = remove_gold_pass_val(save_stats)
         helper.colored_text("골드 패스를 성공적으로 제거했습니다.", helper.GREEN)
     else:
-        helper.colored_text(f"Officer ID: &{officer_id}&", helper.GREEN, helper.WHITE)
+        helper.colored_text(f"임원 ID: &{officer_id}&", helper.GREEN, helper.WHITE)
         save_stats = get_gold_pass_val(save_stats, 30, officer_id)
         helper.colored_text("성공적으로 골드 패스를 제공했습니다.", helper.GREEN)
 
     return save_stats
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/other/meow_medals.py` & `Shark sac Korean editor-1.1.2/modkr/edits/other/meow_medals.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 def get_medal_names(is_jp: bool) -> Optional[list[str]]:
     """Get all medal names"""
 
     file_data = game_data_getter.get_file_latest("resLocal", "medalname.tsv", is_jp)
     if file_data is None:
-        helper.error_text("Failed to get medal names")
+        helper.error_text("메달 이름을 가져오지 못했습니다.")
         return None
     medal_names = file_data.decode("utf-8").splitlines()
     names: list[str] = []
     for line in medal_names:
         line_split = line.split("\t")
         name = (
             line_split[0]
@@ -165,17 +165,17 @@
         self.actions = actions
         self.stages = stages
 
 
 def get_medal_data(is_jp: bool) -> Optional[Medals]:
     """Get the medal data"""
 
-    file_data = game_data_getter.get_file_latest_fix("DataLocal", "medallist.json", is_jp)
+    file_data = game_data_getter.get_file_latest("DataLocal", "medallist.json", is_jp)
     if file_data is None:
-        helper.error_text("Failed to get medal data")
+        helper.error_text("메달 데이터를 가져오지 못했습니다.")
         return None
     medal_data = json.loads(file_data.decode("utf-8"))["iconID"]
 
     treasures: list[TreasureMedal] = []
     characters: list[CharacterMedal] = []
     actions: list[ActionMedal] = []
     stages: list[StageMedal] = []
@@ -235,30 +235,30 @@
 
 def medals(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Handler for editting meow medals"""
 
     medal_stats = save_stats["medals"]
     remove = (
         user_input_handler.colored_input(
-            "Do you want to add or remove medals? (&a&/&r&):"
+            "메달을 추가하거나 제거하시겠습니까?(&a&/&r&):"
         )
         == "r"
     )
 
     names = get_medal_names(helper.check_data_is_jp(save_stats))
     if names is None:
         return save_stats
     helper.colored_list(names)
 
     ids = user_input_handler.get_range(
         user_input_handler.colored_input(
-            "Enter medal ids (You can enter all to get &all&, a range e.g &1&-&50&, or ids separate by spaces e.g &5 4 7&):"
+            "메달 ID 입력(&all&, 예: &1&-&50& 또는 공백으로 구분된 ID(예: &5 4 7&)을 얻기 위해 모두 입력할 수 있음):"
         ),
         len(names) + 1,
     )
     if remove:
         medal_stats = remove_medals(medal_stats, ids)
     else:
         medal_stats = set_medals(medal_stats, ids)
     save_stats["medals"] = medal_stats
-    print(f"Successfully {'gave' if not remove else 'removed'} medals")
+    print(f"메달이 성공적으로 {'추가됨' if not remove else '제거됨'} ")
     return save_stats
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/other/missions.py` & `Shark sac Korean editor-1.1.2/modkr/edits/other/missions.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def get_mission_conditions(is_jp: bool) -> Optional[dict[Any, Any]]:
     """Get the mission data and what you need to do to complete it"""
 
     file_data = game_data_getter.get_file_latest(
         "DataLocal", "Mission_Condition.csv", is_jp
     )
     if file_data is None:
-        helper.error_text("Failed to get mission conditions")
+        helper.error_text("미션 조건을 얻지 못했습니다.")
         return None
     mission_condition_data = file_data.decode("utf-8")
     mission_conditions_list = helper.parse_int_list_list(
         csv_handler.parse_csv(mission_condition_data)
     )
     mission_conditions: dict[Any, Any] = {}
     for line in mission_conditions_list[1:]:
@@ -30,15 +30,15 @@
 
 
 def get_mission_names(is_jp: bool) -> Optional[dict[int, Any]]:
     """Get all mission names"""
 
     file_data = game_data_getter.get_file_latest("resLocal", "Mission_Name.csv", is_jp)
     if file_data is None:
-        helper.error_text("Failed to get mission names")
+        helper.error_text("임무 이름을 가져오지 못했습니다.")
         return None
     mission_name = file_data.decode("utf-8")
     mission_name_list = mission_name.split("\n")
     mission_names: dict[int, Any] = {}
     for mission_name in mission_name_list:
         line_data = mission_name.split(helper.get_text_splitter(is_jp))
         if helper.check_int(line_data[0]) is None:
@@ -113,19 +113,19 @@
     if names is None or conditions is None:
         return save_stats
 
     mission_ids_to_use, names_to_use = get_mission_ids(missions, conditions, names)
 
     ids = user_input_handler.select_not_inc(
         options=names_to_use,
-        mode="complete",
+        mode="완벽한",
     )
     re_claim = (
         user_input_handler.colored_input(
-            "이미 받은 미션&(1)&(보상을 다시 받을 수 있음)을 다시 완료하시겠습니까, 아니면 요청하지 않은 미션만 완료하시겠습니까&(2)&:"
+            "이미 요청한 미션 &(1)&(보상을 다시 받을 수 있음)을 다시 완료하시겠습니까, 아니면 요청하지 않은 미션만 완료하시겠습니까&(2)&:"
         )
         == "1"
     )
     missions = set_missions(missions, ids, conditions, mission_ids_to_use, re_claim)
     save_stats["missions"] = missions
     print("성공적으로 완료된 임무")
     return save_stats
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/other/play_time.py` & `Shark sac Korean editor-1.1.2/modkr/edits/other/play_time.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     """Handler for editting play time"""
     play_time = save_stats["play_time"]
 
     hours = play_time["hh"]
     minutes = play_time["mm"]
 
     helper.colored_text(
-        f"현재 플레이 시간은 다음과 같습니다.: &{hours}& 시간과 &{minutes}& 분"
+        f"현재 플레이 시간: &{hours}& 시간&{minutes}& 분"
     )
     hours = helper.check_int_max(
         user_input_handler.colored_input("몇 시로 설정하시겠습니까?:")
     )
     minutes = helper.check_int_max(
         user_input_handler.colored_input("몇 분으로 설정하시겠습니까?:")
     )
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/other/scheme_item.py` & `Shark sac Korean editor-1.1.2/modkr/edits/other/scheme_item.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     Returns:
         list[list[int]]: The scheme data
     """
     scheme_data = game_data_getter.get_file_latest(
         "DataLocal", "schemeItemData.tsv", is_jp
     )
     if scheme_data is None:
-        helper.error_text("Failed to get scheme data")
+        helper.error_text("체계 데이터를 가져오지 못했습니다.")
         return []
 
     scheme_data_data = helper.parse_int_list_list(
         csv_handler.parse_csv(
             scheme_data.decode("utf-8"),
             delimeter="\t",
         )
@@ -56,15 +56,15 @@
 
 
 def get_scheme_names(is_jp: bool, scheme_data: list[list[int]]) -> dict[int, str]:
     """Get the scheme names"""
 
     file_data = game_data_getter.get_file_latest("resLocal", "localizable.tsv", is_jp)
     if file_data is None:
-        helper.error_text("Failed to get scheme names")
+        helper.error_text("체계 이름을 가져오지 못했습니다.")
         return {}
 
     localizable = csv_handler.parse_csv(
         file_data.decode("utf-8"),
         delimeter="\t",
     )
     names: dict[int, str] = {}
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/other/trade_progress.py` & `Shark sac Korean editor-1.1.2/modkr/edits/other/trade_progress.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,17 +31,17 @@
     )
     tickets.edit()
     trade_progress["Value"] = tickets.get_value() * 5
 
     storage, has_space = set_trade_progress_val(storage)
 
     if not has_space:
-        helper.colored_text("고양이 보관함이 가득 찼습니다. 공간 1개를 비워주세요!")
+        helper.colored_text("고양이 창고가 꽉 찼습니다. 1칸을 비워주세요!")
         return save_stats
 
     save_stats["cat_storage"] = storage
     save_stats["trade_progress"] = trade_progress
     helper.colored_text(
-        '이제 저장소로 이동하여 &"모두 사용"&을 누른 다음 &"티켓 교환"을 눌러야 합니다.&'
+        '이제 저장소로 이동하여 &"모두 사용"&을 누른 다음 &"티켓 교환"을 눌러야 합니다."&'
     )
 
     return save_stats
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/other/unlock_enemy_guide.py` & `Shark sac Korean editor-1.1.2/modkr/edits/other/unlock_enemy_guide.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,24 +16,24 @@
         == "2"
     )
     set_val = 1
     if not unlock:
         set_val = 0
     ids = user_input_handler.get_range(
         user_input_handler.colored_input(
-            "적 ID를 입력하십시오(ID를 찾으려면 적군 해제 명령 전투 고양이를 조회하십시오)(모든 범위를 얻으려면 &all&을 입력할 수 있습니다. 예: &1&-&50& 또는 공백으로 구분된 ID(예: &5 4 7&):"
+            "적 ID를 입력하십시오(ID를 찾으려면 적군 해제 명령 전투 고양이를 조회하십시오)(모든 범위를 얻으려면 &all&을 입력할 수 있습니다(예: &1&-&50& 또는 공백으로 구분된 ID(예: &5 4 7&))."
         ),
         total,
     )
 
     for enemy_id in ids:
         if enemy_id >= 2:
             enemy_id -= 2
         if enemy_id >= len(enemy_guide_stats):
-            print(f"Invalid enemy id: {enemy_id+2}")
+            print(f"유효하지 않은 적 ID: {enemy_id+2}")
             continue
         enemy_guide_stats[enemy_id] = set_val
     save_stats["enemy_guide"] = enemy_guide_stats
     if not unlock:
         print("적 가이드 항목을 성공적으로 제거했습니다.")
     else:
         print("적 가이드 항목을 성공적으로 잠금 해제했습니다.")
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/save_management/convert.py` & `Shark sac Korean editor-1.1.2/modkr/edits/save_management/convert.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from ... import helper, user_input_handler
 
 
 def convert_to_jp(save_stats: dict[str, Any]) -> dict[str, Any]:
     save_stats["version"] = "jp"
     save_stats["dst"] = False
 
-    helper.colored_text("jp로 변환된 데이터 저장", helper.GREEN)
+    helper.colored_text("변환된 데이터 저장 jp", helper.GREEN)
     return save_stats
 
 
 def convert_to_non_jp(save_stats: dict[str, Any], cc: str) -> dict[str, Any]:
     save_stats["version"] = cc
     save_stats["dst"] = True
 
@@ -26,23 +26,23 @@
         return convert_to_non_jp(save_stats, version)
 
 
 def convert_save(save_stats: dict[str, Any]) -> dict[str, Any]:
     gvs = ["en", "jp", "kr", "tw"]
 
     helper.colored_text(
-        "경고: 이로 인해 문제가 발생할 수 있으며 두 앱의 버전이 동일해야 합니다(예: 둘 다 12.1.0)!",
+        "경고: 이로 인해 문제가 발생할 수 있으며 두 앱의 버전이 동일해야 합니다(예: 둘 다 12.3)!",
         helper.RED,
     )
 
     if save_stats["version"] in gvs:
         gvs.remove(save_stats["version"])
 
     gv_index = (
         user_input_handler.select_single(
-            gvs, title="저장을 변환할 버전 선택:"
+            gvs, title="저장을 다음으로 변환할 버전을 선택하십시오."
         )
         - 1
     )
     gv = gvs[gv_index]
 
     return convert(save_stats, gv)
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/save_management/load.py` & `Shark sac Korean editor-1.1.2/modkr/edits/save_management/load.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,65 +9,65 @@
         "전송 및 확인 코드를 사용하여 게임에서 저장 데이터 다운로드",
         "파일에서 저장 파일 선택",
         "adb를 사용하여 루팅된 장치에서 저장을 가져옵니다.",
         "json에서 저장 데이터 불러오기",
     ]
     index = (
         user_input_handler.select_single(
-            options, title="저장 데이터를 가져오는 옵션을 선택하세요.:"
+            options, title="저장 데이터를 가져오는 옵션을 선택합니다."
         )
         - 1
     )
     save_path = handle_index(index)
     if not save_path:
         return save_stats
     helper.set_save_path(save_path)
     data = helper.load_save_file(save_path)
     save_stats = data["save_stats"]
     if save_path.endswith(".json"):
         input(
-            "저장 데이터가 json 형식인 것 같습니다. json 데이터를 로드하려면 json 옵션을 가져오기 위해 사용하십시오.\n계속하려면 Enter 키를 누르십시오...:"
+            "저장 데이터가 json 형식인 것 같습니다. json 데이터를 로드하려면 json 옵션을 가져오기 위해 사용하십시오.\n계속하려면 엔터 키를 누르십시오...:"
         )
     if not clear_tutorial.is_tutorial_cleared(save_stats):
         save_stats = clear_tutorial.clear_tutorial(save_stats)
     return save_stats
 
 
 def handle_index(index: int) -> Optional[str]:
     path = None
     if index == 0:
-        print("데이터 전송에 대한 세부 정보 입력:")
+        print("Enter details for data transfer:")
         path = server_handler.download_handler()
     elif index == 1:
-        print("저장 파일 선택:")
+        print("Select save file:")
         path = helper.select_file(
-            "세이브 파일 선택:",
+            "Select a save file:",
             helper.get_save_file_filetype(),
             initial_file=helper.get_save_path_home(),
         )
     elif index == 2:
-        print("세이브 풀링을 위한 세부 정보 입력:")
+        print("Enter details for save pulling:")
         game_versions = adb_handler.find_game_versions()
         if not game_versions:
             game_version = helper.ask_cc()
         else:
             index = (
                 user_input_handler.select_single(
-                    game_versions, "선택하다", "가져올 게임 버전 선택:", True
+                    game_versions, "Select", "Select a game version to pull from:", True
                 )
                 - 1
             )
             game_version = game_versions[index]
         path = adb_handler.adb_pull_save_data(game_version)
     elif index == 3:
-        print("저장 데이터 json 파일 선택")
+        print("Select save data json file")
         js_path = helper.select_file(
-            "저장 데이터 json 파일 선택",
+            "Select save data json file",
             [("Json", "*.json")],
             initial_file=helper.get_save_path_home() + ".json",
         )
         if js_path:
             path = helper.load_json_handler(js_path)
     else:
-        helper.colored_text("인식할 수 있는 옵션을 입력하세요.", base=helper.RED)
+        helper.colored_text("Please enter a recognised option", base=helper.RED)
         return None
     return path
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/save_management/other.py` & `Shark sac Korean editor-1.1.2/modkr/edits/save_management/other.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/save_management/save.py` & `Shark sac Korean editor-1.1.2/modkr/edits/save_management/save.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,55 +9,55 @@
     """Serialise the save data and exit"""
 
     save_data = serialise_save.start_serialize(save_stats)
     helper.write_save_data(
         save_data, save_stats["version"], helper.get_save_path(), True
     )
 
-    helper.check_tracker(save_stats, helper.get_save_path())
+    helper.check_managed_items(save_stats, helper.get_save_path())
 
     return save_stats
 
 
 def save_save(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Serialise the save data"""
 
     save_data = serialise_save.start_serialize(save_stats)
     helper.write_save_data(
         save_data, save_stats["version"], helper.get_save_path(), False
     )
 
-    helper.check_tracker(save_stats, helper.get_save_path())
+    helper.check_managed_items(save_stats, helper.get_save_path())
 
     return save_stats
 
 
 def save_and_push(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Serialise the save data and and push it to the game"""
 
     save_data = serialise_save.start_serialize(save_stats)
     save_data = patcher.patch_save_data(save_data, save_stats["version"])
     helper.write_file_bytes(helper.get_save_path(), save_data)
 
-    helper.check_tracker(save_stats, helper.get_save_path())
+    helper.check_managed_items(save_stats, helper.get_save_path())
 
     if not helper.is_android():
         adb_handler.adb_push_save_data(save_stats["version"], helper.get_save_path())
 
     return save_stats
 
 
 def save_and_push_rerun(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Serialise the save data and push it to the game and restart the game"""
 
     save_data = serialise_save.start_serialize(save_stats)
     save_data = patcher.patch_save_data(save_data, save_stats["version"])
     helper.write_file_bytes(helper.get_save_path(), save_data)
 
-    helper.check_tracker(save_stats, helper.get_save_path())
+    helper.check_managed_items(save_stats, helper.get_save_path())
 
     if not helper.is_android():
         adb_handler.adb_push_save_data(save_stats["version"], helper.get_save_path())
         adb_handler.rerun_game(save_stats["version"])
     else:
         root_handler.rerun_game(save_stats["version"])
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/edits/save_management/server_upload.py` & `Shark sac Korean editor-1.1.2/modkr/edits/save_management/server_upload.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Handler for server save management functions"""
 from typing import Any
 
-from ... import helper, serialise_save, server_handler
+from ... import helper, serialise_save, server_handler, user_info
 
 
 def upload_metadata(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Upload the metadata to the game server"""
 
     _, save_stats = server_handler.meta_data_upload_handler(
         save_stats, helper.get_save_path()
@@ -16,39 +16,47 @@
 def set_managed_items(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Set the managed items for the save stats"""
 
     data = server_handler.check_gen_token(save_stats)
     token = data["token"]
     save_stats = data["save_stats"]
     if token is None:
-        helper.colored_text("Error generating token")
+        helper.colored_text("토큰 생성 오류")
         return save_stats
     server_handler.update_managed_items(save_stats["inquiry_code"], token, save_stats)
     return save_stats
 
 
+def handle_upload_error(inquiry_code: str):
+    """Show an error message"""
+    info = user_info.UserInfo(inquiry_code)
+    info.set_auth_token("")
+    info.set_password("")
+    helper.colored_text(
+        "저장 데이터를 업로드하는 중 오류가 발생했습니다.\n다시 시도하십시오. 오류가 지속되면 #bug-reports에 신고해 주세요."
+    )
+
+
 def save_and_upload(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Serialise the save data, and upload it to the game server"""
 
     save_data = serialise_save.start_serialize(save_stats)
     save_data = helper.write_save_data(
         save_data, save_stats["version"], helper.get_save_path(), False
     )
     upload_data = server_handler.upload_handler(save_stats, helper.get_save_path())
     if upload_data is None:
-        helper.colored_text(
-            "Error uploading save data\nPlease report this in #bug-reports"
-        )
+        handle_upload_error(save_stats["inquiry_code"])
+        return save_stats
+    upload_data, save_stats = upload_data
+    inquiry_code = save_stats["inquiry_code"]
+    if upload_data is None:
+        handle_upload_error(inquiry_code)
         return save_stats
     if "transferCode" not in upload_data:
-        helper.colored_text(
-            "Error uploading save data\nPlease report this in #bug-reports"
-        )
-    if len(upload_data["transferCode"]) < 5:
-        helper.colored_text(
-            "Error uploading save data\nPlease report this in #bug-reports"
-        )
+        handle_upload_error(inquiry_code)
+        return save_stats
     else:
         helper.colored_text(f"이어하기 코드 : &{upload_data['transferCode']}&")
-        helper.colored_text(f"인증 코드 : &{upload_data['pin']}&")
+        helper.colored_text(f"확인 코드 : &{upload_data['pin']}&")
 
     return save_stats
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/feature_handler.py` & `Shark sac Korean editor-1.1.2/modkr/feature_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,21 +5,22 @@
 from . import (
     helper,
     user_input_handler,
     config_manager,
 )
 from .edits import basic, cats, gamototo, levels, other, save_management
 
+
 def fix_elsewhere_old(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Fix the elsewhere error using 2 save files"""
 
     main_token = save_stats["token"]
     main_iq = save_stats["inquiry_code"]
     input(
-        "다른 곳 오류가 없고 금지되지 않은 현재 게임 내 로드된 저장 파일을 선택하세요.\n 계속하려면 엔터 키를 누르세요.:"
+        "다른곳에 오류가 없고 금지되지 않은 현재 게임 내에서 로드된 저장 파일을 선택하십시오.\n계속하려면 엔터 키를 누르십시오."
     )
     new_path = helper.select_file(
         "클리어 세이브 파일 선택",
         helper.get_save_file_filetype(),
         helper.get_save_path(),
     )
     if not new_path:
@@ -36,142 +37,142 @@
     helper.colored_text(f"대체된 문의 코드: &{main_iq}& with &{new_iq}&")
     helper.colored_text(f"교체된 토큰: &{main_token}& with &{new_token}&")
     return save_stats
 
 
 FEATURES: dict[str, Any] = {
     "저장 관리": {
-        "저장 저장": save_management.save.save_save,
+        "저장하기": save_management.save.save_save,
         "변경 사항 저장 및 게임 서버에 업로드(전송 및 확인 코드 받기)": save_management.server_upload.save_and_upload,
         "변경 사항을 파일에 저장": save_management.save.save,
         "adb를 사용하여 변경 사항을 저장하고 저장 데이터를 게임에 푸시합니다(게임을 다시 열지 않음).": save_management.save.save_and_push,
         "adb를 사용하여 변경 사항을 저장하고 저장 데이터를 게임에 푸시(게임 다시 열기)": save_management.save.save_and_push_rerun,
         "저장 데이터를 json으로 내보내기": save_management.other.export,
         "adb로 저장 데이터 지우기(게임을 재설치하지 않고 새 계정을 생성하는 데 사용)": save_management.other.clear_data,
         "추적 금지 항목 업로드(저장 또는 종료 시 자동으로 수행됨)": save_management.server_upload.upload_metadata,
         "세이브 데이터 불러오기": save_management.load.select,
         "저장 데이터를 다른 버전으로 변환": save_management.convert.convert_save,
         # "Manage Presets": preset_handler.preset_manager,
     },
-    "아이템": {
+    "아이템류": {
         "통조림": basic.basic_items.edit_cat_food,
         "경험치": basic.basic_items.edit_xp,
-        "티켓": {
-            "일반 티켓": basic.basic_items.edit_normal_tickets,
-            "희귀 티켓": basic.basic_items.edit_rare_tickets,
-            "플래티넘 티켓": basic.basic_items.edit_platinum_tickets,
-            "플래티넘 조각": basic.basic_items.edit_platinum_shards,
+        "티켓류": {
+            "노말 티켓": basic.basic_items.edit_normal_tickets,
+            "레어 티켓": basic.basic_items.edit_rare_tickets,
+            "플레티넘 티켓": basic.basic_items.edit_platinum_tickets,
+            "플레티넘 조각": basic.basic_items.edit_platinum_shards,
             "레전드 티켓": basic.basic_items.edit_legend_tickets,
         },
         "NP": basic.basic_items.edit_np,
         "리더쉽": basic.basic_items.edit_leadership,
-        "전투 아이템": basic.basic_items.edit_battle_items,
+        "배틀 아이템": basic.basic_items.edit_battle_items,
         "캣츠아이": basic.catseyes.edit_catseyes,
         "개다래 / 베히모스 스톤": basic.catfruit.edit_catfruit,
-        "본능구슬": basic.talent_orbs_new.edit_talent_orbs,
+        "본능 구슬": basic.talent_orbs_new.edit_talent_orbs,
         "가마토토 드링크": basic.basic_items.edit_catamins,
         "아이템구성 (금지할 수 없는 아이템을 얻을 수 있음)": other.scheme_item.edit_scheme_data,
     },
     "가마토토 / 오토토": {
         "오토토 조수": basic.basic_items.edit_engineers,
-        "오토토 기본 재료": basic.ototo_base_mats.edit_base_mats,
+        "오토토 재료": basic.ototo_base_mats.edit_base_mats,
         "가마토토 드링크": basic.basic_items.edit_catamins,
-        "가마토토 경험치/ 레벨": gamototo.gamatoto_xp.edit_gamatoto_xp,
+        "가마토토 경험치 / 레벨": gamototo.gamatoto_xp.edit_gamatoto_xp,
         "오토토 대포": gamototo.ototo_cat_cannon.edit_cat_cannon,
-        "가마토토 조수": gamototo.helpers.edit_helpers,
-        "가마토토 때려서 오류 고치기": gamototo.fix_gamatoto.fix_gamatoto,
+        "가마토토 도우미": gamototo.helpers.edit_helpers,
+        "충돌 하는 가마토토 오류 수정하기": gamototo.fix_gamatoto.fix_gamatoto,
     },
-    "냥코 / 특수 기술 ": {
-        "냥코 얻다 / 삭제 ": {
-            "냥코 캐릭터를 얻다": cats.get_remove_cats.get_cat,
-            "냥코 캐릭터를 삭제": cats.get_remove_cats.remove_cats,
-        },
-        "업글레이드 냥코캐릭터": cats.upgrade_cats.upgrade_cats,
-        "진정한 형태의 캐틱터얻기": {
-            "진정한 냥코캐릭터 얻기": cats.evolve_cats.get_evolve,
-            "진정한 냥코캐릭터 삭제": cats.evolve_cats.remove_evolve,
-            "강제로 진정한 형태의 고양이 (진정한 형태가 없는 캐릭터를 위한 빈 캐릭터로 이어질 것입니다.)": cats.evolve_cats.get_evolve_forced,
+    "고양이 / 스페셜 스킬[지갑]": {
+        "고양이를 추가 / 고양이를 제거 ": {
+            "➕고양이추가": cats.get_remove_cats.get_cat,
+            "➖고양이제거": cats.get_remove_cats.remove_cats,
+        },
+        "고양이 업그레이드": cats.upgrade_cats.upgrade_cats,
+        "고양이 진화시키기[3진]": {
+            "고양이 3진화 추가": cats.evolve_cats.get_evolve,
+            "고양이 3진화 제거": cats.evolve_cats.remove_evolve,
+            "강제로 진정한 형태의 고양이[냥코id코드로 추가]\n[⚠️모든 고양이 선택 금지] (진정한 형태가 없는 캐릭터를 위한 빈 캐릭터로 이어질 것입니다.)": cats.evolve_cats.get_evolve_forced,
         },
         "본능": {
-            "선택한 각 고양이의 재능을 개별적으로 설정": cats.talents.edit_talents_individual,
-            "최대 / 선택된 모든 고양이 재능 제거": cats.talents.max_all_talents,
+            "선택한 각 고양이의 본능을 개별적으로 설정": cats.talents.edit_talents_individual,
+            "최대 / 선택된 모든 고양이 본능 제거": cats.talents.max_all_talents,
         },
         "고양이 가이드 수집/제거": {
             "고양이 가이드 항목 설정(참조하지 않음)": cats.clear_cat_guide.collect_cat_guide,
-            "고양이 가이드 항목 설정 취소": cats.clear_cat_guide.remove_cat_guide,
+            "고양이 가이드 항목 청구 취소": cats.clear_cat_guide.remove_cat_guide,
         },
-        '스테이지 단위 드랍을 가져오면 이 스테이지를 클리어하여 특별한 고양이 대화 상자를 제거합니다[안씀].': cats.chara_drop.get_character_drops,
-        "특수 기술/능력 업그레이드[안씀]": cats.upgrade_blue.upgrade_blue,
+        ##'스테이지 단위 드랍을 가져오면 이 스테이지를 클리어하여 특별한 고양이 대화 상자를 제거합니다[안씀]': cats.chara_drop.get_character_drops,
+        "특수 기술/능력 업그레이드": cats.upgrade_blue.upgrade_blue,
     },
     "레벨 / 보물": {
-        "메인 스토리 챕터 클리어/노클리어": {
+        "메인 스토리 챕터 클리어/언클리어": {
             "선택한 모든 챕터의 모든 챕터에서 각 스테이지 클리어": levels.main_story.clear_all,
             "선택한 각 챕터의 모든 챕터에서 각 스테이지 클리어": levels.main_story.clear_each,
         },
         "보물": {
-            "보물 그룹 (예: 에너지 드링크, 아쿠아 크리스탈 등)": levels.treasures.treasure_groups,
+            "트레저 그룹 (예: 에너지 드링크, 아쿠아 크리스탈 등)": levels.treasures.treasure_groups,
             "개별적으로 특정 단계 및 특정 챕터": levels.treasures.specific_stages,
             "특정 스테이지와 챕터를 한 번에": levels.treasures.specific_stages_all_chapters,
         },
-        "좀비 스테이지 / 바이러스": levels.outbreaks.edit_outbreaks,
+        "좀비스테이지 / 노출": levels.outbreaks.edit_outbreaks,
         "이벤트 스테이지": levels.event_stages.event_stages,
-        "레전드리 스토리": levels.event_stages.stories_of_legend,
-        "신레전드리 스토리": levels.uncanny.edit_uncanny,
+        "레전드 스토리": levels.event_stages.stories_of_legend,
+        "신 레전드스토리": levels.uncanny.edit_uncanny,
         "마계편 스테이지/게이트 클리어": levels.aku.edit_aku,
         "마계편 스테이지/게이트 잠금 해제": levels.unlock_aku_realm.unlock_aku_realm,
-        "건틀릿[한국냥코사용불가]": levels.gauntlet.edit_gauntlet,
-        "콜라보 건틀릿[한국냥코사용불가]": levels.gauntlet.edit_collab_gauntlet,
+        ##"Gauntlets": levels.gauntlet.edit_gauntlet,
+        ##"Collab Gauntlets": levels.gauntlet.edit_collab_gauntlet,
         "타워": levels.towers.edit_tower,
         "레전드리스토리[빅 하앜마양 강림 클리어]": levels.behemoth_culling.edit_behemoth_culling,
         "미래편 시간 초과 점수": levels.itf_timed_scores.timed_scores,
         "도전 전투 점수": basic.basic_items.edit_challenge_battle,
         "튜토리얼 클리어": levels.clear_tutorial.clear_tutorial,
         "랭킹 점수(입문자의 전당)": basic.basic_items.edit_dojo_score,
         "수수께끼 단계 추가": levels.enigma_stages.edit_enigma_stages,
-        "필리버스터 단계 재청산 허용": levels.allow_filibuster_clearing.allow_filibuster_clearing,
+        "필리버스터 단계 언클리어": levels.allow_filibuster_clearing.allow_filibuster_clearing,
         "레전드 퀘스트": levels.legend_quest.edit_legend_quest,
     },
     "계정 / 문의 코드 / 토큰 ": {
         "문의 코드": basic.basic_items.edit_inquiry_code,
         "토큰": basic.basic_items.edit_token,
         "다른 곳 오류 수정 / 계정 차단 해제": other.fix_elsewhere.fix_elsewhere,
-        "이전 수정 다른 곳 오류 / 계정 금지 해제(2개의 저장 파일 필요)": fix_elsewhere_old,
+        ##"이전 수정 다른 곳 오류 / 계정 금지 해제(2개의 저장 파일 필요)": fix_elsewhere_old,
         "새로운 조회 코드 및 토큰 생성": other.create_new_account.create_new_account,
     },
-    "다른": {
+    "기타": {
         "레어 가챠 씨앗": basic.basic_items.edit_rare_gacha_seed,
         "잠금 해제된 장비 슬롯": basic.basic_items.edit_unlocked_slots,
-        "재시작 팩 받기/ 귀환자 모드": basic.basic_items.edit_restart_pack,
+        "재시작 팩 받기/ 귀환자 모드\n[⚠️재시작팩 하실려면 먼저 하셔야됩니다\n아니면초기화됩니다]": basic.basic_items.edit_restart_pack,
         "냥코 메달": other.meow_medals.medals,
         "플레이 타임": other.play_time.edit_play_time,
         "적 가이드 항목 잠금 해제/제거": other.unlock_enemy_guide.enemy_guide,
-        "개다래 챌린지 / 임무": other.missions.edit_missions,
+        "개다레 챌린지 / 미션": other.missions.edit_missions,
         "일반 티켓 최대 거래 진행률(금지할 수 없는 희귀 티켓 허용)": other.trade_progress.set_trade_progress,
         "골드 패스 받기/제거": other.get_gold_pass.get_gold_pass,
         "클레임 / 모든 사용자 등급 보상 제거(아무 아이템도 주지 않음)": other.claim_user_rank_rewards.edit_rewards,
-        "냥코 신전 레벨 / 경험치": other.cat_shrine.edit_shrine_xp,
+        "고양이 신전 레벨 / 경험치[모르겟네요]": other.cat_shrine.edit_shrine_xp,
     },
     "수정": {
         "시간 오류 수정": other.fix_time_issues.fix_time_issues,
         "장비 메뉴 잠금 해제": other.unlock_equip_menu.unlock_equip,
         "튜토리얼 클리어": levels.clear_tutorial.clear_tutorial,
         "다른 곳 오류 수정 / 계정 차단 해제": other.fix_elsewhere.fix_elsewhere,
-        "오래된 다른 곳 수정 오류 / 계정 금지 해제(2개의 저장 파일 필요)": fix_elsewhere_old,
-        "게임 충돌에서 가마모토 수정": gamototo.fix_gamatoto.fix_gamatoto,
+        ##"이전 수정 다른 곳 오류 / 계정 금지 해제(2개의 저장 파일 필요)": fix_elsewhere_old,
+        "게임 충돌에서 가마토토 수정": gamototo.fix_gamatoto.fix_gamatoto,
     },
-    "구성 편집": {
-        "현지화 편집": config_manager.edit_locale,
-        "기본 국가 코드 편집": config_manager.edit_default_gv,
-        "기본 저장 경로 편집": config_manager.edit_default_save_file_path,
-        "고정 저장 경로 편집": config_manager.edit_fixed_save_path,
-       "에디터 설정 편집": config_manager.edit_editor_settings,
-        "시작 설정 편집": config_manager.edit_start_up_settings,
-        "변경 사항 저장 설정 편집": config_manager.edit_save_changes_settings,
-        "서버 설정 편집": config_manager.edit_server_settings,
-        "구성 경로 편집": config_manager.edit_config_path,
+    "에디터 편집[사용하지마세요]": {
+        "Edit LOCALIZATION": config_manager.edit_locale,
+        "Edit DEFAULT_COUNTRY_CODE": config_manager.edit_default_gv,
+        "Edit DEFAULT_SAVE_PATH": config_manager.edit_default_save_file_path,
+        "Edit FIXED_SAVE_PATH": config_manager.edit_fixed_save_path,
+        "Edit EDITOR settings": config_manager.edit_editor_settings,
+        "Edit START_UP settings": config_manager.edit_start_up_settings,
+        "Edit SAVE_CHANGES settings": config_manager.edit_save_changes_settings,
+        "Edit SERVER settings": config_manager.edit_server_settings,
+        "Edit config path": config_manager.edit_config_path,
     },
     "종료": helper.exit_check_changes,
 }
 
 
 def get_feature(
     selected_features: Any, search_string: str, results: dict[str, Any]
@@ -189,26 +190,26 @@
 
 def show_options(
     save_stats: dict[str, Any], features_to_use: dict[str, Any]
 ) -> dict[str, Any]:
     """Allow the user to either enter a feature number or a feature name, and get the features that match"""
 
     if (
-       not config_manager.get_config_value_category("EDITOR", "SHOW_CATEGORIES")
+        not config_manager.get_config_value_category("EDITOR", "SHOW_CATEGORIES")
         and FEATURES == features_to_use
     ):
         user_input = ""
     else:
         prompt = (
             "무엇을 편집하시겠습니까(일부 옵션에는 다른 기능이 포함되어 있음)"
         )
         if config_manager.get_config_value_category(
-           "EDITOR", "SHOW_FEATURE_SELECT_EXPLANATION"
+            "EDITOR", "SHOW_FEATURE_SELECT_EXPLANATION"
         ):
-            prompt += "\n숫자를 입력하여 기능을 실행하거나 단어를 입력하여 해당 기능을 검색할 수 있습니다(예: catfood를 입력하면 통조림 기능이 실행되고 티켓을 입력하면 티켓을 편집하는 모든 기능이 표시됨)\nEnter를 눌러 목록을 볼 수 있습니다. 모든 기능의"
+            prompt += "\n숫자를 입력하여 기능을 실행하거나 단어를 입력하여 해당 기능을 검색할 수 있습니다(예: catfood를 입력하면 통조림 기능이 실행되고 티켓을 입력하면 티켓을 편집하는 모든 기능이 표시됨)\n엔터를 눌러 목록을 볼 수 있습니다. 모든 기능의"
         user_input = user_input_handler.colored_input(f"{prompt}:\n")
     user_int = helper.check_int(user_input)
     results = []
     if user_int is None:
         results = get_feature(features_to_use, user_input, {})
     else:
         if user_int < 1 or user_int > len(features_to_use) + 1:
@@ -222,15 +223,15 @@
             results = features_to_use[list(features_to_use)[user_int - 1]]
     if not isinstance(results, dict):
         save_stats_return = results(save_stats)
         if save_stats_return is None:
             return save_stats
         return save_stats_return
     if len(results) == 0:
-        helper.colored_text("해당 이름의 기능을 찾을 수 없습니다..", helper.RED)
+        helper.colored_text("해당 이름의 기능을 찾을 수 없습니다.", helper.RED)
         return menu(save_stats)
     if len(results) == 1 and isinstance(list(results.values())[0], dict):
         results = results[list(results)[0]]
     if len(results) == 1:
         save_stats_return = results[list(results)[0]](save_stats)
         if save_stats_return is None:
             return save_stats
@@ -239,15 +240,15 @@
     helper.colored_list(["뒤로가기"] + list(results))
     return show_options(save_stats, results)
 
 
 def menu(
     save_stats: dict[str, Any], path_save: Union[str, None] = None
 ) -> dict[str, Any]:
-    """메뉴를 표시하고 사용자가 편집할 기능을 선택할 수 있도록 합니다."""
+    """Show the menu and allow the user to select a feature to edit"""
 
     if path_save:
         helper.set_save_path(path_save)
     if config_manager.get_config_value_category("EDITOR", "SHOW_CATEGORIES"):
         helper.colored_list(list(FEATURES))
     save_stats = show_options(save_stats, FEATURES)
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/game_data_getter.py` & `Shark sac Korean editor-1.1.2/modkr/game_data_getter.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,55 +3,14 @@
 from typing import Optional
 import requests
 
 from . import helper
 
 URL = "https://raw.githubusercontent.com/fieryhenry/BCData/master/"
 
-def download_file_en_fix(
-    game_version: str,
-    pack_name: str,
-    file_name: str,
-    get_data: bool = True,
-    print_progress: bool = True,
-) -> bytes:
-    """
-    Downloads the file.
-
-    Args:
-        game_version (str): The game version to download from.
-        pack_name (str): The pack name to download from.
-        file_name (str): The file name to download.
-        get_data (bool, optional): Whether to return the data. Defaults to True.
-        print_progress (bool, optional): Whether to print the progress. Defaults to True.
-
-    Returns:
-        bytes: The data of the file.
-    """
-
-    path = helper.get_file(os.path.join("game_data", game_version, pack_name))
-    file_path = os.path.join(path, file_name)
-    if os.path.exists(file_path):
-        if get_data:
-            return helper.read_file_bytes(file_path)
-        return b""
-
-    if print_progress:
-        helper.colored_text(
-            f"Downloading game data file &{file_name}& from &{pack_name}& with game version &{game_version}&",
-            helper.GREEN,
-            helper.WHITE,
-        )
-    url = "https://raw.githubusercontent.com/cintagram/BCData_Fix/main/medallist.json"
-    response = requests.get(url)
-
-    helper.create_dirs(path)
-    helper.write_file_bytes(file_path, response.content)
-    return response.content
-
 
 def download_file(
     game_version: str,
     pack_name: str,
     file_name: str,
     get_data: bool = True,
     print_progress: bool = True,
@@ -75,15 +34,15 @@
     if os.path.exists(file_path):
         if get_data:
             return helper.read_file_bytes(file_path)
         return b""
 
     if print_progress:
         helper.colored_text(
-            f"Downloading game data file &{file_name}& from &{pack_name}& with game version &{game_version}&",
+            f"게임 데이터 파일 다운로드 중 &{file_name}& ~에서 &{pack_name}& 게임 버전으로 &{game_version}&",
             helper.GREEN,
             helper.WHITE,
         )
     url = URL + game_version + "/" + pack_name + "/" + file_name
     response = requests.get(url)
 
     helper.create_dirs(path)
@@ -138,31 +97,14 @@
         Optional[bytes]: The data of the file.
     """
     version = get_latest_version(is_jp)
     if version is None:
         return None
     return download_file(version, pack_name, file_name)
 
-def get_file_latest_fix(pack_name: str, file_name: str, is_jp: bool) -> Optional[bytes]:
-    """
-    Gets the latest version of the file.
-
-    Args:
-        pack_name (str): The pack name to find.
-        file_name (str): The file name to find.
-        is_jp (bool): Whether to get the japanese version.
-
-    Returns:
-        Optional[bytes]: The data of the file.
-    """
-    version = get_latest_version(is_jp)
-    if version is None:
-        return None
-    return download_file_en_fix(version, pack_name, file_name)
-
 
 def get_file_latest_path(path: str, is_jp: bool) -> Optional[bytes]:
     """
     Gets the latest version of the file.
 
     Args:
         path (str): The path to find.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/helper.py` & `Shark sac Korean editor-1.1.2/modkr/helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 
 from . import (
     user_input_handler,
     server_handler,
     patcher,
     serialise_save,
     parse_save,
-    tracker,
     config_manager,
+    user_info,
 )
 
 GREEN = "#008000"
 RED = "#FF0000"
 DARK_YELLOW = "#D7C32A"
 BLACK = "#000000"
 WHITE = "#FFFFFF"
@@ -56,14 +56,17 @@
 
     return [dir for dir in os.listdir(path) if os.path.isdir(os.path.join(path, dir))]
 
 
 def delete_dir(path: str) -> None:
     """Delete a directory and all of its contents"""
 
+    if not os.path.exists(path):
+        return
+
     for root, dirs, files in os.walk(path, topdown=False):
         for name in files:
             os.remove(os.path.join(root, name))
         for name in dirs:
             os.rmdir(os.path.join(root, name))
     os.rmdir(path)
 
@@ -124,21 +127,25 @@
 def get_local_files_path() -> str:
     """Get the local files path"""
 
     dir_path = os.path.join(os.path.dirname(os.path.realpath(__file__)), "files")
     return dir_path
 
 
-def read_file_string(file_path: str) -> str:
+def read_file_string(file_path: str, create: bool = False) -> str:
     """Reads a file and returns its contents as a string"""
 
     try:
         with open(file_path, "r", encoding="utf-8") as file:
             return file.read()
     except FileNotFoundError as err:
+        if create:
+            os.makedirs(os.path.dirname(file_path), exist_ok=True)
+            write_file_string(file_path, "")
+            return ""
         raise Exception("File not found: " + file_path) from err
     except UnicodeDecodeError as err:
         raise Exception("Error reading file: " + file_path + ": " + str(err)) from err
 
 
 def chunks(lst: list[Any], chunk_len: int) -> Generator[Any, Any, Any]:
     """Split list into chunks of n"""
@@ -299,14 +306,25 @@
 def write_file_string(file_path: str, data: str):
     """Write file as string"""
 
     with open(file_path, "w", encoding="utf-8") as file:
         file.write(data)
 
 
+def config_clamp(value: int, min: int, max: int, clamp_max_int: bool = True):
+    """Clamp a value between 0 and a max value"""
+
+    disable = config_manager.get_config_value_category("EDITOR", "DISABLE_MAXES")
+    if disable:
+        if clamp_max_int:
+            return clamp_int(value)
+        return value
+    return clamp(value, min, max)
+
+
 def check_clamp(
     values: Any, max_value: int, min_value: int = 0, offset: int = -1
 ) -> list[int]:
     """turn a list of strings into a list of ints and clamp them between a min and max"""
 
     if isinstance(values, str):
         values = [values]
@@ -402,28 +420,38 @@
     """Check if the save data is a Japanese save, checking the config file"""
 
     if config_manager.get_config_value_category("EDITOR", "ONLY_GET_EN_DATA"):
         return False
     return is_jp(save_stats)
 
 
-def check_tracker(save_stats: dict[str, Any], path: str) -> None:
-    """Check if the tracker is enabled"""
-    item_tracker = tracker.Tracker()
+def check_managed_items(save_stats: dict[str, Any], path: str) -> None:
+    """Check if the user has untracked bannable items"""
+    info = user_info.UserInfo(save_stats["inquiry_code"])
 
-    if item_tracker.has_data():
+    if info.has_managed_items():
         upload = (
             user_input_handler.colored_input(
-                "You have untracked bannable items that need to be uploaded. Do you want to upload them now? (&y&/&n&) (You will be unable to do so after exiting unless you have WIPE_TRACKED_ITEMS_ON_START set to False):"
+                "업로드해야 하는 추적되지 않은 금지 항목이 있습니다. 지금 업로드하시겠습니까? (&y&/&n&) (밴을 피하려면 &y&라고 말하는 것이 좋습니다):"
             )
             == "y"
         )
         if upload:
             server_handler.meta_data_upload_handler(save_stats, path)
-            colored_text("Uploaded meta data", new=GREEN)
+            colored_text("&Uploaded meta data", new=GREEN)
+        else:
+            delete = (
+                user_input_handler.colored_input(
+                    "항목 로그를 제거하시겠습니까? (&y&/&n&):"
+                )
+                == "y"
+            )
+            if delete:
+                info.clear_managed_items()
+                colored_text("&Removed item logs", new=GREEN)
 
 
 def exit_editor():
     """Exit the editor"""
 
     sys.exit(0)
 
@@ -470,18 +498,18 @@
         current_path = get_save_path()
         temp_file_path = os.path.join(
             config_manager.get_app_data_folder(), "SAVE_DATA_temp"
         )
         if os.path.exists(temp_file_path):
             data = read_file_bytes(temp_file_path)
             save_stats = parse_save.start_parse(data, get_country_code(data))
-            check_tracker(save_stats, temp_file_path)
+            check_managed_items(save_stats, temp_file_path)
             write_file_bytes(current_path, read_file_bytes(temp_file_path))
             colored_text(
-                f"Save data saved to &{current_path}&",
+                f"에 저장된 데이터 저장 &{current_path}&",
                 base=GREEN,
                 new=WHITE,
             )
 
 
 def are_identical_files(file1: str, file2: str) -> bool:
     """Check if two files are identical"""
@@ -490,15 +518,15 @@
 
 
 def check_cat_ids(cat_ids: list[int], save_stats: dict[str, Any]) -> list[int]:
     """Check if a list of cat ids is valid"""
     new_cat_ids: list[int] = []
     for cat_id in cat_ids:
         if cat_id > len(save_stats["cats"]) - 1:
-            colored_text(f"Invalid cat id {cat_id}", base=RED)
+            colored_text(f"잘못된 고양이 ID {cat_id}", base=RED)
             continue
         new_cat_ids.append(cat_id)
     return new_cat_ids
 
 
 def error_text(text: str):
     """Print error text"""
@@ -607,15 +635,15 @@
     if prompt:
         new_path = save_file("Save File", get_save_file_filetype(), path)
         if new_path is None:
             colored_text("Save cancelled", new=RED)
             return
         path = new_path
     write_file_bytes(path, save_data)
-    colored_text(f"저장 위치: &{os.path.abspath(path)}&", new=GREEN)
+    colored_text(f"Saved to: &{os.path.abspath(path)}&", new=GREEN)
     return save_data
 
 
 def select_dir(title: str, default_dir: str) -> str:
     """
     Select a directory from the user
 
@@ -743,14 +771,15 @@
     except PermissionError:
         print(
             colored_text(
                 "권한이 거부되었습니다. 파일이 사용 중이 아닌지 확인", base=RED
             )
         )
         exit_editor()
+        return
     return path_d.name
 
 
 def select_file(
     title: str,
     file_types: list[tuple[str, str]],
     default_dir: str = "",
@@ -834,27 +863,27 @@
     default_gv = config_manager.get_config_value("DEFAULT_COUNTRY_CODE")
     if default_gv:
         if len(default_gv) == 2:
             colored_text(f"기본 국가 코드 사용: &{default_gv}&")
             return default_gv
 
     country_code = user_input_handler.colored_input(
-        "국가 코드를 입력하세요(&en&, &jp&, &kr&, &tw&):"
+        "국가 코드를 입력하세요 (&en&, &jp&, &kr&, &tw&):"
     )
     return country_code
 
 
 def export_json(save_stats: dict[str, Any], path: str) -> None:
     """Export the save stats to a json file"""
 
     ordered_data = parse_save.re_order(save_stats)
     if os.path.isdir(path):
         path = os.path.join(path, f"{get_save_path_home()}.json")
     write_file_string(path, json.dumps(ordered_data, indent=4))
-    colored_text(f"json을 성공적으로 작성했습니다. &{os.path.abspath(path)}&")
+    colored_text(f"json을 성공적으로 작성했습니다.&{os.path.abspath(path)}&")
 
 
 def load_json_handler(json_path: str) -> Union[None, str]:
     """Load a save_data json file and serialise it"""
 
     save_stats = load_json(json_path)
     save_data = serialise_save.start_serialize(save_stats)
@@ -864,7 +893,21 @@
         get_save_file_filetype(),
         os.path.join(os.path.dirname(json_path), get_save_path_home()),
     )
     if path is None:
         return None
     write_file_bytes(path, save_data)
     return path
+
+
+def format_text(text: list[str]) -> list[str]:
+    for i, order in enumerate(text):
+        if order.startswith("bcsfe:"):
+            try:
+                counter = int(order.split(":")[1])
+            except ValueError:
+                counter = 0
+            text[i] = f"bcsfe:{counter + 1}"
+            break
+    else:
+        text.append("bcsfe:1")
+    return text
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/item.py` & `Shark sac Korean editor-1.1.2/modkr/item.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,27 @@
 from typing import Optional, Union
-from . import managed_item, user_input_handler, helper, locale_handler, tracker
+from . import (
+    managed_item,
+    user_input_handler,
+    helper,
+    locale_handler,
+    config_manager,
+    user_info,
+)
 
 
 class Bannable:
-    def __init__(self, type: "managed_item.ManagedItemType", work_around: str = ""):
+    def __init__(
+        self,
+        type: "managed_item.ManagedItemType",
+        inquiry_code: str,
+        work_around: str = "",
+    ):
         self.type = type
+        self.inquiry_code = inquiry_code
         self.work_around = work_around
 
 
 class Int:
     def __init__(self, value: Optional[int], byte_size: int = 4, signed: bool = True):
         self.value = value
         self.byte_size = byte_size
@@ -27,15 +40,20 @@
         value: Int,
         max_value: Optional[int],
         bannable: Optional[Bannable] = None,
         offset: int = 0,
     ):
         self.name = name
         self.__value = value
+        disable_maxes = config_manager.get_config_value_category(
+            "EDITOR", "DISABLE_MAXES"
+        )
         self.max_value = max_value
+        if disable_maxes:
+            self.max_value = None
         self.bannable = bannable
         self.offset = offset
         self.locale_manager = locale_handler.LocalManager.from_config()
 
     def get_max_value(self) -> int:
         if self.max_value is not None:
             return self.max_value
@@ -77,18 +95,17 @@
                 self.get_value_off(),
             )
         )
         if self.bannable is not None and self.__value.value != original_value:
             new_value = self.__value.value
             if original_value is None:
                 original_value = 0
-            item_tracker = tracker.Tracker()
-            item_tracker.update_tracker(
-                self.__value.value - original_value, self.bannable.type
-            )
+
+            info = user_info.UserInfo(self.bannable.inquiry_code)
+            info.update_item(self.bannable.type, self.__value.value - original_value)
 
     def get_value_off(self) -> int:
         if self.__value.value is None:
             return 0
         return self.__value.value + self.offset
 
     def get_value(self) -> int:
@@ -147,16 +164,16 @@
                 self.locale_manager.search_key("enter_value_text")
                 % (self.group_name, max_str)
             )
             new_value -= offset
             entered_value = helper.clamp(new_value, 0, max_value)
             for id in ids:
                 max_value = self.items[id].get_max_value()
-                new_value = helper.clamp(new_value, 0, max_value)
-                self.items[id].set_value(new_value)
+                value = helper.clamp(new_value, 0, max_value)
+                self.items[id].set_value(value)
 
             helper.colored_text(
                 self.locale_manager.search_key("success_set")
                 % (self.group_name, entered_value + offset)
             )
 
     def get_max_max_value(self) -> int:
@@ -169,18 +186,22 @@
         maxes: Union[list[int], int, None],
         group_name: str,
         offset: int = 0,
     ) -> "IntItemGroup":
         items: list[IntItem] = []
         for i in range(len(names)):
             max_value = maxes[i] if isinstance(maxes, list) else maxes
+            try:
+                value = values[i] if values is not None else None
+            except IndexError:
+                value = None
             items.append(
                 IntItem(
                     names[i],
-                    Int(values[i]) if values is not None else Int(None),
+                    Int(value),
                     max_value,
                     offset=offset,
                 )
             )
         return IntItemGroup(group_name, items)
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/locale_handler.py` & `Shark sac Korean editor-1.1.2/modkr/locale_handler.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.1/modkr/managed_item.py` & `Shark sac Korean editor-1.1.2/modkr/managed_item.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.1/modkr/parse_save.py` & `Shark sac Korean editor-1.1.2/modkr/parse_save.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Handler for parsing the save file"""
 
 import collections
 import datetime
+import enum
 import json
 import struct
 import traceback
 from typing import Any, Optional, Union
 
 
 from . import helper
@@ -39,19 +40,19 @@
     address = val
 
 
 def next_int_len(number: int) -> dict[str, int]:
     """Get the next int of a specified byte length from the save file"""
 
     if number < 0:
-        raise Exception("Invalid number")
+        raise Exception("잘못된 번호")
     if save_data_g is None:
-        raise Exception("Invalid save data")
+        raise Exception("잘못된 저장 데이터")
     if number > len(save_data_g):
-        raise Exception("Byte length is greater than the length of the save data")
+        raise Exception("바이트 길이가 저장 데이터의 길이보다 큽니다.")
     val = convert_little(save_data_g[address : address + number])
     data: dict[str, int] = {}
     set_address(address + number)
     data["Value"] = val
     data["Length"] = number
     return data
 
@@ -122,37 +123,36 @@
     time = datetime.datetime(year, month, day, hour, minute, second)
     return time.isoformat()
 
 
 def get_length_data(
     length_bytes: int = 4, separator: int = 4, length: Union[int, None] = None
 ) -> list[int]:
-
     data: list[int] = []
     if length is None:
         length = next_int(length_bytes)
     if save_data_g is None:
-        raise Exception("Invalid save data")
+        raise Exception("잘못된 저장 데이터")
     if length > len(save_data_g):
-        raise Exception("Length too large")
+        raise Exception("길이가 너무 큼")
     for _ in range(length):
         data.append(next_int(separator))
     return data
 
 
 def get_length_doubles(
     length_bytes: int = 4, length: Union[int, None] = None
 ) -> list[float]:
     data: list[float] = []
     if length is None:
         length = next_int(length_bytes)
     if save_data_g is None:
-        raise Exception("Invalid save data")
+        raise Exception("잘못된 저장 데이터")
     if length > len(save_data_g):
-        raise Exception("Length too large")
+        raise Exception("길이가 너무 큼")
     for _ in range(length):
         data.append(get_double())
     return data
 
 
 def get_equip_slots() -> list[list[int]]:
     length = next_int(1)
@@ -266,15 +266,15 @@
     stars_per_sub_chapter = next_int(1)
     stages_per_sub_chapter = next_int(1)
 
     clear_progress = get_length_data(1, 1, total_sub_chapters * stars_per_sub_chapter)
     clear_progress = list(helper.chunks(clear_progress, stars_per_sub_chapter))
 
     return {
-        "클리어": clear_progress,
+        "Clear": clear_progress,
         "unknown": unknown_val,
         "total": total_sub_chapters,
         "stages": stages_per_sub_chapter,
         "stars": stars_per_sub_chapter,
     }
 
 
@@ -497,33 +497,35 @@
 
         val_2 = next_int_len(1)
         data.append(val_2)
 
     return data
 
 
-def get_cat_cannon_data() -> dict[int, dict[str, int]]:
+def get_cat_cannon_data() -> dict[int, dict[str, Any]]:
     length = next_int(4)
-    cannon_data: dict[int, dict[str, int]] = {}
+    cannon_data: dict[int, dict[str, Any]] = {}
     for _ in range(length):
-        cannon = {"level": 0, "unlock_flag": 0}
+        cannon: dict[str, Any] = {}
         cannon_id = next_int(4)
         len_val = next_int(4)
         unlock_flag = next_int(4)
-        level = next_int(4)
-        extra_1 = 0
-        extra_2 = 0
+        effect_level = next_int(4)
+        foundation_level = 0
+        style_level = 0
         if len_val == 4:
-            extra_1 = next_int(4)
-            extra_2 = next_int(4)
-        cannon["level"] = level
+            foundation_level = next_int(4)
+            style_level = next_int(4)
+        cannon["levels"] = {
+            "effect": effect_level,
+            "foundation": foundation_level,
+            "style": style_level,
+        }
         cannon["unlock_flag"] = unlock_flag
         cannon["len_val"] = len_val
-        cannon["extra_1"] = extra_1
-        cannon["extra_2"] = extra_2
         cannon_data[cannon_id] = cannon
     return cannon_data
 
 
 def get_data_near_ht() -> list[dict[str, int]]:
     data: list[dict[str, int]] = []
 
@@ -782,15 +784,15 @@
         next_int(4)
         raise Exception("Invalid total subchapters")
     else:
         clear_progress = get_length_data(4, 4, total_subchapters * stars)
     clear_progress = list(helper.chunks(clear_progress, stars))
 
     return {
-        "클리어": clear_progress,
+        "Clear": clear_progress,
         "total": total_subchapters,
         "stages": stages_per_subchapter,
         "stars": stars,
     }
 
 
 def get_event_timed_scores() -> dict[str, Any]:
@@ -999,15 +1001,15 @@
     stages_per_subchapter = next_int(1)
     stars = next_int(1)
 
     clear_progress = get_length_data(4, 1, total_subchapters * stars)
     clear_progress = list(helper.chunks(clear_progress, stars))
 
     return {
-        "클리어": clear_progress,
+        "Clear": clear_progress,
         "total": total_subchapters,
         "stages": stages_per_subchapter,
         "stars": stars,
     }
 
 
 def get_legend_quest_progress(lengths: dict[str, Any]):
@@ -1089,15 +1091,15 @@
     stages_per_subchapter = next_int(1)
     stars = next_int(1)
 
     clear_progress = get_length_data(4, 1, total_subchapters * stars)
     clear_progress = list(helper.chunks(clear_progress, stars))
 
     return {
-        "클리어": clear_progress,
+        "Clear": clear_progress,
         "total": total_subchapters,
         "stages": stages_per_subchapter,
         "stars": stars,
     }
 
 
 def get_gauntlet_progress(
@@ -1577,14 +1579,15 @@
                 f"\nThis save is from before &11.0.0& (current save version is &{helper.gv_to_str(game_version)}&), so this is likely the cause for the issue. &The save editor is not designed to work with saves from before 11.0.0&"
             )
         else:
             helper.colored_text(
                 "\nPlease report this to &#bug-reports&, and/or &dm me your save& on discord"
             )
         helper.exit_editor()
+        return {}
     return save_stats
 
 
 def get_game_version(save_data: bytes) -> int:
     """Get the game version from the save data."""
 
     return convert_little(save_data[0:3])
@@ -1724,21 +1727,170 @@
         elif value_type == bool:
             data[key] = next_int(1) == 1
         else:
             raise Exception("Invalid value type")
     return data
 
 
+class BackupState(enum.Enum):
+    IDLE = 0
+    GO_TO_CAN_BACKUP = 1
+    IN_CAN_BACKUP = 2
+    GO_TO_CHECK_BAN = 3
+    IN_CHECK_BAN = 4
+    GO_TO_BACKUP = 5
+    IN_BACKUP = 6
+    FINISHED = 7
+
+
+def get_110900_data() -> list[dict[str, int]]:
+    data: list[dict[str, int]] = []
+
+    data.append(next_int_len(4))
+    data.append(next_int_len(2))
+    data.append(next_int_len(1))
+    data.append(next_int_len(1))
+    data.append(next_int_len(1))
+    data.append(next_int_len(1))
+
+    ivar_14 = next_int_len(1)
+    data.append(ivar_14)
+
+    for _ in range(ivar_14["Value"]):
+        data.append(next_int_len(2))
+
+    svar6 = next_int_len(2)
+    data.append(svar6)
+
+    for _ in range(svar6["Value"]):
+        data.append(next_int_len(2))
+
+    svar6 = next_int_len(2)
+    data.append(svar6)
+
+    for _ in range(svar6["Value"]):
+        data.append(next_int_len(2))
+
+    data.append(next_int_len(4))
+    data.append(next_int_len(4))
+    data.append(next_int_len(4))
+    data.append(next_int_len(2))
+    data.append(next_int_len(2))
+    data.append(next_int_len(2))
+    data.append(next_int_len(2))
+    data.append(next_int_len(1))
+    data.append(next_int_len(1))
+    data.append(next_int_len(1))
+    data.append(next_int_len(1))
+    data.append(next_int_len(1))
+    data.append(next_int_len(1))
+    data.append(next_int_len(1))
+    data.append(next_int_len(1))
+    svar6 = next_int_len(2)
+    data.append(svar6)
+
+    for _ in range(svar6["Value"]):
+        data.append(next_int_len(2))
+
+    data.append(next_int_len(1))
+    data.append(next_int_len(1))
+    data.append(next_int_len(1))
+    data.append(next_int_len(1))
+    data.append(next_int_len(1))
+    data.append(next_int_len(1))
+    data.append(next_int_len(1))
+    data.append(next_int_len(1))
+    data.append(next_int_len(1))
+    data.append(next_int_len(1))
+    data.append(next_int_len(1))
+    data.append(next_int_len(1))
+    data.append(next_int_len(1))
+    data.append(next_int_len(1))
+
+    cvar4 = next_int_len(1)
+    data.append(cvar4)
+    if 0 < cvar4["Value"]:
+        data.append(next_int_len(2))
+        if cvar4["Value"] != 1:
+            data.append(next_int_len(2))
+            if cvar4["Value"] != 2:
+                data.append(next_int_len(2))
+                if cvar4["Value"] != 3:
+                    data.append(next_int_len(2))
+                    if cvar4["Value"] != 4:
+                        ivar32 = cvar4["Value"] + 4
+                        for _ in range(ivar32):
+                            data.append(next_int_len(2))
+    return data
+
+
+def get_zero_legends() -> list[Any]:
+    total_chapters = next_int(2)
+    chapters: list[dict[str, Any]] = []
+    for _ in range(total_chapters):
+        unknown_1 = next_int(1)
+        total_stars = next_int(1)
+        stars: list[dict[str, Any]] = []
+        for _ in range(total_stars):
+            selected_stage = next_int(1)
+            stages_cleared = next_int(1)
+            unlock_next = next_int(1)
+            total_stages = next_int(2)
+            stages: list[Any] = []
+            for _ in range(total_stages):
+                clear_amount = next_int(2)
+                stages.append(clear_amount)
+            stars.append(
+                {
+                    "selected_stage": selected_stage,
+                    "stages_cleared": stages_cleared,
+                    "unlock_next": unlock_next,
+                    "stages": stages,
+                }
+            )
+        chapters.append(
+            {
+                "unknown_1": unknown_1,
+                "stars": stars,
+            }
+        )
+    return chapters
+
+
+def get_120100_data() -> list[dict[str, int]]:
+    data: list[dict[str, int]] = []
+    svar19 = next_int_len(2)
+    data.append(svar19)
+    for _ in range(svar19["Value"]):
+        data.append(next_int_len(2))
+
+    return data
+
+
+def get_120200_data() -> list[dict[str, int]]:
+    data: list[dict[str, int]] = []
+    data.append(next_int_len(1))
+    data.append(next_int_len(2))
+    cvar4 = next_int_len(1)
+    data.append(cvar4)
+    for _ in range(cvar4["Value"]):
+        data.append(next_int_len(2))
+        data.append(next_int_len(2))
+
+    return data
+
+
 def parse_save(
     save_data: bytes,
     country_code: Union[str, None],
     dst: Optional[bool] = None,
 ) -> dict[str, Any]:
     """Parse the save data."""
-
+    if country_code == "ja" or country_code == "":
+        country_code = "jp"
     set_address(0)
     global save_data_g
     save_data_g = save_data
     save_stats: dict[str, Any] = {}
     save_stats["editor_version"] = updater.get_local_version()
 
     save_stats["game_version"] = next_int_len(4)
@@ -2319,15 +2471,40 @@
     save_stats["unknown_129"] = get_110800_data()
 
     save_stats["dojo_3x_speed"] = next_int_len(1)
 
     save_stats["unknown_132"] = get_110800_data_2()
 
     save_stats["gv_110800"] = next_int_len(4)  # 110800
-    save_stats = check_gv(save_stats, 110800)
+    save_stats = check_gv(save_stats, 110900)
+    if save_stats["exit"]:
+        return save_stats
+
+    save_stats["unknown_135"] = get_110900_data()
+    save_stats["gv_110900"] = next_int_len(4)  # 110900
+    save_stats = check_gv(save_stats, 120000)
+    if save_stats["exit"]:
+        return save_stats
+
+    save_stats["zero_legends"] = get_zero_legends()
+    save_stats["unknown_136"] = next_int_len(1)
+    save_stats["gv_120000"] = next_int_len(4)  # 120000
+    save_stats = check_gv(save_stats, 120100)
+    if save_stats["exit"]:
+        return save_stats
+
+    save_stats["unknown_137"] = get_120100_data()
+    save_stats["gv_120100"] = next_int_len(4)  # 120100
+    save_stats = check_gv(save_stats, 120200)
+    if save_stats["exit"]:
+        return save_stats
+
+    save_stats["unknown_138"] = get_120200_data()
+    save_stats["gv_120200"] = next_int_len(4)  # 120200
+    save_stats = check_gv(save_stats, 120200)
     if save_stats["exit"]:
         return save_stats
 
     length = len(save_data) - address - 32
     save_stats["extra_data"] = next_int_len(length)
 
     save_stats = exit_parser(save_stats)
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/patcher.py` & `Shark sac Korean editor-1.1.2/modkr/patcher.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.1/modkr/root_handler.py` & `Shark sac Korean editor-1.1.2/modkr/root_handler.py`

 * *Files 14% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     """
     if not helper.is_android():
         return False
     try:
         os.listdir(get_data_path())
     except PermissionError:
         helper.colored_text(
-            "설치된 게임 버전을 얻으려면 루트 액세스가 필요합니다. 실행 명령 앞에 sudo를 추가해 보십시오.",
+            "Root access is required to get installed game versions. Try adding sudo before the run command",
             base=helper.RED,
         )
         return False
     return True
 
 
 def rerun_game(version: str) -> None:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/serialise_save.py` & `Shark sac Korean editor-1.1.2/modkr/serialise_save.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,16 +224,16 @@
     stages_per_sub_chapter = event_current["stages"]
 
     save_data = write(save_data, unknown_val, 1)
     save_data = write(save_data, total_sub_chapters, 2)
     save_data = write(save_data, stars_per_sub_chapter, 1)
     save_data = write(save_data, stages_per_sub_chapter, 1)
 
-    for i in range(len(event_current["클리어"])):
-        save_data = write_length_data(save_data, event_current["클리어"][i], 1, 1, False)
+    for i in range(len(event_current["Clear"])):
+        save_data = write_length_data(save_data, event_current["Clear"][i], 1, 1, False)
 
     return save_data
 
 
 def flatten_list(_2d_list: Union[list[list[Any]], list[Any]]) -> list[Any]:
     flat_list: list[Any] = []
     # Iterate through the outer list
@@ -311,35 +311,36 @@
     save_data = write(save_data, len(ototo_cannon), 4)
     for cannon_id in ototo_cannon:
         cannon = ototo_cannon[cannon_id]
 
         save_data = write(save_data, int(cannon_id), 4)
         save_data = write(save_data, cannon["len_val"], 4)
         save_data = write(save_data, cannon["unlock_flag"], 4)
-        save_data = write(save_data, cannon["level"], 4)
+        levels = cannon["levels"]
+        save_data = write(save_data, levels["effect"], 4)
         if cannon["len_val"] == 4:
-            save_data = write(save_data, cannon["extra_1"], 4)
-            save_data = write(save_data, cannon["extra_2"], 4)
+            save_data = write(save_data, levels["foundation"], 4)
+            save_data = write(save_data, levels["style"], 4)
     return save_data
 
 
 def serialise_uncanny_current(
     save_data: list[int], uncanny_current: dict[str, Any]
 ) -> list[int]:
     total_sub_chapters = uncanny_current["total"]
     stars_per_sub_chapter = uncanny_current["stars"]
     stages_per_sub_chapter = uncanny_current["stages"]
 
     save_data = write(save_data, total_sub_chapters, 4)
     save_data = write(save_data, stages_per_sub_chapter, 4)
     save_data = write(save_data, stars_per_sub_chapter, 4)
 
-    for i in range(len(uncanny_current["클리어"])):
+    for i in range(len(uncanny_current["Clear"])):
         save_data = write_length_data(
-            save_data, uncanny_current["클리어"][i], 4, 4, False
+            save_data, uncanny_current["Clear"][i], 4, 4, False
         )
 
     return save_data
 
 
 def serialise_event_timed_scores(
     save_data: list[int], timed_scores: dict[str, Any]
@@ -400,17 +401,17 @@
 def serialise_gauntlet_current(
     save_data: list[int], gauntlet_current: dict[str, Any]
 ) -> list[int]:
     save_data = write(save_data, gauntlet_current["total"], 2)
     save_data = write(save_data, gauntlet_current["stages"], 1)
     save_data = write(save_data, gauntlet_current["stars"], 1)
 
-    for i in range(len(gauntlet_current["클리어"])):
+    for i in range(len(gauntlet_current["Clear"])):
         save_data = write_length_data(
-            save_data, gauntlet_current["클리어"][i], 1, 1, False
+            save_data, gauntlet_current["Clear"][i], 1, 1, False
         )
 
     return save_data
 
 
 def serialise_gauntlet_progress(
     save_data: list[int], gauntlets: dict[str, Any]
@@ -442,17 +443,17 @@
 def serialise_legend_quest_current(
     save_data: list[int], legend_quest_current: dict[str, Any]
 ) -> list[int]:
     save_data = write(save_data, legend_quest_current["total"], 1)
     save_data = write(save_data, legend_quest_current["stages"], 1)
     save_data = write(save_data, legend_quest_current["stars"], 1)
 
-    for i in range(len(legend_quest_current["클리어"])):
+    for i in range(len(legend_quest_current["Clear"])):
         save_data = write_length_data(
-            save_data, legend_quest_current["클리어"][i], 1, 1, False
+            save_data, legend_quest_current["Clear"][i], 1, 1, False
         )
 
     return save_data
 
 
 def serialise_legend_quest_progress(
     save_data: list[int], legend_quests: dict[str, Any]
@@ -873,14 +874,40 @@
             save_data = write(save_data, value, 1)
         else:
             save_data = write(save_data, value, 4)
 
     return save_data
 
 
+def serialise_zero_legends(save_data: list[int], data: list[Any]):
+    """
+    Serialises the zero legends data
+
+    Args:
+        save_data (list[int]): The save data
+        data (list[Any]): The zero legends data
+    """
+    save_data = write(save_data, len(data), 2)
+    for chapter in data:
+        unknown_1 = chapter["unknown_1"]
+        save_data = write(save_data, unknown_1, 1)
+        save_data = write(save_data, len(chapter["stars"]), 1)
+        for star in chapter["stars"]:
+            selected_stage = star["selected_stage"]
+            stages_cleared = star["stages_cleared"]
+            unlock_next = star["unlock_next"]
+            save_data = write(save_data, selected_stage, 1)
+            save_data = write(save_data, stages_cleared, 1)
+            save_data = write(save_data, unlock_next, 1)
+            save_data = write(save_data, len(star["stages"]), 2)
+            for clear_amount in star["stages"]:
+                save_data = write(save_data, clear_amount, 2)
+    return save_data
+
+
 def serialize_save(save_stats: dict[str, Any]) -> bytes:
     """Serialises the save stats"""
 
     save_data: list[int] = []
 
     save_data = write(save_data, save_stats["game_version"])
 
@@ -1014,17 +1041,18 @@
     save_data = write_length_data(save_data, save_stats["unknown_105"], 4, 4, False)
 
     save_data = write_length_data(
         save_data, save_stats["unknown_107"], write_length=False, bytes_per_val=1
     )
     if save_stats["dst"]:
         save_data = serialise_utf8_string(save_data, save_stats["unknown_110"])
-    save_data = write(save_data, len(save_stats["unknown_108"]), 4)
-    for i in range(len(save_stats["unknown_108"])):
-        save_data = serialise_utf8_string(save_data, save_stats["unknown_108"][i])
+    unknown_108 = helper.format_text(save_stats["unknown_108"])
+    save_data = write(save_data, len(unknown_108), 4)
+    for i in range(len(unknown_108)):
+        save_data = serialise_utf8_string(save_data, unknown_108[i])
 
     if save_stats["dst"]:
         save_data = write_length_doubles(
             save_data, save_stats["time_stamps"], write_length=False
         )
 
         save_data = write(save_data, len(save_stats["unknown_112"]), 4)
@@ -1498,17 +1526,47 @@
     save_data = serialise_dumped_data(save_data, save_stats["unknown_129"])
 
     save_data = write(save_data, save_stats["dojo_3x_speed"])
 
     save_data = serialise_dumped_data(save_data, save_stats["unknown_132"])
 
     save_data = write(save_data, save_stats["gv_110800"])
-    data = check_gv(save_data, save_stats, 110800)
+    data = check_gv(save_data, save_stats, 110900)
+    save_data = data["save_data"]
+    if data["exit"]:
+        return bytes(save_data)
+
+    save_data = serialise_dumped_data(save_data, save_stats["unknown_135"])
+
+    save_data = write(save_data, save_stats["gv_110900"])
+    data = check_gv(save_data, save_stats, 120000)
     save_data = data["save_data"]
     if data["exit"]:
         return bytes(save_data)
 
+    save_data = serialise_zero_legends(save_data, save_stats["zero_legends"])
+
+    save_data = write(save_data, save_stats["unknown_136"])
+
+    save_data = write(save_data, save_stats["gv_120000"])
+    data = check_gv(save_data, save_stats, 120100)
+    save_data = data["save_data"]
+    if data["exit"]:
+        return bytes(save_data)
+
+    save_data = serialise_dumped_data(save_data, save_stats["unknown_137"])
+
+    save_data = write(save_data, save_stats["gv_120100"])
+    data = check_gv(save_data, save_stats, 120200)
+    save_data = data["save_data"]
+    if data["exit"]:
+        return bytes(save_data)
+
+    save_data = serialise_dumped_data(save_data, save_stats["unknown_138"])
+
+    save_data = write(save_data, save_stats["gv_120200"])
+
     save_data = write(save_data, save_stats["extra_data"])
 
     save_data = exit_serialiser(save_data, save_stats)
 
     return bytes(save_data)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/server_handler.py` & `Shark sac Korean editor-1.1.2/modkr/server_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,23 @@
 import json
 from random import randint
 import time
 from typing import Any, Optional, Union
 
 import requests
 
-from . import helper, managed_item, serialise_save, patcher, config_manager, tracker
+from . import (
+    helper,
+    managed_item,
+    serialise_save,
+    patcher,
+    config_manager,
+    user_info,
+    parse_save,
+)
 
 
 def get_current_time() -> int:
     """Get current time."""
 
     return int(time.time())
 
@@ -254,15 +262,15 @@
 
 
 def download_save(
     country_code: str,
     transfer_code: str,
     confirmation_code: str,
     game_version: str,
-) -> bytes:
+) -> requests.Response:
     """Downloads the save for the given country_code, transfer_code, confirmation_code
     and game_version"""
 
     country_code = country_code.replace("jp", "ja")
     url = get_nyanko_save_url() + "/v2/transfers/" + transfer_code + "/reception"
     data = get_client_info(country_code, game_version)
     data["pin"] = confirmation_code
@@ -275,15 +283,15 @@
         "connection": "keep-alive",
         "user-agent": "Dalvik/2.1.0 (Linux; U; Android 9; SM-G955F Build/N2G48B)",
     }
     try:
         response = requests.post(url, data=data_s, headers=headers)
     except requests.exceptions.RequestException as err:
         raise Exception("Error getting save: " + str(err)) from err
-    return response.content
+    return response
 
 
 def upload_save_data_body_v2(
     save_data: bytes,
     save_key_data: dict[str, Any],
 ) -> tuple[bytes, bytes]:
     """Returns the body for the upload save data request
@@ -579,115 +587,134 @@
 
 
 def check_gen_token(
     save_stats: dict[str, Any], path: Optional[str] = None
 ) -> dict[str, Any]:
     """Gets the account auth token"""
 
-    save_stats, password_refresh_data = check_gen_password(save_stats)
+    save_stats, password = check_gen_password(save_stats)
     inquiry_code = save_stats["inquiry_code"]
 
     save_data = None
 
     if path is not None:
         save_data = serialise_save.start_serialize(save_stats)
         save_data = patcher.patch_save_data(save_data, save_stats["version"])
         save_data = helper.write_file_bytes(path, save_data)
 
+    # token = get_auth_token_from_file(inquiry_code)
+    # if token is None:
     token = get_token(
         inquiry_code,
-        password_refresh_data["password"],
+        password,
         save_stats["version"],
         save_stats["game_version"]["Value"],
     )
 
+    info = user_info.UserInfo(inquiry_code)
+
+    info.set_auth_token("" if token is None else token)
+
     return {
         "token": token,
         "save_data": save_data,
         "inquiry_code": inquiry_code,
-        "password_refresh_data": password_refresh_data,
         "save_stats": save_stats,
     }
 
 
-def check_gen_password(
-    save_stats: dict[str, Any]
-) -> tuple[dict[str, Any], dict[str, str]]:
+def check_gen_password(save_stats: dict[str, Any]) -> tuple[dict[str, Any], str]:
     """Checks the password for the given save_stats and generates new if stuff is invalid"""
 
     inquiry_code = save_stats["inquiry_code"]
     password_refresh_token = save_stats["token"]
 
+    info = user_info.UserInfo(inquiry_code)
+
+    password = info.get_password()
+    if password:
+        return save_stats, password
+
     password_refresh_data = get_password_refresh(inquiry_code, password_refresh_token)
     if password_refresh_data is not None:
-        return save_stats, password_refresh_data
+        info.set_password(password_refresh_data["password"])
+        save_stats["token"] = password_refresh_data["passwordRefreshToken"]
+        return save_stats, password_refresh_data["password"]
 
     password_refresh_data = get_password(inquiry_code)
     if password_refresh_data is None:
         inquiry_code = get_inquiry_code()
         save_stats["inquiry_code"] = inquiry_code
 
         return check_gen_password(save_stats)
 
     if "accountCode" in password_refresh_data:
         save_stats["inquiry_code"] = password_refresh_data["accountCode"]
+        info = user_info.UserInfo(password_refresh_data["accountCode"])
 
     password_refresh_token = password_refresh_data["passwordRefreshToken"]
     save_stats["token"] = password_refresh_token
-    return save_stats, password_refresh_data
+    info.set_password(password_refresh_data["password"])
+    return save_stats, password_refresh_data["password"]
 
 
 def prepare_upload(
     save_stats: dict[str, Any],
     path: str,
     print_text: bool = True,
     managed_items: Optional[list[managed_item.ManagedItem]] = None,
-) -> Optional[tuple[str, Any, bytes, int, list[managed_item.ManagedItem]]]:
+) -> Optional[
+    tuple[str, Any, bytes, int, list[managed_item.ManagedItem], dict[str, Any]]
+]:
     """Handles the pre-upload of the save data"""
 
     original_iq = save_stats["inquiry_code"]
     if print_text:
-        helper.colored_text("Getting account password...", helper.GREEN)
+        helper.colored_text("계정 비밀번호를 가져오는 중...", helper.GREEN)
     data = check_gen_token(save_stats, path)
     token = data["token"]
     inquiry_code = data["inquiry_code"]
     save_data = data["save_data"]
+    save_stats = data["save_stats"]
+    info = user_info.UserInfo(inquiry_code)
     if token is None:
-        if print_text:
-            helper.colored_text(
-                "Error getting account auth token",
-                helper.RED,
-            )
-        return None
-    item_tracker = tracker.Tracker()
+        token = info.get_auth_token()
+        if not token:
+            info.set_password("")
+            if print_text:
+                helper.colored_text(
+                    "계정 인증 토큰을 가져오는 중에 오류가 발생했습니다. 다시 시도해 주세요. 이 오류가 지속되면 디스코드 서버에 신고해 주세요.",
+                    helper.RED,
+                )
+            return None
     if original_iq != inquiry_code:
-        item_tracker.reset_tracker()
+        info.clear_managed_items()
         update_managed_items(save_stats["inquiry_code"], token, save_stats)
 
     if print_text:
-        helper.colored_text("Adding meta data...", helper.GREEN)
+        helper.colored_text("메타 데이터 추가 중...", helper.GREEN)
     if managed_items is None:
-        managed_items = item_tracker.parse_tracker_managed()
+        managed_items = info.get_managed_items_lst()
     playtime = helper.time_to_frames(save_stats["play_time"])
-    tracker.Tracker().reset_tracker()
+    info.clear_managed_items()
 
-    return token, inquiry_code, save_data, playtime, managed_items
+    return token, inquiry_code, save_data, playtime, managed_items, save_stats
 
 
 def upload_handler(
     save_stats: dict[str, Any], path: str
-) -> Union[None, dict[str, Any]]:
+) -> Optional[tuple[Union[None, dict[str, Any]], dict[str, Any]]]:
     """Handles the upload of the save data"""
 
     data = prepare_upload(save_stats, path)
     if data is None:
         return None
-    token, inquiry_code, save_data, playtime, managed_items = data
+    token, inquiry_code, save_data, playtime, managed_items, save_stats = data
 
-    helper.colored_text("Uploading save data...", helper.GREEN)
+    helper.colored_text("저장 데이터 업로드 중...", helper.GREEN)
     upload_data = upload_save_data_v2(
         token,
         inquiry_code,
         save_data,
         playtime,
         managed_items,
         helper.calculate_user_rank(save_stats),
@@ -698,32 +725,32 @@
     #    save_data,
     #    playtime,
     #    managed_items,
     #    helper.calculate_user_rank(save_stats),
     # )
 
     helper.colored_text(
-        "게임에서 이 코드를 입력한 후 플레이를 누르면 금지 메시지가 표시될 수 있습니다. 그런 경우 재생을 다시 누르면 사라집니다.\n코드를 받으려면 엔터를 누르세요...",
+        "게임에서 이 코드를 입력한 후 플레이를 누르면 금지 메시지가 표시될 수 있습니다. 그런 경우 재생을 다시 누르면 사라집니다.\n코드를 받으려면 엔터키를 누르세요...",
         helper.DARK_YELLOW,
     )
     input()
-    return upload_data
+    return upload_data, save_stats
 
 
 def meta_data_upload_handler(
     save_stats: dict[str, Any], path: str
 ) -> tuple[Union[None, dict[str, Any]], dict[str, Any]]:
     """Handles the upload of the meta data"""
 
     data = prepare_upload(save_stats, path)
     if data is None:
         return None, save_stats
-    token, inquiry_code, save_data, playtime, managed_items = data
+    token, inquiry_code, save_data, playtime, managed_items, save_stats = data
 
-    helper.colored_text("Uploading meta data...", helper.GREEN)
+    helper.colored_text("메타 데이터 업로드 중...", helper.GREEN)
     upload_data = upload_metadata_v2(
         token,
         inquiry_code,
         save_data,
         playtime,
         managed_items,
         helper.calculate_user_rank(save_stats),
@@ -746,15 +773,15 @@
 def download_handler() -> Optional[str]:
     """Handles the download of the save data"""
 
     country_code = helper.ask_cc()
     if country_code == "jp":
         country_code = "ja"
     transfer_code = helper.check_hex(
-        input("전송 코드 입력:").lower().replace("o", "0")
+        input("이어하기 코드 입력:").lower().replace("o", "0")
     )
     if transfer_code is None:
         helper.colored_text(
             "전송 코드는 숫자 0-9와 문자 a-f로만 구성되어야 합니다.",
             helper.RED,
         )
         return None
@@ -763,29 +790,37 @@
     )
     if confirmation_code is None:
         helper.colored_text(
             "확인 코드는 숫자 0-9로만 구성되어야 합니다.",
             helper.RED,
         )
         return None
-    game_version = input("현재 게임 버전 입력 (e.g 11.3, 9.6, 10.4.0, 12.2.1):")
+    game_version = input("현재 게임 버전 입력 (e.g 11.3, 9.6, 10.4.0, 12.2.1, 12.3):")
     game_version = helper.str_to_gv(game_version)
-    save_data = download_save(
+    response = download_save(
         country_code, transfer_code, confirmation_code, game_version
     )
+    save_data = response.content
     if test_is_save_data(save_data):
         helper.colored_text("저장 데이터를 성공적으로 다운로드했습니다.\n", base=helper.GREEN)
     else:
         helper.colored_text(
-            "잘못된 전송 코드/확인 코드",
+            "잘못된 이전 코드/확인 코드/국가 코드",
             base=helper.RED,
         )
         return None
+    headers = response.headers
+    save_stats = parse_save.start_parse(save_data, country_code)
+    save_stats["token"] = headers["nyanko-password-refresh-token"]
+    info = user_info.UserInfo(save_stats["inquiry_code"])
+    info.set_password(headers["nyanko-password"])
+    save_data = serialise_save.start_serialize(save_stats)
+    save_data = patcher.patch_save_data(save_data, country_code)
     path = helper.save_file(
-        "Save save data",
+        "저장 데이터 저장",
         helper.get_save_file_filetype(),
         helper.get_save_path_home(),
     )
     if path is None:
         return None
     helper.write_file_bytes(path, save_data)
     return path
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/tracker.py` & `Shark sac Korean editor-1.1.2/modkr/tracker.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.1/modkr/updater.py` & `Shark sac Korean editor-1.1.2/modkr/updater.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 
 from . import config_manager, helper
 
 
 def update(latest_version: str, command: str = "py") -> bool:
     """Update pypi package testing for py and python"""
 
-    helper.colored_text("Updating...", base=helper.GREEN)
+    helper.colored_text("업데이트 중...", base=helper.GREEN)
     try:
         full_cmd = f"{command} -m pip install --upgrade battle-cats-save-editor=={latest_version}"
         subprocess.run(
             full_cmd,
             shell=True,
             capture_output=True,
             check=True,
         )
-        helper.colored_text("Update successful", base=helper.GREEN)
+        helper.colored_text("업데이트 완료", base=helper.GREEN)
         return True
     except subprocess.CalledProcessError:
         return False
 
 
 def try_update(latest_version: str):
     """
@@ -39,15 +39,15 @@
     success = update(latest_version, "python3")
     if success:
         return
     success = update(latest_version, "python")
     if success:
         return
     helper.colored_text(
-        "Update failed\nYou may need to manually update with py -m pip install -U battle-cats-save-editor",
+        "업데이트가 실패\n다음을 사용하여 수동으로 업데이트해야 할 수도 있습니다.py -m pip install -U battle-cats-save-editor",
         base=helper.RED,
     )
 
 
 def get_local_version() -> str:
     """Returns the local version of the editor"""
 
@@ -106,16 +106,16 @@
 
     check_pre = "b" in local_version or config_manager.get_config_value_category(
         "START_UP", "UPDATE_TO_BETAS"
     )
     if check_pre and pypi_is_newer(
         local_version, latest_prerelease_version, remove_b=False
     ):
-        helper.colored_text("Prerelease update available\n", base=helper.GREEN)
+        helper.colored_text("프리릴리즈 업데이트 가능\n", base=helper.GREEN)
         return True, latest_prerelease_version
 
     if pypi_is_newer(local_version, pypi_version):
-        helper.colored_text("Stable update available\n", base=helper.GREEN)
+        helper.colored_text("안정적인 업데이트 가능e\n", base=helper.GREEN)
         return True, pypi_version
 
-    helper.colored_text("No update available\n", base=helper.GREEN)
+    helper.colored_text("사용 가능한 업데이트 없음\n", base=helper.GREEN)
     return False, local_version
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Shark sac Korean editor-1.1.1/modkr/user_input_handler.py` & `Shark sac Korean editor-1.1.2/modkr/user_input_handler.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.1/setup.py` & `Shark sac Korean editor-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 basedir = path.abspath(path.dirname(__file__))
 with open(path.join(basedir, 'README.md'), encoding='utf-8') as file:
     long_description = file.read().replace('\r\n', '\n')
 
 setup(
     name='Shark sac Korean editor',
-    version='1.1.1',
+    version='1.1.2',
     description='냥코에디터 한글화',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='익명',
     author_email='',
     url='https://github.com/sharkwodm/koreditor',
     packages=find_packages(exclude=['contrib', 'docs', 'tests']),
```

