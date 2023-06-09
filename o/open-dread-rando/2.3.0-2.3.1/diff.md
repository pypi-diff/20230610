# Comparing `tmp/open-dread-rando-2.3.0.tar.gz` & `tmp/open-dread-rando-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open-dread-rando-2.3.0.tar", last modified: Thu Jun  8 20:43:36 2023, max compression
+gzip compressed data, was "open-dread-rando-2.3.1.tar", last modified: Fri Jun  9 23:40:52 2023, max compression
```

## Comparing `open-dread-rando-2.3.0.tar` & `open-dread-rando-2.3.1.tar`

### file list

```diff
@@ -1,242 +1,242 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.331267 open-dread-rando-2.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.291267 open-dread-rando-2.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.291267 open-dread-rando-2.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/.github/workflows/patch.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/.github/workflows/python.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.291267 open-dread-rando-2.3.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-08 20:43:36.331267 open-dread-rando-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.299267 open-dread-rando-2.3.0/open_dread_rando/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.303267 open-dread-rando-2.3.0/open_dread_rando/__pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/__pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/__pyinstaller/hook-open_dread_rando.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/cosmetic_patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/custom_door_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    21271 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/door_patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    10941 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/dread_patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/elevator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/environmental_damage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/environmental_damage_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/exefs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.303267 open-dread-rando-2.3.0/open_dread_rando/files/
--rw-r--r--   0 runner    (1001) docker     (123)    15151 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/custom_scenario.lua
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.303267 open-dread-rando-2.3.0/open_dread_rando/files/dread_depackager/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/dread_depackager/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/dread_depackager/main.npdm
--rw-r--r--   0 runner    (1001) docker     (123)   190964 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/dread_depackager/subsdk9
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.303267 open-dread-rando-2.3.0/open_dread_rando/files/exefs_patches/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/exefs_patches/debug_input.s
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.307267 open-dread-rando-2.3.0/open_dread_rando/files/levels/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/levels/readme.txt
--rw-r--r--   0 runner    (1001) docker     (123)    67135 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/levels/s010_cave.lc.lua
--rw-r--r--   0 runner    (1001) docker     (123)    37704 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/levels/s020_magma.lc.lua
--rw-r--r--   0 runner    (1001) docker     (123)    23300 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/levels/s030_baselab.lc.lua
--rw-r--r--   0 runner    (1001) docker     (123)    32062 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/levels/s040_aqua.lc.lua
--rw-r--r--   0 runner    (1001) docker     (123)    25145 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/levels/s050_forest.lc.lua
--rw-r--r--   0 runner    (1001) docker     (123)    10649 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/levels/s060_quarantine.lc.lua
--rw-r--r--   0 runner    (1001) docker     (123)    30569 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/levels/s070_basesanc.lc.lua
--rw-r--r--   0 runner    (1001) docker     (123)    16577 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/levels/s080_shipyard.lc.lua
--rw-r--r--   0 runner    (1001) docker     (123)     7290 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/levels/s090_skybase.lc.lua
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.307267 open-dread-rando-2.3.0/open_dread_rando/files/lua_libraries/
--rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/lua_libraries/bit.lua
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/lua_libraries/data_structures.lua
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/lua_libraries/death_counter.lua
--rw-r--r--   0 runner    (1001) docker     (123)    12239 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/lua_libraries/guilib.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/lua_libraries/input_handling.lua
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/lua_libraries/room_names.lua
--rw-r--r--   0 runner    (1001) docker     (123)    26346 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/msemenu_mainmenu.lua
--rw-r--r--   0 runner    (1001) docker     (123)    12274 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/randomizer_powerup.lua
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.283267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.283267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.279267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.275267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/item_cube/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.275267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/item_cube/model/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.307267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_camo.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_sonr.bsmat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.279267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/item_cube_broken/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.311267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/
--rw-r--r--   0 runner    (1001) docker     (123)   422936 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_camo.bcmdl
--rw-r--r--   0 runner    (1001) docker     (123)   422936 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_sonr.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.279267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/item_missiletank/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.315267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/item_missiletank/models/
--rw-r--r--   0 runner    (1001) docker     (123)    16460 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__BK.bcmdl
--rw-r--r--   0 runner    (1001) docker     (123)    16460 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__BL.bcmdl
--rw-r--r--   0 runner    (1001) docker     (123)    16460 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__CY.bcmdl
--rw-r--r--   0 runner    (1001) docker     (123)    16460 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__GN.bcmdl
--rw-r--r--   0 runner    (1001) docker     (123)    16460 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__GY.bcmdl
--rw-r--r--   0 runner    (1001) docker     (123)    16460 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__MG.bcmdl
--rw-r--r--   0 runner    (1001) docker     (123)    16460 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__OR.bcmdl
--rw-r--r--   0 runner    (1001) docker     (123)    16460 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__PK.bcmdl
--rw-r--r--   0 runner    (1001) docker     (123)    16460 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__PR.bcmdl
--rw-r--r--   0 runner    (1001) docker     (123)    16460 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__WH.bcmdl
--rw-r--r--   0 runner    (1001) docker     (123)    16460 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__YL.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.279267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/itemsphere/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.315267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/itemsphere/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.315267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/itemsphere/models/imats/
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/itemsphere/models/imats/speedboost_mp_opaque_01.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)     9508 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/itemsphere/models/speed_booster.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.279267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/powerup_bomb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.315267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.315267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphhologram.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphmaterial.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)    19348 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/powerup_morph.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.279267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/powerup_doublejump/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.315267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.315267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_magnet01.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_white__01.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)    33012 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/powerup_magnet.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.279267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.315267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.315267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/powerup_powerbomb_mat0001.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/powerup_powerbomb_mp_fxhologram_0001.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)    13404 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/powerup_powerbomb.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.279267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/powerup_supermissile/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.315267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.315267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/imats/
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/imats/powerup_ice__missile_mp_opaque_01.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)    28948 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/powerup_ice__missile.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.283267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/powerup_widebeam/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.319267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.319267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_autoilum.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_bola.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_cangrejo.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)    47996 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/powerup_wavebeam.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.283267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/props/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.283267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/props/doorshieldmissile/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.319267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/props/doorshieldmissile/collisions/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/props/doorshieldmissile/collisions/shield_bomb_colls.bmscd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.283267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/props/doorshieldpowerbomb___/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.319267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/props/doorshieldpowerbomb___/models/
--rw-r--r--   0 runner    (1001) docker     (123)    23292 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/props/doorshieldpowerbomb___/models/doorshieldpowerbomb___.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.319267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/props/doorshieldpowerbomb___/models/imats/
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/props/doorshieldpowerbomb___/models/imats/doorshieldpowerbomb____mp_opaque_01.bsmat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.283267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/props/shield___diffusion/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.319267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.319267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/imats/
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/imats/shield_diffusion_matfx.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/imats/shield_diffusion_mp_opaque_01.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)   140588 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/shield_diffusion.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.283267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/props/shield_bombs_regular__/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.319267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/props/shield_bombs_regular__/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.319267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/props/shield_bombs_regular__/models/imats/
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/props/shield_bombs_regular__/models/imats/shield_bombs_regular___mp_opaque_01.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)    23292 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/props/shield_bombs_regular__/models/shield_bombs_regular__.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.283267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/props/shield_cross_bomb_____/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.319267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/props/shield_cross_bomb_____/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.323267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/props/shield_cross_bomb_____/models/imats/
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/props/shield_cross_bomb_____/models/imats/shield_cross_bomb______mp_opaque_01.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)    23292 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/props/shield_cross_bomb_____/models/shield_cross_bomb_____.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.283267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/props/shield_icemissile/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.323267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/props/shield_icemissile/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.323267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/props/shield_icemissile/models/imats/
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/props/shield_icemissile/models/imats/shield_icemissile_mp_opaque_01.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)    22156 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/props/shield_icemissile/models/shield_icemissile.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.283267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/props/shield_storm_mssl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.323267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/props/shield_storm_mssl/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.323267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/props/shield_storm_mssl/models/imats/
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/props/shield_storm_mssl/models/imats/shield_storm_mssl_mp_opaque_01.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)    22156 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/props/shield_storm_mssl/models/shield_storm_mssl.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.287267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.287267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.287267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/items/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.283267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/items/itemsphere/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.287267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.323267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/
--rw-r--r--   0 runner    (1001) docker     (123)    28804 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_at.bctex
--rw-r--r--   0 runner    (1001) docker     (123)    19894 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_bc.bctex
--rw-r--r--   0 runner    (1001) docker     (123)    42001 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_nm.bctex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.287267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.287267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.323267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/
--rw-r--r--   0 runner    (1001) docker     (123)    14467 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphat.bctex
--rw-r--r--   0 runner    (1001) docker     (123)    17196 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphbc.bctex
--rw-r--r--   0 runner    (1001) docker     (123)    34728 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphnm.bctex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.287267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.287267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.323267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/textures/
--rw-r--r--   0 runner    (1001) docker     (123)    75887 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/textures/powerup_spi_magnet_bc.bctex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.287267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.287267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.323267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/textures/
--rw-r--r--   0 runner    (1001) docker     (123)    71298 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/textures/powerup_ice__missile_bc.bctex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.287267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.287267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.323267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/textures/
--rw-r--r--   0 runner    (1001) docker     (123)   155165 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/textures/pup_wavebeam_bc.bctex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.287267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/props/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.287267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.287267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.327268 open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/textures/
--rw-r--r--   0 runner    (1001) docker     (123)    28577 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/textures/doorshield_____bomb_bc.bctex
--rw-r--r--   0 runner    (1001) docker     (123)    31290 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/textures/doorshieldcrossbomb_bc.bctex
--rw-r--r--   0 runner    (1001) docker     (123)    35688 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/textures/doorshieldpowerbomb_bc.bctex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.287267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/props/shield_storm_mssl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.287267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/props/shield_storm_mssl/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.327268 open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/props/shield_storm_mssl/models/textures/
--rw-r--r--   0 runner    (1001) docker     (123)    24331 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/props/shield_storm_mssl/models/textures/shield_storm_mssl_bc.bctex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.287267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/system/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.287267 open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/system/minimap/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.327268 open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/system/minimap/icons/
--rw-r--r--   0 runner    (1001) docker     (123)   431407 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/system/minimap/icons/icons.bctex
--rw-r--r--   0 runner    (1001) docker     (123)    28273 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/files/schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/game_patches.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/lua_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/lua_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    14311 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/map_icons.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/missile_color_patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    27016 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/model_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/objective.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/output_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/patch_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     7146 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/patcher_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13669 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/pickup.py
--rw-r--r--   0 runner    (1001) docker     (123)    13484 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/static_fixes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.331267 open-dread-rando-2.3.0/open_dread_rando/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/templates/boss_powerup_template.lua
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/templates/cc_to_room_name.lua
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/templates/custom_core_x.lua
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/templates/custom_core_x_superquetzoa.lua
--rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/templates/custom_init.lua
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/templates/progressive_model_template.lua
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/templates/randomizer_progressive_template.lua
--rw-r--r--   0 runner    (1001) docker     (123)    10303 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/templates/template_doorshield_energy_bmsad.json
--rw-r--r--   0 runner    (1001) docker     (123)     9345 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/templates/template_doorshield_hexs_bmsad.json
--rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/templates/template_doorshield_tris_bmsad.json
--rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/templates/template_powerup_bmsad.json
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/text_patches.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/tilegroup_patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/open_dread_rando/validator_with_default.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-08 20:43:36.000000 open-dread-rando-2.3.0/open_dread_rando/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.299267 open-dread-rando-2.3.0/open_dread_rando.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-08 20:43:36.000000 open-dread-rando-2.3.0/open_dread_rando.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-06-08 20:43:36.000000 open-dread-rando-2.3.0/open_dread_rando.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 20:43:36.000000 open-dread-rando-2.3.0/open_dread_rando.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-08 20:43:36.000000 open-dread-rando-2.3.0/open_dread_rando.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 20:43:23.000000 open-dread-rando-2.3.0/open_dread_rando.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-08 20:43:36.000000 open-dread-rando-2.3.0/open_dread_rando.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-08 20:43:36.000000 open-dread-rando-2.3.0/open_dread_rando.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-08 20:43:36.331267 open-dread-rando-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.331267 open-dread-rando-2.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/tests/test_dread_patcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:43:36.331267 open-dread-rando-2.3.0/tests/test_files/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/tests/test_files/randomizer_progressive_expected.lua
--rw-r--r--   0 runner    (1001) docker     (123)   153802 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/tests/test_files/starter_preset_patcher.json
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/tests/test_lua_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-08 20:43:02.000000 open-dread-rando-2.3.0/tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.399672 open-dread-rando-2.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.379672 open-dread-rando-2.3.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.379672 open-dread-rando-2.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/.github/workflows/patch.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/.github/workflows/python.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.379672 open-dread-rando-2.3.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-09 23:40:52.399672 open-dread-rando-2.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.383673 open-dread-rando-2.3.1/open_dread_rando/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.383673 open-dread-rando-2.3.1/open_dread_rando/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/__pyinstaller/hook-open_dread_rando.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/cosmetic_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/custom_door_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21271 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/door_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10941 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/dread_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/elevator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/environmental_damage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/environmental_damage_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/exefs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.383673 open-dread-rando-2.3.1/open_dread_rando/files/
+-rw-r--r--   0 runner    (1001) docker     (123)    15151 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/custom_scenario.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.383673 open-dread-rando-2.3.1/open_dread_rando/files/dread_depackager/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/dread_depackager/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/dread_depackager/main.npdm
+-rw-r--r--   0 runner    (1001) docker     (123)   190964 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/dread_depackager/subsdk9
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.383673 open-dread-rando-2.3.1/open_dread_rando/files/exefs_patches/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/exefs_patches/debug_input.s
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.387673 open-dread-rando-2.3.1/open_dread_rando/files/levels/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/levels/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    67135 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/levels/s010_cave.lc.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    37704 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/levels/s020_magma.lc.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    23300 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/levels/s030_baselab.lc.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    32062 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/levels/s040_aqua.lc.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    25145 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/levels/s050_forest.lc.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    10649 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/levels/s060_quarantine.lc.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    30569 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/levels/s070_basesanc.lc.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    16577 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/levels/s080_shipyard.lc.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     7290 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/levels/s090_skybase.lc.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.387673 open-dread-rando-2.3.1/open_dread_rando/files/lua_libraries/
+-rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/lua_libraries/bit.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/lua_libraries/data_structures.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/lua_libraries/death_counter.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    12239 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/lua_libraries/guilib.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/lua_libraries/input_handling.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/lua_libraries/room_names.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    26346 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/msemenu_mainmenu.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    12659 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/randomizer_powerup.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.375672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.371672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.371672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.371672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/item_cube/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.371672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/item_cube/model/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.387673 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_camo.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_sonr.bsmat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.371672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/item_cube_broken/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.387673 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/
+-rw-r--r--   0 runner    (1001) docker     (123)   422936 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_camo.bcmdl
+-rw-r--r--   0 runner    (1001) docker     (123)   422936 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_sonr.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.371672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/item_missiletank/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.391672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/item_missiletank/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    16460 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__BK.bcmdl
+-rw-r--r--   0 runner    (1001) docker     (123)    16460 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__BL.bcmdl
+-rw-r--r--   0 runner    (1001) docker     (123)    16460 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__CY.bcmdl
+-rw-r--r--   0 runner    (1001) docker     (123)    16460 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__GN.bcmdl
+-rw-r--r--   0 runner    (1001) docker     (123)    16460 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__GY.bcmdl
+-rw-r--r--   0 runner    (1001) docker     (123)    16460 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__MG.bcmdl
+-rw-r--r--   0 runner    (1001) docker     (123)    16460 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__OR.bcmdl
+-rw-r--r--   0 runner    (1001) docker     (123)    16460 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__PK.bcmdl
+-rw-r--r--   0 runner    (1001) docker     (123)    16460 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__PR.bcmdl
+-rw-r--r--   0 runner    (1001) docker     (123)    16460 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__WH.bcmdl
+-rw-r--r--   0 runner    (1001) docker     (123)    16460 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__YL.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.371672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/itemsphere/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.391672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/itemsphere/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.391672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/itemsphere/models/imats/
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/itemsphere/models/imats/speedboost_mp_opaque_01.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)     9508 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/itemsphere/models/speed_booster.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.371672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/powerup_bomb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.391672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.391672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphhologram.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphmaterial.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)    19348 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/powerup_morph.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.371672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/powerup_doublejump/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.391672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.391672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_magnet01.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_white__01.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)    33012 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/powerup_magnet.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.371672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.391672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.391672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/powerup_powerbomb_mat0001.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/powerup_powerbomb_mp_fxhologram_0001.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)    13404 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/powerup_powerbomb.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.371672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/powerup_supermissile/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.391672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.391672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/imats/
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/imats/powerup_ice__missile_mp_opaque_01.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)    28948 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/powerup_ice__missile.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.371672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/powerup_widebeam/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.391672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.391672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_autoilum.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_bola.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_cangrejo.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)    47996 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/powerup_wavebeam.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.375672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/props/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.375672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/props/doorshieldmissile/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.391672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/props/doorshieldmissile/collisions/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/props/doorshieldmissile/collisions/shield_bomb_colls.bmscd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.375672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/props/doorshieldpowerbomb___/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.391672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/props/doorshieldpowerbomb___/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    23292 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/props/doorshieldpowerbomb___/models/doorshieldpowerbomb___.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.391672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/props/doorshieldpowerbomb___/models/imats/
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/props/doorshieldpowerbomb___/models/imats/doorshieldpowerbomb____mp_opaque_01.bsmat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.375672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/props/shield___diffusion/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.391672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.391672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/imats/
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/imats/shield_diffusion_matfx.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/imats/shield_diffusion_mp_opaque_01.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)   140588 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/shield_diffusion.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.375672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/props/shield_bombs_regular__/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.391672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/props/shield_bombs_regular__/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.395672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/props/shield_bombs_regular__/models/imats/
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/props/shield_bombs_regular__/models/imats/shield_bombs_regular___mp_opaque_01.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)    23292 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/props/shield_bombs_regular__/models/shield_bombs_regular__.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.375672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/props/shield_cross_bomb_____/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.395672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/props/shield_cross_bomb_____/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.395672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/props/shield_cross_bomb_____/models/imats/
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/props/shield_cross_bomb_____/models/imats/shield_cross_bomb______mp_opaque_01.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)    23292 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/props/shield_cross_bomb_____/models/shield_cross_bomb_____.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.375672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/props/shield_icemissile/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.395672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/props/shield_icemissile/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.395672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/props/shield_icemissile/models/imats/
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/props/shield_icemissile/models/imats/shield_icemissile_mp_opaque_01.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)    22156 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/props/shield_icemissile/models/shield_icemissile.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.375672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/props/shield_storm_mssl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.395672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/props/shield_storm_mssl/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.395672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/props/shield_storm_mssl/models/imats/
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/props/shield_storm_mssl/models/imats/shield_storm_mssl_mp_opaque_01.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)    22156 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/props/shield_storm_mssl/models/shield_storm_mssl.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.375672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.375672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.375672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/items/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.375672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/items/itemsphere/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.375672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.395672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (123)    28804 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_at.bctex
+-rw-r--r--   0 runner    (1001) docker     (123)    19894 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_bc.bctex
+-rw-r--r--   0 runner    (1001) docker     (123)    42001 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_nm.bctex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.375672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.375672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.395672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (123)    14467 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphat.bctex
+-rw-r--r--   0 runner    (1001) docker     (123)    17196 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphbc.bctex
+-rw-r--r--   0 runner    (1001) docker     (123)    34728 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphnm.bctex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.375672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.375672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.395672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (123)    75887 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/textures/powerup_spi_magnet_bc.bctex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.375672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.375672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.395672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (123)    71298 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/textures/powerup_ice__missile_bc.bctex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.375672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.375672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.395672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (123)   155165 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/textures/pup_wavebeam_bc.bctex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.375672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/props/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.375672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.375672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.395672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (123)    28577 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/textures/doorshield_____bomb_bc.bctex
+-rw-r--r--   0 runner    (1001) docker     (123)    31290 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/textures/doorshieldcrossbomb_bc.bctex
+-rw-r--r--   0 runner    (1001) docker     (123)    35688 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/textures/doorshieldpowerbomb_bc.bctex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.375672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/props/shield_storm_mssl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.375672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/props/shield_storm_mssl/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.395672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/props/shield_storm_mssl/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (123)    24331 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/props/shield_storm_mssl/models/textures/shield_storm_mssl_bc.bctex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.379672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/system/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.379672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/system/minimap/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.395672 open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/system/minimap/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)   431407 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/system/minimap/icons/icons.bctex
+-rw-r--r--   0 runner    (1001) docker     (123)    28273 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/files/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/game_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/lua_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/lua_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14311 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/map_icons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/missile_color_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27016 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/model_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/output_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/patch_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7146 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/patcher_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13669 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/pickup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13484 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/static_fixes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.399672 open-dread-rando-2.3.1/open_dread_rando/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/templates/boss_powerup_template.lua
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/templates/cc_to_room_name.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/templates/custom_core_x.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/templates/custom_core_x_superquetzoa.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/templates/custom_init.lua
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/templates/progressive_model_template.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/templates/randomizer_progressive_template.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    10303 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/templates/template_doorshield_energy_bmsad.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9345 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/templates/template_doorshield_hexs_bmsad.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/templates/template_doorshield_tris_bmsad.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/templates/template_powerup_bmsad.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/text_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/tilegroup_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/open_dread_rando/validator_with_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-09 23:40:52.000000 open-dread-rando-2.3.1/open_dread_rando/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.383673 open-dread-rando-2.3.1/open_dread_rando.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-09 23:40:52.000000 open-dread-rando-2.3.1/open_dread_rando.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-06-09 23:40:52.000000 open-dread-rando-2.3.1/open_dread_rando.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 23:40:52.000000 open-dread-rando-2.3.1/open_dread_rando.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-09 23:40:52.000000 open-dread-rando-2.3.1/open_dread_rando.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 23:40:43.000000 open-dread-rando-2.3.1/open_dread_rando.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-09 23:40:52.000000 open-dread-rando-2.3.1/open_dread_rando.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-09 23:40:52.000000 open-dread-rando-2.3.1/open_dread_rando.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-09 23:40:52.399672 open-dread-rando-2.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.399672 open-dread-rando-2.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/tests/test_dread_patcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:40:52.399672 open-dread-rando-2.3.1/tests/test_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/tests/test_files/randomizer_progressive_expected.lua
+-rw-r--r--   0 runner    (1001) docker     (123)   153802 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/tests/test_files/starter_preset_patcher.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/tests/test_lua_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-09 23:40:31.000000 open-dread-rando-2.3.1/tests/test_schema.py
```

### Comparing `open-dread-rando-2.3.0/.github/dependabot.yml` & `open-dread-rando-2.3.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/.github/workflows/patch.yml` & `open-dread-rando-2.3.1/.github/workflows/patch.yml`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/.github/workflows/python.yml` & `open-dread-rando-2.3.1/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/.gitignore` & `open-dread-rando-2.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/LICENSE` & `open-dread-rando-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/PKG-INFO` & `open-dread-rando-2.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-dread-rando
-Version: 2.3.0
+Version: 2.3.1
 Summary: An open source randomizer patcher for Metroid Dread.
 Home-page: https://github.com/randovania/open-dread-rando
 Author: Henrique Gemignani
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `open-dread-rando-2.3.0/README.md` & `open-dread-rando-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/cli.py` & `open-dread-rando-2.3.1/open_dread_rando/cli.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/cosmetic_patches.py` & `open-dread-rando-2.3.1/open_dread_rando/cosmetic_patches.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/custom_door_types.py` & `open-dread-rando-2.3.1/open_dread_rando/custom_door_types.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/door_patcher.py` & `open-dread-rando-2.3.1/open_dread_rando/door_patcher.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/dread_patcher.py` & `open-dread-rando-2.3.1/open_dread_rando/dread_patcher.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/elevator.py` & `open-dread-rando-2.3.1/open_dread_rando/elevator.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/environmental_damage.py` & `open-dread-rando-2.3.1/open_dread_rando/environmental_damage.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/environmental_damage_sources.py` & `open-dread-rando-2.3.1/open_dread_rando/environmental_damage_sources.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/exefs.py` & `open-dread-rando-2.3.1/open_dread_rando/exefs.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,22 +103,22 @@
     offset, data = debug_input.patch(version)
     if offset is not None:
         patch.add_record(offset, data)
 
 def _patch_door_lock_buffer(patch: ips.Patch, version: str):
     """ Update capacities in unknown allocator to avoid doorlock crash
     changes size of buffer inside data field initializer (I think)
-    size of linked-list buffer increased from 500 to 700. 
+    size of linked-list buffer increased from 500 to 1000. 
     if 0x33250c in 1.0.0 is crashing, it's likely that this is still too small. 
     original instruction: MOV w2,#0x1f4
-    patched instruction: MOV w2,#0x2bc
+    patched instruction: MOV w2,#0x3e8
     """
     buffer_size = {
-        "1.0.0": (0x00ae6f70, bytes.fromhex('82578052')),
-        "2.1.0": (0x00ae9d70, bytes.fromhex('82578052')),
+        "1.0.0": (0x00ae6f70, bytes.fromhex('027D8052')),
+        "2.1.0": (0x00ae9d70, bytes.fromhex('027D8052')),
     }
 
     offset, data = buffer_size[version]
     patch.add_record(offset, data)
 
 def patch_exefs(exefs_patches: Path, configuration: dict):
     exefs_patches.mkdir(parents=True, exist_ok=True)
```

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/custom_scenario.lua` & `open-dread-rando-2.3.1/open_dread_rando/files/custom_scenario.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/dread_depackager/main.npdm` & `open-dread-rando-2.3.1/open_dread_rando/files/dread_depackager/main.npdm`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/dread_depackager/subsdk9` & `open-dread-rando-2.3.1/open_dread_rando/files/dread_depackager/subsdk9`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/exefs_patches/debug_input.s` & `open-dread-rando-2.3.1/open_dread_rando/files/exefs_patches/debug_input.s`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/levels/s010_cave.lc.lua` & `open-dread-rando-2.3.1/open_dread_rando/files/levels/s010_cave.lc.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/levels/s020_magma.lc.lua` & `open-dread-rando-2.3.1/open_dread_rando/files/levels/s020_magma.lc.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/levels/s030_baselab.lc.lua` & `open-dread-rando-2.3.1/open_dread_rando/files/levels/s030_baselab.lc.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/levels/s040_aqua.lc.lua` & `open-dread-rando-2.3.1/open_dread_rando/files/levels/s040_aqua.lc.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/levels/s050_forest.lc.lua` & `open-dread-rando-2.3.1/open_dread_rando/files/levels/s050_forest.lc.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/levels/s060_quarantine.lc.lua` & `open-dread-rando-2.3.1/open_dread_rando/files/levels/s060_quarantine.lc.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/levels/s070_basesanc.lc.lua` & `open-dread-rando-2.3.1/open_dread_rando/files/levels/s070_basesanc.lc.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/levels/s080_shipyard.lc.lua` & `open-dread-rando-2.3.1/open_dread_rando/files/levels/s080_shipyard.lc.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/levels/s090_skybase.lc.lua` & `open-dread-rando-2.3.1/open_dread_rando/files/levels/s090_skybase.lc.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/lua_libraries/bit.lua` & `open-dread-rando-2.3.1/open_dread_rando/files/lua_libraries/bit.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/lua_libraries/data_structures.lua` & `open-dread-rando-2.3.1/open_dread_rando/files/lua_libraries/data_structures.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/lua_libraries/death_counter.lua` & `open-dread-rando-2.3.1/open_dread_rando/files/lua_libraries/death_counter.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/lua_libraries/guilib.lua` & `open-dread-rando-2.3.1/open_dread_rando/files/lua_libraries/guilib.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/lua_libraries/input_handling.lua` & `open-dread-rando-2.3.1/open_dread_rando/files/lua_libraries/input_handling.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/lua_libraries/room_names.lua` & `open-dread-rando-2.3.1/open_dread_rando/files/lua_libraries/room_names.lua`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         ColorG = 0.8773584961891174,
         ColorB = 0.8773584961891174,
     })
 
     local label = container:AddLabel("RoomNameGui_Text", "Room: Unknown", {
         X = "0.0075",
         Y = "0.01",
-        SizeX = "0.2",
+        SizeX = "0.3",
         SizeY = "0.04",
         Font = "digital_small",
         Autosize = false,
     })
 
     RoomNameGui.ui = ui
     RoomNameGui.container = container
```

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/msemenu_mainmenu.lua` & `open-dread-rando-2.3.1/open_dread_rando/files/msemenu_mainmenu.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/randomizer_powerup.lua` & `open-dread-rando-2.3.1/open_dread_rando/files/randomizer_powerup.lua`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,22 @@
 function RandomizerPowerup.MarkLocationCollected(locationIdentifier)
     local playerSection = Game.GetPlayerBlackboardSectionName()
     local propName = RandomizerPowerup.PropertyForLocation(locationIdentifier)
     Game.LogWarn(0, propName)
     Blackboard.SetProp(playerSection, propName, "b", true)
 end
 
+function RandomizerPowerup.IncrementInventoryIndex()
+    local playerSection = Game.GetPlayerBlackboardSectionName()
+    local propName = "InventoryIndex"
+    local currentIndex = Blackboard.GetProp(playerSection, propName) or 0
+    currentIndex = currentIndex + 1
+    Blackboard.SetProp(playerSection, propName, "f", currentIndex)
+end
+
 function RandomizerPowerup.OnPickedUp(actor, resources)
     RandomizerPowerup.Self = actor
     local name = "Boss"
     if actor ~= nil then
         name = actor.sName
         RandomizerPowerup.MarkLocationCollected(string.format("%s_%s", Scenario.CurrentScenarioID, name))
     end
@@ -61,14 +69,15 @@
         RandomizerPowerup.IncreaseAmmo(resource)
 
         RandomizerPowerup.CheckArtifacts(resource)
     end
 
     RandomizerPowerup.ApplyTunableChanges()
     Scenario.UpdateProgressiveItemModels()
+    RandomizerPowerup.IncrementInventoryIndex()
     RL.UpdateRDVClient(false)
     return granted
 end
 
 function RandomizerPowerup.DisableInput()
     -- items with unique inputs (Speed Booster, Phantom Cloak) require disabling and re-enabling inputs to work properly
     local oPlayer = Game.GetPlayer()
```

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_camo.bsmat` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_camo.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_sonr.bsmat` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_sonr.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_camo.bcmdl` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_camo.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_sonr.bcmdl` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_sonr.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__BK.bcmdl` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__BK.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__BL.bcmdl` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__BL.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__CY.bcmdl` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__CY.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__GN.bcmdl` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__GN.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__GY.bcmdl` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__GY.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__MG.bcmdl` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__MG.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__OR.bcmdl` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__OR.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__PK.bcmdl` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__PK.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__PR.bcmdl` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__PR.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__WH.bcmdl` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__WH.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__YL.bcmdl` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__YL.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/itemsphere/models/imats/speedboost_mp_opaque_01.bsmat` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/itemsphere/models/imats/speedboost_mp_opaque_01.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/itemsphere/models/speed_booster.bcmdl` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/itemsphere/models/speed_booster.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphhologram.bsmat` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphhologram.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphmaterial.bsmat` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphmaterial.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/powerup_morph.bcmdl` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/powerup_morph.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_magnet01.bsmat` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_magnet01.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_white__01.bsmat` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_white__01.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/powerup_magnet.bcmdl` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/powerup_magnet.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/powerup_powerbomb_mp_fxhologram_0001.bsmat` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/powerup_powerbomb_mp_fxhologram_0001.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/powerup_powerbomb.bcmdl` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/powerup_powerbomb.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/imats/powerup_ice__missile_mp_opaque_01.bsmat` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/imats/powerup_ice__missile_mp_opaque_01.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/powerup_ice__missile.bcmdl` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/powerup_ice__missile.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_cangrejo.bsmat` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_cangrejo.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/powerup_wavebeam.bcmdl` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/powerup_wavebeam.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/props/doorshieldpowerbomb___/models/doorshieldpowerbomb___.bcmdl` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/props/doorshieldpowerbomb___/models/doorshieldpowerbomb___.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/props/doorshieldpowerbomb___/models/imats/doorshieldpowerbomb____mp_opaque_01.bsmat` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/props/doorshieldpowerbomb___/models/imats/doorshieldpowerbomb____mp_opaque_01.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/imats/shield_diffusion_matfx.bsmat` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/imats/shield_diffusion_matfx.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/imats/shield_diffusion_mp_opaque_01.bsmat` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/imats/shield_diffusion_mp_opaque_01.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/shield_diffusion.bcmdl` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/shield_diffusion.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/props/shield_bombs_regular__/models/imats/shield_bombs_regular___mp_opaque_01.bsmat` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/props/shield_bombs_regular__/models/imats/shield_bombs_regular___mp_opaque_01.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/props/shield_bombs_regular__/models/shield_bombs_regular__.bcmdl` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/props/shield_bombs_regular__/models/shield_bombs_regular__.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/props/shield_cross_bomb_____/models/imats/shield_cross_bomb______mp_opaque_01.bsmat` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/props/shield_cross_bomb_____/models/imats/shield_cross_bomb______mp_opaque_01.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/props/shield_cross_bomb_____/models/shield_cross_bomb_____.bcmdl` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/props/shield_cross_bomb_____/models/shield_cross_bomb_____.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/props/shield_icemissile/models/imats/shield_icemissile_mp_opaque_01.bsmat` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/props/shield_icemissile/models/imats/shield_icemissile_mp_opaque_01.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/props/shield_icemissile/models/shield_icemissile.bcmdl` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/props/shield_icemissile/models/shield_icemissile.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/props/shield_storm_mssl/models/imats/shield_storm_mssl_mp_opaque_01.bsmat` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/props/shield_storm_mssl/models/imats/shield_storm_mssl_mp_opaque_01.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/actors/props/shield_storm_mssl/models/shield_storm_mssl.bcmdl` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/actors/props/shield_storm_mssl/models/shield_storm_mssl.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_at.bctex` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_at.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_bc.bctex` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_nm.bctex` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_nm.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphat.bctex` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphat.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphbc.bctex` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphbc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphnm.bctex` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphnm.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/textures/powerup_spi_magnet_bc.bctex` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/textures/powerup_spi_magnet_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/textures/powerup_ice__missile_bc.bctex` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/textures/powerup_ice__missile_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/textures/pup_wavebeam_bc.bctex` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/textures/pup_wavebeam_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/textures/doorshield_____bomb_bc.bctex` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/textures/doorshield_____bomb_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/textures/doorshieldcrossbomb_bc.bctex` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/textures/doorshieldcrossbomb_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/textures/doorshieldpowerbomb_bc.bctex` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/textures/doorshieldpowerbomb_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/actors/props/shield_storm_mssl/models/textures/shield_storm_mssl_bc.bctex` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/actors/props/shield_storm_mssl/models/textures/shield_storm_mssl_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/romfs/textures/system/minimap/icons/icons.bctex` & `open-dread-rando-2.3.1/open_dread_rando/files/romfs/textures/system/minimap/icons/icons.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/files/schema.json` & `open-dread-rando-2.3.1/open_dread_rando/files/schema.json`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/game_patches.py` & `open-dread-rando-2.3.1/open_dread_rando/game_patches.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/lua_editor.py` & `open-dread-rando-2.3.1/open_dread_rando/lua_editor.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/lua_util.py` & `open-dread-rando-2.3.1/open_dread_rando/lua_util.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/map_icons.py` & `open-dread-rando-2.3.1/open_dread_rando/map_icons.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/missile_color_patcher.py` & `open-dread-rando-2.3.1/open_dread_rando/missile_color_patcher.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/model_data.py` & `open-dread-rando-2.3.1/open_dread_rando/model_data.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/objective.py` & `open-dread-rando-2.3.1/open_dread_rando/objective.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/output_config.py` & `open-dread-rando-2.3.1/open_dread_rando/output_config.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/patch_util.py` & `open-dread-rando-2.3.1/open_dread_rando/patch_util.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/patcher_editor.py` & `open-dread-rando-2.3.1/open_dread_rando/patcher_editor.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/pickup.py` & `open-dread-rando-2.3.1/open_dread_rando/pickup.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/static_fixes.py` & `open-dread-rando-2.3.1/open_dread_rando/static_fixes.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/templates/custom_core_x.lua` & `open-dread-rando-2.3.1/open_dread_rando/templates/custom_core_x.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/templates/custom_core_x_superquetzoa.lua` & `open-dread-rando-2.3.1/open_dread_rando/templates/custom_core_x_superquetzoa.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/templates/custom_init.lua` & `open-dread-rando-2.3.1/open_dread_rando/templates/custom_init.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/templates/template_doorshield_energy_bmsad.json` & `open-dread-rando-2.3.1/open_dread_rando/templates/template_doorshield_energy_bmsad.json`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/templates/template_doorshield_hexs_bmsad.json` & `open-dread-rando-2.3.1/open_dread_rando/templates/template_doorshield_hexs_bmsad.json`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/templates/template_doorshield_tris_bmsad.json` & `open-dread-rando-2.3.1/open_dread_rando/templates/template_doorshield_tris_bmsad.json`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/templates/template_powerup_bmsad.json` & `open-dread-rando-2.3.1/open_dread_rando/templates/template_powerup_bmsad.json`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/text_patches.py` & `open-dread-rando-2.3.1/open_dread_rando/text_patches.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/tilegroup_patcher.py` & `open-dread-rando-2.3.1/open_dread_rando/tilegroup_patcher.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando/validator_with_default.py` & `open-dread-rando-2.3.1/open_dread_rando/validator_with_default.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/open_dread_rando.egg-info/PKG-INFO` & `open-dread-rando-2.3.1/open_dread_rando.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-dread-rando
-Version: 2.3.0
+Version: 2.3.1
 Summary: An open source randomizer patcher for Metroid Dread.
 Home-page: https://github.com/randovania/open-dread-rando
 Author: Henrique Gemignani
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `open-dread-rando-2.3.0/open_dread_rando.egg-info/SOURCES.txt` & `open-dread-rando-2.3.1/open_dread_rando.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/setup.cfg` & `open-dread-rando-2.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/tests/test_dread_patcher.py` & `open-dread-rando-2.3.1/tests/test_dread_patcher.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/tests/test_files/starter_preset_patcher.json` & `open-dread-rando-2.3.1/tests/test_files/starter_preset_patcher.json`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.0/tests/test_lua_util.py` & `open-dread-rando-2.3.1/tests/test_lua_util.py`

 * *Files identical despite different names*

