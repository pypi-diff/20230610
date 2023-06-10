# Comparing `tmp/evennia-1.3.0.tar.gz` & `tmp/evennia-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evennia-1.3.0.tar", last modified: Sat Apr 29 06:52:56 2023, max compression
+gzip compressed data, was "evennia-2.0.0.tar", last modified: Sat Jun 10 07:51:20 2023, max compression
```

## Comparing `evennia-1.3.0.tar` & `evennia-2.0.0.tar`

### file list

```diff
@@ -1,953 +1,966 @@
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.532944 evennia-1.3.0/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1531 2023-04-10 11:44:01.000000 evennia-1.3.0/LICENSE.txt
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5239 2023-04-29 06:52:56.532944 evennia-1.3.0/PKG-INFO
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3027 2023-04-10 11:44:01.000000 evennia-1.3.0/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.436944 evennia-1.3.0/bin/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.440944 evennia-1.3.0/bin/unix/
--rwxrwxr-x   0 griatch   (1000) griatch   (1000)      210 2023-04-10 11:44:01.000000 evennia-1.3.0/bin/unix/evennia
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.444944 evennia-1.3.0/evennia/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        6 2023-04-29 06:31:26.000000 evennia-1.3.0/evennia/VERSION.txt
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      438 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/VERSION_REQS.txt
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12647 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1839 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/__main__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.444944 evennia-1.3.0/evennia/accounts/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      214 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/accounts/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    67757 2023-04-20 21:48:41.000000 evennia-1.3.0/evennia/accounts/accounts.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    26733 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/accounts/bots.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9574 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/accounts/manager.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.444944 evennia-1.3.0/evennia/accounts/migrations/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7211 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/accounts/migrations/0001_initial.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      504 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/accounts/migrations/0002_move_defaults.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      612 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/accounts/migrations/0003_auto_20150209_2234.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2158 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/accounts/migrations/0004_auto_20150403_2339.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1010 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/accounts/migrations/0005_auto_20160905_0902.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1488 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/accounts/migrations/0006_auto_20170606_1731.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1927 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/accounts/migrations/0007_copy_player_to_account.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3944 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/accounts/migrations/0008_auto_20190128_1820.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      867 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/accounts/migrations/0009_auto_20191025_0831.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      467 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/accounts/migrations/0010_auto_20210520_2137.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4017 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/accounts/migrations/0011_convert_contrib_typeclass_paths.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      490 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/accounts/migrations/0012_defaultaccount_alter_accountdb_id_account_bot_and_more.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/accounts/migrations/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5740 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/accounts/models.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    16624 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/accounts/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.448944 evennia-1.3.0/evennia/commands/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      304 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/commands/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.448944 evennia-1.3.0/evennia/commands/_trial_temp/
--rwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/commands/_trial_temp/_trial_marker
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    31705 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/commands/cmdhandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8287 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/commands/cmdparser.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    27219 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/commands/cmdset.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    26152 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/commands/cmdsethandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    29198 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/commands/command.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.448944 evennia-1.3.0/evennia/commands/default/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       87 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/commands/default/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    37421 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/commands/default/account.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    19595 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/commands/default/admin.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    23003 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/commands/default/batchprocess.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)   167200 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/commands/default/building.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2358 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/commands/default/cmdset_account.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3032 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/commands/default/cmdset_character.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      371 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/commands/default/cmdset_session.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      872 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/commands/default/cmdset_unloggedin.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    76302 2023-04-29 06:12:49.000000 evennia-1.3.0/evennia/commands/default/comms.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    22494 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/commands/default/general.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    39551 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/commands/default/help.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12788 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/commands/default/muxcommand.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3152 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/commands/default/syscommands.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    41884 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/commands/default/system.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    81813 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/commands/default/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17440 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/commands/default/unloggedin.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    46641 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/commands/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.448944 evennia-1.3.0/evennia/comms/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      207 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    32556 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/comms.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    16863 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/managers.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.452944 evennia-1.3.0/evennia/comms/migrations/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3523 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/migrations/0001_initial.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      500 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/migrations/0002_msg_db_hide_from_objects.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3784 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/migrations/0003_auto_20140917_0756.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      504 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/migrations/0004_auto_20150118_1631.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      641 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/migrations/0005_auto_20150223_1517.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      643 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/migrations/0006_channeldb_db_object_subscriptions.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      615 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/migrations/0007_msg_db_tags.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      434 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/migrations/0008_auto_20160905_0902.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3872 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/migrations/0009_auto_20160921_1731.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1079 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/migrations/0010_auto_20161206_1912.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1029 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/migrations/0011_auto_20170217_2039.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4563 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/migrations/0011_auto_20170606_1731.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      267 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/migrations/0012_merge_20170617_2017.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4778 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/migrations/0013_auto_20170705_1726.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1442 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/migrations/0014_auto_20170705_1736.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      943 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/migrations/0015_auto_20170706_2041.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      462 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/migrations/0016_auto_20180925_1735.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7069 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/migrations/0017_auto_20190128_1820.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      665 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/migrations/0018_auto_20191025_0831.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1713 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/migrations/0019_auto_20210514_2032.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      916 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/migrations/0020_auto_20210514_2210.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3635 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/migrations/0021_auto_20210520_2137.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      711 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/migrations/0022_defaultchannel_alter_channeldb_id_alter_msg_id_and_more.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/migrations/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    22638 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/models.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3166 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.452944 evennia-1.3.0/evennia/contrib/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1895 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      198 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.452944 evennia-1.3.0/evennia/contrib/base_systems/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       80 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.452944 evennia-1.3.0/evennia/contrib/base_systems/awsstorage/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7695 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/awsstorage/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       48 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/awsstorage/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    32480 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/awsstorage/aws_s3_cdn.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    22503 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/awsstorage/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.452944 evennia-1.3.0/evennia/contrib/base_systems/building_menu/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    46012 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/building_menu/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      148 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/building_menu/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    42659 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/building_menu/building_menu.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6878 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/building_menu/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.452944 evennia-1.3.0/evennia/contrib/base_systems/color_markups/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2641 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/color_markups/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       84 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/color_markups/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8605 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/color_markups/color_markups.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3356 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/color_markups/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.452944 evennia-1.3.0/evennia/contrib/base_systems/components/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6397 2023-04-29 05:57:10.000000 evennia-1.3.0/evennia/contrib/base_systems/components/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      952 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/components/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3915 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/components/component.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3762 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/components/dbfield.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11201 2023-04-20 16:46:53.000000 evennia-1.3.0/evennia/contrib/base_systems/components/holder.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7237 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/components/signals.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14575 2023-04-20 16:46:53.000000 evennia-1.3.0/evennia/contrib/base_systems/components/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.452944 evennia-1.3.0/evennia/contrib/base_systems/custom_gametime/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1549 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/custom_gametime/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      439 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/custom_gametime/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10390 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/custom_gametime/custom_gametime.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2017 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/custom_gametime/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.452944 evennia-1.3.0/evennia/contrib/base_systems/email_login/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1022 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/email_login/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      136 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/email_login/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1445 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/email_login/connection_screens.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10264 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/email_login/email_login.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1200 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/email_login/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.452944 evennia-1.3.0/evennia/contrib/base_systems/godotwebsocket/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8938 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/godotwebsocket/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      703 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/godotwebsocket/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3074 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/godotwebsocket/test_text2bbcode.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    27602 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/godotwebsocket/text2bbcode.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2686 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/godotwebsocket/webclient.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.456944 evennia-1.3.0/evennia/contrib/base_systems/ingame_python/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    40300 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/ingame_python/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      128 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/ingame_python/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6777 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/ingame_python/callbackhandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    21872 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/ingame_python/commands.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3048 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/ingame_python/eventfuncs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    23990 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/ingame_python/scripts.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    21618 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/ingame_python/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    34963 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/ingame_python/typeclasses.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8151 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/ingame_python/utils.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.456944 evennia-1.3.0/evennia/contrib/base_systems/menu_login/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      787 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/menu_login/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      143 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/menu_login/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1206 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/menu_login/connection_screens.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8781 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/menu_login/menu_login.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      265 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/menu_login/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.456944 evennia-1.3.0/evennia/contrib/base_systems/mux_comms_cmds/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1936 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/mux_comms_cmds/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      104 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/mux_comms_cmds/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    16012 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/mux_comms_cmds/mux_comms_cmds.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2298 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/mux_comms_cmds/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.456944 evennia-1.3.0/evennia/contrib/base_systems/unixcommand/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2241 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/unixcommand/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       94 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/unixcommand/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1654 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/unixcommand/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9989 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/unixcommand/unixcommand.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.456944 evennia-1.3.0/evennia/contrib/full_systems/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       75 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/full_systems/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       48 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/full_systems/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.456944 evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5210 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      266 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    22699 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/commands.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10565 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/menu.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    34348 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/objects.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7942 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/room.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      753 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/scripts.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9582 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/state.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.456944 evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/states/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1203 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/states/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4168 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/states/state_001_start.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10461 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6112 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/utils.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.456944 evennia-1.3.0/evennia/contrib/game_systems/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      269 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.456944 evennia-1.3.0/evennia/contrib/game_systems/barter/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4322 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/barter/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       80 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/barter/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    29726 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/barter/barter.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5976 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/barter/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.456944 evennia-1.3.0/evennia/contrib/game_systems/clothing/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4249 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/clothing/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      199 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/clothing/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    24574 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/clothing/clothing.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4816 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/clothing/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.456944 evennia-1.3.0/evennia/contrib/game_systems/cooldowns/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2084 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/cooldowns/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       88 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/cooldowns/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7580 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/cooldowns/cooldowns.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6135 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/cooldowns/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.456944 evennia-1.3.0/evennia/contrib/game_systems/crafting/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11186 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/crafting/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      233 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/crafting/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    41599 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/crafting/crafting.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17892 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/crafting/example_recipes.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    24911 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/crafting/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.460944 evennia-1.3.0/evennia/contrib/game_systems/gendersub/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1986 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/gendersub/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      123 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/gendersub/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5096 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/gendersub/gendersub.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1091 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/gendersub/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.460944 evennia-1.3.0/evennia/contrib/game_systems/mail/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1567 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/mail/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      115 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/mail/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14841 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/mail/mail.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1852 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/mail/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.460944 evennia-1.3.0/evennia/contrib/game_systems/multidescer/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      932 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/multidescer/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       83 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/multidescer/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9951 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/multidescer/multidescer.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1404 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/multidescer/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.460944 evennia-1.3.0/evennia/contrib/game_systems/puzzles/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2181 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/puzzles/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      124 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/puzzles/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    27837 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/puzzles/puzzles.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    41328 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/puzzles/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.460944 evennia-1.3.0/evennia/contrib/game_systems/turnbattle/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2940 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/turnbattle/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      209 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/turnbattle/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    28762 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/turnbattle/tb_basic.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    23139 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/turnbattle/tb_equip.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    37446 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/turnbattle/tb_items.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    30705 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/turnbattle/tb_magic.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    38339 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/turnbattle/tb_range.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    29682 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/turnbattle/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.460944 evennia-1.3.0/evennia/contrib/grid/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       84 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       81 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.460944 evennia-1.3.0/evennia/contrib/grid/extended_room/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3172 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/extended_room/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      384 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/extended_room/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    21167 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/extended_room/extended_room.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4793 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/extended_room/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.460944 evennia-1.3.0/evennia/contrib/grid/ingame_map_display/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1358 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/ingame_map_display/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       92 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/ingame_map_display/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10572 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/ingame_map_display/ingame_map_display.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1404 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/ingame_map_display/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.460944 evennia-1.3.0/evennia/contrib/grid/mapbuilder/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9672 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/mapbuilder/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       87 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/mapbuilder/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17398 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/mapbuilder/mapbuilder.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6435 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/mapbuilder/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.460944 evennia-1.3.0/evennia/contrib/grid/simpledoor/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1356 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/simpledoor/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      129 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/simpledoor/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5838 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/simpledoor/simpledoor.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1079 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/simpledoor/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.460944 evennia-1.3.0/evennia/contrib/grid/slow_exit/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1730 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/slow_exit/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      203 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/slow_exit/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5046 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/slow_exit/slow_exit.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      824 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/slow_exit/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.460944 evennia-1.3.0/evennia/contrib/grid/wilderness/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4932 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/wilderness/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      394 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/wilderness/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6026 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/wilderness/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    28916 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/wilderness/wilderness.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.464944 evennia-1.3.0/evennia/contrib/grid/xyzgrid/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    54690 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/xyzgrid/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      202 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/xyzgrid/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    20837 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/xyzgrid/commands.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7822 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/xyzgrid/example.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    13723 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/xyzgrid/launchcmd.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1145 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/xyzgrid/prototypes.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    42072 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/xyzgrid/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1043 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/xyzgrid/utils.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    40413 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/xyzgrid/xymap.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    52070 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/xyzgrid/xymap_legend.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10484 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/xyzgrid/xyzgrid.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    24616 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/xyzgrid/xyzroom.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.464944 evennia-1.3.0/evennia/contrib/rpg/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      406 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.464944 evennia-1.3.0/evennia/contrib/rpg/buffs/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    22364 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/buffs/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/buffs/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    45607 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/buffs/buff.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3893 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/buffs/samplebuffs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    16470 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/buffs/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.464944 evennia-1.3.0/evennia/contrib/rpg/character_creator/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3924 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/character_creator/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      176 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/character_creator/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8148 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/character_creator/character_creator.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    21006 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/character_creator/example_menu.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1552 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/character_creator/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.464944 evennia-1.3.0/evennia/contrib/rpg/dice/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1442 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/dice/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      177 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/dice/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10272 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/dice/dice.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      901 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/dice/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.464944 evennia-1.3.0/evennia/contrib/rpg/health_bar/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1264 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/health_bar/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       94 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/health_bar/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4913 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/health_bar/health_bar.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1634 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/health_bar/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.464944 evennia-1.3.0/evennia/contrib/rpg/rpsystem/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9938 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/rpsystem/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      793 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/rpsystem/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    24722 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/rpsystem/rplanguage.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    65825 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/rpsystem/rpsystem.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14981 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/rpsystem/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.464944 evennia-1.3.0/evennia/contrib/rpg/traits/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14246 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/traits/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      294 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/traits/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    37184 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/traits/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    54252 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/traits/traits.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.464944 evennia-1.3.0/evennia/contrib/tutorials/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      151 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       81 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.464944 evennia-1.3.0/evennia/contrib/tutorials/batchprocessor/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1623 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/batchprocessor/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       50 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/batchprocessor/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1567 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/batchprocessor/example_batch_cmds.ev
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3618 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/batchprocessor/example_batch_code.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.464944 evennia-1.3.0/evennia/contrib/tutorials/bodyfunctions/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      471 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/bodyfunctions/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      104 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/bodyfunctions/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2311 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/bodyfunctions/bodyfunctions.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3324 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/bodyfunctions/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.468944 evennia-1.3.0/evennia/contrib/tutorials/evadventure/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1183 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      164 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3996 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/build_techdemo.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/build_world.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12557 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/characters.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11187 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/chargen.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    48197 2023-04-20 16:49:57.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/combat_turnbased.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    13739 2023-04-20 16:49:57.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/commands.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17844 2023-04-20 16:49:57.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/dungeon.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1533 2023-04-20 16:49:57.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/enums.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14381 2023-04-20 16:49:57.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/equipment.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11894 2023-04-20 16:49:57.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/npcs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6614 2023-04-20 16:49:57.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/objects.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8743 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/quests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11708 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/random_tables.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2983 2023-04-20 16:49:57.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/rooms.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    13120 2023-04-20 16:49:57.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/rules.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17153 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/shops.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.468944 evennia-1.3.0/evennia/contrib/tutorials/evadventure/tests/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/tests/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1389 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/tests/mixins.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1266 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/tests/test_characters.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2151 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/tests/test_chargen.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12871 2023-04-20 16:49:57.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/tests/test_combat.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4159 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/tests/test_commands.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3356 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/tests/test_dungeon.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7811 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/tests/test_equipment.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4629 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/tests/test_quests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8083 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/tests/test_rules.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      712 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/tests/test_utils.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1485 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/utils.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.468944 evennia-1.3.0/evennia/contrib/tutorials/mirror/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      429 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/mirror/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       83 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/mirror/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2235 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/mirror/mirror.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.468944 evennia-1.3.0/evennia/contrib/tutorials/red_button/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1344 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/red_button/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       94 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/red_button/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    18609 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/red_button/red_button.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.468944 evennia-1.3.0/evennia/contrib/tutorials/talking_npc/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      722 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/talking_npc/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      124 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/talking_npc/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3697 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/talking_npc/talking_npc.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      449 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/talking_npc/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.468944 evennia-1.3.0/evennia/contrib/tutorials/tutorial_world/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4302 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/tutorial_world/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      125 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/tutorial_world/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    50297 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/tutorial_world/build.ev
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    25293 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/tutorial_world/intro_menu.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    16130 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/tutorial_world/mob.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    42155 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/tutorial_world/objects.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    42922 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/tutorial_world/rooms.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7342 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/tutorial_world/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.468944 evennia-1.3.0/evennia/contrib/utils/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       67 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.472944 evennia-1.3.0/evennia/contrib/utils/auditing/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3303 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/auditing/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/auditing/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2065 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/auditing/outputs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8515 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/auditing/server.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6023 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/auditing/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.472944 evennia-1.3.0/evennia/contrib/utils/fieldfill/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5816 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/fieldfill/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      288 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/fieldfill/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    26404 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/fieldfill/fieldfill.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.472944 evennia-1.3.0/evennia/contrib/utils/git_integration/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3139 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/git_integration/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       86 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/git_integration/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7743 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/git_integration/git_integration.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2828 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/git_integration/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.472944 evennia-1.3.0/evennia/contrib/utils/name_generator/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9815 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/name_generator/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/name_generator/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)   232619 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/name_generator/btn_givennames.txt
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    56503 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/name_generator/btn_surnames.txt
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14447 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/name_generator/namegen.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4914 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/name_generator/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.472944 evennia-1.3.0/evennia/contrib/utils/random_string_generator/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2165 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/random_string_generator/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      268 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/random_string_generator/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12595 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/random_string_generator/random_string_generator.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      737 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/random_string_generator/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.472944 evennia-1.3.0/evennia/contrib/utils/tree_select/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5935 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/tree_select/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      109 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/tree_select/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2199 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/tree_select/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    20930 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/tree_select/tree_select.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.472944 evennia-1.3.0/evennia/game_template/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1521 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.472944 evennia-1.3.0/evennia/game_template/commands/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      676 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/commands/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/commands/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7738 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/commands/command.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2636 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/commands/default_cmdsets.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      551 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/gitignore
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.472944 evennia-1.3.0/evennia/game_template/server/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1718 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/server/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/server/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.476944 evennia-1.3.0/evennia/game_template/server/conf/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/server/conf/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      629 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/server/conf/at_initial_setup.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2154 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/server/conf/at_search.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1369 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/server/conf/at_server_startstop.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2174 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/server/conf/cmdparser.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1500 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/server/conf/connection_screens.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1159 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/server/conf/inlinefuncs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1419 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/server/conf/inputfuncs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1065 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/server/conf/lockfuncs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4009 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/server/conf/mssp.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      709 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/server/conf/portal_services_plugins.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      714 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/server/conf/secret_settings.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      705 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/server/conf/server_services_plugins.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1347 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/server/conf/serversession.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1500 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/server/conf/settings.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1185 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/server/conf/web_plugins.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.476944 evennia-1.3.0/evennia/game_template/server/logs/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      839 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/server/logs/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.476944 evennia-1.3.0/evennia/game_template/typeclasses/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      733 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/typeclasses/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/typeclasses/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3774 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/typeclasses/accounts.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2920 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/typeclasses/channels.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1525 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/typeclasses/characters.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2044 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/typeclasses/exits.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8847 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/typeclasses/objects.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      551 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/typeclasses/rooms.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4394 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/typeclasses/scripts.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.476944 evennia-1.3.0/evennia/game_template/web/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2939 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.476944 evennia-1.3.0/evennia/game_template/web/admin/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      296 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/admin/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/admin/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      520 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/admin/urls.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.476944 evennia-1.3.0/evennia/game_template/web/api/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/api/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.476944 evennia-1.3.0/evennia/game_template/web/static/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      849 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/static/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.440944 evennia-1.3.0/evennia/game_template/web/static/rest_framework/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.476944 evennia-1.3.0/evennia/game_template/web/static/rest_framework/css/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       53 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/static/rest_framework/css/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.476944 evennia-1.3.0/evennia/game_template/web/static/rest_framework/images/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       47 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/static/rest_framework/images/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.440944 evennia-1.3.0/evennia/game_template/web/static/webclient/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.476944 evennia-1.3.0/evennia/game_template/web/static/webclient/css/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      132 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/static/webclient/css/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.476944 evennia-1.3.0/evennia/game_template/web/static/webclient/js/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      143 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/static/webclient/js/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.440944 evennia-1.3.0/evennia/game_template/web/static/website/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.476944 evennia-1.3.0/evennia/game_template/web/static/website/css/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      129 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/static/website/css/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.476944 evennia-1.3.0/evennia/game_template/web/static/website/images/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      135 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/static/website/images/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.476944 evennia-1.3.0/evennia/game_template/web/templates/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      760 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/templates/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.476944 evennia-1.3.0/evennia/game_template/web/templates/rest_framework/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       58 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/templates/rest_framework/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.476944 evennia-1.3.0/evennia/game_template/web/templates/webclient/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      223 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/templates/webclient/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.476944 evennia-1.3.0/evennia/game_template/web/templates/website/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      217 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/templates/website/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.476944 evennia-1.3.0/evennia/game_template/web/templates/website/flatpages/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      185 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/templates/website/flatpages/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.476944 evennia-1.3.0/evennia/game_template/web/templates/website/registration/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      152 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/templates/website/registration/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1099 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/urls.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.480944 evennia-1.3.0/evennia/game_template/web/webclient/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1102 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/webclient/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/webclient/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      539 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/webclient/urls.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.480944 evennia-1.3.0/evennia/game_template/web/website/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1262 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/website/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/website/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      509 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/website/urls.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.480944 evennia-1.3.0/evennia/game_template/web/website/views/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/website/views/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.480944 evennia-1.3.0/evennia/game_template/world/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      467 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/world/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/world/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      999 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/world/batch_cmds.ev
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2186 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/world/help_entries.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3646 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/world/prototypes.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.480944 evennia-1.3.0/evennia/help/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      217 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/help/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8013 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/help/filehelp.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6229 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/help/manager.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.480944 evennia-1.3.0/evennia/help/migrations/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2222 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/help/migrations/0001_initial.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      577 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/help/migrations/0002_auto_20170606_1731.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1688 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/help/migrations/0003_auto_20190128_1820.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      540 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/help/migrations/0004_auto_20210520_2137.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1166 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/help/migrations/0005_auto_20210530_1818.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      473 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/help/migrations/0006_alter_helpentry_id.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/help/migrations/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9729 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/help/models.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3736 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/help/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7673 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/help/utils.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.480944 evennia-1.3.0/evennia/locale/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2686 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locale/README
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.440944 evennia-1.3.0/evennia/locale/de/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.480944 evennia-1.3.0/evennia/locale/de/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10764 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14475 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locale/de/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.440944 evennia-1.3.0/evennia/locale/es/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.480944 evennia-1.3.0/evennia/locale/es/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3821 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    30981 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locale/es/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.440944 evennia-1.3.0/evennia/locale/fr/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.484944 evennia-1.3.0/evennia/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    26255 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    38581 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locale/fr/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.440944 evennia-1.3.0/evennia/locale/it/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.484944 evennia-1.3.0/evennia/locale/it/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6944 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locale/it/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    35844 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locale/it/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.440944 evennia-1.3.0/evennia/locale/ko/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.484944 evennia-1.3.0/evennia/locale/ko/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3569 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locale/ko/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    30924 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locale/ko/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.440944 evennia-1.3.0/evennia/locale/la/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.484944 evennia-1.3.0/evennia/locale/la/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6537 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locale/la/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    32786 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locale/la/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.440944 evennia-1.3.0/evennia/locale/pl/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.484944 evennia-1.3.0/evennia/locale/pl/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1631 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locale/pl/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    28236 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locale/pl/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.440944 evennia-1.3.0/evennia/locale/pt/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.484944 evennia-1.3.0/evennia/locale/pt/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    25584 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locale/pt/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    42122 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locale/pt/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.440944 evennia-1.3.0/evennia/locale/ru/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.488944 evennia-1.3.0/evennia/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2281 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locale/ru/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    29419 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locale/ru/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.440944 evennia-1.3.0/evennia/locale/sv/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.488944 evennia-1.3.0/evennia/locale/sv/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    29036 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locale/sv/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    43353 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locale/sv/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.440944 evennia-1.3.0/evennia/locale/zh/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.488944 evennia-1.3.0/evennia/locale/zh/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3300 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locale/zh/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    30540 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locale/zh/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.488944 evennia-1.3.0/evennia/locks/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      240 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locks/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    22093 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locks/lockfuncs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    26966 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locks/lockhandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    13732 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locks/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.488944 evennia-1.3.0/evennia/objects/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      120 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/objects/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    29704 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/objects/manager.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.492944 evennia-1.3.0/evennia/objects/migrations/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4315 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/objects/migrations/0001_initial.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1193 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/objects/migrations/0002_auto_20140917_0756.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      810 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/objects/migrations/0003_defaultcharacter_defaultexit_defaultobject_defaultroom.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      530 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/objects/migrations/0004_auto_20150118_1622.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      410 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/objects/migrations/0005_auto_20150403_2339.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1599 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/objects/migrations/0006_auto_20170606_1731.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1203 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/objects/migrations/0007_objectdb_db_account.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      757 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/objects/migrations/0008_auto_20170705_1736.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      643 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/objects/migrations/0009_remove_objectdb_db_player.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5028 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/objects/migrations/0010_auto_20190128_1820.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1351 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/objects/migrations/0011_auto_20191025_0831.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4011 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/objects/migrations/0012_convert_contrib_typeclass_paths.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      488 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/objects/migrations/0013_defaultobject_alter_objectdb_id_defaultcharacter_and_more.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/objects/migrations/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    13399 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/objects/models.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)   119132 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/objects/objects.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14391 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/objects/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.492944 evennia-1.3.0/evennia/prototypes/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6567 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/prototypes/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/prototypes/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    92110 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/prototypes/menus.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2912 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/prototypes/protfuncs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    46545 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/prototypes/prototypes.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    42860 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/prototypes/spawner.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    39636 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/prototypes/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.492944 evennia-1.3.0/evennia/scripts/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      229 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/scripts/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11275 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/scripts/manager.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.492944 evennia-1.3.0/evennia/scripts/migrations/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4762 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/scripts/migrations/0001_initial.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      675 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/scripts/migrations/0002_auto_20150118_1625.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1507 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/scripts/migrations/0003_checksessions_defaultscript_donothing_scriptbase_store_validatechannelhandler_validateidmappercache_.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      861 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/scripts/migrations/0004_auto_20150306_1354.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      430 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/scripts/migrations/0005_auto_20150306_1441.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      710 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/scripts/migrations/0006_auto_20150310_2249.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      396 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/scripts/migrations/0007_auto_20150403_2339.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      913 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/scripts/migrations/0008_auto_20170606_1731.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1271 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/scripts/migrations/0009_scriptdb_db_account.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      757 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/scripts/migrations/0010_auto_20170705_1736.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      596 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/scripts/migrations/0011_remove_scriptdb_db_player.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4655 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/scripts/migrations/0012_auto_20190128_1820.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      666 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/scripts/migrations/0013_auto_20191025_0831.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      752 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/scripts/migrations/0014_auto_20210520_2137.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3329 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/scripts/migrations/0015_convert_contrib_paths.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      478 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/scripts/migrations/0016_scriptbase_alter_scriptdb_id_defaultscript_and_more.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/scripts/migrations/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6311 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/scripts/models.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8746 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/scripts/monitorhandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4987 2023-04-20 16:49:57.000000 evennia-1.3.0/evennia/scripts/scripthandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    27442 2023-04-20 16:49:57.000000 evennia-1.3.0/evennia/scripts/scripts.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    20801 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/scripts/taskhandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10678 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/scripts/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    24704 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/scripts/tickerhandler.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.496944 evennia-1.3.0/evennia/server/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      234 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8697 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/amp_client.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    16629 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/connection_wizard.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7955 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/deprecations.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    79833 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/evennia_launcher.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.496944 evennia-1.3.0/evennia/server/game_index_client/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4321 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/game_index_client/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       45 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/game_index_client/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6277 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/game_index_client/client.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1990 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/game_index_client/service.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7647 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/initial_setup.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    19709 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/inputfuncs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1708 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/manager.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.496944 evennia-1.3.0/evennia/server/migrations/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      812 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/migrations/0001_initial.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1363 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/migrations/0002_auto_20190128_2311.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      478 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/migrations/0003_alter_serverconfig_id.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/migrations/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3818 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/models.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.496944 evennia-1.3.0/evennia/server/portal/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/portal/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17922 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/portal/amp.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17520 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/portal/amp_server.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    18478 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/portal/discord.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11345 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/portal/grapevine.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14242 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/portal/irc.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2571 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/portal/mccp.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3882 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/portal/mssp.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2341 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/portal/mxp.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2359 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/portal/naws.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    16002 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/portal/portal.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17231 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/portal/portalsessionhandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4450 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/portal/rss.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    15788 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/portal/ssh.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3319 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/portal/ssl.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1785 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/portal/suppress_ga.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17379 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/portal/telnet.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    15609 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/portal/telnet_oob.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4861 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/portal/telnet_ssl.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14725 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/portal/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6991 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/portal/ttype.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11265 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/portal/webclient.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    15897 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/portal/webclient_ajax.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.500944 evennia-1.3.0/evennia/server/profiling/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      212 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/profiling/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/profiling/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    20881 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/profiling/dummyrunner.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9427 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/profiling/dummyrunner_settings.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3924 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/profiling/memplot.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1375 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/profiling/settings_mixin.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1095 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/profiling/test_queries.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5371 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/profiling/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1345 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/profiling/timetrace.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    28629 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/server.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14599 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/serversession.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5616 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/session.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    30190 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/sessionhandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4935 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/signals.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.500944 evennia-1.3.0/evennia/server/tests/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/tests/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4721 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/tests/test_amp_connection.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      521 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/tests/test_initial_setup.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7305 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/tests/test_launcher.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4444 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/tests/test_misc.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9256 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/tests/test_server.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1369 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/tests/testrunner.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7101 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/throttle.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2763 2023-04-20 22:23:08.000000 evennia-1.3.0/evennia/server/validators.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8653 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/webserver.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    60833 2023-04-20 21:45:02.000000 evennia-1.3.0/evennia/settings_default.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.500944 evennia-1.3.0/evennia/typeclasses/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      434 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/typeclasses/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    64065 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/typeclasses/attributes.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    31304 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/typeclasses/managers.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.504944 evennia-1.3.0/evennia/typeclasses/migrations/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6101 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/typeclasses/migrations/0001_initial.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      768 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/typeclasses/migrations/0002_auto_20150109_0913.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2266 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/typeclasses/migrations/0003_defaultcharacter_defaultexit_defaultguest_defaultobject_defaultplayer_defaultroom_defaultscript_dono.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      833 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/typeclasses/migrations/0004_auto_20151101_1759.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      922 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/typeclasses/migrations/0005_auto_20160625_1812.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1444 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/typeclasses/migrations/0006_auto_add_dbmodel_value_for_tags_attributes.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3899 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/typeclasses/migrations/0007_tag_migrations_may_be_slow.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1699 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/typeclasses/migrations/0008_lock_and_perm_rename.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4230 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/typeclasses/migrations/0009_rename_player_cmdsets_typeclasses.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1993 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/typeclasses/migrations/0010_delete_old_player_tables.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5265 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/typeclasses/migrations/0011_auto_20190128_1820.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      821 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/typeclasses/migrations/0012_attrs_to_picklev4_may_be_slow.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      592 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/typeclasses/migrations/0013_auto_20191015_1922.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      592 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/typeclasses/migrations/0014_alter_tag_db_category.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      362 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/typeclasses/migrations/0015_alter_attribute_options.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      722 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/typeclasses/migrations/0016_alter_attribute_id_alter_tag_id.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/typeclasses/migrations/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    37091 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/typeclasses/models.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    25077 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/typeclasses/tags.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17813 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/typeclasses/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.504944 evennia-1.3.0/evennia/utils/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      320 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    51381 2023-04-20 16:46:53.000000 evennia-1.3.0/evennia/utils/ansi.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    15392 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/batchprocessors.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8077 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/containers.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10242 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/create.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    32941 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/dbserialize.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    41419 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/eveditor.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2734 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/evennia-mode.el
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    21081 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/evform.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    78095 2023-04-20 16:49:57.000000 evennia-1.3.0/evennia/utils/evmenu.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    18330 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/evmore.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    65173 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/evtable.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    53244 2023-04-20 16:49:57.000000 evennia-1.3.0/evennia/utils/funcparser.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8779 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/gametime.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.504944 evennia-1.3.0/evennia/utils/idmapper/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1309 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/idmapper/LICENSE.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1097 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/idmapper/README_evennia.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1992 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/idmapper/README_orig.rst
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       64 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/idmapper/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1181 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/idmapper/manager.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    24820 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/idmapper/models.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2876 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/idmapper/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    18789 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/logger.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10265 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/optionclasses.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6455 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/optionhandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11093 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/picklefield.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14179 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/search.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    24929 2023-04-29 05:55:25.000000 evennia-1.3.0/evennia/utils/test_resources.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.508944 evennia-1.3.0/evennia/utils/tests/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/tests/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.508944 evennia-1.3.0/evennia/utils/tests/data/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/tests/data/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      274 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/tests/data/broken_script.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1125 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/tests/data/evform_example.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6245 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/tests/data/evmenu_example.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      382 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/tests/data/prototypes_example.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1608 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/tests/test_ansi.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7052 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/tests/test_batchprocessors.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3463 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/tests/test_containers.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7032 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/tests/test_create_functions.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7888 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/tests/test_dbserialize.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11752 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/tests/test_eveditor.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12172 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/tests/test_evform.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11767 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/tests/test_evmenu.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12101 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/tests/test_evtable.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    30844 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/tests/test_funcparser.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3942 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/tests/test_gametime.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4460 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/tests/test_search.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    13564 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/tests/test_tagparsing.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5509 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/tests/test_text2html.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    29939 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/tests/test_utils.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6371 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/tests/test_validatorfuncs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12235 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/text2html.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    97251 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/utils.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9489 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/validatorfuncs.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.508944 evennia-1.3.0/evennia/utils/verb_conjugation/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    18011 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/verb_conjugation/LICENSE.txt
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/verb_conjugation/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9885 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/verb_conjugation/conjugate.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11298 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/verb_conjugation/pronouns.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10493 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/verb_conjugation/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)   554408 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/verb_conjugation/verbs.txt
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.508944 evennia-1.3.0/evennia/web/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1150 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      127 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.512944 evennia-1.3.0/evennia/web/admin/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      428 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/admin/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14125 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/admin/accounts.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8627 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/admin/attributes.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8508 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/admin/comms.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      593 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/admin/frontpage.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1889 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/admin/help.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11915 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/admin/objects.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4499 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/admin/scripts.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      508 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/admin/server.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8955 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/admin/tags.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      878 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/admin/urls.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2884 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/admin/utils.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.512944 evennia-1.3.0/evennia/web/api/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7674 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/api/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/api/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4268 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/api/filters.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3949 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/api/permissions.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      277 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/api/root.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9905 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/api/serializers.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8148 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/api/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2293 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/api/urls.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5828 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/api/views.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.440944 evennia-1.3.0/evennia/web/static/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.440944 evennia-1.3.0/evennia/web/static/rest_framework/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.512944 evennia-1.3.0/evennia/web/static/rest_framework/css/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      298 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/rest_framework/css/api.css
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.512944 evennia-1.3.0/evennia/web/static/rest_framework/images/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1406 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/rest_framework/images/favicon.ico
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.440944 evennia-1.3.0/evennia/web/static/webclient/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.516944 evennia-1.3.0/evennia/web/static/webclient/css/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2104 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/css/goldenlayout.css
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    27268 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/css/webclient.css
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.516944 evennia-1.3.0/evennia/web/static/webclient/fonts/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    22208 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/fonts/DejaVuSansMono-webfont.woff
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      185 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/fonts/DejaVuSansMono.css
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.516944 evennia-1.3.0/evennia/web/static/webclient/js/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    18546 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/js/evennia.js
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.520943 evennia-1.3.0/evennia/web/static/webclient/js/plugins/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      563 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/js/plugins/clienthelp.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3914 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/js/plugins/default_in.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1958 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/js/plugins/default_out.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      345 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/js/plugins/default_unload.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3785 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/js/plugins/font.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    28903 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/js/plugins/goldenlayout.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2114 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/js/plugins/goldenlayout_default_config.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2981 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/js/plugins/history.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5031 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/js/plugins/hotbuttons.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1969 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/js/plugins/html.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1912 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/js/plugins/iframe.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4666 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/js/plugins/message_routing.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4611 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/js/plugins/multimedia.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2842 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/js/plugins/notifications.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      909 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/js/plugins/oob.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6262 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/js/plugins/options2.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2790 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/js/plugins/popups.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10949 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/js/plugins/text2html.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9705 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/js/webclient_gui.js
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.520943 evennia-1.3.0/evennia/web/static/webclient/media/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3624 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/media/notification.wav
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.440944 evennia-1.3.0/evennia/web/static/website/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.524943 evennia-1.3.0/evennia/web/static/website/css/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/website/css/custom.css
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2013 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/website/css/website.css
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.524943 evennia-1.3.0/evennia/web/static/website/images/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      266 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/website/images/LICENCE
--rwxrwxr-x   0 griatch   (1000) griatch   (1000)    17938 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/website/images/evennia_logo.png
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    21167 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/website/images/evennia_logo_festive.png
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1406 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/website/images/favicon.ico
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.440944 evennia-1.3.0/evennia/web/templates/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.524943 evennia-1.3.0/evennia/web/templates/admin/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1621 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/admin/app_list.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6462 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/admin/frontpage.html
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.524943 evennia-1.3.0/evennia/web/templates/rest_framework/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      903 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/rest_framework/api.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      417 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/rest_framework/redoc.html
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.524943 evennia-1.3.0/evennia/web/templates/webclient/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7691 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/webclient/base.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1058 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/webclient/webclient.html
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.528943 evennia-1.3.0/evennia/web/templates/website/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      510 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/404.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      614 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/500.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4078 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/_menu.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3132 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/base.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2858 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/channel_detail.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2667 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/channel_list.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1402 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/character_form.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      546 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/character_list.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1139 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/character_manage_list.html
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.528943 evennia-1.3.0/evennia/web/templates/website/flatpages/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      341 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/flatpages/default.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1501 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/generic_form.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2715 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/help_detail.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5052 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/help_list.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5367 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/index.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      180 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/messages.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      900 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/object_confirm_delete.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1034 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/object_detail.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      546 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/object_list.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1484 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/pagination.html
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.528943 evennia-1.3.0/evennia/web/templates/website/registration/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      942 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/registration/logged_out.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1957 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/registration/login.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      612 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/registration/password_change_done.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1422 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/registration/password_change_form.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      813 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/registration/password_reset_complete.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1747 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/registration/password_reset_confirm.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1185 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/registration/password_reset_done.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      566 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/registration/password_reset_email.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1577 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/registration/password_reset_form.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1895 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/registration/register.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      671 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/tbi.html
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.528943 evennia-1.3.0/evennia/web/templatetags/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      287 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templatetags/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templatetags/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      550 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templatetags/addclass.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1631 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/urls.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.528943 evennia-1.3.0/evennia/web/utils/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/utils/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1256 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/utils/adminsite.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      596 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/utils/apache_wsgi.conf
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1815 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/utils/backends.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2035 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/utils/evennia_modpy_apache.conf
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1819 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/utils/evennia_wsgi_apache.conf
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4137 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/utils/general_context.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2712 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/utils/middleware.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2443 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/utils/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.532944 evennia-1.3.0/evennia/web/webclient/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/webclient/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      209 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/webclient/urls.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      795 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/webclient/views.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.532944 evennia-1.3.0/evennia/web/website/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       31 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/website/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5736 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/website/forms.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12503 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/website/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2575 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/website/urls.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.532944 evennia-1.3.0/evennia/web/website/views/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/website/views/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2120 2023-04-20 22:20:57.000000 evennia-1.3.0/evennia/web/website/views/accounts.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5329 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/website/views/channels.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8330 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/website/views/characters.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      311 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/website/views/errors.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11796 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/website/views/help.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4624 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/website/views/index.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2353 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/website/views/mixins.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9037 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/website/views/objects.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.444944 evennia-1.3.0/evennia.egg-info/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5239 2023-04-29 06:52:55.000000 evennia-1.3.0/evennia.egg-info/PKG-INFO
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    34356 2023-04-29 06:52:56.000000 evennia-1.3.0/evennia.egg-info/SOURCES.txt
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        1 2023-04-29 06:52:55.000000 evennia-1.3.0/evennia.egg-info/dependency_links.txt
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      550 2023-04-29 06:52:55.000000 evennia-1.3.0/evennia.egg-info/requires.txt
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        8 2023-04-29 06:52:55.000000 evennia-1.3.0/evennia.egg-info/top_level.txt
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3961 2023-04-29 06:31:51.000000 evennia-1.3.0/pyproject.toml
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       38 2023-04-29 06:52:56.532944 evennia-1.3.0/setup.cfg
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1388 2023-04-10 11:44:01.000000 evennia-1.3.0/setup.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.528713 evennia-2.0.0/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1531 2023-06-10 07:38:17.000000 evennia-2.0.0/LICENSE.txt
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5239 2023-06-10 07:51:20.528713 evennia-2.0.0/PKG-INFO
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3027 2023-06-10 07:38:17.000000 evennia-2.0.0/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.496713 evennia-2.0.0/bin/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.500713 evennia-2.0.0/bin/unix/
+-rwxrwxr-x   0 griatch   (1000) griatch   (1000)      210 2023-06-10 07:38:17.000000 evennia-2.0.0/bin/unix/evennia
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.500713 evennia-2.0.0/evennia/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        6 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/VERSION.txt
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      438 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/VERSION_REQS.txt
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    13414 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1839 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/__main__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.500713 evennia-2.0.0/evennia/accounts/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      214 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/accounts/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    67542 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/accounts/accounts.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    26018 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/accounts/bots.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9574 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/accounts/manager.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.500713 evennia-2.0.0/evennia/accounts/migrations/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7211 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/accounts/migrations/0001_initial.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      504 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/accounts/migrations/0002_move_defaults.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      612 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/accounts/migrations/0003_auto_20150209_2234.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2158 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/accounts/migrations/0004_auto_20150403_2339.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1010 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/accounts/migrations/0005_auto_20160905_0902.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1488 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/accounts/migrations/0006_auto_20170606_1731.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1927 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/accounts/migrations/0007_copy_player_to_account.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3944 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/accounts/migrations/0008_auto_20190128_1820.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      867 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/accounts/migrations/0009_auto_20191025_0831.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      467 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/accounts/migrations/0010_auto_20210520_2137.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4017 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/accounts/migrations/0011_convert_contrib_typeclass_paths.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      490 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/accounts/migrations/0012_defaultaccount_alter_accountdb_id_account_bot_and_more.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/accounts/migrations/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5740 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/accounts/models.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    16280 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/accounts/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.500713 evennia-2.0.0/evennia/commands/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      304 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/commands/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.500713 evennia-2.0.0/evennia/commands/_trial_temp/
+-rwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/commands/_trial_temp/_trial_marker
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    31705 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/commands/cmdhandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8287 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/commands/cmdparser.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    27219 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/commands/cmdset.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    26150 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/commands/cmdsethandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    29198 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/commands/command.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.500713 evennia-2.0.0/evennia/commands/default/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       87 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/commands/default/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    37414 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/commands/default/account.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    19605 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/commands/default/admin.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    23003 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/commands/default/batchprocess.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)   167198 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/commands/default/building.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2358 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/commands/default/cmdset_account.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3032 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/commands/default/cmdset_character.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      371 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/commands/default/cmdset_session.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      872 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/commands/default/cmdset_unloggedin.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    76302 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/commands/default/comms.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    22494 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/commands/default/general.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    39551 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/commands/default/help.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12788 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/commands/default/muxcommand.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3152 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/commands/default/syscommands.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    42195 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/commands/default/system.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    81792 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/commands/default/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17419 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/commands/default/unloggedin.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    46641 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/commands/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.504713 evennia-2.0.0/evennia/comms/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      207 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/comms/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    32556 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/comms/comms.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    16863 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/comms/managers.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.504713 evennia-2.0.0/evennia/comms/migrations/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3523 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/comms/migrations/0001_initial.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      500 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/comms/migrations/0002_msg_db_hide_from_objects.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3784 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/comms/migrations/0003_auto_20140917_0756.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      504 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/comms/migrations/0004_auto_20150118_1631.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      641 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/comms/migrations/0005_auto_20150223_1517.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      643 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/comms/migrations/0006_channeldb_db_object_subscriptions.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      615 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/comms/migrations/0007_msg_db_tags.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      434 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/comms/migrations/0008_auto_20160905_0902.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3872 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/comms/migrations/0009_auto_20160921_1731.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1079 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/comms/migrations/0010_auto_20161206_1912.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1029 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/comms/migrations/0011_auto_20170217_2039.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4563 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/comms/migrations/0011_auto_20170606_1731.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      267 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/comms/migrations/0012_merge_20170617_2017.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4778 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/comms/migrations/0013_auto_20170705_1726.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1442 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/comms/migrations/0014_auto_20170705_1736.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      943 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/comms/migrations/0015_auto_20170706_2041.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      462 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/comms/migrations/0016_auto_20180925_1735.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7069 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/comms/migrations/0017_auto_20190128_1820.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      665 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/comms/migrations/0018_auto_20191025_0831.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1713 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/comms/migrations/0019_auto_20210514_2032.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      916 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/comms/migrations/0020_auto_20210514_2210.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3635 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/comms/migrations/0021_auto_20210520_2137.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      711 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/comms/migrations/0022_defaultchannel_alter_channeldb_id_alter_msg_id_and_more.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/comms/migrations/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    22638 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/comms/models.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3166 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/comms/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.504713 evennia-2.0.0/evennia/contrib/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1895 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      198 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.504713 evennia-2.0.0/evennia/contrib/base_systems/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       80 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.504713 evennia-2.0.0/evennia/contrib/base_systems/awsstorage/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7695 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/awsstorage/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       48 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/awsstorage/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    32480 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/awsstorage/aws_s3_cdn.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    22503 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/awsstorage/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.504713 evennia-2.0.0/evennia/contrib/base_systems/building_menu/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    46012 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/building_menu/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      148 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/building_menu/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    42659 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/building_menu/building_menu.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6878 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/building_menu/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.504713 evennia-2.0.0/evennia/contrib/base_systems/color_markups/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2641 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/color_markups/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       84 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/color_markups/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8605 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/color_markups/color_markups.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3356 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/color_markups/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.504713 evennia-2.0.0/evennia/contrib/base_systems/components/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6397 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/components/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      952 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/components/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3915 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/components/component.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3762 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/components/dbfield.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11201 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/components/holder.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7237 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/components/signals.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14575 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/components/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.504713 evennia-2.0.0/evennia/contrib/base_systems/custom_gametime/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1549 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/custom_gametime/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      439 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/custom_gametime/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10390 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/custom_gametime/custom_gametime.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2017 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/custom_gametime/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.504713 evennia-2.0.0/evennia/contrib/base_systems/email_login/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1022 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/email_login/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      136 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/email_login/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1445 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/email_login/connection_screens.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10264 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/email_login/email_login.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1200 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/email_login/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.504713 evennia-2.0.0/evennia/contrib/base_systems/godotwebsocket/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8938 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/godotwebsocket/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      703 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/godotwebsocket/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3074 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/godotwebsocket/test_text2bbcode.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    27602 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/godotwebsocket/text2bbcode.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2690 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/godotwebsocket/webclient.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.504713 evennia-2.0.0/evennia/contrib/base_systems/ingame_python/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    40300 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/ingame_python/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      128 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/ingame_python/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6777 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/ingame_python/callbackhandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    21872 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/ingame_python/commands.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3048 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/ingame_python/eventfuncs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    23990 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/ingame_python/scripts.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    21618 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/ingame_python/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    34963 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/ingame_python/typeclasses.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8151 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/ingame_python/utils.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.504713 evennia-2.0.0/evennia/contrib/base_systems/menu_login/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      787 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/menu_login/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      143 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/menu_login/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1206 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/menu_login/connection_screens.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8781 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/menu_login/menu_login.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      265 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/menu_login/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.504713 evennia-2.0.0/evennia/contrib/base_systems/mux_comms_cmds/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1936 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/mux_comms_cmds/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      104 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/mux_comms_cmds/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    16012 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/mux_comms_cmds/mux_comms_cmds.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2298 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/mux_comms_cmds/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.504713 evennia-2.0.0/evennia/contrib/base_systems/unixcommand/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2241 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/unixcommand/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       94 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/unixcommand/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1654 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/unixcommand/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9989 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/base_systems/unixcommand/unixcommand.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.504713 evennia-2.0.0/evennia/contrib/full_systems/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       75 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/full_systems/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       48 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/full_systems/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.504713 evennia-2.0.0/evennia/contrib/full_systems/evscaperoom/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5210 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/full_systems/evscaperoom/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      266 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/full_systems/evscaperoom/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    22699 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/full_systems/evscaperoom/commands.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10565 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/full_systems/evscaperoom/menu.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    34348 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/full_systems/evscaperoom/objects.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7942 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/full_systems/evscaperoom/room.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      753 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/full_systems/evscaperoom/scripts.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9582 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/full_systems/evscaperoom/state.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.504713 evennia-2.0.0/evennia/contrib/full_systems/evscaperoom/states/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1203 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/full_systems/evscaperoom/states/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4168 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/full_systems/evscaperoom/states/state_001_start.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10461 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/full_systems/evscaperoom/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6112 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/full_systems/evscaperoom/utils.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.504713 evennia-2.0.0/evennia/contrib/game_systems/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      269 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/game_systems/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/game_systems/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.504713 evennia-2.0.0/evennia/contrib/game_systems/barter/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4322 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/game_systems/barter/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       80 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/game_systems/barter/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    29726 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/game_systems/barter/barter.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5976 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/game_systems/barter/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.504713 evennia-2.0.0/evennia/contrib/game_systems/clothing/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4249 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/game_systems/clothing/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      199 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/game_systems/clothing/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    24574 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/game_systems/clothing/clothing.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4816 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/game_systems/clothing/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.504713 evennia-2.0.0/evennia/contrib/game_systems/containers/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2508 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/game_systems/containers/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       66 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/game_systems/containers/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9971 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/game_systems/containers/containers.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2584 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/game_systems/containers/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.504713 evennia-2.0.0/evennia/contrib/game_systems/cooldowns/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2084 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/game_systems/cooldowns/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       88 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/game_systems/cooldowns/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7580 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/game_systems/cooldowns/cooldowns.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6135 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/game_systems/cooldowns/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.508714 evennia-2.0.0/evennia/contrib/game_systems/crafting/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11186 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/game_systems/crafting/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      233 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/game_systems/crafting/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    41597 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/game_systems/crafting/crafting.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17892 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/game_systems/crafting/example_recipes.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    24911 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/game_systems/crafting/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.508714 evennia-2.0.0/evennia/contrib/game_systems/gendersub/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1986 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/game_systems/gendersub/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      123 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/game_systems/gendersub/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5096 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/game_systems/gendersub/gendersub.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1091 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/game_systems/gendersub/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.508714 evennia-2.0.0/evennia/contrib/game_systems/mail/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1567 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/game_systems/mail/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      115 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/game_systems/mail/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14841 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/game_systems/mail/mail.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1852 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/game_systems/mail/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.508714 evennia-2.0.0/evennia/contrib/game_systems/multidescer/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      932 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/game_systems/multidescer/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       83 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/game_systems/multidescer/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9951 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/game_systems/multidescer/multidescer.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1404 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/game_systems/multidescer/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.508714 evennia-2.0.0/evennia/contrib/game_systems/puzzles/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2181 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/game_systems/puzzles/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      124 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/game_systems/puzzles/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    27837 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/game_systems/puzzles/puzzles.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    41328 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/game_systems/puzzles/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.508714 evennia-2.0.0/evennia/contrib/game_systems/turnbattle/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2940 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/game_systems/turnbattle/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      209 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/game_systems/turnbattle/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    28762 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/game_systems/turnbattle/tb_basic.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    23139 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/game_systems/turnbattle/tb_equip.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    37446 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/game_systems/turnbattle/tb_items.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    30705 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/game_systems/turnbattle/tb_magic.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    38339 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/game_systems/turnbattle/tb_range.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    29682 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/game_systems/turnbattle/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.508714 evennia-2.0.0/evennia/contrib/grid/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       84 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/grid/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       81 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/grid/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.508714 evennia-2.0.0/evennia/contrib/grid/extended_room/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6348 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/grid/extended_room/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      454 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/grid/extended_room/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    33817 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/grid/extended_room/extended_room.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12997 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/grid/extended_room/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.508714 evennia-2.0.0/evennia/contrib/grid/ingame_map_display/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1358 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/grid/ingame_map_display/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       92 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/grid/ingame_map_display/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10572 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/grid/ingame_map_display/ingame_map_display.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1404 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/grid/ingame_map_display/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.508714 evennia-2.0.0/evennia/contrib/grid/mapbuilder/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9672 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/grid/mapbuilder/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       87 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/grid/mapbuilder/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17398 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/grid/mapbuilder/mapbuilder.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6435 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/grid/mapbuilder/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.508714 evennia-2.0.0/evennia/contrib/grid/simpledoor/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1356 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/grid/simpledoor/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      129 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/grid/simpledoor/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5838 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/grid/simpledoor/simpledoor.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1079 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/grid/simpledoor/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.508714 evennia-2.0.0/evennia/contrib/grid/slow_exit/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1730 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/grid/slow_exit/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      203 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/grid/slow_exit/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5046 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/grid/slow_exit/slow_exit.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      824 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/grid/slow_exit/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.508714 evennia-2.0.0/evennia/contrib/grid/wilderness/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4932 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/grid/wilderness/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      394 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/grid/wilderness/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6026 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/grid/wilderness/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    28916 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/grid/wilderness/wilderness.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.508714 evennia-2.0.0/evennia/contrib/grid/xyzgrid/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    54690 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/grid/xyzgrid/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      202 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/grid/xyzgrid/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    20837 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/grid/xyzgrid/commands.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7822 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/grid/xyzgrid/example.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    13723 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/grid/xyzgrid/launchcmd.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1145 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/grid/xyzgrid/prototypes.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    42072 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/grid/xyzgrid/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1043 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/grid/xyzgrid/utils.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    40413 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/grid/xyzgrid/xymap.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    52070 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/grid/xyzgrid/xymap_legend.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10484 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/grid/xyzgrid/xyzgrid.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    24616 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/grid/xyzgrid/xyzroom.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.508714 evennia-2.0.0/evennia/contrib/rpg/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      406 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/rpg/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/rpg/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.508714 evennia-2.0.0/evennia/contrib/rpg/buffs/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    22364 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/rpg/buffs/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/rpg/buffs/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    45607 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/rpg/buffs/buff.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3893 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/rpg/buffs/samplebuffs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    16470 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/rpg/buffs/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.508714 evennia-2.0.0/evennia/contrib/rpg/character_creator/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3924 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/rpg/character_creator/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      176 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/rpg/character_creator/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8148 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/rpg/character_creator/character_creator.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    21006 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/rpg/character_creator/example_menu.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1552 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/rpg/character_creator/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.508714 evennia-2.0.0/evennia/contrib/rpg/dice/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1442 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/rpg/dice/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      177 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/rpg/dice/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10272 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/rpg/dice/dice.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      901 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/rpg/dice/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.508714 evennia-2.0.0/evennia/contrib/rpg/health_bar/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1264 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/rpg/health_bar/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       94 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/rpg/health_bar/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4913 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/rpg/health_bar/health_bar.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1634 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/rpg/health_bar/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.508714 evennia-2.0.0/evennia/contrib/rpg/rpsystem/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9938 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/rpg/rpsystem/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      793 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/rpg/rpsystem/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    24722 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/rpg/rpsystem/rplanguage.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    65825 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/rpg/rpsystem/rpsystem.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14981 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/rpg/rpsystem/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.508714 evennia-2.0.0/evennia/contrib/rpg/traits/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14246 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/rpg/traits/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      294 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/rpg/traits/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    37184 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/rpg/traits/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    54252 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/rpg/traits/traits.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.508714 evennia-2.0.0/evennia/contrib/tutorials/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      151 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       81 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.508714 evennia-2.0.0/evennia/contrib/tutorials/batchprocessor/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1623 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/batchprocessor/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       50 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/batchprocessor/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1567 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/batchprocessor/example_batch_cmds.ev
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3618 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/batchprocessor/example_batch_code.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.508714 evennia-2.0.0/evennia/contrib/tutorials/bodyfunctions/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      471 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/bodyfunctions/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      104 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/bodyfunctions/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2311 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/bodyfunctions/bodyfunctions.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3324 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/bodyfunctions/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.512714 evennia-2.0.0/evennia/contrib/tutorials/evadventure/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1180 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/evadventure/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      164 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/evadventure/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.512714 evennia-2.0.0/evennia/contrib/tutorials/evadventure/batchscripts/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       73 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/evadventure/batchscripts/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1820 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/evadventure/batchscripts/turnbased_combat_demo.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1436 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/evadventure/batchscripts/twitch_combat_demo.ev
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3996 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/evadventure/build_techdemo.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/evadventure/build_world.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12610 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/evadventure/characters.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11199 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/evadventure/chargen.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17122 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/evadventure/combat_base.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    28417 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/evadventure/combat_turnbased.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    18301 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/evadventure/combat_twitch.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12500 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/evadventure/commands.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17918 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/evadventure/dungeon.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1742 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/evadventure/enums.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14608 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/evadventure/equipment.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12264 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/evadventure/npcs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11174 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/evadventure/objects.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8743 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/evadventure/quests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11708 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/evadventure/random_tables.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3154 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/evadventure/rooms.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12169 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/evadventure/rules.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17153 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/evadventure/shops.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.512714 evennia-2.0.0/evennia/contrib/tutorials/evadventure/tests/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       48 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/evadventure/tests/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1389 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/evadventure/tests/mixins.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1266 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/evadventure/tests/test_characters.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2151 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/evadventure/tests/test_chargen.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    28061 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/evadventure/tests/test_combat.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3741 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/evadventure/tests/test_commands.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3356 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/evadventure/tests/test_dungeon.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7811 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/evadventure/tests/test_equipment.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      542 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/evadventure/tests/test_npcs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4629 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/evadventure/tests/test_quests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2237 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/evadventure/tests/test_rooms.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8083 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/evadventure/tests/test_rules.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      712 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/evadventure/tests/test_utils.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1485 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/evadventure/utils.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.512714 evennia-2.0.0/evennia/contrib/tutorials/mirror/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      429 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/mirror/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       83 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/mirror/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2235 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/mirror/mirror.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.512714 evennia-2.0.0/evennia/contrib/tutorials/red_button/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1344 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/red_button/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       94 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/red_button/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    18609 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/red_button/red_button.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.512714 evennia-2.0.0/evennia/contrib/tutorials/talking_npc/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      722 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/talking_npc/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      124 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/talking_npc/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3697 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/talking_npc/talking_npc.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      449 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/talking_npc/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.512714 evennia-2.0.0/evennia/contrib/tutorials/tutorial_world/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4302 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/tutorial_world/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      125 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/tutorial_world/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    50297 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/tutorial_world/build.ev
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    25293 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/tutorial_world/intro_menu.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    16130 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/tutorial_world/mob.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    42155 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/tutorial_world/objects.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    42922 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/tutorial_world/rooms.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7342 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/tutorials/tutorial_world/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.512714 evennia-2.0.0/evennia/contrib/utils/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       67 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/utils/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/utils/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.512714 evennia-2.0.0/evennia/contrib/utils/auditing/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3303 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/utils/auditing/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/utils/auditing/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2065 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/utils/auditing/outputs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8515 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/utils/auditing/server.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6047 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/utils/auditing/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.512714 evennia-2.0.0/evennia/contrib/utils/fieldfill/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5816 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/utils/fieldfill/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      288 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/utils/fieldfill/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    26382 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/utils/fieldfill/fieldfill.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.512714 evennia-2.0.0/evennia/contrib/utils/git_integration/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3139 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/utils/git_integration/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       86 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/utils/git_integration/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7737 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/utils/git_integration/git_integration.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2828 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/utils/git_integration/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.512714 evennia-2.0.0/evennia/contrib/utils/name_generator/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9815 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/utils/name_generator/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/utils/name_generator/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)   232619 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/utils/name_generator/btn_givennames.txt
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    56503 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/utils/name_generator/btn_surnames.txt
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14447 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/utils/name_generator/namegen.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4914 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/utils/name_generator/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.512714 evennia-2.0.0/evennia/contrib/utils/random_string_generator/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2165 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/utils/random_string_generator/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      268 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/utils/random_string_generator/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12595 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/utils/random_string_generator/random_string_generator.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      737 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/utils/random_string_generator/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.512714 evennia-2.0.0/evennia/contrib/utils/tree_select/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5935 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/utils/tree_select/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      109 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/utils/tree_select/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2199 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/utils/tree_select/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    20930 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/contrib/utils/tree_select/tree_select.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.512714 evennia-2.0.0/evennia/game_template/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1521 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.512714 evennia-2.0.0/evennia/game_template/commands/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      676 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/commands/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/commands/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7738 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/commands/command.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2636 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/commands/default_cmdsets.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      551 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/gitignore
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.512714 evennia-2.0.0/evennia/game_template/server/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1718 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/server/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/server/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.512714 evennia-2.0.0/evennia/game_template/server/conf/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/server/conf/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      629 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/server/conf/at_initial_setup.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2154 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/server/conf/at_search.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1369 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/server/conf/at_server_startstop.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2174 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/server/conf/cmdparser.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1500 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/server/conf/connection_screens.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1159 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/server/conf/inlinefuncs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1419 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/server/conf/inputfuncs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1065 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/server/conf/lockfuncs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4009 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/server/conf/mssp.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      709 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/server/conf/portal_services_plugins.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      714 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/server/conf/secret_settings.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      705 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/server/conf/server_services_plugins.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1347 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/server/conf/serversession.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1500 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/server/conf/settings.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1185 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/server/conf/web_plugins.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.512714 evennia-2.0.0/evennia/game_template/server/logs/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      839 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/server/logs/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.512714 evennia-2.0.0/evennia/game_template/typeclasses/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      733 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/typeclasses/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/typeclasses/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3774 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/typeclasses/accounts.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2920 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/typeclasses/channels.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1525 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/typeclasses/characters.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2044 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/typeclasses/exits.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8847 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/typeclasses/objects.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      551 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/typeclasses/rooms.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4394 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/typeclasses/scripts.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.512714 evennia-2.0.0/evennia/game_template/web/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2939 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/web/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/web/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.512714 evennia-2.0.0/evennia/game_template/web/admin/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      296 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/web/admin/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/web/admin/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      520 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/web/admin/urls.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.512714 evennia-2.0.0/evennia/game_template/web/api/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/web/api/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.512714 evennia-2.0.0/evennia/game_template/web/static/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      849 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/web/static/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.496713 evennia-2.0.0/evennia/game_template/web/static/rest_framework/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.512714 evennia-2.0.0/evennia/game_template/web/static/rest_framework/css/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       53 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/web/static/rest_framework/css/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.516713 evennia-2.0.0/evennia/game_template/web/static/rest_framework/images/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       47 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/web/static/rest_framework/images/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.496713 evennia-2.0.0/evennia/game_template/web/static/webclient/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.516713 evennia-2.0.0/evennia/game_template/web/static/webclient/css/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      132 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/web/static/webclient/css/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.516713 evennia-2.0.0/evennia/game_template/web/static/webclient/js/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      143 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/web/static/webclient/js/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.496713 evennia-2.0.0/evennia/game_template/web/static/website/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.516713 evennia-2.0.0/evennia/game_template/web/static/website/css/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      129 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/web/static/website/css/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.516713 evennia-2.0.0/evennia/game_template/web/static/website/images/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      135 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/web/static/website/images/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.516713 evennia-2.0.0/evennia/game_template/web/templates/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      760 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/web/templates/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.516713 evennia-2.0.0/evennia/game_template/web/templates/rest_framework/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       58 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/web/templates/rest_framework/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.516713 evennia-2.0.0/evennia/game_template/web/templates/webclient/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      223 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/web/templates/webclient/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.516713 evennia-2.0.0/evennia/game_template/web/templates/website/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      217 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/web/templates/website/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.516713 evennia-2.0.0/evennia/game_template/web/templates/website/flatpages/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      185 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/web/templates/website/flatpages/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.516713 evennia-2.0.0/evennia/game_template/web/templates/website/registration/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      152 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/web/templates/website/registration/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1099 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/web/urls.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.516713 evennia-2.0.0/evennia/game_template/web/webclient/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1102 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/web/webclient/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/web/webclient/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      539 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/web/webclient/urls.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.516713 evennia-2.0.0/evennia/game_template/web/website/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1262 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/web/website/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/web/website/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      509 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/web/website/urls.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.516713 evennia-2.0.0/evennia/game_template/web/website/views/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/web/website/views/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.516713 evennia-2.0.0/evennia/game_template/world/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      467 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/world/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/world/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      999 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/world/batch_cmds.ev
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2186 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/world/help_entries.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3646 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/game_template/world/prototypes.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.516713 evennia-2.0.0/evennia/help/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      217 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/help/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8013 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/help/filehelp.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6229 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/help/manager.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.516713 evennia-2.0.0/evennia/help/migrations/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2222 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/help/migrations/0001_initial.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      577 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/help/migrations/0002_auto_20170606_1731.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1688 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/help/migrations/0003_auto_20190128_1820.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      540 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/help/migrations/0004_auto_20210520_2137.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1166 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/help/migrations/0005_auto_20210530_1818.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      473 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/help/migrations/0006_alter_helpentry_id.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/help/migrations/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9729 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/help/models.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3736 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/help/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7673 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/help/utils.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.516713 evennia-2.0.0/evennia/locale/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2686 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/locale/README
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.500713 evennia-2.0.0/evennia/locale/de/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.516713 evennia-2.0.0/evennia/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10764 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14475 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/locale/de/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.500713 evennia-2.0.0/evennia/locale/es/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.516713 evennia-2.0.0/evennia/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3821 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    30981 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/locale/es/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.500713 evennia-2.0.0/evennia/locale/fr/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.516713 evennia-2.0.0/evennia/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    26255 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    38581 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/locale/fr/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.500713 evennia-2.0.0/evennia/locale/it/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.516713 evennia-2.0.0/evennia/locale/it/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6944 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/locale/it/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    35844 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/locale/it/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.500713 evennia-2.0.0/evennia/locale/ko/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.516713 evennia-2.0.0/evennia/locale/ko/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3569 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/locale/ko/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    30924 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/locale/ko/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.500713 evennia-2.0.0/evennia/locale/la/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.516713 evennia-2.0.0/evennia/locale/la/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6537 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/locale/la/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    32786 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/locale/la/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.500713 evennia-2.0.0/evennia/locale/pl/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.516713 evennia-2.0.0/evennia/locale/pl/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1631 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/locale/pl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    28236 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/locale/pl/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.500713 evennia-2.0.0/evennia/locale/pt/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.516713 evennia-2.0.0/evennia/locale/pt/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    25584 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/locale/pt/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    42122 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/locale/pt/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.500713 evennia-2.0.0/evennia/locale/ru/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.516713 evennia-2.0.0/evennia/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2281 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/locale/ru/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    29419 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/locale/ru/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.500713 evennia-2.0.0/evennia/locale/sv/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.516713 evennia-2.0.0/evennia/locale/sv/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    29036 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/locale/sv/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    43353 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/locale/sv/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.500713 evennia-2.0.0/evennia/locale/zh/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.516713 evennia-2.0.0/evennia/locale/zh/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3300 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/locale/zh/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    30540 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/locale/zh/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.516713 evennia-2.0.0/evennia/locks/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      240 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/locks/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    22093 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/locks/lockfuncs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    26966 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/locks/lockhandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    13732 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/locks/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.516713 evennia-2.0.0/evennia/objects/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      120 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/objects/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    29704 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/objects/manager.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.516713 evennia-2.0.0/evennia/objects/migrations/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4315 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/objects/migrations/0001_initial.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1193 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/objects/migrations/0002_auto_20140917_0756.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      810 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/objects/migrations/0003_defaultcharacter_defaultexit_defaultobject_defaultroom.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      530 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/objects/migrations/0004_auto_20150118_1622.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      410 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/objects/migrations/0005_auto_20150403_2339.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1599 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/objects/migrations/0006_auto_20170606_1731.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1203 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/objects/migrations/0007_objectdb_db_account.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      757 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/objects/migrations/0008_auto_20170705_1736.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      643 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/objects/migrations/0009_remove_objectdb_db_player.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5028 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/objects/migrations/0010_auto_20190128_1820.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1351 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/objects/migrations/0011_auto_20191025_0831.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4011 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/objects/migrations/0012_convert_contrib_typeclass_paths.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      488 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/objects/migrations/0013_defaultobject_alter_objectdb_id_defaultcharacter_and_more.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/objects/migrations/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    13399 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/objects/models.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)   118892 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/objects/objects.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17072 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/objects/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.516713 evennia-2.0.0/evennia/prototypes/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6567 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/prototypes/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/prototypes/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    92110 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/prototypes/menus.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2912 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/prototypes/protfuncs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    46537 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/prototypes/prototypes.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    42860 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/prototypes/spawner.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    39636 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/prototypes/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.516713 evennia-2.0.0/evennia/scripts/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      229 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/scripts/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11275 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/scripts/manager.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.520713 evennia-2.0.0/evennia/scripts/migrations/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4762 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/scripts/migrations/0001_initial.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      675 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/scripts/migrations/0002_auto_20150118_1625.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1507 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/scripts/migrations/0003_checksessions_defaultscript_donothing_scriptbase_store_validatechannelhandler_validateidmappercache_.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      861 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/scripts/migrations/0004_auto_20150306_1354.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      430 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/scripts/migrations/0005_auto_20150306_1441.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      710 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/scripts/migrations/0006_auto_20150310_2249.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      396 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/scripts/migrations/0007_auto_20150403_2339.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      913 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/scripts/migrations/0008_auto_20170606_1731.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1271 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/scripts/migrations/0009_scriptdb_db_account.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      757 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/scripts/migrations/0010_auto_20170705_1736.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      596 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/scripts/migrations/0011_remove_scriptdb_db_player.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4655 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/scripts/migrations/0012_auto_20190128_1820.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      666 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/scripts/migrations/0013_auto_20191025_0831.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      752 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/scripts/migrations/0014_auto_20210520_2137.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3329 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/scripts/migrations/0015_convert_contrib_paths.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      478 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/scripts/migrations/0016_scriptbase_alter_scriptdb_id_defaultscript_and_more.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/scripts/migrations/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6311 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/scripts/models.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8746 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/scripts/monitorhandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5326 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/scripts/scripthandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    27441 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/scripts/scripts.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    20801 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/scripts/taskhandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10678 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/scripts/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    24661 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/scripts/tickerhandler.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.520713 evennia-2.0.0/evennia/server/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      234 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8697 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/amp_client.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    16629 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/connection_wizard.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7955 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/deprecations.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    79833 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/evennia_launcher.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.520713 evennia-2.0.0/evennia/server/game_index_client/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4321 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/game_index_client/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       45 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/game_index_client/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6256 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/game_index_client/client.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1990 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/game_index_client/service.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7622 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/initial_setup.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    19709 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/inputfuncs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1708 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/manager.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.520713 evennia-2.0.0/evennia/server/migrations/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      812 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/migrations/0001_initial.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1363 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/migrations/0002_auto_20190128_2311.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      478 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/migrations/0003_alter_serverconfig_id.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/migrations/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3818 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/models.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.520713 evennia-2.0.0/evennia/server/portal/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/portal/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17922 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/portal/amp.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17520 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/portal/amp_server.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    18478 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/portal/discord.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11345 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/portal/grapevine.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14242 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/portal/irc.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2571 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/portal/mccp.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3882 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/portal/mssp.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2341 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/portal/mxp.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2359 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/portal/naws.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    16018 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/portal/portal.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17163 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/portal/portalsessionhandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4450 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/portal/rss.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    15920 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/portal/ssh.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3319 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/portal/ssl.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1785 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/portal/suppress_ga.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17379 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/portal/telnet.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    15609 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/portal/telnet_oob.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4861 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/portal/telnet_ssl.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14725 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/portal/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7073 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/portal/ttype.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11403 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/portal/webclient.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    15897 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/portal/webclient_ajax.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.520713 evennia-2.0.0/evennia/server/profiling/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      212 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/profiling/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/profiling/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    20881 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/profiling/dummyrunner.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9427 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/profiling/dummyrunner_settings.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3924 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/profiling/memplot.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1375 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/profiling/settings_mixin.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1095 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/profiling/test_queries.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5371 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/profiling/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1345 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/profiling/timetrace.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    28633 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/server.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14599 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/serversession.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5616 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/session.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    30009 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/sessionhandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4935 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/signals.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.520713 evennia-2.0.0/evennia/server/tests/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/tests/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4721 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/tests/test_amp_connection.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      521 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/tests/test_initial_setup.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7305 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/tests/test_launcher.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4444 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/tests/test_misc.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9256 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/tests/test_server.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1369 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/tests/testrunner.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7101 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/throttle.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2763 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/validators.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8653 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/server/webserver.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    60833 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/settings_default.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.520713 evennia-2.0.0/evennia/typeclasses/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      434 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/typeclasses/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    64398 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/typeclasses/attributes.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    31304 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/typeclasses/managers.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.520713 evennia-2.0.0/evennia/typeclasses/migrations/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6101 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/typeclasses/migrations/0001_initial.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      768 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/typeclasses/migrations/0002_auto_20150109_0913.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2266 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/typeclasses/migrations/0003_defaultcharacter_defaultexit_defaultguest_defaultobject_defaultplayer_defaultroom_defaultscript_dono.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      833 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/typeclasses/migrations/0004_auto_20151101_1759.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      922 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/typeclasses/migrations/0005_auto_20160625_1812.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1444 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/typeclasses/migrations/0006_auto_add_dbmodel_value_for_tags_attributes.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3899 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/typeclasses/migrations/0007_tag_migrations_may_be_slow.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1699 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/typeclasses/migrations/0008_lock_and_perm_rename.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4230 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/typeclasses/migrations/0009_rename_player_cmdsets_typeclasses.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1993 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/typeclasses/migrations/0010_delete_old_player_tables.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5265 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/typeclasses/migrations/0011_auto_20190128_1820.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      821 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/typeclasses/migrations/0012_attrs_to_picklev4_may_be_slow.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      592 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/typeclasses/migrations/0013_auto_20191015_1922.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      592 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/typeclasses/migrations/0014_alter_tag_db_category.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      362 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/typeclasses/migrations/0015_alter_attribute_options.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      722 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/typeclasses/migrations/0016_alter_attribute_id_alter_tag_id.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/typeclasses/migrations/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    37156 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/typeclasses/models.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    30224 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/typeclasses/tags.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17813 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/typeclasses/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.524713 evennia-2.0.0/evennia/utils/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      320 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    51381 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/ansi.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    15392 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/batchprocessors.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8077 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/containers.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10242 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/create.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    32812 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/dbserialize.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    41419 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/eveditor.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2734 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/evennia-mode.el
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    21081 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/evform.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    78957 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/evmenu.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    18330 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/evmore.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    65173 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/evtable.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    53272 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/funcparser.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8754 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/gametime.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.524713 evennia-2.0.0/evennia/utils/idmapper/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1309 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/idmapper/LICENSE.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1097 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/idmapper/README_evennia.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1992 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/idmapper/README_orig.rst
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       64 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/idmapper/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1181 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/idmapper/manager.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    24820 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/idmapper/models.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2876 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/idmapper/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    18789 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/logger.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10265 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/optionclasses.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6455 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/optionhandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11093 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/picklefield.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14179 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/search.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    25088 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/test_resources.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.524713 evennia-2.0.0/evennia/utils/tests/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/tests/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.524713 evennia-2.0.0/evennia/utils/tests/data/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/tests/data/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      274 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/tests/data/broken_script.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1125 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/tests/data/evform_example.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6245 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/tests/data/evmenu_example.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      382 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/tests/data/prototypes_example.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1608 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/tests/test_ansi.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7052 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/tests/test_batchprocessors.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3463 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/tests/test_containers.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7032 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/tests/test_create_functions.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7888 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/tests/test_dbserialize.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11752 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/tests/test_eveditor.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12172 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/tests/test_evform.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11763 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/tests/test_evmenu.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12101 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/tests/test_evtable.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    30844 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/tests/test_funcparser.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3942 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/tests/test_gametime.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4460 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/tests/test_search.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    13564 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/tests/test_tagparsing.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5509 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/tests/test_text2html.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    29937 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/tests/test_utils.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6371 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/tests/test_validatorfuncs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12235 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/text2html.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    97272 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/utils.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9489 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/validatorfuncs.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.524713 evennia-2.0.0/evennia/utils/verb_conjugation/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    18011 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/verb_conjugation/LICENSE.txt
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/verb_conjugation/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9885 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/verb_conjugation/conjugate.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11298 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/verb_conjugation/pronouns.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10493 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/verb_conjugation/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)   554408 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/utils/verb_conjugation/verbs.txt
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.524713 evennia-2.0.0/evennia/web/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1150 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      127 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.524713 evennia-2.0.0/evennia/web/admin/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      428 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/admin/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14125 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/admin/accounts.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8627 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/admin/attributes.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8508 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/admin/comms.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      593 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/admin/frontpage.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1889 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/admin/help.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11915 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/admin/objects.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4499 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/admin/scripts.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      508 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/admin/server.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8955 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/admin/tags.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      878 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/admin/urls.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2884 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/admin/utils.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.524713 evennia-2.0.0/evennia/web/api/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7674 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/api/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/api/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4268 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/api/filters.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3949 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/api/permissions.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      277 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/api/root.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9905 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/api/serializers.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8148 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/api/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2293 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/api/urls.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5828 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/api/views.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.500713 evennia-2.0.0/evennia/web/static/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.500713 evennia-2.0.0/evennia/web/static/rest_framework/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.524713 evennia-2.0.0/evennia/web/static/rest_framework/css/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      298 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/static/rest_framework/css/api.css
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.524713 evennia-2.0.0/evennia/web/static/rest_framework/images/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1406 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/static/rest_framework/images/favicon.ico
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.500713 evennia-2.0.0/evennia/web/static/webclient/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.524713 evennia-2.0.0/evennia/web/static/webclient/css/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2104 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/static/webclient/css/goldenlayout.css
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    27268 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/static/webclient/css/webclient.css
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.524713 evennia-2.0.0/evennia/web/static/webclient/fonts/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    22208 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/static/webclient/fonts/DejaVuSansMono-webfont.woff
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      185 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/static/webclient/fonts/DejaVuSansMono.css
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.524713 evennia-2.0.0/evennia/web/static/webclient/js/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    18546 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/static/webclient/js/evennia.js
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.528713 evennia-2.0.0/evennia/web/static/webclient/js/plugins/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      563 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/static/webclient/js/plugins/clienthelp.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3914 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/static/webclient/js/plugins/default_in.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1958 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/static/webclient/js/plugins/default_out.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      345 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/static/webclient/js/plugins/default_unload.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3785 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/static/webclient/js/plugins/font.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    29030 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/static/webclient/js/plugins/goldenlayout.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2114 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/static/webclient/js/plugins/goldenlayout_default_config.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2981 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/static/webclient/js/plugins/history.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5031 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/static/webclient/js/plugins/hotbuttons.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1969 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/static/webclient/js/plugins/html.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1912 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/static/webclient/js/plugins/iframe.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4666 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/static/webclient/js/plugins/message_routing.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4611 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/static/webclient/js/plugins/multimedia.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2842 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/static/webclient/js/plugins/notifications.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      909 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/static/webclient/js/plugins/oob.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6262 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/static/webclient/js/plugins/options2.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2790 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/static/webclient/js/plugins/popups.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10949 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/static/webclient/js/plugins/text2html.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9705 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/static/webclient/js/webclient_gui.js
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.528713 evennia-2.0.0/evennia/web/static/webclient/media/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3624 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/static/webclient/media/notification.wav
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.500713 evennia-2.0.0/evennia/web/static/website/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.528713 evennia-2.0.0/evennia/web/static/website/css/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/static/website/css/custom.css
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2013 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/static/website/css/website.css
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.528713 evennia-2.0.0/evennia/web/static/website/images/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      266 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/static/website/images/LICENCE
+-rwxrwxr-x   0 griatch   (1000) griatch   (1000)    17938 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/static/website/images/evennia_logo.png
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    21167 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/static/website/images/evennia_logo_festive.png
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1406 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/static/website/images/favicon.ico
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.500713 evennia-2.0.0/evennia/web/templates/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.528713 evennia-2.0.0/evennia/web/templates/admin/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1621 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/templates/admin/app_list.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6462 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/templates/admin/frontpage.html
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.528713 evennia-2.0.0/evennia/web/templates/rest_framework/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      903 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/templates/rest_framework/api.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      417 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/templates/rest_framework/redoc.html
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.528713 evennia-2.0.0/evennia/web/templates/webclient/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7691 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/templates/webclient/base.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1058 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/templates/webclient/webclient.html
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.528713 evennia-2.0.0/evennia/web/templates/website/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      510 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/templates/website/404.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      614 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/templates/website/500.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4078 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/templates/website/_menu.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3132 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/templates/website/base.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2858 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/templates/website/channel_detail.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2667 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/templates/website/channel_list.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1402 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/templates/website/character_form.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      546 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/templates/website/character_list.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1139 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/templates/website/character_manage_list.html
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.528713 evennia-2.0.0/evennia/web/templates/website/flatpages/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      341 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/templates/website/flatpages/default.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1501 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/templates/website/generic_form.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2715 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/templates/website/help_detail.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5052 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/templates/website/help_list.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5367 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/templates/website/index.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      180 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/templates/website/messages.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      900 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/templates/website/object_confirm_delete.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1034 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/templates/website/object_detail.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      546 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/templates/website/object_list.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1484 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/templates/website/pagination.html
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.528713 evennia-2.0.0/evennia/web/templates/website/registration/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      942 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/templates/website/registration/logged_out.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1957 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/templates/website/registration/login.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      612 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/templates/website/registration/password_change_done.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1422 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/templates/website/registration/password_change_form.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      813 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/templates/website/registration/password_reset_complete.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1747 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/templates/website/registration/password_reset_confirm.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1185 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/templates/website/registration/password_reset_done.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      566 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/templates/website/registration/password_reset_email.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1577 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/templates/website/registration/password_reset_form.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1895 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/templates/website/registration/register.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      671 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/templates/website/tbi.html
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.528713 evennia-2.0.0/evennia/web/templatetags/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      287 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/templatetags/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/templatetags/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      550 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/templatetags/addclass.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1631 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/urls.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.528713 evennia-2.0.0/evennia/web/utils/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/utils/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1256 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/utils/adminsite.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      596 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/utils/apache_wsgi.conf
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1815 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/utils/backends.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2035 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/utils/evennia_modpy_apache.conf
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1819 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/utils/evennia_wsgi_apache.conf
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4137 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/utils/general_context.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2712 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/utils/middleware.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2443 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/utils/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.528713 evennia-2.0.0/evennia/web/webclient/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/webclient/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      209 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/webclient/urls.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      795 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/webclient/views.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.528713 evennia-2.0.0/evennia/web/website/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       31 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/website/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5736 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/website/forms.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12503 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/website/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2575 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/website/urls.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.528713 evennia-2.0.0/evennia/web/website/views/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/website/views/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2120 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/website/views/accounts.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5329 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/website/views/channels.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8330 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/website/views/characters.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      311 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/website/views/errors.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11796 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/website/views/help.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4611 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/website/views/index.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2353 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/website/views/mixins.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9037 2023-06-10 07:38:17.000000 evennia-2.0.0/evennia/web/website/views/objects.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 07:51:20.500713 evennia-2.0.0/evennia.egg-info/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5239 2023-06-10 07:51:20.000000 evennia-2.0.0/evennia.egg-info/PKG-INFO
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    34996 2023-06-10 07:51:20.000000 evennia-2.0.0/evennia.egg-info/SOURCES.txt
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        1 2023-06-10 07:51:20.000000 evennia-2.0.0/evennia.egg-info/dependency_links.txt
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      550 2023-06-10 07:51:20.000000 evennia-2.0.0/evennia.egg-info/requires.txt
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        8 2023-06-10 07:51:20.000000 evennia-2.0.0/evennia.egg-info/top_level.txt
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3961 2023-06-10 07:38:17.000000 evennia-2.0.0/pyproject.toml
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       38 2023-06-10 07:51:20.528713 evennia-2.0.0/setup.cfg
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1388 2023-06-10 07:38:17.000000 evennia-2.0.0/setup.py
```

### Comparing `evennia-1.3.0/LICENSE.txt` & `evennia-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/PKG-INFO` & `evennia-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evennia
-Version: 1.3.0
+Version: 2.0.0
 Summary: A full-featured toolkit and server for text-based multiplayer games (MUDs, MU*, etc).
 Maintainer-email: Griatch <griatch@gmail.com>
 License: BSD
 Project-URL: Homepage, https://www.evennia.com
 Project-URL: Github, https://github.com/evennia/evennia
 Project-URL: Documentation, https://www.evennia.com/docs/latest/index.html
 Project-URL: Live Demo, https://demo.evennia.com/
```

### Comparing `evennia-1.3.0/README.md` & `evennia-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/__init__.py` & `evennia-2.0.0/evennia/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 ScriptDB = None
 ChannelDB = None
 Msg = None
 
 # Properties
 AttributeProperty = None
 TagProperty = None
+TagCategoryProperty = None
 
 # commands
 Command = None
 CmdSet = None
 default_cmds = None
 syscmdkeys = None
 InterruptCommand = None
@@ -89,14 +90,15 @@
 EvMenu = None
 EvTable = None
 EvForm = None
 EvEditor = None
 EvMore = None
 ANSIString = None
 signals = None
+FuncParser = None
 
 # Handlers
 SESSION_HANDLER = None
 TASK_HANDLER = None
 TICKER_HANDLER = None
 MONITOR_HANDLER = None
 
@@ -132,15 +134,15 @@
     return version
 
 
 __version__ = _create_version()
 del _create_version
 
 
-def _init():
+def _init(portal_mode=False):
     """
     This function is called automatically by the launcher only after
     Evennia has fully initialized all its models. It sets up the API
     in a safe environment where all models are available already.
     """
     global DefaultAccount, DefaultObject, DefaultGuest, DefaultCharacter
     global DefaultRoom, DefaultExit, DefaultChannel, DefaultScript
@@ -152,46 +154,40 @@
     global create_message, create_help_entry
     global signals
     global settings, lockfuncs, logger, utils, gametime, ansi, spawn, managers
     global contrib, TICKER_HANDLER, MONITOR_HANDLER, SESSION_HANDLER
     global TASK_HANDLER
     global GLOBAL_SCRIPTS, OPTION_CLASSES
     global EvMenu, EvTable, EvForm, EvMore, EvEditor
-    global ANSIString
-    global AttributeProperty, TagProperty
+    global ANSIString, FuncParser
+    global AttributeProperty, TagProperty, TagCategoryProperty
 
     # Parent typeclasses
     # utilities
     from django.conf import settings
 
     from . import contrib
     from .accounts.accounts import DefaultAccount, DefaultGuest
     from .accounts.models import AccountDB
     from .commands.cmdset import CmdSet
     from .commands.command import Command, InterruptCommand
     from .comms.comms import DefaultChannel
     from .comms.models import ChannelDB, Msg
     from .locks import lockfuncs
     from .objects.models import ObjectDB
-    from .objects.objects import (
-        DefaultCharacter,
-        DefaultExit,
-        DefaultObject,
-        DefaultRoom,
-    )
+    from .objects.objects import DefaultCharacter, DefaultExit, DefaultObject, DefaultRoom
     from .prototypes.spawner import spawn
     from .scripts.models import ScriptDB
     from .scripts.monitorhandler import MONITOR_HANDLER
     from .scripts.scripts import DefaultScript
     from .scripts.taskhandler import TASK_HANDLER
     from .scripts.tickerhandler import TICKER_HANDLER
     from .server import signals
-    from .server.sessionhandler import SESSION_HANDLER
     from .typeclasses.attributes import AttributeProperty
-    from .typeclasses.tags import TagProperty
+    from .typeclasses.tags import TagCategoryProperty, TagProperty
     from .utils import ansi, gametime, logger
     from .utils.ansi import ANSIString
 
     # containers
     from .utils.containers import GLOBAL_SCRIPTS, OPTION_CLASSES
 
     # create functions
@@ -204,25 +200,42 @@
         create_script,
     )
     from .utils.eveditor import EvEditor
     from .utils.evform import EvForm
     from .utils.evmenu import EvMenu
     from .utils.evmore import EvMore
     from .utils.evtable import EvTable
+    from .utils.funcparser import FuncParser
 
     # search functions
     from .utils.search import (
         search_account,
         search_channel,
         search_help,
         search_message,
         search_object,
         search_script,
         search_tag,
     )
+    from .utils.utils import class_from_module
+
+    if portal_mode:
+        # Set up the PortalSessionHandler
+        from evennia.server.portal import portalsessionhandler
+
+        portal_sess_handler_class = class_from_module(settings.PORTAL_SESSION_HANDLER_CLASS)
+        portalsessionhandler.PORTAL_SESSIONS = portal_sess_handler_class()
+    else:
+        # Create the ServerSesssionHandler
+        from evennia.server import sessionhandler
+
+        sess_handler_class = class_from_module(settings.SERVER_SESSION_HANDLER_CLASS)
+        sessionhandler.SESSIONS = sess_handler_class()
+        sessionhandler.SESSION_HANDLER = sessionhandler.SESSIONS
+        SESSION_HANDLER = sessionhandler.SESSIONS
 
     # API containers
 
     class _EvContainer(object):
         """
         Parent for other containers
```

### Comparing `evennia-1.3.0/evennia/__main__.py` & `evennia-2.0.0/evennia/__main__.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/accounts/accounts.py` & `evennia-2.0.0/evennia/accounts/accounts.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 from django.conf import settings
 from django.contrib.auth import authenticate, password_validation
 from django.core.exceptions import ImproperlyConfigured, ValidationError
 from django.utils import timezone
 from django.utils.module_loading import import_string
 from django.utils.translation import gettext as _
+import evennia
 from evennia.accounts.manager import AccountManager
 from evennia.accounts.models import AccountDB
 from evennia.commands.cmdsethandler import CmdSetHandler
 from evennia.comms.models import ChannelDB
 from evennia.objects.models import ObjectDB
 from evennia.scripts.scripthandler import ScriptHandler
 from evennia.server.models import ServerConfig
@@ -37,16 +38,14 @@
 from evennia.typeclasses.models import TypeclassBase
 from evennia.utils import class_from_module, create, logger
 from evennia.utils.optionhandler import OptionHandler
 from evennia.utils.utils import is_iter, lazy_property, make_iter, to_str, variable_from_module
 
 __all__ = ("DefaultAccount", "DefaultGuest")
 
-_SESSIONS = None
-
 _AT_SEARCH_RESULT = variable_from_module(*settings.SEARCH_AT_RESULT.rsplit(".", 1))
 _MULTISESSION_MODE = settings.MULTISESSION_MODE
 _AUTO_CREATE_CHARACTER_WITH_ACCOUNT = settings.AUTO_CREATE_CHARACTER_WITH_ACCOUNT
 _AUTO_PUPPET_ON_LOGIN = settings.AUTO_PUPPET_ON_LOGIN
 _MAX_NR_SIMULTANEOUS_PUPPETS = settings.MAX_NR_SIMULTANEOUS_PUPPETS
 _MAX_NR_CHARACTERS = settings.MAX_NR_CHARACTERS
 _CMDSET_ACCOUNT = settings.CMDSET_ACCOUNT
@@ -91,21 +90,18 @@
                 session id.
 
         Returns:
             sessions (list): A list of Session objects. If `sessid`
                 is given, this is a list with one (or zero) elements.
 
         """
-        global _SESSIONS
-        if not _SESSIONS:
-            from evennia.server.sessionhandler import SESSIONS as _SESSIONS
         if sessid:
-            return make_iter(_SESSIONS.session_from_account(self.account, sessid))
+            return make_iter(evennia.SESSION_HANDLER.session_from_account(self.account, sessid))
         else:
-            return _SESSIONS.sessions_from_account(self.account)
+            return evennia.SESSION_HANDLER.sessions_from_account(self.account)
 
     def all(self):
         """
         Alias to get(), returning all sessions.
 
         Returns:
             sessions (list): All sessions.
@@ -280,18 +276,15 @@
         sessionhandler)
 
         Args:
             session (Session): Session to disconnect.
             reason (str, optional): Eventual reason for the disconnect.
 
         """
-        global _SESSIONS
-        if not _SESSIONS:
-            from evennia.server.sessionhandler import SESSIONS as _SESSIONS
-        _SESSIONS.disconnect(session, reason)
+        evennia.SESSION_HANDLER.disconnect(session, reason)
 
     # puppeting operations
 
     def puppet_object(self, session, obj):
         """
         Use the given session to control (puppet) the given object (usually
         a Character type).
```

### Comparing `evennia-1.3.0/evennia/accounts/bots.py` & `evennia-2.0.0/evennia/accounts/bots.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,27 @@
 """
 
 import time
 
 from django.conf import settings
 from django.utils.translation import gettext as _
 
+import evennia
 from evennia.accounts.accounts import DefaultAccount
 from evennia.scripts.scripts import DefaultScript
 from evennia.utils import logger, search, utils
 from evennia.utils.ansi import strip_ansi
 
 _IDLE_TIMEOUT = settings.IDLE_TIMEOUT
 
 _IRC_ENABLED = settings.IRC_ENABLED
 _RSS_ENABLED = settings.RSS_ENABLED
 _GRAPEVINE_ENABLED = settings.GRAPEVINE_ENABLED
 _DISCORD_ENABLED = settings.DISCORD_ENABLED and hasattr(settings, "DISCORD_BOT_TOKEN")
 
-_SESSIONS = None
-
 
 class BotStarter(DefaultScript):
     """
     This non-repeating script has the
     sole purpose of kicking its bot
     into gear when it is initialized.
 
@@ -57,18 +56,15 @@
         Called self.interval seconds to keep connection. We cannot use
         the IDLE command from inside the game since the system will
         not catch it (commands executed from the server side usually
         has no sessions). So we update the idle counter manually here
         instead. This keeps the bot getting hit by IDLE_TIMEOUT.
 
         """
-        global _SESSIONS
-        if not _SESSIONS:
-            from evennia.server.sessionhandler import SESSIONS as _SESSIONS
-        for session in _SESSIONS.sessions_from_account(self.account):
+        for session in evennia.SESSION_HANDLER.sessions_from_account(self.account):
             session.update_session_counters(idle=True)
 
 
 #
 # Bot base class
 
 
@@ -166,18 +162,14 @@
         """
         if not _IRC_ENABLED:
             # the bot was created, then IRC was turned off. We delete
             # ourselves (this will also kill the start script)
             self.delete()
             return
 
-        global _SESSIONS
-        if not _SESSIONS:
-            from evennia.server.sessionhandler import SESSIONS as _SESSIONS
-
         # if keywords are given, store (the BotStarter script
         # will not give any keywords, so this should normally only
         # happen at initialization)
         if irc_botname:
             self.db.irc_botname = irc_botname
         elif not self.db.irc_botname:
             self.db.irc_botname = self.key
@@ -204,15 +196,15 @@
             "uid": self.dbid,
             "botname": self.db.irc_botname,
             "channel": self.db.irc_channel,
             "network": self.db.irc_network,
             "port": self.db.irc_port,
             "ssl": self.db.irc_ssl,
         }
-        _SESSIONS.start_bot_session(self.factory_path, configdict)
+        evennia.SESSION_HANDLER.start_bot_session(self.factory_path, configdict)
 
     def at_msg_send(self, **kwargs):
         "Shortcut here or we can end up in infinite loop"
         pass
 
     def get_nicklist(self, caller):
         """
@@ -332,20 +324,17 @@
 
         elif kwargs["type"] == "privmsg":
             # A private message to the bot - a command.
             user = kwargs["user"]
 
             if txt.lower().startswith("who"):
                 # return server WHO list (abbreviated for IRC)
-                global _SESSIONS
-                if not _SESSIONS:
-                    from evennia.server.sessionhandler import SESSIONS as _SESSIONS
                 whos = []
                 t0 = time.time()
-                for sess in _SESSIONS.get_sessions():
+                for sess in evennia.SESSION_HANDLER.get_sessions():
                     delta_cmd = t0 - sess.cmd_last_visible
                     delta_conn = t0 - session.conn_time
                     account = sess.get_account()
                     whos.append(
                         "%s (%s/%s)"
                         % (
                             utils.crop("|w%s|n" % account.name, width=25),
@@ -403,33 +392,29 @@
 
         """
         if not _RSS_ENABLED:
             # The bot was created, then RSS was turned off. Delete ourselves.
             self.delete()
             return
 
-        global _SESSIONS
-        if not _SESSIONS:
-            from evennia.server.sessionhandler import SESSIONS as _SESSIONS
-
         if ev_channel:
             # connect to Evennia channel
             channel = search.channel_search(ev_channel)
             if not channel:
                 raise RuntimeError(f"Evennia Channel '{ev_channel}' not found.")
             channel = channel[0]
             self.db.ev_channel = channel
         if rss_url:
             self.db.rss_url = rss_url
         if rss_rate:
             self.db.rss_rate = rss_rate
         # instruct the server and portal to create a new session with
         # the stored configuration
         configdict = {"uid": self.dbid, "url": self.db.rss_url, "rate": self.db.rss_rate}
-        _SESSIONS.start_bot_session("evennia.server.portal.rss.RSSBotFactory", configdict)
+        evennia.SESSION_HANDLER.start_bot_session("evennia.server.portal.rss.RSSBotFactory", configdict)
 
     def execute_cmd(self, txt=None, session=None, **kwargs):
         """
         Take incoming data and send it to connected channel. This is
         triggered by the bot_data_in Inputfunc.
 
         Args:
@@ -464,18 +449,14 @@
         Start by telling the portal to connect to the grapevine network.
 
         """
         if not _GRAPEVINE_ENABLED:
             self.delete()
             return
 
-        global _SESSIONS
-        if not _SESSIONS:
-            from evennia.server.sessionhandler import SESSIONS as _SESSIONS
-
         # connect to Evennia channel
         if ev_channel:
             # connect to Evennia channel
             channel = search.channel_search(ev_channel)
             if not channel:
                 raise RuntimeError(f"Evennia Channel '{ev_channel}' not found.")
             channel = channel[0]
@@ -484,15 +465,15 @@
 
         if grapevine_channel:
             self.db.grapevine_channel = grapevine_channel
 
         # these will be made available as properties on the protocol factory
         configdict = {"uid": self.dbid, "grapevine_channel": self.db.grapevine_channel}
 
-        _SESSIONS.start_bot_session(self.factory_path, configdict)
+        evennia.SESSION_HANDLER.start_bot_session(self.factory_path, configdict)
 
     def at_msg_send(self, **kwargs):
         "Shortcut here or we can end up in infinite loop"
         pass
 
     def msg(self, text=None, **kwargs):
         """
@@ -615,20 +596,17 @@
                 if not channel:
                     raise RuntimeError(f"Evennia Channel {channel_name} not found.")
                 channel = channel[0]
                 self.ndb.ev_channels[channel_name] = channel
                 channel.connect(self)
 
         # connect
-        global _SESSIONS
-        if not _SESSIONS:
-            from evennia.server.sessionhandler import SESSION_HANDLER as _SESSIONS
         # these will be made available as properties on the protocol factory
         configdict = {"uid": self.dbid}
-        _SESSIONS.start_bot_session(self.factory_path, configdict)
+        evennia.SESSION_HANDLER.start_bot_session(self.factory_path, configdict)
 
     def at_pre_channel_msg(self, message, channel, senders=None, **kwargs):
         """
         Called by the Channel just before passing a message into `channel_msg`.
 
         We overload this to set the channel tag prefix.
```

### Comparing `evennia-1.3.0/evennia/accounts/manager.py` & `evennia-2.0.0/evennia/accounts/manager.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/accounts/migrations/0001_initial.py` & `evennia-2.0.0/evennia/accounts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/accounts/migrations/0003_auto_20150209_2234.py` & `evennia-2.0.0/evennia/accounts/migrations/0003_auto_20150209_2234.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/accounts/migrations/0004_auto_20150403_2339.py` & `evennia-2.0.0/evennia/accounts/migrations/0004_auto_20150403_2339.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/accounts/migrations/0005_auto_20160905_0902.py` & `evennia-2.0.0/evennia/accounts/migrations/0005_auto_20160905_0902.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/accounts/migrations/0006_auto_20170606_1731.py` & `evennia-2.0.0/evennia/accounts/migrations/0006_auto_20170606_1731.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/accounts/migrations/0007_copy_player_to_account.py` & `evennia-2.0.0/evennia/accounts/migrations/0007_copy_player_to_account.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/accounts/migrations/0008_auto_20190128_1820.py` & `evennia-2.0.0/evennia/accounts/migrations/0008_auto_20190128_1820.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/accounts/migrations/0009_auto_20191025_0831.py` & `evennia-2.0.0/evennia/accounts/migrations/0009_auto_20191025_0831.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/accounts/migrations/0011_convert_contrib_typeclass_paths.py` & `evennia-2.0.0/evennia/accounts/migrations/0011_convert_contrib_typeclass_paths.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/accounts/models.py` & `evennia-2.0.0/evennia/accounts/models.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/accounts/tests.py` & `evennia-2.0.0/evennia/accounts/tests.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from random import randint
 from unittest import TestCase
 
 from django.test import override_settings
 from mock import MagicMock, Mock, patch
 
+import evennia
 from evennia.accounts.accounts import (
     AccountSessionHandler,
     DefaultAccount,
     DefaultGuest,
 )
 from evennia.utils import create
 from evennia.utils.test_resources import BaseEvenniaTest
@@ -33,30 +34,28 @@
             self.account.delete()
 
     def test_get(self):
         "Check get method"
         self.assertEqual(self.handler.get(), [])
         self.assertEqual(self.handler.get(100), [])
 
-        import evennia.server.sessionhandler
-
         s1 = MagicMock()
         s1.logged_in = True
         s1.uid = self.account.uid
-        evennia.server.sessionhandler.SESSIONS[s1.uid] = s1
+        evennia.SESSION_HANDLER[s1.uid] = s1
 
         s2 = MagicMock()
         s2.logged_in = True
         s2.uid = self.account.uid + 1
-        evennia.server.sessionhandler.SESSIONS[s2.uid] = s2
+        evennia.SESSION_HANDLER[s2.uid] = s2
 
         s3 = MagicMock()
         s3.logged_in = False
         s3.uid = self.account.uid + 2
-        evennia.server.sessionhandler.SESSIONS[s3.uid] = s3
+        evennia.SESSION_HANDLER[s3.uid] = s3
 
         self.assertEqual([s.uid for s in self.handler.get()], [s1.uid])
         self.assertEqual([s.uid for s in [self.handler.get(self.account.uid)]], [s1.uid])
         self.assertEqual([s.uid for s in self.handler.get(self.account.uid + 1)], [])
 
     def test_all(self):
         "Check all method"
@@ -247,24 +246,22 @@
             self.fail("Expected error: 'Session not found'")
         except RuntimeError as re:
             self.assertEqual("Session not found", str(re))
 
     def test_puppet_object_already_puppeting(self):
         "Check puppet_object method called, already puppeting this"
 
-        import evennia.server.sessionhandler
-
         account = create.create_account(
             f"TestAccount{randint(0, 999999)}",
             email="test@test.com",
             password="testpassword",
             typeclass=DefaultAccount,
         )
         self.s1.uid = account.uid
-        evennia.server.sessionhandler.SESSIONS[self.s1.uid] = self.s1
+        evennia.SESSION_HANDLER[self.s1.uid] = self.s1
 
         self.s1.logged_in = True
         self.s1.data_out = Mock(return_value=None)
 
         obj = Mock()
         self.s1.puppet = obj
         account.puppet_object(self.s1, obj)
@@ -272,24 +269,22 @@
             options=None, text="You are already puppeting this object."
         )
         self.assertIsNone(obj.at_post_puppet.call_args)
 
     def test_puppet_object_no_permission(self):
         "Check puppet_object method called, no permission"
 
-        import evennia.server.sessionhandler
-
         account = create.create_account(
             f"TestAccount{randint(0, 999999)}",
             email="test@test.com",
             password="testpassword",
             typeclass=DefaultAccount,
         )
         self.s1.uid = account.uid
-        evennia.server.sessionhandler.SESSIONS[self.s1.uid] = self.s1
+        evennia.SESSION_HANDLER[self.s1.uid] = self.s1
 
         self.s1.data_out = MagicMock()
         obj = Mock()
         obj.access = Mock(return_value=False)
 
         account.puppet_object(self.s1, obj)
 
@@ -298,24 +293,22 @@
         )
         self.assertIsNone(obj.at_post_puppet.call_args)
 
     @override_settings(MULTISESSION_MODE=0)
     def test_puppet_object_joining_other_session(self):
         "Check puppet_object method called, joining other session"
 
-        import evennia.server.sessionhandler
-
         account = create.create_account(
             f"TestAccount{randint(0, 999999)}",
             email="test@test.com",
             password="testpassword",
             typeclass=DefaultAccount,
         )
         self.s1.uid = account.uid
-        evennia.server.sessionhandler.SESSIONS[self.s1.uid] = self.s1
+        evennia.SESSION_HANDLER[self.s1.uid] = self.s1
 
         self.s1.puppet = None
         self.s1.logged_in = True
         self.s1.data_out = MagicMock()
 
         obj = Mock()
         obj.access = Mock(return_value=True)
@@ -328,25 +321,23 @@
             self.s1.data_out.call_args[1]["text"].endswith("from another of your sessions.|n")
         )
         self.assertTrue(obj.at_post_puppet.call_args[1] == {})
 
     def test_puppet_object_already_puppeted(self):
         "Check puppet_object method called, already puppeted"
 
-        import evennia.server.sessionhandler
-
         account = create.create_account(
             f"TestAccount{randint(0, 999999)}",
             email="test@test.com",
             password="testpassword",
             typeclass=DefaultAccount,
         )
         self.account = account
         self.s1.uid = account.uid
-        evennia.server.sessionhandler.SESSIONS[self.s1.uid] = self.s1
+        evennia.SESSION_HANDLER[self.s1.uid] = self.s1
 
         self.s1.puppet = None
         self.s1.logged_in = True
         self.s1.data_out = Mock(return_value=None)
 
         obj = Mock()
         obj.access = Mock(return_value=True)
@@ -406,28 +397,28 @@
     def test_idle_time(self, mock_time):
         self.session.cmd_last_visible = 10000 - 10
         idle = self.account.idle_time
         self.assertEqual(idle, 10)
 
         # test no sessions
         with patch(
-            "evennia.accounts.accounts._SESSIONS.sessions_from_account", return_value=[]
+            "evennia.SESSION_HANDLER.sessions_from_account", return_value=[]
         ) as mock_sessh:
             idle = self.account.idle_time
             self.assertEqual(idle, None)
 
     @patch("evennia.accounts.accounts.time.time", return_value=10000)
     def test_connection_time(self, mock_time):
         self.session.conn_time = 10000 - 10
         conn = self.account.connection_time
         self.assertEqual(conn, 10)
 
         # test no sessions
         with patch(
-            "evennia.accounts.accounts._SESSIONS.sessions_from_account", return_value=[]
+            "evennia.SESSION_HANDLER.sessions_from_account", return_value=[]
         ) as mock_sessh:
             idle = self.account.connection_time
             self.assertEqual(idle, None)
 
     def test_create_account(self):
         acct = create.account(
             "TestAccount3",
```

### Comparing `evennia-1.3.0/evennia/commands/cmdhandler.py` & `evennia-2.0.0/evennia/commands/cmdhandler.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/commands/cmdparser.py` & `evennia-2.0.0/evennia/commands/cmdparser.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/commands/cmdset.py` & `evennia-2.0.0/evennia/commands/cmdset.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/commands/cmdsethandler.py` & `evennia-2.0.0/evennia/commands/cmdsethandler.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,14 @@
 import sys
 from importlib import import_module
 from inspect import trace
 from traceback import format_exc
 
 from django.conf import settings
 from django.utils.translation import gettext as _
-
 from evennia.commands.cmdset import CmdSet
 from evennia.server.models import ServerConfig
 from evennia.utils import logger, utils
 
 __all__ = ("import_cmdset", "CmdSetHandler")
 
 _CACHED_CMDSETS = {}
@@ -162,15 +161,14 @@
 
     """
     python_paths = [path] + [
         "%s.%s" % (prefix, path) for prefix in _CMDSET_PATHS if not path.startswith(prefix)
     ]
     errstring = ""
     for python_path in python_paths:
-
         if "." in path:
             modpath, classname = python_path.rsplit(".", 1)
         else:
             raise ImportError(f"The path '{path}' is not on the form modulepath.ClassName")
 
         try:
             # first try to get from cache
```

### Comparing `evennia-1.3.0/evennia/commands/command.py` & `evennia-2.0.0/evennia/commands/command.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/commands/default/account.py` & `evennia-2.0.0/evennia/commands/default/account.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 method. Otherwise all text will be returned to all connected sessions.
 
 """
 import time
 from codecs import lookup as codecs_lookup
 
 from django.conf import settings
-from evennia.server.sessionhandler import SESSIONS
+import evennia
 from evennia.utils import create, logger, search, utils
 
 COMMAND_DEFAULT_CLASS = utils.class_from_module(settings.COMMAND_DEFAULT_CLASS)
 
 _MAX_NR_CHARACTERS = settings.MAX_NR_CHARACTERS
 _AUTO_PUPPET_ON_LOGIN = settings.AUTO_PUPPET_ON_LOGIN
 
@@ -491,28 +491,27 @@
     # this is used by the parent
     account_caller = True
 
     def func(self):
         """
         Get all connected accounts by polling session.
         """
-
         account = self.account
-        session_list = SESSIONS.get_sessions()
+        session_list = evennia.SESSION_HANDLER.get_sessions()
 
         session_list = sorted(session_list, key=lambda o: o.account.key)
 
         if self.cmdstring == "doing":
             show_session_data = False
         else:
             show_session_data = account.check_permstring("Developer") or account.check_permstring(
                 "Admins"
             )
 
-        naccounts = SESSIONS.account_count()
+        naccounts = evennia.SESSION_HANDLER.account_count()
         if show_session_data:
             # privileged info
             table = self.styled_table(
                 "|wAccount Name",
                 "|wOn for",
                 "|wIdle",
                 "|wPuppeting",
```

### Comparing `evennia-1.3.0/evennia/commands/default/admin.py` & `evennia-2.0.0/evennia/commands/default/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 
 import re
 import time
 
 from django.conf import settings
 
 from evennia.server.models import ServerConfig
-from evennia.server.sessionhandler import SESSIONS
+
+import evennia
 from evennia.utils import class_from_module, evtable, logger, search
 
 COMMAND_DEFAULT_CLASS = class_from_module(settings.COMMAND_DEFAULT_CLASS)
 
 PERMISSION_HIERARCHY = [p.lower() for p in settings.PERMISSION_HIERARCHY]
 
 # limit members for API inclusion
@@ -64,15 +65,15 @@
         else:
             args, reason = args, ""
 
         boot_list = []
 
         if "sid" in self.switches:
             # Boot a particular session id.
-            sessions = SESSIONS.get_sessions(True)
+            sessions = evennia.SESSION_HANDLER.get_sessions(True)
             for sess in sessions:
                 # Find the session with the matching session id.
                 if sess.sessid == int(args):
                     boot_list.append(sess)
                     break
         else:
             # Boot by account object
@@ -81,15 +82,15 @@
                 caller.msg(f"Account {args} was not found.")
                 return
             pobj = pobj[0]
             if not pobj.access(caller, "boot"):
                 caller.msg(f"You don't have the permission to boot {pobj.key}.")
                 return
             # we have a bootable object with a connected user
-            matches = SESSIONS.sessions_from_account(pobj)
+            matches = evennia.SESSION_HANDLER.sessions_from_account(pobj)
             for match in matches:
                 boot_list.append(match)
 
         if not boot_list:
             caller.msg("No matching sessions found. The Account does not seem to be online.")
             return
 
@@ -560,15 +561,15 @@
     def func(self):
         """Implements command"""
         if not self.args:
             self.caller.msg("Usage: wall <message>")
             return
         message = f'{self.caller.name} shouts "{self.args}"'
         self.msg("Announcing to all connected sessions ...")
-        SESSIONS.announce_all(message)
+        evennia.SESSION_HANDLER.announce_all(message)
 
 
 class CmdForce(COMMAND_DEFAULT_CLASS):
     """
     forces an object to execute a command
 
     Usage:
```

### Comparing `evennia-1.3.0/evennia/commands/default/batchprocess.py` & `evennia-2.0.0/evennia/commands/default/batchprocess.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/commands/default/building.py` & `evennia-2.0.0/evennia/commands/default/building.py`

 * *Files 0% similar despite different names*

```diff
@@ -1424,14 +1424,15 @@
     """
 
     key = "@open"
     locks = "cmd:perm(open) or perm(Builder)"
     help_category = "Building"
 
     new_obj_lockstring = "control:id({id}) or perm(Admin);delete:id({id}) or perm(Admin)"
+
     # a custom member method to chug out exits and do checks
     def create_exit(self, exit_name, location, destination, exit_aliases=None, typeclass=None):
         """
         Helper function to avoid code duplication.
         At this point we know destination is a valid location
 
         """
@@ -2050,15 +2051,14 @@
     key = "@typeclass"
     aliases = ["@type", "@parent", "@swap", "@update", "@typeclasses"]
     switch_options = ("show", "examine", "update", "reset", "force", "list", "prototype")
     locks = "cmd:perm(typeclass) or perm(Builder)"
     help_category = "Building"
 
     def _generic_search(self, query, typeclass_path):
-
         caller = self.caller
         if typeclass_path:
             # make sure we search the right database table
             try:
                 new_typeclass = class_from_module(typeclass_path)
             except ImportError:
                 # this could be a prototype and not a typeclass at all
@@ -3263,15 +3263,14 @@
             "|wdesc|n",
             align="r",
             border="tablecols",
             width=self.width,
         )
 
         for script in scripts:
-
             nextrep = script.time_until_next_repeat()
             if nextrep is None:
                 nextrep = script.db._paused_time
                 nextrep = f"PAUSED {int(nextrep)}s" if nextrep else "--"
             else:
                 nextrep = f"{nextrep}s"
 
@@ -3734,15 +3733,14 @@
         elif obj_to_teleport.move_to(
             destination,
             quiet="quiet" in self.switches,
             emit_to_obj=caller,
             use_destination="intoexit" not in self.switches,
             move_type="teleport",
         ):
-
             if obj_to_teleport == caller:
                 caller.msg(f"Teleported to {destination}.")
             else:
                 caller.msg(f"Teleported {obj_to_teleport} -> {destination}.")
         else:
             caller.msg("Teleportation failed.")
```

### Comparing `evennia-1.3.0/evennia/commands/default/cmdset_account.py` & `evennia-2.0.0/evennia/commands/default/cmdset_account.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/commands/default/cmdset_character.py` & `evennia-2.0.0/evennia/commands/default/cmdset_character.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/commands/default/cmdset_unloggedin.py` & `evennia-2.0.0/evennia/commands/default/cmdset_unloggedin.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/commands/default/comms.py` & `evennia-2.0.0/evennia/commands/default/comms.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/commands/default/general.py` & `evennia-2.0.0/evennia/commands/default/general.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/commands/default/help.py` & `evennia-2.0.0/evennia/commands/default/help.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/commands/default/muxcommand.py` & `evennia-2.0.0/evennia/commands/default/muxcommand.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/commands/default/syscommands.py` & `evennia-2.0.0/evennia/commands/default/syscommands.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/commands/default/system.py` & `evennia-2.0.0/evennia/commands/default/system.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,20 +9,19 @@
 import datetime
 import os
 import sys
 import time
 import traceback
 
 import django
+import evennia
 import twisted
 from django.conf import settings
-
 from evennia.accounts.models import AccountDB
 from evennia.scripts.taskhandler import TaskHandlerTask
-from evennia.server.sessionhandler import SESSIONS
 from evennia.utils import gametime, logger, search, utils
 from evennia.utils.eveditor import EvEditor
 from evennia.utils.evmenu import ask_yes_no
 from evennia.utils.evtable import EvTable
 from evennia.utils.utils import class_from_module, iter_to_str
 
 COMMAND_DEFAULT_CLASS = class_from_module(settings.COMMAND_DEFAULT_CLASS)
@@ -70,16 +69,16 @@
         """
         Reload the system.
         """
         reason = ""
         if self.args:
             reason = "(Reason: %s) " % self.args.rstrip(".")
         if _BROADCAST_SERVER_RESTART_MESSAGES:
-            SESSIONS.announce_all(f" Server restart initiated {reason}...")
-        SESSIONS.portal_restart_server()
+            evennia.SESSION_HANDLER.announce_all(f" Server restart initiated {reason}...")
+        evennia.SESSION_HANDLER.portal_restart_server()
 
 
 class CmdReset(COMMAND_DEFAULT_CLASS):
     """
     reset and reboot the server
 
     Usage:
@@ -104,16 +103,16 @@
     locks = "cmd:perm(reload) or perm(Developer)"
     help_category = "System"
 
     def func(self):
         """
         Reload the system.
         """
-        SESSIONS.announce_all(" Server resetting/restarting ...")
-        SESSIONS.portal_reset_server()
+        evennia.SESSION_HANDLER.announce_all(" Server resetting/restarting ...")
+        evennia.SESSION_HANDLER.portal_reset_server()
 
 
 class CmdShutdown(COMMAND_DEFAULT_CLASS):
 
     """
     stop the server completely
 
@@ -133,16 +132,16 @@
         if not self.caller.sessions.get():
             return
         self.msg("Shutting down server ...")
         announcement = "\nServer is being SHUT DOWN!\n"
         if self.args:
             announcement += "%s\n" % self.args
         logger.log_info(f"Server shutdown by {self.caller.name}.")
-        SESSIONS.announce_all(announcement)
-        SESSIONS.portal_shutdown()
+        evennia.SESSION_HANDLER.announce_all(announcement)
+        evennia.SESSION_HANDLER.portal_shutdown()
 
 
 def _py_load(caller):
     return ""
 
 
 def _py_code(caller, buf):
@@ -175,41 +174,42 @@
         pycode (str): The Python code to run.
         measure_time (bool, optional): Should we measure the time of execution?
         client_raw (bool, optional): Should we turn off all client-specific escaping?
         show_input (bookl, optional): Should we display the input?
 
     """
     # Try to retrieve the session
-    session = caller
     if hasattr(caller, "sessions"):
         sessions = caller.sessions.all()
 
     available_vars = evennia_local_vars(caller)
 
     if show_input:
         for session in sessions:
+            data = {
+                # TODO: 'highlight' is not used yet
+                "text": (f">>> {pycode}", {"type": "py_input"}),
+                "options": {"raw": True, "highlight": True},
+            }
             try:
-                caller.msg(">>> %s" % pycode, session=session, options={"raw": True})
+                caller.msg(session=session, **data)
             except TypeError:
-                caller.msg(">>> %s" % pycode, options={"raw": True})
+                caller.msg(**data)
 
     try:
         # reroute standard output to game client console
         old_stdout = sys.stdout
         old_stderr = sys.stderr
 
         class FakeStd:
             def __init__(self, caller):
                 self.caller = caller
 
             def write(self, string):
-                if string.endswith("\n"):
-                    self.caller.msg(string[:-1])
-                else:
-                    self.caller.msg(string)
+                self.caller.msg(text=(string.rstrip("\n"), {"type": "py_output"}))
 
         fake_std = FakeStd(caller)
         sys.stdout = fake_std
         sys.stderr = fake_std
 
         try:
             pycode_compiled = compile(pycode, "", mode)
@@ -218,15 +218,15 @@
             pycode_compiled = compile(pycode, "", mode)
 
         duration = ""
         if measure_time:
             t0 = time.time()
             ret = eval(pycode_compiled, {}, available_vars)
             t1 = time.time()
-            duration = " (runtime ~ %.4f ms)" % ((t1 - t0) * 1000)
+            duration = f" (runtime ~ {(t1 - t0) * 1000:.4f} ms)"
             caller.msg(duration)
         else:
             ret = eval(pycode_compiled, {}, available_vars)
 
     except Exception:
         errlist = traceback.format_exc().split("\n")
         if len(errlist) > 4:
@@ -242,17 +242,24 @@
     elif isinstance(ret, tuple):
         # we must convert here to allow msg to pass it (a tuple is confused
         # with a outputfunc structure)
         ret = str(ret)
 
     for session in sessions:
         try:
-            caller.msg(ret, session=session, options={"raw": True, "client_raw": client_raw})
+            caller.msg(
+                (ret, {"type": "py_output"}),
+                session=session,
+                options={"raw": True, "client_raw": client_raw, "highlight": True},
+            )
         except TypeError:
-            caller.msg(ret, options={"raw": True, "client_raw": client_raw})
+            caller.msg(
+                (ret, {"type": "py_output"}),
+                options={"raw": True, "client_raw": client_raw, "highlight": True},
+            )
 
 
 def evennia_local_vars(caller):
     """Return Evennia local variables usable in the py command as a dictionary."""
     import evennia
 
     return {
@@ -558,15 +565,15 @@
         switches = self.switches
 
         if switches and switches[0] not in ("list", "start", "stop", "delete"):
             caller.msg("Usage: service/<list|start|stop|delete> [servicename]")
             return
 
         # get all services
-        service_collection = SESSIONS.server.services
+        service_collection = evennia.SESSION_HANDLER.server.services
 
         if not switches or switches[0] == "list":
             # Just display the list of installed services and their
             # status, then exit.
             table = self.styled_table(
                 "|wService|n (use services/start|stop|delete)", "|wstatus", align="l"
             )
@@ -1028,25 +1035,23 @@
             self.msg("There are no active tasks.")
             if self.switches or self.args:
                 self.msg("Likely the task has completed and been removed.")
             return
 
         # handle caller's request to manipulate a task(s)
         if self.switches and self.lhs:
-
             # find if the argument is a task id or function name
             action_request = self.switches[0]
             try:
                 arg_is_id = int(self.lhslist[0])
             except ValueError:
                 arg_is_id = False
 
             # if the argument is a task id, proccess the action on a single task
             if arg_is_id:
-
                 err_arg_msg = "Switch and task ID are required when manipulating a task."
                 task_comp_msg = "Task completed while processing request."
 
                 # handle missing arguments or switches
                 if not self.switches and self.lhs:
                     self.msg(err_arg_msg)
                     return
@@ -1103,15 +1108,14 @@
                 else:
                     self.msg(task_comp_msg)
                     return
 
             # the argument is not a task id, process the action on all task deferring the function
             # specified as an argument
             else:
-
                 name_match_found = False
                 arg_func_name = self.lhslist[0].lower()
 
                 # repack tasks into a new dictionary
                 current_tasks = {}
                 for task_id, task_args in _TASK_HANDLER.tasks.items():
                     current_tasks.update({task_id: task_args})
```

### Comparing `evennia-1.3.0/evennia/commands/default/tests.py` & `evennia-2.0.0/evennia/commands/default/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 """
 import datetime
 from unittest.mock import MagicMock, Mock, patch
 
 from anything import Anything
 from django.conf import settings
 from django.test import override_settings
+import evennia
 from evennia import (
     DefaultCharacter,
     DefaultExit,
     DefaultObject,
     DefaultRoom,
     ObjectDB,
     search_object,
@@ -30,15 +31,14 @@
 from evennia.commands.command import Command, InterruptCommand
 from evennia.commands.default import account, admin, batchprocess, building, comms, general
 from evennia.commands.default import help as help_module
 from evennia.commands.default import syscommands, system, unloggedin
 from evennia.commands.default.cmdset_character import CharacterCmdSet
 from evennia.commands.default.muxcommand import MuxCommand
 from evennia.prototypes import prototypes as protlib
-from evennia.server.sessionhandler import SESSIONS
 from evennia.utils import create, gametime, utils
 from evennia.utils.test_resources import BaseEvenniaCommandTest  # noqa
 from evennia.utils.test_resources import BaseEvenniaTest, EvenniaCommandTest
 from parameterized import parameterized
 from twisted.internet import task
 
 # ------------------------------------------------------------
@@ -2109,15 +2109,15 @@
         gametime.SERVER_START_TIME = 86400
         expected = (
             "## BEGIN INFO 1.1\nName: %s\nUptime: %s\nConnected: %d\nVersion: Evennia %s\n## END"
             " INFO"
             % (
                 settings.SERVERNAME,
                 datetime.datetime.fromtimestamp(gametime.SERVER_START_TIME).ctime(),
-                SESSIONS.account_count(),
+                evennia.SESSION_HANDLER.account_count(),
                 utils.get_evennia_version(),
             )
         )
         self.call(unloggedin.CmdUnconnectedInfo(), "", expected)
         del gametime.SERVER_START_TIME
 
     @override_settings(NEW_ACCOUNT_REGISTRATION_ENABLED=False)
```

### Comparing `evennia-1.3.0/evennia/commands/default/unloggedin.py` & `evennia-2.0.0/evennia/commands/default/unloggedin.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 """
 import datetime
 import re
 from codecs import lookup as codecs_lookup
 
 from django.conf import settings
 
+import evennia
 from evennia.commands.cmdhandler import CMD_LOGINSTART
 from evennia.comms.models import ChannelDB
-from evennia.server.sessionhandler import SESSIONS
 from evennia.utils import class_from_module, create, gametime, logger, utils
 
 COMMAND_DEFAULT_CLASS = utils.class_from_module(settings.COMMAND_DEFAULT_CLASS)
 
 # limit symbol import for API
 __all__ = (
     "CmdUnconnectedConnect",
@@ -458,15 +458,15 @@
     def func(self):
         self.caller.msg(
             "## BEGIN INFO 1.1\nName: %s\nUptime: %s\nConnected: %d\nVersion: Evennia %s\n## END"
             " INFO"
             % (
                 settings.SERVERNAME,
                 datetime.datetime.fromtimestamp(gametime.SERVER_START_TIME).ctime(),
-                SESSIONS.account_count(),
+                evennia.SESSION_HANDLER.account_count(),
                 utils.get_evennia_version(),
             )
         )
 
 
 def _create_account(session, accountname, password, permissions, typeclass=None, email=None):
     """
```

### Comparing `evennia-1.3.0/evennia/commands/tests.py` & `evennia-2.0.0/evennia/commands/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/comms/comms.py` & `evennia-2.0.0/evennia/comms/comms.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/comms/managers.py` & `evennia-2.0.0/evennia/comms/managers.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/comms/migrations/0001_initial.py` & `evennia-2.0.0/evennia/comms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/comms/migrations/0003_auto_20140917_0756.py` & `evennia-2.0.0/evennia/comms/migrations/0003_auto_20140917_0756.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/comms/migrations/0005_auto_20150223_1517.py` & `evennia-2.0.0/evennia/comms/migrations/0005_auto_20150223_1517.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/comms/migrations/0006_channeldb_db_object_subscriptions.py` & `evennia-2.0.0/evennia/comms/migrations/0006_channeldb_db_object_subscriptions.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/comms/migrations/0007_msg_db_tags.py` & `evennia-2.0.0/evennia/comms/migrations/0007_msg_db_tags.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/comms/migrations/0009_auto_20160921_1731.py` & `evennia-2.0.0/evennia/comms/migrations/0009_auto_20160921_1731.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/comms/migrations/0010_auto_20161206_1912.py` & `evennia-2.0.0/evennia/comms/migrations/0010_auto_20161206_1912.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/comms/migrations/0011_auto_20170217_2039.py` & `evennia-2.0.0/evennia/comms/migrations/0011_auto_20170217_2039.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/comms/migrations/0011_auto_20170606_1731.py` & `evennia-2.0.0/evennia/comms/migrations/0011_auto_20170606_1731.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/comms/migrations/0013_auto_20170705_1726.py` & `evennia-2.0.0/evennia/comms/migrations/0013_auto_20170705_1726.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/comms/migrations/0014_auto_20170705_1736.py` & `evennia-2.0.0/evennia/comms/migrations/0014_auto_20170705_1736.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/comms/migrations/0015_auto_20170706_2041.py` & `evennia-2.0.0/evennia/comms/migrations/0015_auto_20170706_2041.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/comms/migrations/0017_auto_20190128_1820.py` & `evennia-2.0.0/evennia/comms/migrations/0017_auto_20190128_1820.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/comms/migrations/0018_auto_20191025_0831.py` & `evennia-2.0.0/evennia/comms/migrations/0018_auto_20191025_0831.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/comms/migrations/0019_auto_20210514_2032.py` & `evennia-2.0.0/evennia/comms/migrations/0019_auto_20210514_2032.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/comms/migrations/0020_auto_20210514_2210.py` & `evennia-2.0.0/evennia/comms/migrations/0020_auto_20210514_2210.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/comms/migrations/0021_auto_20210520_2137.py` & `evennia-2.0.0/evennia/comms/migrations/0021_auto_20210520_2137.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/comms/migrations/0022_defaultchannel_alter_channeldb_id_alter_msg_id_and_more.py` & `evennia-2.0.0/evennia/comms/migrations/0022_defaultchannel_alter_channeldb_id_alter_msg_id_and_more.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/comms/models.py` & `evennia-2.0.0/evennia/comms/models.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/comms/tests.py` & `evennia-2.0.0/evennia/comms/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/README.md` & `evennia-2.0.0/evennia/contrib/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/base_systems/awsstorage/README.md` & `evennia-2.0.0/evennia/contrib/base_systems/awsstorage/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/base_systems/awsstorage/aws_s3_cdn.py` & `evennia-2.0.0/evennia/contrib/base_systems/awsstorage/aws_s3_cdn.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/base_systems/awsstorage/tests.py` & `evennia-2.0.0/evennia/contrib/base_systems/awsstorage/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/base_systems/building_menu/README.md` & `evennia-2.0.0/evennia/contrib/base_systems/building_menu/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/base_systems/building_menu/building_menu.py` & `evennia-2.0.0/evennia/contrib/base_systems/building_menu/building_menu.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/base_systems/building_menu/tests.py` & `evennia-2.0.0/evennia/contrib/base_systems/building_menu/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/base_systems/color_markups/README.md` & `evennia-2.0.0/evennia/contrib/base_systems/color_markups/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/base_systems/color_markups/color_markups.py` & `evennia-2.0.0/evennia/contrib/base_systems/color_markups/color_markups.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/base_systems/color_markups/tests.py` & `evennia-2.0.0/evennia/contrib/base_systems/color_markups/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/base_systems/components/README.md` & `evennia-2.0.0/evennia/contrib/base_systems/components/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/base_systems/components/__init__.py` & `evennia-2.0.0/evennia/contrib/base_systems/components/__init__.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/base_systems/components/component.py` & `evennia-2.0.0/evennia/contrib/base_systems/components/component.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/base_systems/components/dbfield.py` & `evennia-2.0.0/evennia/contrib/base_systems/components/dbfield.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/base_systems/components/holder.py` & `evennia-2.0.0/evennia/contrib/base_systems/components/holder.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/base_systems/components/signals.py` & `evennia-2.0.0/evennia/contrib/base_systems/components/signals.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/base_systems/components/tests.py` & `evennia-2.0.0/evennia/contrib/base_systems/components/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/base_systems/custom_gametime/README.md` & `evennia-2.0.0/evennia/contrib/base_systems/custom_gametime/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/base_systems/custom_gametime/custom_gametime.py` & `evennia-2.0.0/evennia/contrib/base_systems/custom_gametime/custom_gametime.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/base_systems/custom_gametime/tests.py` & `evennia-2.0.0/evennia/contrib/base_systems/custom_gametime/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/base_systems/email_login/README.md` & `evennia-2.0.0/evennia/contrib/base_systems/email_login/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/base_systems/email_login/connection_screens.py` & `evennia-2.0.0/evennia/contrib/base_systems/email_login/connection_screens.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/base_systems/email_login/email_login.py` & `evennia-2.0.0/evennia/contrib/base_systems/email_login/email_login.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/base_systems/email_login/tests.py` & `evennia-2.0.0/evennia/contrib/base_systems/email_login/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/base_systems/godotwebsocket/README.md` & `evennia-2.0.0/evennia/contrib/base_systems/godotwebsocket/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/base_systems/godotwebsocket/__init__.py` & `evennia-2.0.0/evennia/contrib/base_systems/godotwebsocket/__init__.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/base_systems/godotwebsocket/test_text2bbcode.py` & `evennia-2.0.0/evennia/contrib/base_systems/godotwebsocket/test_text2bbcode.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/base_systems/godotwebsocket/text2bbcode.py` & `evennia-2.0.0/evennia/contrib/base_systems/godotwebsocket/text2bbcode.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/base_systems/godotwebsocket/webclient.py` & `evennia-2.0.0/evennia/contrib/base_systems/godotwebsocket/webclient.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 from autobahn.twisted import WebSocketServerFactory
 from twisted.application import internet
 
 from evennia import settings
 from evennia.contrib.base_systems.godotwebsocket.text2bbcode import parse_to_bbcode
 from evennia.server.portal import webclient
-from evennia.server.portal.portalsessionhandler import PORTAL_SESSIONS
 from evennia.settings_default import LOCKDOWN_MODE
 
 
 class GodotWebSocketClient(webclient.WebSocketClient):
     """
     Implements the server-side of the Websocket connection specific to Godot.
     It inherits from the basic Websocket implementation and changes only what is necessary.
@@ -66,14 +65,15 @@
     class GodotWebsocket(WebSocketServerFactory):
         "Only here for better naming in logs"
         pass
 
     factory = GodotWebsocket()
     factory.noisy = False
     factory.protocol = GodotWebSocketClient
+    from evennia.server.portal.portalsessionhandler import PORTAL_SESSIONS
     factory.sessionhandler = PORTAL_SESSIONS
 
     interface = "127.0.0.1" if LOCKDOWN_MODE else settings.GODOT_CLIENT_WEBSOCKET_CLIENT_INTERFACE
 
     port = settings.GODOT_CLIENT_WEBSOCKET_PORT
     websocket_service = internet.TCPServer(port, factory, interface=interface)
     websocket_service.setName("GodotWebSocket%s:%s" % (interface, port))
```

### Comparing `evennia-1.3.0/evennia/contrib/base_systems/ingame_python/README.md` & `evennia-2.0.0/evennia/contrib/base_systems/ingame_python/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/base_systems/ingame_python/callbackhandler.py` & `evennia-2.0.0/evennia/contrib/base_systems/ingame_python/callbackhandler.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/base_systems/ingame_python/commands.py` & `evennia-2.0.0/evennia/contrib/base_systems/ingame_python/commands.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/base_systems/ingame_python/eventfuncs.py` & `evennia-2.0.0/evennia/contrib/base_systems/ingame_python/eventfuncs.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/base_systems/ingame_python/scripts.py` & `evennia-2.0.0/evennia/contrib/base_systems/ingame_python/scripts.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/base_systems/ingame_python/tests.py` & `evennia-2.0.0/evennia/contrib/base_systems/ingame_python/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/base_systems/ingame_python/typeclasses.py` & `evennia-2.0.0/evennia/contrib/base_systems/ingame_python/typeclasses.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/base_systems/ingame_python/utils.py` & `evennia-2.0.0/evennia/contrib/base_systems/ingame_python/utils.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/base_systems/menu_login/README.md` & `evennia-2.0.0/evennia/contrib/base_systems/menu_login/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/base_systems/menu_login/connection_screens.py` & `evennia-2.0.0/evennia/contrib/base_systems/menu_login/connection_screens.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/base_systems/menu_login/menu_login.py` & `evennia-2.0.0/evennia/contrib/base_systems/menu_login/menu_login.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/base_systems/mux_comms_cmds/README.md` & `evennia-2.0.0/evennia/contrib/base_systems/mux_comms_cmds/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/base_systems/mux_comms_cmds/mux_comms_cmds.py` & `evennia-2.0.0/evennia/contrib/base_systems/mux_comms_cmds/mux_comms_cmds.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/base_systems/mux_comms_cmds/tests.py` & `evennia-2.0.0/evennia/contrib/base_systems/mux_comms_cmds/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/base_systems/unixcommand/README.md` & `evennia-2.0.0/evennia/contrib/base_systems/unixcommand/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/base_systems/unixcommand/tests.py` & `evennia-2.0.0/evennia/contrib/base_systems/unixcommand/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/base_systems/unixcommand/unixcommand.py` & `evennia-2.0.0/evennia/contrib/base_systems/unixcommand/unixcommand.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/README.md` & `evennia-2.0.0/evennia/contrib/full_systems/evscaperoom/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/commands.py` & `evennia-2.0.0/evennia/contrib/full_systems/evscaperoom/commands.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/menu.py` & `evennia-2.0.0/evennia/contrib/full_systems/evscaperoom/menu.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/objects.py` & `evennia-2.0.0/evennia/contrib/full_systems/evscaperoom/objects.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/room.py` & `evennia-2.0.0/evennia/contrib/full_systems/evscaperoom/room.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/scripts.py` & `evennia-2.0.0/evennia/contrib/full_systems/evscaperoom/scripts.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/state.py` & `evennia-2.0.0/evennia/contrib/full_systems/evscaperoom/state.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/states/README.md` & `evennia-2.0.0/evennia/contrib/full_systems/evscaperoom/states/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/states/state_001_start.py` & `evennia-2.0.0/evennia/contrib/full_systems/evscaperoom/states/state_001_start.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/tests.py` & `evennia-2.0.0/evennia/contrib/full_systems/evscaperoom/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/utils.py` & `evennia-2.0.0/evennia/contrib/full_systems/evscaperoom/utils.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/game_systems/barter/README.md` & `evennia-2.0.0/evennia/contrib/game_systems/barter/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/game_systems/barter/barter.py` & `evennia-2.0.0/evennia/contrib/game_systems/barter/barter.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/game_systems/barter/tests.py` & `evennia-2.0.0/evennia/contrib/game_systems/barter/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/game_systems/clothing/README.md` & `evennia-2.0.0/evennia/contrib/game_systems/clothing/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/game_systems/clothing/clothing.py` & `evennia-2.0.0/evennia/contrib/game_systems/clothing/clothing.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/game_systems/clothing/tests.py` & `evennia-2.0.0/evennia/contrib/game_systems/clothing/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/game_systems/cooldowns/README.md` & `evennia-2.0.0/evennia/contrib/game_systems/cooldowns/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/game_systems/cooldowns/cooldowns.py` & `evennia-2.0.0/evennia/contrib/game_systems/cooldowns/cooldowns.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/game_systems/cooldowns/tests.py` & `evennia-2.0.0/evennia/contrib/game_systems/cooldowns/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/game_systems/crafting/README.md` & `evennia-2.0.0/evennia/contrib/game_systems/crafting/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/game_systems/crafting/crafting.py` & `evennia-2.0.0/evennia/contrib/game_systems/crafting/crafting.py`

 * *Files 1% similar despite different names*

```diff
@@ -600,31 +600,31 @@
             assert len(self.tool_names) == len(self.tool_tags), (
                 f"Crafting {self.__class__}.tool_names list must "
                 "have the same length as .tool_tags."
             )
         else:
             self.tool_names = self.tool_tags
 
+        assert isinstance(
+            self.output_prototypes, (list, tuple)
+        ), "Crafting {self.__class__}.output_prototypes must be a list or tuple."
+
         if self.output_names:
-            assert len(self.consumable_names) == len(self.consumable_tags), (
+            assert len(self.output_names) == len(self.output_prototypes), (
                 f"Crafting {self.__class__}.output_names list must "
                 "have the same length as .output_prototypes."
             )
         else:
             self.output_names = [
                 prot.get("key", prot.get("typeclass", "unnamed"))
                 if isinstance(prot, dict)
                 else str(prot)
                 for prot in self.output_prototypes
             ]
 
-        assert isinstance(
-            self.output_prototypes, (list, tuple)
-        ), "Crafting {self.__class__}.output_prototypes must be a list or tuple."
-
         # don't allow reuse if we have consumables. If only tools we can reuse
         # over and over since nothing changes.
         self.allow_reuse = not bool(self.consumable_tags)
 
     def _format_message(self, message, **kwargs):
 
         missing = iter_to_str(kwargs.get("missing", ""))
```

### Comparing `evennia-1.3.0/evennia/contrib/game_systems/crafting/example_recipes.py` & `evennia-2.0.0/evennia/contrib/game_systems/crafting/example_recipes.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/game_systems/crafting/tests.py` & `evennia-2.0.0/evennia/contrib/game_systems/crafting/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/game_systems/gendersub/README.md` & `evennia-2.0.0/evennia/contrib/game_systems/gendersub/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/game_systems/gendersub/gendersub.py` & `evennia-2.0.0/evennia/contrib/game_systems/gendersub/gendersub.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/game_systems/gendersub/tests.py` & `evennia-2.0.0/evennia/contrib/game_systems/gendersub/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/game_systems/mail/README.md` & `evennia-2.0.0/evennia/contrib/game_systems/mail/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/game_systems/mail/mail.py` & `evennia-2.0.0/evennia/contrib/game_systems/mail/mail.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/game_systems/mail/tests.py` & `evennia-2.0.0/evennia/contrib/game_systems/mail/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/game_systems/multidescer/README.md` & `evennia-2.0.0/evennia/contrib/game_systems/multidescer/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/game_systems/multidescer/multidescer.py` & `evennia-2.0.0/evennia/contrib/game_systems/multidescer/multidescer.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/game_systems/multidescer/tests.py` & `evennia-2.0.0/evennia/contrib/game_systems/multidescer/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/game_systems/puzzles/README.md` & `evennia-2.0.0/evennia/contrib/game_systems/puzzles/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/game_systems/puzzles/puzzles.py` & `evennia-2.0.0/evennia/contrib/game_systems/puzzles/puzzles.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/game_systems/puzzles/tests.py` & `evennia-2.0.0/evennia/contrib/game_systems/puzzles/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/game_systems/turnbattle/README.md` & `evennia-2.0.0/evennia/contrib/game_systems/turnbattle/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/game_systems/turnbattle/tb_basic.py` & `evennia-2.0.0/evennia/contrib/game_systems/turnbattle/tb_basic.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/game_systems/turnbattle/tb_equip.py` & `evennia-2.0.0/evennia/contrib/game_systems/turnbattle/tb_equip.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/game_systems/turnbattle/tb_items.py` & `evennia-2.0.0/evennia/contrib/game_systems/turnbattle/tb_items.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/game_systems/turnbattle/tb_magic.py` & `evennia-2.0.0/evennia/contrib/game_systems/turnbattle/tb_magic.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/game_systems/turnbattle/tb_range.py` & `evennia-2.0.0/evennia/contrib/game_systems/turnbattle/tb_range.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/game_systems/turnbattle/tests.py` & `evennia-2.0.0/evennia/contrib/game_systems/turnbattle/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/grid/extended_room/extended_room.py` & `evennia-2.0.0/evennia/server/profiling/dummyrunner.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,594 +1,639 @@
 """
-Extended Room
+Dummy client runner
 
-Evennia Contribution - Griatch 2012, vincent-lg 2019
+This module implements a stand-alone launcher for stress-testing
+an Evennia game. It will launch any number of fake clients. These
+clients will log into the server and start doing random operations.
+Customizing and weighing these operations differently depends on
+which type of game is tested. The module contains a testing module
+for plain Evennia.
+
+Please note that you shouldn't run this on a production server!
+Launch the program without any arguments or options to see a
+full step-by-step setup help.
+
+Basically (for testing default Evennia):
+
+ - Use an empty/testing database.
+ - set PERMISSION_ACCOUNT_DEFAULT = "Builder"
+ - start server, eventually with profiling active
+ - launch this client runner
+
+If you want to customize the runner's client actions
+(because you changed the cmdset or needs to better
+match your use cases or add more actions), you can
+change which actions by adding a path to
 
-This is an extended Room typeclass for Evennia. It is supported
-by an extended `Look` command and an extended `desc` command, also
-in this module.
+   DUMMYRUNNER_ACTIONS_MODULE = <path.to.your.module>
 
+in your settings. See utils.dummyrunner_actions.py
+for instructions on how to define this module.
 
-Features:
+"""
 
-1) Time-changing description slots
 
-This allows to change the full description text the room shows
-depending on larger time variations. Four seasons (spring, summer,
-autumn and winter) are used by default. The season is calculated
-on-demand (no Script or timer needed) and updates the full text block.
+import random
+import sys
+import time
+from argparse import ArgumentParser
+
+import django
+from twisted.conch import telnet
+from twisted.internet import protocol, reactor
+from twisted.internet.task import LoopingCall
+
+django.setup()
+import evennia  # noqa
+
+evennia._init()
+
+from django.conf import settings  # noqa
+
+from evennia.commands.cmdset import CmdSet  # noqa
+from evennia.commands.command import Command  # noqa
+from evennia.utils import mod_import, time_format  # noqa
+from evennia.utils.ansi import strip_ansi  # noqa
+
+# Load the dummyrunner settings module
+
+DUMMYRUNNER_SETTINGS = mod_import(settings.DUMMYRUNNER_SETTINGS_MODULE)
+if not DUMMYRUNNER_SETTINGS:
+    raise IOError(
+        "Error: Dummyrunner could not find settings file at %s"
+        % settings.DUMMYRUNNER_SETTINGS_MODULE
+    )
+IDMAPPER_CACHE_MAXSIZE = settings.IDMAPPER_CACHE_MAXSIZE
+
+DATESTRING = "%Y%m%d%H%M%S"
+CLIENTS = []
+
+# Settings
+
+# number of clients to launch if no input is given on command line
+NCLIENTS = 1
+# time between each 'tick', in seconds, if not set on command
+# line. All launched clients will be called upon to possibly do an
+# action with this frequency.
+TIMESTEP = DUMMYRUNNER_SETTINGS.TIMESTEP
+# chance of a client performing an action, per timestep. This helps to
+# spread out usage randomly, like it would be in reality.
+CHANCE_OF_ACTION = DUMMYRUNNER_SETTINGS.CHANCE_OF_ACTION
+# spread out the login action separately, having many accounts create accounts
+# and connect simultaneously is generally unlikely.
+CHANCE_OF_LOGIN = DUMMYRUNNER_SETTINGS.CHANCE_OF_LOGIN
+# Port to use, if not specified on command line
+TELNET_PORT = DUMMYRUNNER_SETTINGS.TELNET_PORT or settings.TELNET_PORTS[0]
+#
+NCONNECTED = 0  # client has received a connection
+NLOGIN_SCREEN = 0  # client has seen the login screen (server responded)
+NLOGGING_IN = 0  # client starting login procedure
+NLOGGED_IN = 0  # client has authenticated and logged in
+
+# time when all clients have logged_in
+TIME_ALL_LOGIN = 0
+# actions since all logged in
+TOTAL_ACTIONS = 0
+TOTAL_LAG_MEASURES = 0
+# lag per 30s for all logged in
+TOTAL_LAG = 0
+TOTAL_LAG_IN = 0
+TOTAL_LAG_OUT = 0
+
+
+INFO_STARTING = """
+    Dummyrunner starting using {nclients} dummy account(s). If you don't see
+    any connection messages, make sure that the Evennia server is
+    running.
+
+    TELNET_PORT = {port}
+    IDMAPPER_CACHE_MAXSIZE = {idmapper_cache_size} MB
+    TIMESTEP = {timestep} (rate {rate}/s)
+    CHANCE_OF_LOGIN = {chance_of_login}% per time step
+    CHANCE_OF_ACTION = {chance_of_action}% per time step
+    -> avg rate (per client, after login): {avg_rate} cmds/s
+    -> total avg rate (after login): {avg_rate_total} cmds/s
+
+    Use Ctrl-C (or Cmd-C) to stop/disconnect all clients.
+
+    """
+
+ERROR_NO_MIXIN = """
+    Error: Evennia is not set up for dummyrunner. Before starting the
+    server, make sure to include the following at *the end* of your
+    settings file (remove when not using dummyrunner!):
+
+        from evennia.server.profiling.settings_mixin import *
+
+    This will change the settings in the following way:
+        - change PERMISSION_ACCOUNT_DEFAULT to 'Developer' to allow clients
+          to test all commands
+        - change PASSWORD_HASHERS to use a faster (but less safe) algorithm
+          when creating large numbers of accounts at the same time
+        - set LOGIN_THROTTLE/CREATION_THROTTLE=None to disable it
+
+    If you don't want to use the custom settings of the mixin for some
+    reason, you can change their values manually after the import, or
+    add DUMMYRUNNER_MIXIN=True to your settings file to avoid this
+    error completely.
+
+    Warning: Don't run dummyrunner on a production database! It will
+    create a lot of spammy objects and accounts!
+    """
+
+
+ERROR_FEW_ACTIONS = """
+    Dummyrunner settings error: The ACTIONS tuple is too short: it must
+    contain at least login- and logout functions.
+    """
+
+
+HELPTEXT = """
+DO NOT RUN THIS ON A PRODUCTION SERVER! USE A CLEAN/TESTING DATABASE!
+
+This stand-alone program launches dummy telnet clients against a
+running Evennia server. The idea is to mimic real accounts logging in
+and repeatedly doing resource-heavy commands so as to stress test the
+game. It uses the default command set to log in and issue commands, so
+if that was customized, some of the functionality will not be tested
+(it will not fail, the commands will just not be recognized).  The
+running clients will create new objects and rooms all over the place
+as part of their running, so using a clean/testing database is
+strongly recommended.
+
+Setup:
+  1) setup a fresh/clean database (if using sqlite, just safe-copy
+     away your real evennia.db3 file and create a new one with
+     `evennia migrate`)
+  2) in server/conf/settings.py, add
+
+        PERMISSION_ACCOUNT_DEFAULT="Builder"
+
+     This is so that the dummy accounts can test building operations.
+     You can also customize the dummyrunner by modifying a setting
+     file specified by DUMMYRUNNER_SETTINGS_MODULE
+
+  3) Start Evennia like normal, optionally with profiling (--profile)
+  4) Run this dummy runner via the evennia launcher:
+
+        evennia --dummyrunner <nr_of_clients>
+
+  5) Log on and determine if game remains responsive despite the
+     heavier load. Note that if you activated profiling, there is a
+     considerate additional overhead from the profiler too so you
+     should usually not consider game responsivity when using the
+     profiler at the same time.
+  6) If you use profiling, let the game run long enough to gather
+     data, then stop the server cleanly using evennia stop or @shutdown.
+     @shutdown. The profile appears as
+     server/logs/server.prof/portal.prof (see Python's manual on
+     cProfiler).
+
+Notes:
+
+The dummyrunner tends to create a lot of accounts all at once, which is
+a very heavy operation. This is not a realistic use-case - what you want
+to test is performance during run. A large
+number of clients here may lock up the client until all have been
+created. It may be better to connect multiple dummyrunners instead of
+starting one single one with a lot of accounts. Exactly what this number
+is depends on your computer power. So start with 10-20 clients and increase
+until you see the initial login slows things too much.
 
-There is also a general description which is used as fallback if
-one or more of the seasonal descriptions are not set when their
-time comes.
+"""
 
-An updated `desc` command allows for setting seasonal descriptions.
 
-The room uses the `evennia.utils.gametime.GameTime` global script. This is
-started by default, but if you have deactivated it, you need to
-supply your own time keeping mechanism.
+class CmdDummyRunnerEchoResponse(Command):
+    """
+    Dummyrunner command measuring the round-about response time
+    from sending to receiving a result.
 
+    Usage:
+        dummyrunner_echo_response <timestamp>
 
-2) In-description changing tags
+    Responds with
+        dummyrunner_echo_response:<timestamp>,<current_time>
 
-Within each seasonal (or general) description text, you can also embed
-time-of-day dependent sections. Text inside such a tag will only show
-during that particular time of day. The tags looks like `<timeslot> ...
-</timeslot>`. By default there are four timeslots per day - morning,
-afternoon, evening and night.
+    The dummyrunner will send this and then compare the send time
+    with the receive time on both ends.
 
+    """
 
-3) Details
+    key = "dummyrunner_echo_response"
 
-The Extended Room can be "detailed" with special keywords. This makes
-use of a special `Look` command. Details are "virtual" targets to look
-at, without there having to be a database object created for it. The
-Details are simply stored in a dictionary on the room and if the look
-command cannot find an object match for a `look <target>` command it
-will also look through the available details at the current location
-if applicable. The `detail` command is used to change details.
+    def func(self):
+        # returns (dummy_client_timestamp,current_time)
+        self.msg(f"dummyrunner_echo_response:{self.args},{time.time()}")
+        if self.caller.account.is_superuser:
+            print(f"cmddummyrunner lag in: {time.time() - float(self.args)}s")
 
 
-4) Extra commands
+class DummyRunnerCmdSet(CmdSet):
+    """
+    Dummyrunner injected cmdset.
 
-  CmdExtendedRoomLook - look command supporting room details
-  CmdExtendedRoomDesc - desc command allowing to add seasonal descs,
-  CmdExtendedRoomDetail - command allowing to manipulate details in this room
-                    as well as listing them
-  CmdExtendedRoomGameTime - A simple `time` command, displaying the current
-                    time and season.
+    """
 
+    def at_cmdset_creation(self):
+        self.add(CmdDummyRunnerEchoResponse())
 
-Installation/testing:
 
-Adding the `ExtendedRoomCmdset` to the default character cmdset will add all
-new commands for use.
+# ------------------------------------------------------------
+# Helper functions
+# ------------------------------------------------------------
 
-In more detail, in mygame/commands/default_cmdsets.py:
 
-```
-...
-from evennia.contrib import extended_room   # <---
+ICOUNT = 0
 
-class CharacterCmdset(default_cmds.Character_CmdSet):
-    ...
-    def at_cmdset_creation(self):
-        ...
-        self.add(extended_room.ExtendedRoomCmdSet)  # <---
 
-```
+def idcounter():
+    """
+    Makes unique ids.
 
-Then reload to make the bew commands available. Note that they only work
-on rooms with the typeclass `ExtendedRoom`. Create new rooms with the right
-typeclass or use the `typeclass` command to swap existing rooms.
+    Returns:
+        str: A globally unique id.
 
-"""
+    """
+    global ICOUNT
+    ICOUNT += 1
+    return str("{:03d}".format(ICOUNT))
 
 
-import datetime
-import re
+GCOUNT = 0
 
-from django.conf import settings
 
-from evennia import CmdSet, DefaultRoom, default_cmds, gametime, utils
+def gidcounter():
+    """
+    Makes globally unique ids.
 
-# error return function, needed by Extended Look command
-_AT_SEARCH_RESULT = utils.variable_from_module(*settings.SEARCH_AT_RESULT.rsplit(".", 1))
-
-# regexes for in-desc replacements
-RE_MORNING = re.compile(r"<morning>(.*?)</morning>", re.IGNORECASE)
-RE_AFTERNOON = re.compile(r"<afternoon>(.*?)</afternoon>", re.IGNORECASE)
-RE_EVENING = re.compile(r"<evening>(.*?)</evening>", re.IGNORECASE)
-RE_NIGHT = re.compile(r"<night>(.*?)</night>", re.IGNORECASE)
-# this map is just a faster way to select the right regexes (the first
-# regex in each tuple will be parsed, the following will always be weeded out)
-REGEXMAP = {
-    "morning": (RE_MORNING, RE_AFTERNOON, RE_EVENING, RE_NIGHT),
-    "afternoon": (RE_AFTERNOON, RE_MORNING, RE_EVENING, RE_NIGHT),
-    "evening": (RE_EVENING, RE_MORNING, RE_AFTERNOON, RE_NIGHT),
-    "night": (RE_NIGHT, RE_MORNING, RE_AFTERNOON, RE_EVENING),
-}
-
-# set up the seasons and time slots. This assumes gametime started at the
-# beginning of the year (so month 1 is equivalent to January), and that
-# one CAN divide the game's year into four seasons in the first place ...
-MONTHS_PER_YEAR = 12
-SEASONAL_BOUNDARIES = (3 / 12.0, 6 / 12.0, 9 / 12.0)
-HOURS_PER_DAY = 24
-DAY_BOUNDARIES = (0, 6 / 24.0, 12 / 24.0, 18 / 24.0)
-
-
-# implements the Extended Room
-
-
-class ExtendedRoom(DefaultRoom):
-    """
-    This room implements a more advanced `look` functionality depending on
-    time. It also allows for "details", together with a slightly modified
-    look command.
-    """
-
-    def at_object_creation(self):
-        """Called when room is first created only."""
-        self.db.spring_desc = ""
-        self.db.summer_desc = ""
-        self.db.autumn_desc = ""
-        self.db.winter_desc = ""
-        # the general desc is used as a fallback if a seasonal one is not set
-        self.db.general_desc = ""
-        # will be set dynamically. Can contain raw timeslot codes
-        self.db.raw_desc = ""
-        # this will be set dynamically at first look. Parsed for timeslot codes
-        self.db.desc = ""
-        # these will be filled later
-        self.ndb.last_season = None
-        self.ndb.last_timeslot = None
-        # detail storage
-        self.db.details = {}
-
-    def get_time_and_season(self):
-        """
-        Calculate the current time and season ids.
-        """
-        # get the current time as parts of year and parts of day.
-        # we assume a standard calendar here and use 24h format.
-        timestamp = gametime.gametime(absolute=True)
-        # note that fromtimestamp includes the effects of server time zone!
-        datestamp = datetime.datetime.fromtimestamp(timestamp)
-        season = float(datestamp.month) / MONTHS_PER_YEAR
-        timeslot = float(datestamp.hour) / HOURS_PER_DAY
-
-        # figure out which slots these represent
-        if SEASONAL_BOUNDARIES[0] <= season < SEASONAL_BOUNDARIES[1]:
-            curr_season = "spring"
-        elif SEASONAL_BOUNDARIES[1] <= season < SEASONAL_BOUNDARIES[2]:
-            curr_season = "summer"
-        elif SEASONAL_BOUNDARIES[2] <= season < 1.0 + SEASONAL_BOUNDARIES[0]:
-            curr_season = "autumn"
-        else:
-            curr_season = "winter"
-
-        if DAY_BOUNDARIES[0] <= timeslot < DAY_BOUNDARIES[1]:
-            curr_timeslot = "night"
-        elif DAY_BOUNDARIES[1] <= timeslot < DAY_BOUNDARIES[2]:
-            curr_timeslot = "morning"
-        elif DAY_BOUNDARIES[2] <= timeslot < DAY_BOUNDARIES[3]:
-            curr_timeslot = "afternoon"
-        else:
-            curr_timeslot = "evening"
+    Returns:
+        count (int); A globally unique counter.
 
-        return curr_season, curr_timeslot
+    """
+    global GCOUNT
+    GCOUNT += 1
+    return "%s_%s" % (time.strftime(DATESTRING), GCOUNT)
 
-    def replace_timeslots(self, raw_desc, curr_time):
-        """
-        Filter so that only time markers `<timeslot>...</timeslot>` of
-        the correct timeslot remains in the description.
 
-        Args:
-            raw_desc (str): The unmodified description.
-            curr_time (str): A timeslot identifier.
+def makeiter(obj):
+    """
+    Makes everything iterable.
 
-        Returns:
-            description (str): A possibly moified description.
+    Args:
+        obj (any): Object to turn iterable.
 
-        """
-        if raw_desc:
-            regextuple = REGEXMAP[curr_time]
-            raw_desc = regextuple[0].sub(r"\1", raw_desc)
-            raw_desc = regextuple[1].sub("", raw_desc)
-            raw_desc = regextuple[2].sub("", raw_desc)
-            return regextuple[3].sub("", raw_desc)
-        return raw_desc
+    Returns:
+        iterable (iterable): An iterable object.
+    """
+    return obj if hasattr(obj, "__iter__") else [obj]
 
-    def return_detail(self, key):
-        """
-        This will attempt to match a "detail" to look for in the room.
 
-        Args:
-            key (str): A detail identifier.
+# ------------------------------------------------------------
+# Client classes
+# ------------------------------------------------------------
 
-        Returns:
-            detail (str or None): A detail matching the given key.
 
-        Notes:
-            A detail is a way to offer more things to look at in a room
-            without having to add new objects. For this to work, we
-            require a custom `look` command that allows for `look
-            <detail>` - the look command should defer to this method on
-            the current location (if it exists) before giving up on
-            finding the target.
-
-            Details are not season-sensitive, but are parsed for timeslot
-            markers.
-        """
-        try:
-            detail = self.db.details.get(key.lower(), None)
-        except AttributeError:
-            # this happens if no attribute details is set at all
-            return None
-        if detail:
-            season, timeslot = self.get_time_and_season()
-            detail = self.replace_timeslots(detail, timeslot)
-            return detail
-        return None
+class DummyClient(telnet.StatefulTelnetProtocol):
+    """
+    Handles connection to a running Evennia server,
+    mimicking a real account by sending commands on
+    a timer.
 
-    def set_detail(self, detailkey, description):
-        """
-        This sets a new detail, using an Attribute "details".
+    """
 
-        Args:
-            detailkey (str): The detail identifier to add (for
-                aliases you need to add multiple keys to the
-                same description). Case-insensitive.
-            description (str): The text to return when looking
-                at the given detailkey.
+    def report(self, text, clientkey):
+        pad = " " * (25 - len(text))
+        tim = round(time.time() - self.connection_timestamp)
+        print(
+            f"{text} {clientkey}{pad}\t"
+            f"conn: {NCONNECTED} -> "
+            f"welcome screen: {NLOGIN_SCREEN} -> "
+            f"authing: {NLOGGING_IN} -> "
+            f"loggedin/tot: {NLOGGED_IN}/{NCLIENTS} (after {tim}s)"
+        )
 
+    def connectionMade(self):
         """
-        if self.db.details:
-            self.db.details[detailkey.lower()] = description
-        else:
-            self.db.details = {detailkey.lower(): description}
+        Called when connection is first established.
 
-    def del_detail(self, detailkey, description):
         """
-        Delete a detail.
-
-        The description is ignored.
-
-        Args:
-            detailkey (str): the detail to remove (case-insensitive).
-            description (str, ignored): the description.
+        global NCONNECTED
+        # public properties
+        self.cid = idcounter()
+        self.key = f"Dummy-{self.cid}"
+        self.gid = f"{time.strftime(DATESTRING)}_{self.cid}"
+        self.istep = 0
+        self.exits = []  # exit names created
+        self.objs = []  # obj names created
+        self.connection_timestamp = time.time()
+        self.connection_attempt = 0
+        self.action_started = 0
 
-        The description is only included for compliance but is completely
-        ignored.  Note that this method doesn't raise any exception if
-        the detail doesn't exist in this room.
+        self._connected = False
+        self._loggedin = False
+        self._logging_out = False
+        self._ready = False
+        self._report = ""
+        self._cmdlist = []  # already stepping in a cmd definition
+        self._login = self.factory.actions[0]
+        self._logout = self.factory.actions[1]
+        self._actions = self.factory.actions[2:]
 
-        """
-        if self.db.details and detailkey.lower() in self.db.details:
-            del self.db.details[detailkey.lower()]
+        reactor.addSystemEventTrigger("before", "shutdown", self.logout)
 
-    def return_appearance(self, looker, **kwargs):
-        """
-        This is called when e.g. the look command wants to retrieve
-        the description of this object.
+        NCONNECTED += 1
+        self.report("-> connected", self.key)
 
-        Args:
-            looker (Object): The object looking at us.
-            **kwargs (dict): Arbitrary, optional arguments for users
-                overriding the call (unused by default).
+        reactor.callLater(30, self._retry_welcome_screen)
 
-        Returns:
-            description (str): Our description.
+    def _retry_welcome_screen(self):
+        if not self._connected and not self._ready:
+            # we have connected but not received anything for 30s.
+            # (unclear why this would be - overload?)
+            # try sending a look to get something to start with
+            self.report("?? retrying welcome screen", self.key)
+            self.sendLine(bytes("look", "utf-8"))
+            # make sure to check again later
+            reactor.callLater(30, self._retry_welcome_screen)
 
-        """
-        # ensures that our description is current based on time/season
-        self.update_current_description()
-        # run the normal return_appearance method, now that desc is updated.
-        return super().return_appearance(looker, **kwargs)
-
-    def update_current_description(self):
-        """
-        This will update the description of the room if the time or season
-        has changed since last checked.
-        """
-        update = False
-        # get current time and season
-        curr_season, curr_timeslot = self.get_time_and_season()
-        # compare with previously stored slots
-        last_season = self.ndb.last_season
-        last_timeslot = self.ndb.last_timeslot
-        if curr_season != last_season:
-            # season changed. Load new desc, or a fallback.
-            new_raw_desc = self.attributes.get("%s_desc" % curr_season)
-            if new_raw_desc:
-                raw_desc = new_raw_desc
-            else:
-                # no seasonal desc set. Use fallback
-                raw_desc = self.db.general_desc or self.db.desc
-            self.db.raw_desc = raw_desc
-            self.ndb.last_season = curr_season
-            update = True
-        if curr_timeslot != last_timeslot:
-            # timeslot changed. Set update flag.
-            self.ndb.last_timeslot = curr_timeslot
-            update = True
-        if update:
-            # if anything changed we have to re-parse
-            # the raw_desc for time markers
-            # and re-save the description again.
-            self.db.desc = self.replace_timeslots(self.db.raw_desc, curr_timeslot)
+    def _print_statistics(self):
+        global TIME_ALL_LOGIN, TOTAL_ACTIONS
+        global TOTAL_LAG, TOTAL_LAG_MEASURES, TOTAL_LAG_IN, TOTAL_LAG_OUT
 
+        tim = time.time() - TIME_ALL_LOGIN
+        avgrate = round(TOTAL_ACTIONS / tim)
+        lag = TOTAL_LAG / (TOTAL_LAG_MEASURES or 1)
+        lag_in = TOTAL_LAG_IN / (TOTAL_LAG_MEASURES or 1)
+        lag_out = TOTAL_LAG_OUT / (TOTAL_LAG_MEASURES or 1)
 
-# Custom Look command supporting Room details. Add this to
-# the Default cmdset to use.
+        TOTAL_ACTIONS = 0
+        TOTAL_LAG = 0
+        TOTAL_LAG_IN = 0
+        TOTAL_LAG_OUT = 0
+        TOTAL_LAG_MEASURES = 0
+        TIME_ALL_LOGIN = time.time()
 
+        print(
+            f".. running 30s average: ~{avgrate} actions/s "
+            f"lag: {lag:.2}s (in: {lag_in:.2}s, out: {lag_out:.2}s)"
+        )
 
-class CmdExtendedRoomLook(default_cmds.CmdLook):
-    """
-    look
+        reactor.callLater(30, self._print_statistics)
 
-    Usage:
-      look
-      look <obj>
-      look <room detail>
-      look *<account>
+    def dataReceived(self, data):
+        """
+        Called when data comes in over the protocol. We wait to start
+        stepping until the server actually responds
 
-    Observes your location, details at your location or objects in your vicinity.
-    """
+        Args:
+            data (str): Incoming data.
 
-    def func(self):
         """
-        Handle the looking - add fallback to details.
-        """
-        caller = self.caller
-        args = self.args
-        if args:
-            looking_at_obj = caller.search(
-                args,
-                candidates=caller.location.contents + caller.contents,
-                use_nicks=True,
-                quiet=True,
-            )
-            if not looking_at_obj:
-                # no object found. Check if there is a matching
-                # detail at location.
-                location = caller.location
-                if (
-                    location
-                    and hasattr(location, "return_detail")
-                    and callable(location.return_detail)
-                ):
-                    detail = location.return_detail(args)
-                    if detail:
-                        # we found a detail
-                        # tell all the objects in the room we're looking closely at something
-                        caller.location.msg_contents(f"$You() $conj(look) closely at {args}.\n", from_obj=caller)
-                        # show the detail to the player
-                        caller.msg(detail)
-                        return
-                # no detail found. Trigger delayed error messages
-                _AT_SEARCH_RESULT(looking_at_obj, caller, args, quiet=False)
-                return
-            else:
-                # we need to extract the match manually.
-                looking_at_obj = utils.make_iter(looking_at_obj)[0]
-        else:
-            looking_at_obj = caller.location
-            if not looking_at_obj:
-                caller.msg("You have no location to look at!")
-                return
-
-        if not hasattr(looking_at_obj, "return_appearance"):
-            # this is likely due to us having an account instead
-            looking_at_obj = looking_at_obj.character
-        if not looking_at_obj.access(caller, "view"):
-            caller.msg("Could not find '%s'." % args)
-            return
-        # get object's appearance
-        caller.msg(looking_at_obj.return_appearance(caller))
-        # the object's at_desc() method.
-        looking_at_obj.at_desc(looker=caller)
+        global NLOGIN_SCREEN, NLOGGED_IN, NLOGGING_IN, NCONNECTED
+        global TOTAL_ACTIONS, TIME_ALL_LOGIN
+        global TOTAL_LAG, TOTAL_LAG_MEASURES, TOTAL_LAG_IN, TOTAL_LAG_OUT
+
+        if not data.startswith(b"\xff"):
+            # regular text, not a telnet command
+
+            if NCLIENTS == 1:
+                print("dummy-client sees:", str(data, "utf-8"))
+
+            if not self._connected:
+                # waiting for connection
+                # wait until we actually get text back (not just telnet
+                # negotiation)
+                # start client tick
+                d = LoopingCall(self.step)
+                df = max(abs(TIMESTEP * 0.001), min(TIMESTEP / 10, 0.5))
+                # dither next attempt with random time
+                timestep = TIMESTEP + (-df + (random.random() * df))
+                d.start(timestep, now=True).addErrback(self.error)
+                self.connection_attempt += 1
+
+                self._connected = True
+                NLOGIN_SCREEN += 1
+                NCONNECTED -= 1
+                self.report("<- server sent login screen", self.key)
+
+            elif self._loggedin:
+                if not self._ready:
+                    # logged in, ready to run
+                    NLOGGED_IN += 1
+                    NLOGGING_IN -= 1
+                    self._ready = True
+                    self.report("== logged in", self.key)
+                    if NLOGGED_IN == NCLIENTS and not TIME_ALL_LOGIN:
+                        # all are logged in! We can start collecting statistics
+                        print(".. All clients connected and logged in!")
+                        TIME_ALL_LOGIN = time.time()
+                        reactor.callLater(30, self._print_statistics)
+
+                elif TIME_ALL_LOGIN:
+                    TOTAL_ACTIONS += 1
+
+                    try:
+                        data = strip_ansi(str(data, "utf-8").strip())
+                        if data.startswith("dummyrunner_echo_response:"):
+                            # handle special lag-measuring command. This returns
+                            # dummyrunner_echo_response:<starttime>,<midpointtime>
+                            now = time.time()
+                            _, data = data.split(":", 1)
+                            start_time, mid_time = (float(part) for part in data.split(",", 1))
+                            lag_in = mid_time - start_time
+                            lag_out = now - mid_time
+                            total_lag = now - start_time  # full round-about time
+
+                            TOTAL_LAG += total_lag
+                            TOTAL_LAG_IN += lag_in
+                            TOTAL_LAG_OUT += lag_out
+                            TOTAL_LAG_MEASURES += 1
+                    except Exception:
+                        pass
 
+    def connectionLost(self, reason):
+        """
+        Called when loosing the connection.
 
-# Custom build commands for setting seasonal descriptions
-# and detailing extended rooms.
+        Args:
+            reason (str): Reason for loosing connection.
 
+        """
+        if not self._logging_out:
+            self.report("XX lost connection", self.key)
 
-class CmdExtendedRoomDesc(default_cmds.CmdDesc):
-    """
-    `desc` - describe an object or room.
+    def error(self, err):
+        """
+        Error callback.
 
-    Usage:
-      desc[/switch] [<obj> =] <description>
+        Args:
+            err (Failure): Error instance.
+        """
+        print(err)
 
-    Switches for `desc`:
-      spring  - set description for <season> in current room.
-      summer
-      autumn
-      winter
+    def counter(self):
+        """
+        Produces a unique id, also between clients.
 
-    Sets the "desc" attribute on an object. If an object is not given,
-    describe the current room.
+        Returns:
+            counter (int): A unique counter.
 
-    You can also embed special time markers in your room description, like this:
+        """
+        return gidcounter()
 
-        ```
-        <night>In the darkness, the forest looks foreboding.</night>.
-        ```
+    def logout(self):
+        """
+        Causes the client to log out of the server. Triggered by ctrl-c signal.
 
-    Text marked this way will only display when the server is truly at the given
-    timeslot. The available times are night, morning, afternoon and evening.
+        """
+        self._logging_out = True
+        cmd = self._logout(self)[0]
+        self.report(f"-> logout/disconnect ({self.istep} actions)", self.key)
+        self.sendLine(bytes(cmd, "utf-8"))
 
-    Note that seasons and time-of-day slots only work on rooms in this
-    version of the `desc` command.
+    def step(self):
+        """
+        Perform a step. This is called repeatedly by the runner and
+        causes the client to issue commands to the server.  This holds
+        all "intelligence" of the dummy client.
 
-    """
+        """
+        global NLOGGING_IN, NLOGIN_SCREEN
 
-    aliases = ["describe"]
-    switch_options = ()  # Inherits from default_cmds.CmdDesc, but unused here
+        rand = random.random()
 
-    def reset_times(self, obj):
-        """By deleteting the caches we force a re-load."""
-        obj.ndb.last_season = None
-        obj.ndb.last_timeslot = None
+        if not self._cmdlist:
+            # no commands ready. Load some.
 
-    def func(self):
-        """Define extended command"""
-        caller = self.caller
-        location = caller.location
-        if not self.args:
-            if location:
-                string = "|wDescriptions on %s|n:\n" % location.key
-                string += " |wspring:|n %s\n" % location.db.spring_desc
-                string += " |wsummer:|n %s\n" % location.db.summer_desc
-                string += " |wautumn:|n %s\n" % location.db.autumn_desc
-                string += " |wwinter:|n %s\n" % location.db.winter_desc
-                string += " |wgeneral:|n %s" % location.db.general_desc
-                caller.msg(string)
-                return
-        if self.switches and self.switches[0] in ("spring", "summer", "autumn", "winter"):
-            # a seasonal switch was given
-            if self.rhs:
-                caller.msg("Seasonal descs only work with rooms, not objects.")
-                return
-            switch = self.switches[0]
-            if not location:
-                caller.msg("No location was found!")
-                return
-            if switch == "spring":
-                location.db.spring_desc = self.args
-            elif switch == "summer":
-                location.db.summer_desc = self.args
-            elif switch == "autumn":
-                location.db.autumn_desc = self.args
-            elif switch == "winter":
-                location.db.winter_desc = self.args
-            # clear flag to force an update
-            self.reset_times(location)
-            caller.msg("Seasonal description was set on %s." % location.key)
-        else:
-            # No seasonal desc set, maybe this is not an extended room
-            if self.rhs:
-                text = self.rhs
-                obj = caller.search(self.lhs)
-                if not obj:
+            if not self._loggedin:
+                if rand < CHANCE_OF_LOGIN or NLOGGING_IN < 10:
+                    # lower rate of logins, but not below 1 / s
+                    # get the login commands
+                    self._cmdlist = list(makeiter(self._login(self)))
+                    NLOGGING_IN += 1  # this is for book-keeping
+                    NLOGIN_SCREEN -= 1
+                    self.report("-> create/login", self.key)
+                    self._loggedin = True
+                else:
+                    # no login yet, so cmdlist not yet set
                     return
             else:
-                text = self.args
-                obj = location
-            obj.db.desc = text  # a compatibility fallback
-            if obj.attributes.has("general_desc"):
-                obj.db.general_desc = text
-                self.reset_times(obj)
-                caller.msg("General description was set on %s." % obj.key)
-            else:
-                # this is not an ExtendedRoom.
-                caller.msg("The description was set on %s." % obj.key)
-
-
-class CmdExtendedRoomDetail(default_cmds.MuxCommand):
-
-    """
-    sets a detail on a room
-
-    Usage:
-        @detail[/del] <key> [= <description>]
-        @detail <key>;<alias>;... = description
-
-    Example:
-        @detail
-        @detail walls = The walls are covered in ...
-        @detail castle;ruin;tower = The distant ruin ...
-        @detail/del wall
-        @detail/del castle;ruin;tower
-
-    This command allows to show the current room details if you enter it
-    without any argument.  Otherwise, sets or deletes a detail on the current
-    room, if this room supports details like an extended room. To add new
-    detail, just use the @detail command, specifying the key, an equal sign
-    and the description.  You can assign the same description to several
-    details using the alias syntax (replace key by alias1;alias2;alias3;...).
-    To remove one or several details, use the @detail/del switch.
-
-    """
-
-    key = "@detail"
-    locks = "cmd:perm(Builder)"
-    help_category = "Building"
+                # we always pick a cumulatively random function
+                crand = random.random()
+                cfunc = [func for (cprob, func) in self._actions if cprob >= crand][0]
+                self._cmdlist = list(makeiter(cfunc(self)))
+
+        # at this point we always have a list of commands
+        if rand < CHANCE_OF_ACTION:
+            # send to the game
+            cmd = str(self._cmdlist.pop(0))
+
+            if cmd.startswith("dummyrunner_echo_response"):
+                # we need to set the timer element as close to
+                # the send as possible
+                cmd = cmd.format(timestamp=time.time())
+
+            self.sendLine(bytes(cmd, "utf-8"))
+            self.action_started = time.time()
+            self.istep += 1
+
+            if NCLIENTS == 1:
+                print(f"dummy-client sent: {cmd}")
+
+
+class DummyFactory(protocol.ReconnectingClientFactory):
+    protocol = DummyClient
+    initialDelay = 1
+    maxDelay = 1
+    noisy = False
+
+    def __init__(self, actions):
+        "Setup the factory base (shared by all clients)"
+        self.actions = actions
+
+
+# ------------------------------------------------------------
+# Access method:
+# Starts clients and connects them to a running server.
+# ------------------------------------------------------------
+
+
+def start_all_dummy_clients(nclients):
+    """
+    Initialize all clients, connect them and start to step them
+
+    Args:
+        nclients (int): Number of dummy clients to connect.
+
+    """
+    global NCLIENTS
+    NCLIENTS = int(nclients)
+    actions = DUMMYRUNNER_SETTINGS.ACTIONS
+
+    if len(actions) < 2:
+        print(ERROR_FEW_ACTIONS)
+        return
+
+    # make sure the probabilities add up to 1
+    pratio = 1.0 / sum(tup[0] for tup in actions[2:])
+    flogin, flogout, probs, cfuncs = (
+        actions[0],
+        actions[1],
+        [tup[0] * pratio for tup in actions[2:]],
+        [tup[1] for tup in actions[2:]],
+    )
+    # create cumulative probabilies for the random actions
+    cprobs = [sum(v for i, v in enumerate(probs) if i <= k) for k in range(len(probs))]
+    # rebuild a new, optimized action structure
+    actions = (flogin, flogout) + tuple(zip(cprobs, cfuncs))
+
+    # setting up all clients (they are automatically started)
+    factory = DummyFactory(actions)
+    for i in range(NCLIENTS):
+        reactor.connectTCP("127.0.0.1", TELNET_PORT, factory)
+    # start reactor
+    reactor.run()
+
+
+# ------------------------------------------------------------
+# Command line interface
+# ------------------------------------------------------------
+
+
+if __name__ == "__main__":
+
+    try:
+        settings.DUMMYRUNNER_MIXIN
+    except AttributeError:
+        print(ERROR_NO_MIXIN)
+        sys.exit()
+
+    # parsing command line with default vals
+    parser = ArgumentParser(description=HELPTEXT)
+    parser.add_argument(
+        "-N", nargs=1, default=1, dest="nclients", help="Number of clients to start"
+    )
+
+    args = parser.parse_args()
+    nclients = int(args.nclients[0])
+
+    print(
+        INFO_STARTING.format(
+            nclients=nclients,
+            port=TELNET_PORT,
+            idmapper_cache_size=IDMAPPER_CACHE_MAXSIZE,
+            timestep=TIMESTEP,
+            rate=1 / TIMESTEP,
+            chance_of_login=CHANCE_OF_LOGIN * 100,
+            chance_of_action=CHANCE_OF_ACTION * 100,
+            avg_rate=(1 / TIMESTEP) * CHANCE_OF_ACTION,
+            avg_rate_total=(1 / TIMESTEP) * CHANCE_OF_ACTION * nclients,
+        )
+    )
+
+    # run the dummyrunner
+    TIME_START = t0 = time.time()
+    start_all_dummy_clients(nclients=nclients)
+    ttot = time.time() - t0
 
-    def func(self):
-        location = self.caller.location
-        if not self.args:
-            details = location.db.details
-            if not details:
-                self.msg("|rThe room {} doesn't have any detail set.|n".format(location))
-            else:
-                details = sorted(["|y{}|n: {}".format(key, desc) for key, desc in details.items()])
-                self.msg("Details on Room:\n" + "\n".join(details))
-            return
-
-        if not self.rhs and "del" not in self.switches:
-            detail = location.return_detail(self.lhs)
-            if detail:
-                self.msg("Detail '|y{}|n' on Room:\n{}".format(self.lhs, detail))
-            else:
-                self.msg("Detail '{}' not found.".format(self.lhs))
-            return
-
-        method = "set_detail" if "del" not in self.switches else "del_detail"
-        if not hasattr(location, method):
-            self.caller.msg("Details cannot be set on %s." % location)
-            return
-        for key in self.lhs.split(";"):
-            # loop over all aliases, if any (if not, this will just be
-            # the one key to loop over)
-            getattr(location, method)(key, self.rhs)
-        if "del" in self.switches:
-            self.caller.msg("Detail %s deleted, if it existed." % self.lhs)
-        else:
-            self.caller.msg("Detail set '%s': '%s'" % (self.lhs, self.rhs))
-
-
-# Simple command to view the current time and season
-
-
-class CmdExtendedRoomGameTime(default_cmds.MuxCommand):
-    """
-    Check the game time
-
-    Usage:
-        time
-
-    Shows the current in-game time and season.
-    """
-
-    key = "time"
-    locks = "cmd:all()"
-    help_category = "General"
-
-    def func(self):
-        """Reads time info from current room"""
-        location = self.caller.location
-        if not location or not hasattr(location, "get_time_and_season"):
-            self.caller.msg("No location available - you are outside time.")
-        else:
-            season, timeslot = location.get_time_and_season()
-            prep = "a"
-            if season == "autumn":
-                prep = "an"
-            self.caller.msg("It's %s %s day, in the %s." % (prep, season, timeslot))
-
-
-# CmdSet for easily install all commands
-
-
-class ExtendedRoomCmdSet(CmdSet):
-    """
-    Groups the extended-room commands.
-
-    """
-
-    def at_cmdset_creation(self):
-        self.add(CmdExtendedRoomLook)
-        self.add(CmdExtendedRoomDesc)
-        self.add(CmdExtendedRoomDetail)
-        self.add(CmdExtendedRoomGameTime)
+    # output runtime
+    print("... dummy client runner stopped after %s." % time_format(ttot, style=3))
```

### Comparing `evennia-1.3.0/evennia/contrib/grid/ingame_map_display/README.md` & `evennia-2.0.0/evennia/contrib/grid/ingame_map_display/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/grid/ingame_map_display/ingame_map_display.py` & `evennia-2.0.0/evennia/contrib/grid/ingame_map_display/ingame_map_display.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/grid/ingame_map_display/tests.py` & `evennia-2.0.0/evennia/contrib/grid/ingame_map_display/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/grid/mapbuilder/README.md` & `evennia-2.0.0/evennia/contrib/grid/mapbuilder/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/grid/mapbuilder/mapbuilder.py` & `evennia-2.0.0/evennia/contrib/grid/mapbuilder/mapbuilder.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/grid/mapbuilder/tests.py` & `evennia-2.0.0/evennia/contrib/grid/mapbuilder/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/grid/simpledoor/README.md` & `evennia-2.0.0/evennia/contrib/grid/simpledoor/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/grid/simpledoor/simpledoor.py` & `evennia-2.0.0/evennia/contrib/grid/simpledoor/simpledoor.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/grid/simpledoor/tests.py` & `evennia-2.0.0/evennia/contrib/grid/simpledoor/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/grid/slow_exit/README.md` & `evennia-2.0.0/evennia/contrib/grid/slow_exit/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/grid/slow_exit/slow_exit.py` & `evennia-2.0.0/evennia/contrib/grid/slow_exit/slow_exit.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/grid/slow_exit/tests.py` & `evennia-2.0.0/evennia/contrib/grid/slow_exit/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/grid/wilderness/README.md` & `evennia-2.0.0/evennia/contrib/grid/wilderness/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/grid/wilderness/tests.py` & `evennia-2.0.0/evennia/contrib/grid/wilderness/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/grid/wilderness/wilderness.py` & `evennia-2.0.0/evennia/contrib/grid/wilderness/wilderness.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/grid/xyzgrid/README.md` & `evennia-2.0.0/evennia/contrib/grid/xyzgrid/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/grid/xyzgrid/commands.py` & `evennia-2.0.0/evennia/contrib/grid/xyzgrid/commands.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/grid/xyzgrid/example.py` & `evennia-2.0.0/evennia/contrib/grid/xyzgrid/example.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/grid/xyzgrid/launchcmd.py` & `evennia-2.0.0/evennia/contrib/grid/xyzgrid/launchcmd.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/grid/xyzgrid/prototypes.py` & `evennia-2.0.0/evennia/contrib/grid/xyzgrid/prototypes.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/grid/xyzgrid/tests.py` & `evennia-2.0.0/evennia/contrib/grid/xyzgrid/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/grid/xyzgrid/utils.py` & `evennia-2.0.0/evennia/contrib/grid/xyzgrid/utils.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/grid/xyzgrid/xymap.py` & `evennia-2.0.0/evennia/contrib/grid/xyzgrid/xymap.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/grid/xyzgrid/xymap_legend.py` & `evennia-2.0.0/evennia/contrib/grid/xyzgrid/xymap_legend.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/grid/xyzgrid/xyzgrid.py` & `evennia-2.0.0/evennia/contrib/grid/xyzgrid/xyzgrid.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/grid/xyzgrid/xyzroom.py` & `evennia-2.0.0/evennia/contrib/grid/xyzgrid/xyzroom.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/rpg/buffs/README.md` & `evennia-2.0.0/evennia/contrib/rpg/buffs/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/rpg/buffs/buff.py` & `evennia-2.0.0/evennia/contrib/rpg/buffs/buff.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/rpg/buffs/samplebuffs.py` & `evennia-2.0.0/evennia/contrib/rpg/buffs/samplebuffs.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/rpg/buffs/tests.py` & `evennia-2.0.0/evennia/contrib/rpg/buffs/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/rpg/character_creator/README.md` & `evennia-2.0.0/evennia/contrib/rpg/character_creator/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/rpg/character_creator/character_creator.py` & `evennia-2.0.0/evennia/contrib/rpg/character_creator/character_creator.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/rpg/character_creator/example_menu.py` & `evennia-2.0.0/evennia/contrib/rpg/character_creator/example_menu.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/rpg/character_creator/tests.py` & `evennia-2.0.0/evennia/contrib/rpg/character_creator/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/rpg/dice/README.md` & `evennia-2.0.0/evennia/contrib/rpg/dice/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/rpg/dice/dice.py` & `evennia-2.0.0/evennia/contrib/rpg/dice/dice.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/rpg/dice/tests.py` & `evennia-2.0.0/evennia/contrib/rpg/dice/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/rpg/health_bar/README.md` & `evennia-2.0.0/evennia/contrib/rpg/health_bar/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/rpg/health_bar/health_bar.py` & `evennia-2.0.0/evennia/contrib/rpg/health_bar/health_bar.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/rpg/health_bar/tests.py` & `evennia-2.0.0/evennia/contrib/rpg/health_bar/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/rpg/rpsystem/README.md` & `evennia-2.0.0/evennia/contrib/rpg/rpsystem/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/rpg/rpsystem/__init__.py` & `evennia-2.0.0/evennia/contrib/rpg/rpsystem/__init__.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/rpg/rpsystem/rplanguage.py` & `evennia-2.0.0/evennia/contrib/rpg/rpsystem/rplanguage.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/rpg/rpsystem/rpsystem.py` & `evennia-2.0.0/evennia/contrib/rpg/rpsystem/rpsystem.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/rpg/rpsystem/tests.py` & `evennia-2.0.0/evennia/contrib/rpg/rpsystem/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/rpg/traits/README.md` & `evennia-2.0.0/evennia/contrib/rpg/traits/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/rpg/traits/tests.py` & `evennia-2.0.0/evennia/contrib/rpg/traits/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/rpg/traits/traits.py` & `evennia-2.0.0/evennia/contrib/rpg/traits/traits.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/tutorials/batchprocessor/README.md` & `evennia-2.0.0/evennia/contrib/tutorials/batchprocessor/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/tutorials/batchprocessor/example_batch_cmds.ev` & `evennia-2.0.0/evennia/contrib/tutorials/batchprocessor/example_batch_cmds.ev`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/tutorials/batchprocessor/example_batch_code.py` & `evennia-2.0.0/evennia/contrib/tutorials/batchprocessor/example_batch_code.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/tutorials/bodyfunctions/bodyfunctions.py` & `evennia-2.0.0/evennia/contrib/tutorials/bodyfunctions/bodyfunctions.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/tutorials/bodyfunctions/tests.py` & `evennia-2.0.0/evennia/contrib/tutorials/bodyfunctions/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/tutorials/evadventure/README.md` & `evennia-2.0.0/evennia/contrib/tutorials/evadventure/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # EvAdventure
 
-Contrib by Griatch 2022
+Contrib by Griatch 2023-
 
 
 ```{warning}
-NOTE - this tutorial is WIP and NOT complete! It was put on hold to focus on
-releasing Evennia 1.0. You will still learn things from it, but don't expect
-perfection.
+NOTE - this tutorial is WIP and NOT complete yet! You will still learn
+things from it, but don't expect perfection.
 ```
 
 A complete example MUD using Evennia. This is the final result of what is
-implemented if you follow the Getting-Started tutorial. It's recommended
-that you follow the tutorial step by step and write your own code. But if
-you prefer you can also pick apart or use this as a starting point for your
-own game.
+implemented if you follow [Part 3 of the Getting-Started tutorial](Beginner-Tutorial-Part3-Overview).
+It's recommended that you follow the tutorial step by step and write your own
+code. But if you prefer you can also pick apart or use this as a starting point
+for your own game.
 
 ## Features
 
 - Uses a MUD-version of the [Knave](https://rpggeek.com/rpg/50827/knave) old-school
   fantasy ruleset by Ben Milton (classless and overall compatible with early
   edition D&D), released under the Creative Commons Attribution (all uses,
   including commercial are allowed
```

### Comparing `evennia-1.3.0/evennia/contrib/tutorials/evadventure/build_techdemo.py` & `evennia-2.0.0/evennia/contrib/tutorials/evadventure/build_techdemo.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/tutorials/evadventure/characters.py` & `evennia-2.0.0/evennia/contrib/tutorials/evadventure/characters.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,23 +2,21 @@
 Character class.
 
 """
 
 from evennia.objects.objects import DefaultCharacter
 from evennia.typeclasses.attributes import AttributeProperty
 from evennia.utils.evform import EvForm
-from evennia.utils.evmenu import EvMenu, ask_yes_no
 from evennia.utils.evtable import EvTable
 from evennia.utils.logger import log_trace
 from evennia.utils.utils import lazy_property
 
 from . import rules
 from .equipment import EquipmentError, EquipmentHandler
 from .quests import EvAdventureQuestHandler
-from .utils import get_obj_stats
 
 
 class LivingMixin:
     """
     Mixin class to use for all living things.
 
     """
@@ -60,14 +58,21 @@
         if healer is self:
             self.msg(f"|gYou heal yourself for {healed} health.|n")
         elif healer:
             self.msg(f"|g{healer.key} heals you for {healed} health.|n")
         else:
             self.msg(f"You are healed for {healed} health.")
 
+    def at_attacked(self, attacker, **kwargs):
+        """
+        Called when being attacked / combat starts.
+
+        """
+        pass
+
     def at_damage(self, damage, attacker=None):
         """
         Called when attacked and taking damage.
 
         """
         self.hp -= damage
```

### Comparing `evennia-1.3.0/evennia/contrib/tutorials/evadventure/chargen.py` & `evennia-2.0.0/evennia/contrib/tutorials/evadventure/chargen.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """
 EvAdventure character generation.
 
 """
 from django.conf import settings
-
-from evennia import create_object
 from evennia.objects.models import ObjectDB
 from evennia.prototypes.spawner import spawn
+from evennia.utils.create import create_object
 from evennia.utils.evmenu import EvMenu
 
 from .characters import EvAdventureCharacter
 from .random_tables import chargen_tables
 from .rules import dice
 
 _ABILITIES = {
```

### Comparing `evennia-1.3.0/evennia/contrib/tutorials/evadventure/combat_turnbased.py` & `evennia-2.0.0/evennia/contrib/tutorials/tutorial_world/rooms.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,1411 +1,1198 @@
 """
-EvAdventure turn-based combat
 
-This implements a turn-based combat style, where both sides have a little longer time to
-choose their next action. If they don't react before a timer runs out, the previous action
-will be repeated. This means that a 'twitch' style combat can be created using the same
-mechanism, by just speeding up each 'turn'.
+Room Typeclasses for the TutorialWorld.
 
-The combat is handled with a `Script` shared between all combatants; this tracks the state
-of combat and handles all timing elements.
+This defines special types of Rooms available in the tutorial. To keep
+everything in one place we define them together with the custom
+commands needed to control them. Those commands could also have been
+in a separate module (e.g. if they could have been re-used elsewhere.)
 
-Unlike in base _Knave_, the MUD version's combat is simultaneous; everyone plans and executes
-their turns simultaneously with minimum downtime.
-
-This version is simplified to not worry about things like optimal range etc. So a bow can be used
-the same as a sword in battle. One could add a 1D range mechanism to add more strategy by requiring
-optimizal positioning.
-
-The combat is controlled through a menu:
+"""
 
-------------------- main menu
-Combat
 
-You have 30 seconds to choose your next action. If you don't decide, you will hesitate and do
-nothing. Available actions:
+import random
 
-1. [A]ttack/[C]ast spell at <target> using your equipped weapon/spell
-3. Make [S]tunt <target/yourself> (gain/give advantage/disadvantage for future attacks)
-4. S[W]ap weapon / spell rune
-5. [U]se <item>
-6. [F]lee/disengage (takes two turns)
-7. [B]lock <target> from fleeing
-8. [H]esitate/Do nothing
+# the system error-handling module is defined in the settings. We load the
+# given setting here using utils.object_from_module. This way we can use
+# it regardless of if we change settings later.
+from django.conf import settings
 
-You can also use say/emote between rounds.
-As soon as all combatants have made their choice (or time out), the round will be resolved
-simultaneusly.
+from evennia import (
+    TICKER_HANDLER,
+    CmdSet,
+    Command,
+    DefaultExit,
+    DefaultRoom,
+    create_object,
+    default_cmds,
+    search_object,
+    syscmdkeys,
+    utils,
+)
 
--------------------- attack/cast spell submenu
+from .objects import LightSource
 
-Choose the target of your attack/spell:
-0: Yourself              3: <enemy 3> (wounded)
-1: <enemy 1> (hurt)
-2: <enemy 2> (unharmed)
+_SEARCH_AT_RESULT = utils.object_from_module(settings.SEARCH_AT_RESULT)
 
-------------------- make stunt submenu
+# -------------------------------------------------------------
+#
+# Tutorial room - parent room class
+#
+# This room is the parent of all rooms in the tutorial.
+# It defines a tutorial command on itself (available to
+# all those who are in a tutorial room).
+#
+# -------------------------------------------------------------
 
-Stunts are special actions that don't cause damage but grant advantage for you or
-an ally for future attacks - or grant disadvantage to your enemy's future attacks.
-The effects of stunts start to apply *next* round. The effect does not stack, can only
-be used once and must be taken advantage of within 5 rounds.
+#
+# Special command available in all tutorial rooms
 
-Choose stunt:
-1: Trip <target> (give disadvantage DEX)
-2: Feint <target> (get advantage DEX against target)
-3: ...
 
--------------------- make stunt target submenu
+class CmdTutorial(Command):
+    """
+    Get help during the tutorial
 
-Choose the target of your stunt:
-0: Yourself                  3: <combatant 3> (wounded)
-1: <combatant 1> (hurt)
-2: <combatant 2> (unharmed)
+    Usage:
+      tutorial [obj]
 
--------------------  swap weapon or spell run
+    This command allows you to get behind-the-scenes info
+    about an object or the current location.
 
-Choose the item to wield.
-1: <item1>
-2: <item2> (two hands)
-3: <item3>
-4: ...
+    """
 
-------------------- use item
+    key = "tutorial"
+    aliases = ["tut"]
+    locks = "cmd:all()"
+    help_category = "TutorialWorld"
 
-Choose item to use.
-1: Healing potion (+1d6 HP)
-2: Magic pebble (gain advantage, 1 use)
-3: Potion of glue (give disadvantage to target)
+    def func(self):
+        """
+        All we do is to scan the current location for an Attribute
+        called `tutorial_info` and display that.
+        """
 
-------------------- Hesitate/Do nothing
+        caller = self.caller
 
-You hang back, passively defending.
+        if not self.args:
+            target = self.obj  # this is the room the command is defined on
+        else:
+            target = caller.search(self.args.strip())
+            if not target:
+                return
+        helptext = target.db.tutorial_info or ""
 
-------------------- Disengage
+        if helptext:
+            helptext = f" |G{helptext}|n"
+        else:
+            helptext = " |RSorry, there is no tutorial help available here.|n"
+        helptext += "\n\n (Write 'give up' if you want to abandon your quest.)"
+        caller.msg(helptext)
 
-You retreat, getting ready to get out of combat. Use two times in a row to
-leave combat. You flee last in a round. If anyone Blocks your retreat, this counter resets.
 
-------------------- Block Fleeing
+# for the @detail command we inherit from MuxCommand, since
+# we want to make use of MuxCommand's pre-parsing of '=' in the
+# argument.
+class CmdTutorialSetDetail(default_cmds.MuxCommand):
+    """
+    sets a detail on a room
 
-You move to block the escape route of an opponent. If you win a DEX challenge,
-you'll negate the target's disengage action(s).
+    Usage:
+        @detail <key> = <description>
+        @detail <key>;<alias>;... = description
 
-Choose who to block:
-1: <enemy 1>
-2: <enemy 2>
-3: ...
+    Example:
+        @detail walls = The walls are covered in ...
+        @detail castle;ruin;tower = The distant ruin ...
 
+    This sets a "detail" on the object this command is defined on
+    (TutorialRoom for this tutorial). This detail can be accessed with
+    the TutorialRoomLook command sitting on TutorialRoom objects (details
+    are set as a simple dictionary on the room). This is a Builder command.
 
-"""
+    We custom parse the key for the ;-separator in order to create
+    multiple aliases to the detail all at once.
+    """
 
-from collections import defaultdict
+    key = "@detail"
+    locks = "cmd:perm(Builder)"
+    help_category = "TutorialWorld"
 
-from evennia.scripts.scripts import DefaultScript
-from evennia.typeclasses.attributes import AttributeProperty
-from evennia.utils import dbserialize, delay, evmenu, evtable, logger
-from evennia.utils.utils import inherits_from
+    def func(self):
+        """
+        All this does is to check if the object has
+        the set_detail method and uses it.
+        """
+        if not self.args or not self.rhs:
+            self.caller.msg("Usage: @detail key = description")
+            return
+        if not hasattr(self.obj, "set_detail"):
+            self.caller.msg("Details cannot be set on %s." % self.obj)
+            return
+        for key in self.lhs.split(";"):
+            # loop over all aliases, if any (if not, this will just be
+            # the one key to loop over)
+            self.obj.set_detail(key, self.rhs)
+        self.caller.msg("Detail set: '%s': '%s'" % (self.lhs, self.rhs))
+
+
+class CmdTutorialLook(default_cmds.CmdLook):
+    """
+    looks at the room and on details
+
+    Usage:
+        look <obj>
+        look <room detail>
+        look *<account>
+
+    Observes your location, details at your location or objects
+    in your vicinity.
+
+    Tutorial: This is a child of the default Look command, that also
+    allows us to look at "details" in the room.  These details are
+    things to examine and offers some extra description without
+    actually having to be actual database objects. It uses the
+    return_detail() hook on TutorialRooms for this.
+    """
+
+    # we don't need to specify key/locks etc, this is already
+    # set by the parent.
+    help_category = "TutorialWorld"
+
+    def func(self):
+        """
+        Handle the looking. This is a copy of the default look
+        code except for adding in the details.
+        """
+        caller = self.caller
+        args = self.args
+        if args:
+            # we use quiet=True to turn off automatic error reporting.
+            # This tells search that we want to handle error messages
+            # ourself. This also means the search function will always
+            # return a list (with 0, 1 or more elements) rather than
+            # result/None.
+            looking_at_obj = caller.search(
+                args,
+                # note: excludes room/room aliases
+                candidates=caller.location.contents + caller.contents,
+                use_nicks=True,
+                quiet=True,
+            )
+            if len(looking_at_obj) != 1:
+                # no target found or more than one target found (multimatch)
+                # look for a detail that may match
+                detail = self.obj.return_detail(args)
+                if detail:
+                    self.caller.msg(detail)
+                    return
+                else:
+                    # no detail found, delegate our result to the normal
+                    # error message handler.
+                    _SEARCH_AT_RESULT(looking_at_obj, caller, args)
+                    return
+            else:
+                # we found a match, extract it from the list and carry on
+                # normally with the look handling.
+                looking_at_obj = looking_at_obj[0]
 
-from . import rules
-from .enums import Ability
-from .npcs import EvAdventureNPC
+        else:
+            looking_at_obj = caller.location
+            if not looking_at_obj:
+                caller.msg("You have no location to look at!")
+                return
 
-COMBAT_HANDLER_KEY = "evadventure_turnbased_combathandler"
-COMBAT_HANDLER_INTERVAL = 30
+        if not hasattr(looking_at_obj, "return_appearance"):
+            # this is likely due to us having an account instead
+            looking_at_obj = looking_at_obj.character
+        if not looking_at_obj.access(caller, "view"):
+            caller.msg("Could not find '%s'." % args)
+            return
+        # get object's appearance
+        caller.msg(looking_at_obj.return_appearance(caller))
+        # the object's at_desc() method.
+        looking_at_obj.at_desc(looker=caller)
+        return
 
 
-class CombatFailure(RuntimeError):
+class CmdTutorialGiveUp(default_cmds.MuxCommand):
     """
-    Some failure during actions.
+    Give up the tutorial-world quest and return to Limbo, the start room of the
+    server.
 
     """
 
+    key = "give up"
+    aliases = ["abort"]
 
-# -----------------------------------------------------------------------------------
-#  Combat Actions
-# -----------------------------------------------------------------------------------
-
+    def func(self):
+        outro_room = OutroRoom.objects.all()
+        if outro_room:
+            outro_room = outro_room[0]
+        else:
+            self.caller.msg(
+                "That didn't work (seems like a bug). "
+                "Try to use the |wteleport|n command instead."
+            )
+            return
 
-class CombatAction:
-    """
-    This is the base of a combat-action, like 'attack'  Inherit from this to make new actions.
+        self.caller.move_to(outro_room, move_type="teleport")
 
-    Note:
-        We want to store initialized version of this objects in the CombatHandler (in order to track
-        usages, time limits etc), so we need to make sure we can serialize it into an Attribute. See
-        `Attribute` documentation for more about `__serialize_dbobjs__` and
-        `__deserialize_dbobjs__`.
 
+class TutorialRoomCmdSet(CmdSet):
+    """
+    Implements the simple tutorial cmdset. This will overload the look
+    command in the default CharacterCmdSet since it has a higher
+    priority (ChracterCmdSet has prio 0)
     """
 
-    key = "Action"
-    desc = "Option text"
-    aliases = []
-    help_text = "Combat action to perform."
-
-    # the next combat menu node to go to - this ties the combat action into the UI
-    # use None to do nothing (jump directly to registering the action)
-    next_menu_node = "node_select_action"
+    key = "tutorial_cmdset"
+    priority = 1
 
-    max_uses = None  # None for unlimited
-    # in which order (highest first) to perform the action. If identical, use random order
-    priority = 0
+    def at_cmdset_creation(self):
+        """add the tutorial-room commands"""
+        self.add(CmdTutorial())
+        self.add(CmdTutorialSetDetail())
+        self.add(CmdTutorialLook())
+        self.add(CmdTutorialGiveUp())
 
-    def __init__(self, combathandler, combatant):
-        self.combathandler = combathandler
-        self.combatant = combatant
-        self.uses = 0
 
-    def msg(self, message, broadcast=True):
-        """
-        Convenience route to the combathandler msg-sender mechanism.
+class TutorialRoom(DefaultRoom):
+    """
+    This is the base room type for all rooms in the tutorial world.
+    It defines a cmdset on itself for reading tutorial info about the location.
+    """
 
-        Args:
-            message (str): Message to send; use `$You()` and `$You(other.key)`
-                to refer to the combatant doing the action and other combatants,
-                respectively.
-        """
-        self.combathandler.msg(message, combatant=self.combatant, broadcast=broadcast)
+    def at_object_creation(self):
+        """Called when room is first created"""
+        self.db.tutorial_info = (
+            "This is a tutorial room. It allows you to use the 'tutorial' command."
+        )
+        self.cmdset.add_default(TutorialRoomCmdSet)
 
-    def __serialize_dbobjs__(self):
+    def at_object_receive(self, new_arrival, source_location, move_type="move", **kwargs):
         """
-        This is necessary in order to be able to store this entity in an Attribute.
-        We must make sure to tell Evennia how to serialize internally stored db-objects.
-
-        The `__serialize_dbobjs__` and `__deserialize_dbobjs__` methods form a required pair.
+        When an object enter a tutorial room we tell other objects in
+        the room about it by trying to call a hook on them. The Mob object
+        uses this to cheaply get notified of enemies without having
+        to constantly scan for them.
 
-        """
-        self.combathandler = dbserialize.dbserialize(self.combathandler)
-        self.combatant = dbserialize.dbserialize(self.combatant)
+        Args:
+            new_arrival (Object): the object that just entered this room.
+            source_location (Object): the previous location of new_arrival.
 
-    def __deserialize_dbobjs__(self):
         """
-        This is necessary in order to be able to store this entity in an Attribute.
-        We must make sure to tell Evennia how to deserialize internally stored db-objects.
-
-        The `__serialize_dbobjs__` and `__deserialize_dbobjs__` methods form a required pair.
+        if new_arrival.has_account and not new_arrival.is_superuser:
+            # this is a character
+            for obj in self.contents_get(exclude=new_arrival):
+                if hasattr(obj, "at_new_arrival"):
+                    obj.at_new_arrival(new_arrival)
 
+    def return_detail(self, detailkey):
         """
-        if isinstance(self.combathandler, bytes):
-            self.combathandler = dbserialize.dbunserialize(self.combathandler)
-            self.combatant = dbserialize.dbunserialize(self.combatant)
+        This looks for an Attribute "obj_details" and possibly
+        returns the value of it.
 
-    def get_help(self, *args, **kwargs):
-        """
-        Allows to customize help message on the fly. By default, just returns `.help_text`.
+        Args:
+            detailkey (str): The detail being looked at. This is
+                case-insensitive.
 
         """
-        return self.help_text
+        details = self.db.details
+        if details:
+            return details.get(detailkey.lower(), None)
 
-    def can_use(self, *args, **kwargs):
+    def set_detail(self, detailkey, description):
         """
-        Determine if combatant can use this action. In this implementation,
-        it fails if already used up all of a usage-limited action.
+        This sets a new detail, using an Attribute "details".
 
         Args:
-            *args: Any optional arguments.
-            **kwargs: Any optional keyword arguments.
-
-        Returns:
-            tuple: (bool, motivation) - if not available, will describe why,
-                if available, should describe what the action does.
-
-        """
-        return True if self.max_uses is None else self.uses < (self.max_uses or 0)
+            detailkey (str): The detail identifier to add (for
+                aliases you need to add multiple keys to the
+                same description). Case-insensitive.
+            description (str): The text to return when looking
+                at the given detailkey.
 
-    def pre_use(self, *args, **kwargs):
         """
-        Called just before the main action.
+        if self.db.details:
+            self.db.details[detailkey.lower()] = description
+        else:
+            self.db.details = {detailkey.lower(): description}
 
-        """
 
-        pass
+class TutorialStartExit(DefaultExit):
+    """
+    This is like a normal exit except it makes the `intro` command available
+    on itself. We put it on the exit in order to provide this command to the
+    Limbo room without modifying Limbo itself - deleting the tutorial exit
+    will also  clean up the intro command.
 
-    def use(self, *args, **kwargs):
-        """
-        Main activation of the action. This happens simultaneously to other actions.
+    """
 
-        """
-        pass
+    def at_object_creation(self):
+        self.cmdset.add(CmdSetEvenniaIntro, persistent=True)
 
-    def post_use(self, *args, **kwargs):
-        """
-        Called just after the action has been taken.
 
-        """
-        pass
+# -------------------------------------------------------------
+#
+# Weather room - room with a ticker
+#
+# -------------------------------------------------------------
 
+# These are rainy weather strings
+WEATHER_STRINGS = (
+    "The rain coming down from the iron-grey sky intensifies.",
+    "A gust of wind throws the rain right in your face. Despite your cloak you shiver.",
+    "The rainfall eases a bit and the sky momentarily brightens.",
+    "For a moment it looks like the rain is slowing, then it begins anew with renewed force.",
+    "The rain pummels you with large, heavy drops. You hear the rumble of thunder in the distance.",
+    "The wind is picking up, howling around you, throwing water droplets in your face. It's cold.",
+    "Bright fingers of lightning flash over the sky, moments later followed by a deafening rumble.",
+    "It rains so hard you can hardly see your hand in front of you. You'll soon be drenched to the bone.",
+    "Lightning strikes in several thundering bolts, striking the trees in the forest to your west.",
+    "You hear the distant howl of what sounds like some sort of dog or wolf.",
+    "Large clouds rush across the sky, throwing their load of rain over the world.",
+)
 
-class CombatActionAttack(CombatAction):
-    """
-    A regular attack, using a wielded weapon. Depending on weapon type, this will be a ranged or
-    melee attack.
 
+class WeatherRoom(TutorialRoom):
     """
+    This should probably better be called a rainy room...
 
-    key = "Attack or Cast"
-    desc = "[A]ttack/[C]ast spell at <target>"
-    aliases = ("a", "c", "attack", "cast")
-    help_text = "Make an attack using your currently equipped weapon/spell rune"
-    next_menu_node = "node_select_enemy_target"
+    This sets up an outdoor room typeclass. At irregular intervals,
+    the effects of weather will show in the room. Outdoor rooms should
+    inherit from this.
 
-    priority = 1
+    """
 
-    def use(self, defender, *args, **kwargs):
+    def at_object_creation(self):
         """
-        Make an attack against a defender.
+        Called when object is first created.
+        We set up a ticker to update this room regularly.
 
+        Note that we could in principle also use a Script to manage
+        the ticking of the room; the TickerHandler works fine for
+        simple things like this though.
         """
-        attacker = self.combatant
-        weapon = self.combatant.weapon
-
-        # figure out advantage (gained by previous stunts)
-        advantage = bool(self.combathandler.advantage_matrix[attacker].pop(defender, False))
-        # figure out disadvantage (gained by enemy stunts/actions)
-        disadvantage = bool(self.combathandler.disadvantage_matrix[attacker].pop(defender, False))
-
-        is_hit, quality, txt = rules.dice.opposed_saving_throw(
-            attacker,
-            defender,
-            attack_type=weapon.attack_type,
-            defense_type=attacker.weapon.defense_type,
-            advantage=advantage,
-            disadvantage=disadvantage,
+        super().at_object_creation()
+        # subscribe ourselves to a ticker to repeatedly call the hook
+        # "update_weather" on this object. The interval is randomized
+        # so as to not have all weather rooms update at the same time.
+        self.db.interval = random.randint(50, 70)
+        TICKER_HANDLER.add(
+            interval=self.db.interval, callback=self.update_weather, idstring="tutorial"
         )
-        self.msg(f"$You() $conj(attack) $You({defender.key}) with {weapon.key}: {txt}")
-        if is_hit:
-            # enemy hit, calculate damage
-            weapon_dmg_roll = attacker.weapon.damage_roll
-
-            dmg = rules.dice.roll(weapon_dmg_roll)
-
-            if quality is Ability.CRITICAL_SUCCESS:
-                dmg += rules.dice.roll(weapon_dmg_roll)
-                message = (
-                    f" $You() |ycritically|n $conj(hit) $You({defender.key}) for |r{dmg}|n damage!"
-                )
-            else:
-                message = f" $You() $conj(hit) $You({defender.key}) for |r{dmg}|n damage!"
-            self.msg(message)
+        # this is parsed by the 'tutorial' command on TutorialRooms.
+        self.db.tutorial_info = "This room has a Script running that has it echo a weather-related message at irregular intervals."
 
-            # call hook
-            defender.at_damage(dmg, attacker=attacker)
+    def update_weather(self, *args, **kwargs):
+        """
+        Called by the tickerhandler at regular intervals. Even so, we
+        only update 20% of the time, picking a random weather message
+        when we do. The tickerhandler requires that this hook accepts
+        any arguments and keyword arguments (hence the *args, **kwargs
+        even though we don't actually use them in this example)
+        """
+        if random.random() < 0.2:
+            # only update 20 % of the time
+            self.msg_contents("|w%s|n" % random.choice(WEATHER_STRINGS))
 
-            # note that we mustn't remove anyone from combat yet, because this is
-            # happening simultaneously. So checking of the final hp
-            # and rolling of death etc happens in the combathandler at the end of the turn.
 
-        else:
-            # a miss
-            message = f" $You() $conj(miss) $You({defender.key})."
-            if quality is Ability.CRITICAL_FAILURE:
-                attacker.weapon.quality -= 1
-                message += ".. it's a |rcritical miss!|n, damaging the weapon."
-            self.msg(message)
-
-
-class CombatActionStunt(CombatAction):
-    """
-    Perform a stunt. A stunt grants an advantage to yours or another player for their next
-    action, or a disadvantage to yours or an enemy's next action.
-
-    Note that while the check happens between the user and a target, another (the 'beneficiary'
-    could still gain the effect. This allows for boosting allies or making them better
-    defend against an enemy.
-
-    Note: We only count a use if the stunt is successful; they will still spend their turn, but
-    won't spend a use unless they succeed.
-
-    """
+SUPERUSER_WARNING = (
+    "\nWARNING: You are playing as a superuser ({name}). Use the {quell} command to\n"
+    "play without superuser privileges (many functions and puzzles ignore the \n"
+    "presence of a superuser, making this mode useful for exploring things behind \n"
+    "the scenes later).\n"
+)
 
-    key = "Perform a Stunt"
-    desc = "Make [S]tunt against <target>"
-    aliases = ("s", "stunt")
-    help_text = (
-        "A stunt does not cause damage but grants/gives advantage/disadvantage to future "
-        "actions. The effect needs to be used up within 5 turns."
-    )
-    next_menu_node = "node_select_enemy_target"
-
-    give_advantage = True  # if False, give_disadvantage
-    max_uses = 1
-    priority = -1
-    attack_type = Ability.DEX
-    defense_type = Ability.DEX
-    help_text = (
-        "Perform a stunt against a target. This will give you an advantage or an enemy "
-        "disadvantage on your next action."
-    )
-
-    def use(self, defender, *args, **kwargs):
-        # quality doesn't matter for stunts, they are either successful or not
-
-        attacker = self.combatant
-        advantage, disadvantage = False, False
-
-        is_success, _, txt = rules.dice.opposed_saving_throw(
-            attacker,
-            defender,
-            attack_type=self.attack_type,
-            defense_type=self.defense_type,
-            advantage=advantage,
-            disadvantage=disadvantage,
-        )
-        self.msg(f"$You() $conj(attempt) stunt on $You(defender.key). {txt}")
-        if is_success:
-            stunt_duration = self.combathandler.stunt_duration
-            if self.give_advantage:
-                self.combathandler.gain_advantage(attacker, defender)
-                self.msg(
-                    "%You() $conj(gain) advantage against $You(defender.key! "
-                    f"You must use it within {stunt_duration} turns."
-                )
-            else:
-                self.combathandler.gain_disadvantage(defender, attacker)
-                self.msg(
-                    f"$You({defender.key}) $conj(suffer) disadvantage against $You(). "
-                    "Lasts next attack, or until 3 turns passed."
-                )
+# ------------------------------------------------------------
+#
+# Intro Room - unique room
+#
+# This room marks the start of the tutorial. It sets up properties on
+# the player char that is needed for the tutorial.
+#
+# -------------------------------------------------------------
 
-            # only spend a use after being successful
-            self.uses += 1
 
-
-class CombatActionUseItem(CombatAction):
+class CmdEvenniaIntro(Command):
     """
-    Use an item in combat. This is meant for one-off or limited-use items, like potions, scrolls or
-    wands.  We offload the usage checks and usability to the item's own hooks. It's generated
-    dynamically from the items in the character's inventory (you could also consider using items in
-    the room this way).
-
-    Each usable item results in one possible action.
+    Start the Evennia intro wizard.
 
-    It relies on the combat_* hooks on the item:
-        combat_get_help
-        combat_can_use
-        combat_pre_use
-        combat_pre
-        combat_post_use
+    Usage:
+        intro
 
     """
 
-    key = "Use Item"
-    desc = "[U]se item"
-    aliases = ("u", "item", "use item")
-    help_text = "Use an item from your inventory."
-    next_menu_node = "node_select_friendly_target"
+    key = "intro"
 
-    def get_help(self, item, *args):
-        return item.get_help(*args)
+    def func(self):
+        from .intro_menu import init_menu
 
-    def use(self, item, target, *args, **kwargs):
-        item.at_use(self.combatant, target, *args, **kwargs)
+        # quell also superusers
+        if self.caller.account:
+            self.caller.msg("Auto-quelling permissions while in intro ...")
+            self.caller.account.execute_cmd("quell")
+        init_menu(self.caller)
 
-    def post_use(self, item, *args, **kwargs):
-        item.at_post_use(self.combatant, *args, **kwargs)
-        self.msg("$You() $conj(use) an item.")
 
+class CmdSetEvenniaIntro(CmdSet):
+    key = "Evennia Intro StartSet"
 
-class CombatActionSwapWieldedWeaponOrSpell(CombatAction):
-    """
-    Swap Wielded weapon or spell.
-
-    """
+    def at_cmdset_creation(self):
+        self.add(CmdEvenniaIntro())
 
-    key = "Swap weapon/rune/shield"
-    desc = "Swap currently wielded weapon, shield or spell-rune."
-    aliases = (
-        "s",
-        "swap",
-        "draw",
-        "swap weapon",
-        "draw weapon",
-        "swap rune",
-        "draw rune",
-        "swap spell",
-        "draw spell",
-    )
-    help_text = (
-        "Draw a new weapon or spell-rune from your inventory, replacing your current loadout"
-    )
 
-    next_menu_node = "node_select_wield_from_inventory"
-
-    def use(self, _, item, *args, **kwargs):
-        # this will make use of the item
-        self.combatant.equipment.move(item)
-
-
-class CombatActionFlee(CombatAction):
+class IntroRoom(TutorialRoom):
     """
-    Fleeing/disengaging from combat means doing nothing but 'running away' for two turn. Unless
-    someone attempts and succeeds in their 'block' action, you will leave combat by fleeing at the
-    end of the second turn.
+    Intro room
 
+    properties to customize:
+     char_health - integer > 0 (default 20)
     """
 
-    key = "Flee/Disengage"
-    desc = "[F]lee/disengage from combat (takes two turns)"
-    aliases = ("d", "disengage", "flee")
-
-    # this only affects us
-    next_menu_node = "node_confirm_register_action"
-
-    help_text = (
-        "Disengage from combat. Use successfully two times in a row to leave combat at the "
-        "end of the second round. If someone Blocks you successfully, this counter is reset."
-    )
-    priority = -5  # checked last
-
-    def use(self, *args, **kwargs):
-        # it's safe to do this twice
-        self.msg(
-            "$You() $conj(retreat), and will leave combat next round unless someone successfully "
-            "blocks the escape."
+    def at_object_creation(self):
+        """
+        Called when the room is first created.
+        """
+        super().at_object_creation()
+        self.db.tutorial_info = (
+            "The first room of the tutorial. "
+            "This assigns the health Attribute to "
+            "the account."
         )
-        self.combathandler.flee(self.combatant)
-
-
-class CombatActionBlock(CombatAction):
-
-    """
-    Blocking is, in this context, a way to counter an enemy's 'Flee/Disengage' action.
-
-    """
 
-    key = "Block"
-    desc = "[B]lock <target> from fleeing"
-    aliases = ("b", "block", "chase")
-    help_text = (
-        "Move to block a target from fleeing combat. If you succeed "
-        "in a DEX vs DEX challenge, they don't get away."
-    )
-    next_menu_node = "node_select_enemy_target"
-
-    priority = -1  # must be checked BEFORE the flee action of the target!
-
-    attack_type = Ability.DEX
-    defense_type = Ability.DEX
-
-    def use(self, fleeing_target, *args, **kwargs):
+    def at_object_receive(self, character, source_location, move_type="move", **kwargs):
+        """
+        Assign properties on characters
+        """
 
-        advantage = bool(
-            self.combathandler.advantage_matrix[self.combatant].pop(fleeing_target, False)
-        )
-        disadvantage = bool(
-            self.combathandler.disadvantage_matrix[self.combatant].pop(fleeing_target, False)
-        )
+        # setup character for the tutorial
+        health = self.db.char_health or 20
 
-        is_success, _, txt = rules.dice.opposed_saving_throw(
-            self.combatant,
-            fleeing_target,
-            attack_type=self.attack_type,
-            defense_type=self.defense_type,
-            advantage=advantage,
-            disadvantage=disadvantage,
-        )
-        self.msg(
-            f"$You() $conj(try) to block the retreat of $You({fleeing_target.key}). {txt}",
-        )
+        if character.has_account:
+            character.db.health = health
+            character.db.health_max = health
 
-        if is_success:
-            # managed to stop the target from fleeing/disengaging
-            self.combathandler.unflee(fleeing_target)
-            self.msg(f"$You() $conj(block) the retreat of $You({fleeing_target.key})")
+        if character.is_superuser:
+            string = "-" * 78 + SUPERUSER_WARNING + "-" * 78
+            character.msg("|r%s|n" % string.format(name=character.key, quell="|wquell|r"))
         else:
-            self.msg(f"$You({fleeing_target.key}) $conj(dodge) away from you $You()!")
-
-
-class CombatActionDoNothing(CombatAction):
-    """
-    Do nothing this turn.
+            # quell user
+            if character.account:
+                character.account.execute_cmd("quell")
+                character.msg("(Auto-quelling while in tutorial-world)")
+
+
+# -------------------------------------------------------------
+#
+# Bridge - unique room
+#
+# Defines a special west-eastward "bridge"-room, a large room that takes
+# several steps to cross. It is complete with custom commands and a
+# chance of falling off the bridge. This room has no regular exits,
+# instead the exitings are handled by custom commands set on the account
+# upon first entering the room.
+#
+# Since one can enter the bridge room from both ends, it is
+# divided into five steps:
+#       westroom <- 0 1 2 3 4 -> eastroom
+#
+# -------------------------------------------------------------
+
+
+class CmdEast(Command):
+    """
+    Go eastwards across the bridge.
+
+    Tutorial info:
+        This command relies on the caller having two Attributes
+        (assigned by the room when entering):
+            - east_exit: a unique name or dbref to the room to go to
+              when exiting east.
+            - west_exit: a unique name or dbref to the room to go to
+              when exiting west.
+       The room must also have the following Attributes
+           - tutorial_bridge_posistion: the current position on
+             on the bridge, 0 - 4.
 
     """
 
-    key = "Hesitate"
-    desc = "Do [N]othing/Hesitate"
-    aliases = ("n", "hesitate", "nothing", "do nothing")
-    help_text = "Hold you position, doing nothing."
-
-    # affects noone else
-    next_menu_node = "node_confirm_register_action"
-
-    post_action_text = "{combatant} does nothing this turn."
-
-    def use(self, *args, **kwargs):
-        self.msg("$You() $conj(hesitate), accomplishing nothing.")
-
-
-# -----------------------------------------------------------------------------------
-#  Combat handler
-# -----------------------------------------------------------------------------------
+    key = "east"
+    aliases = ["e"]
+    locks = "cmd:all()"
+    help_category = "TutorialWorld"
+
+    def func(self):
+        """move one step eastwards"""
+        caller = self.caller
+
+        bridge_step = min(5, caller.db.tutorial_bridge_position + 1)
+
+        if bridge_step > 4:
+            # we have reached the far east end of the bridge.
+            # Move to the east room.
+            eexit = search_object(self.obj.db.east_exit)
+            if eexit:
+                caller.move_to(eexit[0], move_type="traverse")
+            else:
+                caller.msg("No east exit was found for this room. Contact an admin.")
+            return
+        caller.db.tutorial_bridge_position = bridge_step
+        # since we are really in one room, we have to notify others
+        # in the room when we move.
+        caller.location.msg_contents(
+            "%s steps eastwards across the bridge." % caller.name, exclude=caller
+        )
+        caller.execute_cmd("look")
 
 
-class EvAdventureCombatHandler(DefaultScript):
+# go back across the bridge
+class CmdWest(Command):
     """
-    This script is created when combat is initialized and stores a queue
-    of all active participants.
+    Go westwards across the bridge.
 
-    It's also possible to join (or leave) the fray later.
+    Tutorial info:
+       This command relies on the caller having two Attributes
+       (assigned by the room when entering):
+           - east_exit: a unique name or dbref to the room to go to
+             when exiting east.
+           - west_exit: a unique name or dbref to the room to go to
+             when exiting west.
+       The room must also have the following property:
+           - tutorial_bridge_posistion: the current position on
+             on the bridge, 0 - 4.
 
     """
 
-    # we use the same duration for all stunts
-    stunt_duration = 3
-
-    # Default actions available to everyone
-    default_action_classes = [
-        CombatActionAttack,
-        CombatActionStunt,
-        CombatActionSwapWieldedWeaponOrSpell,
-        CombatActionUseItem,
-        CombatActionFlee,
-        CombatActionBlock,
-        CombatActionDoNothing,
-    ]
-
-    # attributes
-
-    # stores all combatants active in the combat
-    combatants = AttributeProperty(list())
-    # each combatant has its own set of actions that may or may not be available
-    # every round
-    combatant_actions = AttributeProperty(defaultdict(dict))
-
-    action_queue = AttributeProperty(dict())
-
-    turn_stats = AttributeProperty(dict())
-
-    # turn counter - abstract time
-    turn = AttributeProperty(default=0)
-    # advantages or disadvantages gained against different targets
-    advantage_matrix = AttributeProperty(defaultdict(dict))
-    disadvantage_matrix = AttributeProperty(defaultdict(dict))
-
-    fleeing_combatants = AttributeProperty(list())
-    defeated_combatants = AttributeProperty(list())
-
-    _warn_time_task = None
+    key = "west"
+    aliases = ["w"]
+    locks = "cmd:all()"
+    help_category = "TutorialWorld"
 
-    def at_script_creation(self):
+    def func(self):
+        """move one step westwards"""
+        caller = self.caller
 
-        # how often this script ticks - the max length of each turn (in seconds)
-        self.key = COMBAT_HANDLER_KEY
-        self.interval = COMBAT_HANDLER_INTERVAL
+        bridge_step = max(-1, caller.db.tutorial_bridge_position - 1)
 
-    def at_repeat(self, **kwargs):
-        """
-        Called every self.interval seconds. The main tick of the script.
-
-        """
-        if self._warn_time_task:
-            self._warn_time_task.remove()
-
-        if self.turn == 0:
-            self._start_turn()
-        else:
-            self._end_turn()
-            self._start_turn()
-
-    def _init_menu(self, combatant, session=None):
-        """
-        Make sure combatant is in the menu. This is safe to call on a combatant already in a menu.
-
-        """
-        if not combatant.ndb._evmenu:
-            # re-joining the menu is useful during testing
-            evmenu.EvMenu(
-                combatant,
-                {
-                    "node_wait_start": node_wait_start,
-                    "node_select_enemy_target": node_select_enemy_target,
-                    "node_select_friendly_target": node_select_friendly_target,
-                    "node_select_action": node_select_action,
-                    "node_select_wield_from_inventory": node_select_wield_from_inventory,
-                    "node_wait_turn": node_wait_turn,
-                },
-                startnode="node_wait_turn",
-                auto_quit=True,
-                persistent=True,
-                cmdset_mergetype="Union",
-                session=session,
-                combathandler=self,  # makes this available as combatant.ndb._evmenu.combathandler
-            )
-
-    def _warn_time(self, time_remaining):
-        """
-        Send a warning message when time is about to run out.
-
-        """
-        self.msg(f"{time_remaining} seconds left in round!")
-
-    def _start_turn(self):
-        """
-        New turn events
-
-        """
-        self.turn += 1
-        self.action_queue = {}
-        self.turn_stats = defaultdict(list)
-
-        # start a timer to echo a warning to everyone 15 seconds before end of round
-        if self.interval >= 0:
-            # set -1 for unit tests
-            warning_time = 10
-            self._warn_time_task = delay(
-                self.interval - warning_time, self._warn_time, warning_time
-            )
-
-        self.msg(f"|y_______________________ start turn {self.turn} ___________________________|n")
-
-        for combatant in self.combatants:
-            if hasattr(combatant, "ai_combat_next_action"):
-                # NPC needs to get a decision from the AI
-                next_action_key, args, kwargs = combatant.ai_combat_next_action(self)
-                self.register_action(combatant, next_action_key, *args, **kwargs)
+        if bridge_step < 0:
+            # we have reached the far west end of the bridge.
+            # Move to the west room.
+            wexit = search_object(self.obj.db.west_exit)
+            if wexit:
+                caller.move_to(wexit[0], move_type="traverse")
             else:
-                # cycle combat menu for PC
-                self._init_menu(combatant)
-                combatant.ndb._evmenu.goto("node_select_action", "")
-
-    def _end_turn(self):
-        """
-        End of turn operations.
+                caller.msg("No west exit was found for this room. Contact an admin.")
+            return
+        caller.db.tutorial_bridge_position = bridge_step
+        # since we are really in one room, we have to notify others
+        # in the room when we move.
+        caller.location.msg_contents(
+            "%s steps westwards across the bridge." % caller.name, exclude=caller
+        )
+        caller.execute_cmd("look")
 
-        1. Do all regular actions
-        2. Check if fleeing combatants got away - remove them from combat
-        3. Check if anyone has hp <= - defeated
-        4. Check if any one side is alone on the battlefield - they loot the defeated
-        5. If combat is still on, update stunt timers
 
-        """
-        self.msg(
-            f"|y__________________ turn resolution (turn {self.turn}) ____________________|n\n"
+BRIDGE_POS_MESSAGES = (
+    "You are standing |wvery close to the the bridge's western foundation|n."
+    " If you go west you will be back on solid ground ...",
+    "The bridge slopes precariously where it extends eastwards"
+    " towards the lowest point - the center point of the hang bridge.",
+    "You are |whalfways|n out on the unstable bridge.",
+    "The bridge slopes precariously where it extends westwards"
+    " towards the lowest point - the center point of the hang bridge.",
+    "You are standing |wvery close to the bridge's eastern foundation|n."
+    " If you go east you will be back on solid ground ...",
+)
+BRIDGE_MOODS = (
+    "The bridge sways in the wind.",
+    "The hanging bridge creaks dangerously.",
+    "You clasp the ropes firmly as the bridge sways and creaks under you.",
+    "From the castle you hear a distant howling sound, like that of a large dog or other beast.",
+    "The bridge creaks under your feet. Those planks does not seem very sturdy.",
+    "Far below you the ocean roars and throws its waves against the cliff,"
+    " as if trying its best to reach you.",
+    "Parts of the bridge come loose behind you, falling into the chasm far below!",
+    "A gust of wind causes the bridge to sway precariously.",
+    "Under your feet a plank comes loose, tumbling down. For a moment you dangle over the abyss ...",
+    "The section of rope you hold onto crumble in your hands,"
+    " parts of it breaking apart. You sway trying to regain balance.",
+)
+
+FALL_MESSAGE = (
+    "Suddenly the plank you stand on gives way under your feet! You fall!"
+    "\nYou try to grab hold of an adjoining plank, but all you manage to do is to "
+    "divert your fall westwards, towards the cliff face. This is going to hurt ... "
+    "\n ... The world goes dark ...\n\n"
+)
+
+
+class CmdLookBridge(Command):
+    """
+    looks around at the bridge.
+
+    Tutorial info:
+        This command assumes that the room has an Attribute
+        "fall_exit", a unique name or dbref to the place they end upp
+        if they fall off the bridge.
+    """
+
+    key = "look"
+    aliases = ["l"]
+    locks = "cmd:all()"
+    help_category = "TutorialWorld"
+
+    def func(self):
+        """Looking around, including a chance to fall."""
+        caller = self.caller
+        bridge_position = self.caller.db.tutorial_bridge_position
+        # this command is defined on the room, so we get it through self.obj
+        location = self.obj
+        # randomize the look-echo
+        message = "|c%s|n\n%s\n%s" % (
+            location.key,
+            BRIDGE_POS_MESSAGES[bridge_position],
+            random.choice(BRIDGE_MOODS),
         )
 
-        # store those in the process of fleeing
-        already_fleeing = self.fleeing_combatants[:]
-
-        # do all actions
-        for combatant in self.combatants:
-            # read the current action type selected by the player
-            action, args, kwargs = self.action_queue.get(
-                combatant, (CombatActionDoNothing(self, combatant), (), {})
-            )
-            # perform the action on the CombatAction instance
-            try:
-                action.pre_use(*args, **kwargs)
-                action.use(*args, **kwargs)
-                action.post_use(*args, **kwargs)
-            except Exception as err:
-                combatant.msg(
-                    f"An error ({err}) occurred when performing this action.\n"
-                    "Please report the problem to an admin."
+        chars = [obj for obj in self.obj.contents_get(exclude=caller) if obj.has_account]
+        if chars:
+            # we create the You see: message manually here
+            message += "\n You see: %s" % ", ".join("|c%s|n" % char.key for char in chars)
+        self.caller.msg(message)
+
+        # there is a chance that we fall if we are on the western or central
+        # part of the bridge.
+        if bridge_position < 3 and random.random() < 0.05 and not self.caller.is_superuser:
+            # we fall 5% of time.
+            fall_exit = search_object(self.obj.db.fall_exit)
+            if fall_exit:
+                self.caller.msg("|r%s|n" % FALL_MESSAGE)
+                self.caller.move_to(fall_exit[0], quiet=True, move_type="fall")
+                # inform others on the bridge
+                self.obj.msg_contents(
+                    "A plank gives way under %s's feet and "
+                    "they fall from the bridge!" % self.caller.key
                 )
-                logger.log_trace()
-                raise
 
-        # handle disengaging combatants
 
-        to_flee = []
-        to_defeat = []
+# custom help command
+class CmdBridgeHelp(Command):
+    """
+    Overwritten help command while on the bridge.
+    """
 
-        for combatant in self.combatants:
-            # see if fleeing characters managed to do two flee actions in a row.
-            if (combatant in self.fleeing_combatants) and (combatant in already_fleeing):
-                self.fleeing_combatants.remove(combatant)
-                to_flee.append(combatant)
-
-            if combatant.hp <= 0:
-                # check characters that are beaten down.
-                # characters roll on the death table here; but even if they survive, they
-                # count as defeated (unconcious) for this combat.
-                combatant.at_defeat()
-                to_defeat.append(combatant)
-
-        for combatant in to_flee:
-            # combatant leaving combat by fleeing
-            self.msg("|y$You() successfully $conj(flee) from combat.|n", combatant=combatant)
-            self.remove_combatant(combatant)
-
-        for combatant in to_defeat:
-            # combatants leaving combat by being defeated
-            self.msg("|r$You() $conj(fall) to the ground, defeated.|n", combatant=combatant)
-            self.combatants.remove(combatant)
-            self.defeated_combatants.append(combatant)
-
-        # check if only one side remains, divide into allies and enemies based on the first
-        # combatant,then check if either team is empty.
-        if not self.combatants:
-            # everyone's defeated at the same time. This is a tie where everyone loses and
-            # no looting happens.
-            self.msg("|yEveryone takes everyone else out. Today, noone wins.|n")
-            self.stop_combat()
-            return
-        else:
-            combatant = self.combatants[0]
-            allies = self.get_friendly_targets(combatant)  # will always contain at least combatant
-            enemies = self.get_enemy_targets(combatant)
-
-            if not enemies:
-                # no enemies left - allies to combatant won!
-                defeated_enemies = self.get_enemy_targets(
-                    combatant, all_combatants=self.defeated_combatants
-                )
+    key = "help"
+    aliases = ["h", "?"]
+    locks = "cmd:all()"
+    help_category = "Tutorial world"
+
+    def func(self):
+        """Implements the command."""
+        string = (
+            "You are trying hard not to fall off the bridge ..."
+            "\n\nWhat you can do is trying to cross the bridge |weast|n"
+            " or try to get back to the mainland |wwest|n)."
+        )
+        self.caller.msg(string)
 
-                # all surviving allies loot the fallen enemies
-                for ally in allies:
-                    for enemy in defeated_enemies:
-                        try:
-                            if ally.pre_loot(enemy):
-                                enemy.at_looted(ally)
-                                ally.post_loot(enemy)
-                        except Exception:
-                            logger.log_trace()
-                self.stop_combat()
-                return
 
-        # if we get here, combat is still on
+class BridgeCmdSet(CmdSet):
+    """This groups the bridge commands. We will store it on the room."""
 
-        # refresh stunt timeouts (note - self.stunt_duration is the same for
-        # all stunts; # for more complex use we could store the action and let action have a
-        # 'duration' property to use instead.
-        oldest_stunt_age = self.turn - self.stunt_duration
-
-        advantage_matrix = self.advantage_matrix
-        disadvantage_matrix = self.disadvantage_matrix
-        # rebuild advantages with the (possibly cropped) list of combatants
-        # we make new matrices in order to make sure disengaged combatants are
-        # not included.
-        new_advantage_matrix = {}
-        new_disadvantage_matrix = {}
-
-        for combatant in self.combatants:
-            new_advantage_matrix[combatant] = {
-                target: set_at_turn
-                for target, set_at_turn in advantage_matrix[combatant].items()
-                if set_at_turn > oldest_stunt_age
-            }
-            new_disadvantage_matrix[combatant] = {
-                target: set_at_turn
-                for target, set_at_turn in disadvantage_matrix[combatant].items()
-                if set_at_turn > oldest_stunt_age
-            }
+    key = "Bridge commands"
+    priority = 2  # this gives it precedence over the normal look/help commands.
 
-        self.advantage_matrix = new_advantage_matrix
-        self.disadvantage_matrix = new_disadvantage_matrix
+    def at_cmdset_creation(self):
+        """Called at first cmdset creation"""
+        self.add(CmdTutorial())
+        self.add(CmdEast())
+        self.add(CmdWest())
+        self.add(CmdLookBridge())
+        self.add(CmdBridgeHelp())
+
+
+BRIDGE_WEATHER = (
+    "The rain intensifies, making the planks of the bridge even more slippery.",
+    "A gust of wind throws the rain right in your face.",
+    "The rainfall eases a bit and the sky momentarily brightens.",
+    "The bridge shakes under the thunder of a closeby thunder strike.",
+    "The rain pummels you with large, heavy drops. You hear the distinct howl of a large hound in the distance.",
+    "The wind is picking up, howling around you and causing the bridge to sway from side to side.",
+    "Some sort of large bird sweeps by overhead, giving off an eery screech. Soon it has disappeared in the gloom.",
+    "The bridge sways from side to side in the wind.",
+    "Below you a particularly large wave crashes into the rocks.",
+    "From the ruin you hear a distant, otherwordly howl. Or maybe it was just the wind.",
+)
+
+
+class BridgeRoom(WeatherRoom):
+    """
+    The bridge room implements an unsafe bridge. It also enters the player into
+    a state where they get new commands so as to try to cross the bridge.
+
+     We want this to result in the account getting a special set of
+     commands related to crossing the bridge. The result is that it
+     will take several steps to cross it, despite it being represented
+     by only a single room.
+
+     We divide the bridge into steps:
+
+        self.db.west_exit     -   -  |  -   -     self.db.east_exit
+                              0   1  2  3   4
+
+     The position is handled by a variable stored on the character
+     when entering and giving special move commands will
+     increase/decrease the counter until the bridge is crossed.
+
+     We also has self.db.fall_exit, which points to a gathering
+     location to end up if we happen to fall off the bridge (used by
+     the CmdLookBridge command).
+
+    """
+
+    def at_object_creation(self):
+        """Setups the room"""
+        # this will start the weather room's ticker and tell
+        # it to call update_weather regularly.
+        super().at_object_creation()
+        # this identifies the exits from the room (should be the command
+        # needed to leave through that exit). These are defaults, but you
+        # could of course also change them after the room has been created.
+        self.db.west_exit = "cliff"
+        self.db.east_exit = "gate"
+        self.db.fall_exit = "cliffledge"
+        # add the cmdset on the room.
+        self.cmdset.add(BridgeCmdSet, persistent=True)
+        # since the default Character's at_look() will access the room's
+        # return_description (this skips the cmdset) when
+        # first entering it, we need to explicitly turn off the room
+        # as a normal view target - once inside, our own look will
+        # handle all return messages.
+        self.locks.add("view:false()")
+
+    def update_weather(self, *args, **kwargs):
+        """
+        This is called at irregular intervals and makes the passage
+        over the bridge a little more interesting.
+        """
+        if random.random() < 80:
+            # send a message most of the time
+            self.msg_contents("|w%s|n" % random.choice(BRIDGE_WEATHER))
+
+    def at_object_receive(self, character, source_location, move_type="move", **kwargs):
+        """
+        This hook is called by the engine whenever the player is moved
+        into this room.
+        """
+        if character.has_account:
+            # we only run this if the entered object is indeed a player object.
+            # check so our east/west exits are correctly defined.
+            wexit = search_object(self.db.west_exit)
+            eexit = search_object(self.db.east_exit)
+            fexit = search_object(self.db.fall_exit)
+            if not (wexit and eexit and fexit):
+                character.msg(
+                    "The bridge's exits are not properly configured. "
+                    "Contact an admin. Forcing west-end placement."
+                )
+                character.db.tutorial_bridge_position = 0
+                return
+            if source_location == eexit[0]:
+                # we assume we enter from the same room we will exit to
+                character.db.tutorial_bridge_position = 4
+            else:
+                # if not from the east, then from the west!
+                character.db.tutorial_bridge_position = 0
+            character.execute_cmd("look")
 
-    def add_combatant(self, combatant, session=None):
+    def at_object_leave(self, character, target_location, move_type="move", **kwargs):
         """
-        Add combatant to battle.
-
-        Args:
-            combatant (Object): The combatant to add.
-            session (Session, optional): Session to use.
+        This is triggered when the player leaves the bridge room.
+        """
+        if character.has_account:
+            # clean up the position attribute
+            del character.db.tutorial_bridge_position
 
-        Notes:
-            This adds them to the internal list and initiates
-            all possible actions. If the combatant as an Attribute list
-            `custom_combat_actions` containing `CombatAction` items, this
-            will injected and if the `.key` matches, will replace the
-            default action classes.
 
-        """
-        if combatant not in self.combatants:
-            self.combatants.append(combatant)
-            combatant.db.combathandler = self
+# -------------------------------------------------------------------------------
+#
+# Dark Room - a room with states
+#
+# This room limits the movemenets of its denizens unless they carry an active
+# LightSource object (LightSource is defined in
+#                     tutorialworld.objects.LightSource)
+#
+# -------------------------------------------------------------------------------
 
-            # allow custom character actions (not used by default)
-            custom_action_classes = combatant.db.custom_combat_actions or []
 
-            self.combatant_actions[combatant] = {
-                action_class.key: action_class(self, combatant)
-                for action_class in self.default_action_classes + custom_action_classes
-            }
-            self._init_menu(combatant, session=session)
+DARK_MESSAGES = (
+    "It is pitch black. You are likely to be eaten by a grue.",
+    "It's pitch black. You fumble around but cannot find anything.",
+    "You don't see a thing. You feel around, managing to bump your fingers hard against something. Ouch!",
+    "You don't see a thing! Blindly grasping the air around you, you find nothing.",
+    "It's totally dark here. You almost stumble over some un-evenness in the ground.",
+    "You are completely blind. For a moment you think you hear someone breathing nearby ... "
+    "\n ... surely you must be mistaken.",
+    "Blind, you think you find some sort of object on the ground, but it turns out to be just a stone.",
+    "Blind, you bump into a wall. The wall seems to be covered with some sort of vegetation,"
+    " but its too damp to burn.",
+    "You can't see anything, but the air is damp. It feels like you are far underground.",
+)
 
-    def remove_combatant(self, combatant):
-        """
-        Remove combatant from battle.
+ALREADY_LIGHTSOURCE = (
+    "You don't want to stumble around in blindness anymore. You already "
+    "found what you need. Let's get light already!"
+)
 
-        Args:
-            combatant (Object): The combatant to remove.
+FOUND_LIGHTSOURCE = (
+    "Your fingers bump against a splinter of wood in a corner."
+    " It smells of resin and seems dry enough to burn! "
+    "You pick it up, holding it firmly. Now you just need to"
+    " |wlight|n it using the flint and steel you carry with you."
+)
 
-        """
-        if combatant in self.combatants:
-            self.combatants.remove(combatant)
-            self.combatant_actions.pop(combatant, None)
-            if combatant.ndb._evmenu:
-                combatant.ndb._evmenu.close_menu()
-            del combatant.db.combathandler
 
-    def start_combat(self):
-        """
-        Start the combat timer and get everyone going.
+class CmdLookDark(Command):
+    """
+    Look around in darkness
 
-        """
-        for combatant in self.combatants:
-            combatant.ndb._evmenu.goto("node_select_action", "")
-        self.start()  # starts the script timer
-        self._start_turn()
+    Usage:
+      look
 
-    def stop_combat(self):
-        """
-        This is used to stop the combat immediately.
+    Look around in the darkness, trying
+    to find something.
+    """
 
-        It can also be called from external systems, for example by
-        monster AI can do this when only allied players remain.
+    key = "look"
+    aliases = ["l", "feel", "search", "feel around", "fiddle"]
+    locks = "cmd:all()"
+    help_category = "TutorialWorld"
 
+    def func(self):
         """
-        for combatant in self.combatants:
-            self.remove_combatant(combatant)
-        self.delete()
+        Implement the command.
 
-    def get_enemy_targets(self, combatant, excluded=None, all_combatants=None):
+        This works both as a look and a search command; there is a
+        random chance of eventually finding a light source.
         """
-        Get all valid targets the given combatant can target for an attack. This does not apply for
-        'friendly' targeting (like wanting to cast a heal on someone). We assume there are two types
-        of combatants - PCs (player-controlled characters and NPCs (AI-controlled). Here, we assume
-        npcs can never attack one another (or themselves)
+        caller = self.caller
 
-        For PCs to be able to target each other, the `allow_pvp`
-        Attribute flag must be set on the current `Room`.
+        # count how many searches we've done
+        nr_searches = caller.ndb.dark_searches
+        if nr_searches is None:
+            nr_searches = 0
+            caller.ndb.dark_searches = nr_searches
 
-        Args:
-            combatant (Object): The combatant looking for targets.
-            excluded (list, optional): If given, these are not valid targets - this can be used to
-                avoid friendly NPCs.
-            all_combatants (list, optional): If given, use this list to get all combatants, instead
-                of using `self.combatants`.
-
-        """
-        is_pc = not inherits_from(combatant, EvAdventureNPC)
-        allow_pvp = self.obj.allow_pvp
-        targets = []
-        combatants = all_combatants or self.combatants
-
-        if is_pc:
-            if allow_pvp:
-                # PCs may target everyone, including other PCs
-                targets = combatants
+        if nr_searches < 4 and random.random() < 0.90:
+            # we don't find anything
+            caller.msg(random.choice(DARK_MESSAGES))
+            caller.ndb.dark_searches += 1
+        else:
+            # we could have found something!
+            if any(obj for obj in caller.contents if utils.inherits_from(obj, LightSource)):
+                #  we already carry a LightSource object.
+                caller.msg(ALREADY_LIGHTSOURCE)
             else:
-                # PCs may only attack NPCs
-                targets = [target for target in combatants if inherits_from(target, EvAdventureNPC)]
+                # don't have a light source, create a new one.
+                create_object(LightSource, key="splinter", location=caller)
+                caller.msg(FOUND_LIGHTSOURCE)
 
-        else:
-            # NPCs may only attack PCs, not each other
-            targets = [target for target in combatants if not inherits_from(target, EvAdventureNPC)]
 
-        if excluded:
-            targets = [target for target in targets if target not in excluded]
+class CmdDarkHelp(Command):
+    """
+    Help command for the dark state.
+    """
 
-        return targets
+    key = "help"
+    locks = "cmd:all()"
+    help_category = "TutorialWorld"
 
-    def get_friendly_targets(self, combatant, extra=None, all_combatants=None):
+    def func(self):
         """
-        Get a list of all 'friendly' or neutral targets a combatant may target, including
-        themselves.
-
-        Args:
-            combatant (Object): The combatant looking for targets.
-            extra (list, optional): If given, these are additional targets that can be
-                considered target for allied effects (could be used for a friendly NPC).
-            all_combatants (list, optional): If given, use this list to get all combatants, instead
-                of using `self.combatants`.
-
+        Replace the the help command with a not-so-useful help
         """
-        is_pc = not inherits_from(combatant, EvAdventureNPC)
-        combatants = all_combatants or self.combatants
-        if is_pc:
-            # can target other PCs
-            targets = [target for target in combatants if not inherits_from(target, EvAdventureNPC)]
-        else:
-            # can target other NPCs
-            targets = [target for target in combatants if inherits_from(target, EvAdventureNPC)]
-
-        if extra:
-            targets = list(set(targets + extra))
-
-        return targets
+        string = (
+            "Can't help you until you find some light! Try looking/feeling around for something to burn. "
+            "You shouldn't give up even if you don't find anything right away."
+        )
+        self.caller.msg(string)
 
-    def get_combat_summary(self, combatant):
-        """
-        Get a summary of the current combat state from the perspective of a
-        given combatant.
 
-        Args:
-            combatant (Object): The combatant to get the summary for
+class CmdDarkNoMatch(Command):
+    """
+    This is a system command. Commands with special keys are used to
+    override special sitations in the game. The CMD_NOMATCH is used
+    when the given command is not found in the current command set (it
+    replaces Evennia's default behavior or offering command
+    suggestions)
+    """
 
-        Returns:
-            str: The summary.
+    key = syscmdkeys.CMD_NOMATCH
+    locks = "cmd:all()"
 
-        Example:
+    def func(self):
+        """Implements the command."""
+        self.caller.msg(
+            "Until you find some light, there's not much you can do. "
+            "Try feeling around, maybe you'll find something helpful!"
+        )
 
-            ```
-            You (5/10 health)
-            Foo (Hurt) [Running away - use 'block' to stop them!]
-            Bar (Perfect health)
 
-            ```
+class DarkCmdSet(CmdSet):
+    """
+    Groups the commands of the dark room together.  We also import the
+    default say command here so that players can still talk in the
+    darkness.
 
-        """
-        table = evtable.EvTable(border_width=0)
+    We give the cmdset the mergetype "Replace" to make sure it
+    completely replaces whichever command set it is merged onto
+    (usually the default cmdset)
+    """
 
-        # 'You' display
-        fleeing = ""
-        if combatant in self.fleeing_combatants:
-            fleeing = " You are running away! Use 'flee' again next turn."
+    key = "darkroom_cmdset"
+    mergetype = "Replace"
+    priority = 2
 
-        table.add_row(f"You ({combatant.hp} / {combatant.hp_max} health){fleeing}")
+    def at_cmdset_creation(self):
+        """populate the cmdset."""
+        self.add(CmdTutorial())
+        self.add(CmdLookDark())
+        self.add(CmdDarkHelp())
+        self.add(CmdDarkNoMatch())
+        self.add(default_cmds.CmdSay())
+        self.add(default_cmds.CmdQuit())
+        self.add(default_cmds.CmdHome())
 
-        for comb in self.combatants:
 
-            if comb is combatant:
-                continue
+class DarkRoom(TutorialRoom):
+    """
+    A dark room. This tries to start the DarkState script on all
+    objects entering. The script is responsible for making sure it is
+    valid (that is, that there is no light source shining in the room).
 
-            name = comb.key
-            health = f"{comb.hurt_level}"
-            fleeing = ""
-            if comb in self.fleeing_combatants:
-                fleeing = " [Running away! Use 'block' to stop them!"
+    The is_lit Attribute is used to define if the room is currently lit
+    or not, so as to properly echo state changes.
 
-            table.add_row(f"{name} ({health}){fleeing}")
+    Since this room (in the tutorial) is meant as a sort of catch-all,
+    we also make sure to heal characters ending up here, since they
+    may have been beaten up by the ghostly apparition at this point.
 
-        return str(table)
+    """
 
-    def msg(self, message, combatant=None, broadcast=True):
+    def at_object_creation(self):
         """
-        Central place for sending messages to combatants. This allows
-        for adding any combat-specific text-decoration in one place.
-
-        Args:
-            message (str): The message to send.
-            combatant (Object): The 'You' in the message, if any.
-            broadcast (bool): If `False`, `combatant` must be included and
-                will be the only one to see the message. If `True`, send to
-                everyone in the location.
-
-        Notes:
-            If `combatant` is given, use `$You/you()` markup to create
-            a message that looks different depending on who sees it. Use
-            `$You(combatant_key)` to refer to other combatants.
-
+        Called when object is first created.
         """
-        location = self.obj
-        location_objs = location.contents
+        super().at_object_creation()
+        self.db.tutorial_info = "This is a room with custom command sets on itself."
+        # the room starts dark.
+        self.db.is_lit = False
+        self.cmdset.add(DarkCmdSet, persistent=True)
 
-        exclude = []
-        if not broadcast and combatant:
-            exclude = [obj for obj in location_objs if obj is not combatant]
-
-        location.msg_contents(
-            message,
-            exclude=exclude,
-            from_obj=combatant,
-            mapping={locobj.key: locobj for locobj in location_objs},
-        )
-
-    def gain_advantage(self, combatant, target):
+    def at_init(self):
         """
-        Gain advantage against target. Spent by actions.
-
+        Called when room is first recached (such as after a reload)
         """
-        self.advantage_matrix[combatant][target] = self.turn
+        self.check_light_state()
 
-    def gain_disadvantage(self, combatant, target):
+    def _carries_light(self, obj):
         """
-        Gain disadvantage against target. Spent by actions.
+        Checks if the given object carries anything that gives light.
 
+        Note that we do NOT look for a specific LightSource typeclass,
+        but for the Attribute is_giving_light - this makes it easy to
+        later add other types of light-giving items. We also accept
+        if there is a light-giving object in the room overall (like if
+        a splinter was dropped in the room)
         """
-        self.disadvantage_matrix[combatant][target] = self.turn
-
-    def flee(self, combatant):
-        if combatant not in self.fleeing_combatants:
-            self.fleeing_combatants.append(combatant)
-
-    def unflee(self, combatant):
-        if combatant in self.fleeing_combatants:
-            self.fleeing_combatants.remove(combatant)
+        return (
+            obj.is_superuser
+            or obj.db.is_giving_light
+            or any(o for o in obj.contents if o.db.is_giving_light)
+        )
 
-    def register_action(self, combatant, action_key, *args, **kwargs):
+    def _heal(self, character):
         """
-        Register an action based on its `.key`.
-
-        Args:
-            combatant (Object): The one performing the action.
-            action_key (str): The action to perform, by its `.key`.
-            *args: Arguments to pass to `action.use`.
-            **kwargs: Kwargs to pass to `action.use`.
-
+        Heal a character.
         """
-        # get the instantiated action for this combatant
-        action = self.combatant_actions[combatant].get(
-            action_key, CombatActionDoNothing(self, combatant)
-        )
+        health = character.db.health_max or 20
+        character.db.health = health
 
-        # store the action in the queue
-        self.action_queue[combatant] = (action, args, kwargs)
-
-        if len(self.action_queue) >= len(self.combatants):
-            # all combatants registered actions - force the script
-            # to cycle (will fire at_repeat)
-            self.force_repeat()
-
-    def get_available_actions(self, combatant, *args, **kwargs):
+    def check_light_state(self, exclude=None):
         """
-        Get only the actions available to a combatant.
+        This method checks if there are any light sources in the room.
+        If there isn't it makes sure to add the dark cmdset to all
+        characters in the room. It is called whenever characters enter
+        the room and also by the Light sources when they turn on.
 
         Args:
-            combatant (Object): The combatant to get actions for.
-            *args: Passed to `action.can_use()`
-            **kwargs: Passed to `action.can_use()`
-
-        Returns:
-            list: The initiated CombatAction instances available to the
-                combatant right now.
-
-        Note:
-            We could filter this by `.can_use` return already here, but then it would just
-            be removed from the menu. Instead we return all and use `.can_use` in the menu
-            so we can include the option but gray it out.
-
+            exclude (Object): An object to not include in the light check.
         """
-        return list(self.combatant_actions[combatant].values())
-
-
-# -----------------------------------------------------------------------------------
-#  Combat Menu definitions
-# -----------------------------------------------------------------------------------
-
-
-def _register_action(caller, raw_string, **kwargs):
-    """
-    Actually register action with handler.
-
-    """
-    action_key = kwargs.pop("action_key")
-    action_args = kwargs["action_args"]
-    action_kwargs = kwargs["action_kwargs"]
-    action_target = kwargs.pop("action_target", None)
-    combat_handler = caller.ndb._evmenu.combathandler
-    combat_handler.register_action(caller, action_key, action_target, *action_args, **action_kwargs)
-
-    # move into waiting
-    return "node_wait_turn"
-
-
-def node_confirm_register_action(caller, raw_string, **kwargs):
-    """
-    Node where one can confirm registering the action or change one's mind.
-
-    """
-    action_key = kwargs["action_key"]
-    action_target = kwargs.get("action_target", None) or ""
-    if action_target:
-        action_target = f", targeting {action_target.key}"
-
-    text = f"You will {action_key}{action_target}. Confirm? [Y]/n"
-    options = (
-        {
-            "key": "_default",
-            "goto": (_register_action, kwargs),
-        },
-        {"key": ("Abort/Cancel", "abort", "cancel", "a", "no", "n"), "goto": "node_select_action"},
-    )
-    return text, options
-
-
-def _select_target_helper(caller, raw_string, targets, **kwargs):
-    """
-    Helper to select among only friendly or enemy targets (given by the calling node).
-
-    """
-    action_key = kwargs["action_key"]
-    text = f"Select target for |w{action_key}|n."
-
-    # make the apply-self option always the first one, give it key 0
-    if caller in targets:
-        targets.remove(caller)
-        kwargs["action_target"] = caller
-        options = [{"key": "0", "desc": "(yourself)", "goto": (_register_action, kwargs)}]
-    # filter out ourselves and then make options for everyone else
-    for inum, combatant in enumerate(targets):
-        kwargs["action_target"] = combatant
-        options.append(
-            {"key": str(inum + 1), "desc": combatant.key, "goto": (_register_action, kwargs)}
-        )
-
-    # add ability to cancel
-    options.append({"key": "_default", "goto": "node_select_action"})
-
-    return text, options
-
-
-def node_select_enemy_target(caller, raw_string, **kwargs):
-    """
-    Menu node allowing for selecting an enemy target among all combatants. This combines
-    with all other actions.
-
-    """
-    combat = caller.ndb._evmenu.combathandler
-    targets = combat.get_enemy_targets(caller)
-    return _select_target_helper(caller, raw_string, targets, **kwargs)
-
-
-def node_select_friendly_target(caller, raw_string, **kwargs):
-    """
-    Menu node for selecting a friendly target among combatants (including oneself).
-
-    """
-    combat = caller.ndb._evmenu.combathandler
-    targets = combat.get_friendly_targets(caller)
-    return _select_target_helper(caller, raw_string, targets, **kwargs)
-
-
-def _item_broken(caller, raw_string, **kwargs):
-    caller.msg("|rThis item is broken and unusable!|n")
-    return None  # back to previous node
-
-
-def node_select_wield_from_inventory(caller, raw_string, **kwargs):
-    """
-    Menu node allowing for wielding item(s) from inventory.
-
-    """
-    loadout = caller.equipment.display_loadout()
-    text = (
-        f"{loadout}\nSelect weapon, spell or shield to draw. It will swap out "
-        "anything already in the same hand (you can't change armor or helmet in combat)."
-    )
-
-    # get a list of all suitable weapons/spells/shields
-    options = []
-    for obj in caller.equipment.get_wieldable_objects_from_backpack():
-        if obj.quality <= 0:
-            # object is broken
-            options.append(
-                {
-                    "desc": "|Rstr(obj)|n",
-                    "goto": _item_broken,
-                }
-            )
+        if any(self._carries_light(obj) for obj in self.contents if obj != exclude):
+            self.locks.add("view:all()")
+            self.cmdset.remove(DarkCmdSet)
+            self.db.is_lit = True
+            for char in (obj for obj in self.contents if obj.has_account):
+                # this won't do anything if it is already removed
+                char.msg("The room is lit up.")
         else:
-            # normally working item
-            kwargs["action_args"] = (obj,)
-            options.append({"desc": str(obj), "goto": (_register_action, kwargs)})
-
-    # add ability to cancel
-    options.append(
-        {"key": "_default", "desc": "(No input to Abort and go back)", "goto": "node_select_action"}
-    )
-
-    return text, options
+            # noone is carrying light - darken the room
+            self.db.is_lit = False
+            self.locks.add("view:false()")
+            self.cmdset.add(DarkCmdSet, persistent=True)
+            for char in (obj for obj in self.contents if obj.has_account):
+                if char.is_superuser:
+                    char.msg("You are Superuser, so you are not affected by the dark state.")
+                else:
+                    # put players in darkness
+                    char.msg("The room is completely dark.")
+
+    def at_object_receive(self, obj, source_location, move_type="move", **kwargs):
+        """
+        Called when an object enters the room.
+        """
+        if obj.has_account:
+            # a puppeted object, that is, a Character
+            self._heal(obj)
+            # in case the new guy carries light with them
+            self.check_light_state()
+
+    def at_object_leave(self, obj, target_location, move_type="move", **kwargs):
+        """
+        In case people leave with the light, we make sure to clear the
+        DarkCmdSet if necessary.  This also works if they are
+        teleported away.
+        """
+        # since this hook is called while the object is still in the room,
+        # we exclude it from the light check, to ignore any light sources
+        # it may be carrying.
+        self.check_light_state(exclude=obj)
+
+
+# -------------------------------------------------------------
+#
+# Teleport room - puzzles solution
+#
+# This is a sort of puzzle room that requires a certain
+# attribute on the entering character to be the same as
+# an attribute of the room. If not, the character will
+# be teleported away to a target location. This is used
+# by the Obelisk - grave chamber puzzle, where one must
+# have looked at the obelisk to get an attribute set on
+# oneself, and then pick the grave chamber with the
+# matching imagery for this attribute.
+#
+# -------------------------------------------------------------
+
+
+class TeleportRoom(TutorialRoom):
+    """
+    Teleporter - puzzle room.
+
+    Important attributes (set at creation):
+      puzzle_key    - which attr to look for on character
+      puzzle_value  - what char.db.puzzle_key must be set to
+      success_teleport_to -  where to teleport in case if success
+      success_teleport_msg - message to echo while teleporting to success
+      failure_teleport_to - where to teleport to in case of failure
+      failure_teleport_msg - message to echo while teleporting to failure
+
+    """
+
+    def at_object_creation(self):
+        """Called at first creation"""
+        super().at_object_creation()
+        # what character.db.puzzle_clue must be set to, to avoid teleportation.
+        self.db.puzzle_value = 1
+        # target of successful teleportation. Can be a dbref or a
+        # unique room name.
+        self.db.success_teleport_msg = "You are successful!"
+        self.db.success_teleport_to = "treasure room"
+        # the target of the failure teleportation.
+        self.db.failure_teleport_msg = "You fail!"
+        self.db.failure_teleport_to = "dark cell"
 
-
-def node_select_use_item_from_inventory(caller, raw_string, **kwargs):
-    """
-    Menu item allowing for using usable items (like potions) from inventory.
-
-    """
-    text = "Select an item to use."
-
-    # get a list of all suitable weapons/spells/shields
-    options = []
-    for obj in caller.inventory.get_usable_objects_from_backpack():
-        if obj.quality <= 0:
-            # object is broken
-            options.append(
-                {
-                    "desc": "|Rstr(obj)|n",
-                    "goto": _item_broken,
-                }
-            )
+    def at_object_receive(self, character, source_location, move_type="move", **kwargs):
+        """
+        This hook is called by the engine whenever the player is moved into
+        this room.
+        """
+        if not character.has_account:
+            # only act on player characters.
+            return
+        # determine if the puzzle is a success or not
+        is_success = str(character.db.puzzle_clue) == str(self.db.puzzle_value)
+        teleport_to = self.db.success_teleport_to if is_success else self.db.failure_teleport_to
+        # note that this returns a list
+        results = search_object(teleport_to)
+        if not results or len(results) > 1:
+            # we cannot move anywhere since no valid target was found.
+            character.msg("no valid teleport target for %s was found." % teleport_to)
+            return
+        if character.is_superuser:
+            # superusers don't get teleported
+            character.msg("Superuser block: You would have been teleported to %s." % results[0])
+            return
+        # perform the teleport
+        if is_success:
+            character.msg(self.db.success_teleport_msg)
         else:
-            # normally working item
-            kwargs["action_args"] = (obj,)
-            options.append({"desc": str(obj), "goto": (_register_action, kwargs)})
+            character.msg(self.db.failure_teleport_msg)
+        # teleport quietly to the new place
+        character.move_to(results[0], quiet=True, move_hooks=False, move_type="teleport")
+        # we have to call this manually since we turn off move_hooks
+        # - this is necessary to make the target dark room aware of an
+        # already carried light.
+        results[0].at_object_receive(character, self)
 
-    # add ability to cancel
-    options.append({"key": "_default", "goto": "node_select_action"})
 
-    return text, options
+# -------------------------------------------------------------
+#
+# Outro room - unique exit room
+#
+# Cleans up the character from all tutorial-related properties.
+#
+# -------------------------------------------------------------
 
 
-def _action_unavailable(caller, raw_string, **kwargs):
+class OutroRoom(TutorialRoom):
     """
-    Selecting an unavailable action.
+    Outro room.
 
-    """
-    action_key = kwargs["action_key"]
-    caller.msg(f"|rAction |w{action_key}|r is currently not available.|n")
-    # go back to previous node
-    return
+    Called when exiting the tutorial, cleans the
+    character of tutorial-related attributes.
 
-
-def node_select_action(caller, raw_string, **kwargs):
     """
-    Menu node for selecting a combat action.
 
-    """
-    combat = caller.ndb._evmenu.combathandler
-    text = combat.get_combat_summary(caller)
-
-    options = []
-    for icount, action in enumerate(combat.get_available_actions(caller)):
-        # we handle counts manually so we can grey the entire line if action is unavailable.
-        key = str(icount + 1)
-        desc = action.desc
-
-        if not action.can_use():
-            # action is unavailable. Greyscale the option if not available and route to the
-            # _action_unavailable helper
-            key = f"|x{key}|n"
-            desc = f"|x{desc}|n"
-
-            options.append(
-                {
-                    "key": (key,) + tuple(action.aliases),
-                    "desc": desc,
-                    "goto": (_action_unavailable, {"action_key": action.key}),
-                }
-            )
-        elif action.next_menu_node is None:
-            # action is available, but needs no intermediary step. Redirect to register
-            # the action immediately
-            options.append(
-                {
-                    "key": (key,) + tuple(action.aliases),
-                    "desc": desc,
-                    "goto": (
-                        _register_action,
-                        {
-                            "action_key": action.key,
-                            "action_args": (),
-                            "action_kwargs": {},
-                            "action_target": None,
-                        },
-                    ),
-                }
-            )
-        else:
-            # action is available and next_menu_node is set to point to the next node we want
-            options.append(
-                {
-                    "key": (key,) + tuple(action.aliases),
-                    "desc": desc,
-                    "goto": (
-                        action.next_menu_node,
-                        {
-                            "action_key": action.key,
-                            "action_args": (),
-                            "action_kwargs": {},
-                            "action_target": None,
-                        },
-                    ),
-                }
-            )
-        # add ability to cancel
-        options.append(
-            {
-                "key": "_default",
-                "goto": "node_select_action",
-            }
+    def at_object_creation(self):
+        """
+        Called when the room is first created.
+        """
+        super().at_object_creation()
+        self.db.tutorial_info = (
+            "The last room of the tutorial. "
+            "This cleans up all temporary Attributes "
+            "the tutorial may have assigned to the "
+            "character."
         )
 
-    return text, options
-
-
-def node_wait_turn(caller, raw_string, **kwargs):
-    """
-    Menu node routed to waiting for the round to end (for everyone to choose their actions).
-
-    All menu actions route back to the same node. The CombatHandler will handle moving everyone back
-    to the `node_select_action` node when the next round starts.
-
-    """
-    text = "Waiting for other combatants ..."
-
-    options = {
-        "key": "_default",
-        "desc": "(next round will start automatically)",
-        "goto": "node_wait_turn",
-    }
-    return text, options
-
-
-def node_wait_start(caller, raw_string, **kwargs):
-    """
-    Menu node entered when waiting for the combat to start. New players joining an existing
-    combat will end up here until the previous round is over, at which point the combat handler
-    will goto everyone to `node_select_action`.
-
-    """
-    text = "Waiting for combat round to start ..."
-
-    options = {
-        "key": "_default",
-        "desc": "(combat will start automatically)",
-        "goto": "node_wait_start",
-    }
-    return text, options
-
-
-# -----------------------------------------------------------------------------------
-#  Access function
-# -----------------------------------------------------------------------------------
-
-
-def join_combat(caller, *targets, session=None):
-    """
-    Join or create a new combat involving caller and at least one target. The combat
-    is started on the current room location - this means there can only be one combat
-    in each room (this is not hardcoded in the combat per-se, but it makes sense for
-    this implementation).
-
-    Args:
-        caller (Object): The one starting the combat.
-        *targets (Objects): Any other targets to pull into combat. At least one target
-            is required if `combathandler` is not given (a new combat must have at least
-            one opponent!).
-
-    Keyword Args:
-        session (Session, optional): A player session to use. This is useful for multisession modes.
-
-    Returns:
-        EvAdventureCombatHandler: A created or existing combat handler.
-
-    """
-    created = False
-    location = caller.location
-    if not location:
-        raise CombatFailure("Must have a location to start combat.")
-
-    if caller.hp <= 0:
-        raise CombatFailure("You can't start a fight in your current condition!")
-
-    if not getattr(location, "allow_combat", False):
-        raise CombatFailure("This is not the time and place for picking a fight.")
-
-    if not targets:
-        raise CombatFailure("Must have an opponent to start combat.")
-
-    combathandler = location.scripts.get(COMBAT_HANDLER_KEY).first()
-    if not combathandler:
-        combathandler = location.scripts.add(EvAdventureCombatHandler, autostart=False)
-        created = True
-
-    if not hasattr(caller, "hp"):
-        raise CombatFailure("You have no hp and so can't attack anyone.")
-
-    # it's safe to add a combatant to the same combat more than once
-    combathandler.add_combatant(caller, session=session)
-    for target in targets:
-        if target.hp <= 0:
-            caller.msg(f"{target.get_display_name(caller)} is already out of it.")
-            continue
-        combathandler.add_combatant(target)
-
-    if created:
-        combathandler.start_combat()
-
-    return combathandler
+    def at_object_receive(self, character, source_location, move_type="move", **kwargs):
+        """
+        Do cleanup.
+        """
+        if character.has_account:
+            del character.db.health_max
+            del character.db.health
+            del character.db.last_climbed
+            del character.db.puzzle_clue
+            del character.db.combat_parry_mode
+            del character.db.tutorial_bridge_position
+            for obj in character.contents:
+                if obj.typeclass_path.startswith("evennia.contrib.tutorials.tutorial_world"):
+                    obj.delete()
+            character.tags.clear(category="tutorial_world")
+
+    def at_object_leave(self, character, destination, move_type="move", **kwargs):
+        if character.account:
+            character.account.execute_cmd("unquell")
```

### Comparing `evennia-1.3.0/evennia/contrib/tutorials/evadventure/commands.py` & `evennia-2.0.0/evennia/contrib/tutorials/evadventure/commands.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 EvAdventure commands and cmdsets. We don't need that many stand-alone new
 commands since a lot of functionality is managed in menus. These commands
 are in additional to normal Evennia commands and should be added
 to the CharacterCmdSet
 
 New commands:
-    attack/hit <target>[,...]
     inventory
     wield/wear <item>
     unwield/remove <item>
     give <item or coin> to <character>
     talk <npc>
 
 To install, add the `EvAdventureCmdSet` from this module to the default character cmdset:
@@ -29,15 +28,14 @@
 ```
 """
 
 from evennia import CmdSet, Command, InterruptCommand
 from evennia.utils.evmenu import EvMenu
 from evennia.utils.utils import inherits_from
 
-from .combat_turnbased import CombatFailure, join_combat
 from .enums import WieldLocation
 from .equipment import EquipmentError
 from .npcs import EvAdventureTalkativeNPC
 from .utils import get_obj_stats
 
 
 class EvAdventureCommand(Command):
@@ -50,59 +48,14 @@
 
     """
 
     def parse(self):
         self.args = self.args.strip()
 
 
-class CmdAttackTurnBased(EvAdventureCommand):
-    """
-    Attack a target or join an existing combat.
-
-    Usage:
-      attack <target>
-      attack <target>, <target>, ...
-
-    If the target is involved in combat already, you'll join combat with
-    the first target you specify. Attacking multiple will draw them all into
-    combat.
-
-    This will start/join turn-based, combat, where you have a limited
-    time to decide on your next action from a menu of options.
-
-    """
-
-    key = "attack"
-    aliases = ("hit",)
-
-    def parse(self):
-        super().parse()
-        self.targets = [name.strip() for name in self.args.split(",")]
-
-    def func(self):
-
-        # find if
-
-        target_objs = []
-        for target in self.targets:
-            target_obj = self.caller.search(target)
-            if not target_obj:
-                # show a warning but don't abort
-                continue
-            target_objs.append(target_obj)
-
-        if target_objs:
-            try:
-                join_combat(self.caller, *target_objs, session=self.session)
-            except CombatFailure as err:
-                self.caller.msg(f"|r{err}|n")
-        else:
-            self.caller.msg("|rFound noone to attack.|n")
-
-
 class CmdInventory(EvAdventureCommand):
     """
     View your inventory
 
     Usage:
       inventory
 
@@ -265,23 +218,27 @@
         item = giver.equipment.remove(item)
         if item:
             try:
                 # this will also add them to the equipment backpack, if possible
                 item.move_to(caller, quiet=True, move_type="give")
             except EquipmentError:
                 caller.location.msg_contents(
-                    f"$You({giver.key.key}) $conj(try) to give "
-                    f"{item.key} to $You({caller.key}), but they can't accept it since their "
-                    "inventory is full.",
+                    (
+                        f"$You({giver.key.key}) $conj(try) to give "
+                        f"{item.key} to $You({caller.key}), but they can't accept it since their "
+                        "inventory is full."
+                    ),
                     mapping={giver.key: giver, caller.key: caller},
                 )
             else:
                 caller.location.msg_contents(
-                    f"$You({giver.key}) $conj(give) {item.key} to $You({caller.key}), "
-                    "and they accepted the offer.",
+                    (
+                        f"$You({giver.key}) $conj(give) {item.key} to $You({caller.key}), "
+                        "and they accepted the offer."
+                    ),
                     mapping={giver.key: giver, caller.key: caller},
                 )
         giver.ndb._evmenu.close_menu()
         return "node_end"
 
 
 def node_receive(caller, raw_string, **kwargs):
@@ -451,13 +408,12 @@
     Groups all commands in one cmdset which can be added in one go to the DefaultCharacter cmdset.
 
     """
 
     key = "evadventure"
 
     def at_cmdset_creation(self):
-        self.add(CmdAttackTurnBased())
         self.add(CmdInventory())
         self.add(CmdWieldOrWear())
         self.add(CmdRemove())
         self.add(CmdGive())
         self.add(CmdTalk())
```

### Comparing `evennia-1.3.0/evennia/contrib/tutorials/evadventure/dungeon.py` & `evennia-2.0.0/evennia/contrib/tutorials/evadventure/dungeon.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,16 +84,16 @@
 
 class EvAdventureDungeonRoom(EvAdventureRoom):
     """
     Dangerous dungeon room.
 
     """
 
-    allow_combat = True
-    allow_death = True
+    allow_combat = AttributeProperty(True, autocreate=False)
+    allow_death = AttributeProperty(True, autocreate=False)
 
     # dungeon generation attributes; set when room is created
     back_exit = AttributeProperty(None, autocreate=False)
     dungeon_orchestrator = AttributeProperty(None, autocreate=False)
     xy_coords = AttributeProperty(None, autocreate=False)
 
     @property
```

### Comparing `evennia-1.3.0/evennia/contrib/tutorials/evadventure/enums.py` & `evennia-2.0.0/evennia/contrib/tutorials/evadventure/enums.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 """
 Enums are constants representing different things in EvAdventure. The advantage
 of using an Enum over, say, a string is that if you make a typo using an unknown
 enum, Python will give you an error while a typo in a string may go through silently.
 
 It's used as a direct reference:
+::
 
     from enums import Ability
 
     if abi is Ability.STR:
         # ...
 
 To get the `value` of an enum (must always be hashable, useful for Attribute lookups), use
 `Ability.STR.value` (which would return 'strength' in our case).
 
+----
+
 """
 from enum import Enum
 
 
 class Ability(Enum):
     """
     The six base abilities (defense is always bonus + 10)
@@ -36,14 +39,24 @@
     CRITICAL_SUCCESS = "critical_success"
 
     ALLEGIANCE_HOSTILE = "hostile"
     ALLEGIANCE_NEUTRAL = "neutral"
     ALLEGIANCE_FRIENDLY = "friendly"
 
 
+ABILITY_REVERSE_MAP = {
+    "str": Ability.STR,
+    "dex": Ability.DEX,
+    "con": Ability.CON,
+    "int": Ability.INT,
+    "wis": Ability.WIS,
+    "cha": Ability.CHA,
+}
+
+
 class WieldLocation(Enum):
     """
     Wield (or wear) locations.
 
     """
 
     # wield/wear location
@@ -63,10 +76,11 @@
 
     WEAPON = "weapon"
     ARMOR = "armor"
     SHIELD = "shield"
     HELMET = "helmet"
     CONSUMABLE = "consumable"
     GEAR = "gear"
+    THROWABLE = "throwable"
     MAGIC = "magic"
     QUEST = "quest"
     TREASURE = "treasure"
```

### Comparing `evennia-1.3.0/evennia/contrib/tutorials/evadventure/equipment.py` & `evennia-2.0.0/evennia/contrib/tutorials/evadventure/equipment.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Knave has a system of Slots for its inventory.
 
 """
 
 from evennia.utils.utils import inherits_from
 
 from .enums import Ability, WieldLocation
-from .objects import EvAdventureObject, WeaponEmptyHand
+from .objects import EvAdventureObject, get_bare_hands
 
 
 class EquipmentError(TypeError):
     pass
 
 
 class EquipmentHandler:
@@ -45,14 +45,17 @@
                 WieldLocation.SHIELD_HAND: None,
                 WieldLocation.TWO_HANDS: None,
                 WieldLocation.BODY: None,
                 WieldLocation.HEAD: None,
                 WieldLocation.BACKPACK: [],
             },
         )
+        self.slots[WieldLocation.BACKPACK] = [
+            obj for obj in self.slots[WieldLocation.BACKPACK] if obj and obj.id
+        ]
 
     def _save(self):
         """
         Save slot to storage.
 
         """
         self.obj.attributes.add(self.save_attribute, self.slots, category="inventory")
@@ -163,15 +166,15 @@
         # first checks two-handed wield, then one-handed; the two
         # should never appear simultaneously anyhow (checked in `move` method).
         slots = self.slots
         weapon = slots[WieldLocation.TWO_HANDS]
         if not weapon:
             weapon = slots[WieldLocation.WEAPON_HAND]
         if not weapon:
-            weapon = WeaponEmptyHand()
+            weapon = get_bare_hands()
         return weapon
 
     def display_loadout(self):
         """
         Get a visual representation of your current loadout.
 
         Returns:
@@ -353,15 +356,17 @@
             quality, so this may include broken items (we may want to visually show them
             in the list after all).
 
         """
         return [
             obj
             for obj in self.slots[WieldLocation.BACKPACK]
-            if obj.inventory_use_slot
+            if obj
+            and obj.id
+            and obj.inventory_use_slot
             in (WieldLocation.WEAPON_HAND, WieldLocation.TWO_HANDS, WieldLocation.SHIELD_HAND)
         ]
 
     def get_wearable_objects_from_backpack(self):
         """
         Get all wearable items (armor or helmets) from backpack. This is useful in order to
         have a list to select from when swapping your worn loadout.
@@ -371,28 +376,30 @@
             quality, so this may include broken items (we may want to visually show them
             in the list after all).
 
         """
         return [
             obj
             for obj in self.slots[WieldLocation.BACKPACK]
-            if obj.inventory_use_slot in (WieldLocation.BODY, WieldLocation.HEAD)
+            if obj and obj.id and obj.inventory_use_slot in (WieldLocation.BODY, WieldLocation.HEAD)
         ]
 
     def get_usable_objects_from_backpack(self):
         """
         Get all 'usable' items (like potions) from backpack. This is useful for getting a
         list to select from.
 
         Returns:
             list: A list of objects that are usable.
 
         """
         character = self.obj
-        return [obj for obj in self.slots[WieldLocation.BACKPACK] if obj.at_pre_use(character)]
+        return [
+            obj for obj in self.slots[WieldLocation.BACKPACK] if obj and obj.at_pre_use(character)
+        ]
 
     def all(self, only_objs=False):
         """
         Get all objects in inventory, regardless of location.
 
         Keyword Args:
             only_objs (bool): Only return a flat list of objects, not tuples.
```

### Comparing `evennia-1.3.0/evennia/contrib/tutorials/evadventure/npcs.py` & `evennia-2.0.0/evennia/contrib/tutorials/evadventure/npcs.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 EvAdventure NPCs. This includes both friends and enemies, only separated by their AI.
 
 """
 from random import choice
 
 from evennia import DefaultCharacter
 from evennia.typeclasses.attributes import AttributeProperty
+from evennia.typeclasses.tags import TagProperty
 from evennia.utils.evmenu import EvMenu
 from evennia.utils.utils import make_iter
 
 from .characters import LivingMixin
 from .enums import Ability, WieldLocation
-from .objects import WeaponEmptyHand
+from .objects import get_bare_hands
 from .rules import dice
 
 
 class EvAdventureNPC(LivingMixin, DefaultCharacter):
     """
     This is the base class for all non-player entities, including monsters. These
     generally don't advance in level but uses a simplified, abstract measure of how
@@ -46,17 +47,21 @@
     morale = AttributeProperty(default=9, autocreate=False)
     hp_multiplier = AttributeProperty(default=4, autocreate=False)  # 4 default in Knave
     hp = AttributeProperty(default=None, autocreate=False)  # internal tracking, use .hp property
     allegiance = AttributeProperty(default=Ability.ALLEGIANCE_HOSTILE, autocreate=False)
 
     is_idle = AttributeProperty(default=False, autocreate=False)
 
-    weapon = AttributeProperty(default=WeaponEmptyHand, autocreate=False)  # instead of inventory
+    weapon = AttributeProperty(default=get_bare_hands, autocreate=False)  # instead of inventory
     coins = AttributeProperty(default=1, autocreate=False)  # coin loot
 
+    # if this npc is attacked, everyone with the same tag in the current location will also be
+    # pulled into combat.
+    group = TagProperty("npcs")
+
     @property
     def strength(self):
         return self.hit_dice
 
     @property
     def dexterity(self):
         return self.hit_dice
@@ -83,16 +88,24 @@
 
     def at_object_creation(self):
         """
         Start with max health.
 
         """
         self.hp = self.hp_max
+        self.tags.add("npcs", category="group")
+
+    def at_attacked(self, attacker, **kwargs):
+        """
+        Called when being attacked and combat starts.
+
+        """
+        pass
 
-    def ai_combat_next_action(self):
+    def ai_next_action(self, **kwargs):
         """
         The combat engine should ask this method in order to
         get the next action the npc should perform in combat.
 
         """
         pass
 
@@ -239,28 +252,28 @@
     Mob (mobile) NPC; this is usually an enemy.
 
     """
 
     # chance (%) that this enemy will loot you when defeating you
     loot_chance = AttributeProperty(75, autocreate=False)
 
-    def ai_combat_next_action(self, combathandler):
+    def ai_next_action(self, **kwargs):
         """
         Called to get the next action in combat.
 
         Args:
             combathandler (EvAdventureCombatHandler): The currently active combathandler.
 
         Returns:
             tuple: A tuple `(str, tuple, dict)`, being the `action_key`, and the `*args` and
             `**kwargs` for that action. The action-key is that of a CombatAction available to the
             combatant in the current combat handler.
 
         """
-        from .combat_turnbased import CombatActionAttack, CombatActionDoNothing
+        from .combat import CombatActionAttack, CombatActionDoNothing
 
         if self.is_idle:
             # mob just stands around
             return CombatActionDoNothing.key, (), {}
 
         target = choice(combathandler.get_enemy_targets(self))
```

### Comparing `evennia-1.3.0/evennia/contrib/tutorials/evadventure/quests.py` & `evennia-2.0.0/evennia/contrib/tutorials/evadventure/quests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/tutorials/evadventure/random_tables.py` & `evennia-2.0.0/evennia/contrib/tutorials/evadventure/random_tables.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/tutorials/evadventure/rooms.py` & `evennia-2.0.0/evennia/contrib/tutorials/evadventure/rooms.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 the dungeon generation. But one can also mix with other non-EvAdventure rooms (you will
 just not be able to fight in them).
 
 """
 
 from copy import deepcopy
 
-from evennia import DefaultCharacter, DefaultRoom
+from evennia import AttributeProperty, DefaultCharacter, DefaultRoom
 from evennia.utils.utils import inherits_from
 
 CHAR_SYMBOL = "|w@|n"
 CHAR_ALT_SYMBOL = "|w>|n"
 ROOM_SYMBOL = "|bo|n"
 LINK_COLOR = "|B"
 
@@ -40,17 +40,17 @@
 
 class EvAdventureRoom(DefaultRoom):
     """
     Simple room supporting some EvAdventure-specifics.
 
     """
 
-    allow_combat = False
-    allow_pvp = False
-    allow_death = False
+    allow_combat = AttributeProperty(False, autocreate=False)
+    allow_pvp = AttributeProperty(False, autocreate=False)
+    allow_death = AttributeProperty(False, autocreate=False)
 
     def format_appearance(self, appearance, looker, **kwargs):
         """Don't left-strip the appearance string"""
         return appearance.rstrip()
 
     def get_display_header(self, looker, **kwargs):
         """
@@ -86,16 +86,15 @@
 
 class EvAdventurePvPRoom(EvAdventureRoom):
     """
     Room where PvP can happen, but noone gets killed.
 
     """
 
-    allow_combat = True
-    allow_pvp = True
+    allow_combat = AttributeProperty(True, autocreate=False)
+    allow_pvp = AttributeProperty(True, autocreate=False)
 
     def get_display_footer(self, looker, **kwargs):
         """
-        Show if the room is 'cleared' or not as part of its description.
-
+        Customize footer of description.
         """
         return "|yNon-lethal PvP combat is allowed here!|n"
```

### Comparing `evennia-1.3.0/evennia/contrib/tutorials/evadventure/rules.py` & `evennia-2.0.0/evennia/contrib/tutorials/evadventure/rules.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,14 @@
 """
 MUD ruleset based on the _Knave_ OSR tabletop RPG by Ben Milton (modified for MUD use).
 
-The rules are divided into a set of classes. While each class (except chargen) could
-also have been stand-alone functions, having them as classes makes it a little easier
-to use them as the base for your own variation (tweaking values etc).
-
-- Roll-engine: Class with methods for making all dice rolls needed by the rules. Knave only
-  has a few resolution rolls, but we define helper methods for different actions the
-  character will be able to do in-code.
-- Character generation - this is a container used for holding, tweaking and setting
-  all character data during character generation. At the end it will save itself
-  onto the Character for permanent storage.
-- Improvement - this container holds rules used with experience to improve the
-  character over time.
-- Charsheet - a container with tools for visually displaying the character sheet in-game.
-
-This module presents several singletons to import
-
-- `dice` - the `EvAdventureRollEngine` for all random resolution and table-rolling.
-- `character_sheet` - the `EvAdventureCharacterSheet` visualizer.
-- `improvement` - the EvAdventureImprovement` class for handling char xp and leveling.
+The center of the rule system is the "RollEngine", which handles all rolling of dice
+and determining what the outcome is.
+
+----
 
 """
 from random import randint
 
 from .enums import Ability
 from .random_tables import death_and_dismemberment as death_table
 
@@ -153,21 +138,21 @@
         elif advantage:
             rolltxt = "|g2d20|n (advantage: picking highest) "
         elif disadvantage:
             rolltxt = "|r2d20|n (disadvantage: picking lowest) "
         bontxt = f"(+{bonus})"
         modtxt = ""
         if modifier:
-            modtxt = f" + {modifier}" if modifier > 0 else f" - {abs(modifier)}"
+            modtxt = f"+ {modifier}" if modifier > 0 else f" - {abs(modifier)}"
         qualtxt = f" ({quality.value}!)" if quality else ""
 
         txt = (
-            f"rolled {dice_roll} on {rolltxt} "
+            f" rolled {dice_roll} on {rolltxt} "
             f"+ {bonus_type.value}{bontxt}{modtxt} vs "
-            f"{target} -> |w{result}{qualtxt}|n"
+            f"{target} -> |w{'|GSuccess|w' if result else '|RFail|w'}{qualtxt}|n"
         )
 
         return (dice_roll + bonus + modifier) > target, quality, txt
 
     def opposed_saving_throw(
         self,
         attacker,
@@ -241,16 +226,15 @@
         if not table_choices:
             return None
 
         if isinstance(table_choices[0], (tuple, list)):
             # tuple with range conditional, like ('1-5', "Blue") or ('10', "Purple")
             max_range = -1
             min_range = 10**6
-            for (valrange, choice) in table_choices:
-
+            for valrange, choice in table_choices:
                 minval, *maxval = valrange.split("-", 1)
                 minval = abs(int(minval))
                 maxval = abs(int(maxval[0]) if maxval else minval)
 
                 # we store the largest/smallest values so far in case we need to use them
                 max_range = max(max_range, maxval)
                 min_range = min(min_range, minval)
@@ -328,17 +312,19 @@
             else:
                 # refresh health, but get permanent ability loss
                 new_hp = self.roll("1d4")
                 character.heal(new_hp)
                 setattr(character, abi, current_abi)
 
                 character.msg(
-                    "~" * 78 + "\n|yYou survive your brush with death, "
+                    "~" * 78
+                    + "\n|yYou survive your brush with death, "
                     f"but are |r{result.upper()}|y and permanently |rlose {loss} {abi}|y.|n\n"
-                    f"|GYou recover |g{new_hp}|G health|.\n" + "~" * 78
+                    f"|GYou recover |g{new_hp}|G health|.\n"
+                    + "~" * 78
                 )
 
 
 # singletons
 
 # access rolls e.g. with rules.dice.opposed_saving_throw(...)
 dice = EvAdventureRollEngine()
```

### Comparing `evennia-1.3.0/evennia/contrib/tutorials/evadventure/shops.py` & `evennia-2.0.0/evennia/contrib/tutorials/evadventure/shops.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/tutorials/evadventure/tests/mixins.py` & `evennia-2.0.0/evennia/contrib/tutorials/evadventure/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/tutorials/evadventure/tests/test_characters.py` & `evennia-2.0.0/evennia/contrib/tutorials/evadventure/tests/test_characters.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/tutorials/evadventure/tests/test_chargen.py` & `evennia-2.0.0/evennia/contrib/tutorials/evadventure/tests/test_chargen.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/tutorials/evadventure/tests/test_commands.py` & `evennia-2.0.0/evennia/contrib/tutorials/evadventure/tests/test_commands.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 Test the EvAdventure commands.
 
 """
 
 from unittest.mock import call, patch
 
 from anything import Something
-
 from evennia.utils.create import create_object
 from evennia.utils.test_resources import BaseEvenniaCommandTest
 
 from .. import commands
 from ..characters import EvAdventureCharacter
 from ..npcs import EvAdventureMob, EvAdventureShopKeeper
 from .mixins import EvAdventureMixin
@@ -30,26 +29,14 @@
 You are fighting with your bare fists and have no shield.
 You wear no armor and no helmet.
 Backpack is empty.
 You use 0/11 equipment slots.
 """.strip(),
         )
 
-    @patch("evennia.contrib.tutorials.evadventure.commands.join_combat")
-    def test_attack(self, mock_join_combat):
-        self.location.allow_combat = True
-
-        target = create_object(EvAdventureMob, key="Ogre", location=self.location)
-
-        self.call(commands.CmdAttackTurnBased(), "ogre", "")
-
-        mock_join_combat.assert_called_with(self.char1, target, session=Something)
-
-        target.delete()
-
     def test_wield_or_wear(self):
         self.char1.equipment.add(self.helmet)
         self.char1.equipment.add(self.weapon)
         self.shield.location = self.location
 
         self.call(commands.CmdWieldOrWear(), "shield", "Could not find 'shield'")
         self.call(commands.CmdWieldOrWear(), "helmet", "You put helmet on your head.")
@@ -81,15 +68,14 @@
 
         self.call(commands.CmdGive(), "60 to friend", "You only have 50 coins to give.")
 
         recipient.delete()
 
     @patch("evennia.contrib.tutorials.evadventure.commands.EvMenu")
     def test_give__item(self, mock_EvMenu):
-
         self.char1.equipment.add(self.helmet)
         recipient = create_object(EvAdventureCharacter, key="Friend", location=self.location)
 
         self.call(commands.CmdGive(), "helmet to friend", "")
 
         mock_EvMenu.assert_has_calls(
             (
```

### Comparing `evennia-1.3.0/evennia/contrib/tutorials/evadventure/tests/test_dungeon.py` & `evennia-2.0.0/evennia/contrib/tutorials/evadventure/tests/test_dungeon.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/tutorials/evadventure/tests/test_equipment.py` & `evennia-2.0.0/evennia/contrib/tutorials/evadventure/tests/test_equipment.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/tutorials/evadventure/tests/test_quests.py` & `evennia-2.0.0/evennia/contrib/tutorials/evadventure/tests/test_quests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/tutorials/evadventure/tests/test_rules.py` & `evennia-2.0.0/evennia/contrib/tutorials/evadventure/tests/test_rules.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/tutorials/evadventure/tests/test_utils.py` & `evennia-2.0.0/evennia/contrib/tutorials/evadventure/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/tutorials/evadventure/utils.py` & `evennia-2.0.0/evennia/contrib/tutorials/evadventure/utils.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/tutorials/mirror/mirror.py` & `evennia-2.0.0/evennia/contrib/tutorials/mirror/mirror.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/tutorials/red_button/README.md` & `evennia-2.0.0/evennia/contrib/tutorials/red_button/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/tutorials/red_button/red_button.py` & `evennia-2.0.0/evennia/contrib/tutorials/red_button/red_button.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/tutorials/talking_npc/README.md` & `evennia-2.0.0/evennia/contrib/tutorials/talking_npc/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/tutorials/talking_npc/talking_npc.py` & `evennia-2.0.0/evennia/contrib/tutorials/talking_npc/talking_npc.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/tutorials/tutorial_world/README.md` & `evennia-2.0.0/evennia/contrib/tutorials/tutorial_world/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/tutorials/tutorial_world/build.ev` & `evennia-2.0.0/evennia/contrib/tutorials/tutorial_world/build.ev`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/tutorials/tutorial_world/intro_menu.py` & `evennia-2.0.0/evennia/contrib/tutorials/tutorial_world/intro_menu.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/tutorials/tutorial_world/mob.py` & `evennia-2.0.0/evennia/contrib/tutorials/tutorial_world/mob.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/tutorials/tutorial_world/objects.py` & `evennia-2.0.0/evennia/contrib/tutorials/tutorial_world/objects.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/tutorials/tutorial_world/tests.py` & `evennia-2.0.0/evennia/contrib/tutorials/tutorial_world/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/utils/auditing/README.md` & `evennia-2.0.0/evennia/contrib/utils/auditing/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/utils/auditing/outputs.py` & `evennia-2.0.0/evennia/contrib/utils/auditing/outputs.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/utils/auditing/server.py` & `evennia-2.0.0/evennia/contrib/utils/auditing/server.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/utils/auditing/tests.py` & `evennia-2.0.0/evennia/contrib/utils/auditing/tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,33 +5,33 @@
 
 import re
 
 from anything import Anything
 from django.test import override_settings
 from mock import patch
 
-from evennia.server.sessionhandler import SESSIONS
+import evennia
 from evennia.utils.test_resources import BaseEvenniaTest
 
 from .server import AuditedServerSession
 
 
 @override_settings(AUDIT_MASKS=[])
 class AuditingTest(BaseEvenniaTest):
     @patch("evennia.server.sessionhandler._ServerSession", AuditedServerSession)
     def setup_session(self):
         """Overrides default one in EvenniaTest"""
         dummysession = AuditedServerSession()
-        dummysession.init_session("telnet", ("localhost", "testmode"), SESSIONS)
+        dummysession.init_session("telnet", ("localhost", "testmode"), evennia.SESSION_HANDLER)
         dummysession.sessid = 1
-        SESSIONS.portal_connect(
+        evennia.SESSION_HANDLER.portal_connect(
             dummysession.get_sync_data()
         )  # note that this creates a new Session!
-        session = SESSIONS.session_from_sessid(1)  # the real session
-        SESSIONS.login(session, self.account, testmode=True)
+        session = evennia.SESSION_HANDLER.session_from_sessid(1)  # the real session
+        evennia.SESSION_HANDLER.login(session, self.account, testmode=True)
         self.session = session
 
     @patch(
         "evennia.contrib.utils.auditing.server.AUDIT_CALLBACK",
         "evennia.contrib.utils.auditing.outputs.to_syslog",
     )
     @patch("evennia.contrib.utils.auditing.server.AUDIT_IN", True)
```

### Comparing `evennia-1.3.0/evennia/contrib/utils/fieldfill/README.md` & `evennia-2.0.0/evennia/contrib/utils/fieldfill/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/utils/fieldfill/fieldfill.py` & `evennia-2.0.0/evennia/contrib/utils/fieldfill/fieldfill.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,17 +134,16 @@
         the player's input is considered valid - if it returns False,
         the input is rejected. Any other value returned will act as
         the field's new value, replacing the player's input. This
         allows for values that aren't strings or integers (such as
         object dbrefs). For boolean fields, return '0' or '1' to set
         the field to False or True.
 """
-
+import evennia
 from evennia import Command
-from evennia.server.sessionhandler import SESSIONS
 from evennia.utils import delay, evmenu, evtable, list_to_string, logger
 
 
 class FieldEvMenu(evmenu.EvMenu):
     """
     Custom EvMenu type with its own node formatter - removes extraneous lines
     """
@@ -569,15 +568,15 @@
     Returns:
         matched_character (obj or False): dbref to a currently logged in
             character object - reference to the object will be stored in
             the form instead of a string. Returns False if no match is
             made.
     """
     # Get a list of sessions
-    session_list = SESSIONS.get_sessions()
+    session_list = evennia.SESSION_HANDLER.get_sessions()
     char_list = []
     matched_character = None
 
     # Get a list of online characters
     for session in session_list:
         if not session.logged_in:
             # Skip over logged out characters
```

### Comparing `evennia-1.3.0/evennia/contrib/utils/git_integration/README.md` & `evennia-2.0.0/evennia/contrib/utils/git_integration/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/utils/git_integration/git_integration.py` & `evennia-2.0.0/evennia/contrib/utils/git_integration/git_integration.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import datetime
 
 import git
 from django.conf import settings
 
+import evennia
 from evennia import CmdSet, InterruptCommand
 from evennia.commands.default.muxcommand import MuxCommand
-from evennia.server.sessionhandler import SESSIONS
 from evennia.utils.utils import list_to_string
 
 
 class GitCommand(MuxCommand):
     """
     The shared functionality between git/git evennia
     """
@@ -143,18 +143,18 @@
 
         if self.action == "status":
             caller.msg(self.get_status())
         elif self.action == "branch" or (self.action == "checkout" and not self.args):
             caller.msg(self.get_branches())
         elif self.action == "checkout":
             if self.checkout():
-                SESSIONS.portal_restart_server()
+                evennia.SESSION_HANDLER.portal_restart_server()
         elif self.action == "pull":
             if self.pull():
-                SESSIONS.portal_restart_server()
+                evennia.SESSION_HANDLER.portal_restart_server()
         else:
             caller.msg("You can only git status, git branch, git checkout, or git pull.")
             return
 
 
 class CmdGitEvennia(GitCommand):
     """
```

### Comparing `evennia-1.3.0/evennia/contrib/utils/git_integration/tests.py` & `evennia-2.0.0/evennia/contrib/utils/git_integration/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/utils/name_generator/README.md` & `evennia-2.0.0/evennia/contrib/utils/name_generator/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/utils/name_generator/btn_givennames.txt` & `evennia-2.0.0/evennia/contrib/utils/name_generator/btn_givennames.txt`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/utils/name_generator/btn_surnames.txt` & `evennia-2.0.0/evennia/contrib/utils/name_generator/btn_surnames.txt`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/utils/name_generator/namegen.py` & `evennia-2.0.0/evennia/contrib/utils/name_generator/namegen.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/utils/name_generator/tests.py` & `evennia-2.0.0/evennia/contrib/utils/name_generator/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/utils/random_string_generator/README.md` & `evennia-2.0.0/evennia/contrib/utils/random_string_generator/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/utils/random_string_generator/random_string_generator.py` & `evennia-2.0.0/evennia/contrib/utils/random_string_generator/random_string_generator.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/utils/random_string_generator/tests.py` & `evennia-2.0.0/evennia/contrib/utils/random_string_generator/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/utils/tree_select/README.md` & `evennia-2.0.0/evennia/contrib/utils/tree_select/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/utils/tree_select/tests.py` & `evennia-2.0.0/evennia/contrib/utils/tree_select/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/contrib/utils/tree_select/tree_select.py` & `evennia-2.0.0/evennia/contrib/utils/tree_select/tree_select.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/game_template/README.md` & `evennia-2.0.0/evennia/game_template/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/game_template/commands/README.md` & `evennia-2.0.0/evennia/game_template/commands/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/game_template/commands/command.py` & `evennia-2.0.0/evennia/game_template/commands/command.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/game_template/commands/default_cmdsets.py` & `evennia-2.0.0/evennia/game_template/commands/default_cmdsets.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/game_template/gitignore` & `evennia-2.0.0/evennia/game_template/gitignore`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/game_template/server/README.md` & `evennia-2.0.0/evennia/game_template/server/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/game_template/server/conf/at_initial_setup.py` & `evennia-2.0.0/evennia/game_template/server/conf/at_initial_setup.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/game_template/server/conf/at_search.py` & `evennia-2.0.0/evennia/game_template/server/conf/at_search.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/game_template/server/conf/at_server_startstop.py` & `evennia-2.0.0/evennia/game_template/server/conf/at_server_startstop.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/game_template/server/conf/cmdparser.py` & `evennia-2.0.0/evennia/game_template/server/conf/cmdparser.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/game_template/server/conf/connection_screens.py` & `evennia-2.0.0/evennia/game_template/server/conf/connection_screens.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/game_template/server/conf/inlinefuncs.py` & `evennia-2.0.0/evennia/game_template/server/conf/inlinefuncs.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/game_template/server/conf/inputfuncs.py` & `evennia-2.0.0/evennia/game_template/server/conf/inputfuncs.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/game_template/server/conf/lockfuncs.py` & `evennia-2.0.0/evennia/game_template/server/conf/lockfuncs.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/game_template/server/conf/mssp.py` & `evennia-2.0.0/evennia/game_template/server/conf/mssp.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/game_template/server/conf/portal_services_plugins.py` & `evennia-2.0.0/evennia/game_template/server/conf/portal_services_plugins.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/game_template/server/conf/secret_settings.py` & `evennia-2.0.0/evennia/game_template/server/conf/secret_settings.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/game_template/server/conf/server_services_plugins.py` & `evennia-2.0.0/evennia/game_template/server/conf/server_services_plugins.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/game_template/server/conf/serversession.py` & `evennia-2.0.0/evennia/game_template/server/conf/serversession.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/game_template/server/conf/settings.py` & `evennia-2.0.0/evennia/game_template/server/conf/settings.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/game_template/server/conf/web_plugins.py` & `evennia-2.0.0/evennia/game_template/server/conf/web_plugins.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/game_template/server/logs/README.md` & `evennia-2.0.0/evennia/game_template/server/logs/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/game_template/typeclasses/README.md` & `evennia-2.0.0/evennia/game_template/typeclasses/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/game_template/typeclasses/accounts.py` & `evennia-2.0.0/evennia/game_template/typeclasses/accounts.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/game_template/typeclasses/channels.py` & `evennia-2.0.0/evennia/game_template/typeclasses/channels.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/game_template/typeclasses/characters.py` & `evennia-2.0.0/evennia/game_template/typeclasses/characters.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/game_template/typeclasses/exits.py` & `evennia-2.0.0/evennia/game_template/typeclasses/exits.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/game_template/typeclasses/objects.py` & `evennia-2.0.0/evennia/game_template/typeclasses/objects.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/game_template/typeclasses/rooms.py` & `evennia-2.0.0/evennia/game_template/typeclasses/rooms.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/game_template/typeclasses/scripts.py` & `evennia-2.0.0/evennia/game_template/typeclasses/scripts.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/game_template/web/README.md` & `evennia-2.0.0/evennia/game_template/web/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/game_template/web/admin/urls.py` & `evennia-2.0.0/evennia/game_template/web/admin/urls.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/game_template/web/static/README.md` & `evennia-2.0.0/evennia/game_template/web/static/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/game_template/web/templates/README.md` & `evennia-2.0.0/evennia/game_template/web/templates/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/game_template/web/urls.py` & `evennia-2.0.0/evennia/game_template/web/urls.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/game_template/web/webclient/README.md` & `evennia-2.0.0/evennia/game_template/web/webclient/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/game_template/web/webclient/urls.py` & `evennia-2.0.0/evennia/game_template/web/webclient/urls.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/game_template/web/website/README.md` & `evennia-2.0.0/evennia/game_template/web/website/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/game_template/world/batch_cmds.ev` & `evennia-2.0.0/evennia/game_template/world/batch_cmds.ev`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/game_template/world/help_entries.py` & `evennia-2.0.0/evennia/game_template/world/help_entries.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/game_template/world/prototypes.py` & `evennia-2.0.0/evennia/game_template/world/prototypes.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/help/filehelp.py` & `evennia-2.0.0/evennia/help/filehelp.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/help/manager.py` & `evennia-2.0.0/evennia/help/manager.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/help/migrations/0001_initial.py` & `evennia-2.0.0/evennia/help/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/help/migrations/0002_auto_20170606_1731.py` & `evennia-2.0.0/evennia/help/migrations/0002_auto_20170606_1731.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/help/migrations/0003_auto_20190128_1820.py` & `evennia-2.0.0/evennia/help/migrations/0003_auto_20190128_1820.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/help/migrations/0004_auto_20210520_2137.py` & `evennia-2.0.0/evennia/help/migrations/0004_auto_20210520_2137.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/help/migrations/0005_auto_20210530_1818.py` & `evennia-2.0.0/evennia/help/migrations/0005_auto_20210530_1818.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/help/models.py` & `evennia-2.0.0/evennia/help/models.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/help/tests.py` & `evennia-2.0.0/evennia/help/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/help/utils.py` & `evennia-2.0.0/evennia/help/utils.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/locale/README` & `evennia-2.0.0/evennia/locale/README`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/locale/de/LC_MESSAGES/django.mo` & `evennia-2.0.0/evennia/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/locale/de/LC_MESSAGES/django.po` & `evennia-2.0.0/evennia/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/locale/es/LC_MESSAGES/django.mo` & `evennia-2.0.0/evennia/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/locale/es/LC_MESSAGES/django.po` & `evennia-2.0.0/evennia/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/locale/fr/LC_MESSAGES/django.mo` & `evennia-2.0.0/evennia/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/locale/fr/LC_MESSAGES/django.po` & `evennia-2.0.0/evennia/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/locale/it/LC_MESSAGES/django.mo` & `evennia-2.0.0/evennia/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/locale/it/LC_MESSAGES/django.po` & `evennia-2.0.0/evennia/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/locale/ko/LC_MESSAGES/django.mo` & `evennia-2.0.0/evennia/locale/ko/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/locale/ko/LC_MESSAGES/django.po` & `evennia-2.0.0/evennia/locale/ko/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/locale/la/LC_MESSAGES/django.mo` & `evennia-2.0.0/evennia/locale/la/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/locale/la/LC_MESSAGES/django.po` & `evennia-2.0.0/evennia/locale/la/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/locale/pl/LC_MESSAGES/django.mo` & `evennia-2.0.0/evennia/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/locale/pl/LC_MESSAGES/django.po` & `evennia-2.0.0/evennia/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/locale/pt/LC_MESSAGES/django.mo` & `evennia-2.0.0/evennia/locale/pt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/locale/pt/LC_MESSAGES/django.po` & `evennia-2.0.0/evennia/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/locale/ru/LC_MESSAGES/django.mo` & `evennia-2.0.0/evennia/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/locale/ru/LC_MESSAGES/django.po` & `evennia-2.0.0/evennia/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/locale/sv/LC_MESSAGES/django.mo` & `evennia-2.0.0/evennia/locale/sv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/locale/sv/LC_MESSAGES/django.po` & `evennia-2.0.0/evennia/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/locale/zh/LC_MESSAGES/django.mo` & `evennia-2.0.0/evennia/locale/zh/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/locale/zh/LC_MESSAGES/django.po` & `evennia-2.0.0/evennia/locale/zh/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/locks/lockfuncs.py` & `evennia-2.0.0/evennia/locks/lockfuncs.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/locks/lockhandler.py` & `evennia-2.0.0/evennia/locks/lockhandler.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/locks/tests.py` & `evennia-2.0.0/evennia/locks/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/objects/manager.py` & `evennia-2.0.0/evennia/objects/manager.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/objects/migrations/0001_initial.py` & `evennia-2.0.0/evennia/objects/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/objects/migrations/0002_auto_20140917_0756.py` & `evennia-2.0.0/evennia/objects/migrations/0002_auto_20140917_0756.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/objects/migrations/0003_defaultcharacter_defaultexit_defaultobject_defaultroom.py` & `evennia-2.0.0/evennia/objects/migrations/0003_defaultcharacter_defaultexit_defaultobject_defaultroom.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/objects/migrations/0004_auto_20150118_1622.py` & `evennia-2.0.0/evennia/objects/migrations/0004_auto_20150118_1622.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/objects/migrations/0006_auto_20170606_1731.py` & `evennia-2.0.0/evennia/objects/migrations/0006_auto_20170606_1731.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/objects/migrations/0007_objectdb_db_account.py` & `evennia-2.0.0/evennia/objects/migrations/0007_objectdb_db_account.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/objects/migrations/0008_auto_20170705_1736.py` & `evennia-2.0.0/evennia/objects/migrations/0008_auto_20170705_1736.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/objects/migrations/0009_remove_objectdb_db_player.py` & `evennia-2.0.0/evennia/objects/migrations/0009_remove_objectdb_db_player.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/objects/migrations/0010_auto_20190128_1820.py` & `evennia-2.0.0/evennia/objects/migrations/0010_auto_20190128_1820.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/objects/migrations/0011_auto_20191025_0831.py` & `evennia-2.0.0/evennia/objects/migrations/0011_auto_20191025_0831.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/objects/migrations/0012_convert_contrib_typeclass_paths.py` & `evennia-2.0.0/evennia/objects/migrations/0012_convert_contrib_typeclass_paths.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/objects/models.py` & `evennia-2.0.0/evennia/objects/models.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/objects/objects.py` & `evennia-2.0.0/evennia/objects/objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 This is the v1.0 develop version (for ref in doc building).
 
 """
 import time
 from collections import defaultdict
 
+import evennia
 import inflect
 from django.conf import settings
 from django.utils.translation import gettext as _
 from evennia.commands import cmdset
 from evennia.commands.cmdsethandler import CmdSetHandler
 from evennia.objects.manager import ObjectManager
 from evennia.objects.models import ObjectDB
@@ -32,15 +33,14 @@
     variable_from_module,
 )
 
 _INFLECT = inflect.engine()
 _MULTISESSION_MODE = settings.MULTISESSION_MODE
 
 _ScriptDB = None
-_SESSIONS = None
 _CMDHANDLER = None
 
 _AT_SEARCH_RESULT = variable_from_module(*settings.SEARCH_AT_RESULT.rsplit(".", 1))
 _COMMAND_DEFAULT_CLASS = class_from_module(settings.COMMAND_DEFAULT_CLASS)
 # the sessid_max is based on the length of the db_sessid csv field (excluding commas)
 _SESSID_MAX = 16 if _MULTISESSION_MODE in (1, 3) else 1
 
@@ -63,23 +63,22 @@
 
         """
         self.obj = obj
         self._sessid_cache = []
         self._recache()
 
     def _recache(self):
-        global _SESSIONS
-        if not _SESSIONS:
-            from evennia.server.sessionhandler import SESSIONS as _SESSIONS
         self._sessid_cache = list(
             set(int(val) for val in (self.obj.db_sessid or "").split(",") if val)
         )
-        if any(sessid for sessid in self._sessid_cache if sessid not in _SESSIONS):
+        if any(sessid for sessid in self._sessid_cache if sessid not in evennia.SESSION_HANDLER):
             # cache is out of sync with sessionhandler! Only retain the ones in the handler.
-            self._sessid_cache = [sessid for sessid in self._sessid_cache if sessid in _SESSIONS]
+            self._sessid_cache = [
+                sessid for sessid in self._sessid_cache if sessid in evennia.SESSION_HANDLER
+            ]
             self.obj.db_sessid = ",".join(str(val) for val in self._sessid_cache)
             self.obj.save(update_fields=["db_sessid"])
 
     def get(self, sessid=None):
         """
         Get the sessions linked to this Object.
 
@@ -90,26 +89,25 @@
             sessions (list): The sessions connected to this object. If `sessid` is given,
                 this is a list of one (or zero) elements.
 
         Notes:
             Aliased to `self.all()`.
 
         """
-        global _SESSIONS
-        if not _SESSIONS:
-            from evennia.server.sessionhandler import SESSIONS as _SESSIONS
+
         if sessid:
             sessions = (
-                [_SESSIONS[sessid] if sessid in _SESSIONS else None]
+                [evennia.SESSION_HANDLER[sessid] if sessid in evennia.SESSION_HANDLER else None]
                 if sessid in self._sessid_cache
                 else []
             )
         else:
             sessions = [
-                _SESSIONS[ssid] if ssid in _SESSIONS else None for ssid in self._sessid_cache
+                evennia.SESSION_HANDLER[ssid] if ssid in evennia.SESSION_HANDLER else None
+                for ssid in self._sessid_cache
             ]
         if None in sessions:
             # this happens only if our cache has gone out of sync with the SessionHandler.
 
             return self.get(sessid=sessid)
         return sessions
 
@@ -131,24 +129,21 @@
             session (Session or int): Session or session id to add.
 
         Notes:
             We will only add a session/sessid if this actually also exists
             in the the core sessionhandler.
 
         """
-        global _SESSIONS
-        if not _SESSIONS:
-            from evennia.server.sessionhandler import SESSIONS as _SESSIONS
         try:
             sessid = session.sessid
         except AttributeError:
             sessid = session
 
         sessid_cache = self._sessid_cache
-        if sessid in _SESSIONS and sessid not in sessid_cache:
+        if sessid in evennia.SESSION_HANDLER and sessid not in sessid_cache:
             if len(sessid_cache) >= _SESSID_MAX:
                 return
             sessid_cache.append(sessid)
             self.obj.db_sessid = ",".join(str(val) for val in sessid_cache)
             self.obj.save(update_fields=["db_sessid"])
 
     def remove(self, session):
@@ -765,15 +760,14 @@
 
         contents = self.contents
         if exclude:
             exclude = make_iter(exclude)
             contents = [obj for obj in contents if obj not in exclude]
 
         for receiver in contents:
-
             # actor-stance replacements
             outmessage = _MSG_CONTENTS_PARSER.parse(
                 inmessage,
                 raise_errors=raise_funcparse_errors,
                 return_string=True,
                 caller=you,
                 receiver=receiver,
@@ -1294,15 +1288,15 @@
         """
         Get the 'desc' component of the object description. Called by `return_appearance`.
 
         Args:
             looker (Object): Object doing the looking.
             **kwargs: Arbitrary data for use when overriding.
         Returns:
-            str: The desc display string..
+            str: The desc display string.
 
         """
         return self.db.desc or "You see nothing special."
 
     def get_display_exits(self, looker, **kwargs):
         """
         Get the 'exits' component of the object description. Called by `return_appearance`.
```

### Comparing `evennia-1.3.0/evennia/objects/tests.py` & `evennia-2.0.0/evennia/objects/tests.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from evennia import DefaultCharacter, DefaultExit, DefaultObject, DefaultRoom
 from evennia.objects.models import ObjectDB
-from evennia.objects.objects import DefaultObject
 from evennia.typeclasses.attributes import AttributeProperty
-from evennia.typeclasses.tags import AliasProperty, PermissionProperty, TagProperty
+from evennia.typeclasses.tags import (
+    AliasProperty,
+    PermissionProperty,
+    TagCategoryProperty,
+    TagProperty,
+)
 from evennia.utils import create
 from evennia.utils.test_resources import BaseEvenniaTest, EvenniaTestCase
 
 
 class DefaultObjectTest(BaseEvenniaTest):
-
     ip = "212.216.139.14"
 
     def test_object_create(self):
         description = "A home for a grouch."
         home = self.room1.dbref
 
         obj, errors = DefaultObject.create(
@@ -56,15 +59,18 @@
         obj, errors = DefaultRoom.create("alley", self.account, description=description, ip=self.ip)
         self.assertTrue(obj, errors)
         self.assertFalse(errors, errors)
         self.assertEqual(description, obj.db.desc)
         self.assertEqual(obj.db.creator_ip, self.ip)
 
     def test_exit_create(self):
-        description = "The steaming depths of the dumpster, ripe with refuse in various states of decomposition."
+        description = (
+            "The steaming depths of the dumpster, ripe with refuse in various states of"
+            " decomposition."
+        )
         obj, errors = DefaultExit.create(
             "in", self.room1, self.room2, account=self.account, description=description, ip=self.ip
         )
         self.assertTrue(obj, errors)
         self.assertFalse(errors, errors)
         self.assertEqual(description, obj.db.desc)
         self.assertEqual(obj.db.creator_ip, self.ip)
@@ -275,14 +281,16 @@
     tag1 = TagProperty()
     tag2 = TagProperty(category="tagcategory")
     tag3 = SubTagProperty()
     testalias = AliasProperty()
     testperm = PermissionProperty()
     awaretest = 5
     settest = 0
+    tagcategory1 = TagCategoryProperty("category_tag1")
+    tagcategory2 = TagCategoryProperty("category_tag1", "category_tag2", "category_tag3")
 
     @property
     def base_property(self):
         self.property_initialized = True
 
 
 class TestProperties(EvenniaTestCase):
@@ -295,18 +303,15 @@
         self.obj: TestObjectPropertiesClass = create.create_object(
             TestObjectPropertiesClass, key="testobj"
         )
 
     def tearDown(self):
         self.obj.delete()
 
-    def test_properties(self):
-        """
-        Test all properties assigned at class level.
-        """
+    def test_attribute_properties(self):
         obj = self.obj
 
         self.assertEqual(obj.db.attr1, "attr1")
         self.assertEqual(obj.attributes.get("attr1"), "attr1")
         self.assertEqual(obj.attr1, "attr1")
 
         self.assertEqual(obj.attributes.get("attr2", category="attrcategory"), "attr2")
@@ -322,25 +327,85 @@
         self.assertEqual(obj.attr4, "attr4")
 
         obj.attr3 = "attr3b"  # stores it in db!
 
         self.assertEqual(obj.db.attr3, "attr3b")
         self.assertTrue(obj.attributes.has("attr3"))
 
+    def test_tag_properties(self):
+        obj = self.obj
+
         self.assertTrue(obj.tags.has("tag1"))
         self.assertTrue(obj.tags.has("tag2", category="tagcategory"))
         self.assertTrue(obj.tags.has("tag3"))
 
         self.assertTrue(obj.aliases.has("testalias"))
         self.assertTrue(obj.permissions.has("testperm"))
 
         # Verify that regular properties do not get fetched in init_evennia_properties,
         # only Attribute or TagProperties.
         self.assertFalse(hasattr(obj, "property_initialized"))
 
+    def test_tag_category_properties(self):
+        obj = self.obj
+
+        self.assertFalse(obj.tags.has("category_tag1"))  # no category
+        self.assertTrue(obj.tags.has("category_tag1", category="tagcategory1"))
+        self.assertTrue(obj.tags.has("category_tag1", category="tagcategory2"))
+        self.assertTrue(obj.tags.has("category_tag2", category="tagcategory2"))
+        self.assertTrue(obj.tags.has("category_tag3", category="tagcategory2"))
+
+        self.assertEqual(obj.tagcategory1, ["category_tag1"])
+        self.assertEqual(
+            set(obj.tagcategory2), set(["category_tag1", "category_tag2", "category_tag3"])
+        )
+
+    def test_tag_category_properties_external_modification(self):
+        obj = self.obj
+
+        self.assertEqual(obj.tagcategory1, ["category_tag1"])
+        self.assertEqual(
+            set(obj.tagcategory2), set(["category_tag1", "category_tag2", "category_tag3"])
+        )
+
+        # add extra tag to category
+        obj.tags.add("category_tag2", category="tagcategory1")
+        self.assertEqual(
+            set(obj.tags.get(category="tagcategory1")),
+            set(["category_tag1", "category_tag2"]),
+        )
+        self.assertEqual(set(obj.tagcategory1), set(["category_tag1", "category_tag2"]))
+
+        # add/remove extra tags to category
+        obj.tags.add("category_tag4", category="tagcategory2")
+        obj.tags.remove("category_tag3", category="tagcategory2")
+        self.assertEqual(
+            set(obj.tags.get(category="tagcategory2", return_list=True)),
+            set(["category_tag1", "category_tag2", "category_tag4"]),
+        )
+        # note that when we access the property again, it will be updated to contain the same tags
+        self.assertEqual(
+            set(obj.tagcategory2),
+            set(["category_tag1", "category_tag2", "category_tag3", "category_tag4"]),
+        )
+
+        del obj.tagcategory1
+        # should be deleted from database
+        self.assertEqual(obj.tags.get(category="tagcategory1", return_list=True), [])
+        # accessing the property should return the default value
+        self.assertEqual(obj.tagcategory1, ["category_tag1"])
+
+        del obj.tagcategory2
+        # should be deleted from database
+        self.assertEqual(obj.tags.get(category="tagcategory2", return_list=True), [])
+        # accessing the property should return the default value
+        self.assertEqual(
+            set(obj.tagcategory2), set(["category_tag1", "category_tag2", "category_tag3"])
+        )
+
     def test_object_awareness(self):
         """Test the "object-awareness" of customized AttributeProperty getter/setters"""
         obj = self.obj
 
         # attribute properties receive on obj ref in the getter/setter that can customize return
         self.assertEqual(obj.cusattr, 10)
         self.assertEqual(obj.settest, 5)
```

### Comparing `evennia-1.3.0/evennia/prototypes/README.md` & `evennia-2.0.0/evennia/prototypes/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/prototypes/menus.py` & `evennia-2.0.0/evennia/prototypes/menus.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/prototypes/protfuncs.py` & `evennia-2.0.0/evennia/prototypes/protfuncs.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/prototypes/prototypes.py` & `evennia-2.0.0/evennia/prototypes/prototypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import hashlib
 import time
 
 from django.conf import settings
 from django.core.paginator import Paginator
 from django.db.models import Q
 from django.utils.translation import gettext as _
-
 from evennia.locks.lockhandler import check_lockstring, validate_lockstring
 from evennia.objects.models import ObjectDB
 from evennia.scripts.scripts import DefaultScript
 from evennia.typeclasses.attributes import Attribute
 from evennia.utils import dbserialize, logger
 from evennia.utils.create import create_script
 from evennia.utils.evmore import EvMore
@@ -127,15 +126,15 @@
                             homogenized_tags.append(tag[:3])
 
             elif key == "attrs":
                 attrs = list(prototype.get("attrs", []))  # break reference
                 for attr in attrs:
                     # attrs must be on form [(key, value, category, lockstr)]
                     if not is_iter(attr):
-                        logger.log_error(
+                        logger.log_err(
                             f"Prototype's 'attr' field must be a list of tuples: {prototype}"
                         )
                     elif attr:
                         nattr = len(attr)
                         if nattr == 1:
                             # we assume a None-value
                             homogenized_attrs.append((attr[0], None, None, ""))
@@ -292,15 +291,14 @@
 
     if not mod_or_prototypes:
         # in principle this means PROTOTYPE_MODULES could also contain prototypes, but that is
         # rarely useful ...
         mod_or_prototypes = settings.PROTOTYPE_MODULES
 
     for mod_or_dict in mod_or_prototypes:
-
         if isinstance(mod_or_dict, dict):
             # a single prototype; we must make sure it has its key
             prototype_key = mod_or_dict.get("prototype_key")
             if not prototype_key:
                 raise ValidationError(
                     f"The prototype {mod_or_dict} does not contain a 'prototype_key'"
                 )
@@ -1083,15 +1081,15 @@
         key = "|ckey:|n {key}".format(key=key)
     if "aliases" in prototype:
         aliases = prototype["aliases"]
         aliases = "|caliases:|n {aliases}".format(aliases=", ".join(aliases))
     if "attrs" in prototype:
         attrs = prototype["attrs"]
         out = []
-        for (attrkey, value, category, locks) in attrs:
+        for attrkey, value, category, locks in attrs:
             locks = locks if isinstance(locks, str) else ", ".join(lock for lock in locks if lock)
             category = "|ccategory:|n {}".format(category) if category else ""
             cat_locks = ""
             if category or locks:
                 cat_locks = " (|ccategory:|n {category}, ".format(
                     category=category if category else "|wNone|n"
                 )
@@ -1103,15 +1101,15 @@
                     value=value,
                 )
             )
         attrs = "|cattrs:|n\n {attrs}".format(attrs="\n ".join(out))
     if "tags" in prototype:
         tags = prototype["tags"]
         out = []
-        for (tagkey, category, data) in tags:
+        for tagkey, category, data in tags:
             out.append(
                 "{tagkey} (category: {category}{dat})".format(
                     tagkey=tagkey, category=category, dat=", data: {}".format(data) if data else ""
                 )
             )
         tags = "|ctags:|n\n {tags}".format(tags=", ".join(out))
     if "locks" in prototype:
```

### Comparing `evennia-1.3.0/evennia/prototypes/spawner.py` & `evennia-2.0.0/evennia/prototypes/spawner.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/prototypes/tests.py` & `evennia-2.0.0/evennia/prototypes/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/scripts/manager.py` & `evennia-2.0.0/evennia/scripts/manager.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/scripts/migrations/0001_initial.py` & `evennia-2.0.0/evennia/scripts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/scripts/migrations/0002_auto_20150118_1625.py` & `evennia-2.0.0/evennia/scripts/migrations/0002_auto_20150118_1625.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/scripts/migrations/0003_checksessions_defaultscript_donothing_scriptbase_store_validatechannelhandler_validateidmappercache_.py` & `evennia-2.0.0/evennia/scripts/migrations/0003_checksessions_defaultscript_donothing_scriptbase_store_validatechannelhandler_validateidmappercache_.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/scripts/migrations/0004_auto_20150306_1354.py` & `evennia-2.0.0/evennia/scripts/migrations/0004_auto_20150306_1354.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/scripts/migrations/0006_auto_20150310_2249.py` & `evennia-2.0.0/evennia/scripts/migrations/0006_auto_20150310_2249.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/scripts/migrations/0008_auto_20170606_1731.py` & `evennia-2.0.0/evennia/scripts/migrations/0008_auto_20170606_1731.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/scripts/migrations/0009_scriptdb_db_account.py` & `evennia-2.0.0/evennia/scripts/migrations/0009_scriptdb_db_account.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/scripts/migrations/0010_auto_20170705_1736.py` & `evennia-2.0.0/evennia/scripts/migrations/0010_auto_20170705_1736.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/scripts/migrations/0011_remove_scriptdb_db_player.py` & `evennia-2.0.0/evennia/scripts/migrations/0011_remove_scriptdb_db_player.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/scripts/migrations/0012_auto_20190128_1820.py` & `evennia-2.0.0/evennia/scripts/migrations/0012_auto_20190128_1820.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/scripts/migrations/0013_auto_20191025_0831.py` & `evennia-2.0.0/evennia/scripts/migrations/0013_auto_20191025_0831.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/scripts/migrations/0014_auto_20210520_2137.py` & `evennia-2.0.0/evennia/scripts/migrations/0014_auto_20210520_2137.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/scripts/migrations/0015_convert_contrib_paths.py` & `evennia-2.0.0/evennia/scripts/migrations/0015_convert_contrib_paths.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/scripts/models.py` & `evennia-2.0.0/evennia/scripts/models.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/scripts/monitorhandler.py` & `evennia-2.0.0/evennia/scripts/monitorhandler.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/scripts/scripthandler.py` & `evennia-2.0.0/evennia/scripts/scripthandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 The script handler makes sure to check through all stored scripts to
 make sure they are still relevant. A scripthandler is automatically
 added to all game objects. You access it through the property
 `scripts` on the game object.
 
 """
 from django.utils.translation import gettext as _
-
 from evennia.scripts.models import ScriptDB
 from evennia.utils import create, logger
 
 
 class ScriptHandler(object):
     """
     Implements the handler.  This sits on each game object.
@@ -108,14 +107,27 @@
         scripts = ScriptDB.objects.get_all_scripts_on_obj(self.obj, key=key)
         num = 0
         for script in scripts:
             script.start()
             num += 1
         return num
 
+    def has(self, key):
+        """
+        Determine if a given script exists on this object.
+
+        Args:
+            key (str): Search criterion, the script's key or dbref.
+
+        Returns:
+            bool: If the script exists or not.
+
+        """
+        return ScriptDB.objects.get_all_scripts_on_obj(self.obj, key=key).exists()
+
     def get(self, key):
         """
         Search scripts on this object.
 
         Args:
             key (str): Search criterion, the script's key or dbref.
```

### Comparing `evennia-1.3.0/evennia/scripts/scripts.py` & `evennia-2.0.0/evennia/scripts/scripts.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 This module defines Scripts, out-of-character entities that can store
 data both on themselves and on other objects while also having the
 ability to run timers.
 
 """
 
 from django.utils.translation import gettext as _
-from twisted.internet.defer import Deferred, maybeDeferred
-from twisted.internet.task import LoopingCall
-
 from evennia.scripts.manager import ScriptManager
 from evennia.scripts.models import ScriptDB
 from evennia.typeclasses.models import TypeclassBase
 from evennia.utils import create, logger
+from twisted.internet.defer import Deferred, maybeDeferred
+from twisted.internet.task import LoopingCall
 
 __all__ = ["DefaultScript", "DoNothing", "Store"]
 
 
 class ExtendedLoopingCall(LoopingCall):
     """
     Custom child of LoopingCall that can start at a delay different than
```

### Comparing `evennia-1.3.0/evennia/scripts/taskhandler.py` & `evennia-2.0.0/evennia/scripts/taskhandler.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/scripts/tests.py` & `evennia-2.0.0/evennia/scripts/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/scripts/tickerhandler.py` & `evennia-2.0.0/evennia/scripts/tickerhandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -407,33 +407,29 @@
         if self.ticker_storage:
             # get the current times so the tickers can be restarted with a delay later
             start_delays = dict(
                 (interval, ticker.task.next_call_time())
                 for interval, ticker in self.ticker_pool.tickers.items()
             )
 
-            # remove any subscriptions that lost its object in the interim
-            to_save = {
-                store_key: (args, kwargs)
-                for store_key, (args, kwargs) in self.ticker_storage.items()
-                if (
-                    (
-                        store_key[1]
-                        and ("_obj" in kwargs and kwargs["_obj"].pk)
-                        and hasattr(kwargs["_obj"], store_key[1])
-                    )
-                    or store_key[2]  # a valid method with existing obj
-                )
-            }  # a path given
+            to_save = {}
 
-            # update the timers for the tickers
-            for store_key, (args, kwargs) in to_save.items():
-                interval = store_key[1]
-                # this is a mutable, so it's updated in-place in ticker_storage
-                kwargs["_start_delay"] = start_delays.get(interval, None)
+            # remove any subscription that lost its object and update the timers for the tickers
+            for store_key, (args, kwargs) in self.ticker_storage.items():
+                # unpack the store_key to reference its parts
+                packedobj, callfunc, path, interval, idstring, persistent = store_key
+                # verify that there's a valid obj+method or function path
+                if (
+                    callfunc
+                    and ("_obj" in kwargs and kwargs["_obj"].pk)
+                    and hasattr(kwargs["_obj"], callfunc)
+                ) or path:
+                    # this is a mutable, so it's updated in-place in ticker_storage
+                    kwargs["_start_delay"] = start_delays.get(interval, None)
+                    to_save[store_key] = (args, kwargs)
             ServerConfig.objects.conf(key=self.save_name, value=dbserialize(to_save))
         else:
             # make sure we have nothing lingering in the database
             ServerConfig.objects.conf(key=self.save_name, delete=True)
 
     def restore(self, server_reload=True):
         """
```

### Comparing `evennia-1.3.0/evennia/server/amp_client.py` & `evennia-2.0.0/evennia/server/amp_client.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/server/connection_wizard.py` & `evennia-2.0.0/evennia/server/connection_wizard.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/server/deprecations.py` & `evennia-2.0.0/evennia/server/deprecations.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/server/evennia_launcher.py` & `evennia-2.0.0/evennia/server/evennia_launcher.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/server/game_index_client/README.md` & `evennia-2.0.0/evennia/server/game_index_client/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/server/game_index_client/client.py` & `evennia-2.0.0/evennia/server/game_index_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 from twisted.internet import defer, protocol, reactor
 from twisted.internet.defer import inlineCallbacks
 from twisted.web.client import Agent, HTTPConnectionPool, _HTTP11ClientFactory
 from twisted.web.http_headers import Headers
 from twisted.web.iweb import IBodyProducer
 from zope.interface import implementer
 
+import evennia
 from evennia.accounts.models import AccountDB
-from evennia.server.sessionhandler import SESSIONS
 from evennia.utils import get_evennia_version, logger
 
 _EGI_HOST = "http://evennia-game-index.appspot.com"
 _EGI_REPORT_PATH = "/api/v1/game/check_in"
 
 
 class EvenniaGameIndexClient(object):
@@ -94,15 +94,15 @@
                 "long_description": egi_config.get("long_description", ""),
                 "listing_contact": egi_config["listing_contact"],
                 # How to play
                 "telnet_hostname": egi_config.get("telnet_hostname", ""),
                 "telnet_port": egi_config.get("telnet_port", ""),
                 "web_client_url": egi_config.get("web_client_url", ""),
                 # Game stats
-                "connected_account_count": SESSIONS.account_count(),
+                "connected_account_count": evennia.SESSION_HANDLER.account_count(),
                 "total_account_count": AccountDB.objects.num_total_accounts() or 0,
                 # System info
                 "evennia_version": get_evennia_version(),
                 "python_version": platform.python_version(),
                 "django_version": django.get_version(),
                 "server_platform": platform.platform(),
             }
```

### Comparing `evennia-1.3.0/evennia/server/game_index_client/service.py` & `evennia-2.0.0/evennia/server/game_index_client/service.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/server/initial_setup.py` & `evennia-2.0.0/evennia/server/initial_setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 
 import time
 
 from django.conf import settings
 from django.utils.translation import gettext as _
 
+import evennia
 from evennia.accounts.models import AccountDB
 from evennia.server.models import ServerConfig
 from evennia.utils import create, logger
 
 ERROR_NO_SUPERUSER = """
     No superuser exists yet. The superuser is the 'owner' account on
     the Evennia server. Create a new superuser using the command
@@ -176,18 +177,17 @@
     We end the initialization by resetting the server. This makes sure
     the first login is the same as all the following ones,
     particularly it cleans all caches for the special objects.  It
     also checks so the warm-reset mechanism works as it should.
 
     """
     ServerConfig.objects.conf("server_epoch", time.time())
-    from evennia.server.sessionhandler import SESSIONS
 
     logger.log_info("Initial setup complete. Restarting Server once.")
-    SESSIONS.portal_reset_server()
+    evennia.SESSION_HANDLER.portal_reset_server()
 
 
 def handle_setup(last_step=None):
     """
     Main logic for the module. It allows for restarting the
     initialization at any point if one of the modules should crash.
```

### Comparing `evennia-1.3.0/evennia/server/inputfuncs.py` & `evennia-2.0.0/evennia/server/inputfuncs.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/server/manager.py` & `evennia-2.0.0/evennia/server/manager.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/server/migrations/0001_initial.py` & `evennia-2.0.0/evennia/server/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/server/migrations/0002_auto_20190128_2311.py` & `evennia-2.0.0/evennia/server/migrations/0002_auto_20190128_2311.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/server/models.py` & `evennia-2.0.0/evennia/server/models.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/server/portal/amp.py` & `evennia-2.0.0/evennia/server/portal/amp.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/server/portal/amp_server.py` & `evennia-2.0.0/evennia/server/portal/amp_server.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/server/portal/discord.py` & `evennia-2.0.0/evennia/server/portal/discord.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/server/portal/grapevine.py` & `evennia-2.0.0/evennia/server/portal/grapevine.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/server/portal/irc.py` & `evennia-2.0.0/evennia/server/portal/irc.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/server/portal/mccp.py` & `evennia-2.0.0/evennia/server/portal/mccp.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/server/portal/mssp.py` & `evennia-2.0.0/evennia/server/portal/mssp.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/server/portal/mxp.py` & `evennia-2.0.0/evennia/server/portal/mxp.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/server/portal/naws.py` & `evennia-2.0.0/evennia/server/portal/naws.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/server/portal/portal.py` & `evennia-2.0.0/evennia/server/portal/portal.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 
 django.setup()
 from django.conf import settings
 from django.db import connection
 
 import evennia
 
-evennia._init()
-
+evennia._init(portal_mode=True)
 from evennia.server.portal.portalsessionhandler import PORTAL_SESSIONS
+
 from evennia.server.webserver import EvenniaReverseProxyResource
 from evennia.utils import logger
 from evennia.utils.utils import (
     class_from_module,
     get_evennia_version,
     make_iter,
     mod_import,
```

### Comparing `evennia-1.3.0/evennia/server/portal/portalsessionhandler.py` & `evennia-2.0.0/evennia/server/portal/portalsessionhandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -485,9 +485,9 @@
                         # note that send_default always takes cmdname
                         # as arg too.
                         session.send_default(cmdname, *cmdargs, **cmdkwargs)
                     except Exception:
                         log_trace()
 
 
-_PORTAL_SESSION_HANDLER_CLASS = class_from_module(settings.PORTAL_SESSION_HANDLER_CLASS)
-PORTAL_SESSIONS = _PORTAL_SESSION_HANDLER_CLASS()
+# This will be filled in when the portal boots.
+PORTAL_SESSIONS = None
```

### Comparing `evennia-1.3.0/evennia/server/portal/rss.py` & `evennia-2.0.0/evennia/server/portal/rss.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/server/portal/ssh.py` & `evennia-2.0.0/evennia/server/portal/ssh.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,14 +123,18 @@
         # Clear the previous input line, redraw it at the new
         # cursor position
         self.terminal.eraseDisplay()
         self.terminal.cursorHome()
         self.width = width
         self.height = height
 
+        # Set color defaults
+        for color in ("ANSI", "XTERM256", "TRUECOLOR"):
+            self.protocol_flags[color] = True
+
         # initialize the session
         client_address = self.getClientAddress()
         client_address = client_address.host if client_address else None
         self.init_session("ssh", client_address, self.cfactory.sessionhandler)
 
         # since we might have authenticated already, we might set this here.
         if self.authenticated_account:
```

### Comparing `evennia-1.3.0/evennia/server/portal/ssl.py` & `evennia-2.0.0/evennia/server/portal/ssl.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/server/portal/suppress_ga.py` & `evennia-2.0.0/evennia/server/portal/suppress_ga.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/server/portal/telnet.py` & `evennia-2.0.0/evennia/server/portal/telnet.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/server/portal/telnet_oob.py` & `evennia-2.0.0/evennia/server/portal/telnet_oob.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/server/portal/telnet_ssl.py` & `evennia-2.0.0/evennia/server/portal/telnet_ssl.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/server/portal/tests.py` & `evennia-2.0.0/evennia/server/portal/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/server/portal/ttype.py` & `evennia-2.0.0/evennia/server/portal/ttype.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,18 @@
 # telnet option codes
 TTYPE = bytes([24])  # b"\x18"
 IS = bytes([0])  # b"\x00"
 SEND = bytes([1])  # b"\x01"
 
 # terminal capabilities and their codes
 MTTS = [
+    (2048, "SSL"),
+    (1024, "MSLP"),
+    (512, "MNES"),
+    (256, "TRUECOLOR"),
     (128, "PROXY"),
     (64, "SCREENREADER"),
     (32, "OSC_COLOR_PALETTE"),
     (16, "MOUSE_TRACKING"),
     (8, "XTERM256"),
     (4, "UTF-8"),
     (2, "VT100"),
```

### Comparing `evennia-1.3.0/evennia/server/portal/webclient.py` & `evennia-2.0.0/evennia/server/portal/webclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,14 +127,17 @@
                     self.sessid = old_session.sessid
                     self.sessionhandler.disconnect(old_session)
 
         browserstr = f":{self.browserstr}" if self.browserstr else ""
         self.protocol_flags["CLIENTNAME"] = f"Evennia Webclient (websocket{browserstr})"
         self.protocol_flags["UTF-8"] = True
         self.protocol_flags["OOB"] = True
+        self.protocol_flags["TRUECOLOR"] = True
+        self.protocol_flags["XTERM256"] = True
+        self.protocol_flags["ANSI"] = True
 
         # watch for dead links
         self.transport.setTcpKeepAlive(1)
         # actually do the connection
         self.sessionhandler.connect(self)
 
     def disconnect(self, reason=None):
```

### Comparing `evennia-1.3.0/evennia/server/portal/webclient_ajax.py` & `evennia-2.0.0/evennia/server/portal/webclient_ajax.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/server/profiling/dummyrunner.py` & `evennia-2.0.0/evennia/utils/evform.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,639 +1,560 @@
+# coding=utf-8
 """
-Dummy client runner
+EvForm - a way to create advanced ASCII forms
 
-This module implements a stand-alone launcher for stress-testing
-an Evennia game. It will launch any number of fake clients. These
-clients will log into the server and start doing random operations.
-Customizing and weighing these operations differently depends on
-which type of game is tested. The module contains a testing module
-for plain Evennia.
-
-Please note that you shouldn't run this on a production server!
-Launch the program without any arguments or options to see a
-full step-by-step setup help.
-
-Basically (for testing default Evennia):
-
- - Use an empty/testing database.
- - set PERMISSION_ACCOUNT_DEFAULT = "Builder"
- - start server, eventually with profiling active
- - launch this client runner
-
-If you want to customize the runner's client actions
-(because you changed the cmdset or needs to better
-match your use cases or add more actions), you can
-change which actions by adding a path to
+This is intended for creating advanced ASCII game forms, such as a large pretty character sheet or
+info document.
 
-   DUMMYRUNNER_ACTIONS_MODULE = <path.to.your.module>
+The system works on the basis of a readin template that is given in a separate Python file imported
+into the handler. This file contains some optional settings and a string mapping out the form. The
+template has markers in it to denounce fields to fill. The markers map the absolute size of the
+field and will be filled with an `evtable.EvCell` object when displaying the form.
+
+Example of input file `testform.py`:
+
+```python
+FORMCHAR = "x"
+TABLECHAR = "c"
+
+FORM = '''
+.------------------------------------------------.
+|                                                |
+|  Name: xxxxx1xxxxx    Player: xxxxxxx2xxxxxxx  |
+|        xxxxxxxxxxx                             |
+|                                                |
+ >----------------------------------------------<
+|                                                |
+| Desc:  xxxxxxxxxxx    STR: x4x    DEX: x5x     |
+|        xxxxx3xxxxx    INT: x6x    STA: x7x     |
+|        xxxxxxxxxxx    LUC: x8x    MAG: x9x     |
+|                                                |
+ >----------------------------------------------<
+|          |                                     |
+| cccccccc | ccccccccccccccccccccccccccccccccccc |
+| cccccccc | ccccccccccccccccccccccccccccccccccc |
+| cccAcccc | ccccccccccccccccccccccccccccccccccc |
+| cccccccc | ccccccccccccccccccccccccccccccccccc |
+| cccccccc | cccccccccccccccccBccccccccccccccccc |
+|          |                                     |
+|                                           v&   |
+-------------------------------------------------
+'''
+```
+
+The first line of the `FORM` string is ignored if empty. The forms and table markers must mark out
+complete, unbroken rectangles, each containing one embedded single-character identifier (so the
+smallest element possible is a 3-character wide form). The identifier can be any character except
+for the `FORM_CHAR` and `TABLE_CHAR` and some of the common ASCII-art elements, like space, `_` `|`
+`*` etc (see `INVALID_FORMCHARS` in this module). Form Rectangles can have any size, but must be
+separated from each other by at least one other character's width.
+
+The form can also replace literal markers not abiding by these rules. For example, the `v&` in the
+bottom right corner could be such literal marker. If a literal-mapping for 'v&' is provided, all
+occurrences of this marker will be replaced. This will happen *before* any other parsing, so in
+principle this could be used to inject new fields/tables into the form dynamically.  This literal
+mapping does not consider width, but it will affect to total width of the form, so make sure what
+you inject does not break things.  Using literal markers is the only way to inject 1 or 2-character
+replacements.
+
+Usage
+
+```python
+from evennia import EvForm, EvTable
+
+# create a new form from the template - using the python path
+form = EvForm("path.to.testform")
+
+# alteratively, you can supply the template as a dict:
+
+form = EvForm({"FORM": "....", "TABLECHAR": "c", "FORMCHAR": "x"})
+
+# EvForm can also take a dictionary instead of a filepath, as long
+# as the dict contains the keys FORMCHAR, TABLECHAR and FORM
+# form = EvForm(form=form_dict)
+
+# add data to each tagged form cell
+form.map(cells={1: "Tom the Bouncer",
+                2: "Griatch",
+                3: "A sturdy fellow",
+                4: 12,
+                5: 10,
+                6:  5,
+                7: 18,
+                8: 10,
+                9:  3})
+# create the EvTables
+tableA = EvTable("HP","MV","MP",
+                           table=[["**"], ["*****"], ["***"]],
+                           border="incols")
+tableB = EvTable("Skill", "Value", "Exp",
+                           table=[["Shooting", "Herbalism", "Smithing"],
+                                  [12,14,9],["550/1200", "990/1400", "205/900"]],
+                           border="incols")
+# map 'literal' replacents (here, a version string)
+custom_mapping = {"v&", "v2"}
+
+# add the tables to the proper ids in the form
+form.map(tables={"A": tableA,
+                 "B": tableB})
+
+print(form)
+```
+
+This produces the following result:
+
+::
+
+    .------------------------------------------------.
+    |                                                |
+    |  Name: Tom the        Player: Griatch          |
+    |        Bouncer                                 |
+    |                                                |
+     >----------------------------------------------<
+    |                                                |
+    | Desc:  A sturdy       STR: 12     DEX: 10      |
+    |        fellow         INT: 5      STA: 18      |
+    |                       LUC: 10     MAG: 3       |
+    |                                                |
+     >----------------------------------------------<
+    |          |                                     |
+    | HP|MV|MP | Skill      |Value      |Exp         |
+    | ~~+~~+~~ | ~~~~~~~~~~~+~~~~~~~~~~~+~~~~~~~~~~~ |
+    | **|**|** | Shooting   |12         |550/1200    |
+    |   |**|*  | Herbalism  |14         |990/1400    |
+    |   |* |   | Smithing   |9          |205/900     |
+    |          |                                     |
+    |                                           v2   |
+     ------------------------------------------------
+
+The marked forms have been replaced with EvCells of text and with EvTables. The literal marker `v&`
+was replaced with `v2`.
+
+If you change the form layout on disk, you can use `form.reload()` to re-read it from disk without
+creating a new form.
+
+If you want to update the data of an existing form, you can use `form.map()` with the changes - the
+mappings will be updated, keeping the things you want. You can also update the template itself this
+way, by supplying it as a dict.
+
+Each component (except literal mappings) is restrained to the width and height specified by the
+template, so it will resize to fit (or crop text if the area is too small for it). If you try to fit
+a table into an area it cannot fit into (when including its borders and at least one line of text),
+the form will raise an error.
 
-in your settings. See utils.dummyrunner_actions.py
-for instructions on how to define this module.
+----
 
 """
 
+import re
+from copy import copy
 
-import random
-import sys
-import time
-from argparse import ArgumentParser
-
-import django
-from twisted.conch import telnet
-from twisted.internet import protocol, reactor
-from twisted.internet.task import LoopingCall
-
-django.setup()
-import evennia  # noqa
-
-evennia._init()
-
-from django.conf import settings  # noqa
-
-from evennia.commands.cmdset import CmdSet  # noqa
-from evennia.commands.command import Command  # noqa
-from evennia.utils import mod_import, time_format  # noqa
-from evennia.utils.ansi import strip_ansi  # noqa
-
-# Load the dummyrunner settings module
-
-DUMMYRUNNER_SETTINGS = mod_import(settings.DUMMYRUNNER_SETTINGS_MODULE)
-if not DUMMYRUNNER_SETTINGS:
-    raise IOError(
-        "Error: Dummyrunner could not find settings file at %s"
-        % settings.DUMMYRUNNER_SETTINGS_MODULE
-    )
-IDMAPPER_CACHE_MAXSIZE = settings.IDMAPPER_CACHE_MAXSIZE
-
-DATESTRING = "%Y%m%d%H%M%S"
-CLIENTS = []
-
-# Settings
-
-# number of clients to launch if no input is given on command line
-NCLIENTS = 1
-# time between each 'tick', in seconds, if not set on command
-# line. All launched clients will be called upon to possibly do an
-# action with this frequency.
-TIMESTEP = DUMMYRUNNER_SETTINGS.TIMESTEP
-# chance of a client performing an action, per timestep. This helps to
-# spread out usage randomly, like it would be in reality.
-CHANCE_OF_ACTION = DUMMYRUNNER_SETTINGS.CHANCE_OF_ACTION
-# spread out the login action separately, having many accounts create accounts
-# and connect simultaneously is generally unlikely.
-CHANCE_OF_LOGIN = DUMMYRUNNER_SETTINGS.CHANCE_OF_LOGIN
-# Port to use, if not specified on command line
-TELNET_PORT = DUMMYRUNNER_SETTINGS.TELNET_PORT or settings.TELNET_PORTS[0]
-#
-NCONNECTED = 0  # client has received a connection
-NLOGIN_SCREEN = 0  # client has seen the login screen (server responded)
-NLOGGING_IN = 0  # client starting login procedure
-NLOGGED_IN = 0  # client has authenticated and logged in
-
-# time when all clients have logged_in
-TIME_ALL_LOGIN = 0
-# actions since all logged in
-TOTAL_ACTIONS = 0
-TOTAL_LAG_MEASURES = 0
-# lag per 30s for all logged in
-TOTAL_LAG = 0
-TOTAL_LAG_IN = 0
-TOTAL_LAG_OUT = 0
-
-
-INFO_STARTING = """
-    Dummyrunner starting using {nclients} dummy account(s). If you don't see
-    any connection messages, make sure that the Evennia server is
-    running.
-
-    TELNET_PORT = {port}
-    IDMAPPER_CACHE_MAXSIZE = {idmapper_cache_size} MB
-    TIMESTEP = {timestep} (rate {rate}/s)
-    CHANCE_OF_LOGIN = {chance_of_login}% per time step
-    CHANCE_OF_ACTION = {chance_of_action}% per time step
-    -> avg rate (per client, after login): {avg_rate} cmds/s
-    -> total avg rate (after login): {avg_rate_total} cmds/s
+from evennia.utils.ansi import ANSIString
+from evennia.utils.ansi import raw as ansi_raw
+from evennia.utils.evtable import EvCell, EvTable
+from evennia.utils.utils import all_from_module, is_iter, to_str
+
+# non-valid form-identifying characters (which can thus be
+# used as separators between forms without being detected
+# as an identifier). These should be listed in regex form.
+INVALID_FORMCHARS = r"\s\/\|\\\*\_\-\#\<\>\~\^\:\;\.\,"
+# if there is an ansi-escape (||) we have to replace this with ||| to make sure
+# to properly escape down the line
+_ANSI_ESCAPE = re.compile(r"\|\|")
+
+
+class EvForm:
+    """
+    This object is instantiated with a text file and parses
+    it for rectangular form fields. It can then be fed a
+    mapping so as to populate the fields with fixed-width
+    EvCell or Tables.
+
+    """
+
+    # cell option defaults
+    cell_options = {
+        "pad_left": 0,
+        "pad_right": 0,
+        "pad_top": 0,
+        "pad_bottom": 0,
+        "align": "l",
+        "valign": "t",
+        "enforce_size": True,
+    }
+
+    # table option defaults
+    table_options = {
+        "pad_left": 0,
+        "pad_right": 0,
+        "pad_top": 0,
+        "pad_bottom": 0,
+        "align": "l",
+        "valign": "t",
+        "enforce_size": True,
+    }
+
+    def __init__(self, data=None, cells=None, tables=None, literals=None, **kwargs):
+        """
+        Initiate the form
+
+        Keyword Args:
+            data (str or dict): Path to template file or a dict with
+                "formchar", "tablechar" and "form" keys (not case sensitive, so FORM etc
+                also works, to stay compatible with the in-file names). While "form/FORM"
+                is required, if FORMCHAR/TABLECHAR are not given, they will default to
+                'x' and 'c' respectively.
+            cells (dict): A dictionary mapping  `{id: str}`
+            tables (dict): A dictionary mapping  `{id: EvTable}`.
+            literals (dict): A dictionary mapping `{id: str}`. Will be replaced
+                after width of form is calculated, but before cells/tables are mapped.
+                All occurrences of the identifier on the form will be replaced. Note
+                that there is no length-restriction on the remap, you are responsible
+                for not breaking the form.
+
+        Notes:
+            Other kwargs are fed as options to the EvCells and EvTables
+            (see `evtable.EvCell` and `evtable.EvTable` for more info).
 
-    Use Ctrl-C (or Cmd-C) to stop/disconnect all clients.
-
-    """
-
-ERROR_NO_MIXIN = """
-    Error: Evennia is not set up for dummyrunner. Before starting the
-    server, make sure to include the following at *the end* of your
-    settings file (remove when not using dummyrunner!):
-
-        from evennia.server.profiling.settings_mixin import *
-
-    This will change the settings in the following way:
-        - change PERMISSION_ACCOUNT_DEFAULT to 'Developer' to allow clients
-          to test all commands
-        - change PASSWORD_HASHERS to use a faster (but less safe) algorithm
-          when creating large numbers of accounts at the same time
-        - set LOGIN_THROTTLE/CREATION_THROTTLE=None to disable it
-
-    If you don't want to use the custom settings of the mixin for some
-    reason, you can change their values manually after the import, or
-    add DUMMYRUNNER_MIXIN=True to your settings file to avoid this
-    error completely.
-
-    Warning: Don't run dummyrunner on a production database! It will
-    create a lot of spammy objects and accounts!
-    """
-
-
-ERROR_FEW_ACTIONS = """
-    Dummyrunner settings error: The ACTIONS tuple is too short: it must
-    contain at least login- and logout functions.
-    """
-
-
-HELPTEXT = """
-DO NOT RUN THIS ON A PRODUCTION SERVER! USE A CLEAN/TESTING DATABASE!
-
-This stand-alone program launches dummy telnet clients against a
-running Evennia server. The idea is to mimic real accounts logging in
-and repeatedly doing resource-heavy commands so as to stress test the
-game. It uses the default command set to log in and issue commands, so
-if that was customized, some of the functionality will not be tested
-(it will not fail, the commands will just not be recognized).  The
-running clients will create new objects and rooms all over the place
-as part of their running, so using a clean/testing database is
-strongly recommended.
-
-Setup:
-  1) setup a fresh/clean database (if using sqlite, just safe-copy
-     away your real evennia.db3 file and create a new one with
-     `evennia migrate`)
-  2) in server/conf/settings.py, add
-
-        PERMISSION_ACCOUNT_DEFAULT="Builder"
-
-     This is so that the dummy accounts can test building operations.
-     You can also customize the dummyrunner by modifying a setting
-     file specified by DUMMYRUNNER_SETTINGS_MODULE
-
-  3) Start Evennia like normal, optionally with profiling (--profile)
-  4) Run this dummy runner via the evennia launcher:
-
-        evennia --dummyrunner <nr_of_clients>
-
-  5) Log on and determine if game remains responsive despite the
-     heavier load. Note that if you activated profiling, there is a
-     considerate additional overhead from the profiler too so you
-     should usually not consider game responsivity when using the
-     profiler at the same time.
-  6) If you use profiling, let the game run long enough to gather
-     data, then stop the server cleanly using evennia stop or @shutdown.
-     @shutdown. The profile appears as
-     server/logs/server.prof/portal.prof (see Python's manual on
-     cProfiler).
-
-Notes:
-
-The dummyrunner tends to create a lot of accounts all at once, which is
-a very heavy operation. This is not a realistic use-case - what you want
-to test is performance during run. A large
-number of clients here may lock up the client until all have been
-created. It may be better to connect multiple dummyrunners instead of
-starting one single one with a lot of accounts. Exactly what this number
-is depends on your computer power. So start with 10-20 clients and increase
-until you see the initial login slows things too much.
-
-"""
-
-
-class CmdDummyRunnerEchoResponse(Command):
-    """
-    Dummyrunner command measuring the round-about response time
-    from sending to receiving a result.
-
-    Usage:
-        dummyrunner_echo_response <timestamp>
-
-    Responds with
-        dummyrunner_echo_response:<timestamp>,<current_time>
-
-    The dummyrunner will send this and then compare the send time
-    with the receive time on both ends.
-
-    """
-
-    key = "dummyrunner_echo_response"
-
-    def func(self):
-        # returns (dummy_client_timestamp,current_time)
-        self.msg(f"dummyrunner_echo_response:{self.args},{time.time()}")
-        if self.caller.account.is_superuser:
-            print(f"cmddummyrunner lag in: {time.time() - float(self.args)}s")
-
-
-class DummyRunnerCmdSet(CmdSet):
-    """
-    Dummyrunner injected cmdset.
-
-    """
-
-    def at_cmdset_creation(self):
-        self.add(CmdDummyRunnerEchoResponse())
-
-
-# ------------------------------------------------------------
-# Helper functions
-# ------------------------------------------------------------
-
-
-ICOUNT = 0
-
-
-def idcounter():
-    """
-    Makes unique ids.
-
-    Returns:
-        str: A globally unique id.
-
-    """
-    global ICOUNT
-    ICOUNT += 1
-    return str("{:03d}".format(ICOUNT))
-
-
-GCOUNT = 0
-
-
-def gidcounter():
-    """
-    Makes globally unique ids.
+        """
+        self.indata = data  # storing here so we can reload later in case of a filename
+        self.options = self._parse_inkwargs(**kwargs)
 
-    Returns:
-        count (int); A globally unique counter.
+        self.cells_mapping = (
+            dict((to_str(key), value) for key, value in cells.items()) if cells else {}
+        )
+        self.tables_mapping = (
+            dict((to_str(key), value) for key, value in tables.items()) if tables else {}
+        )
+        self.literals_mapping = (
+            dict((to_str(key), to_str(value)) for key, value in literals.items())
+            if literals
+            else {}
+        )
 
-    """
-    global GCOUNT
-    GCOUNT += 1
-    return "%s_%s" % (time.strftime(DATESTRING), GCOUNT)
+        # work arrays
+        self.literal_form = ""
+        self.mapping = {}
+        self.matrix = []
+        self.form = []
 
+        # will parse and build the form
+        self.reload()
 
-def makeiter(obj):
-    """
-    Makes everything iterable.
+    def _parse_indata(self):
+        """
+        Parse and validate the `self.indata` property. We do this in order to be able to
+        re-load the evform module if indata is a filename and catch any on-file changes.
 
-    Args:
-        obj (any): Object to turn iterable.
+        Returns:
+            dict: The data dict parsed/generated from the in-data.
 
-    Returns:
-        iterable (iterable): An iterable object.
-    """
-    return obj if hasattr(obj, "__iter__") else [obj]
+        """
+        data = self.indata
 
+        default_formchar = "x"
+        default_tablechar = "c"
 
-# ------------------------------------------------------------
-# Client classes
-# ------------------------------------------------------------
+        if isinstance(data, str):
+            # a module path - read all variables from it
+            data = all_from_module(data)
 
+        if isinstance(data, dict):
+            data = {
+                "form": str(data.get("form", data.get("FORM", None))),
+                "formchar": str(data.get("formchar", data.get("FORMCHAR", default_formchar))),
+                "tablechar": str(data.get("tablechar", data.get("TABLECHAR", default_tablechar))),
+            }
+        else:
+            raise RuntimeError(f"EvForm invalid input: {data}.")
 
-class DummyClient(telnet.StatefulTelnetProtocol):
-    """
-    Handles connection to a running Evennia server,
-    mimicking a real account by sending commands on
-    a timer.
+        if not data or data["form"] is None:
+            raise RuntimeError("Evform data must specify a valid 'form' or 'FORM'.")
 
-    """
+        # handle empty or multi-character form/tablechars (not supported)
+        data["formchar"] = data["formchar"][0] if data["formchar"] else default_formchar
+        data["tablechar"] = data["tablechar"][0] if data["tablechar"] else default_tablechar
+        if re.match(rf"[{INVALID_FORMCHARS}]", data["formchar"]):
+            raise RuntimeError(f"Invalid formchar: {data['formchar']}")
+        if re.match(rf"[{INVALID_FORMCHARS}]", data["tablechar"]):
+            raise RuntimeError(f"Invalid tablechar: {data['tablechar']}")
 
-    def report(self, text, clientkey):
-        pad = " " * (25 - len(text))
-        tim = round(time.time() - self.connection_timestamp)
-        print(
-            f"{text} {clientkey}{pad}\t"
-            f"conn: {NCONNECTED} -> "
-            f"welcome screen: {NLOGIN_SCREEN} -> "
-            f"authing: {NLOGGING_IN} -> "
-            f"loggedin/tot: {NLOGGED_IN}/{NCLIENTS} (after {tim}s)"
-        )
+        return data
 
-    def connectionMade(self):
+    def _parse_inkwargs(self, **kwargs):
         """
-        Called when connection is first established.
+        Validate incoming kwargs that will be passed on to become cell/table options.
 
-        """
-        global NCONNECTED
-        # public properties
-        self.cid = idcounter()
-        self.key = f"Dummy-{self.cid}"
-        self.gid = f"{time.strftime(DATESTRING)}_{self.cid}"
-        self.istep = 0
-        self.exits = []  # exit names created
-        self.objs = []  # obj names created
-        self.connection_timestamp = time.time()
-        self.connection_attempt = 0
-        self.action_started = 0
-
-        self._connected = False
-        self._loggedin = False
-        self._logging_out = False
-        self._ready = False
-        self._report = ""
-        self._cmdlist = []  # already stepping in a cmd definition
-        self._login = self.factory.actions[0]
-        self._logout = self.factory.actions[1]
-        self._actions = self.factory.actions[2:]
-
-        reactor.addSystemEventTrigger("before", "shutdown", self.logout)
-
-        NCONNECTED += 1
-        self.report("-> connected", self.key)
-
-        reactor.callLater(30, self._retry_welcome_screen)
-
-    def _retry_welcome_screen(self):
-        if not self._connected and not self._ready:
-            # we have connected but not received anything for 30s.
-            # (unclear why this would be - overload?)
-            # try sending a look to get something to start with
-            self.report("?? retrying welcome screen", self.key)
-            self.sendLine(bytes("look", "utf-8"))
-            # make sure to check again later
-            reactor.callLater(30, self._retry_welcome_screen)
-
-    def _print_statistics(self):
-        global TIME_ALL_LOGIN, TOTAL_ACTIONS
-        global TOTAL_LAG, TOTAL_LAG_MEASURES, TOTAL_LAG_IN, TOTAL_LAG_OUT
-
-        tim = time.time() - TIME_ALL_LOGIN
-        avgrate = round(TOTAL_ACTIONS / tim)
-        lag = TOTAL_LAG / (TOTAL_LAG_MEASURES or 1)
-        lag_in = TOTAL_LAG_IN / (TOTAL_LAG_MEASURES or 1)
-        lag_out = TOTAL_LAG_OUT / (TOTAL_LAG_MEASURES or 1)
-
-        TOTAL_ACTIONS = 0
-        TOTAL_LAG = 0
-        TOTAL_LAG_IN = 0
-        TOTAL_LAG_OUT = 0
-        TOTAL_LAG_MEASURES = 0
-        TIME_ALL_LOGIN = time.time()
-
-        print(
-            f".. running 30s average: ~{avgrate} actions/s "
-            f"lag: {lag:.2}s (in: {lag_in:.2}s, out: {lag_out:.2}s)"
-        )
+        Keyword Args:
+            any: Kwargs to process.
 
-        reactor.callLater(30, self._print_statistics)
+        Returns:
+            dict: A validated/cleaned kwarg to use for options.
 
-    def dataReceived(self, data):
         """
-        Called when data comes in over the protocol. We wait to start
-        stepping until the server actually responds
+        if "filename" in kwargs:
+            raise DeprecationWarning(
+                "EvForm's 'filename' kwarg was renamed to 'data' and can now accept both "
+                "a python path and a dict with 'FORMCHAR', 'TABLECHAR' and 'FORM' keys."
+            )
+        if "form" in kwargs:
+            raise DeprecationWarning(
+                "EvForms's 'form' kwarg was renamed to 'data' and can now accept both "
+                "a python path and a dict detailing the form."
+            )
 
-        Args:
-            data (str): Incoming data.
+        # clean cell kwarg options (these cannot be overridden on the cell but must be controlled
+        # by the evform itself)
+        kwargs.pop("enforce_size", None)
+        kwargs.pop("width", None)
+        kwargs.pop("height", None)
 
-        """
-        global NLOGIN_SCREEN, NLOGGED_IN, NLOGGING_IN, NCONNECTED
-        global TOTAL_ACTIONS, TIME_ALL_LOGIN
-        global TOTAL_LAG, TOTAL_LAG_MEASURES, TOTAL_LAG_IN, TOTAL_LAG_OUT
-
-        if not data.startswith(b"\xff"):
-            # regular text, not a telnet command
-
-            if NCLIENTS == 1:
-                print("dummy-client sees:", str(data, "utf-8"))
-
-            if not self._connected:
-                # waiting for connection
-                # wait until we actually get text back (not just telnet
-                # negotiation)
-                # start client tick
-                d = LoopingCall(self.step)
-                df = max(abs(TIMESTEP * 0.001), min(TIMESTEP / 10, 0.5))
-                # dither next attempt with random time
-                timestep = TIMESTEP + (-df + (random.random() * df))
-                d.start(timestep, now=True).addErrback(self.error)
-                self.connection_attempt += 1
-
-                self._connected = True
-                NLOGIN_SCREEN += 1
-                NCONNECTED -= 1
-                self.report("<- server sent login screen", self.key)
-
-            elif self._loggedin:
-                if not self._ready:
-                    # logged in, ready to run
-                    NLOGGED_IN += 1
-                    NLOGGING_IN -= 1
-                    self._ready = True
-                    self.report("== logged in", self.key)
-                    if NLOGGED_IN == NCLIENTS and not TIME_ALL_LOGIN:
-                        # all are logged in! We can start collecting statistics
-                        print(".. All clients connected and logged in!")
-                        TIME_ALL_LOGIN = time.time()
-                        reactor.callLater(30, self._print_statistics)
-
-                elif TIME_ALL_LOGIN:
-                    TOTAL_ACTIONS += 1
-
-                    try:
-                        data = strip_ansi(str(data, "utf-8").strip())
-                        if data.startswith("dummyrunner_echo_response:"):
-                            # handle special lag-measuring command. This returns
-                            # dummyrunner_echo_response:<starttime>,<midpointtime>
-                            now = time.time()
-                            _, data = data.split(":", 1)
-                            start_time, mid_time = (float(part) for part in data.split(",", 1))
-                            lag_in = mid_time - start_time
-                            lag_out = now - mid_time
-                            total_lag = now - start_time  # full round-about time
-
-                            TOTAL_LAG += total_lag
-                            TOTAL_LAG_IN += lag_in
-                            TOTAL_LAG_OUT += lag_out
-                            TOTAL_LAG_MEASURES += 1
-                    except Exception:
-                        pass
+        return kwargs
 
-    def connectionLost(self, reason):
+    def _do_literal_mapping(self):
         """
-        Called when loosing the connection.
-
-        Args:
-            reason (str): Reason for loosing connection.
+        Do literal replacement in the EvForm.
 
         """
-        if not self._logging_out:
-            self.report("XX lost connection", self.key)
+        literal_form = copy(self.data["form"])
 
-    def error(self, err):
-        """
-        Error callback.
+        for key, repl in self.literals_mapping.items():
+            literal_form = literal_form.replace(key, repl)
+        return literal_form
 
-        Args:
-            err (Failure): Error instance.
+    def _parse_to_matrix(self):
         """
-        print(err)
+        Forces all lines to be as long as the longest line, filling with whitespace.
 
-    def counter(self):
-        """
-        Produces a unique id, also between clients.
+        Args:
+            lines (list): list of `ANSIString`s
 
         Returns:
-            counter (int): A unique counter.
+            (list): list of `ANSIString`s of
+            same length as the longest input line
 
         """
-        return gidcounter()
+        matrix = EvForm._to_ansi(self.literal_form.split("\n"))
 
-    def logout(self):
-        """
-        Causes the client to log out of the server. Triggered by ctrl-c signal.
-
-        """
-        self._logging_out = True
-        cmd = self._logout(self)[0]
-        self.report(f"-> logout/disconnect ({self.istep} actions)", self.key)
-        self.sendLine(bytes(cmd, "utf-8"))
+        maxl = max(len(line) for line in matrix)
+        matrix = [line + " " * (maxl - len(line)) for line in matrix]
+        if matrix and not matrix[0].strip():
+            # the first line is normally empty, we strip it.
+            matrix = matrix[1:]
+        return matrix
+
+    @staticmethod
+    def _to_ansi(obj, regexable=False):
+        "convert anything to ANSIString"
+
+        if isinstance(obj, ANSIString):
+            return obj
+        elif isinstance(obj, str):
+            # since ansi will be parsed twice (here and in the normal ansi send), we have to
+            # escape ansi twice.
+            obj = ansi_raw(obj)
+
+        if isinstance(obj, dict):
+            return dict(
+                (key, EvForm._to_ansi(value, regexable=regexable)) for key, value in obj.items()
+            )
+        # regular _to_ansi (from EvTable)
+        elif is_iter(obj):
+            return [EvForm._to_ansi(o) for o in obj]
+        else:
+            return ANSIString(obj, regexable=regexable)
+
+    def _rectangles_to_mapping(self):
+        """
+        Parse a form for rectangular formfields identified by formchar/tablechar enclosing an
+        identifier.
+
+        """
+        formchar = self.data["formchar"]
+        tablechar = self.data["tablechar"]
+        matrix = self.matrix
+
+        cell_options = copy(self.cell_options)
+        cell_options.update(self.options)
+
+        table_options = copy(self.table_options)
+        table_options.update(self.options)
+
+        nmatrix = len(matrix)
+
+        mapping = {}
+
+        def _get_rectangles(char):
+            """Find all identified rectangles marked with given char"""
+            rects = []
+            coords = {}
+            regex = re.compile(rf"{char}+([^{INVALID_FORMCHARS}{char}]+){char}+")
+
+            # find the start/width of rectangles for each line
+            for iy, line in enumerate(EvForm._to_ansi(matrix, regexable=True)):
+                ix0 = 0
+                while True:
+                    match = regex.search(line, ix0)
+                    if match:
+                        # get the width of the rectangle directly from the match
+                        coords[match.group(1)] = [iy, match.start(), match.end()]
+                        ix0 = match.end()
+                    else:
+                        break
+
+            for key, (iy, leftix, rightix) in coords.items():
+                # scan up to find top of rectangle
+                dy_up = 0
+                if iy > 0:
+                    for i in range(1, iy):
+                        if all(matrix[iy - i][ix] == char for ix in range(leftix, rightix)):
+                            dy_up += 1
+                        else:
+                            break
+                # find bottom edge of rectangle
+                dy_down = 0
+                if iy < nmatrix - 1:
+                    for i in range(1, nmatrix - iy - 1):
+                        if all(matrix[iy + i][ix] == char for ix in range(leftix, rightix)):
+                            dy_down += 1
+                        else:
+                            break
+
+                #  we have our rectangle. Calculate size
+                iyup = iy - dy_up
+                iydown = iy + dy_down
+                width = rightix - leftix
+                height = abs(iyup - iydown) + 1
+
+                # store (key, y, x, width, height) of triangle
+                rects.append((key, iyup, leftix, width, height))
+
+            return rects
+
+        # Map EvCells into form rectangles
+        for (key, y, x, width, height) in _get_rectangles(formchar):
+
+            # get data to populate cell
+            data = self.cells_mapping.get(key, "")
+            if isinstance(data, EvCell):
+                # mapping already provides the cell. We need to override some
+                # of the cell's options to make it work in the evform rectangle.
+                # We retain the align/valign since this may be interesting to
+                # play with within the rectangle.
+                cell = data
+                custom_align = cell.align
+                custom_valign = cell.valign
+                cell.reformat(
+                    width=width,
+                    height=height,
+                    **{**cell_options, **{"align": custom_align, "valign": custom_valign}},
+                )
+            else:
+                # generating cell on the fly
+                cell = EvCell(data, width=width, height=height, **cell_options)
 
-    def step(self):
-        """
-        Perform a step. This is called repeatedly by the runner and
-        causes the client to issue commands to the server.  This holds
-        all "intelligence" of the dummy client.
+            mapping[key] = (y, x, width, height, cell)
 
-        """
-        global NLOGGING_IN, NLOGIN_SCREEN
+        # Map EvTables into form rectangles
+        for (key, y, x, width, height) in _get_rectangles(tablechar):
 
-        rand = random.random()
+            # get EvTable from mapping
+            table = self.tables_mapping.get(key, None)
 
-        if not self._cmdlist:
-            # no commands ready. Load some.
-
-            if not self._loggedin:
-                if rand < CHANCE_OF_LOGIN or NLOGGING_IN < 10:
-                    # lower rate of logins, but not below 1 / s
-                    # get the login commands
-                    self._cmdlist = list(makeiter(self._login(self)))
-                    NLOGGING_IN += 1  # this is for book-keeping
-                    NLOGIN_SCREEN -= 1
-                    self.report("-> create/login", self.key)
-                    self._loggedin = True
-                else:
-                    # no login yet, so cmdlist not yet set
-                    return
+            if table:
+                table.reformat(width=width, height=height, **table_options)
             else:
-                # we always pick a cumulatively random function
-                crand = random.random()
-                cfunc = [func for (cprob, func) in self._actions if cprob >= crand][0]
-                self._cmdlist = list(makeiter(cfunc(self)))
+                table = EvTable(width=width, height=height, **table_options)
 
-        # at this point we always have a list of commands
-        if rand < CHANCE_OF_ACTION:
-            # send to the game
-            cmd = str(self._cmdlist.pop(0))
+            mapping[key] = (y, x, width, height, table)
 
-            if cmd.startswith("dummyrunner_echo_response"):
-                # we need to set the timer element as close to
-                # the send as possible
-                cmd = cmd.format(timestamp=time.time())
+        return mapping
 
-            self.sendLine(bytes(cmd, "utf-8"))
-            self.action_started = time.time()
-            self.istep += 1
+    def _build_form(self):
+        """
+        Insert cell/table contents into form at given locations to create
+        the final result.
 
-            if NCLIENTS == 1:
-                print(f"dummy-client sent: {cmd}")
+        """
+        form = copy(self.matrix)
+        mapping = self.mapping
 
+        for key, (y, x, width, height, cell_or_table) in mapping.items():
 
-class DummyFactory(protocol.ReconnectingClientFactory):
-    protocol = DummyClient
-    initialDelay = 1
-    maxDelay = 1
-    noisy = False
+            # rect is a list of <height> lines, each <width> wide
+            rect = cell_or_table.get()
+            for il, rectline in enumerate(rect):
+                formline = form[y + il]
+                # insert new content, replacing old
+                form[y + il] = formline[:x] + rectline + formline[x + width :]
 
-    def __init__(self, actions):
-        "Setup the factory base (shared by all clients)"
-        self.actions = actions
+        return form
 
+    def reload(self):
+        """
+        Creates the form from a filename or data structure.
 
-# ------------------------------------------------------------
-# Access method:
-# Starts clients and connects them to a running server.
-# ------------------------------------------------------------
+        Args:
+            data (str or dict): Can be used to update an existing form using
+                the same cells/tables provided on initialization or using `.map()`.
 
+        Notes:
+            Kwargs are passed through to Cel creation.
 
-def start_all_dummy_clients(nclients):
-    """
-    Initialize all clients, connect them and start to step them
+        """
+        self.data = self._parse_indata()
 
-    Args:
-        nclients (int): Number of dummy clients to connect.
+        # Map any literals into the string
+        self.literal_form = self._do_literal_mapping()
+        # Create raw form matrix, indexable with (y, x) coords
+        self.matrix = self._parse_to_matrix()
+        # parse and identify all rectangles in the form
+        self.mapping = self._rectangles_to_mapping()
+        # combine mapping with form template into a final result
+        self.form = self._build_form()
 
-    """
-    global NCLIENTS
-    NCLIENTS = int(nclients)
-    actions = DUMMYRUNNER_SETTINGS.ACTIONS
-
-    if len(actions) < 2:
-        print(ERROR_FEW_ACTIONS)
-        return
-
-    # make sure the probabilities add up to 1
-    pratio = 1.0 / sum(tup[0] for tup in actions[2:])
-    flogin, flogout, probs, cfuncs = (
-        actions[0],
-        actions[1],
-        [tup[0] * pratio for tup in actions[2:]],
-        [tup[1] for tup in actions[2:]],
-    )
-    # create cumulative probabilies for the random actions
-    cprobs = [sum(v for i, v in enumerate(probs) if i <= k) for k in range(len(probs))]
-    # rebuild a new, optimized action structure
-    actions = (flogin, flogout) + tuple(zip(cprobs, cfuncs))
-
-    # setting up all clients (they are automatically started)
-    factory = DummyFactory(actions)
-    for i in range(NCLIENTS):
-        reactor.connectTCP("127.0.0.1", TELNET_PORT, factory)
-    # start reactor
-    reactor.run()
-
-
-# ------------------------------------------------------------
-# Command line interface
-# ------------------------------------------------------------
-
-
-if __name__ == "__main__":
-
-    try:
-        settings.DUMMYRUNNER_MIXIN
-    except AttributeError:
-        print(ERROR_NO_MIXIN)
-        sys.exit()
-
-    # parsing command line with default vals
-    parser = ArgumentParser(description=HELPTEXT)
-    parser.add_argument(
-        "-N", nargs=1, default=1, dest="nclients", help="Number of clients to start"
-    )
-
-    args = parser.parse_args()
-    nclients = int(args.nclients[0])
-
-    print(
-        INFO_STARTING.format(
-            nclients=nclients,
-            port=TELNET_PORT,
-            idmapper_cache_size=IDMAPPER_CACHE_MAXSIZE,
-            timestep=TIMESTEP,
-            rate=1 / TIMESTEP,
-            chance_of_login=CHANCE_OF_LOGIN * 100,
-            chance_of_action=CHANCE_OF_ACTION * 100,
-            avg_rate=(1 / TIMESTEP) * CHANCE_OF_ACTION,
-            avg_rate_total=(1 / TIMESTEP) * CHANCE_OF_ACTION * nclients,
+    def map(self, cells=None, tables=None, data=None, literals=None, **kwargs):
+        """
+        Add mapping for form. This allows for updating an existing
+        evform.
+
+        Args:
+            cells (dict): A dictionary of {identifier:celltext}. These
+                will be appended to the existing mappings.
+            tables (dict): A dictionary of {identifier:table}. Will
+                be appended to the existing mapping.
+            data (str or dict): A path to a evform module or a dict with
+                the needed "FORM", "TABLE/FORMCHAR" keys. Will replace
+                the originally initialized form.
+            literals
+
+        Keyword Args:
+            These will be appended to the existing cell/table options.
+
+        Notes:
+            kwargs will be forwarded to tables/cells. See
+            `evtable.EvCell` and `evtable.EvTable` for info.
+
+        """
+        if data:
+            # storing so ._parse_indata will find it during reload
+            self.indata = data
+
+        new_cells = dict((to_str(key), value) for key, value in cells.items()) if cells else {}
+        self.cells_mapping.update(new_cells)
+        new_tables = dict((to_str(key), value) for key, value in tables.items()) if tables else {}
+        self.tables_mapping.update(new_tables)
+        new_literals = (
+            dict((to_str(key), to_str(value)) for key, value in literals.items())
+            if literals
+            else {}
         )
-    )
+        self.literals_mapping.update(new_literals)
+
+        self.options.update(self._parse_inkwargs(**kwargs))
 
-    # run the dummyrunner
-    TIME_START = t0 = time.time()
-    start_all_dummy_clients(nclients=nclients)
-    ttot = time.time() - t0
+        # parse and build the form
+        self.reload()
 
-    # output runtime
-    print("... dummy client runner stopped after %s." % time_format(ttot, style=3))
+    def __str__(self):
+        "Prints the form"
+        return str(ANSIString("\n").join([line for line in self.form]))
```

### Comparing `evennia-1.3.0/evennia/server/profiling/dummyrunner_settings.py` & `evennia-2.0.0/evennia/server/profiling/dummyrunner_settings.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/server/profiling/memplot.py` & `evennia-2.0.0/evennia/server/profiling/memplot.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/server/profiling/settings_mixin.py` & `evennia-2.0.0/evennia/server/profiling/settings_mixin.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/server/profiling/test_queries.py` & `evennia-2.0.0/evennia/server/profiling/test_queries.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/server/profiling/tests.py` & `evennia-2.0.0/evennia/server/profiling/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/server/profiling/timetrace.py` & `evennia-2.0.0/evennia/server/profiling/timetrace.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/server/server.py` & `evennia-2.0.0/evennia/server/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,26 +23,30 @@
 
 import importlib
 
 import evennia
 
 evennia._init()
 
+from evennia.server.sessionhandler import SESSIONS
+
 from django.conf import settings
 from django.db import connection
 from django.db.utils import OperationalError
 from django.utils.translation import gettext as _
 
 from evennia.accounts.models import AccountDB
 from evennia.scripts.models import ScriptDB
 from evennia.server.models import ServerConfig
-from evennia.server.sessionhandler import SESSIONS
+
 from evennia.utils import logger
 from evennia.utils.utils import get_evennia_version, make_iter, mod_import
 
+
+
 _SA = object.__setattr__
 
 # a file with a flag telling the server to restart after shutdown or not.
 SERVER_RESTART = os.path.join(settings.GAME_DIR, "server", "server.restart")
 
 # modules containing hook methods called during start_stop
 SERVER_STARTSTOP_MODULES = [
```

### Comparing `evennia-1.3.0/evennia/server/serversession.py` & `evennia-2.0.0/evennia/server/serversession.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/server/session.py` & `evennia-2.0.0/evennia/server/session.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/server/sessionhandler.py` & `evennia-2.0.0/evennia/server/sessionhandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -870,13 +870,10 @@
                         _INPUT_FUNCS["default"](session, cname, *cmdargs, **cmdkwargs)
                 except Exception as err:
                     if input_debug:
                         session.msg(err)
                     log_trace()
 
 
-# import class from settings
-_SESSION_HANDLER_CLASS = class_from_module(settings.SERVER_SESSION_HANDLER_CLASS)
-
-# Instantiate class. These globals are used to provide singleton-like behavior.
-SESSION_HANDLER = _SESSION_HANDLER_CLASS()
-SESSIONS = SESSION_HANDLER  # legacy
+# These are filled in during server boot.
+SESSION_HANDLER = None
+SESSIONS = None  # legacy
```

### Comparing `evennia-1.3.0/evennia/server/signals.py` & `evennia-2.0.0/evennia/server/signals.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/server/tests/test_amp_connection.py` & `evennia-2.0.0/evennia/server/tests/test_amp_connection.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/server/tests/test_initial_setup.py` & `evennia-2.0.0/evennia/server/tests/test_initial_setup.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/server/tests/test_launcher.py` & `evennia-2.0.0/evennia/server/tests/test_launcher.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/server/tests/test_misc.py` & `evennia-2.0.0/evennia/server/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/server/tests/test_server.py` & `evennia-2.0.0/evennia/server/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/server/tests/testrunner.py` & `evennia-2.0.0/evennia/server/tests/testrunner.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/server/throttle.py` & `evennia-2.0.0/evennia/server/throttle.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/server/validators.py` & `evennia-2.0.0/evennia/server/validators.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/server/webserver.py` & `evennia-2.0.0/evennia/server/webserver.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/settings_default.py` & `evennia-2.0.0/evennia/settings_default.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/typeclasses/attributes.py` & `evennia-2.0.0/evennia/typeclasses/attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,49 +155,51 @@
         pass
 
     value = property(__value_get, __value_set, __value_del)
 
 
 class AttributeProperty:
     """
-    Attribute property descriptor. Allows for specifying Attributes as Django-like 'fields'
-    on the class level. Note that while one can set a lock on the Attribute,
-    there is no way to *check* said lock when accessing via the property - use
-    the full `AttributeHandler` if you need to do access checks. Note however that if you use the
-    full `AttributeHandler` to access this Attribute, the `at_get/at_set` methods on this class will
-    _not_ fire (because you are bypassing the `AttributeProperty` entirely in that case).
-
-    Example:
-    ::
-
-        class Character(DefaultCharacter):
-            foo = AttributeProperty(default="Bar")
+    AttributeProperty.
 
     """
 
     attrhandler_name = "attributes"
 
     def __init__(self, default=None, category=None, strattr=False, lockstring="", autocreate=True):
         """
+        Allows for specifying Attributes as Django-like 'fields' on the class level. Note that while
+        one can set a lock on the Attribute, there is no way to *check* said lock when accessing via
+        the property - use the full `AttributeHandler` if you need to do access checks. Note however
+        that if you use the full `AttributeHandler` to access this Attribute, the `at_get/at_set`
+        methods on this class will _not_ fire (because you are bypassing the `AttributeProperty`
+        entirely in that case).
+
         Initialize an Attribute as a property descriptor.
 
         Keyword Args:
-            default (any): A default value if the attr is not set.
+            default (any): A default value if the attr is not set. If a callable, this will be
+                run without any arguments and is expected to return the default value.
             category (str): The attribute's category. If unset, use class default.
             strattr (bool): If set, this Attribute *must* be a simple string, and will be
                 stored more efficiently.
             lockstring (str): This is not itself useful with the property, but only if
                 using the full AttributeHandler.get(accessing_obj=...) to access the
                 Attribute.
             autocreate (bool): True by default; this means Evennia makes sure to create a new
                 copy of the Attribute (with the default value) whenever a new object with this
                 property is created. If `False`, no Attribute will be created until the property
                 is explicitly assigned a value. This makes it more efficient while it retains
                 its default (there's no db access), but without an actual Attribute generated,
                 one cannot access it via .db, the AttributeHandler or see it with `examine`.
+        Example:
+        ::
+
+            class Character(DefaultCharacter):
+                foo = AttributeProperty(default="Bar")
 
         """
         self._default = default
         self._category = category
         self._strattr = strattr
         self._lockstring = lockstring
         self._autocreate = autocreate
@@ -1386,32 +1388,35 @@
             default_access (bool, optional): Use this permission as
                 fallback if `access_obj` is given but there is no lock of
                 type `attredit` on the Attribute in question.
 
         """
         self.backend.clear_attributes(category, accessing_obj, default_access)
 
-    def all(self, accessing_obj=None, default_access=True):
+    def all(self, category=None, accessing_obj=None, default_access=True):
         """
         Return all Attribute objects on this object, regardless of category.
 
         Args:
+            category (str, optional): A given category to limit results to.
             accessing_obj (object, optional): Check the `attrread`
                 lock on each attribute before returning them. If not
                 given, this check is skipped.
             default_access (bool, optional): Use this permission as a
                 fallback if `accessing_obj` is given but one or more
                 Attributes has no lock of type `attrread` defined on them.
 
         Returns:
             Attributes (list): All the Attribute objects (note: Not
                 their values!) in the handler.
 
         """
         attrs = self.backend.get_all_attributes()
+        if category:
+            attrs = [attr for attr in attrs if attr.category == category]
 
         if accessing_obj:
             return [
                 attr
                 for attr in attrs
                 if attr.access(accessing_obj, self._attrread, default=default_access)
             ]
```

### Comparing `evennia-1.3.0/evennia/typeclasses/managers.py` & `evennia-2.0.0/evennia/typeclasses/managers.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/typeclasses/migrations/0001_initial.py` & `evennia-2.0.0/evennia/typeclasses/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/typeclasses/migrations/0002_auto_20150109_0913.py` & `evennia-2.0.0/evennia/typeclasses/migrations/0002_auto_20150109_0913.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/typeclasses/migrations/0003_defaultcharacter_defaultexit_defaultguest_defaultobject_defaultplayer_defaultroom_defaultscript_dono.py` & `evennia-2.0.0/evennia/typeclasses/migrations/0003_defaultcharacter_defaultexit_defaultguest_defaultobject_defaultplayer_defaultroom_defaultscript_dono.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/typeclasses/migrations/0004_auto_20151101_1759.py` & `evennia-2.0.0/evennia/typeclasses/migrations/0004_auto_20151101_1759.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/typeclasses/migrations/0005_auto_20160625_1812.py` & `evennia-2.0.0/evennia/typeclasses/migrations/0005_auto_20160625_1812.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/typeclasses/migrations/0006_auto_add_dbmodel_value_for_tags_attributes.py` & `evennia-2.0.0/evennia/typeclasses/migrations/0006_auto_add_dbmodel_value_for_tags_attributes.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/typeclasses/migrations/0007_tag_migrations_may_be_slow.py` & `evennia-2.0.0/evennia/typeclasses/migrations/0007_tag_migrations_may_be_slow.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/typeclasses/migrations/0008_lock_and_perm_rename.py` & `evennia-2.0.0/evennia/typeclasses/migrations/0008_lock_and_perm_rename.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/typeclasses/migrations/0009_rename_player_cmdsets_typeclasses.py` & `evennia-2.0.0/evennia/typeclasses/migrations/0009_rename_player_cmdsets_typeclasses.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/typeclasses/migrations/0010_delete_old_player_tables.py` & `evennia-2.0.0/evennia/typeclasses/migrations/0010_delete_old_player_tables.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/typeclasses/migrations/0011_auto_20190128_1820.py` & `evennia-2.0.0/evennia/typeclasses/migrations/0011_auto_20190128_1820.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/typeclasses/migrations/0012_attrs_to_picklev4_may_be_slow.py` & `evennia-2.0.0/evennia/typeclasses/migrations/0012_attrs_to_picklev4_may_be_slow.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/typeclasses/migrations/0013_auto_20191015_1922.py` & `evennia-2.0.0/evennia/typeclasses/migrations/0013_auto_20191015_1922.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/typeclasses/migrations/0014_alter_tag_db_category.py` & `evennia-2.0.0/evennia/typeclasses/migrations/0014_alter_tag_db_category.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/typeclasses/migrations/0016_alter_attribute_id_alter_tag_id.py` & `evennia-2.0.0/evennia/typeclasses/migrations/0016_alter_attribute_id_alter_tag_id.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/typeclasses/models.py` & `evennia-2.0.0/evennia/typeclasses/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 from django.core.exceptions import ObjectDoesNotExist
 from django.db import models
 from django.db.models import signals
 from django.db.models.base import ModelBase
 from django.urls import reverse
 from django.utils.encoding import smart_str
 from django.utils.text import slugify
-
 from evennia.locks.lockhandler import LockHandler
 from evennia.server.signals import SIGNAL_TYPED_OBJECT_POST_RENAME
 from evennia.typeclasses import managers
 from evennia.typeclasses.attributes import (
     Attribute,
     AttributeHandler,
     AttributeProperty,
@@ -46,14 +45,15 @@
     InMemoryAttributeBackend,
     ModelAttributeBackend,
 )
 from evennia.typeclasses.tags import (
     AliasHandler,
     PermissionHandler,
     Tag,
+    TagCategoryProperty,
     TagHandler,
     TagProperty,
 )
 from evennia.utils.idmapper.models import SharedMemoryModel, SharedMemoryModelBase
 from evennia.utils.logger import log_trace
 from evennia.utils.utils import class_from_module, inherits_from, is_iter, lazy_property
 
@@ -339,15 +339,15 @@
 
     def init_evennia_properties(self):
         """
         Called by creation methods; makes sure to initialize Attribute/TagProperties
         by fetching them once.
         """
         for propkey, prop in self.__class__.__dict__.items():
-            if isinstance(prop, (AttributeProperty, TagProperty)):
+            if isinstance(prop, (AttributeProperty, TagProperty, TagCategoryProperty)):
                 try:
                     getattr(self, propkey)
                 except Exception:
                     log_trace()
 
     # initialize all handlers in a lazy fashion
     @lazy_property
@@ -622,15 +622,16 @@
         # if we get to this point, the class is ok.
 
         if inherits_from(self, "evennia.scripts.models.ScriptDB"):
             if self.interval > 0:
                 raise RuntimeError(
                     "Cannot use swap_typeclass on time-dependent "
                     "Script '%s'.\nStop and start a new Script of the "
-                    "right type instead." % self.key
+                    "right type instead."
+                    % self.key
                 )
 
         self.typeclass_path = new_typeclass.path
         self.__class__ = new_typeclass
 
         if clean_attributes:
             # Clean out old attributes
```

### Comparing `evennia-1.3.0/evennia/typeclasses/tags.py` & `evennia-2.0.0/evennia/typeclasses/tags.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 respective handlers.
 
 """
 from collections import defaultdict
 
 from django.conf import settings
 from django.db import models
-
 from evennia.locks.lockfuncs import perm as perm_lockfunc
 from evennia.utils.utils import make_iter, to_str
 
 _TYPECLASS_AGGRESSIVE_CACHE = settings.TYPECLASS_AGGRESSIVE_CACHE
 
 # ------------------------------------------------------------
 #
@@ -95,36 +94,39 @@
 #
 # Handlers making use of the Tags model
 #
 
 
 class TagProperty:
     """
-    Tag property descriptor. Allows for setting tags on an object as Django-like 'fields'
-    on the class level. Since Tags are almost always used for querying, Tags are always
-    created/assigned along with the object. Make sure the property/tagname does not collide
-    with an existing method/property on the class. If it does, you must use tags.add()
-    instead.
-
-    Note that while you _can_ check e.g. `obj.tagname,this will give an AttributeError
-    if the Tag is not set. Most often you want to use `obj.tags.get("tagname")` to check
-    if a tag is set on an object.
-
-    Example:
-    ::
-
-            class Character(DefaultCharacter):
-                mytag = TagProperty()  # category=None
-                mytag2 = TagProperty(category="tagcategory")
-
+    Tag Property.
     """
 
     taghandler_name = "tags"
 
     def __init__(self, category=None, data=None):
+        """
+        Tag property descriptor. Allows for setting tags on an object as Django-like 'fields'
+        on the class level. Since Tags are almost always used for querying, Tags are always
+        created/assigned along with the object. Make sure the property/tagname does not collide
+        with an existing method/property on the class. If it does, you must use tags.add()
+        instead.
+
+        Note that while you _can_ check e.g. `obj.tagname,this will give an AttributeError
+        if the Tag is not set. Most often you want to use `obj.tags.get("tagname")` to check
+        if a tag is set on an object.
+
+        Example:
+        ::
+
+                class Character(DefaultCharacter):
+                    mytag = TagProperty()  # category=None
+                    mytag2 = TagProperty(category="tagcategory")
+        """
+
         self._category = category
         self._data = data
         self._key = ""
 
     def __set_name__(self, cls, name):
         """
         Called when descriptor is first assigned to the class (not the instance!).
@@ -163,14 +165,128 @@
         the Tag. Note that the tag will be readded on next fetch unless the
         TagProperty is also removed in code!
 
         """
         getattr(instance, self.taghandler_name).remove(key=self._key, category=self._category)
 
 
+class TagCategoryProperty:
+    """
+    Tag Category Property.
+
+    """
+
+    taghandler_name = "tags"
+
+    def __init__(self, *default_tags):
+        """
+        Assign a property for a Tag Category, with any number of Tag keys.
+        This is often more useful than the `TagProperty` since it's common to want to check which
+        tags of a particular category the object is a member of.
+
+        Args:
+            *args (str or callable): Tag keys to assign to this property, using the category given
+                by the name of the property. Note that, if these tags are always set on the object,
+                if they are removed by some other means, they will be re-added when this property
+                is accessed. Furthermore, changing this list after the object was created, will
+                not remove any old tags (there is no way for the property to know if the
+                new list is new or not).  If a callable, it will be called without arguments to
+                return the tag key. It is not possible to set tag `data` this way (use the
+                Taghandler directly for that). Tag keys are not case sensitive.
+
+        Raises:
+            ValueError: If the input is not a valid tag key or tuple.
+
+        Notes:
+            It is not possible to set Tags with a `None` category using a `TagCategoryProperty` -
+            use `obj.tags.add()` instead.
+
+        Example:
+        ::
+
+                class RogueCharacter(DefaultCharacter):
+                    guild = TagProperty("thieves_guild", "merchant_guild")
+
+        """
+        self._category = ""
+        self._default_tags = self._parse_tag_input(*default_tags)
+
+    def _parse_tag_input(self, *args):
+        """
+        Parse input to the property.
+
+        Args:
+            *args (str or callable): Tags, either as strings or `callable`, which should return
+            the tag key when called without arguments. Keys are not case sensitive.
+
+        Returns:
+            list: A list of tag keys.
+
+        """
+        tags = []
+        for tagkey in args:
+            if callable(tagkey):
+                tagkey = tagkey()
+            tags.append((str(tagkey).lower()))
+        return tags
+
+    def __set_name__(self, cls, name):
+        """
+        Called when descriptor is first assigned to the class (not the instance!).
+        It is called with the name of the field.
+
+        """
+        self._category = name
+
+    def __get__(self, instance, owner):
+        """
+        Called when accessing the tag as a property on the instance. Returns a list
+        of tags under the given category.
+        """
+        taghandler = getattr(instance, self.taghandler_name)
+
+        default_tags = self._default_tags
+        tags = taghandler.get(category=self._category, return_list=True)
+
+        missing_default_tags = set(default_tags) - set(tags)
+
+        if missing_default_tags:
+            getattr(instance, self.taghandler_name).batch_add(
+                *[(tag, self._category) for tag in missing_default_tags]
+            )
+
+            tags += missing_default_tags  # to avoid a second db call
+
+        return tags
+
+    def __set__(self, instance, *args):
+        """
+        Assign a new set of tags to the category. Note that we can't know if previous
+        tags were assigned from this property or from TagHandler, so we don't
+        remove old tags. To refresh to only have the tags in this constructor, first
+        use `del` on this property and re-access the property with the changed default list.
+
+        """
+        getattr(instance, self.taghandler_name).batch_add(*[(tag, self._category) for tag in args])
+
+    def __delete__(self, instance):
+        """
+        Called when running `del` on the property. Will remove all tags of this
+        category from the object. Note that next time this desriptor is accessed, the
+        default ones will be re-added!
+
+        Note:
+            This will remove _all_ tags of this category from the object. This is necessary
+            in order to be able to be able to combine this with `__set__` to get a tag
+            list where property and handler are in sync.
+
+        """
+        getattr(instance, self.taghandler_name).remove(category=self._category)
+
+
 class TagHandler(object):
     """
     Generic tag-handler. Accessed via TypedObject.tags.
 
     """
 
     _m2m_fieldname = "db_tags"
@@ -597,24 +713,45 @@
 
         """
         keys = defaultdict(list)
         data = {}
         for tup in args:
             tup = make_iter(tup)
             nlen = len(tup)
-            if nlen == 1:  # just a key
+            if nlen == 1:  # just a key, no category
                 keys[None].append(tup[0])
             elif nlen == 2:
                 keys[tup[1]].append(tup[0])
             else:
                 keys[tup[1]].append(tup[0])
                 data[tup[1]] = tup[2]  # overwrite previous
         for category, key in keys.items():
             self.add(key=key, category=category, data=data.get(category, None))
 
+    def batch_remove(self, *args):
+        """
+        Batch-remove tags from a list of tuples.
+
+        Args:
+            *args (tuple or str): Each argument should be a `tagstr` keys or tuple
+                `(keystr, category)` or `(keystr, category, data)` (the `data` field is ignored,
+                only `keystr`/`category` matters). It's possible to mix input types.
+
+        """
+        keys = defaultdict(list)
+        for tup in args:
+            tup = make_iter(tup)
+            nlen = len(tup)
+            if nlen == 1:  # just a key, no category
+                keys[None].append(tup[0])
+            elif nlen > 1:
+                keys[tup[1]].append(tup[0])
+        for category, key in keys.items():
+            self.remove(key=key, category=category, data=data.get(category, None))
+
     def __str__(self):
         return ",".join(self.all())
 
 
 class AliasProperty(TagProperty):
     """
     Allows for setting aliases like Django fields:
```

### Comparing `evennia-1.3.0/evennia/typeclasses/tests.py` & `evennia-2.0.0/evennia/typeclasses/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/utils/ansi.py` & `evennia-2.0.0/evennia/utils/ansi.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/utils/batchprocessors.py` & `evennia-2.0.0/evennia/utils/batchprocessors.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/utils/containers.py` & `evennia-2.0.0/evennia/utils/containers.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/utils/create.py` & `evennia-2.0.0/evennia/utils/create.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/utils/dbserialize.py` & `evennia-2.0.0/evennia/utils/dbserialize.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     from pickle import UnpicklingError, dumps, loads
 except ImportError:
     from pickle import dumps, loads
 
 from django.contrib.contenttypes.models import ContentType
 from django.core.exceptions import ObjectDoesNotExist
 from django.utils.safestring import SafeString
+import evennia
 from evennia.utils import logger
 from evennia.utils.utils import is_iter, to_bytes, uses_database
 
 __all__ = ("to_pickle", "from_pickle", "do_pickle", "do_unpickle", "dbserialize", "dbunserialize")
 
 PICKLE_PROTOCOL = 2
 
@@ -67,15 +68,14 @@
 
 
 _GA = object.__getattribute__
 _SA = object.__setattr__
 _FROM_MODEL_MAP = None
 _TO_MODEL_MAP = None
 _IGNORE_DATETIME_MODELS = None
-_SESSION_HANDLER = None
 
 
 def _IS_PACKED_DBOBJ(o):
     return isinstance(o, tuple) and len(o) == 4 and o[0] == "__packed_dbobj__"
 
 
 def _IS_PACKED_SESSION(o):
@@ -110,32 +110,29 @@
             # we have received a None object, for example due to an erroneous save.
             return None
         return _GA(obj, "db_date_created").strftime(_DATESTRING)
 
 
 def _init_globals():
     """Lazy importing to avoid circular import issues"""
-    global _FROM_MODEL_MAP, _TO_MODEL_MAP, _SESSION_HANDLER, _IGNORE_DATETIME_MODELS
+    global _FROM_MODEL_MAP, _TO_MODEL_MAP, _IGNORE_DATETIME_MODELS
     if not _FROM_MODEL_MAP:
         _FROM_MODEL_MAP = defaultdict(str)
         _FROM_MODEL_MAP.update(dict((c.model, c.natural_key()) for c in ContentType.objects.all()))
     if not _TO_MODEL_MAP:
         from django.conf import settings
 
         _TO_MODEL_MAP = defaultdict(str)
         _TO_MODEL_MAP.update(
             dict((c.natural_key(), c.model_class()) for c in ContentType.objects.all())
         )
         _IGNORE_DATETIME_MODELS = []
         for src_key, dst_key in settings.ATTRIBUTE_STORED_MODEL_RENAME:
             _TO_MODEL_MAP[src_key] = _TO_MODEL_MAP.get(dst_key, None)
             _IGNORE_DATETIME_MODELS.append(src_key)
-    if not _SESSION_HANDLER:
-        from evennia.server.sessionhandler import SESSION_HANDLER as _SESSION_HANDLER
-
 
 #
 # SaverList, SaverDict, SaverSet - Attribute-specific helper classes and functions
 #
 
 
 def _save(method):
@@ -605,15 +602,15 @@
     Returns:
         packed (tuple or None): A session-packed tuple on the form
             `(__packed_session__, sessid, conn_time)`. If this sessid
             does not match a session in the Session handler, None is returned.
 
     """
     _init_globals()
-    session = _SESSION_HANDLER.get(item.sessid)
+    session = evennia.SESSION_HANDLER.get(item.sessid)
     if session and session.conn_time == item.conn_time:
         # we require connection times to be identical for the Session
         # to be accepted as actually being a session (sessids gets
         # reused all the time).
         return (
             item.conn_time
             and item.sessid
@@ -632,15 +629,15 @@
 
     Returns:
         unpacked (any): Either the original input or converts the
             internal store back to a Session. If Session no longer
             exists, None will be returned.
     """
     _init_globals()
-    session = _SESSION_HANDLER.get(item[1])
+    session = evennia.SESSION_HANDLER.get(item[1])
     if session and session.conn_time == item[2]:
         # we require connection times to be identical for the Session
         # to be accepted as the same as the one stored (sessids gets
         # reused all the time).
         return session
     return None
```

### Comparing `evennia-1.3.0/evennia/utils/eveditor.py` & `evennia-2.0.0/evennia/utils/eveditor.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/utils/evennia-mode.el` & `evennia-2.0.0/evennia/utils/evennia-mode.el`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/utils/evmenu.py` & `evennia-2.0.0/evennia/utils/evmenu.py`

 * *Files 0% similar despite different names*

```diff
@@ -358,14 +358,29 @@
     locks = "cmd:all()"
     help_category = "Menu"
     auto_help_display_key = "<menu commands>"
 
     def get_help(self):
         return "Menu commands are explained within the menu."
 
+    def _update_aliases(self, menu):
+        """Add aliases to make sure to override defaults if we defined we want it."""
+
+        new_aliases = [_CMD_NOMATCH]
+        if menu.auto_quit and "quit" not in self.aliases:
+            new_aliases.extend(["q", "quit"])
+        if menu.auto_look and "look" not in self.aliases:
+            new_aliases.extend(["l", "look"])
+        if menu.auto_help and "help" not in self.aliases:
+            new_aliases.extend(["h", "help"])
+        if len(new_aliases) > 1:
+            self.set_aliases(new_aliases)
+
+        self.msg(f"aliases: {self.aliases}")
+
     def func(self):
         """
         Implement all menu commands.
         """
 
         def _restore(caller):
             # check if there is a saved menu available.
@@ -378,15 +393,16 @@
                 except ValueError:  # old form of startnode store
                     startnode, startnode_input = startnode_tuple, ""
                 if startnode:
                     saved_options[2]["startnode"] = startnode
                     saved_options[2]["startnode_input"] = startnode_input
                 MenuClass = saved_options[0]
                 # this will create a completely new menu call
-                MenuClass(caller, *saved_options[1], **saved_options[2])
+                menu = MenuClass(caller, *saved_options[1], **saved_options[2])
+                # self._update_aliases(menu)
                 return True
             return None
 
         caller = self.caller
         # we store Session on the menu since this can be hard to
         # get in multisession environments if caller is an Account.
         menu = caller.ndb._evmenu
@@ -404,14 +420,17 @@
                 if not menu:
                     # can't restore from a session
                     err = "Menu object not found as %s.ndb._evmenu!" % orig_caller
                     orig_caller.msg(
                         err
                     )  # don't give the session as a kwarg here, direct to original
                     raise EvMenuError(err)
+
+        # self._update_aliases(menu)
+
         # we must do this after the caller with the menu has been correctly identified since it
         # can be either Account, Object or Session (in the latter case this info will be
         # superfluous).
         caller.ndb._evmenu._session = self.session
         # we have a menu, use it.
         menu.parse_input(self.raw_string)
 
@@ -533,15 +552,15 @@
                 for the very first display of the first node - after that, EvMenu itself
                 will keep the session updated from the command input. So a persistent
                 menu will *not* be using this same session anymore after a reload.
             debug (bool, optional): If set, the 'menudebug' command will be made available
                 by default in all nodes of the menu. This will print out the current state of
                 the menu. Deactivate for production use! When the debug flag is active, the
                 `persistent` flag is deactivated.
-            **kwargs: All kwargs will become initialization variables on `caller.ndb._menutree`,
+            **kwargs: All kwargs will become initialization variables on `caller.ndb._evmenu`,
                 to be available at run.
 
         Raises:
             EvMenuError: If the start/end node is not found in menu tree.
 
         Notes:
             While running, the menu is stored on the caller as `caller.ndb._evmenu`. Also
@@ -627,15 +646,15 @@
                 self.caller.ndb._evmenu.close_menu()
             except Exception:
                 pass
 
         # store ourself on the object
         self.caller.ndb._evmenu = self
 
-        # DEPRECATED - for backwards-compatibility. Use `.ndb._evmenu` instead
+        # TODO DEPRECATED - for backwards-compatibility. Use `.ndb._evmenu` instead
         self.caller.ndb._menutree = self
 
         if persistent:
             # save the menu to the database
             calldict = {
                 "startnode": startnode,
                 "cmdset_mergetype": cmdset_mergetype,
@@ -866,14 +885,17 @@
                     raise EvMenuError(
                         "{}: goto callable must return str or (str, dict)".format(inp_nodename)
                     )
                 nodename, kwargs = nodename[:2]
             if not nodename:
                 # no nodename return. Re-run current node
                 nodename = self.nodename
+        elif nodename_or_callable is None:
+            # repeat current node
+            nodename = self.nodename
         else:
             # the nodename given directly
             nodename = nodename_or_callable
 
         # one way or another, we have the nodename as a string now
 
         try:
@@ -911,15 +933,14 @@
         self.options = {}
         self.default = None
         display_options = []  # options will be displayed in this order
 
         if options:
             options = [options] if isinstance(options, dict) else options
             for inum, dic in enumerate(options):
-
                 # homogenize the options dict
                 keys = make_iter(dic.get("key"))
                 desc = dic.get("desc", dic.get("text", None))
 
                 if "_default" in keys:
                     keys = [key for key in keys if key != "_default"]
                     goto, goto_kwargs = self._extract_goto(nodename, dic)
@@ -949,14 +970,15 @@
         Shutdown menu; occurs when reaching the end node or using the quit command.
         """
         if not self._quitting:
             # avoid multiple calls from different sources
             self._quitting = True
             self.caller.cmdset.remove(EvMenuCmdSet)
             del self.caller.ndb._evmenu
+            del self.caller.ndb._menutree  # TODO Deprecated
             if self._persistent:
                 self.caller.attributes.remove("_menutree_saved")
                 self.caller.attributes.remove("_menutree_saved_startnode")
             if self.cmd_on_exit is not None:
                 self.cmd_on_exit(self.caller, self)
             # special for template-generated menues
             del self.caller.db._evmenu_template_contents
@@ -1303,15 +1325,14 @@
                     # to pass on to the next node
                     kwargs["selection"] = selection
                     return str(select), kwargs
             # this means the previous node will be re-run with these same kwargs
             return None, kwargs
 
         def _list_node(caller, raw_string, **kwargs):
-
             option_list = (
                 option_generator(caller) if callable(option_generator) else option_generator
             )
 
             npages = 0
             page_index = 0
             page = []
```

### Comparing `evennia-1.3.0/evennia/utils/evmore.py` & `evennia-2.0.0/evennia/utils/evmore.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/utils/evtable.py` & `evennia-2.0.0/evennia/utils/evtable.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/utils/funcparser.py` & `evennia-2.0.0/evennia/utils/funcparser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1485,8 +1485,9 @@
     "you": funcparser_callable_you,
     "You": funcparser_callable_you_capitalize,
     "obj": funcparser_callable_you,
     "Obj": funcparser_callable_you_capitalize,
     "conj": funcparser_callable_conjugate,
     "pron": funcparser_callable_pronoun,
     "Pron": funcparser_callable_pronoun_capitalize,
+    **FUNCPARSER_CALLABLES,
 }
```

### Comparing `evennia-1.3.0/evennia/utils/gametime.py` & `evennia-2.0.0/evennia/utils/gametime.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 import time
 from datetime import datetime, timedelta
 
 from django.conf import settings
 from django.db.utils import OperationalError
 
+import evennia
 from evennia import DefaultScript
 from evennia.server.models import ServerConfig
 from evennia.utils.create import create_script
 
 # Speed-up factor of the in-game time compared
 # to real time.
 
@@ -121,17 +122,16 @@
 def portal_uptime():
     """
     Get the current uptime of the portal.
 
     Returns:
         time (float): The uptime of the portal.
     """
-    from evennia.server.sessionhandler import SESSIONS
 
-    return time.time() - SESSIONS.portal_start_time
+    return time.time() - evennia.SESSION_HANDLER.portal_start_time
 
 
 def game_epoch():
     """
     Get the game epoch.
 
     """
```

### Comparing `evennia-1.3.0/evennia/utils/idmapper/LICENSE.md` & `evennia-2.0.0/evennia/utils/idmapper/LICENSE.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/utils/idmapper/README_evennia.md` & `evennia-2.0.0/evennia/utils/idmapper/README_evennia.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/utils/idmapper/README_orig.rst` & `evennia-2.0.0/evennia/utils/idmapper/README_orig.rst`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/utils/idmapper/manager.py` & `evennia-2.0.0/evennia/utils/idmapper/manager.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/utils/idmapper/models.py` & `evennia-2.0.0/evennia/utils/idmapper/models.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/utils/idmapper/tests.py` & `evennia-2.0.0/evennia/utils/idmapper/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/utils/logger.py` & `evennia-2.0.0/evennia/utils/logger.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/utils/optionclasses.py` & `evennia-2.0.0/evennia/utils/optionclasses.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/utils/optionhandler.py` & `evennia-2.0.0/evennia/utils/optionhandler.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/utils/picklefield.py` & `evennia-2.0.0/evennia/utils/picklefield.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/utils/search.py` & `evennia-2.0.0/evennia/utils/search.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/utils/test_resources.py` & `evennia-2.0.0/evennia/utils/test_resources.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,27 +27,27 @@
 import types
 
 from django.conf import settings
 from django.test import TestCase, override_settings
 from mock import MagicMock, Mock, patch
 from twisted.internet.defer import Deferred
 
+import evennia
 from evennia import settings_default
 from evennia.accounts.accounts import DefaultAccount
 from evennia.commands.command import InterruptCommand
 from evennia.commands.default.muxcommand import MuxCommand
 from evennia.objects.objects import (
     DefaultCharacter,
     DefaultExit,
     DefaultObject,
     DefaultRoom,
 )
 from evennia.scripts.scripts import DefaultScript
 from evennia.server.serversession import ServerSession
-from evennia.server.sessionhandler import SESSIONS
 from evennia.utils import ansi, create
 from evennia.utils.idmapper.models import flush_cache
 from evennia.utils.utils import all_from_module, to_str
 
 _RE_STRIP_EVMENU = re.compile(r"^\+|-+\+|\+-+|--+|\|(?:\s|$)", re.MULTILINE)
 
 
@@ -230,62 +230,62 @@
         self.account2.db._last_puppet = self.char2
 
     def create_script(self):
         self.script = create.create_script(self.script_typeclass, key="Script")
 
     def setup_session(self):
         dummysession = ServerSession()
-        dummysession.init_session("telnet", ("localhost", "testmode"), SESSIONS)
+        dummysession.init_session("telnet", ("localhost", "testmode"), evennia.SESSION_HANDLER)
         dummysession.sessid = 1
-        SESSIONS.portal_connect(
+        evennia.SESSION_HANDLER.portal_connect(
             dummysession.get_sync_data()
         )  # note that this creates a new Session!
-        session = SESSIONS.session_from_sessid(1)  # the real session
-        SESSIONS.login(session, self.account, testmode=True)
+        session = evennia.SESSION_HANDLER.session_from_sessid(1)  # the real session
+        evennia.SESSION_HANDLER.login(session, self.account, testmode=True)
         self.session = session
 
     def teardown_session(self):
         if hasattr(self, "sessions"):
-            del SESSIONS[self.session.sessid]
+            del evennia.SESSION_HANDLER[self.session.sessid]
 
     @patch("evennia.scripts.taskhandler.deferLater", _mock_deferlater)
     def setUp(self):
         """
         Sets up testing environment
         """
         self.backups = (
-            SESSIONS.data_out,
-            SESSIONS.disconnect,
+            evennia.SESSION_HANDLER.data_out,
+            evennia.SESSION_HANDLER.disconnect,
             settings.DEFAULT_HOME,
             settings.PROTOTYPE_MODULES,
         )
-        SESSIONS.data_out = Mock()
-        SESSIONS.disconnect = Mock()
+        evennia.SESSION_HANDLER.data_out = Mock()
+        evennia.SESSION_HANDLER.disconnect = Mock()
 
         self.create_accounts()
         self.create_rooms()
         self.create_objs()
         self.create_chars()
         self.create_script()
         self.setup_session()
 
     def tearDown(self):
         flush_cache()
         try:
-            SESSIONS.data_out = self.backups[0]
-            SESSIONS.disconnect = self.backups[1]
+            evennia.SESSION_HANDLER.data_out = self.backups[0]
+            evennia.SESSION_HANDLER.disconnect = self.backups[1]
             settings.DEFAULT_HOME = self.backups[2]
             settings.PROTOTYPE_MODULES = self.backups[3]
         except AttributeError as err:
             raise AttributeError(
                 f"{err}: Teardown error. If you overrode the `setUp()` method "
                 "in your test, make sure you also added `super().setUp()`!"
             )
 
-        del SESSIONS[self.session.sessid]
+        del evennia.SESSION_HANDLER[self.session.sessid]
         self.teardown_accounts()
         super().tearDown()
 
 
 @patch("evennia.server.portal.portal.LoopingCall", new=MagicMock())
 class EvenniaCommandTestMixin:
     """
@@ -418,15 +418,15 @@
         caller = caller if caller else self.char1
         cmdobj.caller = caller
         cmdobj.cmdname = cmdstring if cmdstring else cmdobj.key
         cmdobj.raw_cmdname = cmdobj.cmdname
         cmdobj.cmdstring = cmdobj.cmdname  # deprecated
         cmdobj.args = input_args
         cmdobj.cmdset = cmdset
-        cmdobj.session = SESSIONS.session_from_sessid(1)
+        cmdobj.session = evennia.SESSION_HANDLER.session_from_sessid(1)
         cmdobj.account = self.account
         cmdobj.raw_string = raw_string if raw_string is not None else cmdobj.key + " " + input_args
         cmdobj.obj = obj or (caller if caller else self.char1)
         inputs = inputs or []
 
         # set up receivers
         receiver_mapping = {}
```

### Comparing `evennia-1.3.0/evennia/utils/tests/data/evform_example.py` & `evennia-2.0.0/evennia/utils/tests/data/evform_example.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/utils/tests/data/evmenu_example.py` & `evennia-2.0.0/evennia/utils/tests/data/evmenu_example.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/utils/tests/test_ansi.py` & `evennia-2.0.0/evennia/utils/tests/test_ansi.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/utils/tests/test_batchprocessors.py` & `evennia-2.0.0/evennia/utils/tests/test_batchprocessors.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/utils/tests/test_containers.py` & `evennia-2.0.0/evennia/utils/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/utils/tests/test_create_functions.py` & `evennia-2.0.0/evennia/utils/tests/test_create_functions.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/utils/tests/test_dbserialize.py` & `evennia-2.0.0/evennia/utils/tests/test_dbserialize.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/utils/tests/test_eveditor.py` & `evennia-2.0.0/evennia/utils/tests/test_eveditor.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/utils/tests/test_evform.py` & `evennia-2.0.0/evennia/utils/tests/test_evform.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/utils/tests/test_evmenu.py` & `evennia-2.0.0/evennia/utils/tests/test_evmenu.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,18 +17,17 @@
 
 """
 
 import copy
 
 from anything import Anything
 from django.test import TestCase
-from mock import MagicMock
-
 from evennia.utils import ansi, evmenu
 from evennia.utils.test_resources import BaseEvenniaTest
+from mock import MagicMock
 
 
 class TestEvMenu(TestCase):
     "Run the EvMenu testing."
     menutree = {}  # can also be the path to the menu tree
     startnode = "start"
     cmdset_mergetype = "Replace"
@@ -66,15 +65,14 @@
     def _test_menutree(self, menu):
         """
         This is a automatic tester of the menu tree by recursively progressing through the
         structure.
         """
 
         def _depth_first(menu, tree, visited, indent):
-
             # we are in a given node here
             nodename = menu.nodename
             options = menu.test_options
             if isinstance(options, dict):
                 options = (options,)
 
             # run validation tests for this node
@@ -116,15 +114,14 @@
             if not options:
                 # an end node
                 if nodename not in visited:
                     visited.append(nodename)
                 subtree = nodename
             else:
                 for inum, optdict in enumerate(options):
-
                     key, desc, execute, goto = (
                         optdict.get("key", ""),
                         optdict.get("desc", None),
                         optdict.get("exec", None),
                         optdict.get("goto", None),
                     )
 
@@ -227,15 +224,14 @@
     def test_menu_structure(self):
         if self.menu:
             self._test_menutree(self.menu)
             self._test_menutree(self.pmenu)
 
 
 class TestEvMenuExample(TestEvMenu):
-
     menutree = "evennia.utils.tests.data.evmenu_example"
     startnode = "test_start_node"
     kwargs = {"testval": "val", "testval2": "val2"}
     debug_output = False
 
     expected_node_texts = {"test_view_node": "Your name is"}
```

### Comparing `evennia-1.3.0/evennia/utils/tests/test_evtable.py` & `evennia-2.0.0/evennia/utils/tests/test_evtable.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/utils/tests/test_funcparser.py` & `evennia-2.0.0/evennia/utils/tests/test_funcparser.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/utils/tests/test_gametime.py` & `evennia-2.0.0/evennia/utils/tests/test_gametime.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/utils/tests/test_search.py` & `evennia-2.0.0/evennia/utils/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/utils/tests/test_tagparsing.py` & `evennia-2.0.0/evennia/utils/tests/test_tagparsing.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/utils/tests/test_text2html.py` & `evennia-2.0.0/evennia/utils/tests/test_text2html.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/utils/tests/test_utils.py` & `evennia-2.0.0/evennia/utils/tests/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         input_string = "  hello\n  world"
         expected_string = "hello\nworld"
         self.assertEqual(expected_string, utils.dedent(input_string))
 
 
 class TestListToString(TestCase):
     """
-    Default function header from utils.py:
+    Default function header from time.py:
     list_to_string(inlist, sep=",", endsep=", and", addquote=False)
 
     Examples:
      with defaults:
         [1,2,3] -> '1, 2, and 3'
      with endsep==',':
         [1,2,3] -> '1, 2, 3'
@@ -171,15 +171,15 @@
 
     def test_format(self):
         self.assertEqual(f"{self.example_ansi:0<20}", self.example_output + "000")
 
 
 class TestTimeformat(TestCase):
     """
-    Default function header from utils.py:
+    Default function header from time.py:
     time_format(seconds, style=0)
 
     """
 
     def test_style_0(self):
         """Test the style 0 of time_format."""
         self.assertEqual(utils.time_format(0, 0), "00:00")
```

### Comparing `evennia-1.3.0/evennia/utils/tests/test_validatorfuncs.py` & `evennia-2.0.0/evennia/utils/tests/test_validatorfuncs.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/utils/text2html.py` & `evennia-2.0.0/evennia/utils/text2html.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/utils/utils.py` & `evennia-2.0.0/evennia/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 from django.apps import apps
 from django.conf import settings
 from django.core.exceptions import ValidationError as DjangoValidationError
 from django.core.validators import validate_email as django_validate_email
 from django.utils import timezone
 from django.utils.html import strip_tags
 from django.utils.translation import gettext as _
+
+import evennia
 from evennia.utils import logger
 from simpleeval import simple_eval
 from twisted.internet import reactor, threads
 from twisted.internet.defer import returnValue  # noqa - used as import target
 from twisted.internet.task import deferLater
 
 _MULTIMATCH_TEMPLATE = settings.SEARCH_MULTIMATCH_TEMPLATE
@@ -1057,22 +1059,21 @@
     services are launched in memory, this function will only return
     any results if called from inside the game.
 
     Returns:
         services (dict): A dict of available services.
 
     """
-    from evennia.server.sessionhandler import SESSIONS
 
-    if hasattr(SESSIONS, "server") and hasattr(SESSIONS.server, "services"):
-        server = SESSIONS.server.services.namedServices
+    if hasattr(evennia.SESSION_HANDLER, "server") and hasattr(evennia.SESSION_HANDLER.server, "services"):
+        server = evennia.SESSION_HANDLER.server.services.namedServices
     else:
         # This function must be called from inside the evennia process.
         server = {}
-    del SESSIONS
+    del evennia.SESSION_HANDLER
     return server
 
 
 def uses_database(name="sqlite3"):
     """
     Checks if the game is currently using a given database. This is a
     shortcut to having to use the full backend name.
```

### Comparing `evennia-1.3.0/evennia/utils/validatorfuncs.py` & `evennia-2.0.0/evennia/utils/validatorfuncs.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/utils/verb_conjugation/LICENSE.txt` & `evennia-2.0.0/evennia/utils/verb_conjugation/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/utils/verb_conjugation/conjugate.py` & `evennia-2.0.0/evennia/utils/verb_conjugation/conjugate.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/utils/verb_conjugation/pronouns.py` & `evennia-2.0.0/evennia/utils/verb_conjugation/pronouns.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/utils/verb_conjugation/tests.py` & `evennia-2.0.0/evennia/utils/verb_conjugation/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/utils/verb_conjugation/verbs.txt` & `evennia-2.0.0/evennia/utils/verb_conjugation/verbs.txt`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/README.md` & `evennia-2.0.0/evennia/web/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/admin/accounts.py` & `evennia-2.0.0/evennia/web/admin/accounts.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/admin/attributes.py` & `evennia-2.0.0/evennia/web/admin/attributes.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/admin/comms.py` & `evennia-2.0.0/evennia/web/admin/comms.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/admin/frontpage.py` & `evennia-2.0.0/evennia/web/admin/frontpage.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/admin/help.py` & `evennia-2.0.0/evennia/web/admin/help.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/admin/objects.py` & `evennia-2.0.0/evennia/web/admin/objects.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/admin/scripts.py` & `evennia-2.0.0/evennia/web/admin/scripts.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/admin/tags.py` & `evennia-2.0.0/evennia/web/admin/tags.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/admin/urls.py` & `evennia-2.0.0/evennia/web/admin/urls.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/admin/utils.py` & `evennia-2.0.0/evennia/web/admin/utils.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/api/README.md` & `evennia-2.0.0/evennia/web/api/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/api/filters.py` & `evennia-2.0.0/evennia/web/api/filters.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/api/permissions.py` & `evennia-2.0.0/evennia/web/api/permissions.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/api/serializers.py` & `evennia-2.0.0/evennia/web/api/serializers.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/api/tests.py` & `evennia-2.0.0/evennia/web/api/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/api/urls.py` & `evennia-2.0.0/evennia/web/api/urls.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/api/views.py` & `evennia-2.0.0/evennia/web/api/views.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/static/rest_framework/images/favicon.ico` & `evennia-2.0.0/evennia/web/static/rest_framework/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/static/webclient/css/goldenlayout.css` & `evennia-2.0.0/evennia/web/static/webclient/css/goldenlayout.css`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/static/webclient/css/webclient.css` & `evennia-2.0.0/evennia/web/static/webclient/css/webclient.css`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/static/webclient/fonts/DejaVuSansMono-webfont.woff` & `evennia-2.0.0/evennia/web/static/webclient/fonts/DejaVuSansMono-webfont.woff`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/static/webclient/js/evennia.js` & `evennia-2.0.0/evennia/web/static/webclient/js/evennia.js`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/static/webclient/js/plugins/clienthelp.js` & `evennia-2.0.0/evennia/web/static/webclient/js/plugins/clienthelp.js`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/static/webclient/js/plugins/default_in.js` & `evennia-2.0.0/evennia/web/static/webclient/js/plugins/default_in.js`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/static/webclient/js/plugins/default_out.js` & `evennia-2.0.0/evennia/web/static/webclient/js/plugins/default_out.js`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/static/webclient/js/plugins/font.js` & `evennia-2.0.0/evennia/web/static/webclient/js/plugins/font.js`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/static/webclient/js/plugins/goldenlayout.js` & `evennia-2.0.0/evennia/web/static/webclient/js/plugins/goldenlayout.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -638,24 +638,25 @@
     }
 
 
     //
     // Add new HTML message to an existing Div pane, while
     // honoring the pane's updateMethod and scroll state, etc.
     //
-    var addMessageToPaneDiv = function(textDiv, message) {
+    var addMessageToPaneDiv = function(textDiv, message, kwargs) {
         let atBottom = false;
         let updateMethod = textDiv.attr("updateMethod");
 
         if (updateMethod === "replace") {
             textDiv.html(message);
         } else if (updateMethod === "append") {
             textDiv.append(message);
         } else { // line feed
-            textDiv.append("<div class='out'>" + message + "</div>");
+            var cls = (kwargs === undefined) || (kwargs['cls'] === undefined) ? 'out' : kwargs['cls'];
+            textDiv.append("<div class='" + cls + "'>" + message + "</div>");
         }
 
         // Calculate the scrollback state.
         //
         // This check helps us avoid scrolling to the bottom when someone is
         // manually scrolled back, trying to read their backlog.
         // Auto-scrolling would force them to re-scroll to their previous scroll position.
@@ -784,15 +785,15 @@
         // are any panes set to receive this text message?
         var divs = routeMessage(args, kwargs);
 
         var msgHandled = false;
         divs.forEach(function(div) {
             let txt = args[0];
             // yes, so add this text message to the target div
-            addMessageToPaneDiv(div, txt);
+            addMessageToPaneDiv(div, txt, kwargs);
             msgHandled = true;
         });
 
         return msgHandled;
     }
```

### Comparing `evennia-1.3.0/evennia/web/static/webclient/js/plugins/goldenlayout_default_config.js` & `evennia-2.0.0/evennia/web/static/webclient/js/plugins/goldenlayout_default_config.js`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/static/webclient/js/plugins/history.js` & `evennia-2.0.0/evennia/web/static/webclient/js/plugins/history.js`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/static/webclient/js/plugins/hotbuttons.js` & `evennia-2.0.0/evennia/web/static/webclient/js/plugins/hotbuttons.js`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/static/webclient/js/plugins/html.js` & `evennia-2.0.0/evennia/web/static/webclient/js/plugins/html.js`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/static/webclient/js/plugins/iframe.js` & `evennia-2.0.0/evennia/web/static/webclient/js/plugins/iframe.js`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/static/webclient/js/plugins/message_routing.js` & `evennia-2.0.0/evennia/web/static/webclient/js/plugins/message_routing.js`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/static/webclient/js/plugins/multimedia.js` & `evennia-2.0.0/evennia/web/static/webclient/js/plugins/multimedia.js`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/static/webclient/js/plugins/notifications.js` & `evennia-2.0.0/evennia/web/static/webclient/js/plugins/notifications.js`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/static/webclient/js/plugins/oob.js` & `evennia-2.0.0/evennia/web/static/webclient/js/plugins/oob.js`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/static/webclient/js/plugins/options2.js` & `evennia-2.0.0/evennia/web/static/webclient/js/plugins/options2.js`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/static/webclient/js/plugins/popups.js` & `evennia-2.0.0/evennia/web/static/webclient/js/plugins/popups.js`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/static/webclient/js/plugins/text2html.js` & `evennia-2.0.0/evennia/web/static/webclient/js/plugins/text2html.js`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/static/webclient/js/webclient_gui.js` & `evennia-2.0.0/evennia/web/static/webclient/js/webclient_gui.js`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/static/webclient/media/notification.wav` & `evennia-2.0.0/evennia/web/static/webclient/media/notification.wav`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/static/website/css/website.css` & `evennia-2.0.0/evennia/web/static/website/css/website.css`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/static/website/images/evennia_logo.png` & `evennia-2.0.0/evennia/web/static/website/images/evennia_logo.png`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/static/website/images/evennia_logo_festive.png` & `evennia-2.0.0/evennia/web/static/website/images/evennia_logo_festive.png`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/static/website/images/favicon.ico` & `evennia-2.0.0/evennia/web/static/website/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/templates/admin/app_list.html` & `evennia-2.0.0/evennia/web/templates/admin/app_list.html`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/templates/admin/frontpage.html` & `evennia-2.0.0/evennia/web/templates/admin/frontpage.html`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/templates/rest_framework/api.html` & `evennia-2.0.0/evennia/web/templates/rest_framework/api.html`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/templates/webclient/base.html` & `evennia-2.0.0/evennia/web/templates/webclient/base.html`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/templates/webclient/webclient.html` & `evennia-2.0.0/evennia/web/templates/webclient/webclient.html`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/templates/website/500.html` & `evennia-2.0.0/evennia/web/templates/website/500.html`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/templates/website/_menu.html` & `evennia-2.0.0/evennia/web/templates/website/_menu.html`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/templates/website/base.html` & `evennia-2.0.0/evennia/web/templates/website/base.html`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/templates/website/channel_detail.html` & `evennia-2.0.0/evennia/web/templates/website/channel_detail.html`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/templates/website/channel_list.html` & `evennia-2.0.0/evennia/web/templates/website/channel_list.html`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/templates/website/character_form.html` & `evennia-2.0.0/evennia/web/templates/website/character_form.html`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/templates/website/character_list.html` & `evennia-2.0.0/evennia/web/templates/website/character_list.html`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/templates/website/character_manage_list.html` & `evennia-2.0.0/evennia/web/templates/website/character_manage_list.html`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/templates/website/generic_form.html` & `evennia-2.0.0/evennia/web/templates/website/generic_form.html`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/templates/website/help_detail.html` & `evennia-2.0.0/evennia/web/templates/website/help_detail.html`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/templates/website/help_list.html` & `evennia-2.0.0/evennia/web/templates/website/help_list.html`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/templates/website/index.html` & `evennia-2.0.0/evennia/web/templates/website/index.html`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/templates/website/object_confirm_delete.html` & `evennia-2.0.0/evennia/web/templates/website/object_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/templates/website/object_detail.html` & `evennia-2.0.0/evennia/web/templates/website/object_detail.html`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/templates/website/object_list.html` & `evennia-2.0.0/evennia/web/templates/website/object_list.html`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/templates/website/pagination.html` & `evennia-2.0.0/evennia/web/templates/website/pagination.html`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/templates/website/registration/logged_out.html` & `evennia-2.0.0/evennia/web/templates/website/registration/logged_out.html`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/templates/website/registration/login.html` & `evennia-2.0.0/evennia/web/templates/website/registration/login.html`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/templates/website/registration/password_change_done.html` & `evennia-2.0.0/evennia/web/templates/website/registration/password_change_done.html`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/templates/website/registration/password_change_form.html` & `evennia-2.0.0/evennia/web/templates/website/registration/password_change_form.html`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/templates/website/registration/password_reset_complete.html` & `evennia-2.0.0/evennia/web/templates/website/registration/password_reset_complete.html`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/templates/website/registration/password_reset_confirm.html` & `evennia-2.0.0/evennia/web/templates/website/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/templates/website/registration/password_reset_done.html` & `evennia-2.0.0/evennia/web/templates/website/registration/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/templates/website/registration/password_reset_email.html` & `evennia-2.0.0/evennia/web/templates/website/registration/password_reset_email.html`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/templates/website/registration/password_reset_form.html` & `evennia-2.0.0/evennia/web/templates/website/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/templates/website/registration/register.html` & `evennia-2.0.0/evennia/web/templates/website/registration/register.html`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/templates/website/tbi.html` & `evennia-2.0.0/evennia/web/templates/website/tbi.html`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/templatetags/addclass.py` & `evennia-2.0.0/evennia/web/templatetags/addclass.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/urls.py` & `evennia-2.0.0/evennia/web/urls.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/utils/adminsite.py` & `evennia-2.0.0/evennia/web/utils/adminsite.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/utils/apache_wsgi.conf` & `evennia-2.0.0/evennia/web/utils/apache_wsgi.conf`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/utils/backends.py` & `evennia-2.0.0/evennia/web/utils/backends.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/utils/evennia_modpy_apache.conf` & `evennia-2.0.0/evennia/web/utils/evennia_modpy_apache.conf`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/utils/evennia_wsgi_apache.conf` & `evennia-2.0.0/evennia/web/utils/evennia_wsgi_apache.conf`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/utils/general_context.py` & `evennia-2.0.0/evennia/web/utils/general_context.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/utils/middleware.py` & `evennia-2.0.0/evennia/web/utils/middleware.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/utils/tests.py` & `evennia-2.0.0/evennia/web/utils/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/webclient/views.py` & `evennia-2.0.0/evennia/web/webclient/views.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/website/forms.py` & `evennia-2.0.0/evennia/web/website/forms.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/website/tests.py` & `evennia-2.0.0/evennia/web/website/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/website/urls.py` & `evennia-2.0.0/evennia/web/website/urls.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/website/views/accounts.py` & `evennia-2.0.0/evennia/web/website/views/accounts.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/website/views/channels.py` & `evennia-2.0.0/evennia/web/website/views/channels.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/website/views/characters.py` & `evennia-2.0.0/evennia/web/website/views/characters.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/website/views/help.py` & `evennia-2.0.0/evennia/web/website/views/help.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/website/views/index.py` & `evennia-2.0.0/evennia/web/website/views/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 The main index page, including the game stats
 
 """
 
 from django.conf import settings
 from django.views.generic import TemplateView
 
-from evennia import SESSION_HANDLER
+import evennia
 from evennia.accounts.models import AccountDB
 from evennia.objects.models import ObjectDB
 from evennia.utils import class_from_module
 
 
 def _gamestats():
     """
@@ -21,15 +21,15 @@
     fpage_account_limit = 4
 
     # A QuerySet of the most recently connected accounts.
     recent_users = AccountDB.objects.get_recently_connected_accounts()
     nplyrs_conn_recent = len(recent_users) or "none"
     nplyrs = AccountDB.objects.num_total_accounts() or "none"
     nplyrs_reg_recent = len(AccountDB.objects.get_recently_created_accounts()) or "none"
-    nsess = SESSION_HANDLER.account_count()
+    nsess = evennia.SESSION_HANDLER.account_count()
     # nsess = len(AccountDB.objects.get_connected_accounts()) or "no one"
 
     nobjs = ObjectDB.objects.count()
     nobjs = nobjs or 1  # fix zero-div error with empty database
     Character = class_from_module(
         settings.BASE_CHARACTER_TYPECLASS, fallback=settings.FALLBACK_CHARACTER_TYPECLASS
     )
```

### Comparing `evennia-1.3.0/evennia/web/website/views/mixins.py` & `evennia-2.0.0/evennia/web/website/views/mixins.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia/web/website/views/objects.py` & `evennia-2.0.0/evennia/web/website/views/objects.py`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/evennia.egg-info/PKG-INFO` & `evennia-2.0.0/evennia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evennia
-Version: 1.3.0
+Version: 2.0.0
 Summary: A full-featured toolkit and server for text-based multiplayer games (MUDs, MU*, etc).
 Maintainer-email: Griatch <griatch@gmail.com>
 License: BSD
 Project-URL: Homepage, https://www.evennia.com
 Project-URL: Github, https://github.com/evennia/evennia
 Project-URL: Documentation, https://www.evennia.com/docs/latest/index.html
 Project-URL: Live Demo, https://demo.evennia.com/
```

### Comparing `evennia-1.3.0/evennia.egg-info/SOURCES.txt` & `evennia-2.0.0/evennia.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -165,14 +165,18 @@
 evennia/contrib/game_systems/barter/__init__.py
 evennia/contrib/game_systems/barter/barter.py
 evennia/contrib/game_systems/barter/tests.py
 evennia/contrib/game_systems/clothing/README.md
 evennia/contrib/game_systems/clothing/__init__.py
 evennia/contrib/game_systems/clothing/clothing.py
 evennia/contrib/game_systems/clothing/tests.py
+evennia/contrib/game_systems/containers/README.md
+evennia/contrib/game_systems/containers/__init__.py
+evennia/contrib/game_systems/containers/containers.py
+evennia/contrib/game_systems/containers/tests.py
 evennia/contrib/game_systems/cooldowns/README.md
 evennia/contrib/game_systems/cooldowns/__init__.py
 evennia/contrib/game_systems/cooldowns/cooldowns.py
 evennia/contrib/game_systems/cooldowns/tests.py
 evennia/contrib/game_systems/crafting/README.md
 evennia/contrib/game_systems/crafting/__init__.py
 evennia/contrib/game_systems/crafting/crafting.py
@@ -281,36 +285,43 @@
 evennia/contrib/tutorials/bodyfunctions/tests.py
 evennia/contrib/tutorials/evadventure/README.md
 evennia/contrib/tutorials/evadventure/__init__.py
 evennia/contrib/tutorials/evadventure/build_techdemo.py
 evennia/contrib/tutorials/evadventure/build_world.py
 evennia/contrib/tutorials/evadventure/characters.py
 evennia/contrib/tutorials/evadventure/chargen.py
+evennia/contrib/tutorials/evadventure/combat_base.py
 evennia/contrib/tutorials/evadventure/combat_turnbased.py
+evennia/contrib/tutorials/evadventure/combat_twitch.py
 evennia/contrib/tutorials/evadventure/commands.py
 evennia/contrib/tutorials/evadventure/dungeon.py
 evennia/contrib/tutorials/evadventure/enums.py
 evennia/contrib/tutorials/evadventure/equipment.py
 evennia/contrib/tutorials/evadventure/npcs.py
 evennia/contrib/tutorials/evadventure/objects.py
 evennia/contrib/tutorials/evadventure/quests.py
 evennia/contrib/tutorials/evadventure/random_tables.py
 evennia/contrib/tutorials/evadventure/rooms.py
 evennia/contrib/tutorials/evadventure/rules.py
 evennia/contrib/tutorials/evadventure/shops.py
 evennia/contrib/tutorials/evadventure/utils.py
+evennia/contrib/tutorials/evadventure/batchscripts/__init__.py
+evennia/contrib/tutorials/evadventure/batchscripts/turnbased_combat_demo.py
+evennia/contrib/tutorials/evadventure/batchscripts/twitch_combat_demo.ev
 evennia/contrib/tutorials/evadventure/tests/__init__.py
 evennia/contrib/tutorials/evadventure/tests/mixins.py
 evennia/contrib/tutorials/evadventure/tests/test_characters.py
 evennia/contrib/tutorials/evadventure/tests/test_chargen.py
 evennia/contrib/tutorials/evadventure/tests/test_combat.py
 evennia/contrib/tutorials/evadventure/tests/test_commands.py
 evennia/contrib/tutorials/evadventure/tests/test_dungeon.py
 evennia/contrib/tutorials/evadventure/tests/test_equipment.py
+evennia/contrib/tutorials/evadventure/tests/test_npcs.py
 evennia/contrib/tutorials/evadventure/tests/test_quests.py
+evennia/contrib/tutorials/evadventure/tests/test_rooms.py
 evennia/contrib/tutorials/evadventure/tests/test_rules.py
 evennia/contrib/tutorials/evadventure/tests/test_utils.py
 evennia/contrib/tutorials/mirror/README.md
 evennia/contrib/tutorials/mirror/__init__.py
 evennia/contrib/tutorials/mirror/mirror.py
 evennia/contrib/tutorials/red_button/README.md
 evennia/contrib/tutorials/red_button/__init__.py
```

### Comparing `evennia-1.3.0/evennia.egg-info/requires.txt` & `evennia-2.0.0/evennia.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `evennia-1.3.0/pyproject.toml` & `evennia-2.0.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "evennia"
-version = "1.3.0"
+version = "2.0.0"
 maintainers = [{ name = "Griatch", email = "griatch@gmail.com" }]
 description = "A full-featured toolkit and server for text-based multiplayer games (MUDs, MU*, etc)."
 requires-python = ">=3.10"
 readme = { file = "README.md", content-type = "text/markdown" }
 license = { text = "BSD" }
 keywords = [
   "MUD",
```

### Comparing `evennia-1.3.0/setup.py` & `evennia-2.0.0/setup.py`

 * *Files identical despite different names*

